# Comparing `tmp/vocalpy-0.9.0.tar.gz` & `tmp/vocalpy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalpy-0.9.0.tar", last modified: Thu May 16 03:55:53 2024, max compression
+gzip compressed data, was "vocalpy-0.9.1.tar", last modified: Tue May 21 14:28:09 2024, max compression
```

## Comparing `vocalpy-0.9.0.tar` & `vocalpy-0.9.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0      650 2024-01-26 17:19:50.207528 vocalpy-0.9.0/.all-contributorsrc
--rw-r--r--   0        0        0     1307 2023-09-19 17:23:06.009955 vocalpy-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2023-08-20 18:48:42.054440 vocalpy-0.9.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2023-08-20 18:48:42.054440 vocalpy-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      705 2024-01-17 01:58:19.551347 vocalpy-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      463 2024-02-22 13:15:42.873235 vocalpy-0.9.0/.gitignore
--rw-r--r--   0        0        0      769 2023-08-20 18:48:42.054440 vocalpy-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      334 2023-09-29 20:50:59.859125 vocalpy-0.9.0/.readthedocs.yaml
--rw-r--r--   0        0        0     5556 2023-09-19 17:23:06.009955 vocalpy-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1867 2023-08-20 18:48:42.054440 vocalpy-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1540 2023-04-18 02:08:12.226241 vocalpy-0.9.0/LICENSE
--rw-r--r--   0        0        0    15851 2024-02-12 02:46:58.472428 vocalpy-0.9.0/README.md
--rw-r--r--   0        0        0       46 2024-02-24 00:45:51.665844 vocalpy-0.9.0/codecov.yml
--rw-r--r--   0        0        0     8562 2024-05-16 03:54:52.513377 vocalpy-0.9.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0      775 2024-02-22 13:15:42.873235 vocalpy-0.9.0/docs/Makefile
--rw-r--r--   0        0        0    29965 2023-08-20 18:48:42.054440 vocalpy-0.9.0/docs/_static/vocalpy-logomark.png
--rw-r--r--   0        0        0   285798 2023-08-20 18:48:42.054440 vocalpy-0.9.0/docs/_static/vocalpy-primary.png
--rw-r--r--   0        0        0   194159 2023-08-20 18:48:42.054440 vocalpy-0.9.0/docs/_static/vocalpy-secondary.png
--rw-r--r--   0        0        0      612 2023-12-30 13:28:54.397449 vocalpy-0.9.0/docs/_templates/class.rst
--rw-r--r--   0        0        0     1177 2023-12-30 13:28:54.397449 vocalpy-0.9.0/docs/_templates/module.rst
--rw-r--r--   0        0        0     1279 2024-05-16 03:52:17.046400 vocalpy-0.9.0/docs/api/index.rst
--rw-r--r--   0        0        0     3862 2024-04-02 23:44:46.834318 vocalpy-0.9.0/docs/conf.py
--rw-r--r--   0        0        0    17033 2023-09-19 17:23:06.009955 vocalpy-0.9.0/docs/fa2023/FA2023_template.tex
--rw-r--r--   0        0        0  1735302 2023-09-19 18:23:52.210288 vocalpy-0.9.0/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf
--rw-r--r--   0        0        0     8966 2023-09-19 17:23:06.009955 vocalpy-0.9.0/docs/fa2023/fa2023.sty
--rw-r--r--   0        0        0  1008143 2023-08-20 18:48:42.058440 vocalpy-0.9.0/docs/fa2023/footer_logo_aia.png
--rw-r--r--   0        0        0   313241 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/footer_logo_eaa.jpg
--rw-r--r--   0        0        0    10783 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/forum-acusticum-2023.bib
--rw-r--r--   0        0        0    18787 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/header.png
--rw-r--r--   0        0        0    39228 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/header_onda.png
--rw-r--r--   0        0        0    17958 2024-02-03 13:05:38.608298 vocalpy-0.9.0/docs/fa2023/main.tex
--rw-r--r--   0        0        0   118445 2023-08-20 18:48:42.070440 vocalpy-0.9.0/docs/fa2023/voc-fig1-model.png
--rw-r--r--   0        0        0      141 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/getting_started/index.md
--rw-r--r--   0        0        0     2503 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/getting_started/installation.md
--rw-r--r--   0        0        0    10248 2024-04-03 03:02:45.940030 vocalpy-0.9.0/docs/getting_started/quickstart.md
--rw-r--r--   0        0        0     3554 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/index.md
--rw-r--r--   0        0        0      800 2023-08-20 18:48:42.070440 vocalpy-0.9.0/docs/make.bat
--rw-r--r--   0        0        0      881 2023-09-19 17:23:06.009955 vocalpy-0.9.0/docs/nitpick-ignore.txt
--rw-r--r--   0        0        0     4147 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/user/background.md
--rw-r--r--   0        0        0       67 2024-04-03 03:02:45.940030 vocalpy-0.9.0/docs/user/howto/index.md
--rw-r--r--   0        0        0    15636 2024-04-09 02:06:31.842592 vocalpy-0.9.0/docs/user/howto/segmentation-ir-metrics.md
--rw-r--r--   0        0        0      343 2024-04-03 03:02:45.940030 vocalpy-0.9.0/docs/user/index.md
--rw-r--r--   0        0        0    10030 2024-02-12 02:46:58.472428 vocalpy-0.9.0/docs/user/whatisvocalpy.md
--rw-r--r--   0        0        0     8492 2024-02-24 00:45:51.665844 vocalpy-0.9.0/noxfile.py
--rw-r--r--   0        0        0     2438 2024-05-16 03:55:24.713165 vocalpy-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/src/scripts/example_data/.gitkeep
--rw-r--r--   0        0        0     6836 2024-02-22 13:15:42.873235 vocalpy-0.9.0/src/scripts/make_example_data.py
--rw-r--r--   0        0        0      804 2024-05-16 03:55:24.705165 vocalpy-0.9.0/src/vocalpy/__about__.py
--rw-r--r--   0        0        0     1866 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 17:19:50.211528 vocalpy-0.9.0/src/vocalpy/_spectrogram/__init__.py
--rw-r--r--   0        0        0     9382 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/_spectrogram/data_type.py
--rw-r--r--   0        0        0       36 2024-02-12 02:46:58.472428 vocalpy-0.9.0/src/vocalpy/_vendor/__init__.py
--rw-r--r--   0        0        0     6910 2024-02-12 02:46:58.472428 vocalpy-0.9.0/src/vocalpy/_vendor/evfuncs.py
--rw-r--r--   0        0        0     1092 2023-08-20 18:48:42.070440 vocalpy-0.9.0/src/vocalpy/annotation.py
--rw-r--r--   0        0        0     1830 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/annotation_file.py
--rw-r--r--   0        0        0        0 2023-08-20 18:48:42.070440 vocalpy-0.9.0/src/vocalpy/annotator.py
--rw-r--r--   0        0        0      541 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/audio_file.py
--rw-r--r--   0        0        0       78 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/constants.py
--rw-r--r--   0        0        0     2479 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/dataset_file.py
--rw-r--r--   0        0        0   240044 2024-01-26 17:19:50.215528 vocalpy-0.9.0/src/vocalpy/examples/BM003.wav
--rw-r--r--   0        0        0      186 2024-02-22 13:15:42.873235 vocalpy-0.9.0/src/vocalpy/examples/__init__.py
--rw-r--r--   0        0        0    10264 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/examples/_examples.py
--rw-r--r--   0        0        0   142638 2024-01-26 17:19:50.215528 vocalpy-0.9.0/src/vocalpy/examples/bells.wav
--rw-r--r--   0        0        0   126320 2024-01-26 17:19:50.215528 vocalpy-0.9.0/src/vocalpy/examples/flashcam.wav
--rw-r--r--   0        0        0   130946 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/examples/samba.wav
--rw-r--r--   0        0        0   100696 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/examples/simple.wav
--rw-r--r--   0        0        0       95 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/__init__.py
--rw-r--r--   0        0        0    20055 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/sat.py
--rw-r--r--   0        0        0       95 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/__init__.py
--rw-r--r--   0        0        0     6840 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/detect_peaks.py
--rw-r--r--   0        0        0    17164 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/features.py
--rw-r--r--   0        0        0    20246 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/fundamental.py
--rw-r--r--   0        0        0     3940 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/signal.py
--rw-r--r--   0        0        0     1690 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/sound.py
--rw-r--r--   0        0        0     5185 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature_extractor.py
--rw-r--r--   0        0        0     1869 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/feature_file.py
--rw-r--r--   0        0        0     1401 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/features.py
--rw-r--r--   0        0        0      126 2023-09-28 01:29:32.668511 vocalpy-0.9.0/src/vocalpy/metrics/__init__.py
--rw-r--r--   0        0        0      172 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/metrics/segmentation/__init__.py
--rw-r--r--   0        0        0    31339 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/metrics/segmentation/ir.py
--rw-r--r--   0        0        0      882 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/params.py
--rw-r--r--   0        0        0     1159 2023-09-29 20:50:59.859125 vocalpy-0.9.0/src/vocalpy/paths.py
--rw-r--r--   0        0        0      309 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/plot/__init__.py
--rw-r--r--   0        0        0     7258 2023-09-12 01:52:43.314986 vocalpy-0.9.0/src/vocalpy/plot/annot.py
--rw-r--r--   0        0        0     5230 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/plot/spect.py
--rw-r--r--   0        0        0      508 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/segment/__init__.py
--rw-r--r--   0        0        0    20942 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/segment/ava.py
--rw-r--r--   0        0        0     9565 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/segment/meansquared.py
--rw-r--r--   0        0        0     5402 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/segmenter.py
--rw-r--r--   0        0        0    22648 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/segments.py
--rw-r--r--   0        0        0      928 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/sequence.py
--rw-r--r--   0        0        0      109 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/signal/__init__.py
--rw-r--r--   0        0        0     4370 2024-02-12 02:46:58.476428 vocalpy-0.9.0/src/vocalpy/signal/audio.py
--rw-r--r--   0        0        0      644 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/signal/filter.py
--rw-r--r--   0        0        0     7811 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/sound.py
--rw-r--r--   0        0        0      219 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectral/__init__.py
--rw-r--r--   0        0        0     6273 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectral/sat.py
--rw-r--r--   0        0        0     6675 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectral/soundsig.py
--rw-r--r--   0        0        0     3205 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectrogram.py
--rw-r--r--   0        0        0     1442 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/spectrogram_file.py
--rw-r--r--   0        0        0     9448 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectrogram_maker.py
--rw-r--r--   0        0        0      734 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/spectrogram_parameters.py
--rw-r--r--   0        0        0     1576 2024-03-06 03:50:43.265345 vocalpy-0.9.0/src/vocalpy/unit.py
--rw-r--r--   0        0        0      356 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/validators/__init__.py
--rw-r--r--   0        0        0      699 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/validators/attrs.py
--rw-r--r--   0        0        0     4936 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/validators/validators.py
--rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      224 2024-05-16 03:52:17.046400 vocalpy-0.9.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2744 2023-09-19 17:23:06.009955 vocalpy-0.9.0/tests/fixtures/annot.py
--rw-r--r--   0        0        0     3351 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/fixtures/audio.py
--rw-r--r--   0        0        0      134 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/fixtures/dask.py
--rw-r--r--   0        0        0      834 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/fixtures/datasets.py
--rw-r--r--   0        0        0      210 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/fixtures/paths.py
--rw-r--r--   0        0        0      983 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/fixtures/segments.py
--rw-r--r--   0        0        0     2942 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/fixtures/spect.py
--rw-r--r--   0        0        0     1278 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/fixtures/test_data.py
--rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/__init__.py
--rw-r--r--   0        0        0     9340 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/generate_ava_segment_text_files_from_jourjine_et_al_2023.py
--rw-r--r--   0        0        0     1126 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/generate_test_audio_for_ava_segment_from_jourjine_etal_2023.py
--rw-r--r--   0        0        0     7048 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/scripts/generate_data_for_tests.py
--rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.9.0/tests/test__spectrogram/__init__.py
--rw-r--r--   0        0        0     9635 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test__spectrogram/test_data_type.py
--rw-r--r--   0        0        0     2719 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_annotation_file.py
--rw-r--r--   0        0        0      992 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_audio_file.py
--rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.9.0/tests/test_examples/__init__.py
--rw-r--r--   0        0        0      915 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/test_examples/test__examples.py
--rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.9.0/tests/test_feature/__init__.py
--rw-r--r--   0        0        0     8644 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_feature/test_sat.py
--rw-r--r--   0        0        0      206 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_feature_extractor.py
--rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.0/tests/test_metrics/__init__.py
--rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.0/tests/test_metrics/test_segmentation/__init__.py
--rw-r--r--   0        0        0    26736 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_metrics/test_segmentation/test_ir.py
--rw-r--r--   0        0        0      895 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_params.py
--rw-r--r--   0        0        0     2903 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_paths.py
--rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/test_segment/__init__.py
--rw-r--r--   0        0        0     3062 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_segment/test_ava.py
--rw-r--r--   0        0        0     2276 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_segment/test_meansquared.py
--rw-r--r--   0        0        0     3222 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_segmenter.py
--rw-r--r--   0        0        0    23811 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_segments.py
--rw-r--r--   0        0        0      487 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_sequence.py
--rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/test_signal/__init__.py
--rw-r--r--   0        0        0      886 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_signal/test_audio.py
--rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/test_signal/test_spectrogram.py
--rw-r--r--   0        0        0     8822 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/test_sound.py
--rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.9.0/tests/test_spectral/__init__.py
--rw-r--r--   0        0        0     1187 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_spectral/test_sat.py
--rw-r--r--   0        0        0     1007 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_spectrogram.py
--rw-r--r--   0        0        0     1500 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_spectrogram_file.py
--rw-r--r--   0        0        0     4628 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_spectrogram_maker.py
--rw-r--r--   0        0        0      848 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_unit.py
--rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.0/tests/test_validators/__init__.py
--rw-r--r--   0        0        0     3272 2023-12-30 01:52:55.173763 vocalpy-0.9.0/tests/test_validators/test_validators.py
--rw-r--r--   0        0        0        0 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_vendor/__init__.py
--rw-r--r--   0        0        0     1280 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_vendor/test_evfuncs.py
--rw-r--r--   0        0        0    18176 1970-01-01 00:00:00.000000 vocalpy-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      650 2024-01-26 17:19:50.207528 vocalpy-0.9.1/.all-contributorsrc
+-rw-r--r--   0        0        0     1307 2023-09-19 17:23:06.009955 vocalpy-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-08-20 18:48:42.054440 vocalpy-0.9.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-08-20 18:48:42.054440 vocalpy-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      705 2024-01-17 01:58:19.551347 vocalpy-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      463 2024-02-22 13:15:42.873235 vocalpy-0.9.1/.gitignore
+-rw-r--r--   0        0        0      769 2023-08-20 18:48:42.054440 vocalpy-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      334 2023-09-29 20:50:59.859125 vocalpy-0.9.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5556 2023-09-19 17:23:06.009955 vocalpy-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1867 2023-08-20 18:48:42.054440 vocalpy-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1540 2023-04-18 02:08:12.226241 vocalpy-0.9.1/LICENSE
+-rw-r--r--   0        0        0    15851 2024-02-12 02:46:58.472428 vocalpy-0.9.1/README.md
+-rw-r--r--   0        0        0       46 2024-02-24 00:45:51.665844 vocalpy-0.9.1/codecov.yml
+-rw-r--r--   0        0        0     8777 2024-05-21 14:27:41.351016 vocalpy-0.9.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0      775 2024-02-22 13:15:42.873235 vocalpy-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0    29965 2023-08-20 18:48:42.054440 vocalpy-0.9.1/docs/_static/vocalpy-logomark.png
+-rw-r--r--   0        0        0   285798 2023-08-20 18:48:42.054440 vocalpy-0.9.1/docs/_static/vocalpy-primary.png
+-rw-r--r--   0        0        0   194159 2023-08-20 18:48:42.054440 vocalpy-0.9.1/docs/_static/vocalpy-secondary.png
+-rw-r--r--   0        0        0      612 2023-12-30 13:28:54.397449 vocalpy-0.9.1/docs/_templates/class.rst
+-rw-r--r--   0        0        0     1177 2023-12-30 13:28:54.397449 vocalpy-0.9.1/docs/_templates/module.rst
+-rw-r--r--   0        0        0     1279 2024-05-16 03:52:17.046400 vocalpy-0.9.1/docs/api/index.rst
+-rw-r--r--   0        0        0     3862 2024-04-02 23:44:46.834318 vocalpy-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0    17033 2023-09-19 17:23:06.009955 vocalpy-0.9.1/docs/fa2023/FA2023_template.tex
+-rw-r--r--   0        0        0  1735302 2023-09-19 18:23:52.210288 vocalpy-0.9.1/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf
+-rw-r--r--   0        0        0     8966 2023-09-19 17:23:06.009955 vocalpy-0.9.1/docs/fa2023/fa2023.sty
+-rw-r--r--   0        0        0  1008143 2023-08-20 18:48:42.058440 vocalpy-0.9.1/docs/fa2023/footer_logo_aia.png
+-rw-r--r--   0        0        0   313241 2023-08-20 18:48:42.062440 vocalpy-0.9.1/docs/fa2023/footer_logo_eaa.jpg
+-rw-r--r--   0        0        0    10783 2023-08-20 18:48:42.062440 vocalpy-0.9.1/docs/fa2023/forum-acusticum-2023.bib
+-rw-r--r--   0        0        0    18787 2023-08-20 18:48:42.062440 vocalpy-0.9.1/docs/fa2023/header.png
+-rw-r--r--   0        0        0    39228 2023-08-20 18:48:42.062440 vocalpy-0.9.1/docs/fa2023/header_onda.png
+-rw-r--r--   0        0        0    17958 2024-02-03 13:05:38.608298 vocalpy-0.9.1/docs/fa2023/main.tex
+-rw-r--r--   0        0        0   118445 2023-08-20 18:48:42.070440 vocalpy-0.9.1/docs/fa2023/voc-fig1-model.png
+-rw-r--r--   0        0        0      141 2024-01-26 17:19:50.211528 vocalpy-0.9.1/docs/getting_started/index.md
+-rw-r--r--   0        0        0     2503 2024-01-26 17:19:50.211528 vocalpy-0.9.1/docs/getting_started/installation.md
+-rw-r--r--   0        0        0    10269 2024-05-19 15:06:17.828973 vocalpy-0.9.1/docs/getting_started/quickstart.md
+-rw-r--r--   0        0        0     3554 2024-01-26 17:19:50.211528 vocalpy-0.9.1/docs/index.md
+-rw-r--r--   0        0        0      800 2023-08-20 18:48:42.070440 vocalpy-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0      881 2023-09-19 17:23:06.009955 vocalpy-0.9.1/docs/nitpick-ignore.txt
+-rw-r--r--   0        0        0     4147 2024-01-26 17:19:50.211528 vocalpy-0.9.1/docs/user/background.md
+-rw-r--r--   0        0        0       67 2024-04-03 03:02:45.940030 vocalpy-0.9.1/docs/user/howto/index.md
+-rw-r--r--   0        0        0    15636 2024-04-09 02:06:31.842592 vocalpy-0.9.1/docs/user/howto/segmentation-ir-metrics.md
+-rw-r--r--   0        0        0      343 2024-04-03 03:02:45.940030 vocalpy-0.9.1/docs/user/index.md
+-rw-r--r--   0        0        0    10030 2024-02-12 02:46:58.472428 vocalpy-0.9.1/docs/user/whatisvocalpy.md
+-rw-r--r--   0        0        0     8492 2024-02-24 00:45:51.665844 vocalpy-0.9.1/noxfile.py
+-rw-r--r--   0        0        0     2438 2024-05-21 14:27:41.335016 vocalpy-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.1/src/scripts/example_data/.gitkeep
+-rw-r--r--   0        0        0     6836 2024-02-22 13:15:42.873235 vocalpy-0.9.1/src/scripts/make_example_data.py
+-rw-r--r--   0        0        0      804 2024-05-21 14:27:41.347016 vocalpy-0.9.1/src/vocalpy/__about__.py
+-rw-r--r--   0        0        0     1866 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 17:19:50.211528 vocalpy-0.9.1/src/vocalpy/_spectrogram/__init__.py
+-rw-r--r--   0        0        0     9382 2024-04-09 12:04:39.858685 vocalpy-0.9.1/src/vocalpy/_spectrogram/data_type.py
+-rw-r--r--   0        0        0       36 2024-02-12 02:46:58.472428 vocalpy-0.9.1/src/vocalpy/_vendor/__init__.py
+-rw-r--r--   0        0        0     6910 2024-02-12 02:46:58.472428 vocalpy-0.9.1/src/vocalpy/_vendor/evfuncs.py
+-rw-r--r--   0        0        0     1092 2023-08-20 18:48:42.070440 vocalpy-0.9.1/src/vocalpy/annotation.py
+-rw-r--r--   0        0        0     1830 2024-04-09 12:04:39.858685 vocalpy-0.9.1/src/vocalpy/annotation_file.py
+-rw-r--r--   0        0        0        0 2023-08-20 18:48:42.070440 vocalpy-0.9.1/src/vocalpy/annotator.py
+-rw-r--r--   0        0        0      541 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/audio_file.py
+-rw-r--r--   0        0        0       78 2023-09-28 11:53:11.545674 vocalpy-0.9.1/src/vocalpy/constants.py
+-rw-r--r--   0        0        0     2479 2024-04-09 12:04:39.858685 vocalpy-0.9.1/src/vocalpy/dataset_file.py
+-rw-r--r--   0        0        0   240044 2024-01-26 17:19:50.215528 vocalpy-0.9.1/src/vocalpy/examples/BM003.wav
+-rw-r--r--   0        0        0      186 2024-02-22 13:15:42.873235 vocalpy-0.9.1/src/vocalpy/examples/__init__.py
+-rw-r--r--   0        0        0    10579 2024-05-21 13:48:27.349085 vocalpy-0.9.1/src/vocalpy/examples/_examples.py
+-rw-r--r--   0        0        0   142638 2024-01-26 17:19:50.215528 vocalpy-0.9.1/src/vocalpy/examples/bells.wav
+-rw-r--r--   0        0        0   126320 2024-01-26 17:19:50.215528 vocalpy-0.9.1/src/vocalpy/examples/flashcam.wav
+-rw-r--r--   0        0        0   130946 2024-01-26 17:19:50.219528 vocalpy-0.9.1/src/vocalpy/examples/samba.wav
+-rw-r--r--   0        0        0   100696 2024-01-26 17:19:50.219528 vocalpy-0.9.1/src/vocalpy/examples/simple.wav
+-rw-r--r--   0        0        0       95 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/__init__.py
+-rw-r--r--   0        0        0    20055 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/sat.py
+-rw-r--r--   0        0        0       95 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/soundsig/__init__.py
+-rw-r--r--   0        0        0     6840 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/soundsig/detect_peaks.py
+-rw-r--r--   0        0        0    17164 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/soundsig/features.py
+-rw-r--r--   0        0        0    20246 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/soundsig/fundamental.py
+-rw-r--r--   0        0        0     3940 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/soundsig/signal.py
+-rw-r--r--   0        0        0     1690 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/feature/soundsig/sound.py
+-rw-r--r--   0        0        0     5293 2024-05-21 00:22:58.267622 vocalpy-0.9.1/src/vocalpy/feature_extractor.py
+-rw-r--r--   0        0        0     1869 2024-04-09 12:04:39.862685 vocalpy-0.9.1/src/vocalpy/feature_file.py
+-rw-r--r--   0        0        0     1401 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/features.py
+-rw-r--r--   0        0        0      126 2023-09-28 01:29:32.668511 vocalpy-0.9.1/src/vocalpy/metrics/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/metrics/segmentation/__init__.py
+-rw-r--r--   0        0        0    31339 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/metrics/segmentation/ir.py
+-rw-r--r--   0        0        0      882 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/params.py
+-rw-r--r--   0        0        0     1159 2023-09-29 20:50:59.859125 vocalpy-0.9.1/src/vocalpy/paths.py
+-rw-r--r--   0        0        0      309 2023-09-28 11:53:11.545674 vocalpy-0.9.1/src/vocalpy/plot/__init__.py
+-rw-r--r--   0        0        0     7255 2024-05-19 15:06:17.828973 vocalpy-0.9.1/src/vocalpy/plot/annot.py
+-rw-r--r--   0        0        0     5230 2024-04-09 12:04:39.862685 vocalpy-0.9.1/src/vocalpy/plot/spect.py
+-rw-r--r--   0        0        0      508 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/segment/__init__.py
+-rw-r--r--   0        0        0    20942 2024-04-09 12:04:39.862685 vocalpy-0.9.1/src/vocalpy/segment/ava.py
+-rw-r--r--   0        0        0     9565 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/segment/meansquared.py
+-rw-r--r--   0        0        0     5504 2024-05-21 00:22:58.267622 vocalpy-0.9.1/src/vocalpy/segmenter.py
+-rw-r--r--   0        0        0    22648 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/segments.py
+-rw-r--r--   0        0        0      928 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/sequence.py
+-rw-r--r--   0        0        0      109 2024-01-26 17:19:50.219528 vocalpy-0.9.1/src/vocalpy/signal/__init__.py
+-rw-r--r--   0        0        0     4370 2024-02-12 02:46:58.476428 vocalpy-0.9.1/src/vocalpy/signal/audio.py
+-rw-r--r--   0        0        0      644 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/signal/filter.py
+-rw-r--r--   0        0        0     7811 2024-04-03 03:02:45.944030 vocalpy-0.9.1/src/vocalpy/sound.py
+-rw-r--r--   0        0        0      219 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/spectral/__init__.py
+-rw-r--r--   0        0        0     6273 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/spectral/sat.py
+-rw-r--r--   0        0        0     6675 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/spectral/soundsig.py
+-rw-r--r--   0        0        0     3205 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/spectrogram.py
+-rw-r--r--   0        0        0     1442 2024-04-09 12:04:39.862685 vocalpy-0.9.1/src/vocalpy/spectrogram_file.py
+-rw-r--r--   0        0        0     9556 2024-05-21 00:22:58.267622 vocalpy-0.9.1/src/vocalpy/spectrogram_maker.py
+-rw-r--r--   0        0        0      734 2024-01-26 17:19:50.219528 vocalpy-0.9.1/src/vocalpy/spectrogram_parameters.py
+-rw-r--r--   0        0        0     1576 2024-03-06 03:50:43.265345 vocalpy-0.9.1/src/vocalpy/unit.py
+-rw-r--r--   0        0        0      356 2023-09-28 11:53:11.545674 vocalpy-0.9.1/src/vocalpy/validators/__init__.py
+-rw-r--r--   0        0        0      699 2023-09-28 11:53:11.545674 vocalpy-0.9.1/src/vocalpy/validators/attrs.py
+-rw-r--r--   0        0        0     4936 2024-05-16 03:52:17.046400 vocalpy-0.9.1/src/vocalpy/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-18 02:08:12.226241 vocalpy-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      224 2024-05-16 03:52:17.046400 vocalpy-0.9.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2744 2023-09-19 17:23:06.009955 vocalpy-0.9.1/tests/fixtures/annot.py
+-rw-r--r--   0        0        0     3351 2024-04-03 03:02:45.944030 vocalpy-0.9.1/tests/fixtures/audio.py
+-rw-r--r--   0        0        0      134 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/fixtures/dask.py
+-rw-r--r--   0        0        0      834 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/fixtures/datasets.py
+-rw-r--r--   0        0        0      210 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/fixtures/paths.py
+-rw-r--r--   0        0        0      983 2024-02-24 00:45:51.669844 vocalpy-0.9.1/tests/fixtures/segments.py
+-rw-r--r--   0        0        0     2942 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/fixtures/spect.py
+-rw-r--r--   0        0        0     1278 2024-02-24 00:45:51.669844 vocalpy-0.9.1/tests/fixtures/test_data.py
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/scripts/generate_ava_segment_test_data/__init__.py
+-rw-r--r--   0        0        0     9340 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/scripts/generate_ava_segment_test_data/generate_ava_segment_text_files_from_jourjine_et_al_2023.py
+-rw-r--r--   0        0        0     1126 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/scripts/generate_ava_segment_test_data/generate_test_audio_for_ava_segment_from_jourjine_etal_2023.py
+-rw-r--r--   0        0        0     7048 2024-02-24 00:45:51.669844 vocalpy-0.9.1/tests/scripts/generate_data_for_tests.py
+-rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.9.1/tests/test__spectrogram/__init__.py
+-rw-r--r--   0        0        0     9635 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test__spectrogram/test_data_type.py
+-rw-r--r--   0        0        0     2719 2024-03-06 03:50:43.265345 vocalpy-0.9.1/tests/test_annotation_file.py
+-rw-r--r--   0        0        0      992 2024-03-06 03:50:43.265345 vocalpy-0.9.1/tests/test_audio_file.py
+-rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.9.1/tests/test_examples/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-21 13:48:27.349085 vocalpy-0.9.1/tests/test_examples/test__examples.py
+-rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.9.1/tests/test_feature/__init__.py
+-rw-r--r--   0        0        0     8644 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/test_feature/test_sat.py
+-rw-r--r--   0        0        0      206 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/test_feature_extractor.py
+-rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.1/tests/test_metrics/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.1/tests/test_metrics/test_segmentation/__init__.py
+-rw-r--r--   0        0        0    26736 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test_metrics/test_segmentation/test_ir.py
+-rw-r--r--   0        0        0      895 2024-04-03 03:02:45.944030 vocalpy-0.9.1/tests/test_params.py
+-rw-r--r--   0        0        0     2903 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test_paths.py
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.1/tests/test_segment/__init__.py
+-rw-r--r--   0        0        0     3062 2024-04-03 03:02:45.944030 vocalpy-0.9.1/tests/test_segment/test_ava.py
+-rw-r--r--   0        0        0     2276 2024-04-03 03:02:45.944030 vocalpy-0.9.1/tests/test_segment/test_meansquared.py
+-rw-r--r--   0        0        0     3222 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/test_segmenter.py
+-rw-r--r--   0        0        0    23811 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/test_segments.py
+-rw-r--r--   0        0        0      487 2024-04-03 03:02:45.944030 vocalpy-0.9.1/tests/test_sequence.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.1/tests/test_signal/__init__.py
+-rw-r--r--   0        0        0      886 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test_signal/test_audio.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.1/tests/test_signal/test_spectrogram.py
+-rw-r--r--   0        0        0     8822 2024-02-24 00:45:51.669844 vocalpy-0.9.1/tests/test_sound.py
+-rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.9.1/tests/test_spectral/__init__.py
+-rw-r--r--   0        0        0     1187 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/test_spectral/test_sat.py
+-rw-r--r--   0        0        0     1007 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test_spectrogram.py
+-rw-r--r--   0        0        0     1500 2024-03-06 03:50:43.265345 vocalpy-0.9.1/tests/test_spectrogram_file.py
+-rw-r--r--   0        0        0     4628 2024-05-16 03:52:17.050400 vocalpy-0.9.1/tests/test_spectrogram_maker.py
+-rw-r--r--   0        0        0      848 2024-03-06 03:50:43.265345 vocalpy-0.9.1/tests/test_unit.py
+-rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.1/tests/test_validators/__init__.py
+-rw-r--r--   0        0        0     3272 2023-12-30 01:52:55.173763 vocalpy-0.9.1/tests/test_validators/test_validators.py
+-rw-r--r--   0        0        0        0 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test_vendor/__init__.py
+-rw-r--r--   0        0        0     1280 2024-02-12 02:46:58.476428 vocalpy-0.9.1/tests/test_vendor/test_evfuncs.py
+-rw-r--r--   0        0        0    18176 1970-01-01 00:00:00.000000 vocalpy-0.9.1/PKG-INFO
```

### Comparing `vocalpy-0.9.0/.all-contributorsrc` & `vocalpy-0.9.1/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `vocalpy-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md` & `vocalpy-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/.github/workflows/ci.yml` & `vocalpy-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/.pre-commit-config.yaml` & `vocalpy-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/CODE_OF_CONDUCT.md` & `vocalpy-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/CONTRIBUTING.md` & `vocalpy-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/LICENSE` & `vocalpy-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/README.md` & `vocalpy-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/CHANGELOG.md` & `vocalpy-0.9.1/docs/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.1]
+### Fixed
+- Fix `ConnectionError` when importing VocalPy without internet connection
+  [#153](https://github.com/vocalpy/vocalpy/pull/153).
+  Fixes [#152](https://github.com/vocalpy/vocalpy/issues/152).
+
 ## [0.9.0]
 ### Added
 - Add attributes `channels`, `samples`, and `duration` to `vocalpy.Sound`
   [#124](https://github.com/vocalpy/vocalpy/pull/124).
   Fixes [#90](https://github.com/vocalpy/vocalpy/issues/90).
 - Add functionality to `vocalpy.segment.ava.segment` to replicate segmenting in
   papers that use this method
```

### Comparing `vocalpy-0.9.0/docs/Makefile` & `vocalpy-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/_static/vocalpy-logomark.png` & `vocalpy-0.9.1/docs/_static/vocalpy-logomark.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/_static/vocalpy-primary.png` & `vocalpy-0.9.1/docs/_static/vocalpy-primary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/_static/vocalpy-secondary.png` & `vocalpy-0.9.1/docs/_static/vocalpy-secondary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/_templates/class.rst` & `vocalpy-0.9.1/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/_templates/module.rst` & `vocalpy-0.9.1/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/api/index.rst` & `vocalpy-0.9.1/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/conf.py` & `vocalpy-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/FA2023_template.tex` & `vocalpy-0.9.1/docs/fa2023/FA2023_template.tex`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf` & `vocalpy-0.9.1/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/fa2023.sty` & `vocalpy-0.9.1/docs/fa2023/fa2023.sty`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/footer_logo_aia.png` & `vocalpy-0.9.1/docs/fa2023/footer_logo_aia.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/footer_logo_eaa.jpg` & `vocalpy-0.9.1/docs/fa2023/footer_logo_eaa.jpg`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/forum-acusticum-2023.bib` & `vocalpy-0.9.1/docs/fa2023/forum-acusticum-2023.bib`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/header.png` & `vocalpy-0.9.1/docs/fa2023/header.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/header_onda.png` & `vocalpy-0.9.1/docs/fa2023/header_onda.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/main.tex` & `vocalpy-0.9.1/docs/fa2023/main.tex`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/fa2023/voc-fig1-model.png` & `vocalpy-0.9.1/docs/fa2023/voc-fig1-model.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/getting_started/installation.md` & `vocalpy-0.9.1/docs/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/getting_started/quickstart.md` & `vocalpy-0.9.1/docs/getting_started/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 +++
 
 Let's use one of those classes, `SpectrogramMaker`, to make a spectrogram from each one of the wav files that we loaded above.
 
 We'll write a brief snippet to do so, and then we'll explain what we did.
 
 ```{code-cell} ipython3
+:tags: [hide-output]
 params = {'n_fft': 512, 'hop_length': 64}
 callback = voc.spectrogram
 spect_maker = voc.SpectrogramMaker(callback=callback, params=params)
 spects = spect_maker.make(sounds, parallelize=True)
 ```
 
 Notice a couple of things about this snippet:
```

### Comparing `vocalpy-0.9.0/docs/index.md` & `vocalpy-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/make.bat` & `vocalpy-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/nitpick-ignore.txt` & `vocalpy-0.9.1/docs/nitpick-ignore.txt`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/user/background.md` & `vocalpy-0.9.1/docs/user/background.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/user/howto/segmentation-ir-metrics.md` & `vocalpy-0.9.1/docs/user/howto/segmentation-ir-metrics.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/docs/user/whatisvocalpy.md` & `vocalpy-0.9.1/docs/user/whatisvocalpy.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/noxfile.py` & `vocalpy-0.9.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/pyproject.toml` & `vocalpy-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "vocalpy"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
 description = "A core package for acoustic communication research in Python"
-version = "0.9.0"
+version = "0.9.1"
 classifiers = [
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `vocalpy-0.9.0/src/scripts/make_example_data.py` & `vocalpy-0.9.1/src/scripts/make_example_data.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/__about__.py` & `vocalpy-0.9.1/src/vocalpy/__about__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     base_dir = None
 
 
 __title__ = "vocalpy"
 __summary__ = "A core package for acoustic communication research in Python"
 __uri__ = "https://github.com/vocalpy/vocalpy"
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `vocalpy-0.9.0/src/vocalpy/__init__.py` & `vocalpy-0.9.1/src/vocalpy/__init__.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/_spectrogram/data_type.py` & `vocalpy-0.9.1/src/vocalpy/_spectrogram/data_type.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/_vendor/evfuncs.py` & `vocalpy-0.9.1/src/vocalpy/_vendor/evfuncs.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/annotation.py` & `vocalpy-0.9.1/src/vocalpy/annotation.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/annotation_file.py` & `vocalpy-0.9.1/src/vocalpy/annotation_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/audio_file.py` & `vocalpy-0.9.1/src/vocalpy/audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/dataset_file.py` & `vocalpy-0.9.1/src/vocalpy/dataset_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/examples/BM003.wav` & `vocalpy-0.9.1/src/vocalpy/examples/BM003.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/examples/_examples.py` & `vocalpy-0.9.1/src/vocalpy/examples/_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import pathlib
 import shutil
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Union
 
 import pooch
+import requests.exceptions
 
 if TYPE_CHECKING:
     import vocalpy
 
     ExampleType = Union[
         pathlib.Path,
         list[pathlib.Path],
@@ -128,25 +129,21 @@
         requires_download=True,
     ),
 ]
 
 
 REGISTRY = {example.name: example for example in EXAMPLE_METADATA}
 
-
 VOCALPY_DATA_DIR = "VOCALPY_DATA_DIR"
 
-
 ZENODO_DATASET_BASE_URL = "doi:10.5281/zenodo.10688472"
 
-
 POOCH = pooch.create(
     path=pooch.os_cache("vocalpy"), base_url=ZENODO_DATASET_BASE_URL, registry=None, env=VOCALPY_DATA_DIR
 )
-POOCH.load_registry_from_doi()
 
 
 def get_cache_dir() -> pathlib.Path:
     """Returns path to directory where example data is cached.
 
     By
     """
@@ -216,14 +213,21 @@
             )
     else:
         return_type = "path"
     import vocalpy  # avoid circular import
 
     example_: ExampleMeta = REGISTRY[name]
     if example_.requires_download:
+        try:
+            POOCH.load_registry_from_doi()
+        except requests.exceptions.ConnectionError as e:
+            raise ConnectionError(
+                "Unable to connect to registry to download example dataset. "
+                "This may be due to an issue with an internet connection."
+            ) from e
         if example_.fname.endswith(".tar.gz"):
             path = POOCH.fetch(example_.fname, processor=pooch.Untar())
         else:
             path = POOCH.fetch(example_.fname)
         if isinstance(path, list):
             path = [pathlib.Path(path_) for path_ in path]
         else:
```

### Comparing `vocalpy-0.9.0/src/vocalpy/examples/bells.wav` & `vocalpy-0.9.1/src/vocalpy/examples/bells.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/examples/flashcam.wav` & `vocalpy-0.9.1/src/vocalpy/examples/flashcam.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/examples/samba.wav` & `vocalpy-0.9.1/src/vocalpy/examples/samba.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/examples/simple.wav` & `vocalpy-0.9.1/src/vocalpy/examples/simple.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature/sat.py` & `vocalpy-0.9.1/src/vocalpy/feature/sat.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature/soundsig/detect_peaks.py` & `vocalpy-0.9.1/src/vocalpy/feature/soundsig/detect_peaks.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature/soundsig/features.py` & `vocalpy-0.9.1/src/vocalpy/feature/soundsig/features.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature/soundsig/fundamental.py` & `vocalpy-0.9.1/src/vocalpy/feature/soundsig/fundamental.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature/soundsig/signal.py` & `vocalpy-0.9.1/src/vocalpy/feature/soundsig/signal.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature/soundsig/sound.py` & `vocalpy-0.9.1/src/vocalpy/feature/soundsig/sound.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/feature_extractor.py` & `vocalpy-0.9.1/src/vocalpy/feature_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,17 @@
             invalid_params = [param for param in params if param not in signature.parameters]
             raise ValueError(
                 f"Invalid params for callback: {invalid_params}\n" f"Callback parameters are: {signature.parameters}"
             )
 
         self.params = params
 
+    def __repr__(self):
+        return f"FeatureExtractor(callback={self.callback}, params={self.params})"
+
     def extract(self, source: FeatureSource, parallelize: bool = True) -> Features | list[Features]:
         from . import Segment, Segments, Sound, Features
 
         if not isinstance(source, (list, Segment, Segments, Sound)):
             raise TypeError(
                 "`source` to extract features from must be an instance of a `Sound`, a `Segment`, "
                 f"a `list` of `Sound` or `Segment` instances, or a `Segments` instance, "
```

### Comparing `vocalpy-0.9.0/src/vocalpy/feature_file.py` & `vocalpy-0.9.1/src/vocalpy/feature_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/features.py` & `vocalpy-0.9.1/src/vocalpy/features.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/metrics/segmentation/ir.py` & `vocalpy-0.9.1/src/vocalpy/metrics/segmentation/ir.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/params.py` & `vocalpy-0.9.1/src/vocalpy/params.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/paths.py` & `vocalpy-0.9.1/src/vocalpy/paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/plot/annot.py` & `vocalpy-0.9.1/src/vocalpy/plot/annot.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     """
     if ax is None:
         fig, ax = plt.subplots
 
     if label_color_map is None:
         if lbl is not None:
             labelset = set(lbl)
-            cmap = plt.cm.get_cmap("tab20")
+            cmap = plt.get_cmap("tab20")
             colors = [cmap(ind) for ind in range(len(labelset))]
             label_color_map = {label: color for label, color in zip(labelset, colors)}
 
     labels_to_plot = []
     label_plot_times = []
     rectangles = []
     if lbl is not None:
```

### Comparing `vocalpy-0.9.0/src/vocalpy/plot/spect.py` & `vocalpy-0.9.1/src/vocalpy/plot/spect.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/segment/ava.py` & `vocalpy-0.9.1/src/vocalpy/segment/ava.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/segment/meansquared.py` & `vocalpy-0.9.1/src/vocalpy/segment/meansquared.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/segmenter.py` & `vocalpy-0.9.1/src/vocalpy/segmenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,18 @@
             invalid_params = [param for param in params if param not in signature.parameters]
             raise ValueError(
                 f"Invalid params for callback: {invalid_params}\n" f"Callback parameters are: {signature.parameters}"
             )
 
         self.params = params
 
+
+    def __repr__(self):
+        return f"Segmenter(callback={self.callback}, params={self.params})"
+
     def segment(
         self,
         sound: Sound | AudioFile | list[Sound | AudioFile],
         parallelize: bool = True,
     ) -> Segments | list[Segments]:
         """Segment sound.
```

### Comparing `vocalpy-0.9.0/src/vocalpy/segments.py` & `vocalpy-0.9.1/src/vocalpy/segments.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/sequence.py` & `vocalpy-0.9.1/src/vocalpy/sequence.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/signal/audio.py` & `vocalpy-0.9.1/src/vocalpy/signal/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/signal/filter.py` & `vocalpy-0.9.1/src/vocalpy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/sound.py` & `vocalpy-0.9.1/src/vocalpy/sound.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/spectral/sat.py` & `vocalpy-0.9.1/src/vocalpy/spectral/sat.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/spectral/soundsig.py` & `vocalpy-0.9.1/src/vocalpy/spectral/soundsig.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/spectrogram.py` & `vocalpy-0.9.1/src/vocalpy/spectrogram.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/spectrogram_file.py` & `vocalpy-0.9.1/src/vocalpy/spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/spectrogram_maker.py` & `vocalpy-0.9.1/src/vocalpy/spectrogram_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,17 @@
             invalid_params = [param for param in params if param not in signature.parameters]
             raise ValueError(
                 f"Invalid params for callback: {invalid_params}\n" f"Callback parameters are: {signature.parameters}"
             )
 
         self.params = params
 
+    def __repr__(self):
+        return f"FeatureExtractor(callback={self.callback}, params={self.params})"
+
     def make(
         self,
         sound: Sound | AudioFile | Sequence[Sound | AudioFile],
         parallelize: bool = True,
     ) -> Spectrogram | List[Spectrogram]:
         """Make spectrogram(s) from audio.
```

### Comparing `vocalpy-0.9.0/src/vocalpy/spectrogram_parameters.py` & `vocalpy-0.9.1/src/vocalpy/spectrogram_parameters.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/unit.py` & `vocalpy-0.9.1/src/vocalpy/unit.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/validators/attrs.py` & `vocalpy-0.9.1/src/vocalpy/validators/attrs.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/src/vocalpy/validators/validators.py` & `vocalpy-0.9.1/src/vocalpy/validators/validators.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/fixtures/annot.py` & `vocalpy-0.9.1/tests/fixtures/annot.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/fixtures/audio.py` & `vocalpy-0.9.1/tests/fixtures/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/fixtures/datasets.py` & `vocalpy-0.9.1/tests/fixtures/datasets.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/fixtures/segments.py` & `vocalpy-0.9.1/tests/fixtures/segments.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/fixtures/spect.py` & `vocalpy-0.9.1/tests/fixtures/spect.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/fixtures/test_data.py` & `vocalpy-0.9.1/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/generate_ava_segment_text_files_from_jourjine_et_al_2023.py` & `vocalpy-0.9.1/tests/scripts/generate_ava_segment_test_data/generate_ava_segment_text_files_from_jourjine_et_al_2023.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/generate_test_audio_for_ava_segment_from_jourjine_etal_2023.py` & `vocalpy-0.9.1/tests/scripts/generate_ava_segment_test_data/generate_test_audio_for_ava_segment_from_jourjine_etal_2023.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/scripts/generate_data_for_tests.py` & `vocalpy-0.9.1/tests/scripts/generate_data_for_tests.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test__spectrogram/test_data_type.py` & `vocalpy-0.9.1/tests/test__spectrogram/test_data_type.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_annotation_file.py` & `vocalpy-0.9.1/tests/test_annotation_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_audio_file.py` & `vocalpy-0.9.1/tests/test_audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_feature/test_sat.py` & `vocalpy-0.9.1/tests/test_feature/test_sat.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_metrics/test_segmentation/test_ir.py` & `vocalpy-0.9.1/tests/test_metrics/test_segmentation/test_ir.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_params.py` & `vocalpy-0.9.1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_paths.py` & `vocalpy-0.9.1/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_segment/test_ava.py` & `vocalpy-0.9.1/tests/test_segment/test_ava.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_segment/test_meansquared.py` & `vocalpy-0.9.1/tests/test_segment/test_meansquared.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_segmenter.py` & `vocalpy-0.9.1/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_segments.py` & `vocalpy-0.9.1/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_signal/test_audio.py` & `vocalpy-0.9.1/tests/test_signal/test_audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_sound.py` & `vocalpy-0.9.1/tests/test_sound.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_spectral/test_sat.py` & `vocalpy-0.9.1/tests/test_spectral/test_sat.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_spectrogram.py` & `vocalpy-0.9.1/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_spectrogram_file.py` & `vocalpy-0.9.1/tests/test_spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_spectrogram_maker.py` & `vocalpy-0.9.1/tests/test_spectrogram_maker.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_unit.py` & `vocalpy-0.9.1/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_validators/test_validators.py` & `vocalpy-0.9.1/tests/test_validators/test_validators.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/tests/test_vendor/test_evfuncs.py` & `vocalpy-0.9.1/tests/test_vendor/test_evfuncs.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.9.0/PKG-INFO` & `vocalpy-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalpy
-Version: 0.9.0
+Version: 0.9.1
 Summary: A core package for acoustic communication research in Python
 Author-email: David Nicholson <nickledave@users.noreply.github.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

