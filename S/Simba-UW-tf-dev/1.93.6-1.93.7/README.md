# Comparing `tmp/Simba-UW-tf-dev-1.93.6.tar.gz` & `tmp/Simba-UW-tf-dev-1.93.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.93.6.tar", last modified: Mon May 20 17:02:13 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.93.7.tar", last modified: Tue May 21 13:35:55 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.93.6.tar` & `Simba-UW-tf-dev-1.93.7.tar`

### file list

```diff
@@ -1,689 +1,690 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.93.6/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)   144897 2024-05-20 15:03:49.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.6/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.6/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.6/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.6/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.93.6/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.93.6/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-20 14:20:14.000000 Simba-UW-tf-dev-1.93.6/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.93.6/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1173 2024-05-19 16:18:01.000000 Simba-UW-tf-dev-1.93.6/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84123 2024-05-09 15:16:46.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    47980 2024-05-09 16:28:06.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    38682 2024-05-14 17:44:58.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35785 2024-05-09 15:22:35.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   181387 2024-05-17 20:42:23.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   167515 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.6/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26136 2024-05-09 20:56:18.000000 Simba-UW-tf-dev-1.93.6/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.6/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.6/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.93.6/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    56026 2024-05-14 14:03:50.000000 Simba-UW-tf-dev-1.93.6/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    79930 2024-05-16 13:13:35.000000 Simba-UW-tf-dev-1.93.6/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    17895 2024-05-20 16:55:27.000000 Simba-UW-tf-dev-1.93.6/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      448 2024-05-20 14:46:12.000000 Simba-UW-tf-dev-1.93.6/simba/utils/find_fonts.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.93.6/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.93.6/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/CLAHE.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     3869 2024-05-14 18:18:20.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/ffmpeg_progress_bar.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     9124 2024-05-20 13:37:45.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_text.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      549 2024-05-14 19:00:13.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/detect_scene_changes.py
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     4950 2024-05-14 14:14:15.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/watermark.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/img_stack_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/sorensen_dice_coefficient.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2024-05-16 13:12:21.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/clean_sleap_filename.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/downsample_video_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/concordance_ratio.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/segment_image_horizontal.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3838 2024-05-14 11:30:22.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/crossfade.py
--rw-r--r--   0 simon      (501) staff       (20)     3043 2024-05-09 15:04:30.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/shift_geometries.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-05-15 19:11:53.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/convert_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/downsample_multiple_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/mahalanobis.py
--rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/superpixels.py
--rw-r--r--   0 simon      (501) staff       (20)     2225 2024-05-09 20:57:38.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/img_conv.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     3137 2024-05-15 15:22:04.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/blurbox.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_frame_count.py
--rw-r--r--   0 simon      (501) staff       (20)     5433 2024-05-14 15:38:59.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/inset_overlay_video.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/lbp.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/brillouins_index.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/eta_squared.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    16301 2024-05-13 14:59:18.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/convert_to_mp4.py
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     6440 2024-05-09 20:10:17.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/change_img_file_format.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/violin.py
--rw-r--r--   0 simon      (501) staff       (20)    16527 2024-05-17 20:38:47.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/bg_substraction.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fleiss_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    12282 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/convert_to_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/rotate image.py
--rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/jaccard_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)      122 2024-05-15 13:58:53.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/profiler.py
--rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/manhattan_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/path_plots.py
--rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/seekable.py
--rw-r--r--   0 simon      (501) staff       (20)    26677 2024-05-20 14:18:40.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_popups.py
--rw-r--r--   0 simon      (501) staff       (20)     6572 2024-05-15 13:42:29.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_elapsed_time.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/relative_risk.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/contrast.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/youden_j.py
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/color_filtering.py
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/make_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.93.6/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-09 13:03:17.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8987 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)     9549 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.93.6/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.93.6/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.93.6/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.93.6/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.6/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    11039 2024-05-09 16:32:28.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50014 2024-05-17 13:19:01.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    18552 2024-05-09 16:13:09.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29746 2024-05-17 13:17:50.000000 Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13867 2024-05-16 18:24:39.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   202043 2024-05-20 15:03:49.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-15 15:29:21.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-05-14 20:38:00.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/brightness_contrast_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.93.6/simba/video_processors/clahe_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    84226 2024-05-20 14:24:05.000000 Simba-UW-tf-dev-1.93.6/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.93.6/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-19 17:46:48.000000 Simba-UW-tf-dev-1.93.6/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.93.6/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.93.6/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     4267 2024-05-20 14:19:55.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/blur.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/brightness.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.6/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    24724 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)     1078 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-20 17:02:12.000000 Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.93.6/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.93.6/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.93.6/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.93.6/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.93.6/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8582 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.6/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.6/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.93.6/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.93.6/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.6/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-20 17:02:10.000000 Simba-UW-tf-dev-1.93.6/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-20 17:02:13.000000 Simba-UW-tf-dev-1.93.6/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.93.7/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)   144937 2024-05-20 18:02:46.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.7/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.7/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.93.7/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.93.7/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-20 18:01:03.000000 Simba-UW-tf-dev-1.93.7/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.93.7/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1173 2024-05-19 16:18:01.000000 Simba-UW-tf-dev-1.93.7/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84123 2024-05-09 15:16:46.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    47980 2024-05-09 16:28:06.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    38682 2024-05-14 17:44:58.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35785 2024-05-09 15:22:35.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   181387 2024-05-17 20:42:23.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   167515 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.7/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26136 2024-05-09 20:56:18.000000 Simba-UW-tf-dev-1.93.7/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.7/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.7/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.93.7/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    56026 2024-05-14 14:03:50.000000 Simba-UW-tf-dev-1.93.7/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    79930 2024-05-16 13:13:35.000000 Simba-UW-tf-dev-1.93.7/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    17894 2024-05-20 18:02:46.000000 Simba-UW-tf-dev-1.93.7/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      449 2024-05-20 18:02:46.000000 Simba-UW-tf-dev-1.93.7/simba/utils/find_fonts.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.93.7/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.93.7/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/CLAHE.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     3869 2024-05-14 18:18:20.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/ffmpeg_progress_bar.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     9124 2024-05-20 13:37:45.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_text.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      549 2024-05-14 19:00:13.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/detect_scene_changes.py
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     4950 2024-05-14 14:14:15.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/watermark.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/img_stack_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/sorensen_dice_coefficient.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2024-05-16 13:12:21.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/clean_sleap_filename.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/downsample_video_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/concordance_ratio.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/segment_image_horizontal.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3838 2024-05-14 11:30:22.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/crossfade.py
+-rw-r--r--   0 simon      (501) staff       (20)     3043 2024-05-09 15:04:30.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/shift_geometries.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-05-15 19:11:53.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/convert_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/downsample_multiple_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/mahalanobis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/superpixels.py
+-rw-r--r--   0 simon      (501) staff       (20)     2225 2024-05-09 20:57:38.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/img_conv.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     3137 2024-05-15 15:22:04.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/blurbox.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_frame_count.py
+-rw-r--r--   0 simon      (501) staff       (20)     5433 2024-05-14 15:38:59.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/inset_overlay_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/lbp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/brillouins_index.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/eta_squared.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    16301 2024-05-13 14:59:18.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/convert_to_mp4.py
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     6440 2024-05-09 20:10:17.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/change_img_file_format.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/violin.py
+-rw-r--r--   0 simon      (501) staff       (20)     5465 2024-05-20 20:01:42.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/bg_remover_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    16527 2024-05-17 20:38:47.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/bg_substraction.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fleiss_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    12282 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/convert_to_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/rotate image.py
+-rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/jaccard_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)      122 2024-05-15 13:58:53.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/profiler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/manhattan_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/path_plots.py
+-rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/seekable.py
+-rw-r--r--   0 simon      (501) staff       (20)    26677 2024-05-20 14:18:40.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_popups.py
+-rw-r--r--   0 simon      (501) staff       (20)     6572 2024-05-15 13:42:29.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_elapsed_time.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/relative_risk.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/contrast.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/youden_j.py
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/color_filtering.py
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.93.7/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    23558 2024-05-21 13:05:48.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-09 13:03:17.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8987 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    17579 2024-05-21 13:05:48.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9549 2024-05-09 16:36:03.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.93.7/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.93.7/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.93.7/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.93.7/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.93.7/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    11039 2024-05-09 16:32:28.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50014 2024-05-17 13:19:01.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18552 2024-05-09 16:13:09.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29746 2024-05-17 13:17:50.000000 Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13867 2024-05-16 18:24:39.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   202038 2024-05-20 18:02:46.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-05-15 15:29:21.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-05-14 20:38:00.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/brightness_contrast_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.93.7/simba/video_processors/clahe_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    84230 2024-05-20 17:03:19.000000 Simba-UW-tf-dev-1.93.7/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.93.7/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-20 17:43:48.000000 Simba-UW-tf-dev-1.93.7/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.93.7/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     4267 2024-05-20 14:19:55.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/blur.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/brightness.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.93.7/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    24758 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)     1078 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-21 13:35:54.000000 Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.93.7/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.93.7/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.93.7/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.93.7/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.93.7/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8582 2024-05-12 17:13:08.000000 Simba-UW-tf-dev-1.93.7/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.93.7/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.93.7/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.93.7/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.93.7/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-21 13:35:52.000000 Simba-UW-tf-dev-1.93.7/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-21 13:35:55.000000 Simba-UW-tf-dev-1.93.7/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.93.6/PKG-INFO` & `Simba-UW-tf-dev-1.93.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.93.6
+Version: 1.93.7
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 __author__ = "Simon Nilsson"
 
 import glob
 import os
 import subprocess
 import sys
 import threading
-import numpy as np
 from datetime import datetime
 from tkinter import *
 from typing import Optional, Union
 
+import numpy as np
 from PIL import Image, ImageTk
 
 import simba
 from simba.labelling.extract_labelled_frames import AnnotationFrameExtractor
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.plotting.frame_mergerer_ffmpeg import FrameMergererFFmpeg
@@ -22,15 +22,16 @@
                                         FileSelect, FolderSelect)
 from simba.utils.checks import (check_ffmpeg_available,
                                 check_file_exist_and_readable,
                                 check_if_dir_exists,
                                 check_if_filepath_list_is_empty,
                                 check_if_string_value_is_valid_video_timestamp,
                                 check_int, check_nvidea_gpu_available,
-                                check_that_hhmmss_start_is_before_end, check_str)
+                                check_str,
+                                check_that_hhmmss_start_is_before_end)
 from simba.utils.data import convert_roi_definitions
 from simba.utils.enums import Dtypes, Formats, Keys, Links, Options, Paths
 from simba.utils.errors import (CountError, FrameRangeError, InvalidInputError,
                                 MixedMosaicError, NoChoosenClassifierError,
                                 NoFilesFoundError, NotDirectoryError)
 from simba.utils.lookups import get_color_dict, get_fonts
 from simba.utils.printing import SimbaTimer, stdout_success
@@ -54,16 +55,18 @@
     convert_to_webm, convert_to_webp,
     convert_video_powerpoint_compatible_format, copy_img_folder,
     crop_multiple_videos, crop_multiple_videos_circles,
     crop_multiple_videos_polygons, crop_single_video, crop_single_video_circle,
     crop_single_video_polygon, downsample_video, extract_frame_range,
     extract_frames_single_video, frames_to_movie, gif_creator,
     multi_split_video, remove_beginning_of_video, resize_videos_by_height,
-    resize_videos_by_width, superimpose_frame_count, video_concatenator,
-    video_to_greyscale, watermark_video, superimpose_video_progressbar, superimpose_elapsed_time, superimpose_overlay_video, superimpose_video_names, superimpose_freetext, roi_blurbox)
+    resize_videos_by_width, roi_blurbox, superimpose_elapsed_time,
+    superimpose_frame_count, superimpose_freetext, superimpose_overlay_video,
+    superimpose_video_names, superimpose_video_progressbar, video_concatenator,
+    video_to_greyscale, watermark_video)
 
 sys.setrecursionlimit(10**7)
 
 
 class CLAHEPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title="CLAHE VIDEO CONVERSION")
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.93.7/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.93.7/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.93.7/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.93.7/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.93.7/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.93.7/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.93.7/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.93.7/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
 000013f0: 4462 6c6f 6200 0000 08e4 2b79 2913 eec5  Dblob.....+y)...
 00001400: 4100 0000 1b00 7400 6800 6900 7200 6400  A.....t.h.i.r.d.
 00001410: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
 00001420: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
 00001430: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
 00001440: 6f6d 7000 0000 0000 0440 0000 0000 0200  omp......@......
 00001450: 7500 696c 6731 5363 6f6d 7000 0000 0000  u.ilg1Scomp.....
-00001460: 0e78 3600 0000 0200 7500 696d 6f44 4462  .x6.....u.imoDDb
+00001460: 0e84 c500 0000 0200 7500 696d 6f44 4462  ........u.imoDDb
 00001470: 6c6f 6200 0000 0874 394b 535b e7c5 4100  lob....t9KS[..A.
 00001480: 0000 0200 7500 696d 6f64 4462 6c6f 6200  ....u.imodDblob.
 00001490: 0000 0874 394b 535b e7c5 4100 0000 0200  ...t9KS[..A.....
 000014a0: 7500 6970 6831 5363 6f6d 7000 0000 0000  u.iph1Scomp.....
 000014b0: 1230 0000 0000 0c00 7500 6e00 7300 7500  .0......u.n.s.u.
 000014c0: 7000 6500 7200 7600 6900 7300 6500 6462  p.e.r.v.i.s.e.db
 000014d0: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
@@ -459,21 +459,21 @@
 00001ca0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00001cb0: 6261 7208 0908 095f 1018 7b7b 3135 312c  bar...._..{{151,
 00001cc0: 2039 367d 2c20 7b31 3138 302c 2035 3638   96}, {1180, 568
 00001cd0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 00001ce0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 00001cf0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001d00: 0000 0005 0075 0074 0069 006c 0073 6c67  .....u.t.i.l.slg
-00001d10: 3153 636f 6d70 0000 0000 0008 38bd 0000  1Scomp......8...
+00001d10: 3153 636f 6d70 0000 0000 0008 40f8 0000  1Scomp......@...
 00001d20: 0005 0075 0074 0069 006c 0073 6d6f 4444  ...u.t.i.l.smoDD
-00001d30: 626c 6f62 0000 0008 ab4e e1ff 1efb c541  blob.....N.....A
+00001d30: 626c 6f62 0000 0008 d859 d1ff dbfd c541  blob.....Y.....A
 00001d40: 0000 0005 0075 0074 0069 006c 0073 6d6f  .....u.t.i.l.smo
-00001d50: 6444 626c 6f62 0000 0008 ab4e e1ff 1efb  dDblob.....N....
+00001d50: 6444 626c 6f62 0000 0008 d859 d1ff dbfd  dDblob.....Y....
 00001d60: c541 0000 0005 0075 0074 0069 006c 0073  .A.....u.t.i.l.s
-00001d70: 7068 3153 636f 6d70 0000 0000 0009 4000  ph1Scomp......@.
+00001d70: 7068 3153 636f 6d70 0000 0000 0009 5000  ph1Scomp......P.
 00001d80: 0000 0005 0075 0074 0069 006c 0073 7653  .....u.t.i.l.svS
 00001d90: 726e 6c6f 6e67 0000 0001 0000 0010 0076  rnlong.........v
 00001da0: 0069 0064 0065 006f 005f 0070 0072 006f  .i.d.e.o._.p.r.o
 00001db0: 0063 0065 0073 0073 006f 0072 0073 6277  .c.e.s.s.o.r.sbw
 00001dc0: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
 00001dd0: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00001de0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
@@ -485,18 +485,18 @@
 00001e40: 392c 2033 3030 7d2c 207b 3932 302c 2034  9, 300}, {920, 4
 00001e50: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
 00001e60: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
 00001e70: 000d 0000 0000 0000 0000 0000 0000 0000  ................
 00001e80: 008b 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
 00001e90: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00001ea0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00001eb0: 0000 0008 39d4 0000 0010 0076 0069 0064  ....9......v.i.d
+00001eb0: 0000 0008 3d34 0000 0010 0076 0069 0064  ....=4.....v.i.d
 00001ec0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00001ed0: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
-00001ee0: 6f62 0000 0008 818d 2d0f c9fd c541 0000  ob......-....A..
+00001ee0: 6f62 0000 0008 6da5 6aae e3fd c541 0000  ob....m.j....A..
 00001ef0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00001f00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
 00001f10: 0073 6d6f 6444 626c 6f62 0000 0008 818d  .smodDblob......
 00001f20: 2d0f c9fd c541 0000 0010 0076 0069 0064  -....A.....v.i.d
 00001f30: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00001f40: 0073 0073 006f 0072 0073 7068 3153 636f  .s.s.o.r.sph1Sco
 00001f50: 6d70 0000 0000 0009 2000 0000 0010 0076  mp...... ......v
@@ -509,18 +509,18 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 002f 0000 000b  .........../....
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0000 e8f5 0000 000b 005f 005f 0070  ..........._._.p
+00002030: 0000 0000 e94b 0000 000b 005f 005f 0070  .....K....._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 0d7a de28  moDDblob.....z.(
-00002060: c7fd c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 cd04 c725  moDDblob.......%
+00002060: dffd c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 0d7a de28 c7fd  dDblob.....z.(..
 00002090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 0001 0000 0000 0006  comp............
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
 000020d0: 626c 6f62 0000 00b7 6270 6c69 7374 3030  blob....bplist00
@@ -532,22 +532,22 @@
 00002130: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00002140: 6261 7208 0908 095f 1017 7b7b 302c 2031  bar...._..{{0, 1
 00002150: 3236 7d2c 207b 3134 3430 2c20 3633 357d  26}, {1440, 635}
 00002160: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8900  }...#/;R_klmno..
 00002170: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
 00002180: 0000 0000 0000 0000 0000 0000 0000 8a00  ................
 00002190: 0000 0600 6100 7300 7300 6500 7400 736c  ....a.s.s.e.t.sl
-000021a0: 6731 5363 6f6d 7000 0000 0000 8a16 9400  g1Scomp.........
+000021a0: 6731 5363 6f6d 7000 0000 0000 8a27 3f00  g1Scomp......'?.
 000021b0: 0000 0600 6100 7300 7300 6500 7400 736d  ....a.s.s.e.t.sm
 000021c0: 6f44 4462 6c6f 6200 0000 08ee 1690 c8ab  oDDblob.........
 000021d0: bac5 4100 0000 0600 6100 7300 7300 6500  ..A.....a.s.s.e.
 000021e0: 7400 736d 6f64 4462 6c6f 6200 0000 08ee  t.smodDblob.....
 000021f0: 1690 c8ab bac5 4100 0000 0600 6100 7300  ......A.....a.s.
 00002200: 7300 6500 7400 7370 6831 5363 6f6d 7000  s.e.t.sph1Scomp.
-00002210: 0000 0000 8df0 0000 0000 0600 6100 7300  ............a.s.
+00002210: 0000 0000 8e10 0000 0000 0600 6100 7300  ............a.s.
 00002220: 7300 6500 7400 7376 5372 6e6c 6f6e 6700  s.e.t.svSrnlong.
 00002230: 0000 0100 0000 1200 6200 6f00 7500 6e00  ........b.o.u.n.
 00002240: 6400 6900 6e00 6700 5f00 6200 6f00 7800  d.i.n.g._.b.o.x.
 00002250: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
 00002260: 6f6d 7000 0000 0000 0322 2b00 0000 1200  omp......"+.....
 00002270: 6200 6f00 7500 6e00 6400 6900 6e00 6700  b.o.u.n.d.i.n.g.
 00002280: 5f00 6200 6f00 7800 5f00 7400 6f00 6f00  _.b.o.x._.t.o.o.
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.93.7/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/requirements.txt` & `Simba-UW-tf-dev-1.93.7/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.93.7/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.93.7/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/enums.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/checks.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/lookups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 __author__ = "Simon Nilsson"
 
 import glob
 import os
+import platform
 import re
 import struct
 import sys
-from pathlib import Path
-import platform
 from multiprocessing import Lock, Process, Value
+from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
+import matplotlib.font_manager
 import pandas as pd
 from matplotlib import cm
-import  matplotlib.font_manager
 
 import simba
 from simba.utils.checks import (check_file_exist_and_readable,
                                 check_if_dir_exists)
-from simba.utils.enums import Methods, Paths, OS
+from simba.utils.enums import OS, Methods, Paths
 from simba.utils.read_write import get_fn_ext
 from simba.utils.warnings import NoDataFoundWarning
 
 
 class SharedCounter(object):
     """Counter that can be shared across processes on different cores"""
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/errors.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/data.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/utils/printing.py` & `Simba-UW-tf-dev-1.93.7/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.93.7/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/CLAHE.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/CLAHE.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/ffmpeg_progress_bar.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/ffmpeg_progress_bar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_text.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_text.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/detect_scene_changes.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/detect_scene_changes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/watermark.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/watermark.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/img_stack_to_bw.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/img_stack_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/sorensen_dice_coefficient.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/clean_sleap_filename.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/clean_sleap_filename.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/ez_path_plot.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/downsample_video_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/downsample_video_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/concordance_ratio.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/concordance_ratio.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/ROI_analyzer.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/segment_image_horizontal.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/segment_image_horizontal.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/crossfade.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/crossfade.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/shift_geometries.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/shift_geometries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/convert_to_bw.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/convert_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/downsample_multiple_videos_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/downsample_multiple_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/mahalanobis.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/mahalanobis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/superpixels.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/superpixels.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/img_conv.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/img_conv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/blurbox.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/blurbox.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_frame_count.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_frame_count.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/inset_overlay_video.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/inset_overlay_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/brillouins_index.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/brillouins_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/eta_squared.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/eta_squared.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/convert_to_mp4.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/convert_to_mp4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/change_img_file_format.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/change_img_file_format.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/violin.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/violin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/bg_substraction.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/bg_substraction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fleiss_kappa.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/convert_to_popup.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/convert_to_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/rotate image.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/rotate image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/jaccard_distance.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/jaccard_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/manhattan_distance.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/ROI_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/path_plots.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/path_plots.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/seekable.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/seekable.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_popups.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_popups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/superimpose_elapsed_time.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/superimpose_elapsed_time.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/relative_risk.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/relative_risk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/contrast.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/contrast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/youden_j.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/youden_j.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/make_path_plot.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/make_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.93.7/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,20 +189,21 @@
         self.video_meta_data = get_video_meta_data(self.video_path)
         self.temp_folder = os.path.join(self.out_parent_dir, self.video_name, "temp")
         if os.path.exists(self.temp_folder):
             shutil.rmtree(self.temp_folder)
         os.makedirs(self.temp_folder)
 
     def __insert_data(self):
-        roi_entries_dict = self.roi_entries_df[["ANIMAL", "SHAPE NAME", "START FRAME", "END FRAME"]].to_dict(orient="records")
-        for entry_dict in roi_entries_dict:
-            entry, exit = int(entry_dict["START FRAME"]), int(entry_dict["END FRAME"])
-            entry_dict["frame_range"] = list(range(entry, exit + 1))
-            col_name =  f'{entry_dict["ANIMAL"]}_{entry_dict["SHAPE NAME"]}'
-            self.data_df[col_name][self.data_df.index.isin(entry_dict["frame_range"])] = 1
+        if self.roi_entries_df is not None:
+            roi_entries_dict = self.roi_entries_df[["ANIMAL", "SHAPE NAME", "START FRAME", "END FRAME"]].to_dict(orient="records")
+            for entry_dict in roi_entries_dict:
+                entry, exit = int(entry_dict["START FRAME"]), int(entry_dict["END FRAME"])
+                entry_dict["frame_range"] = list(range(entry, exit + 1))
+                col_name =  f'{entry_dict["ANIMAL"]}_{entry_dict["SHAPE NAME"]}'
+                self.data_df[col_name][self.data_df.index.isin(entry_dict["frame_range"])] = 1
 
     def __calc_text_locs(self) -> dict:
         loc_dict = {}
         line_spacer = TextOptions.FIRST_LINE_SPACING.value
         for animal_cnt, animal_name in enumerate(self.animal_names):
             loc_dict[animal_name] = {}
             for shape in self.shape_names:
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/ez_path_plot.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/ROI_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,20 +102,21 @@
         self.__insert_data()
         self.video_path = video_path
         self.cap = cv2.VideoCapture(self.video_path)
         self.video_meta_data = get_video_meta_data(self.video_path)
         self.threshold, self.body_parts = threshold, body_parts
 
     def __insert_data(self):
-        roi_entries_dict = self.roi_entries_df[["ANIMAL", "SHAPE NAME", "START FRAME", "END FRAME"]].to_dict(orient="records")
-        for entry_dict in roi_entries_dict:
-            entry, exit = int(entry_dict["START FRAME"]), int(entry_dict["END FRAME"])
-            entry_dict["frame_range"] = list(range(entry, exit + 1))
-            col_name =  f'{entry_dict["ANIMAL"]}_{entry_dict["SHAPE NAME"]}'
-            self.data_df[col_name][self.data_df.index.isin(entry_dict["frame_range"])] = 1
+        if self.roi_entries_df is not None:
+            roi_entries_dict = self.roi_entries_df[["ANIMAL", "SHAPE NAME", "START FRAME", "END FRAME"]].to_dict(orient="records")
+            for entry_dict in roi_entries_dict:
+                entry, exit = int(entry_dict["START FRAME"]), int(entry_dict["END FRAME"])
+                entry_dict["frame_range"] = list(range(entry, exit + 1))
+                col_name =  f'{entry_dict["ANIMAL"]}_{entry_dict["SHAPE NAME"]}'
+                self.data_df[col_name][self.data_df.index.isin(entry_dict["frame_range"])] = 1
 
     def __calc_text_locs(self) -> dict:
         loc_dict = {}
         line_spacer = TextOptions.FIRST_LINE_SPACING.value
         for animal_cnt, animal_name in enumerate(self.animal_names):
             loc_dict[animal_name] = {}
             for shape in self.shape_names:
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.93.7/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.93.7/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.93.7/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.93.7/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.93.7/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.93.7/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.93.7/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.93.7/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.93.7/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.93.7/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.93.7/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.93.7/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.93.7/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.93.7/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.93.7/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/video_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,20 +106,20 @@
 00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000006a0: 2020 204e 6f46 696c 6573 466f 756e 6445     NoFilesFoundE
 000006b0: 7272 6f72 2c20 4e6f 7444 6972 6563 746f  rror, NotDirecto
 000006c0: 7279 4572 726f 7229 0a66 726f 6d20 7369  ryError).from si
 000006d0: 6d62 612e 7574 696c 732e 6c6f 6f6b 7570  mba.utils.lookup
 000006e0: 7320 696d 706f 7274 2028 6765 745f 6666  s import (get_ff
 000006f0: 6d70 6567 5f63 726f 7373 6661 6465 5f6d  mpeg_crossfade_m
-00000700: 6574 686f 6473 2c0a 2020 2020 2020 2020  ethods,.        
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 2020 2020 2070 6572 6365 6e74           percent
-00000730: 5f74 6f5f 6372 665f 6c6f 6f6b 7570 2c20  _to_crf_lookup, 
-00000740: 7065 7263 656e 745f 746f 5f71 765f 6c6b  percent_to_qv_lk
-00000750: 2c20 6765 745f 666f 6e74 7329 0a66 726f  , get_fonts).fro
+00000700: 6574 686f 6473 2c20 6765 745f 666f 6e74  ethods, get_font
+00000710: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000730: 2020 2020 7065 7263 656e 745f 746f 5f63      percent_to_c
+00000740: 7266 5f6c 6f6f 6b75 702c 2070 6572 6365  rf_lookup, perce
+00000750: 6e74 5f74 6f5f 7176 5f6c 6b29 0a66 726f  nt_to_qv_lk).fro
 00000760: 6d20 7369 6d62 612e 7574 696c 732e 7072  m simba.utils.pr
 00000770: 696e 7469 6e67 2069 6d70 6f72 7420 5369  inting import Si
 00000780: 6d62 6154 696d 6572 2c20 7374 646f 7574  mbaTimer, stdout
 00000790: 5f73 7563 6365 7373 0a66 726f 6d20 7369  _success.from si
 000007a0: 6d62 612e 7574 696c 732e 7265 6164 5f77  mba.utils.read_w
 000007b0: 7269 7465 2069 6d70 6f72 7420 280a 2020  rite import (.  
 000007c0: 2020 6368 6563 6b5f 6966 5f68 686d 6d73    check_if_hhmms
@@ -11827,802 +11827,802 @@
 0002e320: 7365 7320 7468 6520 7669 6465 6f20 6e61  ses the video na
 0002e330: 6d65 206f 6e20 7468 6520 6769 7665 6e20  me on the given 
 0002e340: 7669 6465 6f20 6669 6c65 2873 2920 616e  video file(s) an
 0002e350: 6420 7361 7665 7320 7468 6520 6d6f 6469  d saves the modi
 0002e360: 6669 6564 2076 6964 656f 2873 292e 0a0a  fied video(s)...
 0002e370: 2020 2020 2e2e 2076 6964 656f 3a3a 205f      .. video:: _
 0002e380: 7374 6174 6963 2f69 6d67 2f73 7570 6572  static/img/super
-0002e390: 696d 706f 7365 5f65 6c61 7073 6564 5f74  impose_elapsed_t
-0002e3a0: 696d 652e 7765 626d 0a20 2020 2020 2020  ime.webm.       
-0002e3b0: 3a77 6964 7468 3a20 3930 300a 2020 2020  :width: 900.    
-0002e3c0: 2020 203a 6c6f 6f70 3a0a 0a20 2020 203a     :loop:..    :
-0002e3d0: 7061 7261 6d20 556e 696f 6e5b 7374 722c  param Union[str,
-0002e3e0: 206f 732e 5061 7468 4c69 6b65 5d20 7669   os.PathLike] vi
-0002e3f0: 6465 6f5f 7061 7468 3a20 5061 7468 2074  deo_path: Path t
-0002e400: 6f20 7468 6520 696e 7075 7420 7669 6465  o the input vide
-0002e410: 6f20 6669 6c65 206f 7220 6469 7265 6374  o file or direct
-0002e420: 6f72 7920 636f 6e74 6169 6e69 6e67 2076  ory containing v
-0002e430: 6964 656f 2066 696c 6573 2e0a 2020 2020  ideo files..    
-0002e440: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-0002e450: 696e 745d 2066 6f6e 745f 7369 7a65 3a20  int] font_size: 
-0002e460: 466f 6e74 2073 697a 6520 666f 7220 7468  Font size for th
-0002e470: 6520 7669 6465 6f20 6e61 6d65 2074 6578  e video name tex
-0002e480: 742e 2044 6566 6175 6c74 2033 302e 0a20  t. Default 30.. 
-0002e490: 2020 203a 7061 7261 6d20 4f70 7469 6f6e     :param Option
-0002e4a0: 616c 5b73 7472 5d20 666f 6e74 5f63 6f6c  al[str] font_col
-0002e4b0: 6f72 3a20 2046 6f6e 7420 636f 6c6f 7220  or:  Font color 
-0002e4c0: 666f 7220 7468 6520 7669 6465 6f20 6e61  for the video na
-0002e4d0: 6d65 2074 6578 742e 2044 6566 6175 6c74  me text. Default
-0002e4e0: 2077 6869 7465 0a20 2020 203a 7061 7261   white.    :para
-0002e4f0: 6d20 4f70 7469 6f6e 616c 5b73 7472 5d20  m Optional[str] 
-0002e500: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
-0002e510: 723a 2046 6f6e 7420 626f 7264 6572 2063  r: Font border c
-0002e520: 6f6c 6f72 2066 6f72 2074 6865 2076 6964  olor for the vid
-0002e530: 656f 206e 616d 6520 7465 7874 2e20 4465  eo name text. De
-0002e540: 6661 756c 7420 626c 6163 6b2e 0a20 2020  fault black..   
-0002e550: 203a 7061 7261 6d20 4f70 7469 6f6e 616c   :param Optional
-0002e560: 5b69 6e74 5d20 666f 6e74 5f62 6f72 6465  [int] font_borde
-0002e570: 725f 7769 6474 683a 2046 6f6e 7420 626f  r_width: Font bo
-0002e580: 7264 6572 2077 6964 7468 2066 6f72 2074  rder width for t
-0002e590: 6865 2076 6964 656f 206e 616d 6520 7465  he video name te
-0002e5a0: 7874 2069 6e20 7069 7865 6c73 2e20 4465  xt in pixels. De
-0002e5b0: 6661 756c 7420 322e 0a20 2020 203a 7061  fault 2..    :pa
-0002e5c0: 7261 6d20 4f70 7469 6f6e 616c 5b4c 6974  ram Optional[Lit
-0002e5d0: 6572 616c 5b27 746f 705f 6c65 6674 272c  eral['top_left',
-0002e5e0: 2027 746f 705f 7269 6768 7427 2c20 2762   'top_right', 'b
-0002e5f0: 6f74 746f 6d5f 6c65 6674 272c 2027 626f  ottom_left', 'bo
-0002e600: 7474 6f6d 5f72 6967 6874 272c 2027 746f  ttom_right', 'to
-0002e610: 705f 6d69 6464 6c65 272c 2027 626f 7474  p_middle', 'bott
-0002e620: 6f6d 5f6d 6964 646c 6527 5d5d 2070 6f73  om_middle']] pos
-0002e630: 6974 696f 6e3a 2050 6f73 6974 696f 6e20  ition: Position 
-0002e640: 7768 6572 6520 7468 6520 7669 6465 6f20  where the video 
-0002e650: 6e61 6d65 2077 696c 6c20 6265 2073 7570  name will be sup
-0002e660: 6572 696d 706f 7365 642e 2044 6566 6175  erimposed. Defau
-0002e670: 6c74 2060 6074 6f70 5f6c 6566 7460 602e  lt ``top_left``.
-0002e680: 0a20 2020 203a 7061 7261 6d20 4f70 7469  .    :param Opti
-0002e690: 6f6e 616c 5b55 6e69 6f6e 5b73 7472 2c20  onal[Union[str, 
-0002e6a0: 6f73 2e50 6174 684c 696b 655d 5d20 7361  os.PathLike]] sa
-0002e6b0: 7665 5f64 6972 3a20 4469 7265 6374 6f72  ve_dir: Director
-0002e6c0: 7920 7768 6572 6520 7468 6520 6d6f 6469  y where the modi
-0002e6d0: 6669 6564 2076 6964 656f 2873 2920 7769  fied video(s) wi
-0002e6e0: 6c6c 2062 6520 7361 7665 642e 2049 6620  ll be saved. If 
-0002e6f0: 6e6f 7420 7072 6f76 6964 6564 2c20 7468  not provided, th
-0002e700: 6520 6469 7265 6374 6f72 7920 6f66 2074  e directory of t
-0002e710: 6865 2069 6e70 7574 2076 6964 656f 2873  he input video(s
-0002e720: 2920 7769 6c6c 2062 6520 7573 6564 2e0a  ) will be used..
-0002e730: 2020 2020 3a72 6574 7572 6e3a 204e 6f6e      :return: Non
-0002e740: 650a 0a20 2020 203a 6578 616d 706c 653a  e..    :example:
-0002e750: 0a20 2020 203e 3e3e 2073 7570 6572 696d  .    >>> superim
-0002e760: 706f 7365 5f76 6964 656f 5f6e 616d 6573  pose_video_names
-0002e770: 2876 6964 656f 5f70 6174 683d 272f 5573  (video_path='/Us
-0002e780: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-0002e790: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-0002e7a0: 7562 6c65 7368 6f6f 7469 6e67 2f6d 6f75  ubleshooting/mou
-0002e7b0: 7365 5f6f 7065 6e5f 6669 656c 642f 7072  se_open_field/pr
-0002e7c0: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
-0002e7d0: 656f 732f 7465 7374 5f34 2f31 2e6d 7034  eos/test_4/1.mp4
-0002e7e0: 272c 2070 6f73 6974 696f 6e3d 276d 6964  ', position='mid
-0002e7f0: 646c 655f 746f 7027 2c20 666f 6e74 5f63  dle_top', font_c
-0002e800: 6f6c 6f72 3d27 626c 6163 6b27 2c20 666f  olor='black', fo
-0002e810: 6e74 5f62 6f72 6465 725f 636f 6c6f 723d  nt_border_color=
-0002e820: 2770 696e 6b27 2c20 666f 6e74 5f62 6f72  'pink', font_bor
-0002e830: 6465 725f 7769 6474 683d 352c 2066 6f6e  der_width=5, fon
-0002e840: 745f 7369 7a65 3d33 3029 0a20 2020 2022  t_size=30).    "
-0002e850: 2222 0a0a 2020 2020 6368 6563 6b5f 6666  ""..    check_ff
-0002e860: 6d70 6567 5f61 7661 696c 6162 6c65 2872  mpeg_available(r
-0002e870: 6169 7365 5f65 7272 6f72 3d54 7275 6529  aise_error=True)
-0002e880: 0a20 2020 2074 696d 6572 203d 2053 696d  .    timer = Sim
-0002e890: 6261 5469 6d65 7228 7374 6172 743d 5472  baTimer(start=Tr
-0002e8a0: 7565 290a 2020 2020 504f 5349 5449 4f4e  ue).    POSITION
-0002e8b0: 5320 3d20 5b27 746f 705f 6c65 6674 272c  S = ['top_left',
-0002e8c0: 2027 746f 705f 7269 6768 7427 2c20 2762   'top_right', 'b
-0002e8d0: 6f74 746f 6d5f 6c65 6674 272c 2027 626f  ottom_left', 'bo
-0002e8e0: 7474 6f6d 5f72 6967 6874 272c 2027 746f  ttom_right', 'to
-0002e8f0: 705f 6d69 6464 6c65 272c 2027 626f 7474  p_middle', 'bott
-0002e900: 6f6d 5f6d 6964 646c 6527 5d0a 2020 2020  om_middle'].    
-0002e910: 6368 6563 6b5f 7374 7228 6e61 6d65 3d66  check_str(name=f
-0002e920: 277b 7375 7065 7269 6d70 6f73 655f 7669  '{superimpose_vi
-0002e930: 6465 6f5f 6e61 6d65 732e 5f5f 6e61 6d65  deo_names.__name
-0002e940: 5f5f 7d20 706f 7369 7469 6f6e 272c 2076  __} position', v
-0002e950: 616c 7565 3d70 6f73 6974 696f 6e2c 206f  alue=position, o
-0002e960: 7074 696f 6e73 3d50 4f53 4954 494f 4e53  ptions=POSITIONS
-0002e970: 290a 2020 2020 6368 6563 6b5f 696e 7428  ).    check_int(
-0002e980: 6e61 6d65 3d66 277b 7375 7065 7269 6d70  name=f'{superimp
-0002e990: 6f73 655f 7669 6465 6f5f 6e61 6d65 732e  ose_video_names.
-0002e9a0: 5f5f 6e61 6d65 5f5f 7d20 666f 6e74 5f73  __name__} font_s
-0002e9b0: 697a 6527 2c20 7661 6c75 653d 666f 6e74  ize', value=font
-0002e9c0: 5f73 697a 652c 206d 696e 5f76 616c 7565  _size, min_value
-0002e9d0: 3d31 290a 2020 2020 6368 6563 6b5f 696e  =1).    check_in
-0002e9e0: 7428 6e61 6d65 3d66 277b 7375 7065 7269  t(name=f'{superi
-0002e9f0: 6d70 6f73 655f 7669 6465 6f5f 6e61 6d65  mpose_video_name
-0002ea00: 732e 5f5f 6e61 6d65 5f5f 7d20 666f 6e74  s.__name__} font
-0002ea10: 5f62 6f72 6465 725f 7769 6474 6827 2c20  _border_width', 
-0002ea20: 7661 6c75 653d 666f 6e74 5f62 6f72 6465  value=font_borde
-0002ea30: 725f 7769 6474 682c 206d 696e 5f76 616c  r_width, min_val
-0002ea40: 7565 3d31 290a 2020 2020 666f 6e74 5f64  ue=1).    font_d
-0002ea50: 6963 7420 3d20 6765 745f 666f 6e74 7328  ict = get_fonts(
-0002ea60: 290a 2020 2020 6368 6563 6b5f 7374 7228  ).    check_str(
-0002ea70: 6e61 6d65 3d27 666f 6e74 272c 2076 616c  name='font', val
-0002ea80: 7565 3d66 6f6e 742c 206f 7074 696f 6e73  ue=font, options
-0002ea90: 3d74 7570 6c65 2866 6f6e 745f 6469 6374  =tuple(font_dict
-0002eaa0: 2e6b 6579 7328 2929 290a 2020 2020 666f  .keys())).    fo
-0002eab0: 6e74 5f70 6174 6820 3d20 666f 6e74 5f64  nt_path = font_d
-0002eac0: 6963 745b 666f 6e74 5d0a 2020 2020 666f  ict[font].    fo
-0002ead0: 6e74 5f63 6f6c 6f72 203d 2027 272e 6a6f  nt_color = ''.jo
-0002eae0: 696e 2866 696c 7465 7228 7374 722e 6973  in(filter(str.is
-0002eaf0: 616c 6e75 6d2c 2066 6f6e 745f 636f 6c6f  alnum, font_colo
-0002eb00: 7229 292e 6c6f 7765 7228 290a 2020 2020  r)).lower().    
-0002eb10: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
-0002eb20: 7220 3d20 2727 2e6a 6f69 6e28 6669 6c74  r = ''.join(filt
-0002eb30: 6572 2873 7472 2e69 7361 6c6e 756d 2c20  er(str.isalnum, 
-0002eb40: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
-0002eb50: 7229 292e 6c6f 7765 7228 290a 2020 2020  r)).lower().    
-0002eb60: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
-0002eb70: 6528 7669 6465 6f5f 7061 7468 293a 0a20  e(video_path):. 
-0002eb80: 2020 2020 2020 2076 6964 656f 5f70 6174         video_pat
-0002eb90: 6873 203d 205b 7669 6465 6f5f 7061 7468  hs = [video_path
-0002eba0: 5d0a 2020 2020 656c 6966 206f 732e 7061  ].    elif os.pa
-0002ebb0: 7468 2e69 7364 6972 2876 6964 656f 5f70  th.isdir(video_p
-0002ebc0: 6174 6829 3a0a 2020 2020 2020 2020 7669  ath):.        vi
-0002ebd0: 6465 6f5f 7061 7468 7320 3d20 6c69 7374  deo_paths = list
-0002ebe0: 2866 696e 645f 616c 6c5f 7669 6465 6f73  (find_all_videos
-0002ebf0: 5f69 6e5f 6469 7265 6374 6f72 7928 6469  _in_directory(di
-0002ec00: 7265 6374 6f72 793d 7669 6465 6f5f 7061  rectory=video_pa
-0002ec10: 7468 2c20 6173 5f64 6963 743d 5472 7565  th, as_dict=True
-0002ec20: 2c20 7261 6973 655f 6572 726f 723d 5472  , raise_error=Tr
-0002ec30: 7565 292e 7661 6c75 6573 2829 290a 2020  ue).values()).  
-0002ec40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0002ec50: 7261 6973 6520 496e 7661 6c69 6449 6e70  raise InvalidInp
-0002ec60: 7574 4572 726f 7228 6d73 673d 6627 7b76  utError(msg=f'{v
-0002ec70: 6964 656f 5f70 6174 687d 2069 7320 6e6f  ideo_path} is no
-0002ec80: 7420 6120 7661 6c69 6420 6669 6c65 2070  t a valid file p
-0002ec90: 6174 6820 6f72 2061 2076 616c 6964 2064  ath or a valid d
-0002eca0: 6972 6563 746f 7279 2070 6174 6827 2c20  irectory path', 
-0002ecb0: 736f 7572 6365 3d73 7570 6572 696d 706f  source=superimpo
-0002ecc0: 7365 5f76 6964 656f 5f6e 616d 6573 2e5f  se_video_names._
-0002ecd0: 5f6e 616d 655f 5f29 0a20 2020 2069 6620  _name__).    if 
-0002ece0: 7361 7665 5f64 6972 2069 7320 6e6f 7420  save_dir is not 
-0002ecf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6368  None:.        ch
-0002ed00: 6563 6b5f 6966 5f64 6972 5f65 7869 7374  eck_if_dir_exist
-0002ed10: 7328 696e 5f64 6972 3d73 6176 655f 6469  s(in_dir=save_di
-0002ed20: 7229 0a20 2020 2065 6c73 653a 0a20 2020  r).    else:.   
-0002ed30: 2020 2020 2073 6176 655f 6469 7220 3d20       save_dir = 
-0002ed40: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-0002ed50: 7669 6465 6f5f 7061 7468 735b 305d 290a  video_paths[0]).
-0002ed60: 2020 2020 666f 7220 6669 6c65 5f63 6e74      for file_cnt
-0002ed70: 2c20 7669 6465 6f5f 7061 7468 2069 6e20  , video_path in 
-0002ed80: 656e 756d 6572 6174 6528 7669 6465 6f5f  enumerate(video_
-0002ed90: 7061 7468 7329 3a0a 2020 2020 2020 2020  paths):.        
-0002eda0: 5f2c 2076 6964 656f 5f6e 616d 652c 2065  _, video_name, e
-0002edb0: 7874 203d 2067 6574 5f66 6e5f 6578 7428  xt = get_fn_ext(
-0002edc0: 7669 6465 6f5f 7061 7468 290a 2020 2020  video_path).    
-0002edd0: 2020 2020 7072 696e 7428 6627 5375 7065      print(f'Supe
-0002ede0: 7269 6d70 6f73 696e 6720 7669 6465 6f20  rimposing video 
-0002edf0: 6e61 6d65 206f 6e20 7b76 6964 656f 5f6e  name on {video_n
-0002ee00: 616d 657d 2028 5669 6465 6f20 7b66 696c  ame} (Video {fil
-0002ee10: 655f 636e 7420 2b20 317d 2f7b 6c65 6e28  e_cnt + 1}/{len(
-0002ee20: 7669 6465 6f5f 7061 7468 7329 7d29 2e2e  video_paths)})..
-0002ee30: 2e27 290a 2020 2020 2020 2020 7361 7665  .').        save
-0002ee40: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-0002ee50: 6a6f 696e 2873 6176 655f 6469 722c 2066  join(save_dir, f
-0002ee60: 277b 7669 6465 6f5f 6e61 6d65 7d5f 7669  '{video_name}_vi
-0002ee70: 6465 6f5f 6e61 6d65 5f73 7570 6572 696d  deo_name_superim
-0002ee80: 706f 7365 647b 6578 747d 2729 0a20 2020  posed{ext}').   
-0002ee90: 2020 2020 2069 6620 706f 7369 7469 6f6e       if position
-0002eea0: 203d 3d20 504f 5349 5449 4f4e 535b 305d   == POSITIONS[0]
-0002eeb0: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
-0002eec0: 6420 3d20 6622 6666 6d70 6567 202d 6920  d = f"ffmpeg -i 
-0002eed0: 277b 7669 6465 6f5f 7061 7468 7d27 202d  '{video_path}' -
-0002eee0: 7666 205c 2264 7261 7774 6578 743d 666f  vf \"drawtext=fo
-0002eef0: 6e74 6669 6c65 3d7b 666f 6e74 5f70 6174  ntfile={font_pat
-0002ef00: 687d 3a74 6578 743d 7b76 6964 656f 5f6e  h}:text={video_n
-0002ef10: 616d 657d 3a78 3d35 3a79 3d35 3a66 6f6e  ame}:x=5:y=5:fon
-0002ef20: 7473 697a 653d 7b66 6f6e 745f 7369 7a65  tsize={font_size
-0002ef30: 7d3a 666f 6e74 636f 6c6f 723d 7b66 6f6e  }:fontcolor={fon
-0002ef40: 745f 636f 6c6f 727d 3a62 6f72 6465 7277  t_color}:borderw
-0002ef50: 3d7b 666f 6e74 5f62 6f72 6465 725f 7769  ={font_border_wi
-0002ef60: 6474 687d 3a62 6f72 6465 7263 6f6c 6f72  dth}:bordercolor
-0002ef70: 3d7b 666f 6e74 5f62 6f72 6465 725f 636f  ={font_border_co
-0002ef80: 6c6f 727d 5c22 202d 633a 6120 636f 7079  lor}\" -c:a copy
-0002ef90: 2027 7b73 6176 655f 7061 7468 7d27 202d   '{save_path}' -
-0002efa0: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
-0002efb0: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
-0002efc0: 6572 202d 7922 0a20 2020 2020 2020 2065  er -y".        e
-0002efd0: 6c69 6620 706f 7369 7469 6f6e 203d 3d20  lif position == 
-0002efe0: 504f 5349 5449 4f4e 535b 315d 3a0a 2020  POSITIONS[1]:.  
-0002eff0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-0002f000: 6622 6666 6d70 6567 202d 6920 277b 7669  f"ffmpeg -i '{vi
-0002f010: 6465 6f5f 7061 7468 7d27 202d 7666 205c  deo_path}' -vf \
-0002f020: 2264 7261 7774 6578 743d 666f 6e74 6669  "drawtext=fontfi
-0002f030: 6c65 3d7b 666f 6e74 5f70 6174 687d 3a74  le={font_path}:t
-0002f040: 6578 743d 7b76 6964 656f 5f6e 616d 657d  ext={video_name}
-0002f050: 3a78 3d28 772d 7477 2d35 293a 793d 353a  :x=(w-tw-5):y=5:
-0002f060: 666f 6e74 7369 7a65 3d7b 666f 6e74 5f73  fontsize={font_s
-0002f070: 697a 657d 3a66 6f6e 7463 6f6c 6f72 3d7b  ize}:fontcolor={
-0002f080: 666f 6e74 5f63 6f6c 6f72 7d3a 626f 7264  font_color}:bord
-0002f090: 6572 773d 7b66 6f6e 745f 626f 7264 6572  erw={font_border
-0002f0a0: 5f77 6964 7468 7d3a 626f 7264 6572 636f  _width}:borderco
-0002f0b0: 6c6f 723d 7b66 6f6e 745f 626f 7264 6572  lor={font_border
-0002f0c0: 5f63 6f6c 6f72 7d5c 2220 2d63 3a61 2063  _color}\" -c:a c
-0002f0d0: 6f70 7920 277b 7361 7665 5f70 6174 687d  opy '{save_path}
-0002f0e0: 2720 2d6c 6f67 6c65 7665 6c20 6572 726f  ' -loglevel erro
-0002f0f0: 7220 2d73 7461 7473 202d 6869 6465 5f62  r -stats -hide_b
-0002f100: 616e 6e65 7220 2d79 220a 2020 2020 2020  anner -y".      
-0002f110: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
-0002f120: 3d3d 2050 4f53 4954 494f 4e53 5b32 5d3a  == POSITIONS[2]:
-0002f130: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-0002f140: 203d 2066 2266 666d 7065 6720 2d69 2027   = f"ffmpeg -i '
-0002f150: 7b76 6964 656f 5f70 6174 687d 2720 2d76  {video_path}' -v
-0002f160: 6620 5c22 6472 6177 7465 7874 3d66 6f6e  f \"drawtext=fon
-0002f170: 7466 696c 653d 7b66 6f6e 745f 7061 7468  tfile={font_path
-0002f180: 7d3a 7465 7874 3d7b 7669 6465 6f5f 6e61  }:text={video_na
-0002f190: 6d65 7d3a 783d 353a 793d 2868 2d74 682d  me}:x=5:y=(h-th-
-0002f1a0: 3529 3a66 6f6e 7473 697a 653d 7b66 6f6e  5):fontsize={fon
-0002f1b0: 745f 7369 7a65 7d3a 666f 6e74 636f 6c6f  t_size}:fontcolo
-0002f1c0: 723d 7b66 6f6e 745f 636f 6c6f 727d 3a62  r={font_color}:b
-0002f1d0: 6f72 6465 7277 3d7b 666f 6e74 5f62 6f72  orderw={font_bor
-0002f1e0: 6465 725f 7769 6474 687d 3a62 6f72 6465  der_width}:borde
-0002f1f0: 7263 6f6c 6f72 3d7b 666f 6e74 5f62 6f72  rcolor={font_bor
-0002f200: 6465 725f 636f 6c6f 727d 5c22 202d 633a  der_color}\" -c:
-0002f210: 6120 636f 7079 2027 7b73 6176 655f 7061  a copy '{save_pa
-0002f220: 7468 7d27 202d 6c6f 676c 6576 656c 2065  th}' -loglevel e
-0002f230: 7272 6f72 202d 7374 6174 7320 2d68 6964  rror -stats -hid
-0002f240: 655f 6261 6e6e 6572 202d 7922 0a20 2020  e_banner -y".   
-0002f250: 2020 2020 2065 6c69 6620 706f 7369 7469       elif positi
-0002f260: 6f6e 203d 3d20 504f 5349 5449 4f4e 535b  on == POSITIONS[
-0002f270: 335d 3a0a 2020 2020 2020 2020 2020 2020  3]:.            
-0002f280: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
-0002f290: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
-0002f2a0: 202d 7666 205c 2264 7261 7774 6578 743d   -vf \"drawtext=
-0002f2b0: 666f 6e74 6669 6c65 3d7b 666f 6e74 5f70  fontfile={font_p
-0002f2c0: 6174 687d 3a74 6578 743d 7b76 6964 656f  ath}:text={video
-0002f2d0: 5f6e 616d 657d 3a78 3d28 772d 7477 2d35  _name}:x=(w-tw-5
-0002f2e0: 293a 793d 2868 2d74 682d 3529 3a66 6f6e  ):y=(h-th-5):fon
-0002f2f0: 7473 697a 653d 7b66 6f6e 745f 7369 7a65  tsize={font_size
-0002f300: 7d3a 666f 6e74 636f 6c6f 723d 7b66 6f6e  }:fontcolor={fon
-0002f310: 745f 636f 6c6f 727d 3a62 6f72 6465 7277  t_color}:borderw
-0002f320: 3d7b 666f 6e74 5f62 6f72 6465 725f 7769  ={font_border_wi
-0002f330: 6474 687d 3a62 6f72 6465 7263 6f6c 6f72  dth}:bordercolor
-0002f340: 3d7b 666f 6e74 5f62 6f72 6465 725f 636f  ={font_border_co
-0002f350: 6c6f 727d 5c22 202d 633a 6120 636f 7079  lor}\" -c:a copy
-0002f360: 2027 7b73 6176 655f 7061 7468 7d27 202d   '{save_path}' -
-0002f370: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
-0002f380: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
-0002f390: 6572 202d 7922 0a20 2020 2020 2020 2065  er -y".        e
-0002f3a0: 6c69 6620 706f 7369 7469 6f6e 203d 3d20  lif position == 
-0002f3b0: 504f 5349 5449 4f4e 535b 345d 3a0a 2020  POSITIONS[4]:.  
-0002f3c0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-0002f3d0: 6622 6666 6d70 6567 202d 6920 277b 7669  f"ffmpeg -i '{vi
-0002f3e0: 6465 6f5f 7061 7468 7d27 202d 7666 205c  deo_path}' -vf \
-0002f3f0: 2264 7261 7774 6578 743d 666f 6e74 6669  "drawtext=fontfi
-0002f400: 6c65 3d7b 666f 6e74 5f70 6174 687d 3a74  le={font_path}:t
-0002f410: 6578 743d 7b76 6964 656f 5f6e 616d 657d  ext={video_name}
-0002f420: 3a78 3d28 772d 7477 292f 323a 793d 3130  :x=(w-tw)/2:y=10
-0002f430: 3a66 6f6e 7473 697a 653d 7b66 6f6e 745f  :fontsize={font_
-0002f440: 7369 7a65 7d3a 666f 6e74 636f 6c6f 723d  size}:fontcolor=
-0002f450: 7b66 6f6e 745f 636f 6c6f 727d 3a62 6f72  {font_color}:bor
-0002f460: 6465 7277 3d7b 666f 6e74 5f62 6f72 6465  derw={font_borde
-0002f470: 725f 7769 6474 687d 3a62 6f72 6465 7263  r_width}:borderc
-0002f480: 6f6c 6f72 3d7b 666f 6e74 5f62 6f72 6465  olor={font_borde
-0002f490: 725f 636f 6c6f 727d 5c22 202d 633a 6120  r_color}\" -c:a 
-0002f4a0: 636f 7079 2027 7b73 6176 655f 7061 7468  copy '{save_path
-0002f4b0: 7d27 202d 6c6f 676c 6576 656c 2065 7272  }' -loglevel err
-0002f4c0: 6f72 202d 7374 6174 7320 2d68 6964 655f  or -stats -hide_
-0002f4d0: 6261 6e6e 6572 202d 7922 0a20 2020 2020  banner -y".     
-0002f4e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0002f4f0: 2020 2020 2063 6d64 203d 2066 2266 666d       cmd = f"ffm
-0002f500: 7065 6720 2d69 2027 7b76 6964 656f 5f70  peg -i '{video_p
-0002f510: 6174 687d 2720 2d76 6620 5c22 6472 6177  ath}' -vf \"draw
-0002f520: 7465 7874 3d66 6f6e 7466 696c 653d 7b66  text=fontfile={f
-0002f530: 6f6e 745f 7061 7468 7d3a 7465 7874 3d7b  ont_path}:text={
-0002f540: 7669 6465 6f5f 6e61 6d65 7d3a 783d 2877  video_name}:x=(w
-0002f550: 2d74 7729 2f32 3a79 3d28 682d 7468 2d31  -tw)/2:y=(h-th-1
-0002f560: 3029 3a66 6f6e 7473 697a 653d 7b66 6f6e  0):fontsize={fon
-0002f570: 745f 7369 7a65 7d3a 666f 6e74 636f 6c6f  t_size}:fontcolo
-0002f580: 723d 7b66 6f6e 745f 636f 6c6f 727d 3a62  r={font_color}:b
-0002f590: 6f72 6465 7277 3d7b 666f 6e74 5f62 6f72  orderw={font_bor
-0002f5a0: 6465 725f 7769 6474 687d 3a62 6f72 6465  der_width}:borde
-0002f5b0: 7263 6f6c 6f72 3d7b 666f 6e74 5f62 6f72  rcolor={font_bor
-0002f5c0: 6465 725f 636f 6c6f 727d 5c22 202d 633a  der_color}\" -c:
-0002f5d0: 6120 636f 7079 2027 7b73 6176 655f 7061  a copy '{save_pa
-0002f5e0: 7468 7d27 202d 6c6f 676c 6576 656c 2065  th}' -loglevel e
-0002f5f0: 7272 6f72 202d 7374 6174 7320 2d68 6964  rror -stats -hid
-0002f600: 655f 6261 6e6e 6572 202d 7922 0a20 2020  e_banner -y".   
-0002f610: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
-0002f620: 6361 6c6c 2863 6d64 2c20 7368 656c 6c3d  call(cmd, shell=
-0002f630: 5472 7565 2c20 7374 646f 7574 3d73 7562  True, stdout=sub
-0002f640: 7072 6f63 6573 732e 5049 5045 290a 2020  process.PIPE).  
-0002f650: 2020 7469 6d65 722e 7374 6f70 5f74 696d    timer.stop_tim
-0002f660: 6572 2829 0a20 2020 2073 7464 6f75 745f  er().    stdout_
-0002f670: 7375 6363 6573 7328 6d73 673d 6627 5375  success(msg=f'Su
-0002f680: 7065 722d 696d 706f 7365 6420 7669 6465  per-imposed vide
-0002f690: 6f20 6e61 6d65 206f 6e20 7b6c 656e 2876  o name on {len(v
-0002f6a0: 6964 656f 5f70 6174 6873 297d 2076 6964  ideo_paths)} vid
-0002f6b0: 656f 2873 292c 2073 6176 6564 2069 6e20  eo(s), saved in 
-0002f6c0: 7b73 6176 655f 6469 727d 272c 2065 6c61  {save_dir}', ela
-0002f6d0: 7073 6564 5f74 696d 653d 7469 6d65 722e  psed_time=timer.
-0002f6e0: 656c 6170 7365 645f 7469 6d65 5f73 7472  elapsed_time_str
-0002f6f0: 290a 0a64 6566 2073 7570 6572 696d 706f  )..def superimpo
-0002f700: 7365 5f66 7265 6574 6578 7428 7669 6465  se_freetext(vide
-0002f710: 6f5f 7061 7468 3a20 556e 696f 6e5b 7374  o_path: Union[st
-0002f720: 722c 206f 732e 5061 7468 4c69 6b65 5d2c  r, os.PathLike],
-0002f730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002f740: 2020 2020 2020 2020 2020 7465 7874 3a20            text: 
-0002f750: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-0002f760: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002f770: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-0002f780: 5d20 3d20 2741 7269 616c 272c 0a20 2020  ] = 'Arial',.   
+0002e390: 696d 706f 7365 5f76 6964 656f 5f6e 616d  impose_video_nam
+0002e3a0: 6573 2e77 6562 6d0a 2020 2020 2020 203a  es.webm.       :
+0002e3b0: 7769 6474 683a 2039 3030 0a20 2020 2020  width: 900.     
+0002e3c0: 2020 3a6c 6f6f 703a 0a0a 2020 2020 3a70    :loop:..    :p
+0002e3d0: 6172 616d 2055 6e69 6f6e 5b73 7472 2c20  aram Union[str, 
+0002e3e0: 6f73 2e50 6174 684c 696b 655d 2076 6964  os.PathLike] vid
+0002e3f0: 656f 5f70 6174 683a 2050 6174 6820 746f  eo_path: Path to
+0002e400: 2074 6865 2069 6e70 7574 2076 6964 656f   the input video
+0002e410: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
+0002e420: 7279 2063 6f6e 7461 696e 696e 6720 7669  ry containing vi
+0002e430: 6465 6f20 6669 6c65 732e 0a20 2020 203a  deo files..    :
+0002e440: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
+0002e450: 6e74 5d20 666f 6e74 5f73 697a 653a 2046  nt] font_size: F
+0002e460: 6f6e 7420 7369 7a65 2066 6f72 2074 6865  ont size for the
+0002e470: 2076 6964 656f 206e 616d 6520 7465 7874   video name text
+0002e480: 2e20 4465 6661 756c 7420 3330 2e0a 2020  . Default 30..  
+0002e490: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+0002e4a0: 6c5b 7374 725d 2066 6f6e 745f 636f 6c6f  l[str] font_colo
+0002e4b0: 723a 2020 466f 6e74 2063 6f6c 6f72 2066  r:  Font color f
+0002e4c0: 6f72 2074 6865 2076 6964 656f 206e 616d  or the video nam
+0002e4d0: 6520 7465 7874 2e20 4465 6661 756c 7420  e text. Default 
+0002e4e0: 7768 6974 650a 2020 2020 3a70 6172 616d  white.    :param
+0002e4f0: 204f 7074 696f 6e61 6c5b 7374 725d 2066   Optional[str] f
+0002e500: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
+0002e510: 3a20 466f 6e74 2062 6f72 6465 7220 636f  : Font border co
+0002e520: 6c6f 7220 666f 7220 7468 6520 7669 6465  lor for the vide
+0002e530: 6f20 6e61 6d65 2074 6578 742e 2044 6566  o name text. Def
+0002e540: 6175 6c74 2062 6c61 636b 2e0a 2020 2020  ault black..    
+0002e550: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
+0002e560: 696e 745d 2066 6f6e 745f 626f 7264 6572  int] font_border
+0002e570: 5f77 6964 7468 3a20 466f 6e74 2062 6f72  _width: Font bor
+0002e580: 6465 7220 7769 6474 6820 666f 7220 7468  der width for th
+0002e590: 6520 7669 6465 6f20 6e61 6d65 2074 6578  e video name tex
+0002e5a0: 7420 696e 2070 6978 656c 732e 2044 6566  t in pixels. Def
+0002e5b0: 6175 6c74 2032 2e0a 2020 2020 3a70 6172  ault 2..    :par
+0002e5c0: 616d 204f 7074 696f 6e61 6c5b 4c69 7465  am Optional[Lite
+0002e5d0: 7261 6c5b 2774 6f70 5f6c 6566 7427 2c20  ral['top_left', 
+0002e5e0: 2774 6f70 5f72 6967 6874 272c 2027 626f  'top_right', 'bo
+0002e5f0: 7474 6f6d 5f6c 6566 7427 2c20 2762 6f74  ttom_left', 'bot
+0002e600: 746f 6d5f 7269 6768 7427 2c20 2774 6f70  tom_right', 'top
+0002e610: 5f6d 6964 646c 6527 2c20 2762 6f74 746f  _middle', 'botto
+0002e620: 6d5f 6d69 6464 6c65 275d 5d20 706f 7369  m_middle']] posi
+0002e630: 7469 6f6e 3a20 506f 7369 7469 6f6e 2077  tion: Position w
+0002e640: 6865 7265 2074 6865 2076 6964 656f 206e  here the video n
+0002e650: 616d 6520 7769 6c6c 2062 6520 7375 7065  ame will be supe
+0002e660: 7269 6d70 6f73 6564 2e20 4465 6661 756c  rimposed. Defaul
+0002e670: 7420 6060 746f 705f 6c65 6674 6060 2e0a  t ``top_left``..
+0002e680: 2020 2020 3a70 6172 616d 204f 7074 696f      :param Optio
+0002e690: 6e61 6c5b 556e 696f 6e5b 7374 722c 206f  nal[Union[str, o
+0002e6a0: 732e 5061 7468 4c69 6b65 5d5d 2073 6176  s.PathLike]] sav
+0002e6b0: 655f 6469 723a 2044 6972 6563 746f 7279  e_dir: Directory
+0002e6c0: 2077 6865 7265 2074 6865 206d 6f64 6966   where the modif
+0002e6d0: 6965 6420 7669 6465 6f28 7329 2077 696c  ied video(s) wil
+0002e6e0: 6c20 6265 2073 6176 6564 2e20 4966 206e  l be saved. If n
+0002e6f0: 6f74 2070 726f 7669 6465 642c 2074 6865  ot provided, the
+0002e700: 2064 6972 6563 746f 7279 206f 6620 7468   directory of th
+0002e710: 6520 696e 7075 7420 7669 6465 6f28 7329  e input video(s)
+0002e720: 2077 696c 6c20 6265 2075 7365 642e 0a20   will be used.. 
+0002e730: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
+0002e740: 0a0a 2020 2020 3a65 7861 6d70 6c65 3a0a  ..    :example:.
+0002e750: 2020 2020 3e3e 3e20 7375 7065 7269 6d70      >>> superimp
+0002e760: 6f73 655f 7669 6465 6f5f 6e61 6d65 7328  ose_video_names(
+0002e770: 7669 6465 6f5f 7061 7468 3d27 2f55 7365  video_path='/Use
+0002e780: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+0002e790: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+0002e7a0: 626c 6573 686f 6f74 696e 672f 6d6f 7573  bleshooting/mous
+0002e7b0: 655f 6f70 656e 5f66 6965 6c64 2f70 726f  e_open_field/pro
+0002e7c0: 6a65 6374 5f66 6f6c 6465 722f 7669 6465  ject_folder/vide
+0002e7d0: 6f73 2f74 6573 745f 342f 312e 6d70 3427  os/test_4/1.mp4'
+0002e7e0: 2c20 706f 7369 7469 6f6e 3d27 6d69 6464  , position='midd
+0002e7f0: 6c65 5f74 6f70 272c 2066 6f6e 745f 636f  le_top', font_co
+0002e800: 6c6f 723d 2762 6c61 636b 272c 2066 6f6e  lor='black', fon
+0002e810: 745f 626f 7264 6572 5f63 6f6c 6f72 3d27  t_border_color='
+0002e820: 7069 6e6b 272c 2066 6f6e 745f 626f 7264  pink', font_bord
+0002e830: 6572 5f77 6964 7468 3d35 2c20 666f 6e74  er_width=5, font
+0002e840: 5f73 697a 653d 3330 290a 2020 2020 2222  _size=30).    ""
+0002e850: 220a 0a20 2020 2063 6865 636b 5f66 666d  "..    check_ffm
+0002e860: 7065 675f 6176 6169 6c61 626c 6528 7261  peg_available(ra
+0002e870: 6973 655f 6572 726f 723d 5472 7565 290a  ise_error=True).
+0002e880: 2020 2020 7469 6d65 7220 3d20 5369 6d62      timer = Simb
+0002e890: 6154 696d 6572 2873 7461 7274 3d54 7275  aTimer(start=Tru
+0002e8a0: 6529 0a20 2020 2050 4f53 4954 494f 4e53  e).    POSITIONS
+0002e8b0: 203d 205b 2774 6f70 5f6c 6566 7427 2c20   = ['top_left', 
+0002e8c0: 2774 6f70 5f72 6967 6874 272c 2027 626f  'top_right', 'bo
+0002e8d0: 7474 6f6d 5f6c 6566 7427 2c20 2762 6f74  ttom_left', 'bot
+0002e8e0: 746f 6d5f 7269 6768 7427 2c20 2774 6f70  tom_right', 'top
+0002e8f0: 5f6d 6964 646c 6527 2c20 2762 6f74 746f  _middle', 'botto
+0002e900: 6d5f 6d69 6464 6c65 275d 0a20 2020 2063  m_middle'].    c
+0002e910: 6865 636b 5f73 7472 286e 616d 653d 6627  heck_str(name=f'
+0002e920: 7b73 7570 6572 696d 706f 7365 5f76 6964  {superimpose_vid
+0002e930: 656f 5f6e 616d 6573 2e5f 5f6e 616d 655f  eo_names.__name_
+0002e940: 5f7d 2070 6f73 6974 696f 6e27 2c20 7661  _} position', va
+0002e950: 6c75 653d 706f 7369 7469 6f6e 2c20 6f70  lue=position, op
+0002e960: 7469 6f6e 733d 504f 5349 5449 4f4e 5329  tions=POSITIONS)
+0002e970: 0a20 2020 2063 6865 636b 5f69 6e74 286e  .    check_int(n
+0002e980: 616d 653d 6627 7b73 7570 6572 696d 706f  ame=f'{superimpo
+0002e990: 7365 5f76 6964 656f 5f6e 616d 6573 2e5f  se_video_names._
+0002e9a0: 5f6e 616d 655f 5f7d 2066 6f6e 745f 7369  _name__} font_si
+0002e9b0: 7a65 272c 2076 616c 7565 3d66 6f6e 745f  ze', value=font_
+0002e9c0: 7369 7a65 2c20 6d69 6e5f 7661 6c75 653d  size, min_value=
+0002e9d0: 3129 0a20 2020 2063 6865 636b 5f69 6e74  1).    check_int
+0002e9e0: 286e 616d 653d 6627 7b73 7570 6572 696d  (name=f'{superim
+0002e9f0: 706f 7365 5f76 6964 656f 5f6e 616d 6573  pose_video_names
+0002ea00: 2e5f 5f6e 616d 655f 5f7d 2066 6f6e 745f  .__name__} font_
+0002ea10: 626f 7264 6572 5f77 6964 7468 272c 2076  border_width', v
+0002ea20: 616c 7565 3d66 6f6e 745f 626f 7264 6572  alue=font_border
+0002ea30: 5f77 6964 7468 2c20 6d69 6e5f 7661 6c75  _width, min_valu
+0002ea40: 653d 3129 0a20 2020 2066 6f6e 745f 6469  e=1).    font_di
+0002ea50: 6374 203d 2067 6574 5f66 6f6e 7473 2829  ct = get_fonts()
+0002ea60: 0a20 2020 2063 6865 636b 5f73 7472 286e  .    check_str(n
+0002ea70: 616d 653d 2766 6f6e 7427 2c20 7661 6c75  ame='font', valu
+0002ea80: 653d 666f 6e74 2c20 6f70 7469 6f6e 733d  e=font, options=
+0002ea90: 7475 706c 6528 666f 6e74 5f64 6963 742e  tuple(font_dict.
+0002eaa0: 6b65 7973 2829 2929 0a20 2020 2066 6f6e  keys())).    fon
+0002eab0: 745f 7061 7468 203d 2066 6f6e 745f 6469  t_path = font_di
+0002eac0: 6374 5b66 6f6e 745d 0a20 2020 2066 6f6e  ct[font].    fon
+0002ead0: 745f 636f 6c6f 7220 3d20 2727 2e6a 6f69  t_color = ''.joi
+0002eae0: 6e28 6669 6c74 6572 2873 7472 2e69 7361  n(filter(str.isa
+0002eaf0: 6c6e 756d 2c20 666f 6e74 5f63 6f6c 6f72  lnum, font_color
+0002eb00: 2929 2e6c 6f77 6572 2829 0a20 2020 2066  )).lower().    f
+0002eb10: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
+0002eb20: 203d 2027 272e 6a6f 696e 2866 696c 7465   = ''.join(filte
+0002eb30: 7228 7374 722e 6973 616c 6e75 6d2c 2066  r(str.isalnum, f
+0002eb40: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
+0002eb50: 2929 2e6c 6f77 6572 2829 0a20 2020 2069  )).lower().    i
+0002eb60: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
+0002eb70: 2876 6964 656f 5f70 6174 6829 3a0a 2020  (video_path):.  
+0002eb80: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
+0002eb90: 7320 3d20 5b76 6964 656f 5f70 6174 685d  s = [video_path]
+0002eba0: 0a20 2020 2065 6c69 6620 6f73 2e70 6174  .    elif os.pat
+0002ebb0: 682e 6973 6469 7228 7669 6465 6f5f 7061  h.isdir(video_pa
+0002ebc0: 7468 293a 0a20 2020 2020 2020 2076 6964  th):.        vid
+0002ebd0: 656f 5f70 6174 6873 203d 206c 6973 7428  eo_paths = list(
+0002ebe0: 6669 6e64 5f61 6c6c 5f76 6964 656f 735f  find_all_videos_
+0002ebf0: 696e 5f64 6972 6563 746f 7279 2864 6972  in_directory(dir
+0002ec00: 6563 746f 7279 3d76 6964 656f 5f70 6174  ectory=video_pat
+0002ec10: 682c 2061 735f 6469 6374 3d54 7275 652c  h, as_dict=True,
+0002ec20: 2072 6169 7365 5f65 7272 6f72 3d54 7275   raise_error=Tru
+0002ec30: 6529 2e76 616c 7565 7328 2929 0a20 2020  e).values()).   
+0002ec40: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+0002ec50: 6169 7365 2049 6e76 616c 6964 496e 7075  aise InvalidInpu
+0002ec60: 7445 7272 6f72 286d 7367 3d66 277b 7669  tError(msg=f'{vi
+0002ec70: 6465 6f5f 7061 7468 7d20 6973 206e 6f74  deo_path} is not
+0002ec80: 2061 2076 616c 6964 2066 696c 6520 7061   a valid file pa
+0002ec90: 7468 206f 7220 6120 7661 6c69 6420 6469  th or a valid di
+0002eca0: 7265 6374 6f72 7920 7061 7468 272c 2073  rectory path', s
+0002ecb0: 6f75 7263 653d 7375 7065 7269 6d70 6f73  ource=superimpos
+0002ecc0: 655f 7669 6465 6f5f 6e61 6d65 732e 5f5f  e_video_names.__
+0002ecd0: 6e61 6d65 5f5f 290a 2020 2020 6966 2073  name__).    if s
+0002ece0: 6176 655f 6469 7220 6973 206e 6f74 204e  ave_dir is not N
+0002ecf0: 6f6e 653a 0a20 2020 2020 2020 2063 6865  one:.        che
+0002ed00: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
+0002ed10: 2869 6e5f 6469 723d 7361 7665 5f64 6972  (in_dir=save_dir
+0002ed20: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+0002ed30: 2020 2020 7361 7665 5f64 6972 203d 206f      save_dir = o
+0002ed40: 732e 7061 7468 2e64 6972 6e61 6d65 2876  s.path.dirname(v
+0002ed50: 6964 656f 5f70 6174 6873 5b30 5d29 0a20  ideo_paths[0]). 
+0002ed60: 2020 2066 6f72 2066 696c 655f 636e 742c     for file_cnt,
+0002ed70: 2076 6964 656f 5f70 6174 6820 696e 2065   video_path in e
+0002ed80: 6e75 6d65 7261 7465 2876 6964 656f 5f70  numerate(video_p
+0002ed90: 6174 6873 293a 0a20 2020 2020 2020 205f  aths):.        _
+0002eda0: 2c20 7669 6465 6f5f 6e61 6d65 2c20 6578  , video_name, ex
+0002edb0: 7420 3d20 6765 745f 666e 5f65 7874 2876  t = get_fn_ext(v
+0002edc0: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
+0002edd0: 2020 2070 7269 6e74 2866 2753 7570 6572     print(f'Super
+0002ede0: 696d 706f 7369 6e67 2076 6964 656f 206e  imposing video n
+0002edf0: 616d 6520 6f6e 207b 7669 6465 6f5f 6e61  ame on {video_na
+0002ee00: 6d65 7d20 2856 6964 656f 207b 6669 6c65  me} (Video {file
+0002ee10: 5f63 6e74 202b 2031 7d2f 7b6c 656e 2876  _cnt + 1}/{len(v
+0002ee20: 6964 656f 5f70 6174 6873 297d 292e 2e2e  ideo_paths)})...
+0002ee30: 2729 0a20 2020 2020 2020 2073 6176 655f  ').        save_
+0002ee40: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+0002ee50: 6f69 6e28 7361 7665 5f64 6972 2c20 6627  oin(save_dir, f'
+0002ee60: 7b76 6964 656f 5f6e 616d 657d 5f76 6964  {video_name}_vid
+0002ee70: 656f 5f6e 616d 655f 7375 7065 7269 6d70  eo_name_superimp
+0002ee80: 6f73 6564 7b65 7874 7d27 290a 2020 2020  osed{ext}').    
+0002ee90: 2020 2020 6966 2070 6f73 6974 696f 6e20      if position 
+0002eea0: 3d3d 2050 4f53 4954 494f 4e53 5b30 5d3a  == POSITIONS[0]:
+0002eeb0: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+0002eec0: 203d 2066 2266 666d 7065 6720 2d69 2027   = f"ffmpeg -i '
+0002eed0: 7b76 6964 656f 5f70 6174 687d 2720 2d76  {video_path}' -v
+0002eee0: 6620 5c22 6472 6177 7465 7874 3d66 6f6e  f \"drawtext=fon
+0002eef0: 7466 696c 653d 7b66 6f6e 745f 7061 7468  tfile={font_path
+0002ef00: 7d3a 7465 7874 3d7b 7669 6465 6f5f 6e61  }:text={video_na
+0002ef10: 6d65 7d3a 783d 353a 793d 353a 666f 6e74  me}:x=5:y=5:font
+0002ef20: 7369 7a65 3d7b 666f 6e74 5f73 697a 657d  size={font_size}
+0002ef30: 3a66 6f6e 7463 6f6c 6f72 3d7b 666f 6e74  :fontcolor={font
+0002ef40: 5f63 6f6c 6f72 7d3a 626f 7264 6572 773d  _color}:borderw=
+0002ef50: 7b66 6f6e 745f 626f 7264 6572 5f77 6964  {font_border_wid
+0002ef60: 7468 7d3a 626f 7264 6572 636f 6c6f 723d  th}:bordercolor=
+0002ef70: 7b66 6f6e 745f 626f 7264 6572 5f63 6f6c  {font_border_col
+0002ef80: 6f72 7d5c 2220 2d63 3a61 2063 6f70 7920  or}\" -c:a copy 
+0002ef90: 277b 7361 7665 5f70 6174 687d 2720 2d6c  '{save_path}' -l
+0002efa0: 6f67 6c65 7665 6c20 6572 726f 7220 2d73  oglevel error -s
+0002efb0: 7461 7473 202d 6869 6465 5f62 616e 6e65  tats -hide_banne
+0002efc0: 7220 2d79 220a 2020 2020 2020 2020 656c  r -y".        el
+0002efd0: 6966 2070 6f73 6974 696f 6e20 3d3d 2050  if position == P
+0002efe0: 4f53 4954 494f 4e53 5b31 5d3a 0a20 2020  OSITIONS[1]:.   
+0002eff0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+0002f000: 2266 666d 7065 6720 2d69 2027 7b76 6964  "ffmpeg -i '{vid
+0002f010: 656f 5f70 6174 687d 2720 2d76 6620 5c22  eo_path}' -vf \"
+0002f020: 6472 6177 7465 7874 3d66 6f6e 7466 696c  drawtext=fontfil
+0002f030: 653d 7b66 6f6e 745f 7061 7468 7d3a 7465  e={font_path}:te
+0002f040: 7874 3d7b 7669 6465 6f5f 6e61 6d65 7d3a  xt={video_name}:
+0002f050: 783d 2877 2d74 772d 3529 3a79 3d35 3a66  x=(w-tw-5):y=5:f
+0002f060: 6f6e 7473 697a 653d 7b66 6f6e 745f 7369  ontsize={font_si
+0002f070: 7a65 7d3a 666f 6e74 636f 6c6f 723d 7b66  ze}:fontcolor={f
+0002f080: 6f6e 745f 636f 6c6f 727d 3a62 6f72 6465  ont_color}:borde
+0002f090: 7277 3d7b 666f 6e74 5f62 6f72 6465 725f  rw={font_border_
+0002f0a0: 7769 6474 687d 3a62 6f72 6465 7263 6f6c  width}:bordercol
+0002f0b0: 6f72 3d7b 666f 6e74 5f62 6f72 6465 725f  or={font_border_
+0002f0c0: 636f 6c6f 727d 5c22 202d 633a 6120 636f  color}\" -c:a co
+0002f0d0: 7079 2027 7b73 6176 655f 7061 7468 7d27  py '{save_path}'
+0002f0e0: 202d 6c6f 676c 6576 656c 2065 7272 6f72   -loglevel error
+0002f0f0: 202d 7374 6174 7320 2d68 6964 655f 6261   -stats -hide_ba
+0002f100: 6e6e 6572 202d 7922 0a20 2020 2020 2020  nner -y".       
+0002f110: 2065 6c69 6620 706f 7369 7469 6f6e 203d   elif position =
+0002f120: 3d20 504f 5349 5449 4f4e 535b 325d 3a0a  = POSITIONS[2]:.
+0002f130: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+0002f140: 3d20 6622 6666 6d70 6567 202d 6920 277b  = f"ffmpeg -i '{
+0002f150: 7669 6465 6f5f 7061 7468 7d27 202d 7666  video_path}' -vf
+0002f160: 205c 2264 7261 7774 6578 743d 666f 6e74   \"drawtext=font
+0002f170: 6669 6c65 3d7b 666f 6e74 5f70 6174 687d  file={font_path}
+0002f180: 3a74 6578 743d 7b76 6964 656f 5f6e 616d  :text={video_nam
+0002f190: 657d 3a78 3d35 3a79 3d28 682d 7468 2d35  e}:x=5:y=(h-th-5
+0002f1a0: 293a 666f 6e74 7369 7a65 3d7b 666f 6e74  ):fontsize={font
+0002f1b0: 5f73 697a 657d 3a66 6f6e 7463 6f6c 6f72  _size}:fontcolor
+0002f1c0: 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a 626f  ={font_color}:bo
+0002f1d0: 7264 6572 773d 7b66 6f6e 745f 626f 7264  rderw={font_bord
+0002f1e0: 6572 5f77 6964 7468 7d3a 626f 7264 6572  er_width}:border
+0002f1f0: 636f 6c6f 723d 7b66 6f6e 745f 626f 7264  color={font_bord
+0002f200: 6572 5f63 6f6c 6f72 7d5c 2220 2d63 3a61  er_color}\" -c:a
+0002f210: 2063 6f70 7920 277b 7361 7665 5f70 6174   copy '{save_pat
+0002f220: 687d 2720 2d6c 6f67 6c65 7665 6c20 6572  h}' -loglevel er
+0002f230: 726f 7220 2d73 7461 7473 202d 6869 6465  ror -stats -hide
+0002f240: 5f62 616e 6e65 7220 2d79 220a 2020 2020  _banner -y".    
+0002f250: 2020 2020 656c 6966 2070 6f73 6974 696f      elif positio
+0002f260: 6e20 3d3d 2050 4f53 4954 494f 4e53 5b33  n == POSITIONS[3
+0002f270: 5d3a 0a20 2020 2020 2020 2020 2020 2063  ]:.            c
+0002f280: 6d64 203d 2066 2266 666d 7065 6720 2d69  md = f"ffmpeg -i
+0002f290: 2027 7b76 6964 656f 5f70 6174 687d 2720   '{video_path}' 
+0002f2a0: 2d76 6620 5c22 6472 6177 7465 7874 3d66  -vf \"drawtext=f
+0002f2b0: 6f6e 7466 696c 653d 7b66 6f6e 745f 7061  ontfile={font_pa
+0002f2c0: 7468 7d3a 7465 7874 3d7b 7669 6465 6f5f  th}:text={video_
+0002f2d0: 6e61 6d65 7d3a 783d 2877 2d74 772d 3529  name}:x=(w-tw-5)
+0002f2e0: 3a79 3d28 682d 7468 2d35 293a 666f 6e74  :y=(h-th-5):font
+0002f2f0: 7369 7a65 3d7b 666f 6e74 5f73 697a 657d  size={font_size}
+0002f300: 3a66 6f6e 7463 6f6c 6f72 3d7b 666f 6e74  :fontcolor={font
+0002f310: 5f63 6f6c 6f72 7d3a 626f 7264 6572 773d  _color}:borderw=
+0002f320: 7b66 6f6e 745f 626f 7264 6572 5f77 6964  {font_border_wid
+0002f330: 7468 7d3a 626f 7264 6572 636f 6c6f 723d  th}:bordercolor=
+0002f340: 7b66 6f6e 745f 626f 7264 6572 5f63 6f6c  {font_border_col
+0002f350: 6f72 7d5c 2220 2d63 3a61 2063 6f70 7920  or}\" -c:a copy 
+0002f360: 277b 7361 7665 5f70 6174 687d 2720 2d6c  '{save_path}' -l
+0002f370: 6f67 6c65 7665 6c20 6572 726f 7220 2d73  oglevel error -s
+0002f380: 7461 7473 202d 6869 6465 5f62 616e 6e65  tats -hide_banne
+0002f390: 7220 2d79 220a 2020 2020 2020 2020 656c  r -y".        el
+0002f3a0: 6966 2070 6f73 6974 696f 6e20 3d3d 2050  if position == P
+0002f3b0: 4f53 4954 494f 4e53 5b34 5d3a 0a20 2020  OSITIONS[4]:.   
+0002f3c0: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+0002f3d0: 2266 666d 7065 6720 2d69 2027 7b76 6964  "ffmpeg -i '{vid
+0002f3e0: 656f 5f70 6174 687d 2720 2d76 6620 5c22  eo_path}' -vf \"
+0002f3f0: 6472 6177 7465 7874 3d66 6f6e 7466 696c  drawtext=fontfil
+0002f400: 653d 7b66 6f6e 745f 7061 7468 7d3a 7465  e={font_path}:te
+0002f410: 7874 3d7b 7669 6465 6f5f 6e61 6d65 7d3a  xt={video_name}:
+0002f420: 783d 2877 2d74 7729 2f32 3a79 3d31 303a  x=(w-tw)/2:y=10:
+0002f430: 666f 6e74 7369 7a65 3d7b 666f 6e74 5f73  fontsize={font_s
+0002f440: 697a 657d 3a66 6f6e 7463 6f6c 6f72 3d7b  ize}:fontcolor={
+0002f450: 666f 6e74 5f63 6f6c 6f72 7d3a 626f 7264  font_color}:bord
+0002f460: 6572 773d 7b66 6f6e 745f 626f 7264 6572  erw={font_border
+0002f470: 5f77 6964 7468 7d3a 626f 7264 6572 636f  _width}:borderco
+0002f480: 6c6f 723d 7b66 6f6e 745f 626f 7264 6572  lor={font_border
+0002f490: 5f63 6f6c 6f72 7d5c 2220 2d63 3a61 2063  _color}\" -c:a c
+0002f4a0: 6f70 7920 277b 7361 7665 5f70 6174 687d  opy '{save_path}
+0002f4b0: 2720 2d6c 6f67 6c65 7665 6c20 6572 726f  ' -loglevel erro
+0002f4c0: 7220 2d73 7461 7473 202d 6869 6465 5f62  r -stats -hide_b
+0002f4d0: 616e 6e65 7220 2d79 220a 2020 2020 2020  anner -y".      
+0002f4e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0002f4f0: 2020 2020 636d 6420 3d20 6622 6666 6d70      cmd = f"ffmp
+0002f500: 6567 202d 6920 277b 7669 6465 6f5f 7061  eg -i '{video_pa
+0002f510: 7468 7d27 202d 7666 205c 2264 7261 7774  th}' -vf \"drawt
+0002f520: 6578 743d 666f 6e74 6669 6c65 3d7b 666f  ext=fontfile={fo
+0002f530: 6e74 5f70 6174 687d 3a74 6578 743d 7b76  nt_path}:text={v
+0002f540: 6964 656f 5f6e 616d 657d 3a78 3d28 772d  ideo_name}:x=(w-
+0002f550: 7477 292f 323a 793d 2868 2d74 682d 3130  tw)/2:y=(h-th-10
+0002f560: 293a 666f 6e74 7369 7a65 3d7b 666f 6e74  ):fontsize={font
+0002f570: 5f73 697a 657d 3a66 6f6e 7463 6f6c 6f72  _size}:fontcolor
+0002f580: 3d7b 666f 6e74 5f63 6f6c 6f72 7d3a 626f  ={font_color}:bo
+0002f590: 7264 6572 773d 7b66 6f6e 745f 626f 7264  rderw={font_bord
+0002f5a0: 6572 5f77 6964 7468 7d3a 626f 7264 6572  er_width}:border
+0002f5b0: 636f 6c6f 723d 7b66 6f6e 745f 626f 7264  color={font_bord
+0002f5c0: 6572 5f63 6f6c 6f72 7d5c 2220 2d63 3a61  er_color}\" -c:a
+0002f5d0: 2063 6f70 7920 277b 7361 7665 5f70 6174   copy '{save_pat
+0002f5e0: 687d 2720 2d6c 6f67 6c65 7665 6c20 6572  h}' -loglevel er
+0002f5f0: 726f 7220 2d73 7461 7473 202d 6869 6465  ror -stats -hide
+0002f600: 5f62 616e 6e65 7220 2d79 220a 2020 2020  _banner -y".    
+0002f610: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+0002f620: 616c 6c28 636d 642c 2073 6865 6c6c 3d54  all(cmd, shell=T
+0002f630: 7275 652c 2073 7464 6f75 743d 7375 6270  rue, stdout=subp
+0002f640: 726f 6365 7373 2e50 4950 4529 0a20 2020  rocess.PIPE).   
+0002f650: 2074 696d 6572 2e73 746f 705f 7469 6d65   timer.stop_time
+0002f660: 7228 290a 2020 2020 7374 646f 7574 5f73  r().    stdout_s
+0002f670: 7563 6365 7373 286d 7367 3d66 2753 7570  uccess(msg=f'Sup
+0002f680: 6572 2d69 6d70 6f73 6564 2076 6964 656f  er-imposed video
+0002f690: 206e 616d 6520 6f6e 207b 6c65 6e28 7669   name on {len(vi
+0002f6a0: 6465 6f5f 7061 7468 7329 7d20 7669 6465  deo_paths)} vide
+0002f6b0: 6f28 7329 2c20 7361 7665 6420 696e 207b  o(s), saved in {
+0002f6c0: 7361 7665 5f64 6972 7d27 2c20 656c 6170  save_dir}', elap
+0002f6d0: 7365 645f 7469 6d65 3d74 696d 6572 2e65  sed_time=timer.e
+0002f6e0: 6c61 7073 6564 5f74 696d 655f 7374 7229  lapsed_time_str)
+0002f6f0: 0a0a 6465 6620 7375 7065 7269 6d70 6f73  ..def superimpos
+0002f700: 655f 6672 6565 7465 7874 2876 6964 656f  e_freetext(video
+0002f710: 5f70 6174 683a 2055 6e69 6f6e 5b73 7472  _path: Union[str
+0002f720: 2c20 6f73 2e50 6174 684c 696b 655d 2c0a  , os.PathLike],.
+0002f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f740: 2020 2020 2020 2020 2074 6578 743a 2073           text: s
+0002f750: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+0002f760: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
+0002f770: 743a 204f 7074 696f 6e61 6c5b 7374 725d  t: Optional[str]
+0002f780: 203d 2027 4172 6961 6c27 2c0a 2020 2020   = 'Arial',.    
 0002f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f7a0: 2020 2020 2020 666f 6e74 5f73 697a 653a        font_size:
-0002f7b0: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
-0002f7c0: 2033 302c 0a20 2020 2020 2020 2020 2020   30,.           
-0002f7d0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0002f7e0: 6e74 5f63 6f6c 6f72 3a20 4f70 7469 6f6e  nt_color: Option
-0002f7f0: 616c 5b73 7472 5d20 3d20 2777 6869 7465  al[str] = 'white
-0002f800: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0002f810: 2020 2020 2020 2020 2020 2020 666f 6e74              font
-0002f820: 5f62 6f72 6465 725f 636f 6c6f 723a 204f  _border_color: O
-0002f830: 7074 696f 6e61 6c5b 7374 725d 203d 2027  ptional[str] = '
-0002f840: 626c 6163 6b27 2c0a 2020 2020 2020 2020  black',.        
+0002f7a0: 2020 2020 2066 6f6e 745f 7369 7a65 3a20       font_size: 
+0002f7b0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+0002f7c0: 3330 2c0a 2020 2020 2020 2020 2020 2020  30,.            
+0002f7d0: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
+0002f7e0: 745f 636f 6c6f 723a 204f 7074 696f 6e61  t_color: Optiona
+0002f7f0: 6c5b 7374 725d 203d 2027 7768 6974 6527  l[str] = 'white'
+0002f800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0002f810: 2020 2020 2020 2020 2020 2066 6f6e 745f             font_
+0002f820: 626f 7264 6572 5f63 6f6c 6f72 3a20 4f70  border_color: Op
+0002f830: 7469 6f6e 616c 5b73 7472 5d20 3d20 2762  tional[str] = 'b
+0002f840: 6c61 636b 272c 0a20 2020 2020 2020 2020  lack',.         
 0002f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f860: 2066 6f6e 745f 626f 7264 6572 5f77 6964   font_border_wid
-0002f870: 7468 3a20 4f70 7469 6f6e 616c 5b69 6e74  th: Optional[int
-0002f880: 5d20 3d20 322c 0a20 2020 2020 2020 2020  ] = 2,.         
-0002f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f8a0: 706f 7369 7469 6f6e 3a20 4f70 7469 6f6e  position: Option
-0002f8b0: 616c 5b4c 6974 6572 616c 5b27 746f 705f  al[Literal['top_
-0002f8c0: 6c65 6674 272c 2027 746f 705f 7269 6768  left', 'top_righ
-0002f8d0: 7427 2c20 2762 6f74 746f 6d5f 6c65 6674  t', 'bottom_left
-0002f8e0: 272c 2027 626f 7474 6f6d 5f72 6967 6874  ', 'bottom_right
-0002f8f0: 272c 2027 6d69 6464 6c65 5f74 6f70 272c  ', 'middle_top',
-0002f900: 2027 6d69 6464 6c65 5f62 6f74 746f 6d27   'middle_bottom'
-0002f910: 5d5d 203d 2027 746f 705f 6c65 6674 272c  ]] = 'top_left',
-0002f920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002f930: 2020 2020 2020 2020 2020 7361 7665 5f64            save_d
-0002f940: 6972 3a20 4f70 7469 6f6e 616c 5b55 6e69  ir: Optional[Uni
-0002f950: 6f6e 5b73 7472 2c20 6f73 2e50 6174 684c  on[str, os.PathL
-0002f960: 696b 655d 5d20 3d20 4e6f 6e65 2920 2d3e  ike]] = None) ->
-0002f970: 204e 6f6e 653a 0a20 2020 2022 2222 0a20   None:.    """. 
-0002f980: 2020 2053 7570 6572 696d 706f 7365 7320     Superimposes 
-0002f990: 7061 7373 6564 2074 6578 7420 6f6e 2074  passed text on t
-0002f9a0: 6865 2067 6976 656e 2076 6964 656f 2066  he given video f
-0002f9b0: 696c 6528 7329 2061 6e64 2073 6176 6573  ile(s) and saves
-0002f9c0: 2074 6865 206d 6f64 6966 6965 6420 7669   the modified vi
-0002f9d0: 6465 6f28 7329 2e0a 0a20 2020 202e 2e20  deo(s)...    .. 
-0002f9e0: 7669 6465 6f3a 3a20 5f73 7461 7469 632f  video:: _static/
-0002f9f0: 696d 672f 7375 7065 7269 6d70 6f73 655f  img/superimpose_
-0002fa00: 656c 6170 7365 645f 7469 6d65 2e77 6562  elapsed_time.web
-0002fa10: 6d0a 2020 2020 2020 203a 7769 6474 683a  m.       :width:
-0002fa20: 2039 3030 0a20 2020 2020 2020 3a6c 6f6f   900.       :loo
-0002fa30: 703a 0a0a 2020 2020 3a70 6172 616d 2055  p:..    :param U
-0002fa40: 6e69 6f6e 5b73 7472 2c20 6f73 2e50 6174  nion[str, os.Pat
-0002fa50: 684c 696b 655d 2076 6964 656f 5f70 6174  hLike] video_pat
-0002fa60: 683a 2050 6174 6820 746f 2074 6865 2069  h: Path to the i
-0002fa70: 6e70 7574 2076 6964 656f 2066 696c 6520  nput video file 
-0002fa80: 6f72 2064 6972 6563 746f 7279 2063 6f6e  or directory con
-0002fa90: 7461 696e 696e 6720 7669 6465 6f20 6669  taining video fi
-0002faa0: 6c65 732e 0a20 2020 203a 7061 7261 6d20  les..    :param 
-0002fab0: 7374 7220 7465 7874 3a20 5468 6520 7465  str text: The te
-0002fac0: 7874 2074 6f20 6f76 6572 6c61 7920 6f6e  xt to overlay on
-0002fad0: 2074 6865 2076 6964 656f 0a20 2020 203a   the video.    :
-0002fae0: 7061 7261 6d20 4f70 7469 6f6e 616c 5b69  param Optional[i
-0002faf0: 6e74 5d20 666f 6e74 5f73 697a 653a 2046  nt] font_size: F
-0002fb00: 6f6e 7420 7369 7a65 2066 6f72 2074 6865  ont size for the
-0002fb10: 2074 6578 742e 2044 6566 6175 6c74 2033   text. Default 3
-0002fb20: 302e 0a20 2020 203a 7061 7261 6d20 4f70  0..    :param Op
-0002fb30: 7469 6f6e 616c 5b73 7472 5d20 666f 6e74  tional[str] font
-0002fb40: 5f63 6f6c 6f72 3a20 2046 6f6e 7420 636f  _color:  Font co
-0002fb50: 6c6f 7220 666f 7220 7465 7874 2e20 4465  lor for text. De
-0002fb60: 6661 756c 7420 7768 6974 650a 2020 2020  fault white.    
-0002fb70: 3a70 6172 616d 204f 7074 696f 6e61 6c5b  :param Optional[
-0002fb80: 7374 725d 2066 6f6e 745f 626f 7264 6572  str] font_border
-0002fb90: 5f63 6f6c 6f72 3a20 466f 6e74 2062 6f72  _color: Font bor
-0002fba0: 6465 7220 636f 6c6f 7220 666f 7220 7468  der color for th
-0002fbb0: 6520 7465 7874 2e20 4465 6661 756c 7420  e text. Default 
-0002fbc0: 626c 6163 6b2e 0a20 2020 203a 7061 7261  black..    :para
-0002fbd0: 6d20 4f70 7469 6f6e 616c 5b69 6e74 5d20  m Optional[int] 
-0002fbe0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
-0002fbf0: 683a 2046 6f6e 7420 626f 7264 6572 2077  h: Font border w
-0002fc00: 6964 7468 2066 6f72 2074 6865 2074 6578  idth for the tex
-0002fc10: 7420 696e 2070 6978 656c 732e 2044 6566  t in pixels. Def
-0002fc20: 6175 6c74 2032 2e0a 2020 2020 3a70 6172  ault 2..    :par
-0002fc30: 616d 204f 7074 696f 6e61 6c5b 4c69 7465  am Optional[Lite
-0002fc40: 7261 6c5b 2774 6f70 5f6c 6566 7427 2c20  ral['top_left', 
-0002fc50: 2774 6f70 5f72 6967 6874 272c 2027 626f  'top_right', 'bo
-0002fc60: 7474 6f6d 5f6c 6566 7427 2c20 2762 6f74  ttom_left', 'bot
-0002fc70: 746f 6d5f 7269 6768 7427 2c20 2774 6f70  tom_right', 'top
-0002fc80: 5f6d 6964 646c 6527 2c20 2762 6f74 746f  _middle', 'botto
-0002fc90: 6d5f 6d69 6464 6c65 275d 5d20 706f 7369  m_middle']] posi
-0002fca0: 7469 6f6e 3a20 506f 7369 7469 6f6e 2077  tion: Position w
-0002fcb0: 6865 7265 2074 6865 2074 6578 7420 7769  here the text wi
-0002fcc0: 6c6c 2062 6520 7375 7065 7269 6d70 6f73  ll be superimpos
-0002fcd0: 6564 2e20 4465 6661 756c 7420 6060 746f  ed. Default ``to
-0002fce0: 705f 6c65 6674 6060 2e0a 2020 2020 3a70  p_left``..    :p
-0002fcf0: 6172 616d 204f 7074 696f 6e61 6c5b 556e  aram Optional[Un
-0002fd00: 696f 6e5b 7374 722c 206f 732e 5061 7468  ion[str, os.Path
-0002fd10: 4c69 6b65 5d5d 2073 6176 655f 6469 723a  Like]] save_dir:
-0002fd20: 2044 6972 6563 746f 7279 2077 6865 7265   Directory where
-0002fd30: 2074 6865 206d 6f64 6966 6965 6420 7669   the modified vi
-0002fd40: 6465 6f28 7329 2077 696c 6c20 6265 2073  deo(s) will be s
-0002fd50: 6176 6564 2e20 4966 206e 6f74 2070 726f  aved. If not pro
-0002fd60: 7669 6465 642c 2074 6865 2064 6972 6563  vided, the direc
-0002fd70: 746f 7279 206f 6620 7468 6520 696e 7075  tory of the inpu
-0002fd80: 7420 7669 6465 6f28 7329 2077 696c 6c20  t video(s) will 
-0002fd90: 6265 2075 7365 642e 0a20 2020 203a 7265  be used..    :re
-0002fda0: 7475 726e 3a20 4e6f 6e65 0a20 2020 2022  turn: None.    "
-0002fdb0: 2222 0a0a 2020 2020 6368 6563 6b5f 6666  ""..    check_ff
-0002fdc0: 6d70 6567 5f61 7661 696c 6162 6c65 2872  mpeg_available(r
-0002fdd0: 6169 7365 5f65 7272 6f72 3d54 7275 6529  aise_error=True)
-0002fde0: 0a20 2020 2074 696d 6572 203d 2053 696d  .    timer = Sim
-0002fdf0: 6261 5469 6d65 7228 7374 6172 743d 5472  baTimer(start=Tr
-0002fe00: 7565 290a 2020 2020 504f 5349 5449 4f4e  ue).    POSITION
-0002fe10: 5320 3d20 5b27 746f 705f 6c65 6674 272c  S = ['top_left',
-0002fe20: 2027 746f 705f 7269 6768 7427 2c20 2762   'top_right', 'b
-0002fe30: 6f74 746f 6d5f 6c65 6674 272c 2027 626f  ottom_left', 'bo
-0002fe40: 7474 6f6d 5f72 6967 6874 272c 2027 746f  ttom_right', 'to
-0002fe50: 705f 6d69 6464 6c65 272c 2027 626f 7474  p_middle', 'bott
-0002fe60: 6f6d 5f6d 6964 646c 6527 5d0a 2020 2020  om_middle'].    
-0002fe70: 6368 6563 6b5f 7374 7228 6e61 6d65 3d66  check_str(name=f
-0002fe80: 277b 7375 7065 7269 6d70 6f73 655f 6672  '{superimpose_fr
-0002fe90: 6565 7465 7874 2e5f 5f6e 616d 655f 5f7d  eetext.__name__}
-0002fea0: 2070 6f73 6974 696f 6e27 2c20 7661 6c75   position', valu
-0002feb0: 653d 706f 7369 7469 6f6e 2c20 6f70 7469  e=position, opti
-0002fec0: 6f6e 733d 504f 5349 5449 4f4e 5329 0a20  ons=POSITIONS). 
-0002fed0: 2020 2063 6865 636b 5f69 6e74 286e 616d     check_int(nam
-0002fee0: 653d 6627 7b73 7570 6572 696d 706f 7365  e=f'{superimpose
-0002fef0: 5f66 7265 6574 6578 742e 5f5f 6e61 6d65  _freetext.__name
-0002ff00: 5f5f 7d20 666f 6e74 5f73 697a 6527 2c20  __} font_size', 
-0002ff10: 7661 6c75 653d 666f 6e74 5f73 697a 652c  value=font_size,
-0002ff20: 206d 696e 5f76 616c 7565 3d31 290a 2020   min_value=1).  
-0002ff30: 2020 6368 6563 6b5f 696e 7428 6e61 6d65    check_int(name
-0002ff40: 3d66 277b 7375 7065 7269 6d70 6f73 655f  =f'{superimpose_
-0002ff50: 6672 6565 7465 7874 2e5f 5f6e 616d 655f  freetext.__name_
-0002ff60: 5f7d 2066 6f6e 745f 626f 7264 6572 5f77  _} font_border_w
-0002ff70: 6964 7468 272c 2076 616c 7565 3d66 6f6e  idth', value=fon
-0002ff80: 745f 626f 7264 6572 5f77 6964 7468 2c20  t_border_width, 
-0002ff90: 6d69 6e5f 7661 6c75 653d 3129 0a20 2020  min_value=1).   
-0002ffa0: 2063 6865 636b 5f73 7472 286e 616d 653d   check_str(name=
-0002ffb0: 6627 7b73 7570 6572 696d 706f 7365 5f66  f'{superimpose_f
-0002ffc0: 7265 6574 6578 742e 5f5f 6e61 6d65 5f5f  reetext.__name__
-0002ffd0: 7d20 7465 7874 272c 2076 616c 7565 3d74  } text', value=t
-0002ffe0: 6578 7429 0a20 2020 2066 6f6e 745f 6469  ext).    font_di
-0002fff0: 6374 203d 2067 6574 5f66 6f6e 7473 2829  ct = get_fonts()
-00030000: 0a20 2020 2063 6865 636b 5f73 7472 286e  .    check_str(n
-00030010: 616d 653d 2766 6f6e 7427 2c20 7661 6c75  ame='font', valu
-00030020: 653d 666f 6e74 2c20 6f70 7469 6f6e 733d  e=font, options=
-00030030: 7475 706c 6528 666f 6e74 5f64 6963 742e  tuple(font_dict.
-00030040: 6b65 7973 2829 2929 0a20 2020 2066 6f6e  keys())).    fon
-00030050: 745f 7061 7468 203d 2066 6f6e 745f 6469  t_path = font_di
-00030060: 6374 5b66 6f6e 745d 0a20 2020 2066 6f6e  ct[font].    fon
-00030070: 745f 636f 6c6f 7220 3d20 2727 2e6a 6f69  t_color = ''.joi
-00030080: 6e28 6669 6c74 6572 2873 7472 2e69 7361  n(filter(str.isa
-00030090: 6c6e 756d 2c20 666f 6e74 5f63 6f6c 6f72  lnum, font_color
-000300a0: 2929 2e6c 6f77 6572 2829 0a20 2020 2066  )).lower().    f
-000300b0: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
-000300c0: 203d 2027 272e 6a6f 696e 2866 696c 7465   = ''.join(filte
-000300d0: 7228 7374 722e 6973 616c 6e75 6d2c 2066  r(str.isalnum, f
-000300e0: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
-000300f0: 2929 2e6c 6f77 6572 2829 0a20 2020 2069  )).lower().    i
-00030100: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
-00030110: 2876 6964 656f 5f70 6174 6829 3a0a 2020  (video_path):.  
-00030120: 2020 2020 2020 7669 6465 6f5f 7061 7468        video_path
-00030130: 7320 3d20 5b76 6964 656f 5f70 6174 685d  s = [video_path]
-00030140: 0a20 2020 2065 6c69 6620 6f73 2e70 6174  .    elif os.pat
-00030150: 682e 6973 6469 7228 7669 6465 6f5f 7061  h.isdir(video_pa
-00030160: 7468 293a 0a20 2020 2020 2020 2076 6964  th):.        vid
-00030170: 656f 5f70 6174 6873 203d 206c 6973 7428  eo_paths = list(
-00030180: 6669 6e64 5f61 6c6c 5f76 6964 656f 735f  find_all_videos_
-00030190: 696e 5f64 6972 6563 746f 7279 2864 6972  in_directory(dir
-000301a0: 6563 746f 7279 3d76 6964 656f 5f70 6174  ectory=video_pat
-000301b0: 682c 2061 735f 6469 6374 3d54 7275 652c  h, as_dict=True,
-000301c0: 2072 6169 7365 5f65 7272 6f72 3d54 7275   raise_error=Tru
-000301d0: 6529 2e76 616c 7565 7328 2929 0a20 2020  e).values()).   
-000301e0: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-000301f0: 6169 7365 2049 6e76 616c 6964 496e 7075  aise InvalidInpu
-00030200: 7445 7272 6f72 286d 7367 3d66 277b 7669  tError(msg=f'{vi
-00030210: 6465 6f5f 7061 7468 7d20 6973 206e 6f74  deo_path} is not
-00030220: 2061 2076 616c 6964 2066 696c 6520 7061   a valid file pa
-00030230: 7468 206f 7220 6120 7661 6c69 6420 6469  th or a valid di
-00030240: 7265 6374 6f72 7920 7061 7468 272c 2073  rectory path', s
-00030250: 6f75 7263 653d 7375 7065 7269 6d70 6f73  ource=superimpos
-00030260: 655f 7669 6465 6f5f 6e61 6d65 732e 5f5f  e_video_names.__
-00030270: 6e61 6d65 5f5f 290a 2020 2020 6966 2073  name__).    if s
-00030280: 6176 655f 6469 7220 6973 206e 6f74 204e  ave_dir is not N
-00030290: 6f6e 653a 0a20 2020 2020 2020 2063 6865  one:.        che
-000302a0: 636b 5f69 665f 6469 725f 6578 6973 7473  ck_if_dir_exists
-000302b0: 2869 6e5f 6469 723d 7361 7665 5f64 6972  (in_dir=save_dir
-000302c0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-000302d0: 2020 2020 7361 7665 5f64 6972 203d 206f      save_dir = o
-000302e0: 732e 7061 7468 2e64 6972 6e61 6d65 2876  s.path.dirname(v
-000302f0: 6964 656f 5f70 6174 6873 5b30 5d29 0a20  ideo_paths[0]). 
-00030300: 2020 2066 6f72 2066 696c 655f 636e 742c     for file_cnt,
-00030310: 2076 6964 656f 5f70 6174 6820 696e 2065   video_path in e
-00030320: 6e75 6d65 7261 7465 2876 6964 656f 5f70  numerate(video_p
-00030330: 6174 6873 293a 0a20 2020 2020 2020 205f  aths):.        _
-00030340: 2c20 7669 6465 6f5f 6e61 6d65 2c20 6578  , video_name, ex
-00030350: 7420 3d20 6765 745f 666e 5f65 7874 2876  t = get_fn_ext(v
-00030360: 6964 656f 5f70 6174 6829 0a20 2020 2020  ideo_path).     
-00030370: 2020 2070 7269 6e74 2866 2753 7570 6572     print(f'Super
-00030380: 696d 706f 7369 6e67 2076 6964 656f 206e  imposing video n
-00030390: 616d 6520 6f6e 207b 7669 6465 6f5f 6e61  ame on {video_na
-000303a0: 6d65 7d20 2856 6964 656f 207b 6669 6c65  me} (Video {file
-000303b0: 5f63 6e74 202b 2031 7d2f 7b6c 656e 2876  _cnt + 1}/{len(v
-000303c0: 6964 656f 5f70 6174 6873 297d 292e 2e2e  ideo_paths)})...
-000303d0: 2729 0a20 2020 2020 2020 2073 6176 655f  ').        save_
-000303e0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-000303f0: 6f69 6e28 7361 7665 5f64 6972 2c20 6627  oin(save_dir, f'
-00030400: 7b76 6964 656f 5f6e 616d 657d 5f74 6578  {video_name}_tex
-00030410: 745f 7375 7065 7269 6d70 6f73 6564 7b65  t_superimposed{e
-00030420: 7874 7d27 290a 2020 2020 2020 2020 6966  xt}').        if
-00030430: 2070 6f73 6974 696f 6e20 3d3d 2050 4f53   position == POS
-00030440: 4954 494f 4e53 5b30 5d3a 0a20 2020 2020  ITIONS[0]:.     
-00030450: 2020 2020 2020 2063 6d64 203d 2066 2266         cmd = f"f
-00030460: 666d 7065 6720 2d69 2027 7b76 6964 656f  fmpeg -i '{video
-00030470: 5f70 6174 687d 2720 2d76 6620 5c22 6472  _path}' -vf \"dr
-00030480: 6177 7465 7874 3d66 6f6e 7466 696c 653d  awtext=fontfile=
-00030490: 7b66 6f6e 745f 7061 7468 7d3a 7465 7874  {font_path}:text
-000304a0: 3d7b 7465 7874 7d3a 783d 353a 793d 353a  ={text}:x=5:y=5:
-000304b0: 666f 6e74 7369 7a65 3d7b 666f 6e74 5f73  fontsize={font_s
-000304c0: 697a 657d 3a66 6f6e 7463 6f6c 6f72 3d7b  ize}:fontcolor={
-000304d0: 666f 6e74 5f63 6f6c 6f72 7d3a 626f 7264  font_color}:bord
-000304e0: 6572 773d 7b66 6f6e 745f 626f 7264 6572  erw={font_border
-000304f0: 5f77 6964 7468 7d3a 626f 7264 6572 636f  _width}:borderco
-00030500: 6c6f 723d 7b66 6f6e 745f 626f 7264 6572  lor={font_border
-00030510: 5f63 6f6c 6f72 7d5c 2220 2d63 3a61 2063  _color}\" -c:a c
-00030520: 6f70 7920 277b 7361 7665 5f70 6174 687d  opy '{save_path}
-00030530: 2720 2d6c 6f67 6c65 7665 6c20 6572 726f  ' -loglevel erro
-00030540: 7220 2d73 7461 7473 202d 6869 6465 5f62  r -stats -hide_b
-00030550: 616e 6e65 7220 2d79 220a 2020 2020 2020  anner -y".      
-00030560: 2020 656c 6966 2070 6f73 6974 696f 6e20    elif position 
-00030570: 3d3d 2050 4f53 4954 494f 4e53 5b31 5d3a  == POSITIONS[1]:
-00030580: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
-00030590: 203d 2066 2266 666d 7065 6720 2d69 2027   = f"ffmpeg -i '
-000305a0: 7b76 6964 656f 5f70 6174 687d 2720 2d76  {video_path}' -v
-000305b0: 6620 5c22 6472 6177 7465 7874 3d66 6f6e  f \"drawtext=fon
-000305c0: 7466 696c 653d 7b66 6f6e 745f 7061 7468  tfile={font_path
-000305d0: 7d3a 7465 7874 3d7b 7465 7874 7d3a 783d  }:text={text}:x=
-000305e0: 2877 2d74 772d 3529 3a79 3d35 3a66 6f6e  (w-tw-5):y=5:fon
-000305f0: 7473 697a 653d 7b66 6f6e 745f 7369 7a65  tsize={font_size
-00030600: 7d3a 666f 6e74 636f 6c6f 723d 7b66 6f6e  }:fontcolor={fon
-00030610: 745f 636f 6c6f 727d 3a62 6f72 6465 7277  t_color}:borderw
-00030620: 3d7b 666f 6e74 5f62 6f72 6465 725f 7769  ={font_border_wi
-00030630: 6474 687d 3a62 6f72 6465 7263 6f6c 6f72  dth}:bordercolor
-00030640: 3d7b 666f 6e74 5f62 6f72 6465 725f 636f  ={font_border_co
-00030650: 6c6f 727d 5c22 202d 633a 6120 636f 7079  lor}\" -c:a copy
-00030660: 2027 7b73 6176 655f 7061 7468 7d27 202d   '{save_path}' -
-00030670: 6c6f 676c 6576 656c 2065 7272 6f72 202d  loglevel error -
-00030680: 7374 6174 7320 2d68 6964 655f 6261 6e6e  stats -hide_bann
-00030690: 6572 202d 7922 0a20 2020 2020 2020 2065  er -y".        e
-000306a0: 6c69 6620 706f 7369 7469 6f6e 203d 3d20  lif position == 
-000306b0: 504f 5349 5449 4f4e 535b 325d 3a0a 2020  POSITIONS[2]:.  
-000306c0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-000306d0: 6622 6666 6d70 6567 202d 6920 277b 7669  f"ffmpeg -i '{vi
-000306e0: 6465 6f5f 7061 7468 7d27 202d 7666 205c  deo_path}' -vf \
-000306f0: 2264 7261 7774 6578 743d 666f 6e74 6669  "drawtext=fontfi
-00030700: 6c65 3d7b 666f 6e74 5f70 6174 687d 3a74  le={font_path}:t
-00030710: 6578 743d 7b74 6578 747d 3a78 3d35 3a79  ext={text}:x=5:y
-00030720: 3d28 682d 7468 2d35 293a 666f 6e74 7369  =(h-th-5):fontsi
-00030730: 7a65 3d7b 666f 6e74 5f73 697a 657d 3a66  ze={font_size}:f
-00030740: 6f6e 7463 6f6c 6f72 3d7b 666f 6e74 5f63  ontcolor={font_c
-00030750: 6f6c 6f72 7d3a 626f 7264 6572 773d 7b66  olor}:borderw={f
-00030760: 6f6e 745f 626f 7264 6572 5f77 6964 7468  ont_border_width
-00030770: 7d3a 626f 7264 6572 636f 6c6f 723d 7b66  }:bordercolor={f
-00030780: 6f6e 745f 626f 7264 6572 5f63 6f6c 6f72  ont_border_color
-00030790: 7d5c 2220 2d63 3a61 2063 6f70 7920 277b  }\" -c:a copy '{
-000307a0: 7361 7665 5f70 6174 687d 2720 2d6c 6f67  save_path}' -log
-000307b0: 6c65 7665 6c20 6572 726f 7220 2d73 7461  level error -sta
-000307c0: 7473 202d 6869 6465 5f62 616e 6e65 7220  ts -hide_banner 
-000307d0: 2d79 220a 2020 2020 2020 2020 656c 6966  -y".        elif
-000307e0: 2070 6f73 6974 696f 6e20 3d3d 2050 4f53   position == POS
-000307f0: 4954 494f 4e53 5b33 5d3a 0a20 2020 2020  ITIONS[3]:.     
-00030800: 2020 2020 2020 2063 6d64 203d 2066 2266         cmd = f"f
-00030810: 666d 7065 6720 2d69 2027 7b76 6964 656f  fmpeg -i '{video
-00030820: 5f70 6174 687d 2720 2d76 6620 5c22 6472  _path}' -vf \"dr
-00030830: 6177 7465 7874 3d66 6f6e 7466 696c 653d  awtext=fontfile=
-00030840: 7b66 6f6e 745f 7061 7468 7d3a 7465 7874  {font_path}:text
-00030850: 3d7b 7465 7874 7d3a 783d 2877 2d74 772d  ={text}:x=(w-tw-
-00030860: 3529 3a79 3d28 682d 7468 2d35 293a 666f  5):y=(h-th-5):fo
-00030870: 6e74 7369 7a65 3d7b 666f 6e74 5f73 697a  ntsize={font_siz
-00030880: 657d 3a66 6f6e 7463 6f6c 6f72 3d7b 666f  e}:fontcolor={fo
-00030890: 6e74 5f63 6f6c 6f72 7d3a 626f 7264 6572  nt_color}:border
-000308a0: 773d 7b66 6f6e 745f 626f 7264 6572 5f77  w={font_border_w
-000308b0: 6964 7468 7d3a 626f 7264 6572 636f 6c6f  idth}:bordercolo
-000308c0: 723d 7b66 6f6e 745f 626f 7264 6572 5f63  r={font_border_c
-000308d0: 6f6c 6f72 7d5c 2220 2d63 3a61 2063 6f70  olor}\" -c:a cop
-000308e0: 7920 277b 7361 7665 5f70 6174 687d 2720  y '{save_path}' 
-000308f0: 2d6c 6f67 6c65 7665 6c20 6572 726f 7220  -loglevel error 
-00030900: 2d73 7461 7473 202d 6869 6465 5f62 616e  -stats -hide_ban
-00030910: 6e65 7220 2d79 220a 2020 2020 2020 2020  ner -y".        
-00030920: 656c 6966 2070 6f73 6974 696f 6e20 3d3d  elif position ==
-00030930: 2050 4f53 4954 494f 4e53 5b34 5d3a 0a20   POSITIONS[4]:. 
-00030940: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00030950: 2066 2266 666d 7065 6720 2d69 2027 7b76   f"ffmpeg -i '{v
-00030960: 6964 656f 5f70 6174 687d 2720 2d76 6620  ideo_path}' -vf 
-00030970: 5c22 6472 6177 7465 7874 3d66 6f6e 7466  \"drawtext=fontf
-00030980: 696c 653d 7b66 6f6e 745f 7061 7468 7d3a  ile={font_path}:
-00030990: 7465 7874 3d7b 7465 7874 7d3a 783d 2877  text={text}:x=(w
-000309a0: 2d74 7729 2f32 3a79 3d31 303a 666f 6e74  -tw)/2:y=10:font
-000309b0: 7369 7a65 3d7b 666f 6e74 5f73 697a 657d  size={font_size}
-000309c0: 3a66 6f6e 7463 6f6c 6f72 3d7b 666f 6e74  :fontcolor={font
-000309d0: 5f63 6f6c 6f72 7d3a 626f 7264 6572 773d  _color}:borderw=
-000309e0: 7b66 6f6e 745f 626f 7264 6572 5f77 6964  {font_border_wid
-000309f0: 7468 7d3a 626f 7264 6572 636f 6c6f 723d  th}:bordercolor=
-00030a00: 7b66 6f6e 745f 626f 7264 6572 5f63 6f6c  {font_border_col
-00030a10: 6f72 7d5c 2220 2d63 3a61 2063 6f70 7920  or}\" -c:a copy 
-00030a20: 277b 7361 7665 5f70 6174 687d 2720 2d6c  '{save_path}' -l
-00030a30: 6f67 6c65 7665 6c20 6572 726f 7220 2d73  oglevel error -s
-00030a40: 7461 7473 202d 6869 6465 5f62 616e 6e65  tats -hide_banne
-00030a50: 7220 2d79 220a 2020 2020 2020 2020 656c  r -y".        el
-00030a60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00030a70: 636d 6420 3d20 6622 6666 6d70 6567 202d  cmd = f"ffmpeg -
-00030a80: 6920 277b 7669 6465 6f5f 7061 7468 7d27  i '{video_path}'
-00030a90: 202d 7666 205c 2264 7261 7774 6578 743d   -vf \"drawtext=
-00030aa0: 666f 6e74 6669 6c65 3d7b 666f 6e74 5f70  fontfile={font_p
-00030ab0: 6174 687d 3a74 6578 743d 7b74 6578 747d  ath}:text={text}
-00030ac0: 3a78 3d28 772d 7477 292f 323a 793d 2868  :x=(w-tw)/2:y=(h
-00030ad0: 2d74 682d 3130 293a 666f 6e74 7369 7a65  -th-10):fontsize
-00030ae0: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
-00030af0: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
-00030b00: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
-00030b10: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
-00030b20: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
-00030b30: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
-00030b40: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
-00030b50: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
-00030b60: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
-00030b70: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
-00030b80: 220a 2020 2020 2020 2020 7375 6270 726f  ".        subpro
-00030b90: 6365 7373 2e63 616c 6c28 636d 642c 2073  cess.call(cmd, s
-00030ba0: 6865 6c6c 3d54 7275 652c 2073 7464 6f75  hell=True, stdou
-00030bb0: 743d 7375 6270 726f 6365 7373 2e50 4950  t=subprocess.PIP
-00030bc0: 4529 0a20 2020 2074 696d 6572 2e73 746f  E).    timer.sto
-00030bd0: 705f 7469 6d65 7228 290a 2020 2020 7374  p_timer().    st
-00030be0: 646f 7574 5f73 7563 6365 7373 286d 7367  dout_success(msg
-00030bf0: 3d66 2753 7570 6572 2d69 6d70 6f73 6564  =f'Super-imposed
-00030c00: 2066 7265 652d 7465 7874 206f 6e20 7b6c   free-text on {l
-00030c10: 656e 2876 6964 656f 5f70 6174 6873 297d  en(video_paths)}
-00030c20: 2076 6964 656f 2873 292c 2073 6176 6564   video(s), saved
-00030c30: 2069 6e20 7b73 6176 655f 6469 727d 272c   in {save_dir}',
-00030c40: 2065 6c61 7073 6564 5f74 696d 653d 7469   elapsed_time=ti
-00030c50: 6d65 722e 656c 6170 7365 645f 7469 6d65  mer.elapsed_time
-00030c60: 5f73 7472 290a 0a0a 2320 7669 6465 6f5f  _str)...# video_
-00030c70: 7061 7468 7320 3d20 5b27 2f55 7365 7273  paths = ['/Users
-00030c80: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-00030c90: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-00030ca0: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-00030cb0: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-00030cc0: 6c64 6572 2f6d 6572 6765 2f54 7269 616c  lder/merge/Trial
-00030cd0: 2020 2020 3130 5f63 6c69 7070 6564 5f67      10_clipped_g
-00030ce0: 616e 7474 2e6d 7034 272c 0a23 2020 2020  antt.mp4',.#    
-00030cf0: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
-00030d00: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
-00030d10: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
-00030d20: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
-00030d30: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
-00030d40: 5f66 6f6c 6465 722f 6d65 7267 652f 5472  _folder/merge/Tr
-00030d50: 6961 6c20 2020 2031 305f 636c 6970 7065  ial    10_clippe
-00030d60: 642e 6d70 3427 2c0a 2320 2020 2020 2020  d.mp4',.#       
-00030d70: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
-00030d80: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-00030d90: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-00030da0: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-00030db0: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-00030dc0: 6c64 6572 2f6d 6572 6765 2f54 7269 616c  lder/merge/Trial
-00030dd0: 2020 2020 3130 5f63 6c69 7070 6564 5f6c      10_clipped_l
-00030de0: 696e 652e 6d70 3427 2c0a 2320 2020 2020  ine.mp4',.#     
-00030df0: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
-00030e00: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
-00030e10: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
-00030e20: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
-00030e30: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
-00030e40: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
-00030e50: 616c 2020 2020 2033 5f63 6c69 7070 6564  al     3_clipped
-00030e60: 2e6d 7034 275d 0a23 0a23 2076 6964 656f  .mp4'].#.# video
-00030e70: 5f70 6174 6873 203d 205b 272f 5573 6572  _paths = ['/User
-00030e80: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
-00030e90: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
-00030ea0: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
-00030eb0: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
-00030ec0: 6f6c 6465 722f 7669 6465 6f73 2f54 7269  older/videos/Tri
-00030ed0: 616c 2020 2020 3130 2e6d 7034 272c 0a23  al    10.mp4',.#
-00030ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00030ef0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
-00030f00: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
-00030f10: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
-00030f20: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
-00030f30: 6a65 6374 5f66 6f6c 6465 722f 6d65 7267  ject_folder/merg
-00030f40: 652f 5472 6961 6c20 2020 2031 305f 636c  e/Trial    10_cl
-00030f50: 6970 7065 645f 6761 6e74 742e 6d70 3427  ipped_gantt.mp4'
-00030f60: 2c0a 2320 2020 2020 2020 2020 2020 2020  ,.#             
-00030f70: 2020 2027 2f55 7365 7273 2f73 696d 6f6e     '/Users/simon
-00030f80: 2f44 6573 6b74 6f70 2f65 6e76 732f 7369  /Desktop/envs/si
-00030f90: 6d62 612f 7472 6f75 626c 6573 686f 6f74  mba/troubleshoot
-00030fa0: 696e 672f 6265 6570 626f 6f70 3137 342f  ing/beepboop174/
-00030fb0: 7072 6f6a 6563 745f 666f 6c64 6572 2f6d  project_folder/m
-00030fc0: 6572 6765 2f54 7269 616c 2020 2020 3130  erge/Trial    10
-00030fd0: 5f63 6c69 7070 6564 5f6c 696e 652e 6d70  _clipped_line.mp
-00030fe0: 3427 2c0a 2320 2020 2020 2020 2020 2020  4',.#           
-00030ff0: 2020 2020 2027 2f55 7365 7273 2f73 696d       '/Users/sim
-00031000: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
-00031010: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
-00031020: 6f74 696e 672f 6265 6570 626f 6f70 3137  oting/beepboop17
-00031030: 342f 7072 6f6a 6563 745f 666f 6c64 6572  4/project_folder
-00031040: 2f6d 6572 6765 2f54 7269 616c 2020 2020  /merge/Trial    
-00031050: 2033 5f63 6c69 7070 6564 2e6d 7034 275d   3_clipped.mp4']
-00031060: 0a23 0a23 2073 6176 655f 7061 7468 203d  .#.# save_path =
-00031070: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
-00031080: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-00031090: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-000310a0: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-000310b0: 6f6a 6563 745f 666f 6c64 6572 2f6d 6572  oject_folder/mer
-000310c0: 6765 2f6f 7574 2e6d 7034 270a 0a23 0a23  ge/out.mp4'..#.#
-000310d0: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
-000310e0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
-000310f0: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
-00031100: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
-00031110: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
-00031120: 6a65 6374 5f66 6f6c 6465 722f 6672 616d  ject_folder/fram
-00031130: 6573 2f6f 7574 7075 742f 6761 6e74 745f  es/output/gantt_
-00031140: 706c 6f74 732f 5472 6961 6c20 2020 2031  plots/Trial    1
-00031150: 302e 6d70 3427 2c0a 2320 2020 2020 2020  0.mp4',.#       
-00031160: 2020 2020 2020 2020 2027 2f55 7365 7273           '/Users
-00031170: 2f73 696d 6f6e 2f44 6573 6b74 6f70 2f65  /simon/Desktop/e
-00031180: 6e76 732f 7369 6d62 612f 7472 6f75 626c  nvs/simba/troubl
-00031190: 6573 686f 6f74 696e 672f 6265 6570 626f  eshooting/beepbo
-000311a0: 6f70 3137 342f 7072 6f6a 6563 745f 666f  op174/project_fo
-000311b0: 6c64 6572 2f76 6964 656f 732f 5472 6961  lder/videos/Tria
-000311c0: 6c20 2020 2031 302e 6d70 3427 2c0a 2320  l    10.mp4',.# 
-000311d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000311e0: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
-000311f0: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
-00031200: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
-00031210: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
-00031220: 6563 745f 666f 6c64 6572 2f66 7261 6d65  ect_folder/frame
-00031230: 732f 6f75 7470 7574 2f6c 696e 655f 706c  s/output/line_pl
-00031240: 6f74 2f54 7269 616c 2020 2020 3130 2e6d  ot/Trial    10.m
-00031250: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
-00031260: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
-00031270: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
-00031280: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
-00031290: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
-000312a0: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
-000312b0: 722f 6672 616d 6573 2f6f 7574 7075 742f  r/frames/output/
-000312c0: 6c69 6e65 5f70 6c6f 742f 5472 6961 6c20  line_plot/Trial 
-000312d0: 2020 2020 332e 6d70 3427 5d0a 2320 7361      3.mp4'].# sa
-000312e0: 7665 5f70 6174 6820 3d20 272f 5573 6572  ve_path = '/User
-000312f0: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
-00031300: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
-00031310: 6c65 7368 6f6f 7469 6e67 2f52 4154 5f4e  leshooting/RAT_N
-00031320: 4f52 2f70 726f 6a65 6374 5f66 6f6c 6465  OR/project_folde
-00031330: 722f 7669 6465 6f73 2f74 6573 742f 6e65  r/videos/test/ne
-00031340: 772f 626c 616e 6b5f 7465 7374 2e6d 7034  w/blank_test.mp4
-00031350: 270a 0a23 2076 6964 656f 5f70 6174 6873  '..# video_paths
-00031360: 203d 205b 272f 5573 6572 732f 7369 6d6f   = ['/Users/simo
-00031370: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
-00031380: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
-00031390: 7469 6e67 2f62 6565 7062 6f6f 7031 3734  ting/beepboop174
-000313a0: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
-000313b0: 7669 6465 6f73 2f54 7269 616c 2020 2020  videos/Trial    
-000313c0: 3130 2e6d 7034 272c 0a23 2020 2020 2020  10.mp4',.#      
-000313d0: 2020 2020 2020 2020 2020 272f 5573 6572            '/User
-000313e0: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
-000313f0: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
-00031400: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
-00031410: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
-00031420: 6f6c 6465 722f 6672 616d 6573 2f6f 7574  older/frames/out
-00031430: 7075 742f 6c69 6e65 5f70 6c6f 742f 5472  put/line_plot/Tr
-00031440: 6961 6c20 2020 2031 302e 6d70 3427 2c0a  ial    10.mp4',.
-00031450: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-00031460: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
-00031470: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
-00031480: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
-00031490: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
-000314a0: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
-000314b0: 6d65 732f 6f75 7470 7574 2f6c 696e 655f  mes/output/line_
-000314c0: 706c 6f74 2f54 7269 616c 2020 2020 2033  plot/Trial     3
-000314d0: 2e6d 7034 275d 0a0a 2320 6d69 7865 645f  .mp4']..# mixed_
-000314e0: 6d6f 7361 6963 5f63 6f6e 6361 7465 6e61  mosaic_concatena
-000314f0: 746f 7228 7669 6465 6f5f 7061 7468 733d  tor(video_paths=
-00031500: 7669 6465 6f5f 7061 7468 732c 2073 6176  video_paths, sav
-00031510: 655f 7061 7468 3d73 6176 655f 7061 7468  e_path=save_path
-00031520: 2c20 6770 753d 4661 6c73 652c 2076 6572  , gpu=False, ver
-00031530: 626f 7365 3d54 7275 6529 0a              bose=True).
+0002f860: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
+0002f870: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
+0002f880: 203d 2032 2c0a 2020 2020 2020 2020 2020   = 2,.          
+0002f890: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0002f8a0: 6f73 6974 696f 6e3a 204f 7074 696f 6e61  osition: Optiona
+0002f8b0: 6c5b 4c69 7465 7261 6c5b 2774 6f70 5f6c  l[Literal['top_l
+0002f8c0: 6566 7427 2c20 2774 6f70 5f72 6967 6874  eft', 'top_right
+0002f8d0: 272c 2027 626f 7474 6f6d 5f6c 6566 7427  ', 'bottom_left'
+0002f8e0: 2c20 2762 6f74 746f 6d5f 7269 6768 7427  , 'bottom_right'
+0002f8f0: 2c20 276d 6964 646c 655f 746f 7027 2c20  , 'middle_top', 
+0002f900: 276d 6964 646c 655f 626f 7474 6f6d 275d  'middle_bottom']
+0002f910: 5d20 3d20 2774 6f70 5f6c 6566 7427 2c0a  ] = 'top_left',.
+0002f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f930: 2020 2020 2020 2020 2073 6176 655f 6469           save_di
+0002f940: 723a 204f 7074 696f 6e61 6c5b 556e 696f  r: Optional[Unio
+0002f950: 6e5b 7374 722c 206f 732e 5061 7468 4c69  n[str, os.PathLi
+0002f960: 6b65 5d5d 203d 204e 6f6e 6529 202d 3e20  ke]] = None) -> 
+0002f970: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+0002f980: 2020 5375 7065 7269 6d70 6f73 6573 2070    Superimposes p
+0002f990: 6173 7365 6420 7465 7874 206f 6e20 7468  assed text on th
+0002f9a0: 6520 6769 7665 6e20 7669 6465 6f20 6669  e given video fi
+0002f9b0: 6c65 2873 2920 616e 6420 7361 7665 7320  le(s) and saves 
+0002f9c0: 7468 6520 6d6f 6469 6669 6564 2076 6964  the modified vid
+0002f9d0: 656f 2873 292e 0a0a 2020 2020 2e2e 2076  eo(s)...    .. v
+0002f9e0: 6964 656f 3a3a 205f 7374 6174 6963 2f69  ideo:: _static/i
+0002f9f0: 6d67 2f73 7570 6572 696d 706f 7365 5f66  mg/superimpose_f
+0002fa00: 7265 6574 6578 742e 7765 626d 0a20 2020  reetext.webm.   
+0002fa10: 2020 2020 3a77 6964 7468 3a20 3930 300a      :width: 900.
+0002fa20: 2020 2020 2020 203a 6c6f 6f70 3a0a 0a20         :loop:.. 
+0002fa30: 2020 203a 7061 7261 6d20 556e 696f 6e5b     :param Union[
+0002fa40: 7374 722c 206f 732e 5061 7468 4c69 6b65  str, os.PathLike
+0002fa50: 5d20 7669 6465 6f5f 7061 7468 3a20 5061  ] video_path: Pa
+0002fa60: 7468 2074 6f20 7468 6520 696e 7075 7420  th to the input 
+0002fa70: 7669 6465 6f20 6669 6c65 206f 7220 6469  video file or di
+0002fa80: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
+0002fa90: 6e67 2076 6964 656f 2066 696c 6573 2e0a  ng video files..
+0002faa0: 2020 2020 3a70 6172 616d 2073 7472 2074      :param str t
+0002fab0: 6578 743a 2054 6865 2074 6578 7420 746f  ext: The text to
+0002fac0: 206f 7665 726c 6179 206f 6e20 7468 6520   overlay on the 
+0002fad0: 7669 6465 6f0a 2020 2020 3a70 6172 616d  video.    :param
+0002fae0: 204f 7074 696f 6e61 6c5b 696e 745d 2066   Optional[int] f
+0002faf0: 6f6e 745f 7369 7a65 3a20 466f 6e74 2073  ont_size: Font s
+0002fb00: 697a 6520 666f 7220 7468 6520 7465 7874  ize for the text
+0002fb10: 2e20 4465 6661 756c 7420 3330 2e0a 2020  . Default 30..  
+0002fb20: 2020 3a70 6172 616d 204f 7074 696f 6e61    :param Optiona
+0002fb30: 6c5b 7374 725d 2066 6f6e 745f 636f 6c6f  l[str] font_colo
+0002fb40: 723a 2020 466f 6e74 2063 6f6c 6f72 2066  r:  Font color f
+0002fb50: 6f72 2074 6578 742e 2044 6566 6175 6c74  or text. Default
+0002fb60: 2077 6869 7465 0a20 2020 203a 7061 7261   white.    :para
+0002fb70: 6d20 4f70 7469 6f6e 616c 5b73 7472 5d20  m Optional[str] 
+0002fb80: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
+0002fb90: 723a 2046 6f6e 7420 626f 7264 6572 2063  r: Font border c
+0002fba0: 6f6c 6f72 2066 6f72 2074 6865 2074 6578  olor for the tex
+0002fbb0: 742e 2044 6566 6175 6c74 2062 6c61 636b  t. Default black
+0002fbc0: 2e0a 2020 2020 3a70 6172 616d 204f 7074  ..    :param Opt
+0002fbd0: 696f 6e61 6c5b 696e 745d 2066 6f6e 745f  ional[int] font_
+0002fbe0: 626f 7264 6572 5f77 6964 7468 3a20 466f  border_width: Fo
+0002fbf0: 6e74 2062 6f72 6465 7220 7769 6474 6820  nt border width 
+0002fc00: 666f 7220 7468 6520 7465 7874 2069 6e20  for the text in 
+0002fc10: 7069 7865 6c73 2e20 4465 6661 756c 7420  pixels. Default 
+0002fc20: 322e 0a20 2020 203a 7061 7261 6d20 4f70  2..    :param Op
+0002fc30: 7469 6f6e 616c 5b4c 6974 6572 616c 5b27  tional[Literal['
+0002fc40: 746f 705f 6c65 6674 272c 2027 746f 705f  top_left', 'top_
+0002fc50: 7269 6768 7427 2c20 2762 6f74 746f 6d5f  right', 'bottom_
+0002fc60: 6c65 6674 272c 2027 626f 7474 6f6d 5f72  left', 'bottom_r
+0002fc70: 6967 6874 272c 2027 746f 705f 6d69 6464  ight', 'top_midd
+0002fc80: 6c65 272c 2027 626f 7474 6f6d 5f6d 6964  le', 'bottom_mid
+0002fc90: 646c 6527 5d5d 2070 6f73 6974 696f 6e3a  dle']] position:
+0002fca0: 2050 6f73 6974 696f 6e20 7768 6572 6520   Position where 
+0002fcb0: 7468 6520 7465 7874 2077 696c 6c20 6265  the text will be
+0002fcc0: 2073 7570 6572 696d 706f 7365 642e 2044   superimposed. D
+0002fcd0: 6566 6175 6c74 2060 6074 6f70 5f6c 6566  efault ``top_lef
+0002fce0: 7460 602e 0a20 2020 203a 7061 7261 6d20  t``..    :param 
+0002fcf0: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+0002fd00: 7472 2c20 6f73 2e50 6174 684c 696b 655d  tr, os.PathLike]
+0002fd10: 5d20 7361 7665 5f64 6972 3a20 4469 7265  ] save_dir: Dire
+0002fd20: 6374 6f72 7920 7768 6572 6520 7468 6520  ctory where the 
+0002fd30: 6d6f 6469 6669 6564 2076 6964 656f 2873  modified video(s
+0002fd40: 2920 7769 6c6c 2062 6520 7361 7665 642e  ) will be saved.
+0002fd50: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+0002fd60: 2c20 7468 6520 6469 7265 6374 6f72 7920  , the directory 
+0002fd70: 6f66 2074 6865 2069 6e70 7574 2076 6964  of the input vid
+0002fd80: 656f 2873 2920 7769 6c6c 2062 6520 7573  eo(s) will be us
+0002fd90: 6564 2e0a 2020 2020 3a72 6574 7572 6e3a  ed..    :return:
+0002fda0: 204e 6f6e 650a 2020 2020 2222 220a 0a20   None.    """.. 
+0002fdb0: 2020 2063 6865 636b 5f66 666d 7065 675f     check_ffmpeg_
+0002fdc0: 6176 6169 6c61 626c 6528 7261 6973 655f  available(raise_
+0002fdd0: 6572 726f 723d 5472 7565 290a 2020 2020  error=True).    
+0002fde0: 7469 6d65 7220 3d20 5369 6d62 6154 696d  timer = SimbaTim
+0002fdf0: 6572 2873 7461 7274 3d54 7275 6529 0a20  er(start=True). 
+0002fe00: 2020 2050 4f53 4954 494f 4e53 203d 205b     POSITIONS = [
+0002fe10: 2774 6f70 5f6c 6566 7427 2c20 2774 6f70  'top_left', 'top
+0002fe20: 5f72 6967 6874 272c 2027 626f 7474 6f6d  _right', 'bottom
+0002fe30: 5f6c 6566 7427 2c20 2762 6f74 746f 6d5f  _left', 'bottom_
+0002fe40: 7269 6768 7427 2c20 2774 6f70 5f6d 6964  right', 'top_mid
+0002fe50: 646c 6527 2c20 2762 6f74 746f 6d5f 6d69  dle', 'bottom_mi
+0002fe60: 6464 6c65 275d 0a20 2020 2063 6865 636b  ddle'].    check
+0002fe70: 5f73 7472 286e 616d 653d 6627 7b73 7570  _str(name=f'{sup
+0002fe80: 6572 696d 706f 7365 5f66 7265 6574 6578  erimpose_freetex
+0002fe90: 742e 5f5f 6e61 6d65 5f5f 7d20 706f 7369  t.__name__} posi
+0002fea0: 7469 6f6e 272c 2076 616c 7565 3d70 6f73  tion', value=pos
+0002feb0: 6974 696f 6e2c 206f 7074 696f 6e73 3d50  ition, options=P
+0002fec0: 4f53 4954 494f 4e53 290a 2020 2020 6368  OSITIONS).    ch
+0002fed0: 6563 6b5f 696e 7428 6e61 6d65 3d66 277b  eck_int(name=f'{
+0002fee0: 7375 7065 7269 6d70 6f73 655f 6672 6565  superimpose_free
+0002fef0: 7465 7874 2e5f 5f6e 616d 655f 5f7d 2066  text.__name__} f
+0002ff00: 6f6e 745f 7369 7a65 272c 2076 616c 7565  ont_size', value
+0002ff10: 3d66 6f6e 745f 7369 7a65 2c20 6d69 6e5f  =font_size, min_
+0002ff20: 7661 6c75 653d 3129 0a20 2020 2063 6865  value=1).    che
+0002ff30: 636b 5f69 6e74 286e 616d 653d 6627 7b73  ck_int(name=f'{s
+0002ff40: 7570 6572 696d 706f 7365 5f66 7265 6574  uperimpose_freet
+0002ff50: 6578 742e 5f5f 6e61 6d65 5f5f 7d20 666f  ext.__name__} fo
+0002ff60: 6e74 5f62 6f72 6465 725f 7769 6474 6827  nt_border_width'
+0002ff70: 2c20 7661 6c75 653d 666f 6e74 5f62 6f72  , value=font_bor
+0002ff80: 6465 725f 7769 6474 682c 206d 696e 5f76  der_width, min_v
+0002ff90: 616c 7565 3d31 290a 2020 2020 6368 6563  alue=1).    chec
+0002ffa0: 6b5f 7374 7228 6e61 6d65 3d66 277b 7375  k_str(name=f'{su
+0002ffb0: 7065 7269 6d70 6f73 655f 6672 6565 7465  perimpose_freete
+0002ffc0: 7874 2e5f 5f6e 616d 655f 5f7d 2074 6578  xt.__name__} tex
+0002ffd0: 7427 2c20 7661 6c75 653d 7465 7874 290a  t', value=text).
+0002ffe0: 2020 2020 666f 6e74 5f64 6963 7420 3d20      font_dict = 
+0002fff0: 6765 745f 666f 6e74 7328 290a 2020 2020  get_fonts().    
+00030000: 6368 6563 6b5f 7374 7228 6e61 6d65 3d27  check_str(name='
+00030010: 666f 6e74 272c 2076 616c 7565 3d66 6f6e  font', value=fon
+00030020: 742c 206f 7074 696f 6e73 3d74 7570 6c65  t, options=tuple
+00030030: 2866 6f6e 745f 6469 6374 2e6b 6579 7328  (font_dict.keys(
+00030040: 2929 290a 2020 2020 666f 6e74 5f70 6174  ))).    font_pat
+00030050: 6820 3d20 666f 6e74 5f64 6963 745b 666f  h = font_dict[fo
+00030060: 6e74 5d0a 2020 2020 666f 6e74 5f63 6f6c  nt].    font_col
+00030070: 6f72 203d 2027 272e 6a6f 696e 2866 696c  or = ''.join(fil
+00030080: 7465 7228 7374 722e 6973 616c 6e75 6d2c  ter(str.isalnum,
+00030090: 2066 6f6e 745f 636f 6c6f 7229 292e 6c6f   font_color)).lo
+000300a0: 7765 7228 290a 2020 2020 666f 6e74 5f62  wer().    font_b
+000300b0: 6f72 6465 725f 636f 6c6f 7220 3d20 2727  order_color = ''
+000300c0: 2e6a 6f69 6e28 6669 6c74 6572 2873 7472  .join(filter(str
+000300d0: 2e69 7361 6c6e 756d 2c20 666f 6e74 5f62  .isalnum, font_b
+000300e0: 6f72 6465 725f 636f 6c6f 7229 292e 6c6f  order_color)).lo
+000300f0: 7765 7228 290a 2020 2020 6966 206f 732e  wer().    if os.
+00030100: 7061 7468 2e69 7366 696c 6528 7669 6465  path.isfile(vide
+00030110: 6f5f 7061 7468 293a 0a20 2020 2020 2020  o_path):.       
+00030120: 2076 6964 656f 5f70 6174 6873 203d 205b   video_paths = [
+00030130: 7669 6465 6f5f 7061 7468 5d0a 2020 2020  video_path].    
+00030140: 656c 6966 206f 732e 7061 7468 2e69 7364  elif os.path.isd
+00030150: 6972 2876 6964 656f 5f70 6174 6829 3a0a  ir(video_path):.
+00030160: 2020 2020 2020 2020 7669 6465 6f5f 7061          video_pa
+00030170: 7468 7320 3d20 6c69 7374 2866 696e 645f  ths = list(find_
+00030180: 616c 6c5f 7669 6465 6f73 5f69 6e5f 6469  all_videos_in_di
+00030190: 7265 6374 6f72 7928 6469 7265 6374 6f72  rectory(director
+000301a0: 793d 7669 6465 6f5f 7061 7468 2c20 6173  y=video_path, as
+000301b0: 5f64 6963 743d 5472 7565 2c20 7261 6973  _dict=True, rais
+000301c0: 655f 6572 726f 723d 5472 7565 292e 7661  e_error=True).va
+000301d0: 6c75 6573 2829 290a 2020 2020 656c 7365  lues()).    else
+000301e0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+000301f0: 496e 7661 6c69 6449 6e70 7574 4572 726f  InvalidInputErro
+00030200: 7228 6d73 673d 6627 7b76 6964 656f 5f70  r(msg=f'{video_p
+00030210: 6174 687d 2069 7320 6e6f 7420 6120 7661  ath} is not a va
+00030220: 6c69 6420 6669 6c65 2070 6174 6820 6f72  lid file path or
+00030230: 2061 2076 616c 6964 2064 6972 6563 746f   a valid directo
+00030240: 7279 2070 6174 6827 2c20 736f 7572 6365  ry path', source
+00030250: 3d73 7570 6572 696d 706f 7365 5f76 6964  =superimpose_vid
+00030260: 656f 5f6e 616d 6573 2e5f 5f6e 616d 655f  eo_names.__name_
+00030270: 5f29 0a20 2020 2069 6620 7361 7665 5f64  _).    if save_d
+00030280: 6972 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ir is not None:.
+00030290: 2020 2020 2020 2020 6368 6563 6b5f 6966          check_if
+000302a0: 5f64 6972 5f65 7869 7374 7328 696e 5f64  _dir_exists(in_d
+000302b0: 6972 3d73 6176 655f 6469 7229 0a20 2020  ir=save_dir).   
+000302c0: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+000302d0: 6176 655f 6469 7220 3d20 6f73 2e70 6174  ave_dir = os.pat
+000302e0: 682e 6469 726e 616d 6528 7669 6465 6f5f  h.dirname(video_
+000302f0: 7061 7468 735b 305d 290a 2020 2020 666f  paths[0]).    fo
+00030300: 7220 6669 6c65 5f63 6e74 2c20 7669 6465  r file_cnt, vide
+00030310: 6f5f 7061 7468 2069 6e20 656e 756d 6572  o_path in enumer
+00030320: 6174 6528 7669 6465 6f5f 7061 7468 7329  ate(video_paths)
+00030330: 3a0a 2020 2020 2020 2020 5f2c 2076 6964  :.        _, vid
+00030340: 656f 5f6e 616d 652c 2065 7874 203d 2067  eo_name, ext = g
+00030350: 6574 5f66 6e5f 6578 7428 7669 6465 6f5f  et_fn_ext(video_
+00030360: 7061 7468 290a 2020 2020 2020 2020 7072  path).        pr
+00030370: 696e 7428 6627 5375 7065 7269 6d70 6f73  int(f'Superimpos
+00030380: 696e 6720 7669 6465 6f20 6e61 6d65 206f  ing video name o
+00030390: 6e20 7b76 6964 656f 5f6e 616d 657d 2028  n {video_name} (
+000303a0: 5669 6465 6f20 7b66 696c 655f 636e 7420  Video {file_cnt 
+000303b0: 2b20 317d 2f7b 6c65 6e28 7669 6465 6f5f  + 1}/{len(video_
+000303c0: 7061 7468 7329 7d29 2e2e 2e27 290a 2020  paths)})...').  
+000303d0: 2020 2020 2020 7361 7665 5f70 6174 6820        save_path 
+000303e0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2873  = os.path.join(s
+000303f0: 6176 655f 6469 722c 2066 277b 7669 6465  ave_dir, f'{vide
+00030400: 6f5f 6e61 6d65 7d5f 7465 7874 5f73 7570  o_name}_text_sup
+00030410: 6572 696d 706f 7365 647b 6578 747d 2729  erimposed{ext}')
+00030420: 0a20 2020 2020 2020 2069 6620 706f 7369  .        if posi
+00030430: 7469 6f6e 203d 3d20 504f 5349 5449 4f4e  tion == POSITION
+00030440: 535b 305d 3a0a 2020 2020 2020 2020 2020  S[0]:.          
+00030450: 2020 636d 6420 3d20 6622 6666 6d70 6567    cmd = f"ffmpeg
+00030460: 202d 6920 277b 7669 6465 6f5f 7061 7468   -i '{video_path
+00030470: 7d27 202d 7666 205c 2264 7261 7774 6578  }' -vf \"drawtex
+00030480: 743d 666f 6e74 6669 6c65 3d7b 666f 6e74  t=fontfile={font
+00030490: 5f70 6174 687d 3a74 6578 743d 7b74 6578  _path}:text={tex
+000304a0: 747d 3a78 3d35 3a79 3d35 3a66 6f6e 7473  t}:x=5:y=5:fonts
+000304b0: 697a 653d 7b66 6f6e 745f 7369 7a65 7d3a  ize={font_size}:
+000304c0: 666f 6e74 636f 6c6f 723d 7b66 6f6e 745f  fontcolor={font_
+000304d0: 636f 6c6f 727d 3a62 6f72 6465 7277 3d7b  color}:borderw={
+000304e0: 666f 6e74 5f62 6f72 6465 725f 7769 6474  font_border_widt
+000304f0: 687d 3a62 6f72 6465 7263 6f6c 6f72 3d7b  h}:bordercolor={
+00030500: 666f 6e74 5f62 6f72 6465 725f 636f 6c6f  font_border_colo
+00030510: 727d 5c22 202d 633a 6120 636f 7079 2027  r}\" -c:a copy '
+00030520: 7b73 6176 655f 7061 7468 7d27 202d 6c6f  {save_path}' -lo
+00030530: 676c 6576 656c 2065 7272 6f72 202d 7374  glevel error -st
+00030540: 6174 7320 2d68 6964 655f 6261 6e6e 6572  ats -hide_banner
+00030550: 202d 7922 0a20 2020 2020 2020 2065 6c69   -y".        eli
+00030560: 6620 706f 7369 7469 6f6e 203d 3d20 504f  f position == PO
+00030570: 5349 5449 4f4e 535b 315d 3a0a 2020 2020  SITIONS[1]:.    
+00030580: 2020 2020 2020 2020 636d 6420 3d20 6622          cmd = f"
+00030590: 6666 6d70 6567 202d 6920 277b 7669 6465  ffmpeg -i '{vide
+000305a0: 6f5f 7061 7468 7d27 202d 7666 205c 2264  o_path}' -vf \"d
+000305b0: 7261 7774 6578 743d 666f 6e74 6669 6c65  rawtext=fontfile
+000305c0: 3d7b 666f 6e74 5f70 6174 687d 3a74 6578  ={font_path}:tex
+000305d0: 743d 7b74 6578 747d 3a78 3d28 772d 7477  t={text}:x=(w-tw
+000305e0: 2d35 293a 793d 353a 666f 6e74 7369 7a65  -5):y=5:fontsize
+000305f0: 3d7b 666f 6e74 5f73 697a 657d 3a66 6f6e  ={font_size}:fon
+00030600: 7463 6f6c 6f72 3d7b 666f 6e74 5f63 6f6c  tcolor={font_col
+00030610: 6f72 7d3a 626f 7264 6572 773d 7b66 6f6e  or}:borderw={fon
+00030620: 745f 626f 7264 6572 5f77 6964 7468 7d3a  t_border_width}:
+00030630: 626f 7264 6572 636f 6c6f 723d 7b66 6f6e  bordercolor={fon
+00030640: 745f 626f 7264 6572 5f63 6f6c 6f72 7d5c  t_border_color}\
+00030650: 2220 2d63 3a61 2063 6f70 7920 277b 7361  " -c:a copy '{sa
+00030660: 7665 5f70 6174 687d 2720 2d6c 6f67 6c65  ve_path}' -logle
+00030670: 7665 6c20 6572 726f 7220 2d73 7461 7473  vel error -stats
+00030680: 202d 6869 6465 5f62 616e 6e65 7220 2d79   -hide_banner -y
+00030690: 220a 2020 2020 2020 2020 656c 6966 2070  ".        elif p
+000306a0: 6f73 6974 696f 6e20 3d3d 2050 4f53 4954  osition == POSIT
+000306b0: 494f 4e53 5b32 5d3a 0a20 2020 2020 2020  IONS[2]:.       
+000306c0: 2020 2020 2063 6d64 203d 2066 2266 666d       cmd = f"ffm
+000306d0: 7065 6720 2d69 2027 7b76 6964 656f 5f70  peg -i '{video_p
+000306e0: 6174 687d 2720 2d76 6620 5c22 6472 6177  ath}' -vf \"draw
+000306f0: 7465 7874 3d66 6f6e 7466 696c 653d 7b66  text=fontfile={f
+00030700: 6f6e 745f 7061 7468 7d3a 7465 7874 3d7b  ont_path}:text={
+00030710: 7465 7874 7d3a 783d 353a 793d 2868 2d74  text}:x=5:y=(h-t
+00030720: 682d 3529 3a66 6f6e 7473 697a 653d 7b66  h-5):fontsize={f
+00030730: 6f6e 745f 7369 7a65 7d3a 666f 6e74 636f  ont_size}:fontco
+00030740: 6c6f 723d 7b66 6f6e 745f 636f 6c6f 727d  lor={font_color}
+00030750: 3a62 6f72 6465 7277 3d7b 666f 6e74 5f62  :borderw={font_b
+00030760: 6f72 6465 725f 7769 6474 687d 3a62 6f72  order_width}:bor
+00030770: 6465 7263 6f6c 6f72 3d7b 666f 6e74 5f62  dercolor={font_b
+00030780: 6f72 6465 725f 636f 6c6f 727d 5c22 202d  order_color}\" -
+00030790: 633a 6120 636f 7079 2027 7b73 6176 655f  c:a copy '{save_
+000307a0: 7061 7468 7d27 202d 6c6f 676c 6576 656c  path}' -loglevel
+000307b0: 2065 7272 6f72 202d 7374 6174 7320 2d68   error -stats -h
+000307c0: 6964 655f 6261 6e6e 6572 202d 7922 0a20  ide_banner -y". 
+000307d0: 2020 2020 2020 2065 6c69 6620 706f 7369         elif posi
+000307e0: 7469 6f6e 203d 3d20 504f 5349 5449 4f4e  tion == POSITION
+000307f0: 535b 335d 3a0a 2020 2020 2020 2020 2020  S[3]:.          
+00030800: 2020 636d 6420 3d20 6622 6666 6d70 6567    cmd = f"ffmpeg
+00030810: 202d 6920 277b 7669 6465 6f5f 7061 7468   -i '{video_path
+00030820: 7d27 202d 7666 205c 2264 7261 7774 6578  }' -vf \"drawtex
+00030830: 743d 666f 6e74 6669 6c65 3d7b 666f 6e74  t=fontfile={font
+00030840: 5f70 6174 687d 3a74 6578 743d 7b74 6578  _path}:text={tex
+00030850: 747d 3a78 3d28 772d 7477 2d35 293a 793d  t}:x=(w-tw-5):y=
+00030860: 2868 2d74 682d 3529 3a66 6f6e 7473 697a  (h-th-5):fontsiz
+00030870: 653d 7b66 6f6e 745f 7369 7a65 7d3a 666f  e={font_size}:fo
+00030880: 6e74 636f 6c6f 723d 7b66 6f6e 745f 636f  ntcolor={font_co
+00030890: 6c6f 727d 3a62 6f72 6465 7277 3d7b 666f  lor}:borderw={fo
+000308a0: 6e74 5f62 6f72 6465 725f 7769 6474 687d  nt_border_width}
+000308b0: 3a62 6f72 6465 7263 6f6c 6f72 3d7b 666f  :bordercolor={fo
+000308c0: 6e74 5f62 6f72 6465 725f 636f 6c6f 727d  nt_border_color}
+000308d0: 5c22 202d 633a 6120 636f 7079 2027 7b73  \" -c:a copy '{s
+000308e0: 6176 655f 7061 7468 7d27 202d 6c6f 676c  ave_path}' -logl
+000308f0: 6576 656c 2065 7272 6f72 202d 7374 6174  evel error -stat
+00030900: 7320 2d68 6964 655f 6261 6e6e 6572 202d  s -hide_banner -
+00030910: 7922 0a20 2020 2020 2020 2065 6c69 6620  y".        elif 
+00030920: 706f 7369 7469 6f6e 203d 3d20 504f 5349  position == POSI
+00030930: 5449 4f4e 535b 345d 3a0a 2020 2020 2020  TIONS[4]:.      
+00030940: 2020 2020 2020 636d 6420 3d20 6622 6666        cmd = f"ff
+00030950: 6d70 6567 202d 6920 277b 7669 6465 6f5f  mpeg -i '{video_
+00030960: 7061 7468 7d27 202d 7666 205c 2264 7261  path}' -vf \"dra
+00030970: 7774 6578 743d 666f 6e74 6669 6c65 3d7b  wtext=fontfile={
+00030980: 666f 6e74 5f70 6174 687d 3a74 6578 743d  font_path}:text=
+00030990: 7b74 6578 747d 3a78 3d28 772d 7477 292f  {text}:x=(w-tw)/
+000309a0: 323a 793d 3130 3a66 6f6e 7473 697a 653d  2:y=10:fontsize=
+000309b0: 7b66 6f6e 745f 7369 7a65 7d3a 666f 6e74  {font_size}:font
+000309c0: 636f 6c6f 723d 7b66 6f6e 745f 636f 6c6f  color={font_colo
+000309d0: 727d 3a62 6f72 6465 7277 3d7b 666f 6e74  r}:borderw={font
+000309e0: 5f62 6f72 6465 725f 7769 6474 687d 3a62  _border_width}:b
+000309f0: 6f72 6465 7263 6f6c 6f72 3d7b 666f 6e74  ordercolor={font
+00030a00: 5f62 6f72 6465 725f 636f 6c6f 727d 5c22  _border_color}\"
+00030a10: 202d 633a 6120 636f 7079 2027 7b73 6176   -c:a copy '{sav
+00030a20: 655f 7061 7468 7d27 202d 6c6f 676c 6576  e_path}' -loglev
+00030a30: 656c 2065 7272 6f72 202d 7374 6174 7320  el error -stats 
+00030a40: 2d68 6964 655f 6261 6e6e 6572 202d 7922  -hide_banner -y"
+00030a50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00030a60: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00030a70: 2066 2266 666d 7065 6720 2d69 2027 7b76   f"ffmpeg -i '{v
+00030a80: 6964 656f 5f70 6174 687d 2720 2d76 6620  ideo_path}' -vf 
+00030a90: 5c22 6472 6177 7465 7874 3d66 6f6e 7466  \"drawtext=fontf
+00030aa0: 696c 653d 7b66 6f6e 745f 7061 7468 7d3a  ile={font_path}:
+00030ab0: 7465 7874 3d7b 7465 7874 7d3a 783d 2877  text={text}:x=(w
+00030ac0: 2d74 7729 2f32 3a79 3d28 682d 7468 2d31  -tw)/2:y=(h-th-1
+00030ad0: 3029 3a66 6f6e 7473 697a 653d 7b66 6f6e  0):fontsize={fon
+00030ae0: 745f 7369 7a65 7d3a 666f 6e74 636f 6c6f  t_size}:fontcolo
+00030af0: 723d 7b66 6f6e 745f 636f 6c6f 727d 3a62  r={font_color}:b
+00030b00: 6f72 6465 7277 3d7b 666f 6e74 5f62 6f72  orderw={font_bor
+00030b10: 6465 725f 7769 6474 687d 3a62 6f72 6465  der_width}:borde
+00030b20: 7263 6f6c 6f72 3d7b 666f 6e74 5f62 6f72  rcolor={font_bor
+00030b30: 6465 725f 636f 6c6f 727d 5c22 202d 633a  der_color}\" -c:
+00030b40: 6120 636f 7079 2027 7b73 6176 655f 7061  a copy '{save_pa
+00030b50: 7468 7d27 202d 6c6f 676c 6576 656c 2065  th}' -loglevel e
+00030b60: 7272 6f72 202d 7374 6174 7320 2d68 6964  rror -stats -hid
+00030b70: 655f 6261 6e6e 6572 202d 7922 0a20 2020  e_banner -y".   
+00030b80: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
+00030b90: 6361 6c6c 2863 6d64 2c20 7368 656c 6c3d  call(cmd, shell=
+00030ba0: 5472 7565 2c20 7374 646f 7574 3d73 7562  True, stdout=sub
+00030bb0: 7072 6f63 6573 732e 5049 5045 290a 2020  process.PIPE).  
+00030bc0: 2020 7469 6d65 722e 7374 6f70 5f74 696d    timer.stop_tim
+00030bd0: 6572 2829 0a20 2020 2073 7464 6f75 745f  er().    stdout_
+00030be0: 7375 6363 6573 7328 6d73 673d 6627 5375  success(msg=f'Su
+00030bf0: 7065 722d 696d 706f 7365 6420 6672 6565  per-imposed free
+00030c00: 2d74 6578 7420 6f6e 207b 6c65 6e28 7669  -text on {len(vi
+00030c10: 6465 6f5f 7061 7468 7329 7d20 7669 6465  deo_paths)} vide
+00030c20: 6f28 7329 2c20 7361 7665 6420 696e 207b  o(s), saved in {
+00030c30: 7361 7665 5f64 6972 7d27 2c20 656c 6170  save_dir}', elap
+00030c40: 7365 645f 7469 6d65 3d74 696d 6572 2e65  sed_time=timer.e
+00030c50: 6c61 7073 6564 5f74 696d 655f 7374 7229  lapsed_time_str)
+00030c60: 0a0a 0a23 2076 6964 656f 5f70 6174 6873  ...# video_paths
+00030c70: 203d 205b 272f 5573 6572 732f 7369 6d6f   = ['/Users/simo
+00030c80: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
+00030c90: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
+00030ca0: 7469 6e67 2f62 6565 7062 6f6f 7031 3734  ting/beepboop174
+00030cb0: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
+00030cc0: 6d65 7267 652f 5472 6961 6c20 2020 2031  merge/Trial    1
+00030cd0: 305f 636c 6970 7065 645f 6761 6e74 742e  0_clipped_gantt.
+00030ce0: 6d70 3427 2c0a 2320 2020 2020 2020 2020  mp4',.#         
+00030cf0: 2020 2020 2020 2027 2f55 7365 7273 2f73         '/Users/s
+00030d00: 696d 6f6e 2f44 6573 6b74 6f70 2f65 6e76  imon/Desktop/env
+00030d10: 732f 7369 6d62 612f 7472 6f75 626c 6573  s/simba/troubles
+00030d20: 686f 6f74 696e 672f 6265 6570 626f 6f70  hooting/beepboop
+00030d30: 3137 342f 7072 6f6a 6563 745f 666f 6c64  174/project_fold
+00030d40: 6572 2f6d 6572 6765 2f54 7269 616c 2020  er/merge/Trial  
+00030d50: 2020 3130 5f63 6c69 7070 6564 2e6d 7034    10_clipped.mp4
+00030d60: 272c 0a23 2020 2020 2020 2020 2020 2020  ',.#            
+00030d70: 2020 2020 272f 5573 6572 732f 7369 6d6f      '/Users/simo
+00030d80: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
+00030d90: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
+00030da0: 7469 6e67 2f62 6565 7062 6f6f 7031 3734  ting/beepboop174
+00030db0: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
+00030dc0: 6d65 7267 652f 5472 6961 6c20 2020 2031  merge/Trial    1
+00030dd0: 305f 636c 6970 7065 645f 6c69 6e65 2e6d  0_clipped_line.m
+00030de0: 7034 272c 0a23 2020 2020 2020 2020 2020  p4',.#          
+00030df0: 2020 2020 2020 272f 5573 6572 732f 7369        '/Users/si
+00030e00: 6d6f 6e2f 4465 736b 746f 702f 656e 7673  mon/Desktop/envs
+00030e10: 2f73 696d 6261 2f74 726f 7562 6c65 7368  /simba/troublesh
+00030e20: 6f6f 7469 6e67 2f62 6565 7062 6f6f 7031  ooting/beepboop1
+00030e30: 3734 2f70 726f 6a65 6374 5f66 6f6c 6465  74/project_folde
+00030e40: 722f 6d65 7267 652f 5472 6961 6c20 2020  r/merge/Trial   
+00030e50: 2020 335f 636c 6970 7065 642e 6d70 3427    3_clipped.mp4'
+00030e60: 5d0a 230a 2320 7669 6465 6f5f 7061 7468  ].#.# video_path
+00030e70: 7320 3d20 5b27 2f55 7365 7273 2f73 696d  s = ['/Users/sim
+00030e80: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+00030e90: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+00030ea0: 6f74 696e 672f 6265 6570 626f 6f70 3137  oting/beepboop17
+00030eb0: 342f 7072 6f6a 6563 745f 666f 6c64 6572  4/project_folder
+00030ec0: 2f76 6964 656f 732f 5472 6961 6c20 2020  /videos/Trial   
+00030ed0: 2031 302e 6d70 3427 2c0a 2320 2020 2020   10.mp4',.#     
+00030ee0: 2020 2020 2020 2020 2020 2027 2f55 7365             '/Use
+00030ef0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+00030f00: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+00030f10: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
+00030f20: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
+00030f30: 666f 6c64 6572 2f6d 6572 6765 2f54 7269  folder/merge/Tri
+00030f40: 616c 2020 2020 3130 5f63 6c69 7070 6564  al    10_clipped
+00030f50: 5f67 616e 7474 2e6d 7034 272c 0a23 2020  _gantt.mp4',.#  
+00030f60: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+00030f70: 5573 6572 732f 7369 6d6f 6e2f 4465 736b  Users/simon/Desk
+00030f80: 746f 702f 656e 7673 2f73 696d 6261 2f74  top/envs/simba/t
+00030f90: 726f 7562 6c65 7368 6f6f 7469 6e67 2f62  roubleshooting/b
+00030fa0: 6565 7062 6f6f 7031 3734 2f70 726f 6a65  eepboop174/proje
+00030fb0: 6374 5f66 6f6c 6465 722f 6d65 7267 652f  ct_folder/merge/
+00030fc0: 5472 6961 6c20 2020 2031 305f 636c 6970  Trial    10_clip
+00030fd0: 7065 645f 6c69 6e65 2e6d 7034 272c 0a23  ped_line.mp4',.#
+00030fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00030ff0: 272f 5573 6572 732f 7369 6d6f 6e2f 4465  '/Users/simon/De
+00031000: 736b 746f 702f 656e 7673 2f73 696d 6261  sktop/envs/simba
+00031010: 2f74 726f 7562 6c65 7368 6f6f 7469 6e67  /troubleshooting
+00031020: 2f62 6565 7062 6f6f 7031 3734 2f70 726f  /beepboop174/pro
+00031030: 6a65 6374 5f66 6f6c 6465 722f 6d65 7267  ject_folder/merg
+00031040: 652f 5472 6961 6c20 2020 2020 335f 636c  e/Trial     3_cl
+00031050: 6970 7065 642e 6d70 3427 5d0a 230a 2320  ipped.mp4'].#.# 
+00031060: 7361 7665 5f70 6174 6820 3d20 272f 5573  save_path = '/Us
+00031070: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+00031080: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+00031090: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
+000310a0: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
+000310b0: 5f66 6f6c 6465 722f 6d65 7267 652f 6f75  _folder/merge/ou
+000310c0: 742e 6d70 3427 0a0a 230a 2320 7669 6465  t.mp4'..#.# vide
+000310d0: 6f5f 7061 7468 7320 3d20 5b27 2f55 7365  o_paths = ['/Use
+000310e0: 7273 2f73 696d 6f6e 2f44 6573 6b74 6f70  rs/simon/Desktop
+000310f0: 2f65 6e76 732f 7369 6d62 612f 7472 6f75  /envs/simba/trou
+00031100: 626c 6573 686f 6f74 696e 672f 6265 6570  bleshooting/beep
+00031110: 626f 6f70 3137 342f 7072 6f6a 6563 745f  boop174/project_
+00031120: 666f 6c64 6572 2f66 7261 6d65 732f 6f75  folder/frames/ou
+00031130: 7470 7574 2f67 616e 7474 5f70 6c6f 7473  tput/gantt_plots
+00031140: 2f54 7269 616c 2020 2020 3130 2e6d 7034  /Trial    10.mp4
+00031150: 272c 0a23 2020 2020 2020 2020 2020 2020  ',.#            
+00031160: 2020 2020 272f 5573 6572 732f 7369 6d6f      '/Users/simo
+00031170: 6e2f 4465 736b 746f 702f 656e 7673 2f73  n/Desktop/envs/s
+00031180: 696d 6261 2f74 726f 7562 6c65 7368 6f6f  imba/troubleshoo
+00031190: 7469 6e67 2f62 6565 7062 6f6f 7031 3734  ting/beepboop174
+000311a0: 2f70 726f 6a65 6374 5f66 6f6c 6465 722f  /project_folder/
+000311b0: 7669 6465 6f73 2f54 7269 616c 2020 2020  videos/Trial    
+000311c0: 3130 2e6d 7034 272c 0a23 2020 2020 2020  10.mp4',.#      
+000311d0: 2020 2020 2020 2020 2020 272f 5573 6572            '/User
+000311e0: 732f 7369 6d6f 6e2f 4465 736b 746f 702f  s/simon/Desktop/
+000311f0: 656e 7673 2f73 696d 6261 2f74 726f 7562  envs/simba/troub
+00031200: 6c65 7368 6f6f 7469 6e67 2f62 6565 7062  leshooting/beepb
+00031210: 6f6f 7031 3734 2f70 726f 6a65 6374 5f66  oop174/project_f
+00031220: 6f6c 6465 722f 6672 616d 6573 2f6f 7574  older/frames/out
+00031230: 7075 742f 6c69 6e65 5f70 6c6f 742f 5472  put/line_plot/Tr
+00031240: 6961 6c20 2020 2031 302e 6d70 3427 2c0a  ial    10.mp4',.
+00031250: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00031260: 2027 2f55 7365 7273 2f73 696d 6f6e 2f44   '/Users/simon/D
+00031270: 6573 6b74 6f70 2f65 6e76 732f 7369 6d62  esktop/envs/simb
+00031280: 612f 7472 6f75 626c 6573 686f 6f74 696e  a/troubleshootin
+00031290: 672f 6265 6570 626f 6f70 3137 342f 7072  g/beepboop174/pr
+000312a0: 6f6a 6563 745f 666f 6c64 6572 2f66 7261  oject_folder/fra
+000312b0: 6d65 732f 6f75 7470 7574 2f6c 696e 655f  mes/output/line_
+000312c0: 706c 6f74 2f54 7269 616c 2020 2020 2033  plot/Trial     3
+000312d0: 2e6d 7034 275d 0a23 2073 6176 655f 7061  .mp4'].# save_pa
+000312e0: 7468 203d 2027 2f55 7365 7273 2f73 696d  th = '/Users/sim
+000312f0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+00031300: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+00031310: 6f74 696e 672f 5241 545f 4e4f 522f 7072  oting/RAT_NOR/pr
+00031320: 6f6a 6563 745f 666f 6c64 6572 2f76 6964  oject_folder/vid
+00031330: 656f 732f 7465 7374 2f6e 6577 2f62 6c61  eos/test/new/bla
+00031340: 6e6b 5f74 6573 742e 6d70 3427 0a0a 2320  nk_test.mp4'..# 
+00031350: 7669 6465 6f5f 7061 7468 7320 3d20 5b27  video_paths = ['
+00031360: 2f55 7365 7273 2f73 696d 6f6e 2f44 6573  /Users/simon/Des
+00031370: 6b74 6f70 2f65 6e76 732f 7369 6d62 612f  ktop/envs/simba/
+00031380: 7472 6f75 626c 6573 686f 6f74 696e 672f  troubleshooting/
+00031390: 6265 6570 626f 6f70 3137 342f 7072 6f6a  beepboop174/proj
+000313a0: 6563 745f 666f 6c64 6572 2f76 6964 656f  ect_folder/video
+000313b0: 732f 5472 6961 6c20 2020 2031 302e 6d70  s/Trial    10.mp
+000313c0: 3427 2c0a 2320 2020 2020 2020 2020 2020  4',.#           
+000313d0: 2020 2020 2027 2f55 7365 7273 2f73 696d       '/Users/sim
+000313e0: 6f6e 2f44 6573 6b74 6f70 2f65 6e76 732f  on/Desktop/envs/
+000313f0: 7369 6d62 612f 7472 6f75 626c 6573 686f  simba/troublesho
+00031400: 6f74 696e 672f 6265 6570 626f 6f70 3137  oting/beepboop17
+00031410: 342f 7072 6f6a 6563 745f 666f 6c64 6572  4/project_folder
+00031420: 2f66 7261 6d65 732f 6f75 7470 7574 2f6c  /frames/output/l
+00031430: 696e 655f 706c 6f74 2f54 7269 616c 2020  ine_plot/Trial  
+00031440: 2020 3130 2e6d 7034 272c 0a23 2020 2020    10.mp4',.#    
+00031450: 2020 2020 2020 2020 2020 2020 272f 5573              '/Us
+00031460: 6572 732f 7369 6d6f 6e2f 4465 736b 746f  ers/simon/Deskto
+00031470: 702f 656e 7673 2f73 696d 6261 2f74 726f  p/envs/simba/tro
+00031480: 7562 6c65 7368 6f6f 7469 6e67 2f62 6565  ubleshooting/bee
+00031490: 7062 6f6f 7031 3734 2f70 726f 6a65 6374  pboop174/project
+000314a0: 5f66 6f6c 6465 722f 6672 616d 6573 2f6f  _folder/frames/o
+000314b0: 7574 7075 742f 6c69 6e65 5f70 6c6f 742f  utput/line_plot/
+000314c0: 5472 6961 6c20 2020 2020 332e 6d70 3427  Trial     3.mp4'
+000314d0: 5d0a 0a23 206d 6978 6564 5f6d 6f73 6169  ]..# mixed_mosai
+000314e0: 635f 636f 6e63 6174 656e 6174 6f72 2876  c_concatenator(v
+000314f0: 6964 656f 5f70 6174 6873 3d76 6964 656f  ideo_paths=video
+00031500: 5f70 6174 6873 2c20 7361 7665 5f70 6174  _paths, save_pat
+00031510: 683d 7361 7665 5f70 6174 682c 2067 7075  h=save_path, gpu
+00031520: 3d46 616c 7365 2c20 7665 7262 6f73 653d  =False, verbose=
+00031530: 5472 7565 290a                           True).
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/brightness_contrast_ui.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/brightness_contrast_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/video_processors/clahe_ui.py` & `Simba-UW-tf-dev-1.93.7/simba/video_processors/clahe_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.93.7/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.93.7/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/SimBA.py` & `Simba-UW-tf-dev-1.93.7/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,31 +116,32 @@
     SpontaneousAlternationPopUp
 from simba.ui.pop_ups.subset_feature_extractor_pop_up import \
     FeatureSubsetExtractorPopUp
 from simba.ui.pop_ups.third_party_annotator_appender_pop_up import \
     ThirdPartyAnnotatorAppenderPopUp
 from simba.ui.pop_ups.validation_plot_pop_up import ValidationVideoPopUp
 from simba.ui.pop_ups.video_processing_pop_up import (
-    BrightnessContrastPopUp, CalculatePixelsPerMMInVideoPopUp,
+    BoxBlurPopUp, BrightnessContrastPopUp, CalculatePixelsPerMMInVideoPopUp,
     ChangeFpsMultipleVideosPopUp, ChangeFpsSingleVideoPopUp, CLAHEPopUp,
     ClipSingleVideoByFrameNumbers, ClipVideoPopUp, ConcatenatingVideosPopUp,
     ConcatenatorPopUp, Convert2AVIPopUp, Convert2bmpPopUp, Convert2jpegPopUp,
     Convert2MOVPopUp, Convert2MP4PopUp, Convert2PNGPopUp, Convert2TIFFPopUp,
     Convert2WEBMPopUp, Convert2WEBPPopUp, ConvertROIDefinitionsPopUp,
     CreateGIFPopUP, CropVideoCirclesPopUp, CropVideoPolygonsPopUp,
     CropVideoPopUp, DownsampleMultipleVideosPopUp, DownsampleSingleVideoPopUp,
     DownsampleVideoPopUp, ExtractAllFramesPopUp, ExtractAnnotationFramesPopUp,
     ExtractSEQFramesPopUp, ExtractSpecificFramesPopUp,
     GreyscaleSingleVideoPopUp, ImportFrameDirectoryPopUp,
     InitiateClipMultipleVideosByFrameNumbersPopUp,
     InitiateClipMultipleVideosByTimestampsPopUp, InteractiveClahePopUp,
     MergeFrames2VideoPopUp, MultiCropPopUp, MultiShortenPopUp,
-    SuperImposeFrameCountPopUp, VideoRotatorPopUp, VideoTemporalJoinPopUp,
-    SuperimposeTimerPopUp, SuperimposeWatermarkPopUp, SuperimposeProgressBarPopUp, SuperimposeVideoPopUp, SuperimposeVideoNamesPopUp,
-    SuperimposeTextPopUp, BoxBlurPopUp)
+    SuperImposeFrameCountPopUp, SuperimposeProgressBarPopUp,
+    SuperimposeTextPopUp, SuperimposeTimerPopUp, SuperimposeVideoNamesPopUp,
+    SuperimposeVideoPopUp, SuperimposeWatermarkPopUp, VideoRotatorPopUp,
+    VideoTemporalJoinPopUp)
 from simba.ui.pop_ups.visualize_pose_in_dir_pop_up import \
     VisualizePoseInFolderPopUp
 from simba.ui.tkinter_functions import DropDownMenu, Entry_Box, FileSelect
 from simba.ui.video_info_ui import VideoInfoTable
 from simba.utils.checks import (check_ffmpeg_available,
                                 check_file_exist_and_readable, check_int)
 from simba.utils.custom_feature_extractor import CustomFeatureExtractor
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.93.7/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.93.7/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.93.7/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/assets/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 00001080: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
 00001090: 7208 0908 095f 1017 7b7b 302c 2031 3236  r...._..{{0, 126
 000010a0: 7d2c 207b 3134 3430 2c20 3633 357d 7d09  }, {1440, 635}}.
 000010b0: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
 000010c0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
 000010d0: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
 000010e0: 0500 6900 6300 6f00 6e00 736c 6731 5363  ..i.c.o.n.slg1Sc
-000010f0: 6f6d 7000 0000 0000 0945 4e00 0000 0500  omp......EN.....
+000010f0: 6f6d 7000 0000 0000 0955 f900 0000 0500  omp......U......
 00001100: 6900 6300 6f00 6e00 736c 7376 4362 6c6f  i.c.o.n.slsvCblo
 00001110: 6200 0003 2362 706c 6973 7430 30da 0102  b...#bplist00...
 00001120: 0304 0506 0708 090a 0b0c 0d1a 5455 5456  ............TUTV
 00001130: 0c58 5869 636f 6e53 697a 655f 100f 7368  .XXiconSize_..sh
 00001140: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00001150: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
 00001160: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
@@ -362,19 +362,19 @@
 00001690: 0178 017a 0183 0184 0186 0187 0189 0192  .x.z............
 000016a0: 0193 0194 0196 019f 01a0 01a2 01a3 01a5  ................
 000016b0: 01ae 01af 01b0 01b2 01bb 01bc 01be 01bf  ................
 000016c0: 01c1 01c2 01cb 01d4 01e1 0000 0000 0000  ................
 000016d0: 0201 0000 0000 0000 004b 0000 0000 0000  .........K......
 000016e0: 0000 0000 0000 0000 01e2 0000 0005 0069  ...............i
 000016f0: 0063 006f 006e 0073 6d6f 4444 626c 6f62  .c.o.n.smoDDblob
-00001700: 0000 0008 3825 f76a 88f4 c541 0000 0005  ....8%.j...A....
+00001700: 0000 0008 3a04 4ccf c9fd c541 0000 0005  ....:.L....A....
 00001710: 0069 0063 006f 006e 0073 6d6f 6444 626c  .i.c.o.n.smodDbl
-00001720: 6f62 0000 0008 3825 f76a 88f4 c541 0000  ob....8%.j...A..
+00001720: 6f62 0000 0008 3a04 4ccf c9fd c541 0000  ob....:.L....A..
 00001730: 0005 0069 0063 006f 006e 0073 7068 3153  ...i.c.o.n.sph1S
-00001740: 636f 6d70 0000 0000 000b e000 0000 0005  comp............
+00001740: 636f 6d70 0000 0000 000c 0000 0000 0005  comp............
 00001750: 0069 0063 006f 006e 0073 7653 726e 6c6f  .i.c.o.n.svSrnlo
 00001760: 6e67 0000 0001 0000 0003 0069 006d 0067  ng.........i.m.g
 00001770: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
 00001780: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
 00001790: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000017a0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 000017b0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
@@ -618,19 +618,19 @@
 00002690: 0178 017a 0183 0184 0186 0187 0189 0192  .x.z............
 000026a0: 0193 0194 0196 019f 01a0 01a2 01a3 01a5  ................
 000026b0: 01ae 01af 01b0 01b2 01bb 01bc 01be 01bf  ................
 000026c0: 01c1 01c2 01cb 01d4 01e1 0000 0000 0000  ................
 000026d0: 0201 0000 0000 0000 004b 0000 0000 0000  .........K......
 000026e0: 0000 0000 0000 0000 01e2 0000 0005 0069  ...............i
 000026f0: 0063 006f 006e 0073 6d6f 4444 626c 6f62  .c.o.n.smoDDblob
-00002700: 0000 0008 3825 f76a 88f4 c541 0000 0005  ....8%.j...A....
+00002700: 0000 0008 3a04 4ccf c9fd c541 0000 0005  ....:.L....A....
 00002710: 0069 0063 006f 006e 0073 6d6f 6444 626c  .i.c.o.n.smodDbl
-00002720: 6f62 0000 0008 3825 f76a 88f4 c541 0000  ob....8%.j...A..
+00002720: 6f62 0000 0008 3a04 4ccf c9fd c541 0000  ob....:.L....A..
 00002730: 0005 0069 0063 006f 006e 0073 7068 3153  ...i.c.o.n.sph1S
-00002740: 636f 6d70 0000 0000 000b e000 0000 0005  comp............
+00002740: 636f 6d70 0000 0000 000c 0000 0000 0005  comp............
 00002750: 0069 0063 006f 006e 0073 7653 726e 6c6f  .i.c.o.n.svSrnlo
 00002760: 6e67 0000 0001 0000 0003 0069 006d 0067  ng.........i.m.g
 00002770: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
 00002780: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
 00002790: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000027a0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
 000027b0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
```

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.93.7/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.93.7/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.93.7/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.93.7/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.93.7/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.93.7/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.93.7/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.93.7/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.93.7/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.93.7/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/blur.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/blur.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/brightness.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/brightness.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.93.7/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.93.7/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.93.7/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.93.6
+Version: 1.93.7
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -343,14 +343,15 @@
 simba/sandbox/add_body_part.py.zip
 simba/sandbox/add_probability_cnt_features.py
 simba/sandbox/adjusted_rand_score.py
 simba/sandbox/amber_featurizer.py
 simba/sandbox/amber_tests.py
 simba/sandbox/batch_video_to_greyscale.py
 simba/sandbox/berger_parker.py
+simba/sandbox/bg_remover_popup.py
 simba/sandbox/bg_substraction.py
 simba/sandbox/biweight_midcorrelation.py
 simba/sandbox/blurbox.py
 simba/sandbox/bouts_df
 simba/sandbox/brillouins_index.py
 simba/sandbox/calc_N_degree_direction_switches.py
 simba/sandbox/calinski_harabasz.py
```

### Comparing `Simba-UW-tf-dev-1.93.6/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.93.7/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/LICENSE` & `Simba-UW-tf-dev-1.93.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.93.7/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.93.7/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_stats.py` & `Simba-UW-tf-dev-1.93.7/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.93.7/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.93.7/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.93.7/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.93.7/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.93.7/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.93.7/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.93.7/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.93.7/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.93.7/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.93.7/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/README.md` & `Simba-UW-tf-dev-1.93.7/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.93.6/setup.py` & `Simba-UW-tf-dev-1.93.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.93.6",
+    version="1.93.7",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

