# Comparing `tmp/torcheval_nightly-2024.5.8.tar.gz` & `tmp/torcheval_nightly-2024.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcheval_nightly-2024.5.8.tar", last modified: Wed May  8 12:09:50 2024, max compression
+gzip compressed data, was "torcheval_nightly-2024.5.9.tar", last modified: Thu May  9 12:08:51 2024, max compression
```

## Comparing `torcheval_nightly-2024.5.8.tar` & `torcheval_nightly-2024.5.9.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.997063 torcheval_nightly-2024.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-08 12:09:49.997063 torcheval_nightly-2024.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:09:49.997063 torcheval_nightly-2024.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.977063 torcheval_nightly-2024.5.8/torcheval/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.981063 torcheval_nightly-2024.5.8/torcheval/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.981063 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.981063 torcheval_nightly-2024.5.8/torcheval/metrics/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/audio/fad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.985063 torcheval_nightly-2024.5.8/torcheval/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.985063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.985063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.985063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/frechet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.989063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/image/psnr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.989063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/num_collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/retrieval_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/retrieval_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.989063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.989063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/statistical/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/statistical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/statistical/wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.989063 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/word_information_preserved.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.989063 torcheval_nightly-2024.5.8/torcheval/metrics/image/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/retrieval_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/retrieval_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/metrics/statistical/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/statistical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/statistical/wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/synclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/metrics/text/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/text/word_information_preserved.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/metrics/window/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/window/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/window/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/window/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/window/normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/metrics/window/weighted_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/utils/random_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.993063 torcheval_nightly-2024.5.8/torcheval/utils/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/utils/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/utils/test_utils/dummy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/utils/test_utils/metric_class_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 12:02:57.000000 torcheval_nightly-2024.5.8/torcheval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:09:49.997063 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-08 12:09:49.000000 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-08 12:09:49.000000 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:09:49.000000 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 12:09:49.000000 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 12:09:49.000000 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:09:49.000000 torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.365020 torcheval_nightly-2024.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-09 12:08:51.365020 torcheval_nightly-2024.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:08:51.365020 torcheval_nightly-2024.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.345020 torcheval_nightly-2024.5.9/torcheval/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.345020 torcheval_nightly-2024.5.9/torcheval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.349020 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.349020 torcheval_nightly-2024.5.9/torcheval/metrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/audio/fad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.349020 torcheval_nightly-2024.5.9/torcheval/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/classification/recall_at_fixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.349020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.349020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.353020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/frechet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.353020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/image/psnr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.353020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/num_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/retrieval_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.357020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.357020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/statistical/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/statistical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/statistical/wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.357020 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/word_information_preserved.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.357020 torcheval_nightly-2024.5.9/torcheval/metrics/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.357020 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/retrieval_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.357020 torcheval_nightly-2024.5.9/torcheval/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.361020 torcheval_nightly-2024.5.9/torcheval/metrics/statistical/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/statistical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/statistical/wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/synclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.361020 torcheval_nightly-2024.5.9/torcheval/metrics/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/text/word_information_preserved.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.361020 torcheval_nightly-2024.5.9/torcheval/metrics/window/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/window/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/window/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/window/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/window/normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/metrics/window/weighted_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.361020 torcheval_nightly-2024.5.9/torcheval/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/utils/random_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.361020 torcheval_nightly-2024.5.9/torcheval/utils/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/utils/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/utils/test_utils/dummy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/utils/test_utils/metric_class_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 12:01:55.000000 torcheval_nightly-2024.5.9/torcheval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:08:51.361020 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-09 12:08:51.000000 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-09 12:08:51.000000 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:08:51.000000 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 12:08:51.000000 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 12:08:51.000000 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:08:51.000000 torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/zip-safe
```

### Comparing `torcheval_nightly-2024.5.8/LICENSE` & `torcheval_nightly-2024.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/PKG-INFO` & `torcheval_nightly-2024.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2024.5.8
+Version: 2024.5.9
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.5.8 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.5.9 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torcheval_nightly-2024.5.8/README.md` & `torcheval_nightly-2024.5.9/README.md`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/setup.py` & `torcheval_nightly-2024.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/auc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/cat.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/cat.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/max.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/max.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/mean.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/min.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/min.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/sum.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/aggregation/throughput.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/audio/fad.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/audio/fad.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/accuracy.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/auprc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/auroc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/binary_normalized_entropy.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/binned_auprc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/binned_auroc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/binned_precision_recall_curve.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/confusion_matrix.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/f1_score.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/precision.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/precision_recall_curve.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/recall.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/classification/recall_at_fixed_precision.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/auc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/mean.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/sum.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/aggregation/throughput.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/accuracy.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/auprc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/auroc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binary_normalized_entropy.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binned_auprc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binned_auroc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/binned_precision_recall_curve.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/confusion_matrix.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/f1_score.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/precision.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/precision_recall_curve.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/recall.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/classification/recall_at_fixed_precision.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/frechet.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/frechet.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/image/psnr.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/click_through_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/frequency.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/frequency.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/hit_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/num_collisions.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/num_collisions.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/reciprocal_rank.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/retrieval_precision.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/retrieval_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/retrieval_recall.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/retrieval_recall.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/ranking/weighted_calibration.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/mean_squared_error.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/regression/r2_score.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/statistical/wasserstein.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/statistical/wasserstein.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/tensor_utils.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/bleu.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/helper.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/perplexity.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/word_error_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/word_information_lost.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/functional/text/word_information_preserved.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/functional/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/image/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/image/fid.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/image/fid.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/image/psnr.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/image/ssim.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/metric.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/click_through_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/hit_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/reciprocal_rank.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/retrieval_precision.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/retrieval_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/retrieval_recall.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/retrieval_recall.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/ranking/weighted_calibration.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/regression/mean_squared_error.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/regression/r2_score.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/statistical/wasserstein.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/statistical/wasserstein.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/synclib.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/synclib.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/text/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/text/bleu.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/text/perplexity.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/text/word_error_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/text/word_information_lost.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/text/word_information_preserved.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/toolkit.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/toolkit.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/window/__init__.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/window/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/window/auroc.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/window/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/window/click_through_rate.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/window/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/window/mean_squared_error.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/window/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/window/normalized_entropy.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/window/normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/metrics/window/weighted_calibration.py` & `torcheval_nightly-2024.5.9/torcheval/metrics/window/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/utils/random_data.py` & `torcheval_nightly-2024.5.9/torcheval/utils/random_data.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/utils/test_utils/dummy_metric.py` & `torcheval_nightly-2024.5.9/torcheval/utils/test_utils/dummy_metric.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/utils/test_utils/metric_class_tester.py` & `torcheval_nightly-2024.5.9/torcheval/utils/test_utils/metric_class_tester.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval/version.py` & `torcheval_nightly-2024.5.9/torcheval/version.py`

 * *Files identical despite different names*

### Comparing `torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/PKG-INFO` & `torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2024.5.8
+Version: 2024.5.9
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.5.8 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.5.9 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torcheval_nightly-2024.5.8/torcheval_nightly.egg-info/SOURCES.txt` & `torcheval_nightly-2024.5.9/torcheval_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

