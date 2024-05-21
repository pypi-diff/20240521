# Comparing `tmp/heartkit-1.2.0.tar.gz` & `tmp/heartkit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartkit-1.2.0.tar", max compression
+gzip compressed data, was "heartkit-1.3.0.tar", max compression
```

## Comparing `heartkit-1.2.0.tar` & `heartkit-1.3.0.tar`

### file list

```diff
@@ -1,97 +1,150 @@
--rw-r--r--   0        0        0     1513 2024-04-24 18:00:28.337505 heartkit-1.2.0/LICENSE
--rw-r--r--   0        0        0     7079 2024-04-24 18:00:28.337505 heartkit-1.2.0/README.md
--rw-r--r--   0        0        0      604 2024-04-24 18:00:28.369506 heartkit-1.2.0/heartkit/__init__.py
--rw-r--r--   0        0        0       36 2024-04-24 18:00:28.369506 heartkit-1.2.0/heartkit/__main__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:00:28.369506 heartkit-1.2.0/heartkit/assets/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:00:28.369506 heartkit-1.2.0/heartkit/assets/data/__init__.py
--rw-r--r--   0        0        0  5849305 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/assets/data/nstdb.h5
--rw-r--r--   0        0        0     2061 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/cli.py
--rw-r--r--   0        0        0      924 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/__init__.py
--rw-r--r--   0        0        0     5669 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/augmentation.py
--rw-r--r--   0        0        0    15060 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/dataset.py
--rw-r--r--   0        0        0      319 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/defines.py
--rw-r--r--   0        0        0     1026 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/download.py
--rw-r--r--   0        0        0     1408 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/factory.py
--rw-r--r--   0        0        0    38829 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/icentia11k.py
--rw-r--r--   0        0        0    28262 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/lsad.py
--rw-r--r--   0        0        0    13700 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/ludb.py
--rw-r--r--   0        0        0     3032 2024-04-24 18:00:28.401506 heartkit-1.2.0/heartkit/datasets/nstdb.py
--rw-r--r--   0        0        0    32532 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/datasets/ptbxl.py
--rw-r--r--   0        0        0    15213 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/datasets/qtdb.py
--rw-r--r--   0        0        0    11572 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/datasets/synthetic.py
--rw-r--r--   0        0        0     1660 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/datasets/utils.py
--rw-r--r--   0        0        0    12575 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/defines.py
--rw-r--r--   0        0        0    11360 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/metrics.py
--rw-r--r--   0        0        0     1116 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/__init__.py
--rw-r--r--   0        0        0    10378 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/blocks.py
--rw-r--r--   0        0        0     2795 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/callbacks.py
--rw-r--r--   0        0        0      691 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/defines.py
--rw-r--r--   0        0        0     4740 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/efficientnet.py
--rw-r--r--   0        0        0     1965 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/factory.py
--rw-r--r--   0        0        0    11359 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/mobileone.py
--rw-r--r--   0        0        0     5674 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/multiresnet.py
--rw-r--r--   0        0        0     5288 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/resnet.py
--rw-r--r--   0        0        0    13280 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/tcn.py
--rw-r--r--   0        0        0     3776 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/tsmixer.py
--rw-r--r--   0        0        0    10009 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/unet.py
--rw-r--r--   0        0        0    11407 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/unext.py
--rw-r--r--   0        0        0     4388 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/models/utils.py
--rw-r--r--   0        0        0      529 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/__init__.py
--rw-r--r--   0        0        0     3675 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/client.py
--rw-r--r--   0        0        0     2342 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/common.py
--rw-r--r--   0        0        0      686 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/interface.py
--rw-r--r--   0        0        0     4209 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/server.py
--rw-r--r--   0        0        0      529 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/__init__.py
--rw-r--r--   0        0        0     2934 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/client.py
--rw-r--r--   0        0        0     2342 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/common.py
--rw-r--r--   0        0        0      568 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/interface.py
--rw-r--r--   0        0        0     3394 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/server.py
--rw-r--r--   0        0        0      306 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/__init__.py
--rw-r--r--   0        0        0     6819 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/backends.py
--rw-r--r--   0        0        0      793 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/__init__.py
--rw-r--r--   0        0        0     4462 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/arbitrator.py
--rw-r--r--   0        0        0     4367 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/basic_codec.py
--rw-r--r--   0        0        0     2631 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/client.py
--rw-r--r--   0        0        0     3536 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/codec.py
--rw-r--r--   0        0        0      845 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/crc16.py
--rw-r--r--   0        0        0      176 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/erpc_version.py
--rw-r--r--   0        0        0     2223 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/server.py
--rw-r--r--   0        0        0     1274 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/simple_server.py
--rw-r--r--   0        0        0    14420 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/erpc/transport.py
--rw-r--r--   0        0        0     1370 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/factory.py
--rw-r--r--   0        0        0     2290 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/rpc/utils.py
--rw-r--r--   0        0        0      519 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/__init__.py
--rw-r--r--   0        0        0      200 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/beat/__init__.py
--rw-r--r--   0        0        0    22258 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/beat/beat.py
--rw-r--r--   0        0        0      132 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/beat/defines.py
--rw-r--r--   0        0        0     8795 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/beat/utils.py
--rw-r--r--   0        0        0        0 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/defines.py
--rw-r--r--   0        0        0      178 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/denoise/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/denoise/defines.py
--rw-r--r--   0        0        0    20844 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/denoise/denoise.py
--rw-r--r--   0        0        0     2665 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/denoise/metrics.py
--rw-r--r--   0        0        0     9234 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/denoise/utils.py
--rw-r--r--   0        0        0      236 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/diagnostic/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/diagnostic/defines.py
--rw-r--r--   0        0        0    19666 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/diagnostic/diagnostic.py
--rw-r--r--   0        0        0     8823 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/diagnostic/utils.py
--rw-r--r--   0        0        0     1431 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/factory.py
--rw-r--r--   0        0        0      235 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/rhythm/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/rhythm/defines.py
--rw-r--r--   0        0        0    20273 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/rhythm/rhythm.py
--rw-r--r--   0        0        0     8743 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/rhythm/utils.py
--rw-r--r--   0        0        0      179 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/segmentation/__init__.py
--rw-r--r--   0        0        0      180 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/segmentation/defines.py
--rw-r--r--   0        0        0     1576 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/segmentation/metrics.py
--rw-r--r--   0        0        0    25348 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/segmentation/segmentation.py
--rw-r--r--   0        0        0     8353 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/segmentation/utils.py
--rw-r--r--   0        0        0     1016 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tasks/task.py
--rw-r--r--   0        0        0      240 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tflite/__init__.py
--rw-r--r--   0        0        0     9306 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tflite/convert.py
--rw-r--r--   0        0        0     2759 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tflite/metrics.py
--rw-r--r--   0        0        0     2359 2024-04-24 18:00:28.405506 heartkit-1.2.0/heartkit/tflite/model.py
--rw-r--r--   0        0        0     4216 2024-04-24 18:00:28.409506 heartkit-1.2.0/heartkit/utils.py
--rw-r--r--   0        0        0     2802 2024-04-24 18:00:28.409506 heartkit-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 18:00:28.409506 heartkit-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      326 2024-04-24 18:00:28.409506 heartkit-1.2.0/tests/app_test.py
--rw-r--r--   0        0        0     8446 1970-01-01 00:00:00.000000 heartkit-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1513 2024-05-21 21:20:31.304646 heartkit-1.3.0/LICENSE
+-rw-r--r--   0        0        0     7079 2024-05-21 21:20:31.304646 heartkit-1.3.0/README.md
+-rw-r--r--   0        0        0      593 2024-05-21 21:20:31.336647 heartkit-1.3.0/heartkit/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-21 21:20:31.336647 heartkit-1.3.0/heartkit/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:20:31.336647 heartkit-1.3.0/heartkit/assets/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:20:31.336647 heartkit-1.3.0/heartkit/assets/data/__init__.py
+-rw-r--r--   0        0        0  5849305 2024-05-21 21:20:31.368647 heartkit-1.3.0/heartkit/assets/data/nstdb.h5
+-rw-r--r--   0        0        0     2109 2024-05-21 21:20:31.368647 heartkit-1.3.0/heartkit/cli.py
+-rw-r--r--   0        0        0     1084 2024-05-21 21:20:31.368647 heartkit-1.3.0/heartkit/datasets/__init__.py
+-rw-r--r--   0        0        0     5400 2024-05-21 21:20:31.368647 heartkit-1.3.0/heartkit/datasets/augmentation.py
+-rw-r--r--   0        0        0     7059 2024-05-21 21:20:31.368647 heartkit-1.3.0/heartkit/datasets/dataloader.py
+-rw-r--r--   0        0        0     4097 2024-05-21 21:20:31.368647 heartkit-1.3.0/heartkit/datasets/dataset.py
+-rw-r--r--   0        0        0      207 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/defines.py
+-rw-r--r--   0        0        0      974 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/download.py
+-rw-r--r--   0        0        0     1408 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/factory.py
+-rw-r--r--   0        0        0    16073 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/icentia11k.py
+-rw-r--r--   0        0        0    23099 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/lsad.py
+-rw-r--r--   0        0        0    10796 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/ludb.py
+-rw-r--r--   0        0        0     3272 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/nstdb.py
+-rw-r--r--   0        0        0      895 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/preprocessing.py
+-rw-r--r--   0        0        0    24279 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/ptbxl.py
+-rw-r--r--   0        0        0    12339 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/qtdb.py
+-rw-r--r--   0        0        0     8600 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/synthetic.py
+-rw-r--r--   0        0        0     9455 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/datasets/utils.py
+-rw-r--r--   0        0        0    12661 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/defines.py
+-rw-r--r--   0        0        0    11360 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/metrics.py
+-rw-r--r--   0        0        0     1323 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/__init__.py
+-rw-r--r--   0        0        0    11011 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/blocks.py
+-rw-r--r--   0        0        0     2795 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/callbacks.py
+-rw-r--r--   0        0        0      802 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/defines.py
+-rw-r--r--   0        0        0     4977 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/efficientnet.py
+-rw-r--r--   0        0        0     1979 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/factory.py
+-rw-r--r--   0        0        0    11359 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/mobileone.py
+-rw-r--r--   0        0        0     5674 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/multiresnet.py
+-rw-r--r--   0        0        0       56 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/optimizers/__init__.py
+-rw-r--r--   0        0        0    19556 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/optimizers/contrastive.py
+-rw-r--r--   0        0        0     5302 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/resnet.py
+-rw-r--r--   0        0        0     2989 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/sequentialnet.py
+-rw-r--r--   0        0        0    13294 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/tcn.py
+-rw-r--r--   0        0        0     3776 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/tsmixer.py
+-rw-r--r--   0        0        0    10009 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/unet.py
+-rw-r--r--   0        0        0    11407 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/unext.py
+-rw-r--r--   0        0        0     4388 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/models/utils.py
+-rw-r--r--   0        0        0      529 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/__init__.py
+-rw-r--r--   0        0        0     3675 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/client.py
+-rw-r--r--   0        0        0     2342 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/common.py
+-rw-r--r--   0        0        0      686 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/interface.py
+-rw-r--r--   0        0        0     4209 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/server.py
+-rw-r--r--   0        0        0      529 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/__init__.py
+-rw-r--r--   0        0        0     2934 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/client.py
+-rw-r--r--   0        0        0     2342 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/common.py
+-rw-r--r--   0        0        0      568 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/interface.py
+-rw-r--r--   0        0        0     3394 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/server.py
+-rw-r--r--   0        0        0      306 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/__init__.py
+-rw-r--r--   0        0        0     6830 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/backends.py
+-rw-r--r--   0        0        0      793 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/__init__.py
+-rw-r--r--   0        0        0     4462 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/arbitrator.py
+-rw-r--r--   0        0        0     4367 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/basic_codec.py
+-rw-r--r--   0        0        0     2631 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/client.py
+-rw-r--r--   0        0        0     3536 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/codec.py
+-rw-r--r--   0        0        0      845 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/crc16.py
+-rw-r--r--   0        0        0      176 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/erpc_version.py
+-rw-r--r--   0        0        0     2223 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/server.py
+-rw-r--r--   0        0        0     1274 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/simple_server.py
+-rw-r--r--   0        0        0    14420 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/erpc/transport.py
+-rw-r--r--   0        0        0     1370 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/factory.py
+-rw-r--r--   0        0        0     2290 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/rpc/utils.py
+-rw-r--r--   0        0        0      631 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/dataloaders/__init__.py
+-rw-r--r--   0        0        0     6114 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/dataloaders/icentia11k.py
+-rw-r--r--   0        0        0     9933 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/datasets.py
+-rw-r--r--   0        0        0      132 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/defines.py
+-rw-r--r--   0        0        0     8199 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/demo.py
+-rw-r--r--   0        0        0     3471 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/evaluate.py
+-rw-r--r--   0        0        0     4429 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/export.py
+-rw-r--r--   0        0        0     7196 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/train.py
+-rw-r--r--   0        0        0     2239 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/beat/utils.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/defines.py
+-rw-r--r--   0        0        0      595 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/denoise/__init__.py
+-rw-r--r--   0        0        0      126 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/denoise/dataloaders/__init__.py
+-rw-r--r--   0        0        0     1203 2024-05-21 21:20:31.372647 heartkit-1.3.0/heartkit/tasks/denoise/dataloaders/lsad.py
+-rw-r--r--   0        0        0     1207 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/dataloaders/ptbxl.py
+-rw-r--r--   0        0        0     1223 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/dataloaders/synthetic.py
+-rw-r--r--   0        0        0     9150 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/datasets.py
+-rw-r--r--   0        0        0     4886 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/demo.py
+-rw-r--r--   0        0        0     2501 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/evaluate.py
+-rw-r--r--   0        0        0     4083 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/export.py
+-rw-r--r--   0        0        0     2665 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/metrics.py
+-rw-r--r--   0        0        0     5815 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/train.py
+-rw-r--r--   0        0        0     2038 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/denoise/utils.py
+-rw-r--r--   0        0        0      635 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/dataloaders/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/dataloaders/lsad.py
+-rw-r--r--   0        0        0     3623 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/dataloaders/ptbxl.py
+-rw-r--r--   0        0        0     9950 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/datasets.py
+-rw-r--r--   0        0        0     1377 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/defines.py
+-rw-r--r--   0        0        0     4166 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/demo.py
+-rw-r--r--   0        0        0     2736 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/evaluate.py
+-rw-r--r--   0        0        0     4308 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/export.py
+-rw-r--r--   0        0        0     7546 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/train.py
+-rw-r--r--   0        0        0     2235 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/diagnostic/utils.py
+-rw-r--r--   0        0        0     1431 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/factory.py
+-rw-r--r--   0        0        0      624 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/__init__.py
+-rw-r--r--   0        0        0       78 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/dataloaders/__init__.py
+-rw-r--r--   0        0        0     2101 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/dataloaders/lsad.py
+-rw-r--r--   0        0        0     2105 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/dataloaders/ptbxl.py
+-rw-r--r--   0        0        0     8719 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/datasets.py
+-rw-r--r--   0        0        0     4919 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/demo.py
+-rw-r--r--   0        0        0      326 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/evaluate.py
+-rw-r--r--   0        0        0     2863 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/export.py
+-rw-r--r--   0        0        0     5297 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/foundation/train.py
+-rw-r--r--   0        0        0      623 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/__init__.py
+-rw-r--r--   0        0        0      183 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/dataloaders/__init__.py
+-rw-r--r--   0        0        0     5334 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/dataloaders/icentia11k.py
+-rw-r--r--   0        0        0     2446 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/dataloaders/lsad.py
+-rw-r--r--   0        0        0     2150 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/dataloaders/ptbxl.py
+-rw-r--r--   0        0        0    10397 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/datasets.py
+-rw-r--r--   0        0        0     1168 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/defines.py
+-rw-r--r--   0        0        0     4163 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/demo.py
+-rw-r--r--   0        0        0     3359 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/evaluate.py
+-rw-r--r--   0        0        0     4538 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/export.py
+-rw-r--r--   0        0        0     7199 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/train.py
+-rw-r--r--   0        0        0     2181 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/rhythm/utils.py
+-rw-r--r--   0        0        0      636 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/dataloaders/__init__.py
+-rw-r--r--   0        0        0     5606 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/dataloaders/icentia11k.py
+-rw-r--r--   0        0        0     3490 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/dataloaders/ludb.py
+-rw-r--r--   0        0        0     4472 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/dataloaders/ptbxl.py
+-rw-r--r--   0        0        0     2292 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/dataloaders/qtdb.py
+-rw-r--r--   0        0        0     3704 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/dataloaders/synthetic.py
+-rw-r--r--   0        0        0     9994 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/datasets.py
+-rw-r--r--   0        0        0      180 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/defines.py
+-rw-r--r--   0        0        0     8453 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/demo.py
+-rw-r--r--   0        0        0     2559 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/evaluate.py
+-rw-r--r--   0        0        0     4412 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/export.py
+-rw-r--r--   0        0        0     1576 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/metrics.py
+-rw-r--r--   0        0        0     8203 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/train.py
+-rw-r--r--   0        0        0     1793 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/segmentation/utils.py
+-rw-r--r--   0        0        0     1016 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/task.py
+-rw-r--r--   0        0        0      535 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tasks/utils.py
+-rw-r--r--   0        0        0      240 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tflite/__init__.py
+-rw-r--r--   0        0        0     9359 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tflite/convert.py
+-rw-r--r--   0        0        0     2759 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tflite/metrics.py
+-rw-r--r--   0        0        0     2359 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/tflite/model.py
+-rw-r--r--   0        0        0     6043 2024-05-21 21:20:31.376647 heartkit-1.3.0/heartkit/utils.py
+-rw-r--r--   0        0        0     2865 2024-05-21 21:20:31.380647 heartkit-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 21:20:31.380647 heartkit-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-21 21:20:31.380647 heartkit-1.3.0/tests/app_test.py
+-rw-r--r--   0        0        0     8446 1970-01-01 00:00:00.000000 heartkit-1.3.0/PKG-INFO
```

### Comparing `heartkit-1.2.0/LICENSE` & `heartkit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/README.md` & `heartkit-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/__init__.py` & `heartkit-1.3.0/heartkit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     HKExportParams,
     HKMode,
     HKTestParams,
     HKTrainParams,
     PreprocessParams,
 )
 from .models import ModelFactory
-from .tasks import HeartRate, HKBeat, HKRhythm, HKSegment, HKTask, TaskFactory
+from .tasks import HKBeat, HKRhythm, HKSegment, HKTask, TaskFactory
 from .utils import setup_logger
 
 __version__ = version(__name__)
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
 setup_logger(__name__)
```

### Comparing `heartkit-1.2.0/heartkit/assets/data/nstdb.h5` & `heartkit-1.3.0/heartkit/assets/data/nstdb.h5`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/cli.py` & `heartkit-1.3.0/heartkit/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,17 @@
             content = f.read()
 
     return cls.model_validate_json(json_data=content)
 
 
 @cli.command(name="run")
 def _run(
-    mode: HKMode = ArgField("-m", description="Mode"),
-    task: str = ArgField("-t", description="Task"),
-    config: str = ArgField("-c", description="File path or JSON content"),
+    mode: HKMode = ArgField("-m", description="Mode", default=HKMode.train),
+    task: str = ArgField("-t", description="Task", default=""),
+    config: str = ArgField("-c", description="File path or JSON content", default="{}"),
 ):
     """HeartKit CLI"""
 
     logger.info(f"#STARTED MODE={mode} TASK={task}")
 
     if mode == HKMode.download:
         download_datasets(parse_content(HKDownloadParams, config))
```

### Comparing `heartkit-1.2.0/heartkit/datasets/augmentation.py` & `heartkit-1.3.0/heartkit/datasets/augmentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,15 @@
 import numpy as np
 import numpy.typing as npt
 import physiokit as pk
 
-from ..defines import AugmentationParams, PreprocessParams
+from ..defines import AugmentationParams
+from .nstdb import NstdbNoise
 
-
-def preprocess_pipeline(x: npt.NDArray, preprocesses: list[PreprocessParams], sample_rate: float) -> npt.NDArray:
-    """Apply preprocessing pipeline
-
-    Args:
-        x (npt.NDArray): Signal
-        preprocesses (list[PreprocessParams]): Preprocessing pipeline
-        sample_rate (float): Sampling rate in Hz.
-
-    Returns:
-        npt.NDArray: Preprocessed signal
-    """
-    for preprocess in preprocesses:
-        match preprocess.name:
-            case "filter":
-                x = pk.signal.filter_signal(x, sample_rate=sample_rate, **preprocess.params)
-            case "znorm":
-                x = pk.signal.normalize_signal(x, **preprocess.params)
-            case _:
-                raise ValueError(f"Unknown preprocess '{preprocess.name}'")
-        # END MATCH
-    # END FOR
-    return x
+_nstdb_glb: NstdbNoise | None = None
 
 
 def augment_pipeline(
     x: npt.NDArray,
     augmentations: list[AugmentationParams] | None = None,
     sample_rate: float = 1000,
 ) -> tuple[npt.NDArray, npt.NDArray | None]:
@@ -111,25 +90,35 @@
                     scale=x_sd * np.random.uniform(scale[0], scale[1]),
                 )
             case "cutout":
                 feat_len = x.shape[0]
                 prob = args.get("probability", [0, 0.25])[1]
                 amp = args.get("amplitude", [0, 0])
                 width = args.get("width", [0, 1])
-                ctype = args.get("type", "cut")
+                ctype = args.get("type", "cut")[0]
                 if np.random.rand() < prob:
                     dur = int(np.random.uniform(width[0], width[1]) * feat_len)
                     start = np.random.randint(0, feat_len - dur)
                     stop = start + dur
                     scale = np.random.uniform(amp[0], amp[1]) * x_sd
-                    if ctype == "cut":
+                    if ctype == 0:  # Cut
                         x[start:stop] = 0
-                    else:
+                    else:  # noise
                         x[start:stop] += np.random.normal(0, scale, size=x[start:stop].shape)
                     # END IF
-            # END IF
+                # END IF
+
+            case "nstdb":
+                global _nstdb_glb  # pylint: disable=global-statement
+                if _nstdb_glb is None:
+                    _nstdb_glb = NstdbNoise(target_rate=sample_rate)
+                _nstdb_glb.set_target_rate(sample_rate)
+                noise_range = args.get("noise_level", [0.1, 0.1])
+                noise_level = np.random.uniform(noise_range[0], noise_range[1])
+                x = _nstdb_glb.apply_noise(x, noise_level)
+
             case _:  # default
                 pass
                 # raise ValueError(f"Unknown augmentation '{augmentation.name}'")
         # END MATCH
     # END FOR
     return x
```

### Comparing `heartkit-1.2.0/heartkit/datasets/download.py` & `heartkit-1.3.0/heartkit/datasets/download.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,19 +18,18 @@
     os.makedirs(params.job_dir, exist_ok=True)
     logger.info(f"Creating working directory in {params.job_dir}")
 
     handler = logging.FileHandler(params.job_dir / "download.log", mode="w")
     handler.setLevel(logging.INFO)
     logger.addHandler(handler)
 
-    os.makedirs(params.ds_path, exist_ok=True)
-
-    for ds_name in params.datasets:
-        if DatasetFactory.has(ds_name):
-            Dataset = DatasetFactory.get(ds_name)
-            ds = Dataset(ds_path=params.ds_path, task="", frame_size=1, target_rate=1, spec=((), ()))
+    for ds in params.datasets:
+        if DatasetFactory.has(ds.name):
+            os.makedirs(ds.path, exist_ok=True)
+            Dataset = DatasetFactory.get(ds.name)
+            ds = Dataset(ds_path=ds.path, **ds.params)
             ds.download(
                 num_workers=params.data_parallelism,
                 force=params.force,
             )
         # END IF
     # END FOR
```

### Comparing `heartkit-1.2.0/heartkit/datasets/factory.py` & `heartkit-1.3.0/heartkit/datasets/factory.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/datasets/ludb.py` & `heartkit-1.3.0/heartkit/datasets/qtdb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,86 +1,64 @@
+import contextlib
 import functools
 import logging
 import os
 import random
 import tempfile
 import zipfile
 from multiprocessing import Pool
-from pathlib import Path
+from typing import Generator
 
 import h5py
 import numpy as np
 import numpy.typing as npt
 import physiokit as pk
-import tensorflow as tf
 from tqdm import tqdm
 
 from ..utils import download_file
 from .dataset import HKDataset
-from .defines import PatientGenerator, SampleGenerator
+from .defines import PatientGenerator
+from .utils import download_s3_objects
 
 logger = logging.getLogger(__name__)
 
-LudbSymbolMap = {
+QtdbSymbolMap = {
     "o": 0,  # Other
     "p": 1,  # P Wave
     "N": 2,  # QRS complex
     "t": 3,  # T Wave
 }
-LudbLeadsMap = {
-    "i": 0,
-    "ii": 1,
-    "iii": 2,
-    "avr": 3,
-    "avl": 4,
-    "avf": 5,
-    "v1": 6,
-    "v2": 7,
-    "v3": 8,
-    "v4": 9,
-    "v5": 10,
-    "v6": 11,
-}
 
 FID_LEAD_IDX = 0
 FID_LBL_IDX = 1
 FID_LOC_IDX = 2
 SEG_LEAD_IDX = 0
 SEG_LBL_IDX = 1
 SEG_BEG_IDX = 2
 SEG_END_IDX = 3
 
 
-class LudbDataset(HKDataset):
-    """LUDB dataset"""
+class QtdbDataset(HKDataset):
+    """QT dataset"""
 
     def __init__(
         self,
         ds_path: os.PathLike,
-        task: str,
-        frame_size: int,
-        target_rate: int,
-        spec: tuple[tf.TensorSpec, tf.TensorSpec],
-        class_map: dict[int, int] | None = None,
-        leads: list[int] | None = None,
     ) -> None:
-        super().__init__(
-            ds_path=ds_path / "ludb",
-            task=task,
-            frame_size=frame_size,
-            target_rate=target_rate,
-            spec=spec,
-            class_map=class_map,
-        )
-        self.leads = leads or list(range(12))
+        super().__init__(ds_path=ds_path)
+
+    @property
+    def name(self) -> str:
+        """Dataset name"""
+        return "qtdb"
 
     @property
     def sampling_rate(self) -> int:
         """Sampling rate in Hz"""
-        return 500
+        return 250
 
     @property
     def mean(self) -> float:
         """Dataset mean"""
         return 0
 
     @property
@@ -91,241 +69,305 @@
     @property
     def patient_ids(self) -> npt.NDArray:
         """Get dataset patient IDs
 
         Returns:
             npt.NDArray: patient IDs
         """
-        return np.arange(1, 201)
+
+        # fmt: off
+        return np.array(
+            [
+                30,
+                31,
+                32,
+                33,
+                34,
+                35,
+                36,
+                37,
+                38,
+                39,
+                40,
+                41,
+                42,
+                43,
+                44,
+                45,
+                46,
+                47,
+                48,
+                49,
+                50,
+                51,
+                52,
+                100,
+                102,
+                103,
+                104,
+                106,
+                107,
+                110,
+                111,
+                112,
+                114,
+                116,
+                117,
+                121,
+                122,
+                123,
+                124,
+                126,
+                129,
+                133,
+                136,
+                166,
+                170,
+                203,
+                210,
+                211,
+                213,
+                221,
+                223,
+                230,
+                231,
+                232,
+                233,
+                301,
+                302,
+                303,
+                306,
+                307,
+                308,
+                310,
+                405,
+                406,
+                409,
+                411,
+                509,
+                603,
+                604,
+                606,
+                607,
+                609,
+                612,
+                704,
+                803,
+                808,
+                811,
+                820,
+                821,
+                840,
+                847,
+                853,
+                871,
+                872,
+                873,
+                883,
+                891,
+                14046,
+                14157,
+                14172,
+                15814,
+                16265,
+                16272,
+                16273,
+                16420,
+                16483,
+                16539,
+                16773,
+                16786,
+                16795,
+                17152,
+                17453,
+            ]
+            # fmt: on
+        )  # 104, 114, 116 have multiple recordings
 
     def get_train_patient_ids(self) -> npt.NDArray:
         """Get dataset training patient IDs
 
         Returns:
             npt.NDArray: patient IDs
         """
-        return self.patient_ids[:180]
+        return self.patient_ids[:82]
 
     def get_test_patient_ids(self) -> npt.NDArray:
         """Get dataset patient IDs reserved for testing only
 
         Returns:
             npt.NDArray: patient IDs
         """
-        return self.patient_ids[180:]
+        return self.patient_ids[82:]
 
-    def task_data_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Task-level data generator.
+    def _pt_key(self, patient_id: int):
+        """Get patient key"""
+        return f"{patient_id}"
+
+    @contextlib.contextmanager
+    def patient_data(self, patient_id: int) -> Generator[h5py.Group, None, None]:
+        """Get patient data
 
         Args:
-            patient_generator (PatientGenerator): Patient data generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
+            patient_id (int): Patient ID
 
         Returns:
-            SampleGenerator: Sample data generator
+            Generator[h5py.Group, None, None]: Patient data
         """
-        if self.task == "segmentation":
-            return self.segmentation_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
-        raise NotImplementedError()
+        with h5py.File(self.ds_path / f"{self._pt_key(patient_id)}.h5", mode="r") as h5:
+            yield h5
 
-    def segmentation_generator(
+    def signal_generator(
         self,
         patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Generate frames and segment labels.
-
-        Args:
-            patient_generator (PatientGenerator): Patient Generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
-
-        Returns:
-            SampleGenerator: Sample generator
-
-        Yields:
-            Iterator[SampleGenerator]
-        """
-        for _, pt in patient_generator:
-            # NOTE: [:] will load all data into RAM- ideal for small dataset
-            data = pt["data"][:]
-            segs = pt["segmentations"][:]
-            fids = pt["fiducials"][:]
-
-            if self.sampling_rate != self.target_rate:
-                ratio = self.target_rate / self.sampling_rate
-                data = pk.signal.resample_signal(data, self.sampling_rate, self.target_rate, axis=0)
-                segs[:, (SEG_BEG_IDX, SEG_END_IDX)] = segs[:, (SEG_BEG_IDX, SEG_END_IDX)] * ratio
-                fids[:, FID_LOC_IDX] = fids[:, FID_LOC_IDX] * ratio
-            # END IF
-
-            # Create segmentation mask
-            labels = np.zeros_like(data)
-            for seg_idx in range(segs.shape[0]):
-                seg = segs[seg_idx]
-                labels[seg[SEG_BEG_IDX] : seg[SEG_END_IDX], seg[SEG_LEAD_IDX]] = seg[SEG_LBL_IDX]
-            # END FOR
-
-            start_offset = max(0, segs[0][SEG_BEG_IDX] - 100)
-            stop_offset = max(0, data.shape[0] - segs[-1][SEG_END_IDX] + 100)
-            for _ in range(samples_per_patient):
-                # Randomly pick an ECG lead
-                # lead = np.random.randint(data.shape[1])
-                lead = random.choice(self.leads)
-                # Randomly select frame within the segment
-                frame_start = np.random.randint(start_offset, data.shape[0] - self.frame_size - stop_offset)
-                frame_end = frame_start + self.frame_size
-                x = data[frame_start:frame_end, lead].astype(np.float32)
-                y = labels[frame_start:frame_end, lead].astype(np.int32)
-                y = np.vectorize(self.class_map.get, otypes=[int])(y)
-                yield x, y
-            # END FOR
-        # END FOR
-
-    def signal_generator(self, patient_generator: PatientGenerator, samples_per_patient: int = 1) -> SampleGenerator:
-        """
-        Generate frames using patient generator.
-        from the segments in patient data by placing a frame in a random location within one of the segments.
+        frame_size: int,
+        samples_per_patient: int = 1,
+        target_rate: int | None = None,
+    ) -> Generator[npt.NDArray, None, None]:
+        """Generate random frames.
 
         Args:
             patient_generator (PatientGenerator): Generator that yields a tuple of patient id and patient data.
                     Patient data may contain only signals, since labels are not used.
             samples_per_patient (int): Samples per patient.
 
         Returns:
-            SampleGenerator: Generator of input data of shape (frame_size, 1)
+            Generator[npt.NDArray, None, None]: Generator of input data of shape (frame_size, 1)
         """
-        for _, pt in patient_generator:
-            data = pt["data"][:]
-            if self.sampling_rate != self.target_rate:
-                data = pk.signal.resample_signal(data, self.sampling_rate, self.target_rate, axis=0)
-            # END IF
+        if target_rate is None:
+            target_rate = self.sampling_rate
+
+        input_size = int(np.round((self.sampling_rate / target_rate) * frame_size))
+
+        for pt in patient_generator:
+            with self.patient_data(pt) as h5:
+                data: h5py.Dataset = h5["data"][:]
+            # END WITH
             for _ in range(samples_per_patient):
-                # lead = np.random.randint(data.shape[1])
-                lead = random.choice(self.leads)
-                if data.shape[0] > self.frame_size:
-                    frame_start = np.random.randint(data.shape[0] - self.frame_size)
-                else:
-                    frame_start = 0
-                frame_end = frame_start + self.frame_size
-                x = data[frame_start:frame_end, lead].astype(np.float32)
+                lead = random.choice(data.shape[1])
+                start = np.random.randint(0, data.shape[0] - input_size)
+                x = data[start : start + input_size, lead].squeeze()
+                x = np.nan_to_num(x).astype(np.float32)
+                if self.sampling_rate != target_rate:
+                    x = pk.signal.resample_signal(x, self.sampling_rate, target_rate, axis=0)
+                # END IF
                 yield x
             # END FOR
         # END FOR
 
-    def get_patient_data_segments(self, patient: int) -> tuple[npt.NDArray, npt.NDArray]:
+    def get_patient_data_segments(self, patient_id: int) -> tuple[npt.NDArray, npt.NDArray]:
         """Get patient's entire data and segments
 
         Args:
             patient (int): Patient ID (1-based)
 
         Returns:
             tuple[npt.NDArray, npt.NDArray]: (data, segment labels)
         """
-        pt_key = f"p{patient:05d}"
-        with h5py.File(self.ds_path / f"{pt_key}.h5", mode="r") as pt:
+        with self.patient_data(patient_id) as pt:
             data: npt.NDArray = pt["data"][:]
             segs: npt.NDArray = pt["segmentations"][:]
         labels = np.zeros_like(data)
         for seg_idx in range(segs.shape[0]):  # pylint: disable=no-member
             seg = segs[seg_idx]
-            labels[seg[SEG_BEG_IDX] : seg[SEG_END_IDX] + 0, seg[SEG_LEAD_IDX]] = seg[SEG_LBL_IDX]
-        # END FOR
+            labels[seg[2] : seg[3] + 0, seg[0]] = seg[1]
         return data, labels
 
-    def uniform_patient_generator(
-        self,
-        patient_ids: npt.NDArray,
-        repeat: bool = True,
-        shuffle: bool = True,
-    ) -> PatientGenerator:
-        """Yield data for each patient in the array.
+    def download(self, num_workers: int | None = None, force: bool = False):
+        """Download QT dataset
 
         Args:
-            patient_ids (pt.ArrayLike): Array of patient ids
-            repeat (bool, optional): Whether to repeat generator. Defaults to True.
-            shuffle (bool, optional): Whether to shuffle patient ids.. Defaults to True.
+            num_workers (int | None, optional): # parallel workers. Defaults to None.
+            force (bool, optional): Force redownload. Defaults to False.
+        """
+        download_s3_objects(
+            bucket="ambiq-ai-datasets",
+            prefix=self.ds_path.stem,
+            dst=self.ds_path.parent,
+            checksum="size",
+            progress=True,
+            num_workers=num_workers,
+        )
 
-        Returns:
-            PatientGenerator: Patient generator
+    def download_raw_dataset(self, num_workers: int | None = None, force: bool = False):
+        """Downloads full dataset zipfile and converts into individial patient HDF5 files.
 
-        Yields:
-            Iterator[PatientGenerator]
+        Args:
+            force (bool, optional): Whether to force re-download if destination exists. Defaults to False.
+            num_workers (int, optional): # parallel workers. Defaults to os.cpu_count().
         """
-        patient_ids = np.copy(patient_ids)
-        while True:
-            if shuffle:
-                np.random.shuffle(patient_ids)
-            for patient_id in patient_ids:
-                pt_key = f"p{patient_id:05d}"
-                with h5py.File(self.ds_path / f"{pt_key}.h5", mode="r") as h5:
-                    yield patient_id, h5
-            # END FOR
-            if not repeat:
-                break
-        # END WHILE
+        logger.info("Downloading QTDB dataset")
+        ds_url = "https://physionet.org/static/published-projects/qtdb/qt-database-1.0.0.zip"
+        ds_zip_path = self.ds_path / "qtdb.zip"
+        os.makedirs(self.ds_path, exist_ok=True)
+        if os.path.exists(ds_zip_path) and not force:
+            logger.warning(
+                f"Zip file already exists. Please delete or set `force` flag to redownload. PATH={ds_zip_path}"
+            )
+        else:
+            download_file(ds_url, ds_zip_path, progress=True)
+
+        # 2. Extract and convert patient ECG data to H5 files
+        logger.info("Generating QT patient data")
+        self.convert_dataset_zip_to_hdf5(zip_path=ds_zip_path, force=force, num_workers=num_workers)
+        logger.info("Finished QTDB patient data")
 
     def convert_pt_wfdb_to_hdf5(
         self, patient: int, src_path: os.PathLike, dst_path: os.PathLike, force: bool = False
     ) -> tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
-        """Convert LUDB patient data from WFDB to more consumable HDF5 format.
+        """Convert QTDB patient data from WFDB to more consumable HDF5 format.
 
         Args:
             patient (int): Patient id (1-based)
-            src_path (str): Source path to WFDB folder
-            dst_path (str): Destination path to store HDF5 file
+            src_path (PathLike): Source path to WFDB folder
+            dst_path (PathLike): Destination path to store HDF5 file
 
         Returns:
             tuple[npt.NDArray, npt.NDArray, npt.NDArray]: data, segments, and fiducials
         """
         import wfdb  # pylint: disable=import-outside-toplevel
 
-        pt_id = f"p{patient:05d}"
-        pt_src_path = str(src_path / f"{patient}")
+        pt_id = f"sel{patient}" if os.path.isfile(src_path / f"sel{patient}.dat") else f"sele{patient:04d}"
+        pt_src_path = str(src_path / pt_id)
         rec = wfdb.rdrecord(pt_src_path)
         data = np.zeros_like(rec.p_signal)
         segs = []
         fids = []
-        for i, lead in enumerate(rec.sig_name):
-            lead_id = LudbLeadsMap.get(lead)
-            ann = wfdb.rdann(pt_src_path, extension=lead)
+        for i, _ in enumerate(rec.sig_name):
+            lead_id = i
+
+            ann = wfdb.rdann(pt_src_path, extension=f"pu{lead_id}")
+
             seg_start = seg_stop = sym_id = None
             data[:, lead_id] = rec.p_signal[:, i]
             for j, symbol in enumerate(ann.symbol):
                 # Start of segment
                 if symbol == "(":
                     seg_start = ann.sample[j]
                     seg_stop = None
                 # Fiducial / segment type
-                elif symbol in LudbSymbolMap:
-                    sym_id = LudbSymbolMap.get(symbol)
+                elif symbol in QtdbSymbolMap:
+                    sym_id = QtdbSymbolMap.get(symbol)
                     if seg_start is None:
                         seg_start = ann.sample[j]
                     fids.append([lead_id, sym_id, ann.sample[j]])
-                # End of segment (start and symbol are never 0 but can be None)
                 elif symbol == ")" and seg_start and sym_id:
                     seg_stop = ann.sample[j]
                     segs.append([lead_id, sym_id, seg_start, seg_stop])
                 else:
                     seg_start = seg_stop = None
                     sym_id = None
             # END FOR
         # END FOR
-        segs = np.array(segs)
         fids = np.array(fids)
+        segs = np.array(segs)
 
         if dst_path:
             os.makedirs(dst_path, exist_ok=True)
-            pt_dst_path = dst_path / f"{pt_id}.h5"
+            pt_dst_path = dst_path / f"{patient}.h5"
             with h5py.File(pt_dst_path, "w") as h5:
                 h5.create_dataset("data", data=data, compression="gzip")
                 h5.create_dataset("segmentations", data=segs, compression="gzip")
                 h5.create_dataset("fiducials", data=fids, compression="gzip")
             # END WITH
         # END IF
 
@@ -345,48 +387,22 @@
             patient_ids (npt.NDArray | None, optional): List of patient IDs to extract. Defaults to all.
             force (bool, optional): Whether to force re-download if destination exists. Defaults to False.
             num_workers (int, optional): # parallel workers. Defaults to os.cpu_count().
         """
         if not patient_ids:
             patient_ids = self.patient_ids
 
-        subdir = "lobachevsky-university-electrocardiography-database-1.0.1"
+        subdir = "qt-database-1.0.0"
         with Pool(processes=num_workers) as pool, tempfile.TemporaryDirectory() as tmpdir, zipfile.ZipFile(
             zip_path, mode="r"
         ) as zp:
-            ludb_dir = Path(tmpdir, "ludb")
-            zp.extractall(ludb_dir)
+            qtdb_dir = tmpdir / "qtdb"
+            zp.extractall(qtdb_dir)
+
             f = functools.partial(
                 self.convert_pt_wfdb_to_hdf5,
-                src_path=ludb_dir / subdir / "data",
+                src_path=qtdb_dir / subdir,
                 dst_path=self.ds_path,
                 force=force,
             )
             _ = list(tqdm(pool.imap(f, patient_ids), total=len(patient_ids)))
         # END WITH
-
-    def download(self, num_workers: int | None = None, force: bool = False):
-        """Download LUDB dataset
-
-        Args:
-            num_workers (int | None, optional): # parallel workers. Defaults to None.
-            force (bool, optional): Force redownload. Defaults to False.
-        """
-
-        logger.info("Downloading LUDB dataset")
-        ds_url = (
-            "https://physionet.org/static/published-projects/ludb/"
-            "lobachevsky-university-electrocardiography-database-1.0.1.zip"
-        )
-        ds_zip_path = self.ds_path / "ludb.zip"
-        os.makedirs(self.ds_path, exist_ok=True)
-        if os.path.exists(ds_zip_path) and not force:
-            logger.warning(
-                f"Zip file already exists. Please delete or set `force` flag to redownload. PATH={ds_zip_path}"
-            )
-        else:
-            download_file(ds_url, ds_zip_path, progress=True)
-
-        # 2. Extract and convert patient ECG data to H5 files
-        logger.info("Generating LUDB patient data")
-        self.convert_dataset_zip_to_hdf5(zip_path=ds_zip_path, force=force, num_workers=num_workers)
-        logger.info("Finished LUDB patient data")
```

### Comparing `heartkit-1.2.0/heartkit/datasets/nstdb.py` & `heartkit-1.3.0/heartkit/datasets/nstdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,31 @@
 
 
 class NstdbNoise:
     """Noise stress test database (NSTDB) noise generator."""
 
     def __init__(
         self,
-        ds_path: os.PathLike,
         target_rate: int,
     ):
-        self.path = ds_path
         self.target_rate = target_rate
         self._noises: dict[str, npt.NDArray] | None = None
 
     @property
     def sampling_rate(self) -> int:
         """Sampling rate in Hz"""
         return 360
 
+    def set_target_rate(self, target_rate: int):
+        """Set target rate."""
+        if target_rate == self.target_rate:
+            return
+        self._noises = None
+        self.target_rate = target_rate
+
     def _load_noise_data(self):
         """Load noise data from HDF5 file."""
         logger.debug("Loading noise data from HDF5 file.")
         _file_path = os.path.realpath(__file__)
         noise_path = Path(_file_path).parent.parent / "assets" / "data" / "nstdb.h5"
         with h5py.File(noise_path, "r") as f:
             bw = pk.signal.resample_signal(f["bw"][:], self.sampling_rate, self.target_rate, axis=0)
@@ -90,7 +95,11 @@
         em_amp = np.abs(np.random.normal(0, noise_level))
 
         data += bw_amp * bw[bw_start:bw_end, bw_lead]
         data += ma_amp * ma[ma_start:ma_end, ma_lead]
         data += em_amp * em[em_start:em_end, em_lead]
 
         return data
+
+    def close(self):
+        """Close noise generator."""
+        self._noises = None
```

### Comparing `heartkit-1.2.0/heartkit/datasets/ptbxl.py` & `heartkit-1.3.0/heartkit/datasets/ptbxl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import contextlib
+import functools
 import logging
 import os
 import random
 from collections.abc import Iterable
 from enum import IntEnum
 from multiprocessing import Pool
+from typing import Generator
 
 import h5py
 import numpy as np
 import numpy.typing as npt
 import physiokit as pk
 import sklearn.model_selection
-import tensorflow as tf
 from tqdm import tqdm
 
-from ..tasks import HKDiagnostic, HKRhythm, HKSegment
 from ..utils import download_file
 from .dataset import HKDataset
-from .defines import PatientGenerator, SampleGenerator
+from .defines import PatientGenerator
+from .utils import download_s3_objects
 
 logger = logging.getLogger(__name__)
 
 
 class PtbxlScpCode(IntEnum):
     """PTBXL SCP codes"""
 
@@ -174,80 +176,14 @@
     "BIGU": PtbxlScpCode.BIGU,
     "AFLT": PtbxlScpCode.AFLT,
     "SVTAC": PtbxlScpCode.SVTAC,
     "PSVT": PtbxlScpCode.PSVT,
     "TRIGU": PtbxlScpCode.TRIGU,
 }
 
-PtbxlRhythmMap = {
-    PtbxlScpCode.SR: HKRhythm.sr,
-    PtbxlScpCode.AFIB: HKRhythm.afib,
-    PtbxlScpCode.AFLT: HKRhythm.aflut,
-    PtbxlScpCode.STACH: HKRhythm.stach,
-    PtbxlScpCode.SBRAD: HKRhythm.sbrad,
-    PtbxlScpCode.SARRH: HKRhythm.sarrh,
-    PtbxlScpCode.SVARR: HKRhythm.svarr,
-    PtbxlScpCode.SVTAC: HKRhythm.svt,
-    PtbxlScpCode.PSVT: HKRhythm.svt,
-    PtbxlScpCode.BIGU: HKRhythm.bigu,
-    PtbxlScpCode.TRIGU: HKRhythm.trigu,
-    PtbxlScpCode.PACE: HKRhythm.pace,
-}
-
-PtbxlDiagnosticMap = {
-    # NORM
-    PtbxlScpCode.NORM: HKDiagnostic.NORM,
-    # STTC
-    PtbxlScpCode.NDT: HKDiagnostic.STTC,
-    PtbxlScpCode.NST_: HKDiagnostic.STTC,
-    PtbxlScpCode.DIG: HKDiagnostic.STTC,
-    PtbxlScpCode.LNGQT: HKDiagnostic.STTC,
-    PtbxlScpCode.ISC_: HKDiagnostic.STTC,
-    PtbxlScpCode.ISCAL: HKDiagnostic.STTC,
-    PtbxlScpCode.ISCIN: HKDiagnostic.STTC,
-    PtbxlScpCode.ISCIL: HKDiagnostic.STTC,
-    PtbxlScpCode.ISCAS: HKDiagnostic.STTC,
-    PtbxlScpCode.ISCLA: HKDiagnostic.STTC,
-    PtbxlScpCode.ANEUR: HKDiagnostic.STTC,
-    PtbxlScpCode.EL: HKDiagnostic.STTC,
-    PtbxlScpCode.ISCAN: HKDiagnostic.STTC,
-    # MI
-    PtbxlScpCode.IMI: HKDiagnostic.MI,
-    PtbxlScpCode.ASMI: HKDiagnostic.MI,
-    PtbxlScpCode.ILMI: HKDiagnostic.MI,
-    PtbxlScpCode.AMI: HKDiagnostic.MI,
-    PtbxlScpCode.ALMI: HKDiagnostic.MI,
-    PtbxlScpCode.INJAS: HKDiagnostic.MI,
-    PtbxlScpCode.LMI: HKDiagnostic.MI,
-    PtbxlScpCode.INJAL: HKDiagnostic.MI,
-    PtbxlScpCode.IPLMI: HKDiagnostic.MI,
-    PtbxlScpCode.IPMI: HKDiagnostic.MI,
-    PtbxlScpCode.INJIN: HKDiagnostic.MI,
-    PtbxlScpCode.INJLA: HKDiagnostic.MI,
-    PtbxlScpCode.PMI: HKDiagnostic.MI,
-    PtbxlScpCode.INJIL: HKDiagnostic.MI,
-    # HYP
-    PtbxlScpCode.LVH: HKDiagnostic.HYP,
-    PtbxlScpCode.LAO_LAE: HKDiagnostic.HYP,
-    PtbxlScpCode.RVH: HKDiagnostic.HYP,
-    PtbxlScpCode.RAO_RAE: HKDiagnostic.HYP,
-    PtbxlScpCode.SEHYP: HKDiagnostic.HYP,
-    # CD
-    PtbxlScpCode.LAFB: HKDiagnostic.CD,
-    PtbxlScpCode.IRBBB: HKDiagnostic.CD,
-    PtbxlScpCode.AVB1: HKDiagnostic.CD,
-    PtbxlScpCode.IVCD: HKDiagnostic.CD,
-    PtbxlScpCode.CRBBB: HKDiagnostic.CD,
-    PtbxlScpCode.CLBBB: HKDiagnostic.CD,
-    PtbxlScpCode.LPFB: HKDiagnostic.CD,
-    PtbxlScpCode.WPW: HKDiagnostic.CD,
-    PtbxlScpCode.ILBBB: HKDiagnostic.CD,
-    PtbxlScpCode.AVB2: HKDiagnostic.CD,
-    PtbxlScpCode.AVB3: HKDiagnostic.CD,
-}
 
 PtbxlLeadsMap = {
     "i": 0,
     "ii": 1,
     "iii": 2,
     "avr": 3,
     "avl": 4,
@@ -263,30 +199,26 @@
 
 class PtbxlDataset(HKDataset):
     """PTBXL dataset"""
 
     def __init__(
         self,
         ds_path: os.PathLike,
-        task: str,
-        frame_size: int,
-        target_rate: int,
-        spec: tuple[tf.TensorSpec, tf.TensorSpec],
-        class_map: dict[int, int] | None = None,
         leads: list[int] | None = None,
     ) -> None:
         super().__init__(
-            ds_path=ds_path / "ptbxl",
-            task=task,
-            frame_size=frame_size,
-            target_rate=target_rate,
-            spec=spec,
-            class_map=class_map,
+            ds_path=ds_path,
         )
         self.leads = leads or list(range(12))
+        self._data_cache: dict[str, np.ndarray] = {}
+
+    @property
+    def name(self) -> str:
+        """Dataset name"""
+        return "ptbxl"
 
     @property
     def sampling_rate(self) -> int:
         """Sampling rate in Hz"""
         return 500
 
     @property
@@ -366,244 +298,139 @@
         """
         return self.patient_ids[18500:]
 
     def _pt_key(self, patient_id: int):
         """Get patient key"""
         return f"{patient_id:05d}"
 
-    def task_data_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Task-level data generator.
+    def label_key(self, label_type: str = "scp") -> str:
+        """Get label key
 
         Args:
-            patient_generator (PatientGenerator): Patient data generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
+            label_type (str, optional): Label type. Defaults to "scp".
 
         Returns:
-            SampleGenerator: Sample data generator
+            str: Label key
         """
-        if self.task == "rhythm":
-            return self.rhythm_data_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
-
-        if self.task == "diagnostic":
-            return self.diagnostic_data_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
-
-        if self.task == "denoise":
-            return self.denoising_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
-
-        if self.task == "segmentation":
-            return self.segmentation_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
+        if label_type == "scp":
+            return "slabels"
+        if label_type == "beat":
+            return "blabels"
+        raise ValueError(f"Invalid label type: {label_type}")
 
-        raise NotImplementedError()
-
-    def uniform_patient_generator(
-        self,
-        patient_ids: npt.NDArray,
-        repeat: bool = True,
-        shuffle: bool = True,
-    ) -> PatientGenerator:
-        """Yield data for each patient in the array.
+    @contextlib.contextmanager
+    def patient_data(self, patient_id: int) -> Generator[h5py.Group, None, None]:
+        """Get patient data
 
         Args:
-            patient_ids (pt.ArrayLike): Array of patient ids
-            repeat (bool, optional): Whether to repeat generator. Defaults to True.
-            shuffle (bool, optional): Whether to shuffle patient ids.. Defaults to True.
+            patient_id (int): Patient ID
 
         Returns:
-            PatientGenerator: Patient generator
-
-        Yields:
-            Iterator[PatientGenerator]
+            Generator[h5py.Group, None, None]: Patient data
         """
-        patient_ids = np.copy(patient_ids)
-        while True:
-            if shuffle:
-                np.random.shuffle(patient_ids)
-            for patient_id in patient_ids:
-                pt_key = self._pt_key(patient_id)
-                with h5py.File(self.ds_path / f"{pt_key}.h5", mode="r") as h5:
-                    yield patient_id, h5
-                # END WITH
-            # END FOR
-            if not repeat:
-                break
-            # END IF
-        # END WHILE
+        with h5py.File(self.ds_path / f"{self._pt_key(patient_id)}.h5", mode="r") as h5:
+            yield h5
 
-    def random_patient_generator(
+    def signal_generator(
         self,
-        patient_ids: list[int],
-        patient_weights: list[int] | None = None,
-    ) -> PatientGenerator:
-        """Samples patient data from the provided patient distribution.
-
-        Args:
-            patient_ids (list[int]): Patient ids
-            patient_weights (list[int] | None, optional): Probabilities associated with each patient. Defaults to None.
-
-        Returns:
-            PatientGenerator: Patient generator
-
-        Yields:
-            Iterator[PatientGenerator]
-        """
-        while True:
-            for patient_id in np.random.choice(patient_ids, size=1024, p=patient_weights):
-                pt_key = self._pt_key(patient_id)
-                with h5py.File(self.ds_path / f"{pt_key}.h5", mode="r") as h5:
-                    yield patient_id, h5
-                # END WITH
-            # END FOR
-        # END WHILE
-
-    def signal_generator(self, patient_generator: PatientGenerator, samples_per_patient: int = 1) -> SampleGenerator:
-        """Generate random frames using patient generator.
+        patient_generator: PatientGenerator,
+        frame_size: int,
+        samples_per_patient: int = 1,
+        target_rate: int | None = None,
+    ) -> Generator[npt.NDArray, None, None]:
+        """Generate random frames.
 
         Args:
             patient_generator (PatientGenerator): Generator that yields a tuple of patient id and patient data.
                     Patient data may contain only signals, since labels are not used.
             samples_per_patient (int): Samples per patient.
 
         Returns:
-            SampleGenerator: Generator of input data of shape (frame_size, 1)
+            Generator[npt.NDArray, None, None]: Generator of input data of shape (frame_size, 1)
         """
-        input_size = int(np.round((self.sampling_rate / self.target_rate) * self.frame_size))
-        for _, segment in patient_generator:
-            data = segment["data"][:]
+        if target_rate is None:
+            target_rate = self.sampling_rate
+
+        input_size = int(np.round((self.sampling_rate / target_rate) * frame_size))
+
+        for pt in patient_generator:
+            with self.patient_data(pt) as h5:
+                data: h5py.Dataset = h5["data"][:]
+            # END WITH
             for _ in range(samples_per_patient):
                 lead = random.choice(self.leads)
                 start = np.random.randint(0, data.shape[1] - input_size)
                 x = data[lead, start : start + input_size].squeeze()
                 x = np.nan_to_num(x).astype(np.float32)
-                if self.sampling_rate != self.target_rate:
-                    x = pk.signal.resample_signal(x, self.sampling_rate, self.target_rate, axis=0)
+                if self.sampling_rate != target_rate:
+                    x = pk.signal.resample_signal(x, self.sampling_rate, target_rate, axis=0)
                 # END IF
                 yield x
             # END FOR
         # END FOR
 
-    def denoising_generator(
+    def signal_label_generator(
         self,
         patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Generate frames and noise frames."""
-        gen = self.signal_generator(patient_generator, samples_per_patient)
-        for x in gen:
-            y = x.copy()
-            yield x, y
-
-    def rhythm_data_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Generate frames w/ rhythm labels (e.g. afib) using patient generator.
-
-        Args:
-            patient_generator (PatientGenerator): Patient Generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
-
-        Returns:
-            SampleGenerator: Sample generator
-
-        Yields:
-            Iterator[SampleGenerator]
-        """
-        return self._label_data_generator(
-            patient_generator=patient_generator,
-            local_map=PtbxlRhythmMap,
-            samples_per_patient=samples_per_patient,
-        )
-
-    def diagnostic_data_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Generate frames w/ diagnostic labels using patient generator.
-
-        Args:
-            patient_generator (PatientGenerator): Patient Generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
-
-        Returns:
-            SampleGenerator: Sample generator
-
-        Yields:
-            Iterator[SampleGenerator]
-        """
-        return self._label_data_generator(
-            patient_generator=patient_generator,
-            local_map=PtbxlDiagnosticMap,
-            samples_per_patient=samples_per_patient,
-            label_format="multi_hot",
-        )
-
-    def _label_data_generator(
-        self,
-        patient_generator: PatientGenerator,
-        local_map: dict[int, int],
-        samples_per_patient: int | list[int] = 1,
+        frame_size: int,
+        samples_per_patient: int = 1,
+        target_rate: int | None = None,
+        label_map: dict[int, int] | None = None,
+        label_type: str = "scp",
         label_format: str | None = None,
-    ) -> SampleGenerator:
+    ) -> Generator[tuple[npt.NDArray, int], None, None]:
         """Generate frames w/ labels using patient generator.
 
         Args:
             patient_generator (PatientGenerator): Patient Generator
-            local_map (dict[int, int]): Local label map
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
+            frame_size (int): Frame size
+            samples_per_patient (int, optional): Samples per patient. Defaults to 1.
+            target_rate (int, optional): Target rate. Defaults to None.
+            label_map (dict[int, int], optional): Label map. Defaults to None.
+            label_type (str, optional): Class type. Defaults to "scp".
             label_format (str, optional): Label format. Defaults to None.
 
         Returns:
-            SampleGenerator: Sample generator
+            Generator[tuple[npt.NDArray, int], None, None]: Generator of input data and labels
 
         Yields:
-            Iterator[SampleGenerator]
+            tuple[npt.NDArray, int]: Input data and label
         """
-        # Target labels and mapping
-        tgt_labels = list(set(self.class_map.values()))
+        if target_rate is None:
+            target_rate = self.sampling_rate
+        # END IF
 
-        # Convert dataset labels -> HK labels -> class map labels (-1 indicates not in class map)
-        tgt_map = {k: self.class_map.get(v, -1) for (k, v) in local_map.items()}
+        # Target labels and mapping
+        tgt_labels = sorted(list(set((lbl for lbl in label_map.values() if lbl != -1))))
+        label_key = self.label_key(label_type)
         num_classes = len(tgt_labels)
 
         # If samples_per_patient is a list, then it must be the same length as nclasses
         if isinstance(samples_per_patient, Iterable):
             samples_per_tgt = samples_per_patient
         else:
             num_per_tgt = int(max(1, samples_per_patient / num_classes))
             samples_per_tgt = num_classes * [num_per_tgt]
+        # END IF
 
-        input_size = int(np.round((self.sampling_rate / self.target_rate) * self.frame_size))
+        input_size = int(np.round((self.sampling_rate / target_rate) * frame_size))
 
-        for _, seg in patient_generator:
-            # 1. Grab patient scp labels (fixed for all samples)
-            slabels = seg["slabels"][:]
+        for pt in patient_generator:
+
+            # 1. Grab patient scp label (fixed for all samples)
+            with self.patient_data(pt) as h5:
+                data = h5["data"][:]
+                slabels = h5[label_key][:]
+            # END WITH
 
             # 2. Map scp labels (skip patient if not in class map == -1)
             pt_lbls = []
             pt_lbl_weights = []
             for i in range(slabels.shape[0]):
-                label = tgt_map.get(int(slabels[i, 0]), -1)
+                label = label_map.get(int(slabels[i, 0]), -1)
                 if label == -1:
                     continue
                 # END IF
                 if label not in pt_lbls:
                     pt_lbls.append(label)
                     pt_lbl_weights.append(1 + slabels[i, 1])
                 else:
@@ -628,112 +455,165 @@
                 # Its possible to have multiple labels, we assign based on weights
                 y = random.choices(pt_lbls, pt_lbl_weights, k=1)[0]
                 num_samples = samples_per_tgt[tgt_labels.index(y)]
             else:
                 raise ValueError(f"Invalid label_format: {label_format}")
 
             # 3. Generate samples based on samples_per_tgt
-            data = seg["data"][:]
+
+            # print(f'{pt} creating {num_samples} samples')
             for _ in range(num_samples):
                 # select random lead and start index
                 lead = random.choice(self.leads)
                 # lead = self.leads
                 start = np.random.randint(0, data.shape[1] - input_size)
                 # Extract frame
                 x = np.nan_to_num(data[lead, start : start + input_size], posinf=0, neginf=0).astype(np.float32)
                 # Resample if needed
-                if self.sampling_rate != self.target_rate:
-                    x = pk.signal.resample_signal(x, self.sampling_rate, self.target_rate, axis=0)
+                if self.sampling_rate != target_rate:
+                    x = pk.signal.resample_signal(x, self.sampling_rate, target_rate, axis=0)
                 yield x, y
             # END FOR
         # END FOR
 
-    def segmentation_generator(
+    def split_train_test_patients(
         self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Gnerate frames with annotated segments.
+        patient_ids: npt.NDArray,
+        test_size: float,
+        label_map: dict[int, int] | None = None,
+        label_type: str | None = None,
+    ) -> list[list[int]]:
+        """Perform train/test split on patients for given task.
+        NOTE: We only perform inter-patient splits and not intra-patient.
 
         Args:
-            patient_generator (PatientGenerator): Patient generator
-            samples_per_patient (int | list[int], optional):
+            patient_ids (npt.NDArray): Patient Ids
+            test_size (float): Test size
+            label_map (dict[int, int], optional): Label map. Defaults to None.
+            label_type (str, optional): Label type. Defaults to None.
 
         Returns:
-            SampleGenerator: Sample generator
+            list[list[int]]: Train and test sets of patient ids
         """
-        assert not isinstance(samples_per_patient, Iterable)
-        input_size = int(np.round((self.sampling_rate / self.target_rate) * self.frame_size))
+        stratify = None
+        if label_map is not None and label_type is not None:
+            patients_labels = self.get_patients_labels(patient_ids, label_map=label_map, label_type=label_type)
+            # Select random label for stratification or -1 if no labels
+            stratify = np.array([random.choice(x) if len(x) > 0 else -1 for x in patients_labels])
+            # Remove patients w/o labels
+            neg_mask = stratify == -1
+            stratify = stratify[~neg_mask]
+            patient_ids = patient_ids[~neg_mask]
+            num_neg = neg_mask.sum()
+            if num_neg > 0:
+                logger.warning(f"Removed {num_neg} patients w/ no target class")
+            # END IF
+        # END IF
 
-        # For each patient
-        for _, segment in patient_generator:
-            data = segment["data"][:]
-            blabels = segment["blabels"][:]
+        return sklearn.model_selection.train_test_split(
+            patient_ids,
+            test_size=test_size,
+            shuffle=True,
+            stratify=stratify,
+        )
 
-            # NOTE: Multiply by 5 to convert from 100 Hz to 500 Hz
-            blabels[:, 0] = blabels[:, 0] * 5
-            for _ in range(samples_per_patient):
-                # Select random lead and start index
-                lead = random.choice(self.leads)
-                frame_start = np.random.randint(0, data.shape[1] - input_size)
-                frame_end = frame_start + input_size
-                frame_blabels = blabels[(blabels[:, 0] >= frame_start) & (blabels[:, 0] < frame_end)]
-                x = data[lead, frame_start:frame_end].copy()
-                if self.sampling_rate != self.target_rate:
-                    ds_ratio = self.target_rate / self.sampling_rate
-                    x = pk.signal.resample_signal(x, self.sampling_rate, self.target_rate, axis=0)
-                else:
-                    ds_ratio = 1
-                # Create segment mask
-                mask = np.zeros_like(x, dtype=np.int32)
-
-                # # Check if pwave, twave, or uwave are in class_map- if so, add gradient filter to mask
-                # non_qrs = [self.class_map.get(k, -1) for k in (HKSegment.pwave, HKSegment.twave, HKSegment.uwave)]
-                # if any((v != -1 for v in non_qrs)):
-                #     xc = pk.ecg.clean(x.copy(), sample_rate=self.target_rate, lowcut=0.5, highcut=40, order=3)
-                #     grad = pk.signal.moving_gradient_filter(
-                #         xc, sample_rate=self.target_rate, sig_window=0.1, avg_window=1.0, sig_prom_weight=0.15
-                #     )
-                #     mask[grad > 0] = -1
-                # # END IF
-
-                for i in range(frame_blabels.shape[0]):
-                    bidx = int((frame_blabels[i, 0] - frame_start) * ds_ratio)
-                    # btype = frame_blabels[i, 1]
-
-                    # Extract QRS segment
-                    qrs = pk.signal.moving_gradient_filter(
-                        x, sample_rate=self.target_rate, sig_window=0.1, avg_window=1.0, sig_prom_weight=1.5
-                    )
-                    win_len = max(1, int(0.08 * self.target_rate))  # 80 ms
-                    b_left = max(0, bidx - win_len)
-                    b_right = min(x.shape[0], bidx + win_len)
-                    onset = np.where(np.flip(qrs[b_left:bidx]) < 0)[0]
-                    onset = onset[0] if onset.size else win_len
-                    offset = np.where(qrs[bidx + 1 : b_right] < 0)[0]
-                    offset = offset[0] if offset.size else win_len
-                    mask[bidx - onset : bidx + offset] = self.class_map.get(HKSegment.qrs.value, 0)
-                    # END IF
-                # END FOR
-                x = np.nan_to_num(x).astype(np.float32)
-                y = mask.astype(np.int32)
-                yield x, y
-            # END FOR
-        # END FOR
+    def filter_patients_for_labels(
+        self, patient_ids: npt.NDArray, label_map: dict[int, int] | None = None, label_type: str | None = None
+    ) -> npt.NDArray:
+        """Filter patients based on labels.
+        Useful to remove patients w/o labels for task to speed up data loading.
+
+        Args:
+            patient_ids (npt.NDArray): Patient ids
+            label_map (dict[int, int], optional): Label map. Defaults to None.
+            label_type (str, optional): Label type. Defaults to None.
+
+        Returns:
+            npt.NDArray: Filtered patient ids
+        """
+
+        if label_map is None or label_type is None:
+            return patient_ids
+
+        patients_labels = self.get_patients_labels(patient_ids, label_map, label_type)
+        # Find any patient with empty list
+        label_mask = np.array([len(x) > 0 for x in patients_labels])
+        neg_mask = label_mask == -1
+        num_neg = neg_mask.sum()
+        if num_neg > 0:
+            logger.warning(f"Removed {num_neg} of {patient_ids.size} patients w/ no target class")
+        return patient_ids[~neg_mask]
+
+    def get_patients_labels(
+        self, patient_ids: npt.NDArray, label_map: dict[int, int], label_type: str = "scp"
+    ) -> list[list[int]]:
+        """Get class labels for each patient
+
+        Args:
+            patient_ids (npt.NDArray): Patient ids
+            label_map (dict[int, int]): Label map
+            label_type (str, optional): Label type. Defaults to "scp".
+
+        Returns:
+            list[list[int]]: List of class labels per patient
+
+        """
+        ids = patient_ids.tolist()
+        func = functools.partial(self.get_patient_labels, label_map=label_map, label_type=label_type)
+        with Pool() as pool:
+            pts_labels = list(pool.imap(func, ids))
+        return pts_labels
+
+    def get_patient_scp_codes(self, patient_id: int) -> list[int]:
+        """Get SCP codes for patient
+
+        Args:
+            patient_id (int): Patient id
+
+        Returns:
+            list[int]: List of SCP codes
+
+        """
+        with self.patient_data(patient_id) as h5:
+            codes = h5[self.label_key("scp")][:, 0]
+        return np.unique(codes).tolist()
+
+    def get_patient_labels(self, patient_id: int, label_map: dict[int, int], label_type: str = "scp") -> list[int]:
+        """Get class labels for patient
+
+        Args:
+            patient_id (int): Patient id
+
+        Returns:
+            list[int]: List of class labels
+
+        """
+        with self.patient_data(patient_id) as h5:
+            labels = h5[self.label_key(label_type)][:, 0]
+        labels = np.unique(labels)
+        labels: list[int] = [label_map[r] for r in labels if label_map.get(r, -1) != -1]
+        return labels
 
     def download(self, num_workers: int | None = None, force: bool = False):
         """Download dataset
 
         This will download preprocessed HDF5 files from S3.
 
         Args:
             num_workers (int | None, optional): # parallel workers. Defaults to None.
             force (bool, optional): Force redownload. Defaults to False.
         """
-        self.download_raw_dataset(num_workers=num_workers, force=force)
+        download_s3_objects(
+            bucket="ambiq-ai-datasets",
+            prefix=self.ds_path.stem,
+            dst=self.ds_path.parent,
+            checksum="size",
+            progress=True,
+            num_workers=num_workers,
+        )
 
     def download_raw_dataset(self, num_workers: int | None = None, force: bool = False):
         """Downloads full dataset zipfile and converts into individial patient HDF5 files.
 
         Args:
             force (bool, optional): Whether to force re-download if destination exists. Defaults to False.
             num_workers (int, optional): # parallel workers. Defaults to os.cpu_count().
@@ -851,92 +731,7 @@
                 h5.create_dataset(name="/blabels", data=blabels)
                 h5.create_dataset(name="/slabels", data=slabels)
                 # Add patient info as attributes
                 for k, v in pt_info.items():
                     h5.attrs[k] = v
                 # END FOR
             # END WITH
-
-    def filter_patients_for_task(self, patient_ids: npt.NDArray) -> npt.NDArray:
-        """Filter patients based on task.
-        Useful to remove patients w/o labels for task to speed up data loading.
-
-        Args:
-            patient_ids (npt.NDArray): Patient ids
-
-        Returns:
-            npt.NDArray: Filtered patient ids
-        """
-        if self.task in ("rhythm", "diagnotic"):
-            label_mask = self._get_patient_labels(patient_ids)
-            neg_mask = label_mask == -1
-            num_neg = neg_mask.sum()
-            if num_neg > 0:
-                logger.warning(f"Removed {num_neg} of {patient_ids.size} patients w/ no target class")
-            return patient_ids[~neg_mask]
-        return patient_ids
-
-    def split_train_test_patients(self, patient_ids: npt.NDArray, test_size: float) -> list[list[int]]:
-        """Perform train/test split on patients for given task.
-        NOTE: We only perform inter-patient splits and not intra-patient.
-
-        Args:
-            patient_ids (npt.NDArray): Patient Ids
-            test_size (float): Test size
-
-        Returns:
-            list[list[int]]: Train and test sets of patient ids
-        """
-        stratify = None
-
-        # Use stratified split for rhythm task
-        if self.task in ("rhythm", "diagnostic"):
-            stratify = self._get_patient_labels(patient_ids)
-            neg_mask = stratify == -1
-            stratify = stratify[~neg_mask]
-            patient_ids = patient_ids[~neg_mask]
-            num_neg = neg_mask.sum()
-            if num_neg > 0:
-                logger.warning(f"Removed {num_neg} patients w/ no target class")
-
-        return sklearn.model_selection.train_test_split(
-            patient_ids,
-            test_size=test_size,
-            shuffle=True,
-            stratify=stratify,
-        )
-
-    def _get_patient_labels(self, patient_ids: npt.NDArray) -> npt.NDArray:
-        """Get scp labels for each patient
-
-        Args:
-            patient_ids (npt.NDArray): Patient ids
-
-        Returns:
-            npt.NDArray: Patient ids
-
-        """
-        ids = patient_ids.tolist()
-        with Pool() as pool:
-            pt_rhythms = list(pool.imap(self._get_patient_label, ids))
-        return np.array(pt_rhythms)
-
-    def _get_patient_label(self, patient_id: int) -> int:
-        """Get scp label for patient
-
-        Args:
-            patient_id (int): Patient id
-
-        Returns:
-            int: Target rhythm class
-        """
-        tgt_map = {k: self.class_map.get(v, -1) for (k, v) in PtbxlRhythmMap.items()}
-        pt_key = self._pt_key(patient_id)
-        with h5py.File(self.ds_path / f"{pt_key}.h5", mode="r") as h5:
-            pt_rhythms: npt.NDArray[np.int64] = np.array(h5["slabels"][:])
-        if pt_rhythms.size == 0:
-            return -1
-        pt_rhythms = pt_rhythms[:, 0]
-        pt_classes: list[int] = [tgt_map[r] for r in pt_rhythms if tgt_map.get(r, -1) != -1]
-        if len(pt_classes) == 0:
-            return -1
-        return random.choice(pt_classes)
```

### Comparing `heartkit-1.2.0/heartkit/datasets/synthetic.py` & `heartkit-1.3.0/heartkit/datasets/ludb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,95 @@
+import contextlib
+import functools
 import logging
 import os
 import random
+import tempfile
+import zipfile
+from enum import IntEnum
+from multiprocessing import Pool
+from pathlib import Path
+from typing import Generator
 
+import h5py
 import numpy as np
 import numpy.typing as npt
 import physiokit as pk
-import tensorflow as tf
-from pydantic import BaseModel, Field
+from tqdm import tqdm
 
-from ..tasks import HKSegment
+from ..utils import download_file
 from .dataset import HKDataset
-from .defines import PatientGenerator, SampleGenerator
-from .nstdb import NstdbNoise
+from .defines import PatientGenerator
+from .utils import download_s3_objects
 
 logger = logging.getLogger(__name__)
 
+LudbSymbolMap = {
+    "o": 0,  # Other
+    "p": 1,  # P Wave
+    "N": 2,  # QRS complex
+    "t": 3,  # T Wave
+}
+
+
+class LudbSegmentation(IntEnum):
+    """LUDB segmentation labels"""
+
+    normal = 0
+    pwave = 1
+    qrs = 2
+    twave = 3
+
+
+LudbLeadsMap = {
+    "i": 0,
+    "ii": 1,
+    "iii": 2,
+    "avr": 3,
+    "avl": 4,
+    "avf": 5,
+    "v1": 6,
+    "v2": 7,
+    "v3": 8,
+    "v4": 9,
+    "v5": 10,
+    "v6": 11,
+}
+
+FID_LEAD_IDX = 0
+FID_LBL_IDX = 1
+FID_LOC_IDX = 2
+SEG_LEAD_IDX = 0
+SEG_LBL_IDX = 1
+SEG_BEG_IDX = 2
+SEG_END_IDX = 3
 
-class SyntheticParams(BaseModel, extra="allow"):
-    """Synthetic parameters"""
 
-    presets: list[pk.ecg.EcgPreset] = Field(
-        default_factory=lambda: [
-            pk.ecg.EcgPreset.SR,
-            pk.ecg.EcgPreset.AFIB,
-            pk.ecg.EcgPreset.LAHB,
-            pk.ecg.EcgPreset.LPHB,
-            pk.ecg.EcgPreset.LBBB,
-            pk.ecg.EcgPreset.ant_STEMI,
-            pk.ecg.EcgPreset.random_morphology,
-            pk.ecg.EcgPreset.high_take_off,
-        ],
-        description="ECG presets",
-    )
-    preset_weights: list[int] = Field(
-        default_factory=lambda: [14, 1, 1, 1, 1, 1, 1, 1], description="ECG preset weights"
-    )
-    heart_rate: tuple[float, float] = Field((40, 120), description="Heart rate range")
-    impedance: tuple[float, float] = Field((1.0, 2.0), description="Impedance range")
-    p_multiplier: tuple[float, float] = Field((0.80, 1.2), description="P wave width multiplier range")
-    t_multiplier: tuple[float, float] = Field((0.80, 1.2), description="T wave width multiplier range")
-    noise_multiplier: tuple[float, float] = Field((0, 0), description="Noise multiplier range")
-    voltage_factor: tuple[float, float] = Field((800, 1000), description="Voltage factor range")
-
-
-class SyntheticDataset(HKDataset):
-    """Synthetic dataset"""
+class LudbDataset(HKDataset):
+    """LUDB dataset"""
 
     def __init__(
         self,
         ds_path: os.PathLike,
-        task: str,
-        frame_size: int,
-        target_rate: int,
-        spec: tuple[tf.TensorSpec, tf.TensorSpec],
-        class_map: dict[int, int] | None = None,
-        num_pts: int = 250,
-        noise_level: float = 0.0,
         leads: list[int] | None = None,
-        params: dict | None = None,
     ) -> None:
         super().__init__(
-            ds_path=ds_path / "synthetic",
-            task=task,
-            frame_size=frame_size,
-            target_rate=target_rate,
-            spec=spec,
-            class_map=class_map,
+            ds_path=ds_path,
         )
-        self._noise_gen = None
-        self._num_pts = num_pts
-        self.noise_level = noise_level
-        self.leads = leads or list(range(12))
-        self.params = SyntheticParams(**params or {})
+        self.leads = leads or list(LudbLeadsMap.values())
 
     @property
-    def cachable(self) -> bool:
-        """If dataset supports file caching."""
-        return True
+    def name(self) -> str:
+        """Dataset name"""
+        return "ludb"
 
     @property
     def sampling_rate(self) -> int:
         """Sampling rate in Hz"""
-        return self.target_rate
+        return 500
 
     @property
     def mean(self) -> float:
         """Dataset mean"""
         return 0
 
     @property
@@ -96,220 +100,236 @@
     @property
     def patient_ids(self) -> npt.NDArray:
         """Get dataset patient IDs
 
         Returns:
             npt.NDArray: patient IDs
         """
-        return np.arange(0, self._num_pts)
+        return np.arange(1, 201)
 
     def get_train_patient_ids(self) -> npt.NDArray:
         """Get dataset training patient IDs
 
         Returns:
             npt.NDArray: patient IDs
         """
-        numel = int(0.80 * self._num_pts)
-        return self.patient_ids[:numel]
+        return self.patient_ids[:180]
 
     def get_test_patient_ids(self) -> npt.NDArray:
         """Get dataset patient IDs reserved for testing only
 
         Returns:
             npt.NDArray: patient IDs
         """
-        numel = int(0.80 * self._num_pts)
-        return self.patient_ids[numel:]
+        return self.patient_ids[180:]
 
-    def task_data_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Task-level data generator.
+    def _pt_key(self, patient_id: int):
+        """Get patient key"""
+        return f"p{patient_id:05d}"
+
+    @contextlib.contextmanager
+    def patient_data(self, patient_id: int) -> Generator[h5py.Group, None, None]:
+        """Get patient data
 
         Args:
-            patient_generator (PatientGenerator): Patient data generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
+            patient_id (int): Patient ID
 
         Returns:
-            SampleGenerator: Sample data generator
+            Generator[h5py.Group, None, None]: Patient data
         """
-        if self.task == "segmentation":
-            return self.segmentation_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
-        if self.task == "denoise":
-            return self.denoising_generator(
-                patient_generator=patient_generator,
-                samples_per_patient=samples_per_patient,
-            )
-        raise NotImplementedError()
+        with h5py.File(self.ds_path / f"{self._pt_key(patient_id)}.h5", mode="r") as h5:
+            yield h5
 
-    def _synthesize_signal(self, signal_length: int) -> tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
-        """Generate synthetic signal of given length
+    def signal_generator(
+        self,
+        patient_generator: PatientGenerator,
+        frame_size: int,
+        samples_per_patient: int = 1,
+        target_rate: int | None = None,
+    ) -> Generator[npt.NDArray, None, None]:
+        """Generate random frames.
 
         Args:
-            signal_length (int): Signal length
+            patient_generator (PatientGenerator): Patient generator
+            frame_size (int): Frame size
+            samples_per_patient (int, optional): # samples per patient. Defaults to 1.
+            target_rate (int | None, optional): Target sampling rate. Defaults to None.
 
         Returns:
-            tuple[npt.NDArray, npt.NDArray, npt.NDArray]: signal, segments, fiducials
+            Generator[npt.NDArray, None, None]: Generator of input data of shape (frame_size, 1)
         """
-        heart_rate = np.random.uniform(self.params.heart_rate[0], self.params.heart_rate[1])
-        preset = random.choices(self.params.presets, self.params.preset_weights, k=1)[0].value
-        impedance = np.random.uniform(self.params.impedance[0], self.params.impedance[1])
-        p_multiplier = np.random.uniform(self.params.p_multiplier[0], self.params.p_multiplier[1])
-        t_multiplier = np.random.uniform(self.params.t_multiplier[0], self.params.t_multiplier[1])
-        voltage_factor = np.random.uniform(self.params.voltage_factor[0], self.params.voltage_factor[1])
-
-        ecg, segs, fids = pk.ecg.synthesize(
-            signal_length=signal_length,
-            sample_rate=self.sampling_rate,
-            leads=12,  # Use all 12 leads
-            heart_rate=heart_rate,
-            preset=preset,
-            impedance=impedance,
-            p_multiplier=p_multiplier,
-            t_multiplier=t_multiplier,
-            noise_multiplier=0,
-            voltage_factor=voltage_factor,
-        )
-        return ecg, segs, fids
 
-    def signal_generator(self, patient_generator: PatientGenerator, samples_per_patient: int = 1) -> SampleGenerator:
-        """Generate frames using patient generator.
+        if target_rate is None:
+            target_rate = self.sampling_rate
 
-        Args:
-            patient_generator (PatientGenerator): Generator that yields a tuple of patient id and patient data.
-            samples_per_patient (int): Samples per patient.
+        input_size = int(np.round((self.sampling_rate / target_rate) * frame_size))
 
-        Returns:
-            SampleGenerator: Generator of input data of shape (frame_size, 1)
-        """
-
-        signal_length = max(2 * self.frame_size, int(self.frame_size * samples_per_patient / len(self.leads)))
-        for _ in patient_generator:
-            syn_ecg, _, _ = self._synthesize_signal(signal_length)
+        for pt in patient_generator:
+            with self.patient_data(pt) as h5:
+                data: h5py.Dataset = h5["data"][:]
+            # END WITH
             for _ in range(samples_per_patient):
                 lead = random.choice(self.leads)
-                frame_start = np.random.randint(0, syn_ecg.shape[1] - self.frame_size)
-                frame_end = frame_start + self.frame_size
-                x = syn_ecg[lead, frame_start:frame_end].astype(np.float32).reshape((self.frame_size,))
-                x = self._add_noise(x)
+                start = np.random.randint(0, data.shape[0] - input_size)
+                x = data[start : start + input_size, lead].squeeze()
+                x = np.nan_to_num(x).astype(np.float32)
+                if self.sampling_rate != target_rate:
+                    x = pk.signal.resample_signal(x, self.sampling_rate, target_rate, axis=0)
+                # END IF
                 yield x
             # END FOR
         # END FOR
 
-    def segmentation_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Generate frames and segment labels.
+    def get_patient_data_segments(self, patient_id: int) -> tuple[npt.NDArray, npt.NDArray]:
+        """Get patient's entire data and segments
 
         Args:
-            patient_generator (PatientGenerator): Patient Generator
-            samples_per_patient (int | list[int], optional): # samples per patient. Defaults to 1.
+            patient (int): Patient ID (1-based)
 
         Returns:
-            SampleGenerator: Sample generator
+            tuple[npt.NDArray, npt.NDArray]: (data, segment labels)
+        """
+        with self.patient_data(patient_id) as pt:
+            data: npt.NDArray = pt["data"][:]
+            segs: npt.NDArray = pt["segmentations"][:]
+        labels = np.zeros_like(data)
+        for seg_idx in range(segs.shape[0]):  # pylint: disable=no-member
+            seg = segs[seg_idx]
+            labels[seg[SEG_BEG_IDX] : seg[SEG_END_IDX] + 0, seg[SEG_LEAD_IDX]] = seg[SEG_LBL_IDX]
+        # END FOR
+        return data, labels
+
+    def download(self, num_workers: int | None = None, force: bool = False):
+        """Download LUDB dataset
 
-        Yields:
-            Iterator[SampleGenerator]
+        Args:
+            num_workers (int | None, optional): # parallel workers. Defaults to None.
+            force (bool, optional): Force redownload. Defaults to False.
         """
-        start_offset = 0
-        signal_length = max(2 * self.frame_size, int(self.frame_size * samples_per_patient / len(self.leads)))
+        download_s3_objects(
+            bucket="ambiq-ai-datasets",
+            prefix=self.ds_path.stem,
+            dst=self.ds_path.parent,
+            checksum="size",
+            progress=True,
+            num_workers=num_workers,
+        )
 
-        for _ in patient_generator:
-            syn_ecg, syn_segs_t, _ = self._synthesize_signal(signal_length)
-            syn_segs = np.zeros_like(syn_segs_t)
-            for i in range(syn_segs_t.shape[0]):
-                syn_segs[i, np.where((syn_segs_t[i] == pk.ecg.EcgSegment.tp_overlap))[0]] = HKSegment.pwave
-                syn_segs[i, np.where((syn_segs_t[i] == pk.ecg.EcgSegment.p_wave))[0]] = HKSegment.pwave
-                syn_segs[i, np.where((syn_segs_t[i] == pk.ecg.EcgSegment.qrs_complex))[0]] = HKSegment.qrs
-                syn_segs[i, np.where((syn_segs_t[i] == pk.ecg.EcgSegment.t_wave))[0]] = HKSegment.twave
-            # END FOR
+    def download_raw_dataset(self, num_workers: int | None = None, force: bool = False):
+        """Downloads full dataset zipfile and converts into individial patient HDF5 files.
 
-            for i in range(samples_per_patient):
-                lead = random.choice(self.leads)
-                frame_start = np.random.randint(start_offset, syn_ecg.shape[1] - self.frame_size)
-                frame_end = frame_start + self.frame_size
-                x = syn_ecg[lead, frame_start:frame_end].astype(np.float32)
-                x = self._add_noise(x)
-                y = syn_segs[lead, frame_start:frame_end].astype(np.int32)
-                y = np.vectorize(self.class_map.get, otypes=[int])(y)
-                yield x, y
-            # END FOR
-        # END FOR
+        Args:
+            force (bool, optional): Whether to force re-download if destination exists. Defaults to False.
+            num_workers (int, optional): # parallel workers. Defaults to os.cpu_count().
+        """
+        logger.info("Downloading LUDB dataset")
+        ds_url = (
+            "https://physionet.org/static/published-projects/ludb/"
+            "lobachevsky-university-electrocardiography-database-1.0.1.zip"
+        )
+        ds_zip_path = self.ds_path / "ludb.zip"
+        os.makedirs(self.ds_path, exist_ok=True)
+        if os.path.exists(ds_zip_path) and not force:
+            logger.warning(
+                f"Zip file already exists. Please delete or set `force` flag to redownload. PATH={ds_zip_path}"
+            )
+        else:
+            download_file(ds_url, ds_zip_path, progress=True)
 
-    def denoising_generator(
-        self,
-        patient_generator: PatientGenerator,
-        samples_per_patient: int | list[int] = 1,
-    ) -> SampleGenerator:
-        """Generate frames and noise frames."""
-        signal_length = max(2 * self.frame_size, int(self.frame_size * samples_per_patient / len(self.leads)))
-        for _ in patient_generator:
-            syn_ecg, _, _ = self._synthesize_signal(signal_length)
-            for _ in range(samples_per_patient):
-                lead = random.choice(self.leads)
-                frame_start = np.random.randint(0, syn_ecg.shape[1] - self.frame_size)
-                frame_end = frame_start + self.frame_size
-                x = syn_ecg[lead, frame_start:frame_end].astype(np.float32).reshape((self.frame_size,))
-                y = x.copy()
-                x = self._add_noise(x)
-                yield x, y
-            # END FOR
-        # END FOR
+        # 2. Extract and convert patient ECG data to H5 files
+        logger.info("Generating LUDB patient data")
+        self.convert_dataset_zip_to_hdf5(zip_path=ds_zip_path, force=force, num_workers=num_workers)
+        logger.info("Finished LUDB patient data")
 
-    def uniform_patient_generator(
+    def convert_dataset_zip_to_hdf5(
         self,
-        patient_ids: npt.NDArray,
-        repeat: bool = True,
-        shuffle: bool = True,
-    ) -> PatientGenerator:
-        """Yield data for each patient in the array.
+        zip_path: os.PathLike,
+        patient_ids: npt.NDArray | None = None,
+        force: bool = False,
+        num_workers: int | None = None,
+    ):
+        """Convert dataset into individial patient HDF5 files.
 
         Args:
-            patient_ids (pt.ArrayLike): Array of patient ids
-            repeat (bool, optional): Whether to repeat generator. Defaults to True.
-            shuffle (bool, optional): Whether to shuffle patient ids.. Defaults to True.
-
-        Returns:
-            PatientGenerator: Patient generator
-
-        Yields:
-            Iterator[PatientGenerator]
+            zip_path (PathLike): Zip path
+            patient_ids (npt.NDArray | None, optional): List of patient IDs to extract. Defaults to all.
+            force (bool, optional): Whether to force re-download if destination exists. Defaults to False.
+            num_workers (int, optional): # parallel workers. Defaults to os.cpu_count().
         """
-        patient_ids = np.copy(patient_ids)
-        while True:
-            if shuffle:
-                np.random.shuffle(patient_ids)
-            for patient_id in patient_ids:
-                yield patient_id, None
-            # END FOR
-            if not repeat:
-                break
-        # END WHILE
+        if not patient_ids:
+            patient_ids = self.patient_ids
 
-    def download(self, num_workers: int | None = None, force: bool = False):
-        """Download dataset
+        subdir = "lobachevsky-university-electrocardiography-database-1.0.1"
+        with Pool(processes=num_workers) as pool, tempfile.TemporaryDirectory() as tmpdir, zipfile.ZipFile(
+            zip_path, mode="r"
+        ) as zp:
+            ludb_dir = Path(tmpdir, "ludb")
+            zp.extractall(ludb_dir)
+            f = functools.partial(
+                self.convert_pt_wfdb_to_hdf5,
+                src_path=ludb_dir / subdir / "data",
+                dst_path=self.ds_path,
+                force=force,
+            )
+            _ = list(tqdm(pool.imap(f, patient_ids), total=len(patient_ids)))
+        # END WITH
+
+    def convert_pt_wfdb_to_hdf5(
+        self, patient: int, src_path: os.PathLike, dst_path: os.PathLike, force: bool = False
+    ) -> tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
+        """Convert LUDB patient data from WFDB to more consumable HDF5 format.
 
         Args:
-            num_workers (int | None, optional): # parallel workers. Defaults to None.
-            force (bool, optional): Force redownload. Defaults to False.
+            patient (int): Patient id (1-based)
+            src_path (str): Source path to WFDB folder
+            dst_path (str): Destination path to store HDF5 file
+
+        Returns:
+            tuple[npt.NDArray, npt.NDArray, npt.NDArray]: data, segments, and fiducials
         """
-        # Nothing to do
+        import wfdb  # pylint: disable=import-outside-toplevel
 
-    def _add_noise(self, ecg: npt.NDArray):
-        """Add noise to ECG signal."""
-        noise_range = self.params.noise_multiplier
-        if noise_range[0] == 0 and noise_range[1] == 0:
-            return ecg
-        noise_level = np.random.uniform(noise_range[0], noise_range[1])
+        pt_id = f"p{patient:05d}"
+        pt_src_path = str(src_path / f"{patient}")
+        rec = wfdb.rdrecord(pt_src_path)
+        data = np.zeros_like(rec.p_signal)
+        segs = []
+        fids = []
+        for i, lead in enumerate(rec.sig_name):
+            lead_id = LudbLeadsMap.get(lead)
+            ann = wfdb.rdann(pt_src_path, extension=lead)
+            seg_start = seg_stop = sym_id = None
+            data[:, lead_id] = rec.p_signal[:, i]
+            for j, symbol in enumerate(ann.symbol):
+                # Start of segment
+                if symbol == "(":
+                    seg_start = ann.sample[j]
+                    seg_stop = None
+                # Fiducial / segment type
+                elif symbol in LudbSymbolMap:
+                    sym_id = LudbSymbolMap.get(symbol)
+                    if seg_start is None:
+                        seg_start = ann.sample[j]
+                    fids.append([lead_id, sym_id, ann.sample[j]])
+                # End of segment (start and symbol are never 0 but can be None)
+                elif symbol == ")" and seg_start and sym_id:
+                    seg_stop = ann.sample[j]
+                    segs.append([lead_id, sym_id, seg_start, seg_stop])
+                else:
+                    seg_start = seg_stop = None
+                    sym_id = None
+            # END FOR
+        # END FOR
+        segs = np.array(segs)
+        fids = np.array(fids)
 
-        if self._noise_gen is None:
-            self._noise_gen = NstdbNoise(ds_path=self.ds_path.parent, target_rate=self.target_rate)
+        if dst_path:
+            os.makedirs(dst_path, exist_ok=True)
+            pt_dst_path = dst_path / f"{pt_id}.h5"
+            with h5py.File(pt_dst_path, "w") as h5:
+                h5.create_dataset("data", data=data, compression="gzip")
+                h5.create_dataset("segmentations", data=segs, compression="gzip")
+                h5.create_dataset("fiducials", data=fids, compression="gzip")
+            # END WITH
         # END IF
-        self._noise_gen.apply_noise(ecg, noise_level)
-        return ecg
+
+        return data, segs, fids
```

### Comparing `heartkit-1.2.0/heartkit/defines.py` & `heartkit-1.3.0/heartkit/defines.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     params: dict[str, tuple[float | int, float | int]]
 
 
 class DatasetParams(BaseModel, extra="allow"):
     """Dataset parameters"""
 
     name: str
+    path: Path = Field(default_factory=Path, description="Dataset path")
     params: dict[str, Any] = Field(default_factory=dict, description="Parameters")
     weight: float = Field(1, description="Dataset weight")
 
 
 class HKMode(StrEnum):
     """HeartKit Mode"""
 
@@ -56,44 +57,46 @@
     export = "export"
     demo = "demo"
 
 
 class HKDownloadParams(BaseModel, extra="allow"):
     """Download command params"""
 
-    job_dir: Path = Field(default_factory=tempfile.gettempdir, description="Job output directory")
-    ds_path: Path = Field(default_factory=Path, description="Dataset root directory")
-    datasets: list[str] = Field(default_factory=list, description="Datasets")
+    job_dir: Path = Field(default_factory=lambda: Path(tempfile.gettempdir()), description="Job output directory")
+    datasets: list[DatasetParams] = Field(default_factory=list, description="Datasets")
     progress: bool = Field(True, description="Display progress bar")
     force: bool = Field(False, description="Force download dataset- overriding existing files")
     data_parallelism: int = Field(
         default_factory=lambda: os.cpu_count() or 1,
         description="# of data loaders running in parallel",
     )
 
 
 class HKTrainParams(BaseModel, extra="allow"):
     """Train command params"""
 
     name: str = Field("experiment", description="Experiment name")
+    project: str = Field("heartkit", description="Project name")
     job_dir: Path = Field(default_factory=lambda: Path(tempfile.gettempdir()), description="Job output directory")
     # Dataset arguments
-    ds_path: Path = Field(default_factory=lambda: Path("./datasets"), description="Dataset directory")
     datasets: list[DatasetParams] = Field(default_factory=list, description="Datasets")
+
     sampling_rate: int = Field(250, description="Target sampling rate (Hz)")
     frame_size: int = Field(1250, description="Frame size")
     num_classes: int = Field(1, description="# of classes")
     class_map: dict[int, int] = Field(default_factory=lambda: {1: 1}, description="Class/label mapping")
     class_names: list[str] | None = Field(default=None, description="Class names")
+
     samples_per_patient: int | list[int] = Field(1000, description="# train samples per patient")
     val_samples_per_patient: int | list[int] = Field(1000, description="# validation samples per patient")
     train_patients: float | None = Field(None, description="# or proportion of patients for training")
     val_patients: float | None = Field(None, description="# or proportion of patients for validation")
     val_file: Path | None = Field(None, description="Path to load/store pickled validation file")
     val_size: int | None = Field(None, description="# samples for validation")
+
     # Model arguments
     resume: bool = Field(False, description="Resume training")
     architecture: ModelArchitecture | None = Field(default=None, description="Custom model architecture")
     model_file: Path | None = Field(None, description="Path to save model file (.keras)")
     threshold: float | None = Field(None, description="Model output threshold")
 
     weights_file: Path | None = Field(None, description="Path to a checkpoint weights to load")
@@ -132,17 +135,18 @@
         if self.weights_file and len(self.weights_file.parts) == 1:
             self.weights_file = self.job_dir / self.weights_file
 
 
 class HKTestParams(BaseModel, extra="allow"):
     """Test command params"""
 
+    name: str = Field("experiment", description="Experiment name")
+    project: str = Field("heartkit", description="Project name")
     job_dir: Path = Field(default_factory=lambda: Path(tempfile.gettempdir()), description="Job output directory")
     # Dataset arguments
-    ds_path: Path = Field(default_factory=lambda: Path("./datasets"), description="Dataset directory")
     datasets: list[DatasetParams] = Field(default_factory=list, description="Datasets")
     sampling_rate: int = Field(250, description="Target sampling rate (Hz)")
     frame_size: int = Field(1250, description="Frame size")
     num_classes: int = Field(1, description="# of classes")
     class_map: dict[int, int] = Field(default_factory=lambda: {1: 1}, description="Class/label mapping")
     class_names: list[str] | None = Field(default=None, description="Class names")
     test_samples_per_patient: int | list[int] = Field(1000, description="# test samples per patient")
@@ -171,17 +175,18 @@
         if self.model_file and len(self.model_file.parts) == 1:
             self.model_file = self.job_dir / self.model_file
 
 
 class HKExportParams(BaseModel, extra="allow"):
     """Export command params"""
 
+    name: str = Field("experiment", description="Experiment name")
+    project: str = Field("heartkit", description="Project name")
     job_dir: Path = Field(default_factory=lambda: Path(tempfile.gettempdir()), description="Job output directory")
     # Dataset arguments
-    ds_path: Path = Field(default_factory=lambda: Path("./datasets"), description="Dataset directory")
     datasets: list[DatasetParams] = Field(default_factory=list, description="Datasets")
     sampling_rate: int = Field(250, description="Target sampling rate (Hz)")
     frame_size: int = Field(1250, description="Frame size")
     num_classes: int = Field(3, description="# of classes")
     class_map: dict[int, int] = Field(default_factory=lambda: {1: 1}, description="Class/label mapping")
     class_names: list[str] | None = Field(default=None, description="Class names")
     test_samples_per_patient: int | list[int] = Field(100, description="# test samples per patient")
@@ -215,28 +220,30 @@
         if self.tflm_file and len(self.tflm_file.parts) == 1:
             self.tflm_file = self.job_dir / self.tflm_file
 
 
 class HKDemoParams(BaseModel, extra="allow"):
     """HK demo command params"""
 
+    name: str = Field("experiment", description="Experiment name")
+    project: str = Field("heartkit", description="Project name")
     job_dir: Path = Field(default_factory=lambda: Path(tempfile.gettempdir()), description="Job output directory")
     # Dataset arguments
-    ds_path: Path = Field(default_factory=lambda: Path("./datasets"), description="Dataset directory")
     datasets: list[DatasetParams] = Field(default_factory=list, description="Datasets")
     sampling_rate: int = Field(250, description="Target sampling rate (Hz)")
     frame_size: int = Field(1250, description="Frame size")
     num_classes: int = Field(1, description="# of classes")
     class_map: dict[int, int] = Field(default_factory=lambda: {1: 1}, description="Class/label mapping")
     class_names: list[str] | None = Field(default=None, description="Class names")
     preprocesses: list[PreprocessParams] = Field(default_factory=list, description="Preprocesses")
     augmentations: list[AugmentationParams] = Field(default_factory=list, description="Augmentations")
     # Model arguments
     model_file: Path | None = Field(None, description="Path to save model file (.keras)")
     backend: str = Field("pc", description="Backend")
+    # Demo arguments
     demo_size: int | None = Field(1000, description="# samples for demo")
     display_report: bool = Field(True, description="Display report")
     # Extra arguments
     seed: int | None = Field(None, description="Random state seed")
     model_config = ConfigDict(protected_namespaces=())
 
     def model_post_init(self, __context: Any) -> None:
```

### Comparing `heartkit-1.2.0/heartkit/metrics.py` & `heartkit-1.3.0/heartkit/metrics.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/__init__.py` & `heartkit-1.3.0/heartkit/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from .defines import MBConvParams
 from .efficientnet import EfficientNetParams, EfficientNetV2, efficientnetv2_from_object
 from .factory import ModelFactory
 from .mobileone import MobileOne, MobileOneU0, mobileone_from_object
 from .multiresnet import MultiresNet, MultiresNetParams, multiresnet_from_object
 from .resnet import ResNet, ResNetBlockParams, ResNetParams, resnet_from_object
+from .sequentialnet import (
+    SequentialLayerParams,
+    SequentialNetwork,
+    SequentialNetworkParams,
+    sequentialnet_from_object,
+)
 from .tcn import Tcn, TcnBlockParams, TcnParams, tcn_from_object
 from .tsmixer import TsBlockParams, TsMixer, TsMixerParams, tsmixer_from_object
 from .unet import UNet, UNetBlockParams, UNetParams, unet_from_object
 from .unext import UNext, UNextBlockParams, UNextParams, unext_from_object
 
 ModelFactory.register("unet", unet_from_object)
 ModelFactory.register("unext", unext_from_object)
 ModelFactory.register("resnet", resnet_from_object)
 ModelFactory.register("multiresnet", multiresnet_from_object)
 ModelFactory.register("efficientnetv2", efficientnetv2_from_object)
 ModelFactory.register("mobileone", mobileone_from_object)
 ModelFactory.register("tsmixer", tsmixer_from_object)
 ModelFactory.register("tcn", tcn_from_object)
+ModelFactory.register("sequentialnet", sequentialnet_from_object)
```

### Comparing `heartkit-1.2.0/heartkit/models/blocks.py` & `heartkit-1.3.0/heartkit/models/blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,43 @@
 
 def batch_norm(name: str | None = None, momentum=0.9, epsilon=1e-3) -> KerasLayer:
     """Batch normalization layer"""
     name = name + ".bn" if name else None
     return keras.layers.BatchNormalization(momentum=momentum, epsilon=epsilon, name=name)
 
 
+def norm_layer(norm: str, name: str) -> KerasLayer:
+    """Normalization layer
+
+    Args:
+        norm (str): Normalization type
+        name (str): Name
+
+    Returns:
+        KerasLayer: Layer
+    """
+
+    def layer(x: tf.Tensor) -> tf.Tensor:
+        """Functional normalization layer
+
+        Args:
+            x (tf.Tensor): Input tensor
+
+        Returns:
+            tf.Tensor: Output tensor
+        """
+        if norm == "batch":
+            return batch_norm(name=name)(x)
+        if norm == "layer":
+            return layer_norm(name=name)(x)
+        return x
+
+    return layer
+
+
 def glu(dim: int = -1) -> KerasLayer:
     """Gated linear unit layer"""
 
     def layer(x: tf.Tensor) -> tf.Tensor:
         out, gate = tf.split(x, num_or_size_splits=2, axis=dim)
         gate = tf.sigmoid(gate)
         x = tf.multiply(out, gate)
@@ -161,14 +190,15 @@
 def mbconv_block(
     output_filters: int,
     expand_ratio: float = 1,
     kernel_size: int | tuple[int, int] = 3,
     strides: int | tuple[int, int] = 1,
     se_ratio: float = 8,
     droprate: float = 0,
+    norm: str = "batch",
     name: str | None = None,
 ) -> KerasLayer:
     """MBConv block w/ expansion and SE
 
     Args:
         output_filters (int): # output filter channels
         expand_ratio (float, optional): Expansion ratio. Defaults to 1.
@@ -189,15 +219,15 @@
         add_residual = input_filters == output_filters and not is_downsample
 
         # Expand: narrow -> wide
         if expand_ratio != 1:
             name_ex = f"{name}.exp" if name else None
             filters = int(input_filters * expand_ratio)
             y = conv2d(filters, kernel_size=(1, 1), strides=(1, 1), name=name_ex)(x)
-            y = batch_norm(name=name_ex)(y)
+            y = norm_layer(norm, name=name_ex)(y)
             y = relu6(name=name_ex)(y)
         else:
             y = x
 
         # Apply: wide -> wide
         # NOTE: DepthwiseConv2D only supports equal size stride -> use maxpooling instead
         name_dp = f"{name}.dp" if name else None
@@ -205,15 +235,15 @@
             kernel_size=kernel_size,
             strides=(1, 1),
             padding="same",
             use_bias=False,
             depthwise_initializer="he_normal",
             name=name_dp,
         )(y)
-        y = batch_norm(name=name_dp)(y)
+        y = norm_layer(norm, name=name_dp)(y)
         y = relu6(name=name_dp)(y)
         if is_downsample:
             y = keras.layers.MaxPool2D(pool_size=strides, padding="same")(y)
 
         # SE: wide -> wide
         if se_ratio:
             name_se = f"{name}.se" if name else None
@@ -224,15 +254,15 @@
         y = conv2d(
             output_filters,
             kernel_size=(1, 1),
             strides=(1, 1),
             padding="same",
             name=name_red,
         )(y)
-        y = batch_norm(name=name_red)(y)
+        y = norm_layer(norm, name=name_red)(y)
         # No activation
 
         if add_residual:
             name_res = f"{name}.res" if name else None
             if droprate > 0:
                 y = keras.layers.Dropout(droprate, noise_shape=(None, 1, 1, 1))(y)
             y = keras.layers.add([x, y], name=name_res)
```

### Comparing `heartkit-1.2.0/heartkit/models/callbacks.py` & `heartkit-1.3.0/heartkit/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/defines.py` & `heartkit-1.3.0/heartkit/models/defines.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Literal
 
 import tensorflow as tf
 from pydantic import BaseModel, Field
 
 KerasLayer = Callable[[tf.Tensor], tf.Tensor]
 
 
@@ -12,7 +12,8 @@
     filters: int = Field(..., description="# filters")
     depth: int = Field(default=1, description="Layer depth")
     ex_ratio: float = Field(default=1, description="Expansion ratio")
     kernel_size: int | tuple[int, int] = Field(default=3, description="Kernel size")
     strides: int | tuple[int, int] = Field(default=1, description="Stride size")
     se_ratio: float = Field(default=8, description="Squeeze Excite ratio")
     droprate: float = Field(default=0, description="Drop rate")
+    norm: Literal["batch", "layer"] | None = Field(default="layer", description="Normalization type")
```

### Comparing `heartkit-1.2.0/heartkit/models/efficientnet.py` & `heartkit-1.3.0/heartkit/models/efficientnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """ EfficientNet https://arxiv.org/abs/2104.00298"""
 
+from typing import Literal
+
 import keras
 import tensorflow as tf
 from pydantic import BaseModel, Field
 
-from .blocks import batch_norm, conv2d, mbconv_block, relu6
+from .blocks import conv2d, mbconv_block, norm_layer, relu6
 from .defines import KerasLayer, MBConvParams
 from .utils import make_divisible
 
 
 class EfficientNetParams(BaseModel):
     """EfficientNet parameters"""
 
@@ -19,14 +21,15 @@
     output_filters: int = Field(default=0, description="Output filters")
     output_activation: str | None = Field(default=None, description="Output activation")
     include_top: bool = Field(default=True, description="Include top")
     dropout: float = Field(default=0, description="Dropout rate")
     drop_connect_rate: float = Field(default=0, description="Drop connect rate")
     use_logits: bool = Field(default=True, description="Use logits")
     activation: str = Field(default="relu6", description="Activation function")
+    norm: Literal["batch", "layer"] | None = Field(default="layer", description="Normalization type")
     model_name: str = Field(default="EfficientNetV2", description="Model name")
 
 
 def efficientnet_core(blocks: list[MBConvParams], drop_connect_rate: float = 0) -> KerasLayer:
     """EfficientNet core
 
     Args:
@@ -48,14 +51,15 @@
                 x = mbconv_block(
                     filters,
                     block.ex_ratio,
                     block.kernel_size,
                     block.strides if d == 0 else 1,
                     block.se_ratio,
                     droprate=block_drop_rate,
+                    norm=block.norm,
                     name=name,
                 )(x)
                 global_block_id += 1
             # END FOR
         # END FOR
         return x
 
@@ -93,45 +97,48 @@
         filters = make_divisible(params.input_filters, 8)
         y = conv2d(
             filters,
             kernel_size=params.input_kernel_size,
             strides=params.input_strides,
             name=name,
         )(y)
-        y = batch_norm(name=name)(y)
+        y = norm_layer(params.norm, name)(y)
         y = relu6(name=name)(y)
     # END IF
 
     y = efficientnet_core(blocks=params.blocks, drop_connect_rate=params.drop_connect_rate)(y)
 
     if params.output_filters:
         name = "neck"
         filters = make_divisible(params.output_filters, 8)
         y = conv2d(filters, kernel_size=(1, 1), strides=(1, 1), padding="same", name=name)(y)
-        y = batch_norm(name=name)(y)
+        y = norm_layer(params.norm, name)(y)
         y = relu6(name=name)(y)
 
     if params.include_top:
         name = "top"
         y = keras.layers.GlobalAveragePooling2D(name=f"{name}.pool")(y)
         if 0 < params.dropout < 1:
             y = keras.layers.Dropout(params.dropout)(y)
-        y = keras.layers.Dense(num_classes, name=name)(y)
+        if num_classes is not None:
+            y = keras.layers.Dense(num_classes, name=name)(y)
+
         if params.output_activation:
             y = keras.layers.Activation(params.output_activation)(y)
-        # if not params.use_logits:
-        #     y = keras.layers.Softmax()(y)
+        elif not params.use_logits:
+            y = keras.layers.Softmax()(y)
+
     model = keras.Model(x, y, name=params.model_name)
     return model
 
 
 def efficientnetv2_from_object(
     x: tf.Tensor,
     params: dict,
-    num_classes: int,
+    num_classes: int | None = None,
 ) -> keras.Model:
     """Create model from object
 
     Args:
         x (tf.Tensor): Input tensor
         params (dict): Model parameters.
         num_classes (int, optional): # classes.
```

### Comparing `heartkit-1.2.0/heartkit/models/factory.py` & `heartkit-1.3.0/heartkit/models/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         Args:
             name (str): model name
         """
         _models.pop(name, None)
 
     @staticmethod
-    def create(name: str, params: dict, inputs: tf.Tensor, num_classes: int) -> keras.models.Model:
+    def create(name: str, params: dict, inputs: tf.Tensor, num_classes: int | None = None) -> keras.models.Model:
         """Create a model
 
         Args:
             name (str): model name
             params (dict): model parameters
             inputs (tf.Tensor): input tensor
             num_classes (int): number of classes
```

### Comparing `heartkit-1.2.0/heartkit/models/mobileone.py` & `heartkit-1.3.0/heartkit/models/mobileone.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/multiresnet.py` & `heartkit-1.3.0/heartkit/models/multiresnet.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/resnet.py` & `heartkit-1.3.0/heartkit/models/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     model = keras.Model(x, y, name="model")
     return model
 
 
 def resnet_from_object(
     x: tf.Tensor,
     params: dict,
-    num_classes: int,
+    num_classes: int | None = None,
 ) -> keras.Model:
     """Create model from object
 
     Args:
         x (tf.Tensor): Input tensor
         params (dict): Model parameters.
         num_classes (int, optional): # classes.
```

### Comparing `heartkit-1.2.0/heartkit/models/tcn.py` & `heartkit-1.3.0/heartkit/models/tcn.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
     model = keras.Model(x, y, name=params.model_name)
     return model
 
 
 def tcn_from_object(
     x: tf.Tensor,
     params: dict,
-    num_classes: int,
+    num_classes: int | None = None,
 ) -> keras.Model:
     """Create model from object
 
     Args:
         x (tf.Tensor): Input tensor
         params (dict): Model parameters.
         num_classes (int, optional): # classes.
```

### Comparing `heartkit-1.2.0/heartkit/models/tsmixer.py` & `heartkit-1.3.0/heartkit/models/tsmixer.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/unet.py` & `heartkit-1.3.0/heartkit/models/unet.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/unext.py` & `heartkit-1.3.0/heartkit/models/unext.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/models/utils.py` & `heartkit-1.3.0/heartkit/models/utils.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/__init__.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/__init__.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/client.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/client.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/common.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/common.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/interface.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/interface.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_EvbToPc/server.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_EvbToPc/server.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/__init__.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/__init__.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/client.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/client.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/common.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/common.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/interface.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/interface.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/GenericDataOperations_PcToEvb/server.py` & `heartkit-1.3.0/heartkit/rpc/GenericDataOperations_PcToEvb/server.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/backends.py` & `heartkit-1.3.0/heartkit/rpc/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,13 +187,13 @@
         self._model = None
 
     def set_inputs(self, inputs: npt.NDArray):
         self._inputs = inputs
 
     def perform_inference(self):
         if self._is_tf_model():
-            self._outputs = self._model.predict(np.expand_dims(self._inputs, 0)).squeeze(0)
+            self._outputs = self._model.predict(np.expand_dims(self._inputs, 0), verbose=0).squeeze(0)
         else:
             self._outputs = tflite.predict_tflite(self._model, self._inputs)
 
     def get_outputs(self) -> npt.NDArray:
         return self._outputs
```

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/__init__.py` & `heartkit-1.3.0/heartkit/rpc/erpc/__init__.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/arbitrator.py` & `heartkit-1.3.0/heartkit/rpc/erpc/arbitrator.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/basic_codec.py` & `heartkit-1.3.0/heartkit/rpc/erpc/basic_codec.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/client.py` & `heartkit-1.3.0/heartkit/rpc/erpc/client.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/codec.py` & `heartkit-1.3.0/heartkit/rpc/erpc/codec.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/crc16.py` & `heartkit-1.3.0/heartkit/rpc/erpc/crc16.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/server.py` & `heartkit-1.3.0/heartkit/rpc/erpc/server.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/simple_server.py` & `heartkit-1.3.0/heartkit/rpc/erpc/simple_server.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/erpc/transport.py` & `heartkit-1.3.0/heartkit/rpc/erpc/transport.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/factory.py` & `heartkit-1.3.0/heartkit/rpc/factory.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/rpc/utils.py` & `heartkit-1.3.0/heartkit/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/tasks/__init__.py` & `heartkit-1.3.0/heartkit/tasks/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from .beat import BeatTask, HKBeat
 from .denoise import DenoiseTask
 from .diagnostic import DiagnosticTask, HKDiagnostic
 from .factory import TaskFactory
-from .rhythm import HeartRate, HKRhythm, RhythmTask
+from .foundation import FoundationTask
+from .rhythm import HKRhythm, RhythmTask
 from .segmentation import HKSegment, SegmentationTask
 from .task import HKTask
+from .utils import load_datasets
 
 TaskFactory.register("rhythm", RhythmTask)
 TaskFactory.register("beat", BeatTask)
 TaskFactory.register("segmentation", SegmentationTask)
 TaskFactory.register("diagnostic", DiagnosticTask)
 TaskFactory.register("denoise", DenoiseTask)
+TaskFactory.register("foundation", FoundationTask)
```

### Comparing `heartkit-1.2.0/heartkit/tasks/beat/utils.py` & `heartkit-1.3.0/heartkit/datasets/synthetic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,308 +1,258 @@
-from pathlib import Path
+import contextlib
+import io
+import logging
+import os
+import random
+import uuid
+from typing import Generator
 
-import keras
+import h5py
 import numpy as np
 import numpy.typing as npt
-import tensorflow as tf
-from rich.console import Console
+import physiokit as pk
+from pydantic import BaseModel, Field
 
-from ...datasets import DatasetFactory, HKDataset, augment_pipeline, preprocess_pipeline
-from ...defines import (
-    DatasetParams,
-    HKExportParams,
-    HKTestParams,
-    HKTrainParams,
-    ModelArchitecture,
-    PreprocessParams,
-)
-from ...models import EfficientNetParams, EfficientNetV2, MBConvParams, ModelFactory
-
-console = Console()
-
-
-def get_feat_shape(frame_size: int) -> tuple[int, ...]:
-    """Get dataset feature shape.
-
-    Args:
-        frame_size (int): Frame size
-
-    Returns:
-        tuple[int, ...]: Feature shape
-    """
-    return (frame_size, 1)  # Time x Channels
-
-
-def get_class_shape(frame_size: int, nclasses: int) -> tuple[int, ...]:
-    """Get dataset class shape.
-
-    Args:
-        frame_size (int): Frame size
-        nclasses (int): Number of classes
-
-    Returns:
-        tuple[int, ...]: Class shape
-
-    """
-    return (nclasses,)  # One-hot encoded classes
-
-
-def prepare(x: npt.NDArray, sample_rate: float, preprocesses: list[PreprocessParams]) -> npt.NDArray:
-    """Prepare dataset.
-
-    Args:
-        x (npt.NDArray): Input signal
-        sample_rate (float): Sampling rate
-        preprocesses (list[PreprocessParams]): Preprocessing pipeline
-
-    Returns:
-        npt.NDArray: Prepared signal
-    """
-    if not preprocesses:
-        preprocesses = [
-            dict(name="filter", args=dict(axis=0, lowcut=0.5, highcut=30, order=3, sample_rate=sample_rate)),
-            dict(name="znorm", args=dict(axis=None, eps=0.1)),
-        ]
-    return preprocess_pipeline(x, preprocesses=preprocesses, sample_rate=sample_rate)
-
-
-def load_datasets(
-    ds_path: Path,
-    frame_size: int,
-    sampling_rate: int,
-    class_map: dict[int, int] | None,
-    spec: tuple[tf.TensorSpec, tf.TensorSpec],
-    datasets: list[DatasetParams] = None,
-) -> list[HKDataset]:
-    """Load datasets
-
-    Args:
-        ds_path (Path): Path to dataset
-        frame_size (int): Frame size
-        sampling_rate (int): Sampling rate
-        spec (tuple[tf.TensorSpec, tf.TensorSpec]): feat/class shape specs
-        class_map (dict[int, int]): Class map
-        datasets (list[DatasetParams]): List of datasets
-
-    Returns:
-        HeartKitDataset: Dataset
-    """
-    dsets = []
-    for dset in datasets:
-        if DatasetFactory.has(dset.name):
-            dsets.append(
-                DatasetFactory.get(dset.name)(
-                    ds_path=ds_path,
-                    task="beat",
-                    frame_size=frame_size,
-                    target_rate=sampling_rate,
-                    class_map=class_map,
-                    spec=spec,
-                    **dset.params
-                )
+from .dataset import HKDataset
+from .defines import PatientGenerator
+from .nstdb import NstdbNoise
+
+logger = logging.getLogger(__name__)
+
+
+class SyntheticParams(BaseModel, extra="allow"):
+    """Synthetic parameters"""
+
+    presets: list[pk.ecg.EcgPreset] = Field(
+        default_factory=lambda: [
+            pk.ecg.EcgPreset.SR,
+            pk.ecg.EcgPreset.AFIB,
+            pk.ecg.EcgPreset.LAHB,
+            pk.ecg.EcgPreset.LPHB,
+            pk.ecg.EcgPreset.LBBB,
+            pk.ecg.EcgPreset.ant_STEMI,
+            pk.ecg.EcgPreset.random_morphology,
+            pk.ecg.EcgPreset.high_take_off,
+        ],
+        description="ECG presets",
+    )
+    preset_weights: list[int] = Field(
+        default_factory=lambda: [14, 1, 1, 1, 1, 1, 1, 1], description="ECG preset weights"
+    )
+    sample_rate: float = Field(500, description="Signal sample rate (Hz)")
+    duration: int = Field(10, description="Signal duration in sec")
+    heart_rate: tuple[float, float] = Field((40, 120), description="Heart rate range")
+    impedance: tuple[float, float] = Field((1.0, 2.0), description="Impedance range")
+    p_multiplier: tuple[float, float] = Field((0.80, 1.2), description="P wave width multiplier range")
+    t_multiplier: tuple[float, float] = Field((0.80, 1.2), description="T wave width multiplier range")
+    noise_multiplier: tuple[float, float] = Field((0, 0), description="Noise multiplier range")
+    voltage_factor: tuple[float, float] = Field((800, 1000), description="Voltage factor range")
+
+
+class SyntheticDataset(HKDataset):
+    """Synthetic dataset"""
+
+    def __init__(
+        self,
+        ds_path: os.PathLike,
+        num_pts: int = 250,
+        leads: list[int] | None = None,
+        params: dict | None = None,
+    ) -> None:
+        super().__init__(
+            ds_path=ds_path,
+        )
+        self._noise_gen = None
+        self._num_pts = num_pts
+        self.leads = leads or list(range(12))
+        self.params = SyntheticParams(**params or {})
+        self._unique_id = str(uuid.uuid4())
+        self._cache: dict[str, io.BytesIO] = {}
+        os.makedirs(self.ds_path, exist_ok=True)
+
+    @property
+    def name(self) -> str:
+        """Dataset name"""
+        return "synthetic"
+
+    @property
+    def cachable(self) -> bool:
+        """If dataset supports file caching."""
+        return True
+
+    @property
+    def sampling_rate(self) -> int:
+        """Sampling rate in Hz"""
+        return self.params.sample_rate
+
+    @property
+    def mean(self) -> float:
+        """Dataset mean"""
+        return 0
+
+    @property
+    def std(self) -> float:
+        """Dataset st dev"""
+        return 1
+
+    @property
+    def patient_ids(self) -> npt.NDArray:
+        """Get dataset patient IDs
+
+        Returns:
+            npt.NDArray: patient IDs
+        """
+        return np.arange(0, self._num_pts)
+
+    def get_train_patient_ids(self) -> npt.NDArray:
+        """Get dataset training patient IDs
+
+        Returns:
+            npt.NDArray: patient IDs
+        """
+        numel = int(0.80 * self._num_pts)
+        return self.patient_ids[:numel]
+
+    def get_test_patient_ids(self) -> npt.NDArray:
+        """Get dataset patient IDs reserved for testing only
+
+        Returns:
+            npt.NDArray: patient IDs
+        """
+        numel = int(0.80 * self._num_pts)
+        return self.patient_ids[numel:]
+
+    def pt_key(self, patient_id: int):
+        """Get patient key"""
+        return f"{patient_id:05d}"
+
+    @contextlib.contextmanager
+    def patient_data(self, patient_id: int) -> Generator[h5py.Group, None, None]:
+        """Get patient data
+
+        Args:
+            patient_id (int): Patient ID
+
+        Returns:
+            Generator[h5py.Group, None, None]: Patient data
+        """
+
+        pt_key = self.pt_key(patient_id)
+        if pt_key not in self._cache:
+            ecg, segs, fids = self._synthesize_signal(
+                frame_size=int(self.params.duration * self.sampling_rate), target_rate=self.sampling_rate
             )
+            fp = io.BytesIO()
+            with h5py.File(fp, mode="w") as h5:
+                h5.create_dataset("data", data=ecg)
+                h5.create_dataset("segmentations", data=segs)
+                h5.create_dataset("fiducials", data=fids)
+                h5.attrs["unique_id"] = self._unique_id
+            # END WITH
+            fp.seek(0)
+            self._cache[pt_key] = fp
         # END IF
-    # END FOR
-    return dsets
 
-
-def load_train_datasets(
-    datasets: list[HKDataset],
-    params: HKTrainParams,
-) -> tuple[tf.data.Dataset, tf.data.Dataset]:
-    """Load beat train datasets.
-
-    Args:
-        datasets (list[HeartKitDataset]): Datasets
-        params (HKTrainParams): Train params
-
-    Returns:
-        tuple[tf.data.Dataset, tf.data.Dataset]: Train and validation datasets
-    """
-
-    feat_shape = get_feat_shape(params.frame_size)
-
-    def preprocess(x_y: tuple[npt.NDArray, npt.NDArray]) -> tuple[npt.NDArray, npt.NDArray]:
-        xx = x_y[0].copy()
-        yy = x_y[1]
-        # Augment each channel
-        if params.augmentations:
-            xx = augment_pipeline(
-                x=xx,
-                augmentations=params.augmentations,
-                sample_rate=params.sampling_rate,
-            )
+        with h5py.File(self._cache[pt_key], mode="r") as h5:
+            yield h5
+        # END WITH
+
+    def signal_generator(
+        self,
+        patient_generator: PatientGenerator,
+        frame_size: int,
+        samples_per_patient: int = 1,
+        target_rate: int | None = None,
+    ) -> Generator[npt.NDArray, None, None]:
+        """Generate frames using patient generator.
+
+        Args:
+            patient_generator (PatientGenerator): Generator that yields a tuple of patient id and patient data.
+            samples_per_patient (int): Samples per patient.
+
+        Returns:
+            SampleGenerator: Generator of input data of shape (frame_size, 1)
+        """
+        if target_rate is None:
+            target_rate = self.sampling_rate
+
+        input_size = int(np.round((self.sampling_rate / target_rate) * frame_size))
+
+        for pt in patient_generator:
+            with self.patient_data(pt) as h5:
+                data: h5py.Dataset = h5["data"][:]
+            # END WITH
+            for _ in range(samples_per_patient):
+                lead = random.choice(self.leads)
+                start = np.random.randint(0, data.shape[1] - input_size)
+                x = data[lead, start : start + input_size].squeeze()
+                x = np.nan_to_num(x).astype(np.float32)
+                x = self.add_noise(x)
+                if self.sampling_rate != target_rate:
+                    x = pk.signal.resample_signal(x, self.sampling_rate, target_rate, axis=0)
+                # END IF
+                yield x
+            # END FOR
+        # END FOR
+
+    def download(self, num_workers: int | None = None, force: bool = False):
+        """Download dataset
+
+        Args:
+            num_workers (int | None, optional): # parallel workers. Defaults to None.
+            force (bool, optional): Force redownload. Defaults to False.
+        """
+        # Nothing to do
+
+    def close(self):
+        """Close dataset"""
+        if self._noise_gen is not None:
+            self._noise_gen.close()
         # END IF
-        xx = prepare(xx, sample_rate=params.sampling_rate, preprocesses=params.preprocesses).reshape(feat_shape)
-        yy = tf.one_hot(yy, params.num_classes)
-        return xx, yy
-
-    train_datasets = []
-    val_datasets = []
-    for ds in datasets:
-        # Create TF datasets
-        train_ds, val_ds = ds.load_train_datasets(
-            train_patients=params.train_patients,
-            val_patients=params.val_patients,
-            train_pt_samples=params.samples_per_patient,
-            val_pt_samples=params.val_samples_per_patient,
-            val_file=params.val_file,
-            val_size=params.val_size,
-            preprocess=preprocess,
-            num_workers=params.data_parallelism,
-        )
-        train_datasets.append(train_ds)
-        val_datasets.append(val_ds)
-    # END FOR
-
-    ds_weights = np.array([d.weight for d in params.datasets])
-    ds_weights = ds_weights / ds_weights.sum()
-
-    train_ds = tf.data.Dataset.sample_from_datasets(train_datasets, weights=ds_weights)
-    val_ds = tf.data.Dataset.sample_from_datasets(val_datasets, weights=ds_weights)
-
-    # Shuffle and batch datasets for training
-    train_ds = (
-        train_ds.shuffle(
-            buffer_size=params.buffer_size,
-            reshuffle_each_iteration=True,
-        )
-        .batch(
-            batch_size=params.batch_size,
-            drop_remainder=False,
-            num_parallel_calls=tf.data.AUTOTUNE,
-        )
-        .prefetch(buffer_size=tf.data.AUTOTUNE)
-    )
-    val_ds = val_ds.batch(
-        batch_size=params.batch_size,
-        drop_remainder=True,
-        num_parallel_calls=tf.data.AUTOTUNE,
-    )
-    return train_ds, val_ds
-
+        self._cache.clear()
 
-def load_test_datasets(
-    datasets: list[HKDataset],
-    params: HKTestParams | HKExportParams,
-) -> tuple[HKDataset, npt.NDArray, npt.NDArray]:
-    """Load beat test dataset.
-
-    Args:
-        datasets (list[HeartKitDataset]): Datasets
-        params (HKTestParams|HKExportParams): Test params
-
-    Returns:
-        tuple[npt.NDArray, npt.NDArray]: Test data and labels
-    """
-
-    feat_shape = get_feat_shape(params.frame_size)
-
-    def preprocess(x_y: tuple[npt.NDArray, npt.NDArray]) -> tuple[npt.NDArray, npt.NDArray]:
-        xx = x_y[0].copy().squeeze()
-        xx = prepare(xx, sample_rate=params.sampling_rate, preprocesses=params.preprocesses).reshape(feat_shape)
-        yy = tf.one_hot(x_y[1], params.num_classes)
-        return xx, yy
-
-    with console.status("[bold green] Loading test dataset..."):
-        test_datasets = [
-            ds.load_test_dataset(
-                test_pt_samples=params.test_samples_per_patient,
-                test_file=params.test_file,
-                preprocess=preprocess,
-                num_workers=params.data_parallelism,
-            )
-            for ds in datasets
-        ]
+    def add_noise(self, ecg: npt.NDArray):
+        """Add noise to ECG signal."""
+        noise_range = self.params.noise_multiplier
+        if noise_range[0] == 0 and noise_range[1] == 0:
+            return ecg
+        noise_level = np.random.uniform(noise_range[0], noise_range[1])
 
-        ds_weights = np.array([d.weight for d in params.datasets])
-        ds_weights = ds_weights / ds_weights.sum()
+        if self._noise_gen is None:
+            self._noise_gen = NstdbNoise(target_rate=self.sampling_rate)
+        # END IF
+        self._noise_gen.apply_noise(ecg, noise_level)
+        return ecg
 
-        test_ds = tf.data.Dataset.sample_from_datasets(test_datasets, weights=ds_weights)
-        test_x, test_y = next(test_ds.batch(params.test_size).as_numpy_iterator())
-    # END WITH
-    return test_x, test_y
-
-
-def create_model(inputs: tf.Tensor, num_classes: int, architecture: ModelArchitecture | None) -> keras.Model:
-    """Generate model or use default
-
-    Args:
-        inputs (tf.Tensor): Model inputs
-        num_classes (int): Number of classes
-        architecture (ModelArchitecture|None): Model
-
-    Returns:
-        keras.Model: Model
-    """
-    if architecture:
-        return ModelFactory.create(
-            name=architecture.name,
-            params=architecture.params,
-            inputs=inputs,
-            num_classes=num_classes,
+    def _synthesize_signal(
+        self,
+        frame_size: int,
+        target_rate: float | None = None,
+    ) -> tuple[npt.NDArray, npt.NDArray, npt.NDArray]:
+        """Generate synthetic signal of given length
+
+        Args:
+            frame_size (int): Frame size
+
+        Returns:
+            tuple[npt.NDArray, npt.NDArray, npt.NDArray]: signal, segments, fiducials
+        """
+        heart_rate = np.random.uniform(self.params.heart_rate[0], self.params.heart_rate[1])
+        preset = random.choices(self.params.presets, self.params.preset_weights, k=1)[0].value
+        impedance = np.random.uniform(self.params.impedance[0], self.params.impedance[1])
+        p_multiplier = np.random.uniform(self.params.p_multiplier[0], self.params.p_multiplier[1])
+        t_multiplier = np.random.uniform(self.params.t_multiplier[0], self.params.t_multiplier[1])
+        voltage_factor = np.random.uniform(self.params.voltage_factor[0], self.params.voltage_factor[1])
+
+        ecg, segs, fids = pk.ecg.synthesize(
+            signal_length=frame_size,
+            sample_rate=target_rate,
+            leads=12,  # Use all 12 leads
+            heart_rate=heart_rate,
+            preset=preset,
+            impedance=impedance,
+            p_multiplier=p_multiplier,
+            t_multiplier=t_multiplier,
+            noise_multiplier=0,
+            voltage_factor=voltage_factor,
         )
-
-    return _default_model(inputs=inputs, num_classes=num_classes)
-
-
-def _default_model(
-    inputs: tf.Tensor,
-    num_classes: int,
-) -> keras.Model:
-    """Reference beat model
-
-    Args:
-        inputs (tf.Tensor): Model inputs
-        num_classes (int): Number of classes
-
-    Returns:
-        keras.Model: Model
-    """
-    blocks = [
-        MBConvParams(
-            filters=32,
-            depth=2,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 1),
-            se_ratio=2,
-        ),
-        MBConvParams(
-            filters=48,
-            depth=2,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=2,
-        ),
-        MBConvParams(
-            filters=64,
-            depth=3,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=4,
-        ),
-        MBConvParams(
-            filters=96,
-            depth=3,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=4,
-        ),
-    ]
-    return EfficientNetV2(
-        inputs,
-        params=EfficientNetParams(
-            input_filters=24,
-            input_strides=(1, 2),
-            input_kernel_size=(1, 5),
-            output_filters=0,
-            blocks=blocks,
-            include_top=True,
-            dropout=0.0,
-            drop_connect_rate=0.0,
-        ),
-        num_classes=num_classes,
-    )
+        return ecg, segs, fids
```

### Comparing `heartkit-1.2.0/heartkit/tasks/denoise/metrics.py` & `heartkit-1.3.0/heartkit/tasks/denoise/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     D = np.sum(np.square(y2 - y1), axis=1)
 
     SNR = 10 * np.log10(N / D)
 
     return SNR
 
 
-def SNR_improvement(y_in: npt.NDArray, y_out: npt.NDArray, y_clean: npt.NDArray) -> npt.NDArray:
+def snr_improvement(y_in: npt.NDArray, y_out: npt.NDArray, y_clean: npt.NDArray) -> npt.NDArray:
     """Compute signal to noise ratio improvement
 
     Args:
         y_in (npt.NDArray): Input signal
         y_out (npt.NDArray): Output signal
         y_clean (npt.NDArray): Clean signal
```

### Comparing `heartkit-1.2.0/heartkit/tasks/diagnostic/defines.py` & `heartkit-1.3.0/heartkit/tasks/diagnostic/defines.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/tasks/factory.py` & `heartkit-1.3.0/heartkit/tasks/factory.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/tasks/rhythm/defines.py` & `heartkit-1.3.0/heartkit/tasks/rhythm/defines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import IntEnum, StrEnum
 
 
 class HKRhythm(IntEnum):
     """Heart rhythm labels"""
 
-    sr = 0
+    sr = 0  # Sinus rhythm
     sbrad = 1  # Sinus bradycardia
     stach = 2  # Sinus tachycardia
 
     sarrh = 3  # Sinus arrhythmia
     svarr = 4  # Supraventricular arrhythmia
     svt = 5  # Supraventricular tachycardia
     vtach = 6  # Ventricular tachycardia
```

### Comparing `heartkit-1.2.0/heartkit/tasks/rhythm/utils.py` & `heartkit-1.3.0/heartkit/tasks/foundation/datasets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,156 +1,209 @@
+import functools
+import logging
 from pathlib import Path
 
-import keras
 import numpy as np
 import numpy.typing as npt
 import tensorflow as tf
-from rich.console import Console
 
-from ...datasets import DatasetFactory, HKDataset, augment_pipeline, preprocess_pipeline
+from ...datasets import (
+    HKDataset,
+    augment_pipeline,
+    preprocess_pipeline,
+    uniform_id_generator,
+)
+from ...datasets.dataloader import test_dataloader, train_val_dataloader
 from ...defines import (
-    DatasetParams,
+    AugmentationParams,
     HKExportParams,
     HKTestParams,
     HKTrainParams,
-    ModelArchitecture,
     PreprocessParams,
 )
-from ...models import EfficientNetParams, EfficientNetV2, MBConvParams, ModelFactory
-
-# from .defines import HKRhythm
+from ...utils import resolve_template_path
+from .dataloaders import lsad_data_generator, ptbxl_data_generator
 
-console = Console()
+logger = logging.getLogger(__name__)
 
 
-def get_feat_shape(frame_size: int) -> tuple[int, ...]:
-    """Get dataset feature shape.
+def preprocess(x: npt.NDArray, preprocesses: list[PreprocessParams], sample_rate: float) -> npt.NDArray:
+    """Preprocess data pipeline
 
     Args:
-        frame_size (int): Frame size
+        x (npt.NDArray): Input data
+        preprocesses (list[PreprocessParams]): Preprocess parameters
+        sample_rate (float): Sample rate
 
     Returns:
-        tuple[int, ...]: Feature shape
+        npt.NDArray: Preprocessed data
     """
-    return (frame_size, 1)  # Time x Channels
+    return preprocess_pipeline(x, preprocesses=preprocesses, sample_rate=sample_rate)
 
 
-def get_class_shape(frame_size: int, nclasses: int) -> tuple[int, ...]:
-    """Get dataset class shape.
+def augment(x: npt.NDArray, augmentations: list[AugmentationParams], sample_rate: float) -> npt.NDArray:
+    """Augment data pipeline
 
     Args:
-        frame_size (int): Frame size
-        nclasses (int): Number of classes
+        x (npt.NDArray): Input data
+        augmentations (list[AugmentationParams]): Augmentation parameters
+        sample_rate (float): Sample rate
 
     Returns:
-        tuple[int, ...]: Class shape
+        npt.NDArray: Augmented data
     """
-    return (nclasses,)  # One-hot encoded classes
+
+    return augment_pipeline(x=x, augmentations=augmentations, sample_rate=sample_rate)
 
 
-def prepare(x: npt.NDArray, sample_rate: float, preprocesses: list[PreprocessParams]) -> npt.NDArray:
-    """Prepare dataset.
+def prepare(
+    x_y: tuple[npt.NDArray, npt.NDArray],
+    sample_rate: float,
+    preprocesses: list[PreprocessParams],
+    augmentations: list[AugmentationParams],
+    spec: tuple[tf.TensorSpec, tf.TensorSpec],
+    num_classes: int,
+) -> tuple[npt.NDArray, npt.NDArray]:
+    """Prepare dataset
 
     Args:
-        x (npt.NDArray): Input signal
+        x_y (tuple[npt.NDArray, npt.NDArray]): Input data
         sample_rate (float): Sampling rate
         preprocesses (list[PreprocessParams]): Preprocessing pipeline
+        augmentations (list[AugmentationParams]): Augmentation pipeline
+        spec (tuple[tf.TensorSpec, tf.TensorSpec]): Spec
+        num_classes (int): Number of classes
 
     Returns:
-        npt.NDArray: Prepared signal
+        tuple[npt.NDArray, npt.NDArray]: Prepared data
     """
-    if not preprocesses:
-        preprocesses = [
-            dict(name="filter", args=dict(axis=0, lowcut=0.5, highcut=30, order=3, sample_rate=sample_rate)),
-            dict(name="znorm", args=dict(axis=None, eps=0.1)),
-        ]
-    return preprocess_pipeline(x, preprocesses=preprocesses, sample_rate=sample_rate)
+    x, y = x_y[0].copy(), x_y[1].copy()
 
+    if augmentations:
+        x = augment(x, augmentations, sample_rate)
+        y = augment(y, augmentations, sample_rate)
+    # END IF
 
-def load_datasets(
-    ds_path: Path,
-    frame_size: int,
-    sampling_rate: int,
-    spec: tuple[tf.TensorSpec, tf.TensorSpec],
-    class_map: dict[int, int],
-    datasets: list[DatasetParams],
-) -> list[HKDataset]:
-    """Load datasets
+    if preprocesses:
+        x = preprocess(x, preprocesses, sample_rate)
+        y = preprocess(y, preprocesses, sample_rate)
+    # END IF
+
+    x = x.reshape(spec[0].shape)
+    y = y.reshape(spec[0].shape)
+
+    return x, y
+
+
+def get_data_generator(ds: HKDataset, frame_size: int, samples_per_patient: int, target_rate: int):
+    """Get task data generator for dataset
 
     Args:
-        ds_path (Path): Path to dataset
+        ds (HKDataset): Dataset
         frame_size (int): Frame size
-        sampling_rate (int): Sampling rate
-        spec (tuple[tf.TensorSpec, tf.TensorSpec]): feat/class shape specs
-        class_map (dict[int, int]): Class map
-        datasets (list[DatasetParams]): List of datasets
+        samples_per_patient (int): Samples per patient
+        target_rate (int): Target rate
 
     Returns:
-        HeartKitDataset: Dataset
+        callable: Data generator
     """
-    dsets = []
-    for dset in datasets:
-        if DatasetFactory.has(dset.name):
-            dsets.append(
-                DatasetFactory.get(dset.name)(
-                    ds_path=ds_path,
-                    task="rhythm",
-                    frame_size=frame_size,
-                    target_rate=sampling_rate,
-                    class_map=class_map,
-                    spec=spec,
-                    **dset.params
-                )
-            )
-        # END IF
-    # END FOR
-    return dsets
+    match ds.name:
+        case "ptbxl":
+            data_generator = ptbxl_data_generator
+        case "lsad":
+            data_generator = lsad_data_generator
+        case _:
+            raise ValueError(f"Dataset {ds.name} not supported")
+    # END MATCH
+    return functools.partial(
+        data_generator,
+        ds=ds,
+        frame_size=frame_size,
+        samples_per_patient=samples_per_patient,
+        target_rate=target_rate,
+    )
+
+
+def resolve_ds_cache_path(fpath: Path | None, ds: HKDataset, task: str, frame_size: int, sample_rate: int):
+    """Resolve dataset cache path
+
+    Args:
+        fpath (Path|None): File path
+        ds (HKDataset): Dataset
+        task (str): Task
+        frame_size (int): Frame size
+        sample_rate (int): Sampling rate
+
+    Returns:
+        Path|None: Resolved path
+    """
+    if not fpath:
+        return None
+    return resolve_template_path(
+        fpath=fpath,
+        dataset=ds.name,
+        task=task,
+        frame_size=frame_size,
+        sampling_rate=sample_rate,
+    )
 
 
 def load_train_datasets(
     datasets: list[HKDataset],
     params: HKTrainParams,
+    ds_spec: tuple[tf.TensorSpec, tf.TensorSpec],
 ) -> tuple[tf.data.Dataset, tf.data.Dataset]:
-    """Load train datasets.
+    """Load training and validation datasets
 
     Args:
-        datasets (list[HeartKitDataset]): Datasets
-        params (HKTrainParams): Train params
+        datasets (list[HKDataset]): Datasets
+        params (HKTrainParams): Training parameters
+        ds_spec (tuple[tf.TensorSpec, tf.TensorSpec]): TensorSpec
 
     Returns:
         tuple[tf.data.Dataset, tf.data.Dataset]: Train and validation datasets
     """
 
-    feat_shape = get_feat_shape(params.frame_size)
-
-    def preprocess(x_y: tuple[npt.NDArray, npt.NDArray]) -> tuple[npt.NDArray, npt.NDArray]:
-        xx = x_y[0].copy()
-        yy = x_y[1]
-        if params.augmentations:
-            xx = augment_pipeline(
-                x=xx,
-                augmentations=params.augmentations,
-                sample_rate=params.sampling_rate,
-            )
-        xx = prepare(xx, sample_rate=params.sampling_rate, preprocesses=params.preprocesses).reshape(feat_shape)
-        yy = tf.one_hot(yy, params.num_classes)
-        return xx, yy
+    id_generator = functools.partial(uniform_id_generator, repeat=True)
+    train_prepare = functools.partial(
+        prepare,
+        sample_rate=params.sampling_rate,
+        preprocesses=params.preprocesses,
+        augmentations=params.augmentations,
+        spec=ds_spec,
+        num_classes=params.num_classes,
+    )
 
     train_datasets = []
     val_datasets = []
     for ds in datasets:
-        # Create TF datasets
-        train_ds, val_ds = ds.load_train_datasets(
+
+        val_file = resolve_ds_cache_path(
+            params.val_file, ds=ds, task="foundation", frame_size=params.frame_size, sample_rate=params.sampling_rate
+        )
+        data_generator = get_data_generator(
+            ds=ds,
+            frame_size=params.frame_size,
+            samples_per_patient=params.samples_per_patient,
+            target_rate=params.sampling_rate,
+        )
+
+        train_ds, val_ds = train_val_dataloader(
+            ds=ds,
+            spec=ds_spec,
+            data_generator=data_generator,
+            id_generator=id_generator,
             train_patients=params.train_patients,
             val_patients=params.val_patients,
-            train_pt_samples=params.samples_per_patient,
             val_pt_samples=params.val_samples_per_patient,
-            val_file=params.val_file,
+            val_file=val_file,
             val_size=params.val_size,
-            preprocess=preprocess,
+            label_map=None,
+            label_type=None,
+            preprocess=train_prepare,
             num_workers=params.data_parallelism,
         )
         train_datasets.append(train_ds)
         val_datasets.append(val_ds)
     # END FOR
 
     ds_weights = np.array([d.weight for d in params.datasets])
@@ -176,133 +229,71 @@
         batch_size=params.batch_size,
         drop_remainder=True,
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     return train_ds, val_ds
 
 
-def load_test_datasets(
+def load_test_dataset(
     datasets: list[HKDataset],
     params: HKTestParams | HKExportParams,
-) -> tuple[npt.NDArray, npt.NDArray]:
-    """Load test datasets.
+    ds_spec: tuple[tf.TensorSpec, tf.TensorSpec],
+) -> tf.data.Dataset:
+    """Load test dataset
 
     Args:
-        datasets (list[HeartKitDataset]): Datasets
-        params (HKTestParams|HKExportParams): Test params
+        datasets (list[HKDataset]): Datasets
+        params (HKTestParams|HKExportParams): Test parameters
+        ds_spec (tuple[tf.TensorSpec, tf.TensorSpec]): TensorSpec
 
     Returns:
-        tuple[npt.NDArray, npt.NDArray]: Test data and labels
+        tf.data.Dataset: Test dataset
     """
 
-    feat_shape = get_feat_shape(params.frame_size)
-
-    def preprocess(x_y: tuple[npt.NDArray, npt.NDArray]) -> tuple[npt.NDArray, npt.NDArray]:
-        xx = x_y[0].copy().squeeze()
-        xx = prepare(xx, sample_rate=params.sampling_rate, preprocesses=params.preprocesses).reshape(feat_shape)
-        yy = tf.one_hot(x_y[1], params.num_classes)
-        return xx, yy
-
-    with console.status("[bold green] Loading test dataset..."):
-        test_datasets = [
-            ds.load_test_dataset(
-                test_pt_samples=params.test_samples_per_patient,
-                test_file=params.test_file,
-                preprocess=preprocess,
-                num_workers=params.data_parallelism,
-            )
-            for ds in datasets
-        ]
-
-        ds_weights = np.array([d.weight for d in params.datasets])
-        ds_weights = ds_weights / ds_weights.sum()
-
-        test_ds = tf.data.Dataset.sample_from_datasets(test_datasets, weights=ds_weights)
-        test_x, test_y = next(test_ds.batch(params.test_size).as_numpy_iterator())
-    # END WITH
-    return test_x, test_y
-
-
-def create_model(inputs: tf.Tensor, num_classes: int, architecture: ModelArchitecture | None) -> keras.Model:
-    """Generate model or use default
+    id_generator = functools.partial(uniform_id_generator, repeat=True)
+    test_prepare = functools.partial(
+        prepare,
+        preprocesses=params.preprocesses,
+        augmentations=params.augmentations,
+        spec=ds_spec,
+        num_classes=params.num_classes,
+    )
 
-    Args:
-        inputs (tf.Tensor): Model inputs
-        num_classes (int): Number of classes
-        architecture (ModelArchitecture|None): Model
+    test_datasets = []
+    for ds in datasets:
 
-    Returns:
-        keras.Model: Model
-    """
-    if architecture:
-        return ModelFactory.create(
-            name=architecture.name,
-            params=architecture.params,
-            inputs=inputs,
-            num_classes=num_classes,
+        test_file = resolve_ds_cache_path(
+            fpath=params.test_file,
+            ds=ds,
+            task="foundation",
+            frame_size=params.frame_size,
+            sample_rate=params.sampling_rate,
+        )
+        data_generator = get_data_generator(
+            ds=ds,
+            frame_size=params.frame_size,
+            samples_per_patient=params.test_samples_per_patient,
+            target_rate=params.sampling_rate,
         )
 
-    return _default_model(inputs=inputs, num_classes=num_classes)
-
-
-def _default_model(
-    inputs: tf.Tensor,
-    num_classes: int,
-) -> keras.Model:
-    """Reference model
+        test_ds = test_dataloader(
+            ds=ds,
+            spec=ds_spec,
+            data_generator=data_generator,
+            id_generator=id_generator,
+            test_patients=params.test_patients,
+            test_file=test_file,
+            label_map=None,
+            label_type=None,
+            preprocess=test_prepare,
+            num_workers=params.data_parallelism,
+        )
+        test_datasets.append(test_ds)
+    # END FOR
 
-    Args:
-        inputs (tf.Tensor): Model inputs
-        num_classes (int): Number of classes
+    ds_weights = np.array([d.weight for d in params.datasets])
+    ds_weights = ds_weights / ds_weights.sum()
 
-    Returns:
-        keras.Model: Model
-    """
+    test_ds = tf.data.Dataset.sample_from_datasets(test_datasets, weights=ds_weights)
 
-    blocks = [
-        MBConvParams(
-            filters=32,
-            depth=2,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=2,
-        ),
-        MBConvParams(
-            filters=48,
-            depth=1,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=4,
-        ),
-        MBConvParams(
-            filters=64,
-            depth=2,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=4,
-        ),
-        MBConvParams(
-            filters=80,
-            depth=1,
-            ex_ratio=1,
-            kernel_size=(1, 3),
-            strides=(1, 2),
-            se_ratio=4,
-        ),
-    ]
-    return EfficientNetV2(
-        inputs,
-        params=EfficientNetParams(
-            input_filters=24,
-            input_kernel_size=(1, 3),
-            input_strides=(1, 2),
-            blocks=blocks,
-            output_filters=0,
-            include_top=True,
-            dropout=0.0,
-            drop_connect_rate=0.0,
-        ),
-        num_classes=num_classes,
-    )
+    # END WITH
+    return test_ds
```

### Comparing `heartkit-1.2.0/heartkit/tasks/segmentation/metrics.py` & `heartkit-1.3.0/heartkit/tasks/segmentation/metrics.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/tasks/task.py` & `heartkit-1.3.0/heartkit/tasks/task.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/tflite/convert.py` & `heartkit-1.3.0/heartkit/tflite/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 
     # Debug model
     debugger = tf.lite.experimental.QuantizationDebugger(
         converter=converter, debug_dataset=converter.representative_dataset
     )
     debugger.run()
 
+    # Dump layer statistics and convert to DataFrame
     with io.StringIO() as f:
         debugger.layer_statistics_dump(f)
         f.seek(0)
         layer_stats = pd.read_csv(f)
 
     # Add custom metrics
     layer_stats["range"] = 255.0 * layer_stats["scale"]
```

### Comparing `heartkit-1.2.0/heartkit/tflite/metrics.py` & `heartkit-1.3.0/heartkit/tflite/metrics.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/heartkit/tflite/model.py` & `heartkit-1.3.0/heartkit/tflite/model.py`

 * *Files identical despite different names*

### Comparing `heartkit-1.2.0/pyproject.toml` & `heartkit-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heartkit"
-version = "1.2.0"
+version = "1.3.0"
 description = "AI driven heart monitoring kit for ultra low-power wearables."
 license = "BSD-3-Clause"
 authors = ["Ambiq AI <support.aitg@ambiq.com>"]
 readme = "README.md"
 homepage = "https://ambiq.ai"
 packages = [
     { include = "heartkit" },
@@ -86,33 +86,38 @@
 
 [tool.isort]
 profile = 'black'
 
 [tool.black]
 line-length = 120
 
+[tool.pylint]
+ignored-modules = ["h5py"]
+
 [tool.pylint.master]
 ignore-paths = [
     "heartkit/rpc/GenericDataOperations_EvbToPc",
     "heartkit/rpc/GenericDataOperations_PcToEvb",
     "heartkit/rpc/erpc"
 ]
 extension-pkg-whitelist = "pydantic"
 
+
 [tool.pylint.message_control]
 disable = [
     "unused-argument",
     "missing-module-docstring",
     "too-few-public-methods",
     "invalid-name",
     "logging-fstring-interpolation",
     "duplicate-code",
     "use-dict-literal",
     "cyclic-import",
-    "unsubscriptable-object"
+    "unsubscriptable-object",
+    "not-callable"
 ]
 
 [tool.pylint.format]
 max-line-length = 140
 
 [tool.pylint.design]
 max-args = 50
```

### Comparing `heartkit-1.2.0/PKG-INFO` & `heartkit-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartkit
-Version: 1.2.0
+Version: 1.3.0
 Summary: AI driven heart monitoring kit for ultra low-power wearables.
 Home-page: https://ambiq.ai
 License: BSD-3-Clause
 Author: Ambiq AI
 Author-email: support.aitg@ambiq.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: heartkit Version: 1.2.0 Summary: AI driven heart
+Metadata-Version: 2.1 Name: heartkit Version: 1.3.0 Summary: AI driven heart
 monitoring kit for ultra low-power wearables. Home-page: https://ambiq.ai
 License: BSD-3-Clause Author: Ambiq AI Author-email: support.aitg@ambiq.com
 Requires-Python: >=3.11,<3.12 Classifier: License :: OSI Approved :: BSD
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: argdantic[all] (>=1.0.0,<2.0.0)
 Requires-Dist: boto3 (>=1.34.36,<2.0.0) Requires-Dist: fastparquet
 (>=2023.10.1,<2024.0.0) Requires-Dist: matplotlib (==3.8.2) Requires-Dist:
```

