# Comparing `tmp/qytorch-0.0.2.tar.gz` & `tmp/qytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qytorch-0.0.2.tar", last modified: Fri Feb 16 19:05:13 2024, max compression
+gzip compressed data, was "qytorch-0.0.3.tar", last modified: Tue May 21 21:19:54 2024, max compression
```

## Comparing `qytorch-0.0.2.tar` & `qytorch-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 aritra    (1000) aritra    (1000)        0 2024-02-16 19:05:13.294354 qytorch-0.0.2/
--rw-rw-r--   0 aritra    (1000) aritra    (1000)     1077 2024-02-16 14:54:33.000000 qytorch-0.0.2/LICENSE
--rw-rw-r--   0 aritra    (1000) aritra    (1000)     1313 2024-02-16 19:05:13.294354 qytorch-0.0.2/PKG-INFO
--rw-rw-r--   0 aritra    (1000) aritra    (1000)      303 2024-02-16 18:58:56.000000 qytorch-0.0.2/README.md
-drwxrwxr-x   0 aritra    (1000) aritra    (1000)        0 2024-02-16 19:05:13.290354 qytorch-0.0.2/qytorch/
--rw-rw-r--   0 aritra    (1000) aritra    (1000)       68 2024-02-16 11:41:51.000000 qytorch-0.0.2/qytorch/__init__.py
--rw-rw-r--   0 aritra    (1000) aritra    (1000)      574 2024-02-16 11:37:49.000000 qytorch-0.0.2/qytorch/a.py
--rw-rw-r--   0 aritra    (1000) aritra    (1000)    12838 2024-02-16 11:37:49.000000 qytorch-0.0.2/qytorch/qconv.py
--rw-rw-r--   0 aritra    (1000) aritra    (1000)     3225 2024-02-16 11:37:49.000000 qytorch-0.0.2/qytorch/qlinear.py
--rw-rw-r--   0 aritra    (1000) aritra    (1000)    17431 2024-02-16 11:37:49.000000 qytorch-0.0.2/qytorch/qmha.py
--rw-rw-r--   0 aritra    (1000) aritra    (1000)    46048 2024-02-16 11:37:49.000000 qytorch-0.0.2/qytorch/qtransformer.py
--rw-rw-r--   0 aritra    (1000) aritra    (1000)     4158 2024-02-16 11:37:49.000000 qytorch-0.0.2/qytorch/quat_base.py
-drwxrwxr-x   0 aritra    (1000) aritra    (1000)        0 2024-02-16 19:05:13.294354 qytorch-0.0.2/qytorch.egg-info/
--rw-rw-r--   0 aritra    (1000) aritra    (1000)     1313 2024-02-16 19:05:13.000000 qytorch-0.0.2/qytorch.egg-info/PKG-INFO
--rw-rw-r--   0 aritra    (1000) aritra    (1000)      310 2024-02-16 19:05:13.000000 qytorch-0.0.2/qytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 aritra    (1000) aritra    (1000)        1 2024-02-16 19:05:13.000000 qytorch-0.0.2/qytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 aritra    (1000) aritra    (1000)        6 2024-02-16 19:05:13.000000 qytorch-0.0.2/qytorch.egg-info/requires.txt
--rw-rw-r--   0 aritra    (1000) aritra    (1000)        8 2024-02-16 19:05:13.000000 qytorch-0.0.2/qytorch.egg-info/top_level.txt
--rw-rw-r--   0 aritra    (1000) aritra    (1000)       38 2024-02-16 19:05:13.294354 qytorch-0.0.2/setup.cfg
--rw-rw-r--   0 aritra    (1000) aritra    (1000)     1313 2024-02-16 19:04:54.000000 qytorch-0.0.2/setup.py
+drwxrwxr-x   0 aritra    (1000) aritra    (1000)        0 2024-05-21 21:19:54.306807 qytorch-0.0.3/
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)     1077 2024-05-21 18:56:08.000000 qytorch-0.0.3/LICENSE
+-rw-r--r--   0 aritra    (1000) aritra    (1000)     1238 2024-05-21 21:19:54.306807 qytorch-0.0.3/PKG-INFO
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)       27 2024-05-21 18:56:08.000000 qytorch-0.0.3/README.md
+drwxrwxr-x   0 aritra    (1000) aritra    (1000)        0 2024-05-21 21:19:54.306807 qytorch-0.0.3/qytorch/
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)       68 2024-05-21 18:56:08.000000 qytorch-0.0.3/qytorch/__init__.py
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)      580 2024-05-21 19:15:31.000000 qytorch-0.0.3/qytorch/a.py
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)    13217 2024-05-21 21:07:46.000000 qytorch-0.0.3/qytorch/qconv.py
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)     3321 2024-05-21 20:18:56.000000 qytorch-0.0.3/qytorch/qlinear.py
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)    17412 2024-05-21 19:08:25.000000 qytorch-0.0.3/qytorch/qmha.py
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)    46048 2024-05-21 18:56:08.000000 qytorch-0.0.3/qytorch/qtransformer.py
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)     1444 2024-05-21 19:52:55.000000 qytorch-0.0.3/qytorch/quat_base.py
+drwxrwxr-x   0 aritra    (1000) aritra    (1000)        0 2024-05-21 21:19:54.306807 qytorch-0.0.3/qytorch.egg-info/
+-rw-r--r--   0 aritra    (1000) aritra    (1000)     1238 2024-05-21 21:19:54.000000 qytorch-0.0.3/qytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)      310 2024-05-21 21:19:54.000000 qytorch-0.0.3/qytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)        1 2024-05-21 21:19:54.000000 qytorch-0.0.3/qytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)       12 2024-05-21 21:19:54.000000 qytorch-0.0.3/qytorch.egg-info/requires.txt
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)        8 2024-05-21 21:19:54.000000 qytorch-0.0.3/qytorch.egg-info/top_level.txt
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)       38 2024-05-21 21:19:54.306807 qytorch-0.0.3/setup.cfg
+-rw-rw-r--   0 aritra    (1000) aritra    (1000)     1514 2024-05-21 21:19:21.000000 qytorch-0.0.3/setup.py
```

### Comparing `qytorch-0.0.2/LICENSE` & `qytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qytorch-0.0.2/qytorch/a.py` & `qytorch-0.0.3/qytorch/a.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 
 # print(transformer.__all__)
 
 
 # nn.Linear
 
 
-model = nn.Conv2d(4, 16, kernel_size=3, stride=1, padding=1)
+# model = nn.Conv2d(4, 16, kernel_size=3, stride=1, padding=1)
 
-x = torch.randn(10, 4, 32, 32)
+# x = torch.randn(10, 4, 32, 32)
 
-print(model(x).shape)
+# print(model(x).shape)
```

### Comparing `qytorch-0.0.2/qytorch/qconv.py` & `qytorch-0.0.3/qytorch/qconv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import math
-import warnings
-
 import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from typing import Optional, Union, List, Tuple
+
 from torch import Tensor
-from torch.nn.parameter import Parameter, UninitializedParameter
-from torch.nn import functional as F
+from torch.nn.parameter import Parameter
 from torch.nn import init
-import torch.nn as nn
-# from .lazy import LazyModuleMixin
-# from .module import Module
-from torch.nn.modules.utils import _single, _pair, _triple, _reverse_repeat_tuple
-# from torch._torch_docs import reproducibility_notes
 
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
-from typing import Optional, List, Tuple, Union
+from torch.nn.modules.utils import _single, _pair, _triple, _reverse_repeat_tuple
 
 from quat_base import _construct_matrix
 
-nn.Conv2d
+
+
+
 
 class _QConvNd(nn.Module):
 
     __constants__ = ['stride', 'padding', 'dilation', 'groups',
                      'padding_mode', 'output_padding', 'in_channels',
                      'out_channels', 'kernel_size']
     __annotations__ = {'bias': Optional[torch.Tensor]}
@@ -36,18 +35,15 @@
     stride: Tuple[int, ...]
     padding: Union[str, Tuple[int, ...]]
     dilation: Tuple[int, ...]
     transposed: bool
     output_padding: Tuple[int, ...]
     groups: int
     padding_mode: str
-    r_weight: Tensor
-    i_weight: Tensor
-    j_weight: Tensor
-    k_weight: Tensor
+    weight: Tensor
     bias: Optional[Tensor]
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
                  kernel_size: Tuple[int, ...],
                  stride: Tuple[int, ...],
@@ -56,16 +52,14 @@
                  transposed: bool,
                  output_padding: Tuple[int, ...],
                  groups: int,
                  bias: bool,
                  padding_mode: str,
                  device=None,
                  dtype=None) -> None:
-        assert in_channels % 4 == 0 and out_channels % 4 == 0, "in_channels and out_channels must be divisible by 4"
-
         factory_kwargs = {'device': device, 'dtype': dtype}
         super().__init__()
         if groups <= 0:
             raise ValueError('groups must be a positive integer')
         if in_channels % groups != 0:
             raise ValueError('in_channels must be divisible by groups')
         if out_channels % groups != 0:
@@ -87,55 +81,58 @@
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         self.transposed = transposed
         self.output_padding = output_padding
         self.groups = groups
         self.padding_mode = padding_mode
-        # `_reversed_padding_repeated_twice` is the padding to be passed to
-        # `F.pad` if needed (e.g., for non-zero padding types that are
-        # implemented as two ops: padding + conv). `F.pad` accepts paddings in
-        # reverse order than the dimension.
+
         if isinstance(self.padding, str):
             self._reversed_padding_repeated_twice = [0, 0] * len(kernel_size)
             if padding == 'same':
                 for d, k, i in zip(dilation, kernel_size,
                                    range(len(kernel_size) - 1, -1, -1)):
                     total_padding = d * (k - 1)
                     left_pad = total_padding // 2
                     self._reversed_padding_repeated_twice[2 * i] = left_pad
                     self._reversed_padding_repeated_twice[2 * i + 1] = (
                         total_padding - left_pad)
         else:
             self._reversed_padding_repeated_twice = _reverse_repeat_tuple(self.padding, 2)
 
         if transposed:
-            self.r_weight = Parameter(torch.empty((in_channels // 4, out_channels // (groups*4), *kernel_size), **factory_kwargs))
-            self.i_weight = Parameter(torch.empty((in_channels // 4, out_channels // (groups*4), *kernel_size), **factory_kwargs))
-            self.j_weight = Parameter(torch.empty((in_channels // 4, out_channels // (groups*4), *kernel_size), **factory_kwargs))
-            self.k_weight = Parameter(torch.empty((in_channels // 4, out_channels // (groups*4), *kernel_size), **factory_kwargs))
+            # self.weight = Parameter(torch.empty((in_channels, out_channels // groups, *kernel_size), **factory_kwargs))
+            a, b = in_channels, out_channels // groups
+            assert a%4 == 0 and b%4 == 0, f"in_channels={a}, (out_channels//groups)={b} must be divisible by 4"
+            self.r_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
+            self.i_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
+            self.j_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
+            self.k_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
         else:
-            self.r_weight = Parameter(torch.empty((out_channels // 4, in_channels // (groups*4), *kernel_size), **factory_kwargs))
-            self.i_weight = Parameter(torch.empty((out_channels // 4, in_channels // (groups*4), *kernel_size), **factory_kwargs))
-            self.j_weight = Parameter(torch.empty((out_channels // 4, in_channels // (groups*4), *kernel_size), **factory_kwargs))
-            self.k_weight = Parameter(torch.empty((out_channels // 4, in_channels // (groups*4), *kernel_size), **factory_kwargs))
+            # self.weight = Parameter(torch.empty((out_channels, in_channels // groups, *kernel_size), **factory_kwargs))
+            a, b = out_channels, in_channels // groups
+            assert a%4 == 0 and b%4 == 0, f"out_channels={a}, (in_channels//groups)={b} must be divisible by 4"
+            self.r_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
+            self.i_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
+            self.j_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
+            self.k_weight = Parameter(torch.empty((a//4, b//4, *kernel_size), **factory_kwargs))
         if bias:
             self.bias = Parameter(torch.empty(out_channels, **factory_kwargs))
         else:
             self.register_parameter('bias', None)
 
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
-        nn.init.kaiming_uniform_(self.r_weight, a=math.sqrt(5))
-        nn.init.kaiming_uniform_(self.i_weight, a=math.sqrt(5))
-        nn.init.kaiming_uniform_(self.j_weight, a=math.sqrt(5))
-        nn.init.kaiming_uniform_(self.k_weight, a=math.sqrt(5))
+        init.kaiming_uniform_(self.r_weight, a=math.sqrt(5))
+        init.kaiming_uniform_(self.i_weight, a=math.sqrt(5))
+        init.kaiming_uniform_(self.j_weight, a=math.sqrt(5))
+        init.kaiming_uniform_(self.k_weight, a=math.sqrt(5))
         if self.bias is not None:
-            fan_in, _ = init._calculate_fan_in_and_fan_out(torch.zeros((self.r_weight.size(0)*4, self.r_weight.size(1)*4), dtype=torch.bool))
+            fan_in, _ = init._calculate_fan_in_and_fan_out(self.r_weight)
             if fan_in != 0:
                 bound = 1 / math.sqrt(fan_in)
                 init.uniform_(self.bias, -bound, bound)
 
     def extra_repr(self):
         s = ('{in_channels}, {out_channels}, kernel_size={kernel_size}'
              ', stride={stride}')
@@ -155,75 +152,66 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
         if not hasattr(self, 'padding_mode'):
             self.padding_mode = 'zeros'
 
 
-# class QConv1d(_QConvNd):
-#     def __init__(
-#         self,
-#         in_channels: int,
-#         out_channels: int,
-#         kernel_size: _size_1_t,
-#         stride: _size_1_t = 1,
-#         padding: Union[str, _size_1_t] = 0,
-#         dilation: _size_1_t = 1,
-#         groups: int = 1,
-#         bias: bool = True,
-#         padding_mode: str = 'zeros',  # TODO: refine this type
-#         device=None,
-#         dtype=None
-#     ) -> None:
-#         factory_kwargs = {'device': device, 'dtype': dtype}
-#         # we create new variables below to make mypy happy since kernel_size has
-#         # type Union[int, Tuple[int]] and kernel_size_ has type Tuple[int]
-#         kernel_size_ = _single(kernel_size)
-#         stride_ = _single(stride)
-#         padding_ = padding if isinstance(padding, str) else _single(padding)
-#         dilation_ = _single(dilation)
-#         super().__init__(
-#             in_channels, out_channels, kernel_size_, stride_, padding_, dilation_,
-#             False, _single(0), groups, bias, padding_mode, **factory_kwargs)
-
-#     def _conv_forward(self, input: Tensor, weight: Tensor, bias: Optional[Tensor]):
-#         if self.padding_mode != 'zeros':
-#             return F.conv1d(F.pad(input, self._reversed_padding_repeated_twice, mode=self.padding_mode),
-#                             weight, bias, self.stride,
-#                             _single(0), self.dilation, self.groups)
-#         return F.conv1d(input, weight, bias, self.stride,
-#                         self.padding, self.dilation, self.groups)
-
-#     def forward(self, input: Tensor) -> Tensor:
-#         weight = _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
-#         return self._conv_forward(input, weight, self.bias)
+class QConv1d(_QConvNd):
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: _size_1_t,
+        stride: _size_1_t = 1,
+        padding: Union[str, _size_1_t] = 0,
+        dilation: _size_1_t = 1,
+        groups: int = 1,
+        bias: bool = True,
+        padding_mode: str = 'zeros',
+        device=None,
+        dtype=None
+    ) -> None:
+        factory_kwargs = {'device': device, 'dtype': dtype}
+        kernel_size_ = _single(kernel_size)
+        stride_ = _single(stride)
+        padding_ = padding if isinstance(padding, str) else _single(padding)
+        dilation_ = _single(dilation)
+        super().__init__(
+            in_channels, out_channels, kernel_size_, stride_, padding_, dilation_,
+            False, _single(0), groups, bias, padding_mode, **factory_kwargs)
 
+    def _conv_forward(self, input: Tensor, weight: Tensor, bias: Optional[Tensor]):
+        if self.padding_mode != 'zeros':
+            return F.conv1d(F.pad(input, self._reversed_padding_repeated_twice, mode=self.padding_mode),
+                            weight, bias, self.stride,
+                            _single(0), self.dilation, self.groups)
+        return F.conv1d(input, weight, bias, self.stride,
+                        self.padding, self.dilation, self.groups)
 
-class QConv2d(_QConvNd):
-    """Quaternion convolution 2d.
+    def forward(self, input: Tensor) -> Tensor:
+        weight = self.get_weight()
+        return self._conv_forward(input, weight, self.bias)
+
+    def get_weight(self):
+        return _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
 
-    Examples:
-        >>> model = QConv2d(20, 16, kernel_size=3, stride=1, padding=1)  # 20 and 16 are divisible by 4
-        >>> x = torch.randn(128, 20, 32, 32)
-        >>> output = model(x)
-        >>> print(output.size())
-        torch.Size([128, 16, 30, 30])
-    """
 
+class QConv2d(_QConvNd):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size: _size_2_t,
         stride: _size_2_t = 1,
         padding: Union[str, _size_2_t] = 0,
         dilation: _size_2_t = 1,
         groups: int = 1,
         bias: bool = True,
-        padding_mode: str = 'zeros',  # TODO: refine this type
+        padding_mode: str = 'zeros',
         device=None,
         dtype=None
     ) -> None:
         factory_kwargs = {'device': device, 'dtype': dtype}
         kernel_size_ = _pair(kernel_size)
         stride_ = _pair(stride)
         padding_ = padding if isinstance(padding, str) else _pair(padding)
@@ -237,55 +225,101 @@
             return F.conv2d(F.pad(input, self._reversed_padding_repeated_twice, mode=self.padding_mode),
                             weight, bias, self.stride,
                             _pair(0), self.dilation, self.groups)
         return F.conv2d(input, weight, bias, self.stride,
                         self.padding, self.dilation, self.groups)
 
     def forward(self, input: Tensor) -> Tensor:
-        weight = _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
+        weight = self.get_weight()
         return self._conv_forward(input, weight, self.bias)
 
-# class QConv3d(_QConvNd):
-#     def __init__(
-#         self,
-#         in_channels: int,
-#         out_channels: int,
-#         kernel_size: _size_3_t,
-#         stride: _size_3_t = 1,
-#         padding: Union[str, _size_3_t] = 0,
-#         dilation: _size_3_t = 1,
-#         groups: int = 1,
-#         bias: bool = True,
-#         padding_mode: str = 'zeros',
-#         device=None,
-#         dtype=None
-#     ) -> None:
-#         factory_kwargs = {'device': device, 'dtype': dtype}
-#         kernel_size_ = _triple(kernel_size)
-#         stride_ = _triple(stride)
-#         padding_ = padding if isinstance(padding, str) else _triple(padding)
-#         dilation_ = _triple(dilation)
-#         super().__init__(
-#             in_channels, out_channels, kernel_size_, stride_, padding_, dilation_,
-#             False, _triple(0), groups, bias, padding_mode, **factory_kwargs)
-
-#     def _conv_forward(self, input: Tensor, weight: Tensor, bias: Optional[Tensor]):
-#         if self.padding_mode != 'zeros':
-#             return F.conv3d(F.pad(input, self._reversed_padding_repeated_twice, mode=self.padding_mode),
-#                             weight, bias, self.stride,
-#                             _triple(0), self.dilation, self.groups)
-#         return F.conv3d(input, weight, bias, self.stride,
-#                         self.padding, self.dilation, self.groups)
-
-#     def forward(self, input: Tensor) -> Tensor:
-#         weight = _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
-#         return self._conv_forward(input, weight, self.bias)
+    def get_weight(self):
+        return _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
+
+class QConv3d(_QConvNd):
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        kernel_size: _size_3_t,
+        stride: _size_3_t = 1,
+        padding: Union[str, _size_3_t] = 0,
+        dilation: _size_3_t = 1,
+        groups: int = 1,
+        bias: bool = True,
+        padding_mode: str = 'zeros',
+        device=None,
+        dtype=None
+    ) -> None:
+        factory_kwargs = {'device': device, 'dtype': dtype}
+        kernel_size_ = _triple(kernel_size)
+        stride_ = _triple(stride)
+        padding_ = padding if isinstance(padding, str) else _triple(padding)
+        dilation_ = _triple(dilation)
+        super().__init__(
+            in_channels, out_channels, kernel_size_, stride_, padding_, dilation_,
+            False, _triple(0), groups, bias, padding_mode, **factory_kwargs)
+
+    def _conv_forward(self, input: Tensor, weight: Tensor, bias: Optional[Tensor]):
+        if self.padding_mode != "zeros":
+            return F.conv3d(
+                F.pad(
+                    input, self._reversed_padding_repeated_twice, mode=self.padding_mode
+                ),
+                weight,
+                bias,
+                self.stride,
+                _triple(0),
+                self.dilation,
+                self.groups,
+            )
+        return F.conv3d(
+            input, weight, bias, self.stride, self.padding, self.dilation, self.groups
+        )
+
+    def forward(self, input: Tensor) -> Tensor:
+        weight = self.get_weight()
+        return self._conv_forward(input, weight, self.bias)
+    
+    def get_weight(self):
+        return _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
 
 
 if __name__ == '__main__':
-    # model = nn.Conv2d(20, 16, kernel_size=3, stride=1, padding=1)
-    model = QConv2d(20, 16, kernel_size=3, stride=1, padding=1)  # 20 and 16 are divisible by 4
-    x = torch.randn(128, 20, 32, 32)
-    output = model(x)
-    print(output.size())
-    # print(f"{model.weight.size() = }")
-    print(f"{model.r_weight.size() = },\n{model.i_weight.size() = },\n{model.j_weight.size() = },\n{model.k_weight.size() = }")
+    print("QConv1d:")
+    rmodel = nn.Conv1d(20, 16, 3, stride=1, padding=1)
+    qmodel = QConv1d(20, 16, 3, stride=1, padding=1)
+    input_ = torch.randn(128, 20, 32)
+    routput = rmodel(input_)
+    qoutput = qmodel(input_)
+    print(f"{rmodel.weight.size() = }")
+    print(f"{qmodel.r_weight.size() = }")
+    print(f"{qmodel.i_weight.size() = }")
+    print(f"{qmodel.j_weight.size() = }")
+    print(f"{qmodel.k_weight.size() = }")
+    print(f"{input_.size() = }\n{routput.size() = }\n{qoutput.size() = }")
+    
+    print("\nQConv2d:")
+    rmodel = nn.Conv2d(20, 16, 3, stride=1, padding=1)
+    qmodel = QConv2d(20, 16, 3, stride=1, padding=1)
+    input_ = torch.randn(128, 20, 32, 32)
+    routput = rmodel(input_)
+    qoutput = qmodel(input_)
+    print(f"{rmodel.weight.size() = }")
+    print(f"{qmodel.r_weight.size() = }")
+    print(f"{qmodel.i_weight.size() = }")
+    print(f"{qmodel.j_weight.size() = }")
+    print(f"{qmodel.k_weight.size() = }")
+    print(f"{input_.size() = }\n{routput.size() = }\n{qoutput.size() = }")
+    
+    print("\nQConv3d:")
+    rmodel = nn.Conv3d(20, 16, 3, stride=1, padding=1)
+    qmodel = QConv3d(20, 16, 3, stride=1, padding=1)
+    input_ = torch.randn(128, 20, 32, 32, 32)
+    routput = rmodel(input_)
+    qoutput = qmodel(input_)
+    print(f"{rmodel.weight.size() = }")
+    print(f"{qmodel.r_weight.size() = }")
+    print(f"{qmodel.i_weight.size() = }")
+    print(f"{qmodel.j_weight.size() = }")
+    print(f"{qmodel.k_weight.size() = }")
+    print(f"{input_.size() = }\n{routput.size() = }\n{qoutput.size() = }")
```

### Comparing `qytorch-0.0.2/qytorch/qlinear.py` & `qytorch-0.0.3/qytorch/qlinear.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,19 @@
     def __init__(self, in_features: int, out_features: int, bias: bool = True,
                  device=None, dtype=None) -> None:
         assert in_features % 4 == 0 and out_features % 4 == 0, "in_channels and out_channels must be divisible by 4"
         factory_kwargs = {'device': device, 'dtype': dtype}
         super().__init__()
         self.in_features = in_features
         self.out_features = out_features
-        self.r_weight = nn.Parameter(torch.empty((out_features//4, in_features//4), **factory_kwargs))
-        self.i_weight = nn.Parameter(torch.empty((out_features//4, in_features//4), **factory_kwargs))
-        self.j_weight = nn.Parameter(torch.empty((out_features//4, in_features//4), **factory_kwargs))
-        self.k_weight = nn.Parameter(torch.empty((out_features//4, in_features//4), **factory_kwargs))
+        a, b = out_features//4, in_features//4
+        self.r_weight = nn.Parameter(torch.empty((a, b), **factory_kwargs))
+        self.i_weight = nn.Parameter(torch.empty((a, b), **factory_kwargs))
+        self.j_weight = nn.Parameter(torch.empty((a, b), **factory_kwargs))
+        self.k_weight = nn.Parameter(torch.empty((a, b), **factory_kwargs))
         if bias:
             self.bias = nn.Parameter(torch.empty(out_features, **factory_kwargs))
         else:
             self.register_parameter('bias', None)
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
@@ -53,22 +54,28 @@
         if self.bias is not None:
             # fan_in, _ = nn.init._calculate_fan_in_and_fan_out(self.weight)
             fan_in = self.in_features * 4
             bound = 1 / math.sqrt(fan_in) if fan_in > 0 else 0
             nn.init.uniform_(self.bias, -bound, bound)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        weight = _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
+        weight = self.get_weight()
         return F.linear(x, weight, self.bias)
 
     def extra_repr(self) -> str:
         return f'in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}'
 
+    def get_weight(self):
+        return _construct_matrix(self.r_weight, self.i_weight, self.j_weight, self.k_weight)
 
 if __name__ == '__main__':
-    # model = nn.Linear(20, 16)
-    model = QLinear(20, 16)  # 20 and 16 are divisible by 4
-    x = torch.randn(128, 20)
-    output = model(x)
-    print(output.size())
-    # print(f"{model.weight.size() = }")
-    print(f"{model.r_weight.size() = },\n{model.i_weight.size() = },\n{model.j_weight.size() = },\n{model.k_weight.size() = }")
+    rmodel = nn.Linear(20, 16)
+    qmodel = QLinear(20, 16)
+    input_ = torch.randn(128, 20)
+    routput = rmodel(input_)
+    qoutput = qmodel(input_)
+    print(f"{rmodel.weight.size() = }")
+    print(f"{qmodel.r_weight.size() = }")
+    print(f"{qmodel.i_weight.size() = }")
+    print(f"{qmodel.j_weight.size() = }")
+    print(f"{qmodel.k_weight.size() = }")
+    print(f"{input_.size() = }\n{routput.size() = }\n{qoutput.size() = }")
```

### Comparing `qytorch-0.0.2/qytorch/qmha.py` & `qytorch-0.0.3/qytorch/qmha.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
 def _is_make_fx_tracing():
     if not torch.jit.is_scripting():
         torch_dispatch_mode_stack = torch.utils._python_dispatch._get_current_dispatch_mode_stack()
         return any(type(x) == torch.fx.experimental.proxy_tensor.ProxyTorchDispatchMode for x in torch_dispatch_mode_stack)
     else:
         return False
-    
-nn.Transformer
+
 
 class QMultiheadAttention(nn.Module):
     __constants__ = ['batch_first']
     bias_k: Optional[torch.Tensor]
     bias_v: Optional[torch.Tensor]
 
     def __init__(self, embed_dim, num_heads, dropout=0., bias=True, add_bias_kv=False, add_zero_attn=False,
```

### Comparing `qytorch-0.0.2/qytorch/qtransformer.py` & `qytorch-0.0.3/qytorch/qtransformer.py`

 * *Files identical despite different names*

