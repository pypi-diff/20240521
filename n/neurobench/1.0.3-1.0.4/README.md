# Comparing `tmp/neurobench-1.0.3.tar.gz` & `tmp/neurobench-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurobench-1.0.3.tar", max compression
+gzip compressed data, was "neurobench-1.0.4.tar", max compression
```

## Comparing `neurobench-1.0.3.tar` & `neurobench-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0    11357 2024-01-15 21:04:23.558633 neurobench-1.0.3/LICENSE
--rw-r--r--   0        0        0     7378 2024-03-04 19:47:02.911313 neurobench-1.0.3/README.rst
--rw-r--r--   0        0        0        0 2024-01-15 21:04:23.558989 neurobench-1.0.3/neurobench/__init__.py
--rw-r--r--   0        0        0       25 2024-04-12 15:27:09.486417 neurobench-1.0.3/neurobench/benchmarks/__init__.py
--rw-r--r--   0        0        0     6585 2024-04-12 15:27:09.486824 neurobench-1.0.3/neurobench/benchmarks/benchmark.py
--rw-r--r--   0        0        0     3005 2024-04-12 15:27:09.487120 neurobench-1.0.3/neurobench/benchmarks/hooks.py
--rw-r--r--   0        0        0     4845 2024-04-12 15:27:09.487487 neurobench-1.0.3/neurobench/benchmarks/static_metrics.py
--rw-r--r--   0        0        0    13711 2024-04-12 15:27:09.487832 neurobench-1.0.3/neurobench/benchmarks/workload_metrics.py
--rw-r--r--   0        0        0     5704 2024-04-12 15:27:09.488252 neurobench-1.0.3/neurobench/datasets/MSWC_IncrementalLoader.py
--rw-r--r--   0        0        0    11325 2024-04-12 15:27:09.488613 neurobench-1.0.3/neurobench/datasets/MSWC_dataset.py
--rw-r--r--   0        0        0     3773 2024-04-12 15:27:09.488852 neurobench-1.0.3/neurobench/datasets/WISDM.py
--rw-r--r--   0        0        0     1088 2024-04-12 15:27:09.489528 neurobench-1.0.3/neurobench/datasets/__init__.py
--rw-r--r--   0        0        0      845 2024-04-12 15:27:09.490179 neurobench-1.0.3/neurobench/datasets/dataset.py
--rw-r--r--   0        0        0    10055 2024-04-12 15:27:09.490468 neurobench-1.0.3/neurobench/datasets/dvs_gesture.py
--rw-r--r--   0        0        0     9110 2024-04-12 15:27:09.490732 neurobench-1.0.3/neurobench/datasets/mackey_glass.py
--rw-r--r--   0        0        0     6501 2024-04-12 15:27:09.491234 neurobench-1.0.3/neurobench/datasets/megapixel_automotive.py
--rw-r--r--   0        0        0    13965 2024-04-12 15:27:09.491549 neurobench-1.0.3/neurobench/datasets/primate_reaching.py
--rw-r--r--   0        0        0     2705 2024-04-12 15:27:09.492250 neurobench-1.0.3/neurobench/datasets/speech_commands.py
--rw-r--r--   0        0        0     5469 2024-04-12 15:27:09.492651 neurobench-1.0.3/neurobench/datasets/utils.py
--rw-r--r--   0        0        0      346 2024-04-12 15:27:09.496469 neurobench-1.0.3/neurobench/models/__init__.py
--rw-r--r--   0        0        0     4052 2024-04-12 15:27:09.496822 neurobench-1.0.3/neurobench/models/model.py
--rw-r--r--   0        0        0     1674 2024-04-12 15:27:09.497247 neurobench-1.0.3/neurobench/models/snntorch_models.py
--rw-r--r--   0        0        0      818 2024-04-12 15:27:09.497877 neurobench-1.0.3/neurobench/models/torch_model.py
--rw-r--r--   0        0        0        0 2024-01-24 16:02:09.339052 neurobench-1.0.3/neurobench/models/utils.py
--rw-r--r--   0        0        0       29 2024-04-12 15:27:09.498538 neurobench-1.0.3/neurobench/postprocessing/__init__.py
--rw-r--r--   0        0        0     1633 2024-04-12 15:27:09.498864 neurobench-1.0.3/neurobench/postprocessing/postprocessor.py
--rw-r--r--   0        0        0      374 2024-04-12 15:27:09.499414 neurobench-1.0.3/neurobench/preprocessing/__init__.py
--rw-r--r--   0        0        0     3082 2024-04-12 15:27:09.500043 neurobench-1.0.3/neurobench/preprocessing/mfcc.py
--rw-r--r--   0        0        0      952 2024-04-12 15:27:09.500718 neurobench-1.0.3/neurobench/preprocessing/preprocessor.py
--rw-r--r--   0        0        0     6655 2024-04-12 15:27:09.501175 neurobench-1.0.3/neurobench/preprocessing/speech2spikes.py
--rw-r--r--   0        0        0    12063 2024-04-12 15:27:09.501569 neurobench-1.0.3/neurobench/utils.py
--rw-r--r--   0        0        0     1115 2024-04-12 15:28:56.137992 neurobench-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 neurobench-1.0.3/setup.py
--rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 neurobench-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-15 21:04:23.558633 neurobench-1.0.4/LICENSE
+-rw-r--r--   0        0        0     7378 2024-05-08 13:32:22.050662 neurobench-1.0.4/README.rst
+-rw-r--r--   0        0        0        0 2024-01-15 21:04:23.558989 neurobench-1.0.4/neurobench/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-21 15:48:40.886885 neurobench-1.0.4/neurobench/benchmarks/__init__.py
+-rw-r--r--   0        0        0     6624 2024-05-21 15:48:40.887304 neurobench-1.0.4/neurobench/benchmarks/benchmark.py
+-rw-r--r--   0        0        0     3313 2024-05-21 15:48:40.888421 neurobench-1.0.4/neurobench/benchmarks/hooks.py
+-rw-r--r--   0        0        0     4845 2024-05-16 21:10:18.324606 neurobench-1.0.4/neurobench/benchmarks/static_metrics.py
+-rw-r--r--   0        0        0    15861 2024-05-21 15:48:40.889154 neurobench-1.0.4/neurobench/benchmarks/workload_metrics.py
+-rw-r--r--   0        0        0     5704 2024-05-16 21:10:18.325788 neurobench-1.0.4/neurobench/datasets/MSWC_IncrementalLoader.py
+-rw-r--r--   0        0        0    11326 2024-05-21 15:48:40.889638 neurobench-1.0.4/neurobench/datasets/MSWC_dataset.py
+-rw-r--r--   0        0        0     3773 2024-05-16 21:10:18.326578 neurobench-1.0.4/neurobench/datasets/WISDM.py
+-rw-r--r--   0        0        0      945 2024-05-21 15:48:40.890166 neurobench-1.0.4/neurobench/datasets/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-16 21:10:18.326963 neurobench-1.0.4/neurobench/datasets/dataset.py
+-rw-r--r--   0        0        0     9110 2024-05-16 21:10:18.327407 neurobench-1.0.4/neurobench/datasets/mackey_glass.py
+-rw-r--r--   0        0        0     6501 2024-05-16 21:10:18.327904 neurobench-1.0.4/neurobench/datasets/megapixel_automotive.py
+-rw-r--r--   0        0        0    14131 2024-05-21 15:53:47.687640 neurobench-1.0.4/neurobench/datasets/primate_reaching.py
+-rw-r--r--   0        0        0     2705 2024-05-16 21:10:18.329182 neurobench-1.0.4/neurobench/datasets/speech_commands.py
+-rw-r--r--   0        0        0     5469 2024-05-16 21:10:18.329698 neurobench-1.0.4/neurobench/datasets/utils.py
+-rw-r--r--   0        0        0      346 2024-05-08 13:37:16.292392 neurobench-1.0.4/neurobench/models/__init__.py
+-rw-r--r--   0        0        0     4052 2024-05-16 21:10:18.333487 neurobench-1.0.4/neurobench/models/model.py
+-rw-r--r--   0        0        0     1674 2024-05-16 21:10:18.333795 neurobench-1.0.4/neurobench/models/snntorch_models.py
+-rw-r--r--   0        0        0      818 2024-05-16 21:10:18.335008 neurobench-1.0.4/neurobench/models/torch_model.py
+-rw-r--r--   0        0        0        0 2024-01-24 16:02:09.339052 neurobench-1.0.4/neurobench/models/utils.py
+-rw-r--r--   0        0        0       29 2024-05-08 13:37:16.294108 neurobench-1.0.4/neurobench/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1633 2024-05-16 21:10:18.335324 neurobench-1.0.4/neurobench/postprocessing/postprocessor.py
+-rw-r--r--   0        0        0      374 2024-05-08 13:37:16.295079 neurobench-1.0.4/neurobench/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3082 2024-05-16 21:10:18.335597 neurobench-1.0.4/neurobench/preprocessing/mfcc.py
+-rw-r--r--   0        0        0      952 2024-05-16 21:10:18.335895 neurobench-1.0.4/neurobench/preprocessing/preprocessor.py
+-rw-r--r--   0        0        0     6655 2024-05-16 21:10:18.336180 neurobench-1.0.4/neurobench/preprocessing/speech2spikes.py
+-rw-r--r--   0        0        0    12063 2024-05-16 21:10:18.336460 neurobench-1.0.4/neurobench/utils.py
+-rw-r--r--   0        0        0     1115 2024-05-21 15:48:40.894471 neurobench-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8698 1970-01-01 00:00:00.000000 neurobench-1.0.4/setup.py
+-rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 neurobench-1.0.4/PKG-INFO
```

### Comparing `neurobench-1.0.3/LICENSE` & `neurobench-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/README.rst` & `neurobench-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/benchmarks/benchmark.py` & `neurobench-1.0.4/neurobench/benchmarks/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import sys
 from contextlib import redirect_stdout
 from tqdm import tqdm
 
 from . import static_metrics, workload_metrics
 
 # workload metrics which require hooks
-requires_hooks = ["activation_sparsity", "number_neuron_updates", "synaptic_operations"]
+requires_hooks = [
+    "activation_sparsity",
+    "number_neuron_updates",
+    "synaptic_operations",
+    "membrane_updates",
+]
 
 
 class Benchmark:
     """Top-level benchmark class for running benchmarks."""
 
     def __init__(self, model, dataloader, preprocessors, postprocessors, metric_list):
         """
```

### Comparing `neurobench-1.0.3/neurobench/benchmarks/hooks.py` & `neurobench-1.0.4/neurobench/benchmarks/hooks.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
         Args:
             layer: The activation layer which is a PyTorch nn.Module.
 
         """
         self.activation_outputs = []
         self.activation_inputs = []
+        self.pre_fire_mem_potential = []
+        self.post_fire_mem_potential = []
         if layer is not None:
             self.hook = layer.register_forward_hook(self.hook_fn)
             self.hook_pre = layer.register_forward_pre_hook(self.pre_hook_fn)
         else:
             self.hook = None
             self.hook_pre = None
 
@@ -42,14 +44,16 @@
 
         Args:
             layer: The registered layer
             input: Input of the registered layer
 
         """
         self.activation_inputs.append(input)
+        if self.spiking:
+            self.pre_fire_mem_potential.append(layer.mem)
 
     def hook_fn(self, layer, input, output):
         """
         Hook function that will be called after each forward pass of the activation
         layer.
 
         Each output of the activation layer will be stored.
@@ -58,27 +62,30 @@
             layer: The registered layer
             input: Input of the registered layer
             output: Output of the registered layer
 
         """
         if self.spiking:
             self.activation_outputs.append(output[0])
+            self.post_fire_mem_potential.append(layer.mem)
 
         else:
             self.activation_outputs.append(output)
 
     def empty_hook(self):
         """Deletes the contents of the hooks, but keeps the hook registered."""
         self.activation_outputs = []
         self.activation_inputs = []
 
     def reset(self):
         """Resets the stored activation outputs and inputs."""
         self.activation_outputs = []
         self.activation_inputs = []
+        self.pre_fire_mem_potential = []
+        self.post_fire_mem_potential = []
 
     def close(self):
         """Remove the registered hook."""
         if self.hook:
             self.hook.remove()
         if self.hook_pre:
             self.hook_pre.remove()
```

### Comparing `neurobench-1.0.3/neurobench/benchmarks/static_metrics.py` & `neurobench-1.0.4/neurobench/benchmarks/static_metrics.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/benchmarks/workload_metrics.py` & `neurobench-1.0.4/neurobench/benchmarks/workload_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 import numpy as np
 from ..utils import check_shape, make_binary_copy, single_layer_MACs
 from .hooks import ActivationHook, LayerHook
+from collections import defaultdict
 
 
 class AccumulatedMetric:
     """Abstract class for a metric which must save state between batches."""
 
     def __init__(self):
         """Initialize metric."""
@@ -117,14 +118,76 @@
         (total_neuro_num - total_spike_num) / total_neuro_num
         if total_neuro_num != 0
         else 0.0
     )
     return sparsity
 
 
+class membrane_updates(AccumulatedMetric):
+    """
+    Number of membrane potential updates.
+
+    This metric can only be used for spiking models implemented with SNNTorch.
+
+    """
+
+    def __init__(self):
+        """Init metric state."""
+        self.total_samples = 0
+        self.neuron_membrane_updates = defaultdict(int)
+
+    def reset(self):
+        """Reset metric state."""
+        self.total_samples = 0
+        self.neuron_membrane_updates = defaultdict(int)
+
+    def __call__(self, model, preds, data):
+        """
+        Number of membrane updates of the model forward.
+
+        Args:
+            model: A NeuroBenchModel.
+            preds: A tensor of model predictions.
+            data: A tuple of data and labels.
+        Returns:
+            float: Number of membrane potential updates.
+
+        """
+        for hook in model.activation_hooks:
+            for index_mem in range(len(hook.pre_fire_mem_potential) - 1):
+                pre_fire_mem = hook.pre_fire_mem_potential[index_mem + 1]
+                post_fire_mem = hook.post_fire_mem_potential[index_mem + 1]
+                nr_updates = torch.count_nonzero(pre_fire_mem - post_fire_mem)
+                self.neuron_membrane_updates[str(type(hook.layer))] += int(nr_updates)
+            self.neuron_membrane_updates[str(type(hook.layer))] += int(
+                torch.numel(hook.post_fire_mem_potential[0])
+            )
+        self.total_samples += data[0].size(0)
+        return self.compute()
+
+    def compute(self):
+        """
+        Compute membrane updates using accumulated data.
+
+        Returns:
+            float: Compute the total updates to each neuron's membrane potential within the model,
+            aggregated across all neurons and normalized by the number of samples processed.
+
+        """
+        if self.total_samples == 0:
+            return 0
+
+        total_mem_updates = 0
+        for key in self.neuron_membrane_updates:
+            total_mem_updates += self.neuron_membrane_updates[key]
+
+        total_updates_per_sample = total_mem_updates / self.total_samples
+        return total_updates_per_sample
+
+
 def number_neuron_updates(model, preds, data):
     """
     Number of times each neuron type is updated.
 
     Args:
         model: A NeuroBenchModel.
         preds: A tensor of model predictions.
```

### Comparing `neurobench-1.0.3/neurobench/datasets/MSWC_IncrementalLoader.py` & `neurobench-1.0.4/neurobench/datasets/MSWC_IncrementalLoader.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/datasets/MSWC_dataset.py` & `neurobench-1.0.4/neurobench/datasets/MSWC_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,15 @@
 
 
 class MSWC(Dataset):
     """
     Subset version (https://huggingface.co/datasets/NeuroBench/mswc_fscil_subset)
     of the original MSWC dataset (https://mlcommons.org/en/multilingual-spoken-words/)
     for a few-shot class-incremental learning (FSCIL) task consisting of 200 voice commands keywords:
+
     - 100 base classes available for pre-training with:
         - 500 train samples
         - 100 validation samples
         - 100 test samples
     - 100 evaluation classes to do class-incremental learning on with 200 samples each.
 
     The subset of data used for this task, as well as the supporting files for base class and incremental
```

### Comparing `neurobench-1.0.3/neurobench/datasets/WISDM.py` & `neurobench-1.0.4/neurobench/datasets/WISDM.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/datasets/__init__.py` & `neurobench-1.0.4/neurobench/datasets/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,20 +17,14 @@
 
 def Gen4DetectionDataLoader(*args, **kwargs):
     return _lazy_import(
         "neurobench.datasets", ".megapixel_automotive", "Gen4DetectionDataLoader"
     )(*args, **kwargs)
 
 
-def DVSGesture(*args, **kwargs):
-    return _lazy_import("neurobench.datasets", ".dvs_gesture", "DVSGesture")(
-        *args, **kwargs
-    )
-
-
 def MackeyGlass(*args, **kwargs):
     return _lazy_import("neurobench.datasets", ".mackey_glass", "MackeyGlass")(
         *args, **kwargs
     )
 
 
 def WISDM(*args, **kwargs):
```

### Comparing `neurobench-1.0.3/neurobench/datasets/dataset.py` & `neurobench-1.0.4/neurobench/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/datasets/mackey_glass.py` & `neurobench-1.0.4/neurobench/datasets/mackey_glass.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/datasets/megapixel_automotive.py` & `neurobench-1.0.4/neurobench/datasets/megapixel_automotive.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/datasets/primate_reaching.py` & `neurobench-1.0.4/neurobench/datasets/primate_reaching.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self.url = "https://zenodo.org/record/583331/files/"
 
         self.md5s = {
             "indy_20170131_02.mat": "2790b1c869564afaa7772dbf9e42d784",
             "indy_20160630_01.mat": "197413a5339630ea926cbd22b8b43338",
             "indy_20160622_01.mat": "c33d5fff31320d709d23fe445561fb6e",
             "loco_20170301_05.mat": "47342da09f9c950050c9213c3df38ea3",
-            "loco_20170217_02.mat": "739b70762d838f3a1f358733c426bb02",
+            "loco_20170215_02.mat": "739b70762d838f3a1f358733c426bb02",
             "loco_20170210_03.mat": "4cae63b58c4cb9c8abd44929216c703b",
         }
 
         # The samples and labels of the dataset
         self.samples = None
         self.labels = None
 
@@ -220,15 +220,17 @@
         cursor_pos = dataset["cursor_pos"][()]
         target_pos = dataset["target_pos"][()]
         t = np.squeeze(dataset["t"][()])
         new_t = np.arange(t[0] - self.bin_width, t[-1], SAMPLING_RATE)
 
         # Define the segments' start & end indices
         self.start_end_indices = np.array(self.get_flag_index(target_pos))
-        self.time_segments = np.array(self.split_into_segments(self.start_end_indices))
+        self.time_segments = np.array(
+            self.split_into_segments(self.start_end_indices, target_pos.shape[1])
+        )
 
         spike_train = np.zeros((*spikes.shape, len(new_t)), dtype=np.int8)
 
         # iterate over hdf5 dataframe and preprocess data
         for row_idx, row in enumerate(spikes):
             for col_idx, element in enumerate(row):
                 # get indices of spikes and convert data to spike train
@@ -286,15 +288,16 @@
         )  # This is no of segments in each chunk
         stride = int(self.stride / SAMPLING_RATE)
         # print(total_segments, sub_length)
 
         train_len = math.floor(self.train_ratio * sub_length)
         val_len = math.floor((sub_length - train_len) / 2)
 
-        offset = int(np.round(self.bin_width / SAMPLING_RATE)) * self.num_steps
+        # offset = int(np.round(self.bin_width / SAMPLING_RATE)) * self.num_steps
+        offset = 0
 
         # split the data into 4 equal parts
         # for each part, split the data according to training, testing and validation split
         for split_no in range(split_num):
             for i in range(sub_length):
                 # Each segment's Dimension is: No_of_Probes * No_of_Recording
                 if i < train_len and i in self.valid_segments:
@@ -327,16 +330,18 @@
         max_segment_length."""
         return np.nonzero(
             self.time_segments[:, 1] - self.time_segments[:, 0]
             < self.max_segment_length
         )[0]
 
     @staticmethod
-    def split_into_segments(indices):
+    def split_into_segments(indices, last_idx):
         """Combine the start and end index into a NumPy array."""
+        indices = np.insert(indices, 0, 0)
+        indices = np.append(indices, [last_idx])
         start_end = np.array([indices[:-1], indices[1:]])
 
         return np.transpose(start_end)
 
     @staticmethod
     def get_flag_index(target_pos):
         """Find where each segment begins and ends."""
```

### Comparing `neurobench-1.0.3/neurobench/datasets/speech_commands.py` & `neurobench-1.0.4/neurobench/datasets/speech_commands.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/datasets/utils.py` & `neurobench-1.0.4/neurobench/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/models/model.py` & `neurobench-1.0.4/neurobench/models/model.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/models/snntorch_models.py` & `neurobench-1.0.4/neurobench/models/snntorch_models.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/models/torch_model.py` & `neurobench-1.0.4/neurobench/models/torch_model.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/postprocessing/postprocessor.py` & `neurobench-1.0.4/neurobench/postprocessing/postprocessor.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/preprocessing/mfcc.py` & `neurobench-1.0.4/neurobench/preprocessing/mfcc.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/preprocessing/preprocessor.py` & `neurobench-1.0.4/neurobench/preprocessing/preprocessor.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/preprocessing/speech2spikes.py` & `neurobench-1.0.4/neurobench/preprocessing/speech2spikes.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/neurobench/utils.py` & `neurobench-1.0.4/neurobench/utils.py`

 * *Files identical despite different names*

### Comparing `neurobench-1.0.3/pyproject.toml` & `neurobench-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurobench"
-version = "1.0.3"
+version = "1.0.4"
 description = "Collaborative, Fair, and Representative Benchmarks for Neuromorphic Computing"
 authors = ["NeuroBench Team <neurobench@googlegroups.com>"]
 readme = "README.rst"
 exclude = ["docs", "tests", "neurobench/examples"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `neurobench-1.0.3/setup.py` & `neurobench-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 extras_require = \
 {'mackey-glass': ['jitcdde>=1.8.1,<2.0.0'],
  'nehar': ['pytorch-lightning>=1.4.0,<2.0.0', 'gdown>=4.7.1,<5.0.0']}
 
 setup_kwargs = {
     'name': 'neurobench',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'Collaborative, Fair, and Representative Benchmarks for Neuromorphic Computing',
     'long_description': "============\nIntroduction\n============\n\nA harness for running evaluations on\n`NeuroBench <https://neurobench.ai>`__ algorithm benchmarks.\n\nNeuroBench is a community-driven project, and we welcome further\ndevelopment from the community. If you are interested in developing\nextensions to features, programming frameworks, or metrics and tasks,\nplease see the `Contributing Guidelines <https://neurobench.readthedocs.io/en/latest/contributing.html>`__.\n\nNeuroBench Structure\n---------------------\n\nNeuroBench contains the following sections:\n\n.. list-table:: \n   :widths: 20 60\n\n   * - **Section**\n     - **Description**\n   * - `neurobench.benchmarks <https://neurobench.readthedocs.io/en/latest/neurobench.benchmarks.html>`__\n     - Neurobench benchmarks, including data metrics and static metrics\n   * - `neurobench.datasets <https://neurobench.readthedocs.io/en/latest/neurobench.datasets.html>`__\n     - Neurobench benchmark datasets\n   * - `neurobench.models <https://neurobench.readthedocs.io/en/latest/neurobench.models.html>`__\n     - Neurobench framework for Torch and SNNTorch models\n   * - `neurobench.preprocessing <https://neurobench.readthedocs.io/en/latest/neurobench.preprocessing.html>`__\n     - Pre-processing of data, conversion to spikes\n   * - `neurobench.postprocessing <https://neurobench.readthedocs.io/en/latest/neurobench.postprocessing.html>`__\n     - Post-processors take the spiking output from the models and provide several methods of combining them\n\nInstallation\n------------\n\nInstall from PyPI:\n\n::\n\n   pip install neurobench\n\nBenchmarks\n----------\n\nThe following benchmarks are currently available:\n\nv1.0 benchmarks\n~~~~~~~~~~~~~~~\n- Keyword Few-shot Class-incremental Learning (FSCIL)\n- Event Camera Object Detection\n- Non-human Primate (NHP) Motor Prediction\n- Chaotic Function Prediction\n\nAdditional benchmarks\n~~~~~~~~~~~~~~~~~~~~~\n- DVS Gesture Recognition\n- Google Speech Commands (GSC) Classification\n- Neuromorphic Human Activity Recognition (HAR)\n\nGetting started\n---------------\n\nExample benchmark scripts can be found under the ``neurobench/examples`` folder. \n(`https://github.com/NeuroBench/neurobench/tree/main/neurobench/examples/ <https://github.com/NeuroBench/neurobench/tree/main/neurobench/examples/>`__)\n\nIn general, the design flow for using the framework is as follows:\n\n1. Train a network using the train split from a particular dataset.\n2. Wrap the network in a ``NeuroBenchModel``.\n3. Pass the model, evaluation split dataloader, pre-/post-processors,\n   and a list of metrics to the ``Benchmark`` and ``run()``.\n\nDocumentation for the framework interfaces can found in the `API Overview <https://neurobench.readthedocs.io/en/latest/api.html>`__.\n\nDevelopment\n-----------\n\nIf you clone the repo directly for development, `poetry <https://pypi.org/project/poetry/>`__ \ncan be used to maintain a virtualenv consistent with a deployment environment. In the\nroot directory run:\n\n::\n\n   pip install poetry\n   poetry install\n\nPoetry requires python >=3.9. Installation should not take more than a few minutes.\n\nEnd-to-end examples can be run from the poetry environment. As a demo, try the \nGoogle Speech Commands keyword classification benchmark:\n\n::\n\n   # ANN Benchmark Example\n   poetry run python neurobench/examples/gsc/benchmark_ann.py\n   \n   # Expected results:\n   # {'footprint': 109228, 'connection_sparsity': 0.0,\n   # 'classification_accuracy': 0.8653339397251905, 'activation_sparsity': 0.3854464619019532, \n   # 'synaptic_operations': {'Effective_MACs': 1749994.1556565198, 'Effective_ACs': 0.0, 'Dense': 1902179.0}}\n\n\n   # SNN Benchmark Example\n   poetry run python neurobench/examples/gsc/benchmark_snn.py\n   \n   # Expected results:\n   # {'footprint': 583900, 'connection_sparsity': 0.0,\n   # 'classification_accuracy': 0.8484325295196562, 'activation_sparsity': 0.9675956131759854, \n   # 'synaptic_operations': {'Effective_MACs': 0.0, 'Effective_ACs': 3556689.9895502045, 'Dense': 29336955.0}}\n\nThese demos should download the dataset, then run in a couple minutes. Other baseline result scripts and notebook\ntutorials are available in the ``neurobench/examples`` folder.\n\nDevelopers\n----------\n\nNeuroBench is a collaboration between industry and academic engineers\nand researchers. This framework is currently maintained by `Jason\nYik <https://www.linkedin.com/in/jasonlyik/>`__, `Noah\nPacik-Nelson <https://www.linkedin.com/in/noah-pacik-nelson/>`__, and\n`Korneel Van den\nBerghe <https://www.linkedin.com/in/korneel-van-den-berghe/>`__, and\nthere have been technical contributions from many others. A\nnon-exhaustive list includes Gregor Lenz, Denis Kleyko, Younes\nBouhadjar, Paul Hueber, Vincent Sun, Biyan Zhou, George Vathakkattil\nJoseph, Douwe den Blanken, Maxime Fabre, Shenqi Wang, Guangzhi Tang,\nAnurag Kumar Mishra, Soikat Hasan Ahmed, Benedetto Leto, Aurora Micheli,\nTao Sun.\n\nContributing\n------------\n\nIf you are interested in helping to build this framework, please see the\n`Contribution Guidelines <https://neurobench.readthedocs.io/en/latest/contributing.html>`__.\n\nCitation\n--------\n\nIf you use this framework in your research, please cite the following\npreprint article:\n\n::\n\n   @misc{yik2024neurobench,\n      title={NeuroBench: A Framework for Benchmarking Neuromorphic Computing Algorithms and Systems}, \n      author={Jason Yik and Korneel Van den Berghe and Douwe den Blanken and Younes Bouhadjar and Maxime Fabre and Paul Hueber and Denis Kleyko and Noah Pacik-Nelson and Pao-Sheng Vincent Sun and Guangzhi Tang and Shenqi Wang and Biyan Zhou and Soikat Hasan Ahmed and George Vathakkattil Joseph and Benedetto Leto and Aurora Micheli and Anurag Kumar Mishra and Gregor Lenz and Tao Sun and Zergham Ahmed and Mahmoud Akl and Brian Anderson and Andreas G. Andreou and Chiara Bartolozzi and Arindam Basu and Petrut Bogdan and Sander Bohte and Sonia Buckley and Gert Cauwenberghs and Elisabetta Chicca and Federico Corradi and Guido de Croon and Andreea Danielescu and Anurag Daram and Mike Davies and Yigit Demirag and Jason Eshraghian and Tobias Fischer and Jeremy Forest and Vittorio Fra and Steve Furber and P. Michael Furlong and William Gilpin and Aditya Gilra and Hector A. Gonzalez and Giacomo Indiveri and Siddharth Joshi and Vedant Karia and Lyes Khacef and James C. Knight and Laura Kriener and Rajkumar Kubendran and Dhireesha Kudithipudi and Yao-Hong Liu and Shih-Chii Liu and Haoyuan Ma and Rajit Manohar and Josep Maria Margarit-Taulé and Christian Mayr and Konstantinos Michmizos and Dylan Muir and Emre Neftci and Thomas Nowotny and Fabrizio Ottati and Ayca Ozcelikkale and Priyadarshini Panda and Jongkil Park and Melika Payvand and Christian Pehle and Mihai A. Petrovici and Alessandro Pierro and Christoph Posch and Alpha Renner and Yulia Sandamirskaya and Clemens JS Schaefer and André van Schaik and Johannes Schemmel and Samuel Schmidgall and Catherine Schuman and Jae-sun Seo and Sadique Sheik and Sumit Bam Shrestha and Manolis Sifalakis and Amos Sironi and Matthew Stewart and Kenneth Stewart and Terrence C. Stewart and Philipp Stratmann and Jonathan Timcheck and Nergis Tömen and Gianvito Urgese and Marian Verhelst and Craig M. Vineyard and Bernhard Vogginger and Amirreza Yousefzadeh and Fatima Tuz Zohora and Charlotte Frenkel and Vijay Janapa Reddi},\n      year={2024},\n      eprint={2304.04640},\n      archivePrefix={arXiv},\n      primaryClass={cs.AI}\n   }\n",
     'author': 'NeuroBench Team',
     'author_email': 'neurobench@googlegroups.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `neurobench-1.0.3/PKG-INFO` & `neurobench-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurobench
-Version: 1.0.3
+Version: 1.0.4
 Summary: Collaborative, Fair, and Representative Benchmarks for Neuromorphic Computing
 Author: NeuroBench Team
 Author-email: neurobench@googlegroups.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

