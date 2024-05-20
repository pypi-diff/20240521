# Comparing `tmp/mnistvit-1.0.0.tar.gz` & `tmp/mnistvit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnistvit-1.0.0.tar", last modified: Sat May 18 21:02:00 2024, max compression
+gzip compressed data, was "mnistvit-1.0.1.tar", last modified: Mon May 20 22:24:13 2024, max compression
```

## Comparing `mnistvit-1.0.0.tar` & `mnistvit-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-18 21:02:00.940983 mnistvit-1.0.0/
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    35149 2024-02-19 12:26:31.000000 mnistvit-1.0.0/LICENSE
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42823 2024-05-18 21:02:00.940983 mnistvit-1.0.0/PKG-INFO
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)     1376 2024-05-18 16:16:44.000000 mnistvit-1.0.0/README.md
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)      962 2024-05-15 20:03:28.000000 mnistvit-1.0.0/pyproject.toml
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       38 2024-05-18 21:02:00.940983 mnistvit-1.0.0/setup.cfg
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-18 21:02:00.940983 mnistvit-1.0.0/src/
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-18 21:02:00.940983 mnistvit-1.0.0/src/mnistvit/
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)      187 2024-02-19 12:31:36.000000 mnistvit-1.0.0/src/mnistvit/__init__.py
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       34 2024-05-15 20:32:01.000000 mnistvit-1.0.0/src/mnistvit/__main__.py
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)     7641 2024-05-18 13:53:34.000000 mnistvit-1.0.0/src/mnistvit/model.py
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)     7311 2024-05-18 17:54:04.000000 mnistvit-1.0.0/src/mnistvit/predict.py
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)     4218 2024-05-16 18:45:53.000000 mnistvit-1.0.0/src/mnistvit/preprocess.py
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    11231 2024-05-18 20:22:51.000000 mnistvit-1.0.0/src/mnistvit/train.py
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)     8176 2024-05-18 20:42:35.000000 mnistvit-1.0.0/src/mnistvit/tune.py
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)     1283 2024-05-14 18:51:42.000000 mnistvit-1.0.0/src/mnistvit/utils.py
-drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-18 21:02:00.940983 mnistvit-1.0.0/src/mnistvit.egg-info/
--rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42823 2024-05-18 21:02:00.000000 mnistvit-1.0.0/src/mnistvit.egg-info/PKG-INFO
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      399 2024-05-18 21:02:00.000000 mnistvit-1.0.0/src/mnistvit.egg-info/SOURCES.txt
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        1 2024-05-18 21:02:00.000000 mnistvit-1.0.0/src/mnistvit.egg-info/dependency_links.txt
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       43 2024-05-18 21:02:00.000000 mnistvit-1.0.0/src/mnistvit.egg-info/requires.txt
--rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        9 2024-05-18 21:02:00.000000 mnistvit-1.0.0/src/mnistvit.egg-info/top_level.txt
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.124329 mnistvit-1.0.1/
+-rw-r--r--   0 asnelt    (1000) asnelt    (1000)    35149 2024-02-19 12:26:31.000000 mnistvit-1.0.1/LICENSE
+-rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42823 2024-05-20 22:24:13.124329 mnistvit-1.0.1/PKG-INFO
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     1376 2024-05-20 21:08:59.000000 mnistvit-1.0.1/README.md
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      962 2024-05-20 22:22:44.000000 mnistvit-1.0.1/pyproject.toml
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       38 2024-05-20 22:24:13.124329 mnistvit-1.0.1/setup.cfg
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.120329 mnistvit-1.0.1/src/
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.124329 mnistvit-1.0.1/src/mnistvit/
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      187 2024-05-20 21:07:20.000000 mnistvit-1.0.1/src/mnistvit/__init__.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       34 2024-05-20 21:08:56.000000 mnistvit-1.0.1/src/mnistvit/__main__.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     7629 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/model.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     7297 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/predict.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     4247 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/preprocess.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)    11772 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/train.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     8182 2024-05-20 21:09:01.000000 mnistvit-1.0.1/src/mnistvit/tune.py
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)     1283 2024-05-20 21:08:52.000000 mnistvit-1.0.1/src/mnistvit/utils.py
+drwxrwxr-x   0 asnelt    (1000) asnelt    (1000)        0 2024-05-20 22:24:13.124329 mnistvit-1.0.1/src/mnistvit.egg-info/
+-rw-r--r--   0 asnelt    (1000) asnelt    (1000)    42823 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/PKG-INFO
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)      399 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/SOURCES.txt
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        1 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/dependency_links.txt
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)       43 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/requires.txt
+-rw-rw-r--   0 asnelt    (1000) asnelt    (1000)        9 2024-05-20 22:24:13.000000 mnistvit-1.0.1/src/mnistvit.egg-info/top_level.txt
```

### Comparing `mnistvit-1.0.0/LICENSE` & `mnistvit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.0/PKG-INFO` & `mnistvit-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnistvit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A vision transformer for training on MNIST
 Author-email: Arno Onken <asnelt@asnelt.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mnistvit-1.0.0/README.md` & `mnistvit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.0/pyproject.toml` & `mnistvit-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnistvit"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name = "Arno Onken", email = "asnelt@asnelt.org"}]
 description = "A vision transformer for training on MNIST"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.10"
 dependencies = [
     "torch",
```

### Comparing `mnistvit-1.0.0/src/mnistvit/model.py` & `mnistvit-1.0.1/src/mnistvit/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from math import prod
 from numbers import Number
-from typing import Dict, List, Literal
+from typing import Literal
 
 from torch import Tensor, cat, nn, randn
 
 
 class VisionTransformer(nn.Module):
     """Configurable vision transformer (ViT).
 
@@ -28,22 +28,22 @@
         head_activation (str, optional): MLP head activation function string, `'relu'`,
             `'gelu'` or `'tanh'`.  Default: `'gelu'`.
     """
 
     def __init__(
         self,
         num_channels: int,
-        input_sizes: List[int],
+        input_sizes: list[int],
         output_size: int,
         patch_size: int,
         num_heads: int,
         latent_size_multiplier: int,
         num_layers: int,
         encoder_size: int,
-        head_size: int | List[int],
+        head_size: int | list[int],
         dropout: float = 0,
         encoder_activation: Literal["relu", "gelu"] = "gelu",
         head_activation: Literal["relu", "gelu", "tanh"] = "gelu",
     ) -> None:
         super().__init__()
         self.kwargs = {
             "num_channels": num_channels,
@@ -107,15 +107,15 @@
         latent_size (int): Size of the embedding.
         dropout (float, optional): Dropout probability.  Default: 0.
     """
 
     def __init__(
         self,
         num_channels: int,
-        input_sizes: List[int],
+        input_sizes: list[int],
         patch_size: int,
         latent_size: int,
         dropout: float = 0,
     ) -> None:
         super().__init__()
         # Use Unfold to split the input image into patches
         self.unfold = nn.Unfold(kernel_size=patch_size, stride=patch_size)
@@ -156,16 +156,16 @@
             `'tanh'`.  Default: `'relu'`.
     """
 
     def __init__(
         self,
         input_size: int,
         output_size: int,
-        hidden_sizes: List[int] = None,
-        dropout: float | List[float] = None,
+        hidden_sizes: list[int] = None,
+        dropout: float | list[float] = None,
         activation: Literal["relu", "gelu", "tanh"] = "relu",
     ) -> None:
         super().__init__()
         self.flatten = nn.Flatten()
         if hidden_sizes is None:
             hidden_sizes = []
         layers = [
```

### Comparing `mnistvit-1.0.0/src/mnistvit/predict.py` & `mnistvit-1.0.1/src/mnistvit/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import argparse
-from typing import Dict
 
 import torch
 
 from .preprocess import get_test_loader_mnist, read_digit_image
 from .utils import FILE_LIKE, load_model
 
 
 def test_mnist(
-    config: Dict,
+    config: dict[str, int],
     data_dir: str,
     model_file: FILE_LIKE,
     use_loss: bool = True,
     use_accuracy: bool = True,
     device: torch.device = "cpu",
 ) -> None:
     """Loads a model, tests it on MNIST and prints the results.
```

### Comparing `mnistvit-1.0.0/src/mnistvit/preprocess.py` & `mnistvit-1.0.1/src/mnistvit/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from typing import Tuple
-
 import torch
 from torch.utils.data import DataLoader, random_split
 from torchvision import datasets, transforms
 from torchvision.io import ImageReadMode, read_image
 
 from .utils import FILE_LIKE
 
 
 def preprocess_mnist(
     data_dir: str, train: bool, use_augmentation: bool = False
-) -> Tuple:
+) -> torch.utils.data.dataset.Dataset:
     """Preprocesses the MNIST dataset.
 
     Normalizes the MNIST dataset with training mean and variance and eventually
     augments the dataset with random affine transformations.
 
     Args:
         data_dir (str): Directory of the MNIST dataset.
         train (bool): If true, loads the training set, else the test set.
         use_augmentation (bool, optional): If true, augments the dataset with random
             affine transformations.  Default: `False`.
 
     Returns:
-        tuple: Image, target pairs.
+        torch.utils.data.dataset.Dataset: Image, target pairs.
     """
     transform = transforms.Compose(
         [transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))]
     )
     if use_augmentation:
         # Data augmentation
         transform = transforms.Compose(
@@ -43,15 +41,15 @@
 
 
 def get_train_loaders_mnist(
     data_dir: str,
     batch_size: int,
     train_fraction: float = 1.0,
     use_augmentation: bool = True,
-) -> Tuple:
+) -> tuple[DataLoader, DataLoader]:
     """Training loaders of the MNIST dataset.
 
     Args:
         data_dir (str): Directory of the MNIST dataset.
         batch_size (int): Size of the batches of the training loaders.
         train_fraction (float, optional): Fraction of the set used for the training
             loader.  The remainder is used for the validation loader.  Default: 1.0.
@@ -74,17 +72,15 @@
             dataset, [num_train, len(dataset) - num_train]
         )
         train_loader = DataLoader(train_set, **loader_kwargs)
         val_loader = DataLoader(val_set, **loader_kwargs)
     return train_loader, val_loader
 
 
-def get_test_loader_mnist(
-    data_dir: str, batch_size: int
-) -> torch.utils.data.DataLoader:
+def get_test_loader_mnist(data_dir: str, batch_size: int) -> DataLoader:
     """Test loader of the MNIST dataset.
 
     Args:
         data_dir (str): Directory of the MNIST dataset.
         batch_size (int): Size of the batches of the test loader.
 
     Returns:
```

### Comparing `mnistvit-1.0.0/src/mnistvit/train.py` & `mnistvit-1.0.1/src/mnistvit/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import argparse
-from typing import Callable, Dict
+from typing import Any, Callable
 
 import torch
 
 from .model import VisionTransformer
 from .predict import prediction_loss
 from .preprocess import get_train_loaders_mnist
 from .utils import FILE_LIKE, save_model
 
 
 def train_mnist(
-    config: Dict,
+    config: dict[str, int | float | list[int]],
     data_dir: str,
     use_validation: bool = True,
     use_augmentation: bool = True,
     model_file: FILE_LIKE = None,
-    report_fn: Callable = None,
-    resume_states: Dict = None,
+    report_fn: Callable[
+        [
+            int,
+            float,
+            float,
+            torch.nn.Module,
+            torch.optim.Optimizer,
+            torch.optim.lr_scheduler.LRScheduler,
+        ],
+        None,
+    ] = None,
+    resume_states: dict[str, int | dict[str, Any]] = None,
     device: torch.device = "cpu",
 ) -> None:
     """Trains a single model on MNIST and eventually saves the model.
 
     Args:
         config (dict): Training configuration including `'batch_size'`, `'num_epochs'`,
             `'lr'`, `'weight_decay'`, `'epoch_lr_restart'`, `'patch_size'`,
@@ -68,15 +78,17 @@
         resume_states,
         device,
     )
     if model_file is not None:
         save_model(model, model_file)
 
 
-def init_mnist_model(config: Dict, device: torch.device = "cpu") -> torch.nn.Module:
+def init_mnist_model(
+    config: dict[str, int | float | list[int]], device: torch.device = "cpu"
+) -> torch.nn.Module:
     """Initializes a vision transformer for training on MNIST.
 
     Args:
         config (dict): Training configuration including `'patch_size'`, `'num_heads'`,
             `'latent_size_multiplier'`, `'num_layers'`, `'encoder_size'`, `'head_size'`
             and `'dropout'`.
         device (torch.device, optional): Device to load the model on.
@@ -105,16 +117,26 @@
     train_loader: torch.utils.data.DataLoader,
     loss_fn: torch.nn.Module,
     num_epochs: int,
     lr: float,
     weight_decay: float,
     epoch_lr_restart: int,
     val_loader: torch.utils.data.DataLoader = None,
-    report_fn: Callable = None,
-    resume_states: Dict = None,
+    report_fn: Callable[
+        [
+            int,
+            float,
+            float,
+            torch.nn.Module,
+            torch.optim.Optimizer,
+            torch.optim.lr_scheduler.LRScheduler,
+        ],
+        None,
+    ] = None,
+    resume_states: dict[str, int | dict[str, Any]] = None,
     device: torch.device = "cpu",
 ) -> None:
     """Main training function for model training.
 
     Initializes an optimizer and learning rate scheduler, contains the loop over epochs
     and eventually evaluates validation performance.
```

### Comparing `mnistvit-1.0.0/src/mnistvit/tune.py` & `mnistvit-1.0.1/src/mnistvit/tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import argparse
 import os
 from tempfile import TemporaryDirectory
-from typing import Dict
 
 import torch
 from ray import train, tune
 from ray.tune.schedulers import ASHAScheduler
 from ray.tune.search.optuna import OptunaSearch
 
 from .train import init_mnist_model, train_mnist
 from .utils import FILE_LIKE, save_model
 
 
-def objective(config: Dict, data_dir: str) -> None:
+def objective(config: dict[str, int | float], data_dir: str) -> None:
     """Objective function for hyperparameter tuning.
 
     Trains a model on MNIST according to the configuration and reports the mean loss.
     Also saves checkpoints to `'checkpoint.pt'` files.  Checkpoints contain model,
     optimizer and learning rate scheduler states as well as `'epoch'` metadata.
 
     Args:
@@ -76,15 +75,15 @@
 
 def fit(
     exp_name: str,
     storage_path: str,
     num_samples: int,
     num_epochs: int,
     model_file: FILE_LIKE,
-    resources: Dict = None,
+    resources: dict[str, float] = None,
 ) -> None:
     """Tunes hyperparameters of a model to MNIST.
 
     Selects the checkpoint with the best validation performance and prints the best
     result and the best checkpoint metadata.  The best model is then saved to the
     provided model file name.
```

### Comparing `mnistvit-1.0.0/src/mnistvit/utils.py` & `mnistvit-1.0.1/src/mnistvit/utils.py`

 * *Files identical despite different names*

### Comparing `mnistvit-1.0.0/src/mnistvit.egg-info/PKG-INFO` & `mnistvit-1.0.1/src/mnistvit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnistvit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A vision transformer for training on MNIST
 Author-email: Arno Onken <asnelt@asnelt.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

