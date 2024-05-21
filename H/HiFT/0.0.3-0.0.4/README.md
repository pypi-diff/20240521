# Comparing `tmp/HiFT-0.0.3.tar.gz` & `tmp/HiFT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HiFT-0.0.3.tar", last modified: Wed May 15 12:42:06 2024, max compression
+gzip compressed data, was "dist/HiFT-0.0.4.tar", last modified: Tue May 21 01:02:20 2024, max compression
```

## Comparing `HiFT-0.0.3.tar` & `HiFT-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.140874 HiFT-0.0.3/
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.024879 HiFT-0.0.3/HiFT.egg-info/
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/SOURCES.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/dependency_links.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-15 12:42:05.000000 HiFT-0.0.3/HiFT.egg-info/top_level.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)    11324 2024-05-14 23:32:09.000000 HiFT-0.0.3/LICENSE.md
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-15 12:42:06.136874 HiFT-0.0.3/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.3/README.md
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.044878 HiFT-0.0.3/examples/
--rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.3/examples/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4135 2024-05-14 12:27:27.000000 HiFT-0.0.3/examples/build_dataset.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    23087 2024-05-14 20:25:29.000000 HiFT-0.0.3/examples/instruct_tuning.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.3/examples/llama2_flash_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.3/examples/llama_flash_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.3/examples/llama_xformers_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    30731 2024-05-14 15:18:26.000000 HiFT-0.0.3/examples/pretrain_tuning.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    35374 2024-05-14 21:31:37.000000 HiFT-0.0.3/examples/run_generation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    33754 2024-05-14 20:20:10.000000 HiFT-0.0.3/examples/run_glue.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    32543 2024-05-14 20:20:40.000000 HiFT-0.0.3/examples/run_ner.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    37615 2024-05-14 20:20:53.000000 HiFT-0.0.3/examples/run_qa.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.3/examples/utils_qa.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    20863 2024-05-14 20:21:08.000000 HiFT-0.0.3/examples/vicuna_train.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.048878 HiFT-0.0.3/hift/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/__init__.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.112875 HiFT-0.0.3/hift/optimizers/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      761 2024-05-14 15:15:35.000000 HiFT-0.0.3/hift/optimizers/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/adagrad.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.132874 HiFT-0.0.3/hift/optimizers/bitsandbytes/
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/adagrad.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/adam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/adamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/lamb.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/lars.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/lion.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/bitsandbytes/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/optimization.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/optimizer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    37568 2024-05-14 15:15:17.000000 HiFT-0.0.3/hift/optimizers/replace_operation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/torchAdam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/optimizers/torchAdamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/qatrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12584 2024-05-15 12:39:58.000000 HiFT-0.0.3/hift/registerCallBack.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/seqtrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    77451 2024-05-14 15:15:05.000000 HiFT-0.0.3/hift/trainer.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-15 12:42:06.136874 HiFT-0.0.3/hift/utils/
--rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/utils/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.3/hift/utils/utils.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-15 12:42:06.140874 HiFT-0.0.3/setup.cfg
--rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-15 12:41:58.000000 HiFT-0.0.3/setup.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.687325 HiFT-0.0.4/
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.627328 HiFT-0.0.4/HiFT.egg-info/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/SOURCES.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/dependency_links.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/top_level.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11324 2024-05-14 23:32:09.000000 HiFT-0.0.4/LICENSE.md
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-21 01:02:20.687325 HiFT-0.0.4/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.4/README.md
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.647327 HiFT-0.0.4/examples/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.4/examples/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4135 2024-05-14 12:27:27.000000 HiFT-0.0.4/examples/build_dataset.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23087 2024-05-14 20:25:29.000000 HiFT-0.0.4/examples/instruct_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.4/examples/llama2_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.4/examples/llama_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.4/examples/llama_xformers_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30731 2024-05-14 15:18:26.000000 HiFT-0.0.4/examples/pretrain_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    35374 2024-05-20 23:57:56.000000 HiFT-0.0.4/examples/run_generation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    33754 2024-05-14 20:20:10.000000 HiFT-0.0.4/examples/run_glue.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    32543 2024-05-14 20:20:40.000000 HiFT-0.0.4/examples/run_ner.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37615 2024-05-14 20:20:53.000000 HiFT-0.0.4/examples/run_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.4/examples/utils_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    20863 2024-05-14 20:21:08.000000 HiFT-0.0.4/examples/vicuna_train.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.655326 HiFT-0.0.4/hift/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/__init__.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.671326 HiFT-0.0.4/hift/optimizers/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      761 2024-05-14 15:15:35.000000 HiFT-0.0.4/hift/optimizers/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/adagrad.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.683325 HiFT-0.0.4/hift/optimizers/bitsandbytes/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/adagrad.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/adam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/adamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/lamb.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/lars.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/lion.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/optimization.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/optimizer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37568 2024-05-14 15:15:17.000000 HiFT-0.0.4/hift/optimizers/replace_operation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/torchAdam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/torchAdamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/qatrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12599 2024-05-21 01:00:32.000000 HiFT-0.0.4/hift/registerCallBack.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/seqtrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    77451 2024-05-14 15:15:05.000000 HiFT-0.0.4/hift/trainer.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.683325 HiFT-0.0.4/hift/utils/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/utils/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/utils/utils.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-21 01:02:20.687325 HiFT-0.0.4/setup.cfg
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-21 01:00:41.000000 HiFT-0.0.4/setup.py
```

### Comparing `HiFT-0.0.3/HiFT.egg-info/PKG-INFO` & `HiFT-0.0.4/HiFT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.3/HiFT.egg-info/SOURCES.txt` & `HiFT-0.0.4/HiFT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/LICENSE.md` & `HiFT-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/PKG-INFO` & `HiFT-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.3/README.md` & `HiFT-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/build_dataset.py` & `HiFT-0.0.4/examples/build_dataset.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/instruct_tuning.py` & `HiFT-0.0.4/examples/instruct_tuning.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/llama2_flash_attn_monkey_patch.py` & `HiFT-0.0.4/examples/llama2_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/llama_flash_attn_monkey_patch.py` & `HiFT-0.0.4/examples/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/llama_xformers_attn_monkey_patch.py` & `HiFT-0.0.4/examples/llama_xformers_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/pretrain_tuning.py` & `HiFT-0.0.4/examples/pretrain_tuning.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/run_generation.py` & `HiFT-0.0.4/examples/run_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     "openai-gpt": (OpenAIGPTLMHeadModel, OpenAIGPTTokenizer,OpenAIGPTConfig),
     "xlnet": (XLNetLMHeadModel, XLNetTokenizer,XLNetConfig),
     "transfo-xl": (TransfoXLLMHeadModel, TransfoXLTokenizer,TransfoXLConfig),
     "xlm": (XLMWithLMHeadModel, XLMTokenizer,XLMConfig),
     "gptj": (GPTJForCausalLM, AutoTokenizer,GPTJConfig),
     "bloom": (BloomForCausalLM, BloomTokenizerFast,BloomConfig),
     "llama": (AutoModelForCausalLM, AutoTokenizer,AutoConfig),
-    "opt": (OPTForCausalLM, GPT2Tokenizer,OPTConfig),
+    "opt": (OPTForCausalLM, AutoTokenizer,OPTConfig),
 }
 
 
 # Will error if the minimal version of Transformers is not installed. Remove at your own risks.
 check_min_version("4.27.0")
 
 require_version("datasets>=1.8.0", "To fix: pip install -r examples/pytorch/summarization/requirements.txt")
```

### Comparing `HiFT-0.0.3/examples/run_glue.py` & `HiFT-0.0.4/examples/run_glue.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/run_ner.py` & `HiFT-0.0.4/examples/run_ner.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/run_qa.py` & `HiFT-0.0.4/examples/run_qa.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/utils_qa.py` & `HiFT-0.0.4/examples/utils_qa.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/examples/vicuna_train.py` & `HiFT-0.0.4/examples/vicuna_train.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/__init__.py` & `HiFT-0.0.4/hift/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/adagrad.py` & `HiFT-0.0.4/hift/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/__init__.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/__init__.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/adagrad.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/adagrad.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/adam.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/adam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/adamw.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/adamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/lamb.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/lamb.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/lars.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/lars.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/lion.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/lion.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/rmsprop.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/bitsandbytes/sgd.py` & `HiFT-0.0.4/hift/optimizers/bitsandbytes/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/optimization.py` & `HiFT-0.0.4/hift/optimizers/optimization.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/optimizer.py` & `HiFT-0.0.4/hift/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/replace_operation.py` & `HiFT-0.0.4/hift/optimizers/replace_operation.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/rmsprop.py` & `HiFT-0.0.4/hift/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/sgd.py` & `HiFT-0.0.4/hift/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/torchAdam.py` & `HiFT-0.0.4/hift/optimizers/torchAdam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/optimizers/torchAdamw.py` & `HiFT-0.0.4/hift/optimizers/torchAdamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/qatrainer.py` & `HiFT-0.0.4/hift/qatrainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/registerCallBack.py` & `HiFT-0.0.4/hift/registerCallBack.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                     if matches[0] not in group_parameters:
                         group_parameters.append(matches[0])
         if hasattr(self,"merge_param"):
             group_parameters = self.merge_param(group_parameters)
         if len(self.freeze_layers)>0:
             for index in self.freeze_layers:
                 group_parameters[int(index)]=-1
-                group_parameters = [element for element in group_parameters if element != -1]
+        group_parameters = [element for element in group_parameters if element != -1]
         if self.strategy=="up2down":
            group_parameters.reverse()
         elif self.strategy == "random":
             random.shuffle(group_parameters)
         elif self.strategy != "down2up":
             raise ValueError("providing proper strategy")
         print(group_parameters)
@@ -356,8 +356,10 @@
         return MODDELS_HiFT_PROCESS["gptneox"]
     if "gptneo" in model_name_path.lower() or "gpt-neo" in model_name_path.lower():
         return MODDELS_HiFT_PROCESS["gptneo"]
     if "opt" in model_name_path.lower():
         return MODDELS_HiFT_PROCESS["opt"]
     if "llamafamily" in model_name_path.lower() or "llama" in model_name_path.lower():
         return MODDELS_HiFT_PROCESS["llamafamily"]
+    else:
+        pass
```

### Comparing `HiFT-0.0.3/hift/seqtrainer.py` & `HiFT-0.0.4/hift/seqtrainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/trainer.py` & `HiFT-0.0.4/hift/trainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/hift/utils/utils.py` & `HiFT-0.0.4/hift/utils/utils.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.3/setup.py` & `HiFT-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HiFT",
-    version="0.0.3",
+    version="0.0.4",
     author="Yongkang Liu",
     author_email="misonsky@163.com",
     description="PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/misonsky/HiFT",
     packages=setuptools.find_packages(),
```

