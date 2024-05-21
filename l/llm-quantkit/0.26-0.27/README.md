# Comparing `tmp/llm_quantkit-0.26.tar.gz` & `tmp/llm_quantkit-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_quantkit-0.26.tar", last modified: Wed Apr 24 12:02:24 2024, max compression
+gzip compressed data, was "llm_quantkit-0.27.tar", last modified: Tue May 21 06:05:08 2024, max compression
```

## Comparing `llm_quantkit-0.26.tar` & `llm_quantkit-0.27.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:02:24.656302 llm_quantkit-0.26/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 12:02:13.000000 llm_quantkit-0.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-24 12:02:24.656302 llm_quantkit-0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-24 12:02:13.000000 llm_quantkit-0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:02:24.656302 llm_quantkit-0.26/llm_quantkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 12:02:24.000000 llm_quantkit-0.26/llm_quantkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 12:02:13.000000 llm_quantkit-0.26/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:02:24.656302 llm_quantkit-0.26/quantkit/
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15984 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/quantkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-24 12:02:13.000000 llm_quantkit-0.26/quantkit/safetensor.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:02:24.656302 llm_quantkit-0.26/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:05:08.000717 llm_quantkit-0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-21 06:04:58.000000 llm_quantkit-0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-21 06:05:08.000717 llm_quantkit-0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-21 06:04:58.000000 llm_quantkit-0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:05:08.000717 llm_quantkit-0.27/llm_quantkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-21 06:05:07.000000 llm_quantkit-0.27/llm_quantkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 06:05:07.000000 llm_quantkit-0.27/llm_quantkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 06:05:07.000000 llm_quantkit-0.27/llm_quantkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 06:05:07.000000 llm_quantkit-0.27/llm_quantkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-21 06:05:07.000000 llm_quantkit-0.27/llm_quantkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 06:05:07.000000 llm_quantkit-0.27/llm_quantkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-21 06:04:58.000000 llm_quantkit-0.27/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 06:05:08.000717 llm_quantkit-0.27/quantkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-21 06:04:58.000000 llm_quantkit-0.27/quantkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71261 2024-05-21 06:04:58.000000 llm_quantkit-0.27/quantkit/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113763 2024-05-21 06:04:58.000000 llm_quantkit-0.27/quantkit/convert_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-21 06:04:58.000000 llm_quantkit-0.27/quantkit/quantkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-21 06:04:58.000000 llm_quantkit-0.27/quantkit/safetensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 06:05:08.000717 llm_quantkit-0.27/setup.cfg
```

### Comparing `llm_quantkit-0.26/LICENSE` & `llm_quantkit-0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.26/PKG-INFO` & `llm_quantkit-0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.26
+Version: 0.27
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `llm_quantkit-0.26/README.md` & `llm_quantkit-0.27/README.md`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.26/llm_quantkit.egg-info/PKG-INFO` & `llm_quantkit-0.27/llm_quantkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.26
+Version: 0.27
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `llm_quantkit-0.26/pyproject.toml` & `llm_quantkit-0.27/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-quantkit"
 description = "cli tool for downloading and quantizing LLMs"
 readme = "README.md"
 license = { text = "MIT License" }
-version = "0.26"
+version = "0.27"
 authors = [{ name = "xhedit", email = "jevd@protonmail.com" }]
 dependencies = [
     "click",
     "torch>=2.0.0",
     "einops",
     "tqdm",
     "transformers",
```

### Comparing `llm_quantkit-0.26/quantkit/cli.py` & `llm_quantkit-0.27/quantkit/cli.py`

 * *Files identical despite different names*

### Comparing `llm_quantkit-0.26/quantkit/convert.py` & `llm_quantkit-0.27/quantkit/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
+import logging
 import argparse
 import concurrent.futures
 import enum
 import faulthandler
 import functools
 import itertools
 import json
@@ -19,25 +20,27 @@
 import textwrap
 import time
 import zipfile
 from abc import ABC, abstractmethod
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, IO, Iterable, Literal, Protocol, TypeVar, runtime_checkable
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, IO, Iterable, Literal, Protocol, TypeVar, runtime_checkable, Optional
 
 import numpy as np
 from sentencepiece import SentencePieceProcessor
 
 if 'NO_LOCAL_GGUF' not in os.environ:
     sys.path.insert(1, str(Path(__file__).parent / 'gguf-py'))
 import gguf
 
 if TYPE_CHECKING:
-    from typing import TypeAlias
+    from typing_extensions import Self, TypeAlias
+
+logger = logging.getLogger("convert")
 
 if hasattr(faulthandler, 'register') and hasattr(signal, 'SIGUSR1'):
     faulthandler.register(signal.SIGUSR1)
 
 NDArray: TypeAlias = 'np.ndarray[Any, Any]'
 
 ARCH = gguf.MODEL_ARCH.LLAMA
@@ -135,15 +138,16 @@
     MostlyF16  = 1  # except 1d tensors
     MostlyQ8_0 = 7  # except 1d tensors
 
     def type_for_tensor(self, name: str, tensor: LazyTensor) -> DataType:
         dt = GGML_FILE_TYPE_TO_DATA_TYPE.get(self)
         if dt is None:
             raise ValueError(self)
-        # 1D tensors are always F32.
+        # Convert all 1D tensors to F32.  Most of the codebase that takes in 1D tensors only handles F32 tensors, and most of the outputs tensors are F32.
+        #  Also The 1d tensors aren't much of a performance/size issue.  So instead of having to have separate F32 and F16 implementations of both, just convert everything to F32 for now.
         return dt if len(tensor.shape) > 1 else DT_F32
 
 
 GGML_FILE_TYPE_TO_DATA_TYPE: dict[GGMLFileType, DataType] = {
     GGMLFileType.AllF32    : DT_F32,
     GGMLFileType.MostlyF16 : DT_F16,
     GGMLFileType.MostlyQ8_0: DT_Q8_0,
@@ -276,14 +280,15 @@
     def loadOriginalParamsJson(model: LazyModel, config_path: Path) -> Params:
         with open(config_path) as f:
             config = json.load(f)
 
         n_experts      = None
         n_experts_used = None
         f_rope_freq_base = None
+        n_ff = None
 
         # hack to determine LLaMA v1 vs v2 vs CodeLlama
         if config.get("moe"):
             # Mixtral
             n_ctx = 32768
         elif config.get("rope_theta") == 1000000:
             # CodeLlama
@@ -300,14 +305,16 @@
 
         if config.get("moe"):
             n_ff = model["layers.0.feed_forward.experts.0.w1.weight"].shape[0]
             n_experts      = config["moe"]["num_experts"]
             n_experts_used = config["moe"]["num_experts_per_tok"]
             f_rope_freq_base = 1e6
 
+        assert n_ff is not None
+
         return Params(
             n_vocab          = model["tok_embeddings.weight"].shape[0],
             n_embd           = config["dim"],
             n_layer          = config["n_layers"],
             n_ctx            = n_ctx,
             n_ff             = n_ff,
             n_head           = (n_head := config["n_heads"]),
@@ -333,18 +340,55 @@
             raise ValueError('Cannot guess params when model format is none')
 
         params.path_model = model_plus.paths[0].parent
 
         return params
 
 
+@dataclass
+class Metadata:
+    name: Optional[str] = None
+    author: Optional[str] = None
+    version: Optional[str] = None
+    url: Optional[str] = None
+    description: Optional[str] = None
+    licence: Optional[str] = None
+    source_url: Optional[str] = None
+    source_hf_repo: Optional[str] = None
+
+    @staticmethod
+    def load(metadata_path: Path) -> Metadata:
+        if metadata_path is None or not metadata_path.exists():
+            return Metadata()
+
+        with open(metadata_path, 'r') as file:
+            data = json.load(file)
+
+        # Create a new Metadata instance
+        metadata = Metadata()
+
+        # Assigning values to Metadata attributes if they exist in the JSON file
+        # This is based on LLM_KV_NAMES mapping in llama.cpp
+        metadata.name = data.get("general.name")
+        metadata.author = data.get("general.author")
+        metadata.version = data.get("general.version")
+        metadata.url = data.get("general.url")
+        metadata.description = data.get("general.description")
+        metadata.license = data.get("general.license")
+        metadata.source_url = data.get("general.source.url")
+        metadata.source_hf_repo = data.get("general.source.huggingface.repository")
+
+        return metadata
+
+
 #
 # vocab
 #
 
+
 @runtime_checkable
 class BaseVocab(Protocol):
     tokenizer_model: ClassVar[str]
     name: ClassVar[str]
 
 
 class NoVocab(BaseVocab):
@@ -454,15 +498,16 @@
                     added_tokens = json.load(f)
             except FileNotFoundError:
                 pass
         elif not (fname_tokenizer := base_path.parent / 'tokenizer.model').exists():
             # not found in alternate location either
             raise FileNotFoundError('Cannot find tokenizer.model')
 
-        self.sentencepiece_tokenizer = SentencePieceProcessor(str(fname_tokenizer))
+        self.sentencepiece_tokenizer = SentencePieceProcessor()
+        self.sentencepiece_tokenizer.LoadFromFile(str(fname_tokenizer))
         vocab_size = self.sentencepiece_tokenizer.vocab_size()
 
         new_tokens       = {id: piece for piece, id in added_tokens.items() if id >= vocab_size}
         expected_new_ids = list(range(vocab_size, vocab_size + len(new_tokens)))
         actual_new_ids   = sorted(new_tokens.keys())
 
         if expected_new_ids != actual_new_ids:
@@ -474,31 +519,31 @@
         self.vocab_size_base    = vocab_size
         self.vocab_size         = self.vocab_size_base + len(self.added_tokens_list)
         self.fname_tokenizer    = fname_tokenizer
 
     def sentencepiece_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]:
         tokenizer = self.sentencepiece_tokenizer
         for i in range(tokenizer.vocab_size()):
-            piece = tokenizer.id_to_piece(i)
+            piece = tokenizer.IdToPiece(i)
             text         = piece.encode("utf-8")
-            score: float = tokenizer.get_score(i)
+            score: float = tokenizer.GetScore(i)
 
             toktype = gguf.TokenType.NORMAL
-            if tokenizer.is_unknown(i):
+            if tokenizer.IsUnknown(i):
                 toktype = gguf.TokenType.UNKNOWN
-            if tokenizer.is_control(i):
+            if tokenizer.IsControl(i):
                 toktype = gguf.TokenType.CONTROL
 
             # NOTE: I think added_tokens are user defined.
             # ref: https://github.com/google/sentencepiece/blob/master/src/sentencepiece_model.proto
             # if tokenizer.is_user_defined(i): toktype = gguf.TokenType.USER_DEFINED
 
-            if tokenizer.is_unused(i):
+            if tokenizer.IsUnused(i):
                 toktype = gguf.TokenType.UNUSED
-            if tokenizer.is_byte(i):
+            if tokenizer.IsByte(i):
                 toktype = gguf.TokenType.BYTE
 
             yield text, score, toktype
 
     def added_tokens(self) -> Iterable[tuple[bytes, float, gguf.TokenType]]:
         for text in self.added_tokens_list:
             score = -1000.0
@@ -512,25 +557,30 @@
         return f"<SentencePieceVocab with {self.vocab_size_base} base tokens and {len(self.added_tokens_list)} added tokens>"
 
 
 class LlamaHfVocab(Vocab):
     tokenizer_model = "llama"
     name = "hfft"
 
-    def __init__(self, base_path: Path, ignore_nonllama: bool = False):
+    def __init__(self, base_path: Path):
         fname_tokenizer = base_path / FAST_TOKENIZER_FILE
         # if this fails, FileNotFoundError propagates to caller
         with open(fname_tokenizer, encoding='utf-8') as f:
             tokenizer_json = json.load(f)
 
         # pre-check so we know if we need transformers
         tokenizer_model: dict[str, Any] = tokenizer_json['model']
-        if ignore_nonllama:
-            pass  # workaround incorrect use of this class for WordPiece
-        elif (
+        is_llama3 = (
+            tokenizer_model['type'] == 'BPE' and tokenizer_model.get('ignore_merges', False)
+            and not tokenizer_model.get('byte_fallback', True)
+        )
+        if is_llama3:
+            raise TypeError('Llama 3 must be converted with BpeVocab')
+
+        if not is_llama3 and (
             tokenizer_model['type'] != 'BPE' or not tokenizer_model.get('byte_fallback', False)
             or tokenizer_json['decoder']['type'] != 'Sequence'
         ):
             raise FileNotFoundError('Cannot find Llama BPE tokenizer')
 
         try:
             from transformers import AutoTokenizer
@@ -633,33 +683,33 @@
 #
 # data loading
 # TODO: reuse (probably move to gguf.py?)
 #
 
 
 def permute(weights: NDArray, n_head: int, n_head_kv: int) -> NDArray:
-    # print( "permute debug " + str(weights.shape[0]) + " x " + str(weights.shape[1]) + " nhead " + str(n_head) + " nheadkv " + str(n_kv_head) )
     if n_head_kv is not None and n_head != n_head_kv:
         n_head = n_head_kv
     return (weights.reshape(n_head, 2, weights.shape[0] // n_head // 2, *weights.shape[1:])
             .swapaxes(1, 2)
             .reshape(weights.shape))
 
 
 class Tensor(ABC):
+    ndarray: NDArray
     data_type: DataType
 
     @abstractmethod
-    def astype(self, data_type: DataType) -> Tensor: ...
+    def astype(self, data_type: DataType) -> Self: ...
     @abstractmethod
-    def permute(self, n_head: int, n_head_kv: int) -> Tensor: ...
+    def permute(self, n_head: int, n_head_kv: int) -> Self: ...
     @abstractmethod
-    def permute_part(self, n_part: int, n_head: int, n_head_kv: int) -> UnquantizedTensor: ...
+    def permute_part(self, n_part: int, n_head: int, n_head_kv: int) -> Self: ...
     @abstractmethod
-    def part(self, n_part: int) -> UnquantizedTensor: ...
+    def part(self, n_part: int) -> Self: ...
     @abstractmethod
     def to_ggml(self) -> GGMLCompatibleTensor: ...
 
 
 def bf16_to_fp32(bf16_arr: np.ndarray[Any, np.dtype[np.uint16]]) -> NDArray:
     assert bf16_arr.dtype == np.uint16, f"Input array should be of dtype uint16, but got {bf16_arr.dtype}"
     fp32_arr = bf16_arr.astype(np.uint32) << 16
@@ -668,21 +718,21 @@
 
 class UnquantizedTensor(Tensor):
     def __init__(self, ndarray: NDArray):
         assert isinstance(ndarray, np.ndarray)
         self.ndarray = ndarray
         self.data_type = NUMPY_TYPE_TO_DATA_TYPE[ndarray.dtype]
 
-    def astype(self, data_type: DataType) -> Tensor:
+    def astype(self, data_type: DataType) -> UnquantizedTensor:
         dtype = data_type.dtype
         if self.data_type == DT_BF16:
             self.ndarray = bf16_to_fp32(self.ndarray)
         return UnquantizedTensor(self.ndarray.astype(dtype))
 
-    def to_ggml(self) -> UnquantizedTensor:
+    def to_ggml(self) -> Self:
         return self
 
     def permute_part(self, n_part: int, n_head: int, n_head_kv: int) -> UnquantizedTensor:
         r = self.ndarray.shape[0] // 3
         return UnquantizedTensor(permute(self.ndarray[r * n_part : r * n_part + r, ...], n_head, n_head_kv))
 
     def part(self, n_part: int) -> UnquantizedTensor:
@@ -893,15 +943,15 @@
         description = f'pickled storage_offset={storage_offset} in {storage.description}'
         return LazyTensor(load, list(size), storage.kind.data_type, description)
 
     @staticmethod
     def rebuild_from_type_v2(func, new_type, args, state):
         return func(*args)
 
-    CLASSES = {
+    CLASSES: dict[tuple[str, str], type[LazyTensor] | LazyStorageKind] = {
         # getattr used here as a workaround for mypy not being smart enough to determine
         # the staticmethods have a __func__ attribute.
         ('torch._tensor', '_rebuild_from_type_v2'): getattr(rebuild_from_type_v2, '__func__'),
         ('torch._utils', '_rebuild_tensor_v2'): getattr(lazy_rebuild_tensor_v2, '__func__'),
         ('torch', 'BFloat16Storage'): LazyStorageKind(DT_BF16),
         ('torch', 'HalfStorage'): LazyStorageKind(DT_F16),
         ('torch', 'FloatStorage'): LazyStorageKind(DT_F32),
@@ -1022,20 +1072,20 @@
             + (f" Maybe {vocab.vocab_size}?" if isinstance(vocab, Vocab) else ""),
         )
     if not isinstance(vocab, Vocab):
         return  # model has no vocab
 
     # Check for a vocab size mismatch
     if params.n_vocab == vocab.vocab_size:
-        print("Ignoring added_tokens.json since model matches vocab size without it.")
+        logger.warning("Ignoring added_tokens.json since model matches vocab size without it.")
         return
 
     if pad_vocab and params.n_vocab > vocab.vocab_size:
         pad_count = params.n_vocab - vocab.vocab_size
-        print(
+        logger.debug(
             f"Padding vocab with {pad_count} token(s) - <dummy00001> through <dummy{pad_count:05}>"
         )
         for i in range(1, pad_count + 1):
             vocab.added_tokens_dict[f"<dummy{i:05}>"] = -1
             vocab.added_tokens_list.append(f"<dummy{i:05}>")
         vocab.vocab_size = params.n_vocab
         return
@@ -1049,28 +1099,50 @@
     raise ValueError(msg)
 
 
 class OutputFile:
     def __init__(self, fname_out: Path, endianess:gguf.GGUFEndian = gguf.GGUFEndian.LITTLE):
         self.gguf = gguf.GGUFWriter(fname_out, gguf.MODEL_ARCH_NAMES[ARCH], endianess=endianess)
 
-    def add_meta_arch(self, params: Params) -> None:
+    def add_meta_model(self, params: Params, metadata: Metadata) -> None:
+        # Metadata About The Model And Its Provenence
         name = "LLaMA"
-
-        # TODO: better logic to determine model name
-        if params.n_ctx == 4096:
-            name = "LLaMA v2"
+        if metadata is not None and metadata.name is not None:
+            name = metadata.name
         elif params.path_model is not None:
-            name = str(params.path_model.parent).split('/')[-1]
+            name = params.path_model.name
+        elif params.n_ctx == 4096:
+            # Heuristic detection of LLaMA v2 model
+            name = "LLaMA v2"
 
-        self.gguf.add_name                (name)
-        self.gguf.add_context_length      (params.n_ctx)
-        self.gguf.add_embedding_length    (params.n_embd)
-        self.gguf.add_block_count         (params.n_layer)
-        self.gguf.add_feed_forward_length (params.n_ff)
+        self.gguf.add_name(name)
+
+        if metadata is not None:
+            if metadata.author is not None:
+                self.gguf.add_author(metadata.author)
+            if metadata.version is not None:
+                self.gguf.add_version(metadata.version)
+            if metadata.url is not None:
+                self.gguf.add_url(metadata.url)
+            if metadata.description is not None:
+                self.gguf.add_description(metadata.description)
+            if metadata.licence is not None:
+                self.gguf.add_licence(metadata.licence)
+            if metadata.source_url is not None:
+                self.gguf.add_source_url(metadata.source_url)
+            if metadata.source_hf_repo is not None:
+                self.gguf.add_source_hf_repo(metadata.source_hf_repo)
+
+    def add_meta_arch(self, params: Params) -> None:
+        # Metadata About The Neural Architecture Itself
+        self.gguf.add_vocab_size(params.n_vocab)
+        self.gguf.add_context_length(params.n_ctx)
+        self.gguf.add_embedding_length(params.n_embd)
+        self.gguf.add_block_count(params.n_layer)
+        self.gguf.add_feed_forward_length(params.n_ff)
         self.gguf.add_rope_dimension_count(params.n_embd // params.n_head)
         self.gguf.add_head_count          (params.n_head)
         self.gguf.add_head_count_kv       (params.n_head_kv)
 
         if params.n_experts:
             self.gguf.add_expert_count(params.n_experts)
 
@@ -1154,32 +1226,33 @@
             ndarrays = map(OutputFile.maybe_do_quantize, ndarrays_inner)
 
         start = time.time()
         for i, ((name, lazy_tensor), ndarray) in enumerate(zip(model.items(), ndarrays)):
             elapsed = time.time() - start
             size = ' x '.join(f"{dim:6d}" for dim in lazy_tensor.shape)
             padi = len(str(len(model)))
-            print(
+            logger.info(
                 f"[{i + 1:{padi}d}/{len(model)}] Writing tensor {name:38s} | size {size:16} | type {lazy_tensor.data_type.name:4} | T+{int(elapsed):4}"
             )
             self.gguf.write_tensor_data(ndarray)
 
     def close(self) -> None:
         self.gguf.close()
 
     @staticmethod
     def write_vocab_only(
         fname_out: Path, params: Params, vocab: Vocab, svocab: gguf.SpecialVocab,
-        endianess: gguf.GGUFEndian = gguf.GGUFEndian.LITTLE, pad_vocab: bool = False,
+        endianess: gguf.GGUFEndian = gguf.GGUFEndian.LITTLE, pad_vocab: bool = False, metadata: Metadata = None,
     ) -> None:
         check_vocab_size(params, vocab, pad_vocab=pad_vocab)
 
         of = OutputFile(fname_out, endianess=endianess)
 
         # meta data
+        of.add_meta_model(params, metadata)
         of.add_meta_arch(params)
         of.add_meta_vocab(vocab)
         of.add_meta_special_vocab(svocab)
 
         of.write_meta()
 
         of.close()
@@ -1198,20 +1271,22 @@
         return dt.quantize(arr)
 
     @staticmethod
     def write_all(
         fname_out: Path, ftype: GGMLFileType, params: Params, model: LazyModel, vocab: BaseVocab, svocab: gguf.SpecialVocab,
         concurrency: int = DEFAULT_CONCURRENCY, endianess: gguf.GGUFEndian = gguf.GGUFEndian.LITTLE,
         pad_vocab: bool = False,
+        metadata: Metadata = None,
     ) -> None:
         check_vocab_size(params, vocab, pad_vocab=pad_vocab)
 
         of = OutputFile(fname_out, endianess=endianess)
 
         # meta data
+        of.add_meta_model(params, metadata)
         of.add_meta_arch(params)
         if isinstance(vocab, Vocab):
             of.add_meta_vocab(vocab)
             of.add_meta_special_vocab(svocab)
         else:  # NoVocab
             of.gguf.add_tokenizer_model(vocab.tokenizer_model)
 
@@ -1239,14 +1314,45 @@
         return GGMLFileType.MostlyQ8_0
 
     name_to_type = {name: lazy_tensor.data_type for (name, lazy_tensor) in model.items()}
 
     raise ValueError(f"Unexpected combination of types: {name_to_type}")
 
 
+def model_parameter_count(model: LazyModel) -> int:
+    total_model_parameters = 0
+    for i, (name, lazy_tensor) in enumerate(model.items()):
+        sum_weights_in_tensor = 1
+        for dim in lazy_tensor.shape:
+            sum_weights_in_tensor *= dim
+        total_model_parameters += sum_weights_in_tensor
+    return total_model_parameters
+
+
+def model_parameter_count_rounded_notation(model_params_count: int) -> str:
+    if model_params_count > 1e12 :
+        # Trillions Of Parameters
+        scaled_model_params = model_params_count * 1e-12
+        scale_suffix = "T"
+    elif model_params_count > 1e9 :
+        # Billions Of Parameters
+        scaled_model_params = model_params_count * 1e-9
+        scale_suffix = "B"
+    elif model_params_count > 1e6 :
+        # Millions Of Parameters
+        scaled_model_params = model_params_count * 1e-6
+        scale_suffix = "M"
+    else:
+        # Thousands Of Parameters
+        scaled_model_params = model_params_count * 1e-3
+        scale_suffix = "K"
+
+    return f"{round(scaled_model_params)}{scale_suffix}"
+
+
 def convert_to_output_type(model: LazyModel, output_type: GGMLFileType) -> LazyModel:
     return {name: tensor.astype(output_type.type_for_tensor(name, tensor))
             for (name, tensor) in model.items()}
 
 
 def convert_model_names(model: LazyModel, params: Params, skip_unknown: bool) -> LazyModel:
     tmap = gguf.TensorNameMap(ARCH, params.n_layer)
@@ -1269,41 +1375,41 @@
                     else:
                         raise ValueError(f"Expert tensor not found: layers.{i_l}.feed_forward.experts.{e}.w{w}.weight")
                 tmp[f"layers.{i_l}.feed_forward.experts.w{w}.weight"] = pack_experts_lazy(experts)
 
     # HF models permut or pack some of the tensors, so we need to undo that
     for i in itertools.count():
         if f"model.layers.{i}.self_attn.q_proj.weight" in model:
-            print(f"Permuting layer {i}")
+            logger.debug(f"Permuting layer {i}")
             tmp[f"model.layers.{i}.self_attn.q_proj.weight"] = permute_lazy(model[f"model.layers.{i}.self_attn.q_proj.weight"], params.n_head, params.n_head)
             tmp[f"model.layers.{i}.self_attn.k_proj.weight"] = permute_lazy(model[f"model.layers.{i}.self_attn.k_proj.weight"], params.n_head, params.n_head_kv)
             # tmp[f"model.layers.{i}.self_attn.v_proj.weight"] =              model[f"model.layers.{i}.self_attn.v_proj.weight"]
         elif f"model.layers.{i}.self_attn.W_pack.weight" in model:
-            print(f"Unpacking and permuting layer {i}")
+            logger.debug(f"Unpacking and permuting layer {i}")
             tmp[f"model.layers.{i}.self_attn.q_proj.weight"] = permute_part_lazy(model[f"model.layers.{i}.self_attn.W_pack.weight"], 0, params.n_head, params.n_head)
             tmp[f"model.layers.{i}.self_attn.k_proj.weight"] = permute_part_lazy(model[f"model.layers.{i}.self_attn.W_pack.weight"], 1, params.n_head, params.n_head_kv)
             tmp[f"model.layers.{i}.self_attn.v_proj.weight"] = part_lazy        (model[f"model.layers.{i}.self_attn.W_pack.weight"], 2)
             del tmp[f"model.layers.{i}.self_attn.W_pack.weight"]
         else:
             break
 
     out: LazyModel = {}
     for name, lazy_tensor in model.items():
         tensor_type, name_new = tmap.get_type_and_name(name, try_suffixes = (".weight", ".bias")) or (None, None)
         if name_new is None:
             if skip_unknown:
-                print(f"Unexpected tensor name: {name} - skipping")
+                logger.warning(f"Unexpected tensor name: {name} - skipping")
                 continue
             raise ValueError(f"Unexpected tensor name: {name}. Use --skip-unknown to ignore it (e.g. LLaVA)")
 
         if tensor_type in should_skip:
-            print(f"skipping tensor {name_new}")
+            logger.debug(f"skipping tensor {name_new}")
             continue
 
-        print(f"{name:48s} -> {name_new:40s} | {lazy_tensor.data_type.name:6s} | {lazy_tensor.shape}")
+        logger.debug(f"{name:48s} -> {name_new:40s} | {lazy_tensor.data_type.name:6s} | {lazy_tensor.shape}")
         out[name_new] = lazy_tensor
 
     return out
 
 
 def nth_multifile_path(path: Path, n: int) -> Path | None:
     '''Given any path belonging to a multi-file model (e.g. foo.bin.1), return
@@ -1345,30 +1451,30 @@
 
 
 def load_some_model(path: Path) -> ModelPlus:
     '''Load a model of any supported format.'''
     # Be extra-friendly and accept either a file or a directory:
     if path.is_dir():
         # Check if it's a set of safetensors files first
-        globs = ["model-00001-of-*.safetensors", "model.safetensors"]
+        globs = ["model-00001-of-*.safetensors", "model.safetensors", "consolidated.safetensors"]
         files = [file for glob in globs for file in path.glob(glob)]
         if not files:
             # Try the PyTorch patterns too, with lower priority
             globs = ["consolidated.00.pth", "pytorch_model-00001-of-*.bin", "*.pt", "pytorch_model.bin"]
             files = [file for glob in globs for file in path.glob(glob)]
         if not files:
             raise FileNotFoundError(f"Can't find model in directory {path}")
         if len(files) > 1:
             raise ValueError(f"Found multiple models in {path}, not sure which to pick: {files}")
         path = files[0]
 
     paths = find_multifile_paths(path)
     models_plus: list[ModelPlus] = []
     for path in paths:
-        print(f"Loading model file {path}")
+        logger.info(f"Loading model file {path}")
         models_plus.append(lazy_load_file(path))
 
     model_plus = merge_multifile_models(models_plus)
     return model_plus
 
 
 class VocabFactory:
@@ -1401,15 +1507,15 @@
                 vocab = cls(self.path)
                 break
             except FileNotFoundError:
                 pass  # ignore unavailable tokenizers
         else:
             raise FileNotFoundError(f"Could not find a tokenizer matching any of {vocab_types}")
 
-        print(f"Loaded vocab file {vocab.fname_tokenizer!r}, type {vocab.name!r}")
+        logger.info(f"Loaded vocab file {vocab.fname_tokenizer!r}, type {vocab.name!r}")
         return vocab
 
     def load_vocab(self, vocab_types: list[str] | None, model_parent_path: Path) -> tuple[BaseVocab, gguf.SpecialVocab]:
         vocab: BaseVocab
         if vocab_types is None:
             vocab = NoVocab()
         else:
@@ -1418,35 +1524,57 @@
         special_vocab = self._create_special_vocab(
             vocab,
             model_parent_path,
         )
         return vocab, special_vocab
 
 
-def default_outfile(model_paths: list[Path], file_type: GGMLFileType) -> Path:
-    namestr = {
-        GGMLFileType.AllF32:    "f32",
-        GGMLFileType.MostlyF16: "f16",
-        GGMLFileType.MostlyQ8_0:"q8_0",
+def default_convention_outfile(file_type: GGMLFileType, params: Params, model_params_count: int, metadata: Metadata) -> str:
+    quantization = {
+        GGMLFileType.AllF32:    "F32",
+        GGMLFileType.MostlyF16: "F16",
+        GGMLFileType.MostlyQ8_0: "Q8_0",
     }[file_type]
-    ret = model_paths[0].parent / f"ggml-model-{namestr}.gguf"
+
+    parameters = model_parameter_count_rounded_notation(model_params_count)
+
+    expert_count = ""
+    if params.n_experts is not None:
+        expert_count = f"{params.n_experts}x"
+
+    version = ""
+    if metadata is not None and metadata.version is not None:
+        version = f"-{metadata.version}"
+
+    name = "ggml-model"
+    if metadata is not None and metadata.name is not None:
+        name = metadata.name
+    elif params.path_model is not None:
+        name = params.path_model.name
+
+    return f"{name}{version}-{expert_count}{parameters}-{quantization}"
+
+
+def default_outfile(model_paths: list[Path], file_type: GGMLFileType, params: Params, model_params_count: int, metadata: Metadata) -> Path:
+    default_filename = default_convention_outfile(file_type, params, model_params_count, metadata)
+    ret = model_paths[0].parent / f"{default_filename}.gguf"
     if ret in model_paths:
-        sys.stderr.write(
+        logger.error(
             f"Error: Default output path ({ret}) would overwrite the input. "
-            "Please explicitly specify a path using --outfile.\n")
+            "Please explicitly specify a path using --outfile.")
         sys.exit(1)
     return ret
 
 
 def do_dump_model(model_plus: ModelPlus) -> None:
-    print(f"model_plus.paths = {model_plus.paths!r}")
-    print(f"model_plus.format = {model_plus.format!r}")
-    print(f"model_plus.vocab = {model_plus.vocab!r}")
+    print(f"model_plus.paths = {model_plus.paths!r}") # noqa: NP100
+    print(f"model_plus.format = {model_plus.format!r}") # noqa: NP100
+    print(f"model_plus.vocab = {model_plus.vocab!r}") # noqa: NP100
     for name, lazy_tensor in model_plus.model.items():
-        print(f"{name}: shape={lazy_tensor.shape} type={lazy_tensor.data_type}; {lazy_tensor.description}")
+        print(f"{name}: shape={lazy_tensor.shape} type={lazy_tensor.data_type}; {lazy_tensor.description}") # noqa: NP100
 
 
 def main(args_in: list[str] | None = None) -> None:
     output_choices = ["f32", "f16"]
     if np.uint32(1) == np.uint32(1).newbyteorder("<"):
         # We currently only support Q8_0 output on little endian systems.
         output_choices.append("q8_0")
@@ -1461,90 +1589,129 @@
     parser.add_argument("--outfile",      type=Path,              help="path to write to; default: based on input")
     parser.add_argument("model",          type=Path,              help="directory containing model file, or model file itself (*.pth, *.pt, *.bin)")
     parser.add_argument("--ctx",          type=int,               help="model training context (default: based on input)")
     parser.add_argument("--concurrency",  type=int,               help=f"concurrency used for conversion (default: {DEFAULT_CONCURRENCY})", default=DEFAULT_CONCURRENCY)
     parser.add_argument("--big-endian",   action="store_true",    help="model is executed on big endian machine")
     parser.add_argument("--pad-vocab",    action="store_true",    help="add pad tokens when model vocab expects more than tokenizer metadata provides")
     parser.add_argument("--skip-unknown", action="store_true",    help="skip unknown tensor names instead of failing")
+    parser.add_argument("--verbose",      action="store_true",    help="increase output verbosity")
+    parser.add_argument("--metadata",     type=Path,              help="Specify the path for a metadata file")
+    parser.add_argument("--get-outfile",  action="store_true",    help="get calculated default outfile name")
 
     args = parser.parse_args(args_in)
+
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
+    elif args.dump_single or args.dump or args.get_outfile:
+        # Avoid printing anything besides the dump output
+        logging.basicConfig(level=logging.WARNING)
+    else:
+        logging.basicConfig(level=logging.INFO)
+
+    metadata = Metadata.load(args.metadata)
+
+    if args.get_outfile:
+        model_plus = load_some_model(args.model)
+        params = Params.load(model_plus)
+        model   = convert_model_names(model_plus.model, params, args.skip_unknown)
+        model_params_count = model_parameter_count(model_plus.model)
+        ftype   = pick_output_type(model, args.outtype)
+        print(f"{default_convention_outfile(ftype, params, model_params_count, metadata)}") # noqa: NP100
+        return
+
     if args.no_vocab and args.vocab_only:
         raise ValueError("--vocab-only does not make sense with --no-vocab")
 
     if args.dump_single:
         model_plus = lazy_load_file(args.model)
         do_dump_model(model_plus)
         return
 
     if not args.vocab_only:
         model_plus = load_some_model(args.model)
     else:
         model_plus = ModelPlus(model = {}, paths = [args.model / 'dummy'], format = 'none', vocab = None)
 
+    model_params_count = model_parameter_count(model_plus.model)
+    logger.info(f"model parameters count : {model_params_count} ({model_parameter_count_rounded_notation(model_params_count)})")
+
     if args.dump:
         do_dump_model(model_plus)
         return
+
     endianess = gguf.GGUFEndian.LITTLE
     if args.big_endian:
         endianess = gguf.GGUFEndian.BIG
 
-    params = Params.load(model_plus)
-    if params.n_ctx == -1:
-        if args.ctx is None:
-            msg = """\
-                The model doesn't have a context size, and you didn't specify one with --ctx
-                Please specify one with --ctx:
-                 - LLaMA v1: --ctx 2048
-                 - LLaMA v2: --ctx 4096"""
-            parser.error(textwrap.dedent(msg))
-        params.n_ctx = args.ctx
-
-    if args.outtype:
-        params.ftype = {
-            "f32": GGMLFileType.AllF32,
-            "f16": GGMLFileType.MostlyF16,
-            "q8_0": GGMLFileType.MostlyQ8_0,
-        }[args.outtype]
+    params = None
+    if args.pad_vocab or not args.vocab_only:
+        params = Params.load(model_plus)
+        if params.n_ctx == -1:
+            if args.ctx is None:
+                msg = """\
+                    The model doesn't have a context size, and you didn't specify one with --ctx
+                    Please specify one with --ctx:
+                     - LLaMA v1: --ctx 2048
+                     - LLaMA v2: --ctx 4096"""
+                parser.error(textwrap.dedent(msg))
+            params.n_ctx = args.ctx
+
+        if args.outtype:
+            params.ftype = {
+                "f32": GGMLFileType.AllF32,
+                "f16": GGMLFileType.MostlyF16,
+                "q8_0": GGMLFileType.MostlyQ8_0,
+            }[args.outtype]
 
-    print(f"params = {params}")
+        logger.info(f"params = {params}")
 
     model_parent_path = model_plus.paths[0].parent
     vocab_path = Path(args.vocab_dir or args.model or model_parent_path)
     vocab_factory = VocabFactory(vocab_path)
     vocab_types = None if args.no_vocab else args.vocab_type.split(",")
     vocab, special_vocab = vocab_factory.load_vocab(vocab_types, model_parent_path)
 
     if args.vocab_only:
         assert isinstance(vocab, Vocab)
         if not args.outfile:
             raise ValueError("need --outfile if using --vocab-only")
         outfile = args.outfile
+        if params is None:
+            params = Params(
+                n_vocab    = vocab.vocab_size,
+                n_embd     = 1,
+                n_layer    = 1,
+                n_ctx      = 1,
+                n_ff       = 1,
+                n_head     = 1,
+                n_head_kv  = 1,
+                f_norm_eps = 1e-5,
+            )
         OutputFile.write_vocab_only(outfile, params, vocab, special_vocab,
-                                    endianess=endianess, pad_vocab=args.pad_vocab)
-        print(f"Wrote {outfile}")
+                                    endianess=endianess, pad_vocab=args.pad_vocab, metadata=metadata)
+        logger.info(f"Wrote {outfile}")
         return
 
     if model_plus.vocab is not None and args.vocab_dir is None and not args.no_vocab:
         vocab = model_plus.vocab
 
-    print(f"Vocab info: {vocab}")
-    print(f"Special vocab info: {special_vocab}")
-
+    logger.info(f"Vocab info: {vocab}")
+    logger.info(f"Special vocab info: {special_vocab}")
     model   = model_plus.model
     model   = convert_model_names(model, params, args.skip_unknown)
     ftype   = pick_output_type(model, args.outtype)
     model   = convert_to_output_type(model, ftype)
-    outfile = args.outfile or default_outfile(model_plus.paths, ftype)
+    outfile = args.outfile or default_outfile(model_plus.paths, ftype, params, model_params_count, metadata)
 
     params.ftype = ftype
-    print(f"Writing {outfile}, format {ftype}")
+    logger.info(f"Writing {outfile}, format {ftype}")
 
     OutputFile.write_all(outfile, ftype, params, model, vocab, special_vocab,
-                         concurrency=args.concurrency, endianess=endianess, pad_vocab=args.pad_vocab)
-    print(f"Wrote {outfile}")
+                         concurrency=args.concurrency, endianess=endianess, pad_vocab=args.pad_vocab, metadata=metadata)
+    logger.info(f"Wrote {outfile}")
 
 
 if __name__ == '__main__':
     main()
 
 def do_gguf_conversion(model: str, output: str, out_type: str, vocab_dir: str, vocab_type: str, context: int, pad_vocab: bool, concurrency: bool, big_endian: bool) -> None:
     model_plus = load_some_model(model)
```

### Comparing `llm_quantkit-0.26/quantkit/quantkit.py` & `llm_quantkit-0.27/quantkit/quantkit.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import site
 import time
 import datetime
 
 from pathlib import Path
 from quantkit.safetensor import convert_multi
 from quantkit.convert import do_gguf_conversion
+from quantkit.convert_hf import do_gguf_conversion as do_gguf_conversion_hf
 
 def run_download(model, output, hf_cache, force_download, resume_download, safetensors_only, branch):
     if output is None:
         model_dir = model.split("/")[1]
         path = Path(model_dir)
     else:
         path = Path(output)
@@ -39,14 +40,15 @@
 
 def run_gguf(model, quant_type, output, keep, f32, built_in_imatrix, imatrix, cal_file, n_gpu_layers):
     if cal_file is not None:
         if not Path(cal_file).is_file():
             print(f"quantkit: could not load {cal_file}")
             return
 
+    bf16 = False
     path = Path(model)
     if path.is_dir():
         if Path(path / "config.json").is_file():
             model_dir = path
         else:
             click.echo("no config.json found in model dir")
             return
@@ -54,42 +56,52 @@
         model_dir = model.split("/")[1]
         path = Path(model_dir)
 
         from huggingface_hub import snapshot_download
         snapshot_download(model, local_dir=path, local_dir_use_symlinks=True, resume_download=True)
 
     do_step_two = False
+    import json
+    with open(path / "config.json") as f:
+        config = json.load(f)
+        if 'torch_dtype' in config:
+            if config['torch_dtype'] == 'bfloat16':
+                bf16 = True
 
     #if lower(quant_type) not in ["F32", "F16", "Q8_0"]:
-    if quant_type.lower() not in [x.lower() for x in ["F32", "F16", "Q8_0"]]:
+    if quant_type.lower() not in [x.lower() for x in ["F32", "F16", "BF16", "Q8_0"]]:
         # two step
         if quant_type.lower() not in [x.lower() for x in ["Q4_0", "Q4_1", "Q5_0", "Q5_1", "Q8_0", "Q8_1", "Q2_K", "IQ3_XS",
                                                           "Q3_K", "Q4_K", "Q5_K", "Q6_K", "Q8_K", "IQ2_XXS", "IQ2_XS", "IQ3_XXS",
                                                           "Q2_K_S", "Q3_K_S", "Q3_K_M", "Q3_K_L", "Q4_K_S", "Q4_K_M", "Q5_K_S", "Q5_K_M",
                                                           "IQ1_S", "IQ4_NL", "IQ3_S", "IQ2_S", "IQ4_XS", "IQ2_M", "IQ3_M"] ]:
             raise ValueError("quant_type must be a valid gguf quant type")
         step_two = quant_type
         do_step_two = True
-        quant_type = "F32" if f32 else "F16"
+        quant_type = "F32" if f32 else "BF16" if bf16 else "F16"
 
     # fix vocab here
+    if Path(path / "tokenizer.model").is_file():
+        vocab_type = "spm,hfft"
+    else:
+        vocab_type = "bpe"
 
     if output is None:
         output = str(model_dir) + "_" + (step_two.upper() or quant_type.upper()) + ".gguf"
 
     #def do_gguf_conversion(model: str, output: str, out_type: str, vocab_dir: str, vocab_type: str, context: int, pad_vocab: bool, concurrency: bool, big_endian: bool) -> None:
     if do_step_two:
-        do_gguf_conversion(Path(model_dir), "tmp.gguf", quant_type.lower(), None, "spm,hfft", -1, False, False, False)
+        do_gguf_conversion_hf(Path(model_dir), "tmp.gguf", quant_type.lower(), None, vocab_type, -1, False, False, False)
 
         if built_in_imatrix or (imatrix is None and cal_file is not None):
             imatrix = run_imatrix(cal_file, n_gpu_layers)
 
         quantize("tmp.gguf", output, step_two, imatrix)
     else:
-        do_gguf_conversion(Path(model_dir), output, quant_type.lower(), None, "spm,hfft", -1, False, False, False)
+        do_gguf_conversion_hf(Path(model_dir), output, quant_type.lower(), None, vocab_type, -1, False, False, False)
 
     if not keep:
         os.remove("tmp.gguf")
         print("deleted tmp.gguf")
     print(f"Finished with {output}")
 
 def run_imatrix(cal_file, n_gpu_layers):
```

### Comparing `llm_quantkit-0.26/quantkit/safetensor.py` & `llm_quantkit-0.27/quantkit/safetensor.py`

 * *Files identical despite different names*

