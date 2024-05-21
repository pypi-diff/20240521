# Comparing `tmp/pytorch_optimizer-2.9.1.tar.gz` & `tmp/pytorch_optimizer-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_optimizer-2.9.1.tar", max compression
+gzip compressed data, was "pytorch_optimizer-3.0.0.tar", max compression
```

## Comparing `pytorch_optimizer-2.9.1.tar` & `pytorch_optimizer-3.0.0.tar`

### file list

```diff
@@ -1,72 +1,94 @@
--rw-r--r--   0        0        0    11357 2023-05-19 12:09:37.191772 pytorch_optimizer-2.9.1/LICENSE
--rw-r--r--   0        0        0    60156 2023-05-19 12:09:37.191772 pytorch_optimizer-2.9.1/README.rst
--rw-r--r--   0        0        0     4305 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     7354 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/exception.py
--rw-r--r--   0        0        0     5633 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/optimizer.py
--rw-r--r--   0        0        0     2761 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/scheduler.py
--rw-r--r--   0        0        0      491 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/base/types.py
--rw-r--r--   0        0        0      131 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/__init__.py
--rw-r--r--   0        0        0      971 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/chebyshev.py
--rw-r--r--   0        0        0     4034 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py
--rw-r--r--   0        0        0        0 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/experimental/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py
--rw-r--r--   0        0        0     1255 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/linear_warmup.py
--rw-r--r--   0        0        0     1400 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/proportion.py
--rw-r--r--   0        0        0        0 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/__init__.py
--rw-r--r--   0        0        0     4464 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/a2grad.py
--rw-r--r--   0        0        0     6701 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabelief.py
--rw-r--r--   0        0        0     5470 2023-05-19 12:09:37.195772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabound.py
--rw-r--r--   0        0        0     3573 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adadelta.py
--rw-r--r--   0        0        0     8782 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adafactor.py
--rw-r--r--   0        0        0     6115 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adai.py
--rw-r--r--   0        0        0     4976 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamax.py
--rw-r--r--   0        0        0     4664 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamod.py
--rw-r--r--   0        0        0     6494 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamp.py
--rw-r--r--   0        0        0     6417 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adams.py
--rw-r--r--   0        0        0     6267 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adan.py
--rw-r--r--   0        0        0     5253 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adanorm.py
--rw-r--r--   0        0        0     6014 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adapnm.py
--rw-r--r--   0        0        0     4169 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adashift.py
--rw-r--r--   0        0        0     4138 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adasmooth.py
--rw-r--r--   0        0        0      784 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/agc.py
--rw-r--r--   0        0        0     3172 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/aggmo.py
--rw-r--r--   0        0        0     3618 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/alig.py
--rw-r--r--   0        0        0     5367 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/apollo.py
--rw-r--r--   0        0        0     4803 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/avagrad.py
--rw-r--r--   0        0        0    25140 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/dadapt.py
--rw-r--r--   0        0        0     6749 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/diffgrad.py
--rw-r--r--   0        0        0    10702 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fp16.py
--rw-r--r--   0        0        0     2764 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fromage.py
--rw-r--r--   0        0        0      396 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gc.py
--rw-r--r--   0        0        0     2517 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gravity.py
--rw-r--r--   0        0        0     7544 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gsam.py
--rw-r--r--   0        0        0     8316 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lamb.py
--rw-r--r--   0        0        0     3546 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lars.py
--rw-r--r--   0        0        0     4099 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lion.py
--rw-r--r--   0        0        0     4155 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lookahead.py
--rw-r--r--   0        0        0     6466 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/madgrad.py
--rw-r--r--   0        0        0     3172 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/msvag.py
--rw-r--r--   0        0        0     3595 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/nero.py
--rw-r--r--   0        0        0     4520 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/novograd.py
--rw-r--r--   0        0        0     4242 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pcgrad.py
--rw-r--r--   0        0        0     4233 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pid.py
--rw-r--r--   0        0        0     3741 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pnm.py
--rw-r--r--   0        0        0     4827 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhadam.py
--rw-r--r--   0        0        0     3249 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhm.py
--rw-r--r--   0        0        0     5622 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/radam.py
--rw-r--r--   0        0        0     6737 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger.py
--rw-r--r--   0        0        0    12385 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger21.py
--rw-r--r--   0        0        0    15565 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/rotograd.py
--rw-r--r--   0        0        0     4638 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sam.py
--rw-r--r--   0        0        0    10375 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgd.py
--rw-r--r--   0        0        0     4276 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgdp.py
--rw-r--r--   0        0        0    16137 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo.py
--rw-r--r--   0        0        0    20625 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo_utils.py
--rw-r--r--   0        0        0     5081 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sm3.py
--rw-r--r--   0        0        0     2852 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/srmm.py
--rw-r--r--   0        0        0     7165 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/swats.py
--rw-r--r--   0        0        0     8755 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/utils.py
--rw-r--r--   0        0        0     5306 2023-05-19 12:09:37.199772 pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/yogi.py
--rw-r--r--   0        0        0    62572 1970-01-01 00:00:00.000000 pytorch_optimizer-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 09:03:09.201609 pytorch_optimizer-3.0.0/LICENSE
+-rw-r--r--   0        0        0    49009 2024-05-21 09:03:09.201609 pytorch_optimizer-3.0.0/README.md
+-rw-r--r--   0        0        0     4810 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10573 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/base/__init__.py
+-rw-r--r--   0        0        0     1583 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/base/exception.py
+-rw-r--r--   0        0        0    10703 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/base/optimizer.py
+-rw-r--r--   0        0        0     2728 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/base/scheduler.py
+-rw-r--r--   0        0        0      574 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/base/types.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:03:09.205609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/__init__.py
+-rw-r--r--   0        0        0     9735 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/bi_tempered.py
+-rw-r--r--   0        0        0      946 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/cross_entropy.py
+-rw-r--r--   0        0        0     5461 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/dice.py
+-rw-r--r--   0        0        0      804 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/f1.py
+-rw-r--r--   0        0        0     3658 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/focal.py
+-rw-r--r--   0        0        0     4147 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/jaccard.py
+-rw-r--r--   0        0        0     1306 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/ldam.py
+-rw-r--r--   0        0        0     1527 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/lovasz.py
+-rw-r--r--   0        0        0      846 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/loss/tversky.py
+-rw-r--r--   0        0        0      131 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/chebyshev.py
+-rw-r--r--   0        0        0     4034 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/experimental/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py
+-rw-r--r--   0        0        0     1254 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/linear_warmup.py
+-rw-r--r--   0        0        0     1400 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/proportion.py
+-rw-r--r--   0        0        0     1770 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/rex.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/__init__.py
+-rw-r--r--   0        0        0     4464 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/a2grad.py
+-rw-r--r--   0        0        0     6702 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adabelief.py
+-rw-r--r--   0        0        0     5470 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adabound.py
+-rw-r--r--   0        0        0     3573 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adadelta.py
+-rw-r--r--   0        0        0     8784 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adafactor.py
+-rw-r--r--   0        0        0     5662 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adahessian.py
+-rw-r--r--   0        0        0     6115 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adai.py
+-rw-r--r--   0        0        0     6271 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adalite.py
+-rw-r--r--   0        0        0     4976 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adamax.py
+-rw-r--r--   0        0        0     4664 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adamod.py
+-rw-r--r--   0        0        0     6494 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adamp.py
+-rw-r--r--   0        0        0     6417 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adams.py
+-rw-r--r--   0        0        0     6267 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adan.py
+-rw-r--r--   0        0        0     5253 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adanorm.py
+-rw-r--r--   0        0        0     6014 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adapnm.py
+-rw-r--r--   0        0        0     4169 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adashift.py
+-rw-r--r--   0        0        0     4136 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adasmooth.py
+-rw-r--r--   0        0        0      784 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/agc.py
+-rw-r--r--   0        0        0     3172 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/aggmo.py
+-rw-r--r--   0        0        0     7527 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/aida.py
+-rw-r--r--   0        0        0     3618 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/alig.py
+-rw-r--r--   0        0        0     5003 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/amos.py
+-rw-r--r--   0        0        0     5367 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/apollo.py
+-rw-r--r--   0        0        0     4803 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/avagrad.py
+-rw-r--r--   0        0        0     8294 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/came.py
+-rw-r--r--   0        0        0    29447 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/dadapt.py
+-rw-r--r--   0        0        0     6749 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/diffgrad.py
+-rw-r--r--   0        0        0    10769 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/fp16.py
+-rw-r--r--   0        0        0     2764 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/fromage.py
+-rw-r--r--   0        0        0    10127 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/galore.py
+-rw-r--r--   0        0        0      396 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/gc.py
+-rw-r--r--   0        0        0     2517 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/gravity.py
+-rw-r--r--   0        0        0     8316 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lamb.py
+-rw-r--r--   0        0        0     3608 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lars.py
+-rw-r--r--   0        0        0     4099 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lion.py
+-rw-r--r--   0        0        0     7198 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lomo.py
+-rw-r--r--   0        0        0     4564 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lookahead.py
+-rw-r--r--   0        0        0     6466 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/madgrad.py
+-rw-r--r--   0        0        0     3172 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/msvag.py
+-rw-r--r--   0        0        0     3595 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/nero.py
+-rw-r--r--   0        0        0     4520 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/novograd.py
+-rw-r--r--   0        0        0     4045 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/padam.py
+-rw-r--r--   0        0        0     4242 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/pcgrad.py
+-rw-r--r--   0        0        0     4233 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/pid.py
+-rw-r--r--   0        0        0     3741 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/pnm.py
+-rw-r--r--   0        0        0     6564 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/prodigy.py
+-rw-r--r--   0        0        0     4827 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/qhadam.py
+-rw-r--r--   0        0        0     3249 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/qhm.py
+-rw-r--r--   0        0        0     5622 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/radam.py
+-rw-r--r--   0        0        0     6808 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/ranger.py
+-rw-r--r--   0        0        0    12817 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/ranger21.py
+-rw-r--r--   0        0        0    15522 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/rotograd.py
+-rw-r--r--   0        0        0    21575 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sam.py
+-rw-r--r--   0        0        0    10883 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/schedulefree.py
+-rw-r--r--   0        0        0    12933 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sgd.py
+-rw-r--r--   0        0        0     4276 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sgdp.py
+-rw-r--r--   0        0        0    16137 2024-05-21 09:03:09.209609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/shampoo.py
+-rw-r--r--   0        0        0    20625 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/shampoo_utils.py
+-rw-r--r--   0        0        0     5081 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sm3.py
+-rw-r--r--   0        0        0     5309 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sophia.py
+-rw-r--r--   0        0        0     2864 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/srmm.py
+-rw-r--r--   0        0        0     7226 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/swats.py
+-rw-r--r--   0        0        0     2942 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/tiger.py
+-rw-r--r--   0        0        0     9837 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/utils.py
+-rw-r--r--   0        0        0     5306 2024-05-21 09:03:09.213609 pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/yogi.py
+-rw-r--r--   0        0        0    51434 1970-01-01 00:00:00.000000 pytorch_optimizer-3.0.0/PKG-INFO
```

### Comparing `pytorch_optimizer-2.9.1/LICENSE` & `pytorch_optimizer-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/README.rst` & `pytorch_optimizer-3.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,386 +1,373 @@
-=================
-pytorch-optimizer
-=================
-
-+--------------+------------------------------------------+
-| Build        | |workflow| |Documentation Status|        |
-+--------------+------------------------------------------+
-| Quality      | |codecov| |black| |ruff|                 |
-+--------------+------------------------------------------+
-| Package      | |PyPI version| |PyPI pyversions|         |
-+--------------+------------------------------------------+
-| Status       | |PyPi download| |PyPi month download|    |
-+--------------+------------------------------------------+
-| License      | |apache|                                 |
-+--------------+------------------------------------------+
-
-| **pytorch-optimizer** is optimizer & lr scheduler collections in PyTorch.
-| I just re-implemented (speed & memory tweaks, plug-ins) the algorithm while based on the original paper. Also, It includes useful and practical optimization ideas.
-| Currently, 50 optimizers, 6 lr schedulers are supported!
-|
-| Highly inspired by `pytorch-optimizer <https://github.com/jettify/pytorch-optimizer>`__.
+Metadata-Version: 2.1
+Name: pytorch_optimizer
+Version: 3.0.0
+Summary: optimizer & lr scheduler & objective function collections in PyTorch
+Home-page: https://github.com/kozistr/pytorch_optimizer
+License: Apache-2.0
+Keywords: pytorch,deep-learning,optimizer,lr scheduler,A2Grad,ASGD,AccSGD,AdaBelief,AdaBound,AdaDelta,AdaFactor,AdaMax,AdaMod,AdaNorm,AdaPNM,AdaSmooth,AdaHessian,Adai,Adalite,AdamP,AdamS,Adan,AggMo,Aida,AliG,Amos,Apollo,AvaGrad,bSAM,CAME,DAdaptAdaGrad,DAdaptAdam,DAdaptAdan,DAdaptSGD,DAdaptLion,DiffGrad,Fromage,GaLore,Gravity,GSAM,LARS,Lamb,Lion,LOMO,Lookahead,MADGRAD,MSVAG,Nero,NovoGrad,PAdam,PCGrad,PID,PNM,Prodigy,QHAdam,QHM,RAdam,Ranger,Ranger21,RotoGrad,SAM,ScheduleFreeSGD,ScheduleFreeAdamW,SGDP,Shampoo,ScalableShampoo,SGDW,SignSGD,SM3,SopihaH,SRMM,SWATS,Tiger,WSAM,Yogi,BCE,BCEFocal,Focal,FocalCosine,SoftF1,Dice,LDAM,Jaccard,Bi-Tempered,Tversky,FocalTversky,LovaszHinge,bitsandbytes
+Author: kozistr
+Author-email: kozistr@gmail.com
+Maintainer: kozistr
+Maintainer-email: kozistr@gmail.com
+Requires-Python: >=3.8,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: bitsandbytes
+Requires-Dist: bitsandbytes (>=0.43,<0.44) ; extra == "bitsandbytes"
+Requires-Dist: numpy ; python_version >= "3.8"
+Requires-Dist: torch (>=1.10) ; python_version >= "3.8"
+Project-URL: Documentation, https://pytorch-optimizers.readthedocs.io/en/latest
+Project-URL: Repository, https://github.com/kozistr/pytorch_optimizer
+Description-Content-Type: text/markdown
+
+# pytorch-optimizer
+
+|         |                                                                                                                                                                                                                                                                                                                                                                                                       |
+|---------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Build   | ![workflow](https://github.com/kozistr/pytorch_optimizer/actions/workflows/ci.yml/badge.svg?branch=main) [![Documentation Status](https://readthedocs.org/projects/pytorch-optimizers/badge/?version=latest)](https://pytorch-optimizers.readthedocs.io/en/latest/?badge=latest)                                                                                                                      |
+| Quality | [![codecov](https://codecov.io/gh/kozistr/pytorch_optimizer/branch/main/graph/badge.svg?token=L4K00EA0VD)](https://codecov.io/gh/kozistr/pytorch_optimizer) ![black](https://img.shields.io/badge/code%20style-black-000000.svg) [![ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff) |
+| Package | [![PyPI version](https://badge.fury.io/py/pytorch-optimizer.svg)](https://badge.fury.io/py/pytorch-optimizer) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytorch-optimizer.svg)](https://pypi.python.org/pypi/pytorch-optimizer/)                                                                                                                                                     |
+| Status  | [![PyPi download](https://static.pepy.tech/badge/pytorch-optimizer)](https://pepy.tech/project/pytorch-optimizer) [![PyPi month download](https://static.pepy.tech/badge/pytorch-optimizer/month)](https://pepy.tech/project/pytorch-optimizer)                                                                                                                                                       |
+| License | [![apache](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)                                                                                                                                                                                                                                                                                     |
+
+**pytorch-optimizer** is optimizer & lr scheduler collections in PyTorch. 
+I just re-implemented (speed & memory tweaks, plug-ins) the algorithm while based on the original paper. Also, It includes useful and practical optimization ideas.  
+Currently, **67 optimizers (+ `bitsandbytes`)**, **11 lr schedulers**, and **13 loss functions** are supported!  
 
-Getting Started
----------------
+Highly inspired by [pytorch-optimizer](https://github.com/jettify/pytorch-optimizer).
 
-For more, see the `documentation <https://pytorch-optimizers.readthedocs.io/en/latest/>`__.
+## Getting Started
 
-Most optimizers are under MIT or Apache 2.0 license, but a few optimizers like `Fromage` have BY-NC-SA 4.0 license, which is non-commercial.
+For more, see the [documentation](https://pytorch-optimizers.readthedocs.io/en/latest/).
+
+Most optimizers are under MIT or Apache 2.0 license, but a few optimizers like `Fromage`, `Nero` have `CC BY-NC-SA 4.0 license`, which is non-commercial. 
 So, please double-check the license before using it at your work.
 
-Installation
-~~~~~~~~~~~~
+### Installation
 
-::
+```bash
+$ pip3 install pytorch-optimizer
+```
 
-    $ pip3 install -U pytorch-optimizer
+From `v2.12.0`, you can install and import `bitsandbytes` optimizers. 
+please check [the requirements](https://github.com/TimDettmers/bitsandbytes?tab=readme-ov-file#tldr) before installing it.
 
-If there's a version issue when installing the package, try with `--no-deps` option.
+From `v3.0.0`, drop `Python 3.7` support. However, you can still use this package with `Python 3.7` by installing with `--ignore-requires-python` option.
 
-::
+```bash
+$ pip install "pytorch-optimizer[bitsandbytes]"
+```
 
-    $ pip3 install -U --no-deps pytorch-optimizer
+### Simple Usage
 
-Simple Usage
-~~~~~~~~~~~~
+```python
+from pytorch_optimizer import AdamP
 
-::
+model = YourModel()
+optimizer = AdamP(model.parameters())
 
-    from pytorch_optimizer import AdamP
+# or you can use optimizer loader, simply passing a name of the optimizer.
 
-    model = YourModel()
-    optimizer = AdamP(model.parameters())
+from pytorch_optimizer import load_optimizer
 
-    # or you can use optimizer loader, simply passing a name of the optimizer.
+optimizer = load_optimizer(optimizer='adamp')(model.parameters())
 
-    from pytorch_optimizer import load_optimizer
+# if you install `bitsandbytes` optimizer, you can use `8-bit` optimizers from `pytorch-optimizer`.
 
-    model = YourModel()
-    opt = load_optimizer(optimizer='adamp')
-    optimizer = opt(model.parameters())
+from pytorch_optimizer import load_optimizer
 
-Also, you can load the optimizer via `torch.hub`
+opt = load_optimizer(optimizer='bnb_adamw8bit')
+optimizer = opt(model.parameters())
+```
 
-::
+Also, you can load the optimizer via `torch.hub`.
 
-    import torch
+```python
+import torch
 
-    model = YourModel()
-    opt = torch.hub.load('kozistr/pytorch_optimizer', 'adamp')
-    optimizer = opt(model.parameters())
+model = YourModel()
+opt = torch.hub.load('kozistr/pytorch_optimizer', 'adamp')
+optimizer = opt(model.parameters())
+```
 
 If you want to build the optimizer with parameters & configs, there's `create_optimizer()` API.
 
-::
-
-    from pytorch_optimizer import create_optimizer
+```python
+from pytorch_optimizer import create_optimizer
 
-    optimizer = create_optimizer(
-        model,
-        'adamp',
-        lr=1e-3,
-        weight_decay=1e-3,
-        use_gc=True,
-        use_lookahead=True,
-    )
-
-Supported Optimizers
---------------------
-
-You can check the supported optimizers & lr schedulers.
-
-::
-
-    from pytorch_optimizer import get_supported_optimizers, get_supported_lr_schedulers
-
-    supported_optimizers = get_supported_optimizers()
-    supported_lr_schedulers = get_supported_lr_schedulers()
-
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Optimizer    | Description                                                                                       | Official Code                                                                     | Paper                                                                                         |                                                              Citation                                                |
-+==============+===================================================================================================+===================================================================================+===============================================================================================+======================================================================================================================+
-| AdaBelief    | *Adapting Step-sizes by the Belief in Observed Gradients*                                         | `github <https://github.com/juntang-zhuang/Adabelief-Optimizer>`__                | `https://arxiv.org/abs/2010.07468 <https://arxiv.org/abs/2010.07468>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201007468Z/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaBound     | *Adaptive Gradient Methods with Dynamic Bound of Learning Rate*                                   | `github <https://github.com/Luolc/AdaBound/blob/master/adabound/adabound.py>`__   | `https://openreview.net/forum?id=Bkg3g2R9FX <https://openreview.net/forum?id=Bkg3g2R9FX>`__   | `cite <https://github.com/Luolc/AdaBound#citing>`__                                                                  |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaHessian   | *An Adaptive Second Order Optimizer for Machine Learning*                                         | `github <https://github.com/amirgholami/adahessian>`__                            | `https://arxiv.org/abs/2006.00719 <https://arxiv.org/abs/2006.00719>`__                       | `cite <https://github.com/amirgholami/adahessian#citation>`__                                                        |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdamD        | *Improved bias-correction in Adam*                                                                |                                                                                   | `https://arxiv.org/abs/2110.10828 <https://arxiv.org/abs/2110.10828>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv211010828S/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdamP        | *Slowing Down the Slowdown for Momentum Optimizers on Scale-invariant Weights*                    | `github <https://github.com/clovaai/AdamP>`__                                     | `https://arxiv.org/abs/2006.08217 <https://arxiv.org/abs/2006.08217>`__                       | `cite <https://github.com/clovaai/AdamP#how-to-cite>`__                                                              |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| diffGrad     | *An Optimization Method for Convolutional Neural Networks*                                        | `github <https://github.com/shivram1987/diffGrad>`__                              | `https://arxiv.org/abs/1909.11015v3 <https://arxiv.org/abs/1909.11015v3>`__                   | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190911015D/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| MADGRAD      | *A Momentumized, Adaptive, Dual Averaged Gradient Method for Stochastic*                          | `github <https://github.com/facebookresearch/madgrad>`__                          | `https://arxiv.org/abs/2101.11075 <https://arxiv.org/abs/2101.11075>`__                       | `cite <https://github.com/facebookresearch/madgrad#tech-report>`__                                                   |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| RAdam        | *On the Variance of the Adaptive Learning Rate and Beyond*                                        | `github <https://github.com/LiyuanLucasLiu/RAdam>`__                              | `https://arxiv.org/abs/1908.03265 <https://arxiv.org/abs/1908.03265>`__                       | `cite <https://github.com/LiyuanLucasLiu/RAdam#citation>`__                                                          |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Ranger       | *a synergistic optimizer combining RAdam and LookAhead, and now GC in one optimizer*              | `github <https://github.com/lessw2020/Ranger-Deep-Learning-Optimizer>`__          | `https://bit.ly/3zyspC3 <https://bit.ly/3zyspC3>`__                                           | `cite <https://github.com/lessw2020/Ranger-Deep-Learning-Optimizer#citing-this-work>`__                              |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Ranger21     | *a synergistic deep learning optimizer*                                                           | `github <https://github.com/lessw2020/Ranger21>`__                                | `https://arxiv.org/abs/2106.13731 <https://arxiv.org/abs/2106.13731>`__                       | `cite <https://github.com/lessw2020/Ranger21#referencing-this-work>`__                                               |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Lamb         | *Large Batch Optimization for Deep Learning*                                                      | `github <https://github.com/cybertronai/pytorch-lamb>`__                          | `https://arxiv.org/abs/1904.00962 <https://arxiv.org/abs/1904.00962>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190400962Y/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Shampoo      | *Preconditioned Stochastic Tensor Optimization*                                                   | `github <https://github.com/moskomule/shampoo.pytorch>`__                         | `https://arxiv.org/abs/1802.09568 <https://arxiv.org/abs/1802.09568>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv180209568G/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Nero         | *Learning by Turning: Neural Architecture Aware Optimisation*                                     | `github <https://github.com/jxbz/nero>`__                                         | `https://arxiv.org/abs/2102.07227 <https://arxiv.org/abs/2102.07227>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210207227L/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Adan         | *Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models*                          | `github <https://github.com/sail-sg/Adan>`__                                      | `https://arxiv.org/abs/2208.06677 <https://arxiv.org/abs/2208.06677>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2022arXiv220806677X/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Adai         | *Disentangling the Effects of Adaptive Learning Rate and Momentum*                                | `github <https://github.com/zeke-xie/adaptive-inertia-adai>`__                    | `https://arxiv.org/abs/2006.15815 <https://arxiv.org/abs/2006.15815>`__                       | `cite <https://github.com/zeke-xie/adaptive-inertia-adai#citing>`__                                                  |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SAM          | *Sharpness-Aware Minimization*                                                                    | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2010.01412 <https://arxiv.org/abs/2010.01412>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201001412F/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| ASAM         | *Adaptive Sharpness-Aware Minimization*                                                           | `github <https://github.com/davda54/sam>`__                                       | `https://arxiv.org/abs/2102.11600 <https://arxiv.org/abs/2102.11600>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210211600K/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| GSAM         | *Surrogate Gap Guided Sharpness-Aware Minimization*                                               | `github <https://github.com/juntang-zhuang/GSAM>`__                               | `https://openreview.net/pdf?id=edONMAnhLu- <https://openreview.net/pdf?id=edONMAnhLu->`__     | `cite <https://github.com/juntang-zhuang/GSAM#citation>`__                                                           |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| D-Adaptation | *Learning-Rate-Free Learning by D-Adaptation*                                                     | `github <https://github.com/facebookresearch/dadaptation>`__                      | `https://arxiv.org/abs/2301.07733 <https://arxiv.org/abs/2301.07733>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2023arXiv230107733D/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaFactor    | *Adaptive Learning Rates with Sublinear Memory Cost*                                              | `github <https://github.com/DeadAt0m/adafactor-pytorch>`__                        | `https://arxiv.org/abs/1804.04235 <https://arxiv.org/abs/1804.04235>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv180404235S/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Apollo       | *An Adaptive Parameter-wise Diagonal Quasi-Newton Method for Nonconvex Stochastic Optimization*   | `github <https://github.com/XuezheMax/apollo>`__                                  | `https://arxiv.org/abs/2009.13586 <https://arxiv.org/abs/2009.13586>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv200913586M/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| NovoGrad     | *Stochastic Gradient Methods with Layer-wise Adaptive Moments for Training of Deep Networks*      | `github <https://github.com/lonePatient/NovoGrad-pytorch>`__                      | `https://arxiv.org/abs/1905.11286 <https://arxiv.org/abs/1905.11286>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190511286G/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Lion         | *Symbolic Discovery of Optimization Algorithms*                                                   | `github <https://github.com/google/automl/tree/master/lion>`__                    | `https://arxiv.org/abs/2302.06675 <https://arxiv.org/abs/2302.06675>`__                       | `cite <https://github.com/google/automl/tree/master/lion#citation>`__                                                |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Ali-G        | *Adaptive Learning Rates for Interpolation with Gradients*                                        | `github <https://github.com/oval-group/ali-g>`__                                  | `https://arxiv.org/abs/1906.05661 <https://arxiv.org/abs/1906.05661>`__                       | `cite <https://github.com/oval-group/ali-g#adaptive-learning-rates-for-interpolation-with-gradients>`__              |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SM3          | *Memory-Efficient Adaptive Optimization*                                                          | `github <https://github.com/google-research/google-research/tree/master/sm3>`__   | `https://arxiv.org/abs/1901.11150 <https://arxiv.org/abs/1901.11150>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaNorm      | *Adaptive Gradient Norm Correction based Optimizer for CNNs*                                      | `github <https://github.com/shivram1987/AdaNorm>`__                               | `https://arxiv.org/abs/2210.06364 <https://arxiv.org/abs/2210.06364>`__                       | `cite <https://github.com/shivram1987/AdaNorm/tree/main#citation>`__                                                 |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| RotoGrad     | *Gradient Homogenization in Multitask Learning*                                                   | `github <https://github.com/adrianjav/rotograd>`__                                | `https://openreview.net/pdf?id=T8wHz4rnuGL <https://openreview.net/pdf?id=T8wHz4rnuGL>`__     | `cite <https://github.com/adrianjav/rotograd#citing>`__                                                              |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| A2Grad       | *Optimal Adaptive and Accelerated Stochastic Gradient Descent*                                    | `github <https://github.com/severilov/A2Grad_optimizer>`__                        | `https://arxiv.org/abs/1810.00553 <https://arxiv.org/abs/1810.00553>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv181000553D/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AccSGD       | *Accelerating Stochastic Gradient Descent For Least Squares Regression*                           | `github <https://github.com/rahulkidambi/AccSGD>`__                               | `https://arxiv.org/abs/1704.08227 <https://arxiv.org/abs/1704.08227>`__                       | `cite <https://github.com/rahulkidambi/AccSGD#citation>`__                                                           |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SGDW         | *Decoupled Weight Decay Regularization*                                                           | `github <https://github.com/loshchil/AdamW-and-SGDW>`__                           | `https://arxiv.org/abs/1711.05101 <https://arxiv.org/abs/1711.05101>`__                       | `cite <https://github.com/loshchil/AdamW-and-SGDW#contact>`__                                                        |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| ASGD         | *Adaptive Gradient Descent without Descent*                                                       | `github <https://github.com/ymalitsky/adaptive_GD>`__                             | `https://arxiv.org/abs/1910.09529 <https://arxiv.org/abs/1910.09529>`__                       | `cite <https://github.com/ymalitsky/adaptive_GD#reference>`__                                                        |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Yogi         | *Adaptive Methods for Nonconvex Optimization*                                                     |                                                                                   | `NIPS 2018 <https://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization>`__ | `cite <https://proceedings.neurips.cc/paper_files/paper/2018/hash/90365351ccc7437a1309dc64e4db32a3-Abstract.html>`__ |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SWATS        | *Improving Generalization Performance by Switching from Adam to SGD*                              |                                                                                   | `https://arxiv.org/abs/1712.07628 <https://arxiv.org/abs/1712.07628>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2017arXiv171207628S/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Fromage      | *On the distance between two neural networks and the stability of learning*                       | `github <https://github.com/jxbz/fromage>`__                                      | `https://arxiv.org/abs/2002.03432 <https://arxiv.org/abs/2002.03432>`__                       | `cite <https://github.com/jxbz/fromage#citation>`__                                                                  |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| MSVAG        | *Dissecting Adam: The Sign, Magnitude and Variance of Stochastic Gradients*                       | `github <https://github.com/lballes/msvag>`__                                     | `https://arxiv.org/abs/1705.07774 <https://arxiv.org/abs/1705.07774>`__                       | `cite <https://github.com/lballes/msvag#citation>`__                                                                 |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaMod       | *An Adaptive and Momental Bound Method for Stochastic Learning*                                   | `github <https://github.com/lancopku/AdaMod>`__                                   | `https://arxiv.org/abs/1910.12249 <https://arxiv.org/abs/1910.12249>`__                       | `cite <https://github.com/lancopku/AdaMod#citation>`__                                                               |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AggMo        | *Aggregated Momentum: Stability Through Passive Damping*                                          | `github <https://github.com/AtheMathmo/AggMo>`__                                  | `https://arxiv.org/abs/1804.00325 <https://arxiv.org/abs/1804.00325>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv180400325L/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| QHAdam       | *Quasi-hyperbolic momentum and Adam for deep learning*                                            | `github <https://github.com/facebookresearch/qhoptim>`__                          | `https://arxiv.org/abs/1810.06801 <https://arxiv.org/abs/1810.06801>`__                       | `cite <https://github.com/facebookresearch/qhoptim#reference>`__                                                     |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| PID          | *A PID Controller Approach for Stochastic Optimization of Deep Networks*                          | `github <https://github.com/tensorboy/PIDOptimizer>`__                            | `CVPR 18 <http://www4.comp.polyu.edu.hk/~cslzhang/paper/CVPR18_PID.pdf>`__                    | `cite <https://github.com/tensorboy/PIDOptimizer#citation>`__                                                        |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Gravity      | *a Kinematic Approach on Optimization in Deep Learning*                                           | `github <https://github.com/dariush-bahrami/gravity.optimizer>`__                 | `https://arxiv.org/abs/2101.09192 <https://arxiv.org/abs/2101.09192>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210109192B/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaSmooth    | *An Adaptive Learning Rate Method based on Effective Ratio*                                       |                                                                                   | `https://arxiv.org/abs/2204.00825v1 <https://arxiv.org/abs/2204.00825v1>`__                   | `cite <https://ui.adsabs.harvard.edu/abs/2022arXiv220400825L/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| SRMM         | *Stochastic regularized majorization-minimization with weakly convex and multi-convex surrogates* | `github <https://github.com/HanbaekLyu/SRMM>`__                                   | `https://arxiv.org/abs/2201.01652 <https://arxiv.org/abs/2201.01652>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2022arXiv220101652L/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AvaGrad      | *Domain-independent Dominance of Adaptive Methods*                                                | `github <https://github.com/lolemacs/avagrad>`__                                  | `https://arxiv.org/abs/1912.01823 <https://arxiv.org/abs/1912.01823>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv191201823S/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| PCGrad       | *Gradient Surgery for Multi-Task Learning*                                                        | `github <https://github.com/tianheyu927/PCGrad>`__                                | `https://arxiv.org/abs/2001.06782 <https://arxiv.org/abs/2001.06782>`__                       | `cite <https://github.com/tianheyu927/PCGrad#reference>`__                                                           |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AMSGrad      | *On the Convergence of Adam and Beyond*                                                           |                                                                                   | `https://openreview.net/pdf?id=ryQu7f-RZ <https://openreview.net/pdf?id=ryQu7f-RZ>`__         | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190409237R/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Lookahead    | *k steps forward, 1 step back*                                                                    | `github <https://github.com/pytorch/examples/tree/main/imagenet>`__               | `https://arxiv.org/abs/1907.08610 <https://arxiv.org/abs/1907.08610>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190708610Z/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| PNM          | *Manipulating Stochastic Gradient Noise to Improve Generalization*                                | `github <https://github.com/zeke-xie/Positive-Negative-Momentum>`__               | `https://arxiv.org/abs/2103.17182 <https://arxiv.org/abs/2103.17182>`__                       | `cite <https://github.com/zeke-xie/Positive-Negative-Momentum#citing>`__                                             |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| GC           | *Gradient Centralization*                                                                         | `github <https://github.com/Yonghongwei/Gradient-Centralization>`__               | `https://arxiv.org/abs/2004.01461 <https://arxiv.org/abs/2004.01461>`__                       | `cite <https://github.com/Yonghongwei/Gradient-Centralization#citation>`__                                           |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AGC          | *Adaptive Gradient Clipping*                                                                      | `github <https://github.com/deepmind/deepmind-research/tree/master/nfnets>`__     | `https://arxiv.org/abs/2102.06171 <https://arxiv.org/abs/2102.06171>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210206171B/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Stable WD    | *Understanding and Scheduling Weight Decay*                                                       | `github <https://github.com/zeke-xie/stable-weight-decay-regularization>`__       | `https://arxiv.org/abs/2011.11152 <https://arxiv.org/abs/2011.11152>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv201111152X/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Softplus T   | *Calibrating the Adaptive Learning Rate to Improve Convergence of ADAM*                           |                                                                                   | `https://arxiv.org/abs/1908.00700 <https://arxiv.org/abs/1908.00700>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv190800700T/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| EE LRS       | *Wide-minima Density Hypothesis and the Explore-Exploit Learning Rate Schedule*                   |                                                                                   | `https://arxiv.org/abs/2003.03977 <https://arxiv.org/abs/2003.03977>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2020arXiv200303977I/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Norm Loss    | *An efficient yet effective regularization method for deep neural networks*                       |                                                                                   | `https://arxiv.org/abs/2103.06583 <https://arxiv.org/abs/2103.06583>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210306583G/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Chebyshev LR | *Acceleration via Fractal Learning Rate Schedules*                                                |                                                                                   | `https://arxiv.org/abs/2103.01338 <https://arxiv.org/abs/2103.01338>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2021arXiv210301338A/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| Un-tuned WU  | *On the adequacy of untuned warmup for adaptive optimization*                                     |                                                                                   | `https://arxiv.org/abs/1910.04209 <https://arxiv.org/abs/1910.04209>`__                       | `cite <https://ui.adsabs.harvard.edu/abs/2019arXiv191004209M/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaShift     | *Decorrelation and Convergence of Adaptive Learning Rate Methods*                                 | `github <https://github.com/MichaelKonobeev/adashift>`__                          | `https://arxiv.org/abs/1810.00143v4 <https://arxiv.org/abs/1810.00143v4>`__                   | `cite <https://ui.adsabs.harvard.edu/abs/2018arXiv181000143Z/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-| AdaDelta     | *An Adaptive Learning Rate Method*                                                                |                                                                                   | `https://arxiv.org/abs/1212.5701v1 <https://arxiv.org/abs/1212.5701v1>`__                     | `cite <https://ui.adsabs.harvard.edu/abs/2012arXiv1212.5701Z/exportcitation>`__                                      |
-+--------------+---------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------+
-
-Useful Resources
-----------------
-
-Several optimization ideas to regularize & stabilize the training. Most
-of the ideas are applied in ``Ranger21`` optimizer.
-
-Also, most of the captures are taken from ``Ranger21`` paper.
-
-+------------------------------------------+---------------------------------------------+--------------------------------------------+
-| `Adaptive Gradient Clipping`_            | `Gradient Centralization`_                  | `Softplus Transformation`_                 |
-+------------------------------------------+---------------------------------------------+--------------------------------------------+
-| `Gradient Normalization`_                | `Norm Loss`_                                | `Positive-Negative Momentum`_              |
-+------------------------------------------+---------------------------------------------+--------------------------------------------+
-| `Linear learning rate warmup`_           | `Stable weight decay`_                      | `Explore-exploit learning rate schedule`_  |
-+------------------------------------------+---------------------------------------------+--------------------------------------------+
-| `Lookahead`_                             | `Chebyshev learning rate schedule`_         | `(Adaptive) Sharpness-Aware Minimization`_ |
-+------------------------------------------+---------------------------------------------+--------------------------------------------+
-| `On the Convergence of Adam and Beyond`_ | `Improved bias-correction in Adam`_         | `Adaptive Gradient Norm Correction`_       |
-+------------------------------------------+---------------------------------------------+--------------------------------------------+
-
-Adaptive Gradient Clipping
---------------------------
-
-| This idea originally proposed in ``NFNet (Normalized-Free Network)`` paper.
-| ``AGC (Adaptive Gradient Clipping)`` clips gradients based on the ``unit-wise ratio of gradient norms to parameter norms``.
-
--  code : `github <https://github.com/deepmind/deepmind-research/tree/master/nfnets>`__
--  paper : `arXiv <https://arxiv.org/abs/2102.06171>`__
-
-Gradient Centralization
------------------------
-
-+-----------------------------------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/gradient_centralization.png  |
-+-----------------------------------------------------------------------------------------------------------------+
+optimizer = create_optimizer(
+    model,
+    'adamp',
+    lr=1e-3,
+    weight_decay=1e-3,
+    use_gc=True,
+    use_lookahead=True,
+)
+```
+
+## Supported Optimizers
+
+You can check the supported optimizers with below code.
+
+```python
+from pytorch_optimizer import get_supported_optimizers
+
+supported_optimizers = get_supported_optimizers()
+```
+
+| Optimizer     | Description                                                                                       | Official Code                                                                                                  | Paper                                                                                      | Citation                                                                                                          |
+|---------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
+| AdaBelief     | *Adapting Step-sizes by the Belief in Observed Gradients*                                         | [github](https://github.com/juntang-zhuang/Adabelief-Optimizer)                                                | <https://arxiv.org/abs/2010.07468>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2020arXiv201007468Z/exportcitation)                                      |
+| AdaBound      | *Adaptive Gradient Methods with Dynamic Bound of Learning Rate*                                   | [github](https://github.com/Luolc/AdaBound/blob/master/adabound/adabound.py)                                   | <https://openreview.net/forum?id=Bkg3g2R9FX>                                               | [cite](https://github.com/Luolc/AdaBound#citing)                                                                  |
+| AdaHessian    | *An Adaptive Second Order Optimizer for Machine Learning*                                         | [github](https://github.com/amirgholami/adahessian)                                                            | <https://arxiv.org/abs/2006.00719>                                                         | [cite](https://github.com/amirgholami/adahessian#citation)                                                        |
+| AdamD         | *Improved bias-correction in Adam*                                                                |                                                                                                                | <https://arxiv.org/abs/2110.10828>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv211010828S/exportcitation)                                      |
+| AdamP         | *Slowing Down the Slowdown for Momentum Optimizers on Scale-invariant Weights*                    | [github](https://github.com/clovaai/AdamP)                                                                     | <https://arxiv.org/abs/2006.08217>                                                         | [cite](https://github.com/clovaai/AdamP#how-to-cite)                                                              |
+| diffGrad      | *An Optimization Method for Convolutional Neural Networks*                                        | [github](https://github.com/shivram1987/diffGrad)                                                              | <https://arxiv.org/abs/1909.11015v3>                                                       | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190911015D/exportcitation)                                      |
+| MADGRAD       | *A Momentumized, Adaptive, Dual Averaged Gradient Method for Stochastic*                          | [github](https://github.com/facebookresearch/madgrad)                                                          | <https://arxiv.org/abs/2101.11075>                                                         | [cite](https://github.com/facebookresearch/madgrad#tech-report)                                                   |
+| RAdam         | *On the Variance of the Adaptive Learning Rate and Beyond*                                        | [github](https://github.com/LiyuanLucasLiu/RAdam)                                                              | <https://arxiv.org/abs/1908.03265>                                                         | [cite](https://github.com/LiyuanLucasLiu/RAdam#citation)                                                          |
+| Ranger        | *a synergistic optimizer combining RAdam and LookAhead, and now GC in one optimizer*              | [github](https://github.com/lessw2020/Ranger-Deep-Learning-Optimizer)                                          | <https://bit.ly/3zyspC3>                                                                   | [cite](https://github.com/lessw2020/Ranger-Deep-Learning-Optimizer#citing-this-work)                              |
+| Ranger21      | *a synergistic deep learning optimizer*                                                           | [github](https://github.com/lessw2020/Ranger21)                                                                | <https://arxiv.org/abs/2106.13731>                                                         | [cite](https://github.com/lessw2020/Ranger21#referencing-this-work)                                               |
+| Lamb          | *Large Batch Optimization for Deep Learning*                                                      | [github](https://github.com/cybertronai/pytorch-lamb)                                                          | <https://arxiv.org/abs/1904.00962>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190400962Y/exportcitation)                                      |
+| Shampoo       | *Preconditioned Stochastic Tensor Optimization*                                                   | [github](https://github.com/moskomule/shampoo.pytorch)                                                         | <https://arxiv.org/abs/1802.09568>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2018arXiv180209568G/exportcitation)                                      |
+| Nero          | *Learning by Turning: Neural Architecture Aware Optimisation*                                     | [github](https://github.com/jxbz/nero)                                                                         | <https://arxiv.org/abs/2102.07227>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210207227L/exportcitation)                                      |
+| Adan          | *Adaptive Nesterov Momentum Algorithm for Faster Optimizing Deep Models*                          | [github](https://github.com/sail-sg/Adan)                                                                      | <https://arxiv.org/abs/2208.06677>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2022arXiv220806677X/exportcitation)                                      |
+| Adai          | *Disentangling the Effects of Adaptive Learning Rate and Momentum*                                | [github](https://github.com/zeke-xie/adaptive-inertia-adai)                                                    | <https://arxiv.org/abs/2006.15815>                                                         | [cite](https://github.com/zeke-xie/adaptive-inertia-adai#citing)                                                  |
+| SAM           | *Sharpness-Aware Minimization*                                                                    | [github](https://github.com/davda54/sam)                                                                       | <https://arxiv.org/abs/2010.01412>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2020arXiv201001412F/exportcitation)                                      |
+| ASAM          | *Adaptive Sharpness-Aware Minimization*                                                           | [github](https://github.com/davda54/sam)                                                                       | <https://arxiv.org/abs/2102.11600>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210211600K/exportcitation)                                      |
+| GSAM          | *Surrogate Gap Guided Sharpness-Aware Minimization*                                               | [github](https://github.com/juntang-zhuang/GSAM)                                                               | <https://openreview.net/pdf?id=edONMAnhLu->                                                | [cite](https://github.com/juntang-zhuang/GSAM#citation)                                                           |
+| D-Adaptation  | *Learning-Rate-Free Learning by D-Adaptation*                                                     | [github](https://github.com/facebookresearch/dadaptation)                                                      | <https://arxiv.org/abs/2301.07733>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2023arXiv230107733D/exportcitation)                                      |
+| AdaFactor     | *Adaptive Learning Rates with Sublinear Memory Cost*                                              | [github](https://github.com/DeadAt0m/adafactor-pytorch)                                                        | <https://arxiv.org/abs/1804.04235>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2018arXiv180404235S/exportcitation)                                      |
+| Apollo        | *An Adaptive Parameter-wise Diagonal Quasi-Newton Method for Nonconvex Stochastic Optimization*   | [github](https://github.com/XuezheMax/apollo)                                                                  | <https://arxiv.org/abs/2009.13586>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2020arXiv200913586M/exportcitation)                                      |
+| NovoGrad      | *Stochastic Gradient Methods with Layer-wise Adaptive Moments for Training of Deep Networks*      | [github](https://github.com/lonePatient/NovoGrad-pytorch)                                                      | <https://arxiv.org/abs/1905.11286>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190511286G/exportcitation)                                      |
+| Lion          | *Symbolic Discovery of Optimization Algorithms*                                                   | [github](https://github.com/google/automl/tree/master/lion)                                                    | <https://arxiv.org/abs/2302.06675>                                                         | [cite](https://github.com/google/automl/tree/master/lion#citation)                                                |
+| Ali-G         | *Adaptive Learning Rates for Interpolation with Gradients*                                        | [github](https://github.com/oval-group/ali-g)                                                                  | <https://arxiv.org/abs/1906.05661>                                                         | [cite](https://github.com/oval-group/ali-g#adaptive-learning-rates-for-interpolation-with-gradients)              |
+| SM3           | *Memory-Efficient Adaptive Optimization*                                                          | [github](https://github.com/google-research/google-research/tree/master/sm3)                                   | <https://arxiv.org/abs/1901.11150>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190111150A/exportcitation)                                      |
+| AdaNorm       | *Adaptive Gradient Norm Correction based Optimizer for CNNs*                                      | [github](https://github.com/shivram1987/AdaNorm)                                                               | <https://arxiv.org/abs/2210.06364>                                                         | [cite](https://github.com/shivram1987/AdaNorm/tree/main#citation)                                                 |
+| RotoGrad      | *Gradient Homogenization in Multitask Learning*                                                   | [github](https://github.com/adrianjav/rotograd)                                                                | <https://openreview.net/pdf?id=T8wHz4rnuGL>                                                | [cite](https://github.com/adrianjav/rotograd#citing)                                                              |
+| A2Grad        | *Optimal Adaptive and Accelerated Stochastic Gradient Descent*                                    | [github](https://github.com/severilov/A2Grad_optimizer)                                                        | <https://arxiv.org/abs/1810.00553>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2018arXiv181000553D/exportcitation)                                      |
+| AccSGD        | *Accelerating Stochastic Gradient Descent For Least Squares Regression*                           | [github](https://github.com/rahulkidambi/AccSGD)                                                               | <https://arxiv.org/abs/1704.08227>                                                         | [cite](https://github.com/rahulkidambi/AccSGD#citation)                                                           |
+| SGDW          | *Decoupled Weight Decay Regularization*                                                           | [github](https://github.com/loshchil/AdamW-and-SGDW)                                                           | <https://arxiv.org/abs/1711.05101>                                                         | [cite](https://github.com/loshchil/AdamW-and-SGDW#contact)                                                        |
+| ASGD          | *Adaptive Gradient Descent without Descent*                                                       | [github](https://github.com/ymalitsky/adaptive_GD)                                                             | <https://arxiv.org/abs/1910.09529>                                                         | [cite](https://github.com/ymalitsky/adaptive_GD#reference)                                                        |
+| Yogi          | *Adaptive Methods for Nonconvex Optimization*                                                     |                                                                                                                | [NIPS 2018](https://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization) | [cite](https://proceedings.neurips.cc/paper_files/paper/2018/hash/90365351ccc7437a1309dc64e4db32a3-Abstract.html) |
+| SWATS         | *Improving Generalization Performance by Switching from Adam to SGD*                              |                                                                                                                | <https://arxiv.org/abs/1712.07628>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2017arXiv171207628S/exportcitation)                                      |
+| Fromage       | *On the distance between two neural networks and the stability of learning*                       | [github](https://github.com/jxbz/fromage)                                                                      | <https://arxiv.org/abs/2002.03432>                                                         | [cite](https://github.com/jxbz/fromage#citation)                                                                  |
+| MSVAG         | *Dissecting Adam: The Sign, Magnitude and Variance of Stochastic Gradients*                       | [github](https://github.com/lballes/msvag)                                                                     | <https://arxiv.org/abs/1705.07774>                                                         | [cite](https://github.com/lballes/msvag#citation)                                                                 |
+| AdaMod        | *An Adaptive and Momental Bound Method for Stochastic Learning*                                   | [github](https://github.com/lancopku/AdaMod)                                                                   | <https://arxiv.org/abs/1910.12249>                                                         | [cite](https://github.com/lancopku/AdaMod#citation)                                                               |
+| AggMo         | *Aggregated Momentum: Stability Through Passive Damping*                                          | [github](https://github.com/AtheMathmo/AggMo)                                                                  | <https://arxiv.org/abs/1804.00325>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2018arXiv180400325L/exportcitation)                                      |
+| QHAdam        | *Quasi-hyperbolic momentum and Adam for deep learning*                                            | [github](https://github.com/facebookresearch/qhoptim)                                                          | <https://arxiv.org/abs/1810.06801>                                                         | [cite](https://github.com/facebookresearch/qhoptim#reference)                                                     |
+| PID           | *A PID Controller Approach for Stochastic Optimization of Deep Networks*                          | [github](https://github.com/tensorboy/PIDOptimizer)                                                            | [CVPR 18](http://www4.comp.polyu.edu.hk/~cslzhang/paper/CVPR18_PID.pdf)                    | [cite](https://github.com/tensorboy/PIDOptimizer#citation)                                                        |
+| Gravity       | *a Kinematic Approach on Optimization in Deep Learning*                                           | [github](https://github.com/dariush-bahrami/gravity.optimizer)                                                 | <https://arxiv.org/abs/2101.09192>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210109192B/exportcitation)                                      |
+| AdaSmooth     | *An Adaptive Learning Rate Method based on Effective Ratio*                                       |                                                                                                                | <https://arxiv.org/abs/2204.00825v1>                                                       | [cite](https://ui.adsabs.harvard.edu/abs/2022arXiv220400825L/exportcitation)                                      |
+| SRMM          | *Stochastic regularized majorization-minimization with weakly convex and multi-convex surrogates* | [github](https://github.com/HanbaekLyu/SRMM)                                                                   | <https://arxiv.org/abs/2201.01652>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2022arXiv220101652L/exportcitation)                                      |
+| AvaGrad       | *Domain-independent Dominance of Adaptive Methods*                                                | [github](https://github.com/lolemacs/avagrad)                                                                  | <https://arxiv.org/abs/1912.01823>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv191201823S/exportcitation)                                      |
+| PCGrad        | *Gradient Surgery for Multi-Task Learning*                                                        | [github](https://github.com/tianheyu927/PCGrad)                                                                | <https://arxiv.org/abs/2001.06782>                                                         | [cite](https://github.com/tianheyu927/PCGrad#reference)                                                           |
+| AMSGrad       | *On the Convergence of Adam and Beyond*                                                           |                                                                                                                | <https://openreview.net/pdf?id=ryQu7f-RZ>                                                  | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190409237R/exportcitation)                                      |
+| Lookahead     | *k steps forward, 1 step back*                                                                    | [github](https://github.com/pytorch/examples/tree/main/imagenet)                                               | <https://arxiv.org/abs/1907.08610>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190708610Z/exportcitation)                                      |
+| PNM           | *Manipulating Stochastic Gradient Noise to Improve Generalization*                                | [github](https://github.com/zeke-xie/Positive-Negative-Momentum)                                               | <https://arxiv.org/abs/2103.17182>                                                         | [cite](https://github.com/zeke-xie/Positive-Negative-Momentum#citing)                                             |
+| GC            | *Gradient Centralization*                                                                         | [github](https://github.com/Yonghongwei/Gradient-Centralization)                                               | <https://arxiv.org/abs/2004.01461>                                                         | [cite](https://github.com/Yonghongwei/Gradient-Centralization#citation)                                           |
+| AGC           | *Adaptive Gradient Clipping*                                                                      | [github](https://github.com/deepmind/deepmind-research/tree/master/nfnets)                                     | <https://arxiv.org/abs/2102.06171>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210206171B/exportcitation)                                      |
+| Stable WD     | *Understanding and Scheduling Weight Decay*                                                       | [github](https://github.com/zeke-xie/stable-weight-decay-regularization)                                       | <https://arxiv.org/abs/2011.11152>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2020arXiv201111152X/exportcitation)                                      |
+| Softplus T    | *Calibrating the Adaptive Learning Rate to Improve Convergence of ADAM*                           |                                                                                                                | <https://arxiv.org/abs/1908.00700>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190800700T/exportcitation)                                      |
+| Un-tuned w/u  | *On the adequacy of untuned warmup for adaptive optimization*                                     |                                                                                                                | <https://arxiv.org/abs/1910.04209>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv191004209M/exportcitation)                                      |
+| Norm Loss     | *An efficient yet effective regularization method for deep neural networks*                       |                                                                                                                | <https://arxiv.org/abs/2103.06583>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210306583G/exportcitation)                                      |
+| AdaShift      | *Decorrelation and Convergence of Adaptive Learning Rate Methods*                                 | [github](https://github.com/MichaelKonobeev/adashift)                                                          | <https://arxiv.org/abs/1810.00143v4>                                                       | [cite](https://ui.adsabs.harvard.edu/abs/2018arXiv181000143Z/exportcitation)                                      |
+| AdaDelta      | *An Adaptive Learning Rate Method*                                                                |                                                                                                                | <https://arxiv.org/abs/1212.5701v1>                                                        | [cite](https://ui.adsabs.harvard.edu/abs/2012arXiv1212.5701Z/exportcitation)                                      |
+| Amos          | *An Adam-style Optimizer with Adaptive Weight Decay towards Model-Oriented Scale*                 | [github](https://github.com/google-research/jestimator)                                                        | <https://arxiv.org/abs/2210.11693>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2022arXiv221011693T/exportcitation)                                      |
+| SignSGD       | *Compressed Optimisation for Non-Convex Problems*                                                 | [github](https://github.com/jxbz/signSGD)                                                                      | <https://arxiv.org/abs/1802.04434>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2018arXiv180204434B/exportcitation)                                      |
+| Sophia        | *A Scalable Stochastic Second-order Optimizer for Language Model Pre-training*                    | [github](https://github.com/Liuhong99/Sophia)                                                                  | <https://arxiv.org/abs/2305.14342>                                                         | [cite](https://github.com/Liuhong99/Sophia)                                                                       |
+| Prodigy       | *An Expeditiously Adaptive Parameter-Free Learner*                                                | [github](https://github.com/konstmish/prodigy)                                                                 | <https://arxiv.org/abs/2306.06101>                                                         | [cite](https://github.com/konstmish/prodigy#how-to-cite)                                                          |
+| PAdam         | *Closing the Generalization Gap of Adaptive Gradient Methods in Training Deep Neural Networks*    | [github](https://github.com/uclaml/Padam)                                                                      | <https://arxiv.org/abs/1806.06763>                                                         | [cite](https://github.com/uclaml/Padam#citation)                                                                  |
+| LOMO          | *Full Parameter Fine-tuning for Large Language Models with Limited Resources*                     | [github](https://github.com/OpenLMLab/LOMO)                                                                    | <https://arxiv.org/abs/2306.09782>                                                         | [cite](https://github.com/OpenLMLab/LOMO#citation)                                                                |
+| Tiger         | *A Tight-fisted Optimizer, an optimizer that is extremely budget-conscious*                       | [github](https://github.com/bojone/tiger)                                                                      |                                                                                            | [cite](https://github.com/bojone/tiger/blob/main/README_en.md#citation)                                           |
+| CAME          | *Confidence-guided Adaptive Memory Efficient Optimization*                                        | [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/CAME)                            | <https://aclanthology.org/2023.acl-long.243/>                                              | [cite](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/CAME#citation)                        |
+| WSAM          | *Sharpness-Aware Minimization Revisited: Weighted Sharpness as a Regularization Term*             | [github](https://github.com/intelligent-machine-learning/dlrover/blob/master/atorch/atorch/optimizers/wsam.py) | <https://arxiv.org/abs/2305.15817>                                                         | [cite](https://github.com/intelligent-machine-learning/dlrover)                                                   |
+| Aida          | *A DNN Optimizer that Improves over AdaBelief by Suppression of the Adaptive Stepsize Range*      | [github](https://github.com/guoqiang-zhang-x/Aida-Optimizer)                                                   | <https://arxiv.org/abs/2203.13273>                                                         | [cite](https://github.com/guoqiang-zhang-x/Aida-Optimizer?tab=readme-ov-file#1-brief-description-of-aida)         |
+| GaLore        | *Memory-Efficient LLM Training by Gradient Low-Rank Projection*                                   | [github](https://github.com/jiaweizzhao/GaLore)                                                                | <https://arxiv.org/abs/2403.03507>                                                         | [cite](https://github.com/jiaweizzhao/GaLore/tree/master?tab=readme-ov-file#citation)                             |
+| Adalite       | *Adalite optimizer*                                                                               | [github](https://github.com/VatsaDev/adalite)                                                                  | <https://github.com/VatsaDev/adalite>                                                      | [cite](https://github.com/VatsaDev/adalite)                                                                       |
+| bSAM          | *SAM as an Optimal Relaxation of Bayes*                                                           | [github](https://github.com/team-approx-bayes/bayesian-sam)                                                    | <https://arxiv.org/abs/2210.01620>                                                         | [cite](https://ui.adsabs.harvard.edu/abs/2022arXiv221001620M/exportcitation)                                      |
+| Schedule-Free | *Schedule-Free Optimizers*                                                                        | [github](https://github.com/facebookresearch/schedule_free)                                                    | <https://github.com/facebookresearch/schedule_free>                                        | [cite](https://github.com/facebookresearch/schedule_free)                                                         |
+
+## Supported LR Scheduler
+
+You can check the supported learning rate schedulers with below code.
+
+```python
+from pytorch_optimizer import get_supported_lr_schedulers
+
+supported_lr_schedulers = get_supported_lr_schedulers()
+```
+
+| LR Scheduler    | Description                                                                     | Official Code                                                                                                                       | Paper                              | Citation                                                                     |
+|-----------------|---------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------|------------------------------------|------------------------------------------------------------------------------|
+| Explore-Exploit | *Wide-minima Density Hypothesis and the Explore-Exploit Learning Rate Schedule* |                                                                                                                                     | <https://arxiv.org/abs/2003.03977> | [cite](https://ui.adsabs.harvard.edu/abs/2020arXiv200303977I/exportcitation) |
+| Chebyshev       | *Acceleration via Fractal Learning Rate Schedules*                              |                                                                                                                                     | <https://arxiv.org/abs/2103.01338> | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210301338A/exportcitation) |
+| REX             | *Revisiting Budgeted Training with an Improved Schedule*                        | [github](https://github.com/Nerogar/OneTrainer/blob/2c6f34ea0838e5a86774a1cf75093d7e97c70f03/modules/util/lr_scheduler_util.py#L66) | <https://arxiv.org/abs/2107.04197> | [cite](https://ui.adsabs.harvard.edu/abs/2021arXiv210704197C/exportcitation) |
+
+## Supported Loss Function
+
+You can check the supported loss functions with below code.
+
+```python
+from pytorch_optimizer import get_supported_loss_functions
+
+supported_loss_functions = get_supported_loss_functions()
+```
+
+| Loss Functions  | Description                                                                                                             | Official Code                                          | Paper                              | Citation                                                                     |
+|-----------------|-------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|------------------------------------|------------------------------------------------------------------------------|
+| Label Smoothing | *Rethinking the Inception Architecture for Computer Vision*                                                             |                                                        | <https://arxiv.org/abs/1512.00567> | [cite](https://ui.adsabs.harvard.edu/abs/2015arXiv151200567S/exportcitation) |
+| Focal           | *Focal Loss for Dense Object Detection*                                                                                 |                                                        | <https://arxiv.org/abs/1708.02002> | [cite](https://ui.adsabs.harvard.edu/abs/2017arXiv170802002L/exportcitation) |
+| Focal Cosine    | *Data-Efficient Deep Learning Method for Image Classification Using Data Augmentation, Focal Cosine Loss, and Ensemble* |                                                        | <https://arxiv.org/abs/2007.07805> | [cite](https://ui.adsabs.harvard.edu/abs/2020arXiv200707805K/exportcitation) |
+| LDAM            | *Learning Imbalanced Datasets with Label-Distribution-Aware Margin Loss*                                                | [github](https://github.com/kaidic/LDAM-DRW)           | <https://arxiv.org/abs/1906.07413> | [cite](https://github.com/kaidic/LDAM-DRW#reference)                         |
+| Jaccard (IOU)   | *IoU Loss for 2D/3D Object Detection*                                                                                   |                                                        | <https://arxiv.org/abs/1908.03851> | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190803851Z/exportcitation) |
+| Bi-Tempered     | *The Principle of Unchanged Optimality in Reinforcement Learning Generalization*                                        |                                                        | <https://arxiv.org/abs/1906.03361> | [cite](https://ui.adsabs.harvard.edu/abs/2019arXiv190600336I/exportcitation) |
+| Tversky         | *Tversky loss function for image segmentation using 3D fully convolutional deep networks*                               |                                                        | <https://arxiv.org/abs/1706.05721> | [cite](https://ui.adsabs.harvard.edu/abs/2017arXiv170605721S/exportcitation) |
+| Lovasz Hinge    | *A tractable surrogate for the optimization of the intersection-over-union measure in neural networks*                  | [github](https://github.com/bermanmaxim/LovaszSoftmax) | <https://arxiv.org/abs/1705.08790> | [cite](https://github.com/bermanmaxim/LovaszSoftmax#citation)                |
+
+## Useful Resources
+
+Several optimization ideas to regularize & stabilize the training. Most of the ideas are applied in `Ranger21` optimizer.
+
+Also, most of the captures are taken from `Ranger21` paper.
+
+|                                                                                 |                                                                       |                                                                                   |
+|---------------------------------------------------------------------------------|-----------------------------------------------------------------------|-----------------------------------------------------------------------------------|
+| [Adaptive Gradient Clipping](#adaptive-gradient-clipping)                       | [Gradient Centralization](#gradient-centralization)                   | [Softplus Transformation](#softplus-transformation)                               |
+| [Gradient Normalization](#gradient-normalization)                               | [Norm Loss](#norm-loss)                                               | [Positive-Negative Momentum](#positive-negative-momentum)                         |
+| [Linear learning rate warmup](#linear-learning-rate-warmup)                     | [Stable weight decay](#stable-weight-decay)                           | [Explore-exploit learning rate schedule](#explore-exploit-learning-rate-schedule) |
+| [Lookahead](#lookahead)                                                         | [Chebyshev learning rate schedule](#chebyshev-learning-rate-schedule) | [(Adaptive) Sharpness-Aware Minimization](#adaptive-sharpness-aware-minimization) |
+| [On the Convergence of Adam and Beyond](#on-the-convergence-of-adam-and-beyond) | [Improved bias-correction in Adam](#improved-bias-correction-in-adam) | [Adaptive Gradient Norm Correction](#adaptive-gradient-norm-correction)           |
+
+### Adaptive Gradient Clipping
+
+This idea originally proposed in `NFNet (Normalized-Free Network)` paper. `AGC (Adaptive Gradient Clipping)` clips gradients based on the `unit-wise ratio of gradient norms to parameter norms`.
+
+* code : [github](https://github.com/deepmind/deepmind-research/tree/master/nfnets)
+* paper : [arXiv](https://arxiv.org/abs/2102.06171)
+
+### Gradient Centralization
+
+|                                                                                                               |
+|---------------------------------------------------------------------------------------------------------------|
+| ![image](https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/gradient_centralization.png) |
 
-``Gradient Centralization (GC)`` operates directly on gradients by centralizing the gradient to have zero mean.
+`Gradient Centralization (GC)` operates directly on gradients by centralizing the gradient to have zero mean.
 
--  code : `github <https://github.com/Yonghongwei/Gradient-Centralization>`__
--  paper : `arXiv <https://arxiv.org/abs/2004.01461>`__
+* code : [github](https://github.com/Yonghongwei/Gradient-Centralization)
+* paper : [arXiv](https://arxiv.org/abs/2004.01461)
 
-Softplus Transformation
------------------------
+### Softplus Transformation
 
 By running the final variance denom through the softplus function, it lifts extremely tiny values to keep them viable.
 
--  paper : `arXiv <https://arxiv.org/abs/1908.00700>`__
+* paper : [arXiv](https://arxiv.org/abs/1908.00700)
 
-Gradient Normalization
-----------------------
+### Gradient Normalization
 
-Norm Loss
----------
+### Norm Loss
 
-+---------------------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/norm_loss.png  |
-+---------------------------------------------------------------------------------------------------+
+|                                                                                                 |
+|-------------------------------------------------------------------------------------------------|
+| ![image](https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/norm_loss.png) |
 
--  paper : `arXiv <https://arxiv.org/abs/2103.06583>`__
+* paper : [arXiv](https://arxiv.org/abs/2103.06583)
 
-Positive-Negative Momentum
---------------------------
+### Positive-Negative Momentum
 
-+--------------------------------------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/positive_negative_momentum.png  |
-+--------------------------------------------------------------------------------------------------------------------+
+|                                                                                                                  |
+|------------------------------------------------------------------------------------------------------------------|
+| ![image](https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/positive_negative_momentum.png) |
 
--  code : `github <https://github.com/zeke-xie/Positive-Negative-Momentum>`__
--  paper : `arXiv <https://arxiv.org/abs/2103.17182>`__
+* code : [github](https://github.com/zeke-xie/Positive-Negative-Momentum)
+* paper : [arXiv](https://arxiv.org/abs/2103.17182)
 
-Linear learning rate warmup
----------------------------
+### Linear learning rate warmup
 
-+----------------------------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/linear_lr_warmup.png  |
-+----------------------------------------------------------------------------------------------------------+
+|                                                                                                        |
+|--------------------------------------------------------------------------------------------------------|
+| ![image](https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/linear_lr_warmup.png) |
 
--  paper : `arXiv <https://arxiv.org/abs/1910.04209>`__
+* paper : [arXiv](https://arxiv.org/abs/1910.04209)
 
-Stable weight decay
--------------------
+### Stable weight decay
 
-+-------------------------------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/stable_weight_decay.png  |
-+-------------------------------------------------------------------------------------------------------------+
+|                                                                                                           |
+|-----------------------------------------------------------------------------------------------------------|
+| ![image](https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/stable_weight_decay.png) |
 
--  code : `github <https://github.com/zeke-xie/stable-weight-decay-regularization>`__
--  paper : `arXiv <https://arxiv.org/abs/2011.11152>`__
+* code : [github](https://github.com/zeke-xie/stable-weight-decay-regularization)
+* paper : [arXiv](https://arxiv.org/abs/2011.11152)
 
-Explore-exploit learning rate schedule
---------------------------------------
+### Explore-exploit learning rate schedule
 
-+---------------------------------------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/explore_exploit_lr_schedule.png  |
-+---------------------------------------------------------------------------------------------------------------------+
+|                                                                                                                   |
+|-------------------------------------------------------------------------------------------------------------------|
+| ![image](https://raw.githubusercontent.com/kozistr/pytorch_optimizer/main/assets/explore_exploit_lr_schedule.png) |
 
--  code : `github <https://github.com/nikhil-iyer-97/wide-minima-density-hypothesis>`__
--  paper : `arXiv <https://arxiv.org/abs/2003.03977>`__
+* code : [github](https://github.com/nikhil-iyer-97/wide-minima-density-hypothesis)
+* paper : [arXiv](https://arxiv.org/abs/2003.03977)
 
-Lookahead
----------
+### Lookahead
 
-| ``k`` steps forward, 1 step back. ``Lookahead`` consisting of keeping an exponential moving average of the weights that is
-| updated and substituted to the current weights every ``k_{lookahead}`` steps (5 by default).
+`k` steps forward, 1 step back. `Lookahead` consisting of keeping an exponential moving average of the weights that is updated and substituted to the current weights every `k` lookahead steps (5 by default).
 
-Chebyshev learning rate schedule
---------------------------------
+### Chebyshev learning rate schedule
 
 Acceleration via Fractal Learning Rate Schedules.
 
-(Adaptive) Sharpness-Aware Minimization
----------------------------------------
+### (Adaptive) Sharpness-Aware Minimization
+
+Sharpness-Aware Minimization (SAM) simultaneously minimizes loss value and loss sharpness.  
+In particular, it seeks parameters that lie in neighborhoods having uniformly low loss.
 
-| Sharpness-Aware Minimization (SAM) simultaneously minimizes loss value and loss sharpness.
-| In particular, it seeks parameters that lie in neighborhoods having uniformly low loss.
+### On the Convergence of Adam and Beyond
 
-On the Convergence of Adam and Beyond
--------------------------------------
+Convergence issues can be fixed by endowing such algorithms with 'long-term memory' of past gradients.
 
-| Convergence issues can be fixed by endowing such algorithms with 'long-term memory' of past gradients.
+### Improved bias-correction in Adam
 
-Improved bias-correction in Adam
---------------------------------
+With the default bias-correction, Adam may actually make larger than requested gradient updates early in training.
 
-| With the default bias-correction, Adam may actually make larger than requested gradient updates early in training.
+### Adaptive Gradient Norm Correction
 
-Adaptive Gradient Norm Correction
----------------------------------
+Correcting the norm of a gradient in each iteration based on the adaptive training history of gradient norm.
 
-| Correcting the norm of gradient in each iteration based on the adaptive training history of gradient norm.
+## Frequently asked questions
 
-Citation
---------
+[here](./qa.md)
 
-Please cite original authors of optimization algorithms. If you use this software, please cite it as below.
-Or you can get from "cite this repository" button.
+## Citation
 
-::
+Please cite the original authors of optimization algorithms. You can easily find it in the above table! 
+If you use this software, please cite it below. Or you can get it from "cite this repository" button.
 
-    @software{Kim_pytorch_optimizer_Optimizer_and_2022,
+    @software{Kim_pytorch_optimizer_optimizer_2021,
         author = {Kim, Hyeongchan},
-        month = {1},
-        title = {{pytorch_optimizer: optimizer and lr scheduler collections in PyTorch}},
-        version = {1.0.0},
-        year = {2022}
+        month = jan,
+        title = {{pytorch_optimizer: optimizer & lr scheduler & loss function collections in PyTorch}},
+        url = {https://github.com/kozistr/pytorch_optimizer},
+        version = {2.12.0},
+        year = {2021}
     }
 
-Author
-------
+## Maintainer
 
-Hyeongchan Kim / `@kozistr <http://kozistr.tech/about>`__
+Hyeongchan Kim / [@kozistr](http://kozistr.tech/about)
 
-.. |workflow| image:: https://github.com/kozistr/pytorch_optimizer/actions/workflows/ci.yml/badge.svg?branch=main
-.. |Documentation Status| image:: https://readthedocs.org/projects/pytorch-optimizers/badge/?version=latest
-   :target: https://pytorch-optimizers.readthedocs.io/en/latest/?badge=latest
-.. |PyPI version| image:: https://badge.fury.io/py/pytorch-optimizer.svg
-   :target: https://badge.fury.io/py/pytorch-optimizer
-.. |PyPi download| image:: https://pepy.tech/badge/pytorch-optimizer
-   :target: https://pepy.tech/project/pytorch-optimizer
-.. |PyPi month download| image:: https://pepy.tech/badge/pytorch-optimizer/month
-   :target: https://pepy.tech/project/pytorch-optimizer
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/pytorch-optimizer.svg
-   :target: https://pypi.python.org/pypi/pytorch-optimizer/
-.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-.. |ruff| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
-   :target: https://github.com/charliermarsh/ruff
-.. |codecov| image:: https://codecov.io/gh/kozistr/pytorch_optimizer/branch/main/graph/badge.svg?token=L4K00EA0VD
-   :target: https://codecov.io/gh/kozistr/pytorch_optimizer
-.. |apache| image:: https://img.shields.io/badge/License-Apache_2.0-blue.svg
-   :target: https://opensource.org/licenses/Apache-2.0
```

### Comparing `pytorch_optimizer-2.9.1/pyproject.toml` & `pytorch_optimizer-3.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,129 @@
 [tool.poetry]
 name = "pytorch_optimizer"
-version = "2.9.1"
-description = "optimizer & lr scheduler collections in PyTorch"
+version = "3.0.0"
+description = "optimizer & lr scheduler & objective function collections in PyTorch"
 license = "Apache-2.0"
 authors = ["kozistr <kozistr@gmail.com>"]
 maintainers = ["kozistr <kozistr@gmail.com>"]
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/kozistr/pytorch_optimizer"
 repository = "https://github.com/kozistr/pytorch_optimizer"
 documentation = "https://pytorch-optimizers.readthedocs.io/en/latest"
-keywords = ["pytorch", "deep-learning", "optimizer", "lr scheduler", "A2Grad", "ASGD", "AccSGD", "AdaBelief", "AdaBound", "AdaDelta", "AdaFactor", "AdaMax", "AdaMod", "AdaNorm", "AdaPNM", "AdaSmooth", "Adai", "AdamP", "AdamS", "Adan", "AggMo", "AliG", "Apollo", "AvaGrad", "DAdaptAdaGrad", "DAdaptAdam", "DAdaptAdan", "DAdaptSGD", "DiffGrad", "Fromage", "Gravity", "LARS", "Lamb", "Lion", "MADGRAD", "MSVAG", "Nero", "NovoGrad", "PID", "PNM", "QHAdam", "QHM", "RAdam", "Ranger", "Ranger21", "SGDP", "SGDW", "SM3", "SRMM", "SWATS", "ScalableShampoo", "Shampoo", "Yogi", "SAM", "GSAM", "PCGrad", "RotoGrad"]
+keywords = [
+    "pytorch", "deep-learning", "optimizer", "lr scheduler", "A2Grad", "ASGD", "AccSGD", "AdaBelief", "AdaBound",
+    "AdaDelta", "AdaFactor", "AdaMax", "AdaMod", "AdaNorm", "AdaPNM", "AdaSmooth", "AdaHessian", "Adai", "Adalite",
+    "AdamP", "AdamS", "Adan", "AggMo", "Aida", "AliG", "Amos", "Apollo", "AvaGrad", "bSAM", "CAME", "DAdaptAdaGrad",
+    "DAdaptAdam", "DAdaptAdan", "DAdaptSGD", "DAdaptLion", "DiffGrad", "Fromage", "GaLore", "Gravity", "GSAM", "LARS",
+    "Lamb", "Lion", "LOMO", "Lookahead", "MADGRAD", "MSVAG", "Nero", "NovoGrad", "PAdam", "PCGrad", "PID", "PNM",
+    "Prodigy", "QHAdam", "QHM", "RAdam", "Ranger", "Ranger21", "RotoGrad", "SAM", "ScheduleFreeSGD",
+    "ScheduleFreeAdamW", "SGDP", "Shampoo", "ScalableShampoo", "SGDW", "SignSGD", "SM3", "SopihaH", "SRMM", "SWATS",
+    "Tiger", "WSAM", "Yogi", "BCE", "BCEFocal", "Focal", "FocalCosine", "SoftF1", "Dice", "LDAM", "Jaccard",
+    "Bi-Tempered", "Tversky", "FocalTversky", "LovaszHinge", "bitsandbytes",
+]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Education",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
-numpy = [
-    { version = "=1.21.1", python = ">=3.7,<3.8" },
-    { version = "*", python = ">=3.8" },
-]
-torch = [
-    { version = ">=1.10", python = ">=3.8", source = "torch" },
-    { version = "^1.10", python = ">=3.7,<3.8", source = "torch" },
-]
+python = ">=3.8,<4.0.0"
+numpy = { version = "*", python = ">=3.8" }
+torch = { version = ">=1.10", python = ">=3.8", source = "torch" }
+bitsandbytes = { version = "^0.43", optional = true }
 
 [tool.poetry.dev-dependencies]
-isort = [
-    { version = "==5.11.5", python = ">=3.7,<3.8"},
-    { version = "^5.12.0", python = ">=3.8"}
-]
-black = "^23.3.0"
-ruff = "^0.0.264"
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+isort = { version = "^5", python = ">=3.8" }
+black = { version = "^24", python = ">=3.8" }
+ruff = "*"
+pytest = "*"
+pytest-cov = "*"
+
+[tool.poetry.extras]
+bitsandbytes = ["bitsandbytes"]
 
 [[tool.poetry.source]]
 name = "torch"
 url = "https://download.pytorch.org/whl/cpu"
-secondary = true
+priority = "explicit"
 
 [tool.ruff]
-select = ["A", "B", "C4", "D", "E", "F", "G", "I", "N", "S", "T", "ISC", "ICN", "W", "INP", "PIE", "T20", "RET", "SIM", "TID", "ARG", "ERA", "RUF", "YTT", "PL"]
-ignore = ["D100", "D102", "D104", "D105", "D107", "D203", "D213", "PIE790", "PLR0912", "PLR0913", "PLR0915", "PLR2004"]
-fixable = ["A", "B", "C", "D", "E", "F"]
-unfixable = ["F401"]
+lint.select = [
+    "A", "B", "C4", "D", "E", "F", "G", "I", "N", "S", "T", "ISC", "ICN", "W", "INP", "PIE", "T20", "RET", "SIM",
+    "TID", "ARG", "ERA", "RUF", "YTT", "PL", "Q"
+]
+lint.ignore = [
+    "B905", "D100", "D102", "D104", "D105", "D107", "D203", "D213", "D413", "PIE790", "PLR0912", "PLR0913", "PLR0915",
+    "PLR2004", "RUF013", "Q003",
+]
+lint.fixable = ["ALL"]
+lint.unfixable = ["F401"]
 exclude = [
-    ".eggs",
     ".git",
-    ".mypy_cache",
-    ".ruff_cache",
     ".github",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "build",
+    ".idea",
+    ".ipynb_checkpoints",
+    ".pytest_cache",
+    ".ruff_cache",
+    "assets",
     "dist",
-    "node_modules",
-    "venv",
     "docs",
-    "assets",
+    ".venv",
+    "__pypackages__",
 ]
 line-length = 119
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-target-version = "py39"
+lint.dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+target-version = "py311"
+lint.flake8-quotes.docstring-quotes = "double"
+lint.flake8-quotes.inline-quotes = "single"
+lint.pylint.max-args = 7
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.format]
+quote-style = "single"
+
+[tool.ruff.lint.per-file-ignores]
+"./pytorch_optimizer/__init__.py" = ["F401"]
+"./pytorch_optimizer/lr_scheduler/__init__.py" = ["F401"]
 "./hubconf.py" = ["D", "INP001"]
 "./tests/__init__.py" = ["D"]
 "./tests/constants.py" = ["D"]
 "./tests/utils.py" = ["D"]
 "./tests/test_base.py" = ["D", "S101"]
-"./tests/test_utils.py" = ["D", "S101"]
+"./tests/test_utils.py" = ["D", "S101", "ERA001"]
 "./tests/test_gradients.py" = ["D", "S101"]
 "./tests/test_optimizers.py" = ["D", "S101"]
 "./tests/test_optimizer_parameters.py" = ["D", "S101"]
 "./tests/test_general_optimizer_parameters.py" = ["D", "S101"]
-"./tests/test_load_optimizers.py" = ["D", "S101"]
-"./tests/test_load_lr_schedulers.py" = ["D", "S101"]
-"./tests/test_lr_schedulers.py" = ["D"]
+"./tests/test_lr_schedulers.py" = ["D", "S101"]
 "./tests/test_lr_scheduler_parameters.py" = ["D", "S101"]
 "./tests/test_create_optimizer.py" = ["D"]
-"./pytorch_optimizer/__init__.py" = ["F401"]
-"./pytorch_optimizer/lr_scheduler/__init__.py" = ["F401"]
+"./tests/test_loss_functions.py" = ["D", "S101"]
+"./tests/test_load_modules.py" = ["D", "S101"]
+
+[tool.pytest.ini_options]
+testpaths = "tests"
 
 [tool.coverage.run]
 omit = [
-    "./pytorch_optimizer/optimizer/gsam.py",
-    "./pytorch_optimizer/optimizer/fp16.py",
     "./pytorch_optimizer/optimizer/rotograd.py",
-    "./pytorch_optimizer/optimizer/swats.py",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/base/exception.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/base/exception.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/base/scheduler.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/base/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,22 +72,21 @@
         elif self.step_t == self.warmup_steps:
             value = self.max_lr
         else:
             value = self._step()
 
         self.step_t += 1
 
-        # apply the lr to optimizer if it's provided
         if self.optimizer is not None:
             for param_group in self.optimizer.param_groups:
                 param_group['lr'] = value
 
         self.last_lr = [value]
 
         return value
 
     @abstractmethod
-    def _step(self) -> float:
+    def _step(self) -> float:  # pragma: no cover
         raise NotImplementedError
 
     def get_lr(self) -> float:
         return self.last_lr[0]
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/cosine_anealing.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/cosine_anealing.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/experimental/deberta_v3_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/linear_warmup.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/linear_warmup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         phase: float = (self.step_t - self.warmup_steps) / (self.total_steps - self.warmup_steps) * math.pi
         return self.min_lr + (self.max_lr - self.min_lr) * (np.cos(phase) + 1.0) / 2.0
 
 
 class PolyScheduler(BaseLinearWarmupScheduler):
     r"""Poly LR Scheduler.
 
-    :param: poly_order: float. lr scheduler decreases with steps.
+    :param poly_order: float. lr scheduler decreases with steps.
     """
 
     def __init__(self, poly_order: float = 0.5, **kwargs):
         self.poly_order = poly_order
 
         if poly_order <= 0:
             raise ValueError(f'[-] poly_order must be positive. {poly_order}')
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/lr_scheduler/proportion.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/lr_scheduler/proportion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/a2grad.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/a2grad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabelief.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adabelief.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
         betas: BETAS = (0.9, 0.999),
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
         fixed_decay: bool = False,
-        rectify: bool = True,
+        rectify: bool = False,
         n_sma_threshold: int = 5,
         degenerated_to_sgd: bool = True,
         ams_bound: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
         eps: float = 1e-16,
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adabound.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adabound.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adadelta.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adadelta.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adafactor.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adafactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def get_options(shape: Tuple[int, ...]) -> bool:
         r"""Get `factored`."""
         return len(shape) >= 2
 
     @staticmethod
     def get_rms(x: torch.Tensor) -> float:
         r"""Get RMS."""
-        return x.norm(2) / (x.numel() ** 0.5)
+        return x.norm(2) / math.sqrt(x.numel())
 
     @staticmethod
     def approximate_sq_grad(
         exp_avg_sq_row: torch.Tensor,
         exp_avg_sq_col: torch.Tensor,
         output: torch.Tensor,
     ):
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adai.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adai.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamax.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adamax.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamod.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adamod.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adamp.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adamp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adams.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adams.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adan.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adan.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adanorm.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adanorm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adapnm.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adapnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adashift.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adashift.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/adasmooth.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/adasmooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     state['prev_param'] = torch.zeros_like(p)
                     state['s'] = torch.zeros_like(p)
                     state['n'] = torch.zeros_like(p)
                     state['exp_avg_sq'] = torch.zeros_like(p)
 
                 self.apply_weight_decay(
                     p=p,
-                    grad=p.grad,
+                    grad=grad,
                     lr=group['lr'],
                     weight_decay=group['weight_decay'],
                     weight_decouple=group['weight_decouple'],
                     fixed_decay=group['fixed_decay'],
                 )
 
                 prev_param = state['prev_param']
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/agc.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/agc.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/aggmo.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/aggmo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/alig.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/alig.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/apollo.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/apollo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/avagrad.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/avagrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/dadapt.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/dadapt.py`

 * *Files 8% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         betas: BETAS = (0.9, 0.999),
         d0: float = 1e-6,
         growth_rate: float = float('inf'),
         weight_decay: float = 0.0,
         weight_decouple: bool = False,
         fixed_decay: bool = False,
         bias_correction: bool = False,
-        eps: float = 0.0,
+        eps: float = 1e-8,
     ):
         self.validate_learning_rate(lr)
         self.validate_betas(betas)
         self.validate_non_negative(weight_decay, 'weight_decay')
         self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
@@ -695,7 +695,136 @@
 
                 if not group['weight_decouple']:
                     p.div_(1.0 + d_lr * group['weight_decay'])
 
             group['k'] += 1
 
         return loss
+
+
+class DAdaptLion(Optimizer, BaseOptimizer):
+    r"""Lion with D-Adaptation. Leave LR set to 1 unless you encounter instability. This implementation is based on V3.
+
+    :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
+    :param lr: float. learning rate.
+    :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
+    :param d0: float. initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
+    :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    :param fixed_decay: bool. fix weight decay.
+    """
+
+    def __init__(
+        self,
+        params: PARAMETERS,
+        lr: float = 1.0,
+        betas: BETAS = (0.9, 0.999),
+        d0: float = 1e-6,
+        weight_decay: float = 0.0,
+        weight_decouple: bool = False,
+        fixed_decay: bool = False,
+    ):
+        self.validate_learning_rate(lr)
+        self.validate_betas(betas)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'betas': betas,
+            'd': d0,
+            'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+            'fixed_decay': fixed_decay,
+            'step': 0,
+        }
+        super().__init__(params, defaults)
+
+    def __str__(self) -> str:
+        return 'DAdaptLion'
+
+    @torch.no_grad()
+    def reset(self):
+        for group in self.param_groups:
+            group['step'] = 0
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                state = self.state[p]
+
+                state['exp_avg'] = torch.zeros_like(p)
+                state['s'] = torch.zeros_like(p)
+
+    @torch.no_grad()
+    def step(self, closure: CLOSURE = None) -> LOSS:
+        loss: LOSS = None
+        if closure is not None:
+            with torch.enable_grad():
+                loss = closure()
+
+        group = self.param_groups[0]
+        device = group['params'][0].device
+
+        if 'numerator_weighted' not in group:
+            group['numerator_weighted'] = torch.tensor([0.0], device=device)
+        numerator_weighted = group['numerator_weighted']
+
+        sk_l1 = torch.tensor([0.0], device=device)
+        numerator_accumulator = torch.tensor([0.0], device=device)
+
+        beta1, beta2 = group['betas']
+        beta2_sq = math.sqrt(beta2)
+
+        d, lr = group['d'], group['lr']
+        d_lr: float = d * lr
+
+        for group in self.param_groups:
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                grad = p.grad
+                if grad.is_sparse:
+                    raise NoSparseGradientError(str(self))
+
+                state = self.state[p]
+                if len(state) == 0:
+                    state['exp_avg'] = torch.zeros_like(p)
+                    state['s'] = torch.zeros_like(p)
+
+                self.apply_weight_decay(
+                    p=p,
+                    grad=grad,
+                    lr=d_lr,
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=group['fixed_decay'],
+                )
+
+                exp_avg, s = state['exp_avg'], state['s']
+
+                update = exp_avg.clone().mul_(beta1).add_(grad, alpha=1.0 - beta1).sign_()
+                p.add_(update, alpha=-d_lr)
+
+                exp_avg.mul_(beta2).add_(grad, alpha=(1.0 - beta2) * d_lr)
+
+                numerator_accumulator.add_(torch.dot(update.flatten(), s.flatten()), alpha=d_lr)
+                s.mul_(beta2_sq).add_(update, alpha=(1.0 - beta2_sq) * d_lr)
+
+                sk_l1.add_(s.abs().sum())
+
+        numerator_weighted.mul_(beta2_sq).add_(numerator_accumulator, alpha=1.0 - beta2_sq)
+
+        if sk_l1 == 0:
+            return loss
+
+        if lr > 0.0:
+            d_hat: float = (numerator_weighted / ((1.0 - beta2_sq) * sk_l1)).item()
+            d = max(d, d_hat)
+
+        for group in self.param_groups:
+            group['step'] += 1
+
+            group['numerator_weighted'] = numerator_weighted
+            group['d'] = d
+
+        return loss
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/diffgrad.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/diffgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fp16.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/fp16.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         self.tolerance = tolerance
         self.threshold = threshold
 
         self.iter: int = 0
         self.last_overflow_iter: int = -1
         self.last_rescale_iter: int = -1
         self.overflows_since_rescale: int = 0
+        self.has_overflow_serial: bool = False
 
     def update_scale(self, overflow: bool):
         r"""Update the loss scale.
 
             If overflow exceeds our tolerance, we decrease the loss scale.
             If the number of iterations since the last overflow exceeds the scale window, we increase the loss scale.
 
@@ -85,15 +86,15 @@
         NOTE: the loss_scale will not go below `self.threshold`.
         """
         self.loss_scale /= self.scale_factor
         if self.threshold is not None:
             self.loss_scale = max(self.loss_scale, self.threshold)
 
 
-class SafeFP16Optimizer(Optimizer):
+class SafeFP16Optimizer(Optimizer):  # pragma: no cover
     r"""Safe FP16 Optimizer.
 
     :param optimizer: OPTIMIZER.
     :param aggregate_g_norms: bool. aggregate_g_norms.
     :param min_loss_scale: float. min_loss_scale.
     """
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/fromage.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/fromage.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/gravity.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/gravity.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lamb.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lars.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lars.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         dampening: float = 0.0,
         trust_coefficient: float = 1e-3,
         nesterov: bool = False,
     ):
         self.validate_learning_rate(lr)
         self.validate_non_negative(weight_decay, 'weight_decay')
         self.validate_range(momentum, 'momentum', 0.0, 1.0)
+        self.validate_range(dampening, 'dampening', 0.0, 1.0)
         self.validate_non_negative(trust_coefficient, 'trust_coefficient')
 
         defaults: DEFAULTS = {
             'lr': lr,
             'weight_decay': weight_decay,
             'momentum': momentum,
             'dampening': dampening,
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lion.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lion.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/lookahead.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/lookahead.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections import defaultdict
-from typing import Dict
+from typing import Callable, Dict
 
 import torch
+from torch.optim import Optimizer
 
 from pytorch_optimizer.base.optimizer import BaseOptimizer
-from pytorch_optimizer.base.types import CLOSURE, LOSS, OPTIMIZER, STATE
+from pytorch_optimizer.base.types import CLOSURE, DEFAULTS, LOSS, OPTIMIZER, STATE
 
 
-class Lookahead(BaseOptimizer):
+class Lookahead(Optimizer, BaseOptimizer):
     r"""k steps forward, 1 step back.
 
     :param optimizer: OPTIMIZER. base optimizer.
     :param k: int. number of lookahead steps.
     :param alpha: float. linear interpolation factor.
     :param pullback_momentum: str. change to inner optimizer momentum on interpolation update.
     """
@@ -23,33 +24,44 @@
         alpha: float = 0.5,
         pullback_momentum: str = 'none',
     ):
         self.validate_positive(k, 'k')
         self.validate_range(alpha, 'alpha', 0.0, 1.0)
         self.validate_options(pullback_momentum, 'pullback_momentum', ['none', 'reset', 'pullback'])
 
+        self._optimizer_step_pre_hooks: Dict[int, Callable] = {}
+        self._optimizer_step_post_hooks: Dict[int, Callable] = {}
+
         self.alpha = alpha
         self.k = k
         self.pullback_momentum = pullback_momentum
 
         self.optimizer = optimizer
         self.param_groups = self.optimizer.param_groups
+
         self.state: STATE = defaultdict(dict)
 
         for group in self.param_groups:
             if 'counter' not in group:
                 group['counter'] = 0
 
             for p in group['params']:
                 state = self.state[p]
                 state['slow_params'] = torch.empty_like(p)
                 state['slow_params'].copy_(p)
                 if self.pullback_momentum == 'pullback':
                     state['slow_momentum'] = torch.zeros_like(p)
 
+        self.defaults: DEFAULTS = {
+            'lookahead_alpha': alpha,
+            'lookahead_k': k,
+            'lookahead_pullback_momentum': pullback_momentum,
+            **optimizer.defaults,
+        }
+
     def __getstate__(self):
         return {
             'state': self.state,
             'optimizer': self.optimizer,
             'alpha': self.alpha,
             'k': self.k,
             'pullback_momentum': self.pullback_momentum,
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/madgrad.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/msvag.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/msvag.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/nero.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/nero.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/novograd.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/novograd.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pcgrad.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/pcgrad.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pid.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/pid.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/pnm.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/pnm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhadam.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/qhadam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/qhm.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/qhm.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/radam.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/ranger.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,34 @@
     :param eps: float. term added to the denominator to improve numerical stability.
     """
 
     def __init__(
         self,
         params: PARAMETERS,
         lr: float = 1e-3,
+        betas: BETAS = (0.95, 0.999),
         alpha: float = 0.5,
         k: int = 6,
         n_sma_threshold: int = 5,
         degenerated_to_sgd: bool = False,
-        betas: BETAS = (0.95, 0.999),
-        eps: float = 1e-5,
         weight_decay: float = 0.0,
         weight_decouple: bool = True,
         fixed_decay: bool = False,
         use_gc: bool = True,
         gc_conv_only: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
+        eps: float = 1e-5,
     ):
         self.validate_learning_rate(lr)
         self.validate_betas(betas)
-        self.validate_non_negative(weight_decay, 'weight_decay')
+        self.validate_range(alpha, 'alpha', 0.0, 1.0, range_type='[]')
         self.validate_positive(k, 'k')
+        self.validate_non_negative(weight_decay, 'weight_decay')
         self.validate_non_negative(eps, 'eps')
 
         self.n_sma_threshold = n_sma_threshold
         self.degenerated_to_sgd = degenerated_to_sgd
         self.use_gc = use_gc
         self.gc_gradient_threshold: int = 3 if gc_conv_only else 1
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/ranger21.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/ranger21.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,26 @@
             * Explore-exploit learning rate schedule
             * Lookahead
             * Softplus transformation
             * Gradient Normalization
             * Corrects the denominator (AdamD).
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
+    :param num_iterations: int. number of the total training steps. Ranger21 optimizer schedules the learning rate
+        with its own recipes.
     :param lr: float. learning rate.
     :param beta0: float. Manages the amplitude of the noise introduced by positive negative momentum
         While 0.9 is a recommended default value, you can use -0.5 to minimize the noise.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param use_softplus: bool. use softplus to smooth.
     :param beta_softplus: float. beta.
+    :param num_warm_up_iterations: Optional[int]. number of warm-up iterations. Ranger21 performs linear learning rate
+        warmup.
+    :param num_warm_down_iterations: Optional[int]. number of warm-down iterations. Ranger21 performs Explore-exploit
+        learning rate scheduling.
     :param agc_clipping_value: float.
     :param agc_eps: float. eps for AGC
     :param centralize_gradients: bool. use GC both convolution & fc layers.
     :param normalize_gradients: bool. use gradient normalization.
     :param lookahead_merge_time: int. merge time.
     :param lookahead_blending_alpha: float. blending alpha.
     :param weight_decay: float. weight decay (L2 penalty).
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/rotograd.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/rotograd.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     def backbone(self) -> nn.Module:
         return self._backbone[0]
 
     def to(self, *args, **kwargs):
         self.backbone.to(*args, **kwargs)
         for head in self.heads:
             head.to(*args, **kwargs)
-        return super(RotateOnly, self).to(*args, **kwargs)
+        return super().to(*args, **kwargs)
 
     def train(self, mode: bool = True) -> nn.Module:
         super().train(mode)
         self.backbone.train(mode)
         for head in self.heads:
             head.train(mode)
         return self
@@ -280,15 +280,15 @@
 
         :param losses: Sequence[torch.Tensor]. losses.
         :param backbone_loss: Optional[torch.Tensor]. backbone loss.
         """
         if not self.training:
             raise AssertionError('Backward should only be called when training')
 
-        if self.iteration_counter == 0 or self.iteration_counter == self.burn_in_period:
+        if self.iteration_counter in (0, self.burn_in_period):
             for i, loss in enumerate(losses):
                 self.initial_losses[i] = loss.item()
 
             if self.normalize_losses and backbone_loss is not None:
                 self.initial_backbone_loss = backbone_loss.item()
 
         self.iteration_counter += 1
@@ -342,15 +342,15 @@
     :param heads: List[nn.Module]. task-specific modules.
     :param latent_size: int. size of the shared representation, size of the output of the backbone.z.
     :param burn_in_period: int. When back-propagating towards the shared parameters, *each task loss is normalized
         dividing by its initial value*, :math:`{L_k(t)}/{L_k(t_0 = 0)}`. This parameter sets a number of iterations
         after which the denominator will be replaced by the value of the loss at that iteration, that is,
         :math:`t_0 = burn\_in\_period`. This is done to overcome problems with losses quickly changing
         in the first iterations.
-    :param normalized_losses: bool. Whether to use this normalized losses to back-propagate through the task-specific
+    :param normalize_losses: bool. Whether to use this normalized losses to back-propagate through the task-specific
         parameters as well.
     """
 
     num_tasks: int
     backbone: nn.Module
     heads: Sequence[nn.Module]
     rep: torch.Tensor
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgd.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sgd.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
     def __str__(self) -> str:
         return 'AccSGD'
 
     @torch.no_grad()
     def reset(self):
         for group in self.param_groups:
+            group['step'] = 0
             for p in group['params']:
                 state = self.state[p]
 
                 state['momentum_buffer'] = p.clone()
 
     @torch.no_grad()
     def step(self, closure: CLOSURE = None) -> LOSS:
@@ -82,16 +83,22 @@
                     raise NoSparseGradientError(str(self))
 
                 state = self.state[p]
 
                 if len(state) == 0:
                     state['momentum_buffer'] = p.clone()
 
-                if group['weight_decay'] > 0.0:
-                    grad.add_(p, alpha=group['weight_decay'])
+                self.apply_weight_decay(
+                    p,
+                    grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=False,
+                    fixed_decay=False,
+                )
 
                 buf = state['momentum_buffer']
                 buf.mul_((1.0 / beta) - 1.0).add_(grad, alpha=-large_lr).add_(p).mul_(beta)
 
                 p.add_(grad, alpha=-group['lr']).mul_(zeta).add_(buf, alpha=1.0 - zeta)
 
         return loss
@@ -173,19 +180,22 @@
                     buf.mul_(momentum).add_(grad, alpha=1.0 - group['dampening'])
 
                     if group['nesterov']:
                         grad.add_(buf, alpha=momentum)
                     else:
                         grad = buf
 
-                if group['weight_decay'] > 0.0:
-                    if group['weight_decouple']:
-                        p.mul_(1.0 - group['lr'] * group['weight_decay'])
-                    else:
-                        grad.add_(p, alpha=group['weight_decay'])
+                self.apply_weight_decay(
+                    p,
+                    grad,
+                    lr=group['lr'],
+                    weight_decay=group['weight_decay'],
+                    weight_decouple=group['weight_decouple'],
+                    fixed_decay=False,
+                )
 
                 p.add_(grad, alpha=-group['lr'])
 
         return loss
 
 
 class ASGD(Optimizer, BaseOptimizer):
@@ -307,7 +317,79 @@
                     weight_decouple=group['weight_decouple'],
                     fixed_decay=group['fixed_decay'],
                 )
 
                 p.add_(grad, alpha=-new_lr)
 
         return loss
+
+
+class SignSGD(Optimizer, BaseOptimizer):
+    r"""Compressed Optimisation for Non-Convex Problems.
+
+    :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
+    :param lr: float. learning rate.
+    :param momentum: float. momentum factor (0.0 = SignSGD, >0 = Signum).
+    :param weight_decay: float. weight decay (L2 penalty).
+    :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
+    """
+
+    def __init__(
+        self,
+        params: PARAMETERS,
+        lr: float = 1e-3,
+        momentum: float = 0.9,
+        weight_decay: float = 0.0,
+        weight_decouple: bool = True,
+    ):
+        self.validate_learning_rate(lr)
+        self.validate_range(momentum, 'beta', 0.0, 1.0)
+        self.validate_non_negative(weight_decay, 'weight_decay')
+
+        defaults: DEFAULTS = {
+            'lr': lr,
+            'momentum': momentum,
+            'weight_decay': weight_decay,
+            'weight_decouple': weight_decouple,
+        }
+        super().__init__(params, defaults)
+
+    @torch.no_grad()
+    def reset(self):
+        for group in self.param_groups:
+            group['step'] = 0
+            for p in group['params']:
+                state = self.state[p]
+
+                if group['momentum'] > 0.0:
+                    state['momentum_buffer'] = torch.zeros_like(p)
+
+    @torch.no_grad()
+    def step(self, closure: CLOSURE = None) -> LOSS:
+        loss: LOSS = None
+        if closure is not None:
+            with torch.enable_grad():
+                loss = closure()
+
+        for group in self.param_groups:
+            momentum = group['momentum']
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+
+                grad = p.grad
+                if grad.is_sparse:
+                    raise NoSparseGradientError(str(self))
+
+                state = self.state[p]
+                if momentum > 0.0:
+                    if len(state) == 0:
+                        state['momentum_buffer'] = torch.zeros_like(p)
+
+                    buf = state['momentum_buffer']
+                    buf.mul_(momentum).add_(grad, alpha=1.0 - momentum)
+                else:
+                    buf = grad
+
+                p.add_(torch.sign(buf), alpha=-group['lr'])
+
+        return loss
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sgdp.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sgdp.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/shampoo.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/shampoo_utils.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/shampoo_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/sm3.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/sm3.py`

 * *Files identical despite different names*

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/srmm.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/srmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class SRMM(Optimizer, BaseOptimizer):
     """Stochastic regularized majorization-minimization with weakly convex and multi-convex surrogates.
 
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param beta: float. adaptivity weight.
-    :param l: Optional[int]. internal memory length for moving average. None for no refreshing.
+    :param memory_length: Optional[int]. internal memory length for moving average. None for no refreshing.
     """
 
     def __init__(self, params: PARAMETERS, lr: float = 0.01, beta: float = 0.5, memory_length: Optional[int] = 100):
         self.validate_learning_rate(lr)
         self.validate_range(beta, 'beta', 0.0, 1.0, range_type='[]')
 
         defaults: DEFAULTS = {'lr': lr, 'beta': beta, 'memory_length': memory_length}
@@ -49,15 +49,15 @@
         for group in self.param_groups:
             if 'step' in group:
                 group['step'] += 1
             else:
                 group['step'] = 1
 
             w_t: float = (
-                (group['step'] + 1) % (group['memory_length'] if group['memory_length'] is not None else 1)
+                (group['step'] % (group['memory_length'] if group['memory_length'] is not None else 1)) + 1
             ) ** -group['beta']
 
             for p in group['params']:
                 if p.grad is None:
                     continue
 
                 grad = p.grad
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/swats.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/swats.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from pytorch_optimizer.base.optimizer import BaseOptimizer
 from pytorch_optimizer.base.types import BETAS, CLOSURE, DEFAULTS, LOSS, PARAMETERS
 
 
 class SWATS(Optimizer, BaseOptimizer):
     r"""Improving Generalization Performance by Switching from Adam to SGD.
 
-        Currently, there's convergence issue. So, careful at using it.
-
     :param params: PARAMETERS. iterable of parameters to optimize or dicts defining parameter groups.
     :param lr: float. learning rate.
     :param betas: BETAS. coefficients used for computing running averages of gradient and the squared hessian trace.
     :param weight_decay: float. weight decay (L2 penalty).
     :param weight_decouple: bool. the optimizer uses decoupled weight decay as in AdamW.
     :param fixed_decay: bool. fix weight decay.
     :param ams_bound: bool. whether to use the ams_bound variant of this algorithm from the paper.
@@ -36,15 +34,15 @@
         weight_decouple: bool = False,
         fixed_decay: bool = False,
         ams_bound: bool = False,
         nesterov: bool = False,
         r: float = 0.95,
         adanorm: bool = False,
         adam_debias: bool = False,
-        eps: float = 1e-9,
+        eps: float = 1e-6,
     ):
         self.validate_learning_rate(lr)
         self.validate_betas(betas)
         self.validate_non_negative(weight_decay, 'weight_decay')
         self.validate_non_negative(eps, 'eps')
 
         defaults: DEFAULTS = {
@@ -132,21 +130,21 @@
                 if group['phase'] == 'sgd':
                     if 'momentum_buffer' not in state:
                         state['momentum_buffer'] = torch.zeros_like(grad)
 
                     buf = state['momentum_buffer']
                     buf.mul_(beta1).add_(grad)
 
-                    grad = buf.clone()
+                    update = buf.clone()
+                    update.mul_(1.0 - beta1)
 
-                    grad.mul_(1.0 - beta1)
                     if group['nesterov']:
-                        grad.add_(buf, alpha=beta1)
+                        update.add_(buf, alpha=beta1)
 
-                    p.add_(grad, alpha=-group['lr'])
+                    p.add_(update, alpha=-group['lr'])
 
                     continue
 
                 s_grad = self.get_adanorm_gradient(
                     grad=grad,
                     adanorm=group['adanorm'],
                     exp_grad_norm=state.get('exp_grad_norm', None),
@@ -167,27 +165,31 @@
                 step_size: float = self.apply_adam_debias(
                     adam_debias=group['adam_debias'],
                     step_size=group['lr'] * math.sqrt(bias_correction2),
                     bias_correction1=bias_correction1,
                 )
 
                 perturb = exp_avg.clone()
-                perturb.div_(de_nom).mul(-step_size)
+                perturb.div_(de_nom).mul_(-step_size)
 
                 p.add_(perturb)
 
                 perturb_view = perturb.view(-1)
                 pg = perturb_view.dot(grad.view(-1))
 
                 if pg != 0:
                     scaling = perturb_view.dot(perturb_view).div_(-pg)
 
                     exp_avg2 = state['exp_avg2']
                     exp_avg2.mul_(beta2).add_(scaling, alpha=1.0 - beta2)
 
                     corrected_exp_avg = exp_avg2 / bias_correction2
 
-                    if group['step'] > 1 and corrected_exp_avg.allclose(scaling, rtol=group['eps']):
+                    if (
+                        group['step'] > 1
+                        and corrected_exp_avg > 0.0
+                        and corrected_exp_avg.allclose(scaling, rtol=group['eps'])
+                    ):
                         group['phase'] = 'sgd'
                         group['lr'] = corrected_exp_avg.item()
 
         return loss
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/utils.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def is_valid_parameters(parameters: PARAMETERS) -> bool:
     r"""Check where the parameters are valid."""
     return isinstance(parameters, (list, tuple)) and len(parameters) > 0 and isinstance(parameters[0], dict)
 
 
 def has_overflow(grad_norm: torch.Tensor) -> bool:
     r"""Detect inf and NaN in grad_norm."""
-    return grad_norm != grad_norm or grad_norm == float('inf')
+    return bool(torch.logical_or(torch.isnan(grad_norm), torch.isinf(grad_norm)).any())
 
 
 def to_real(x: torch.Tensor) -> torch.Tensor:
     r"""Return real value of tensor."""
     return x.real if torch.is_complex(x) else x
 
 
@@ -83,15 +83,19 @@
     :param view_func: Callable. view (channel or layer) function.
     """
     x = view_func(x)
     y = view_func(y)
     return f.cosine_similarity(x, y, dim=1, eps=eps).abs_()
 
 
-def clip_grad_norm(parameters: PARAMETERS, max_norm: float = 0, sync: bool = False) -> Union[torch.Tensor, float]:
+def clip_grad_norm(
+    parameters: PARAMETERS,
+    max_norm: float = 0.0,
+    sync: bool = False,
+) -> Union[torch.Tensor, float]:  # pragma: no cover
     r"""Clip gradient norms.
 
         During combination with FSDP, will also ensure that grad norms are aggregated across all workers,
         since each worker only stores their shard of the gradients.
 
     :param parameters: PARAMETERS. Parameters whose gradients we wish to clip.
     :param max_norm: float. Maximum norm we wish the gradients to have. If non-positive, then we will not perform
@@ -270,7 +274,34 @@
     if dim >= rank:
         raise ValueError(f'[-] given dim is bigger than rank. {dim} >= {rank}')
 
     for d in range(rank):
         if d != dim:
             x = x.max(dim=d, keepdim=True).values
     return x
+
+
+def reg_noise(
+    network1: nn.Module, network2: nn.Module, num_data: int, lr: float, eta: float = 8e-3, temperature: float = 1e-4
+) -> torch.Tensor | float:
+    r"""Entropy-MCMC: Sampling from flat basins with ease.
+
+    usage: https://github.com/lblaoke/EMCMC/blob/master/exp/cifar10_emcmc.py
+
+    :param network1: nn.Module. network.
+    :param network2: nn.Module. network.
+    :param num_data: int. number of training data.
+    :param lr: float. learning rate.
+    :param eta: float. eta.
+    :param temperature: float. temperature.
+    """
+    reg_coef: float = 0.5 / (eta * num_data)
+    noise_coef: float = math.sqrt(2.0 / lr / num_data * temperature)
+
+    loss = 0
+    for param1, param2 in zip(network1.parameters(), network2.parameters(), strict=True):
+        reg = torch.sub(param1, param2).pow_(2) * reg_coef
+        noise1 = param1 * torch.randn_like(param1) * noise_coef
+        noise2 = param2 * torch.randn_like(param2) * noise_coef
+        loss += torch.sum(reg - noise1 - noise2)
+
+    return loss
```

### Comparing `pytorch_optimizer-2.9.1/pytorch_optimizer/optimizer/yogi.py` & `pytorch_optimizer-3.0.0/pytorch_optimizer/optimizer/yogi.py`

 * *Files identical despite different names*

