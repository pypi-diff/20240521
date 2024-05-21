# Comparing `tmp/ibis_substrait-3.2.0.tar.gz` & `tmp/ibis_substrait-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis_substrait-3.2.0.tar", max compression
+gzip compressed data, was "ibis_substrait-3.2.1.tar", max compression
```

## Comparing `ibis_substrait-3.2.0.tar` & `ibis_substrait-3.2.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0    11345 2024-02-06 22:27:38.887536 ibis_substrait-3.2.0/LICENSE
--rw-r--r--   0        0        0      951 2024-02-06 22:27:38.887536 ibis_substrait-3.2.0/README.md
--rw-r--r--   0        0        0      147 2024-02-06 22:28:51.084419 ibis_substrait-3.2.0/ibis_substrait/__init__.py
--rw-r--r--   0        0        0        0 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/compiler/__init__.py
--rw-r--r--   0        0        0    11401 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/compiler/core.py
--rw-r--r--   0        0        0     6127 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/compiler/mapping.py
--rw-r--r--   0        0        0    47662 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/compiler/translate.py
--rw-r--r--   0        0        0        0 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/__init__.py
--rw-r--r--   0        0        0      149 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/extension_types.yaml
--rw-r--r--   0        0        0      722 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_aggregate_approx.yaml
--rw-r--r--   0        0        0      921 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_aggregate_generic.yaml
--rw-r--r--   0        0        0    42855 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_arithmetic.yaml
--rw-r--r--   0        0        0     4467 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_arithmetic_decimal.yaml
--rw-r--r--   0        0        0     3252 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_boolean.yaml
--rw-r--r--   0        0        0     4956 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_comparison.yaml
--rw-r--r--   0        0        0     6238 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_datetime.yaml
--rw-r--r--   0        0        0     4213 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_logarithmic.yaml
--rw-r--r--   0        0        0    11507 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_rounding.yaml
--rw-r--r--   0        0        0      733 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_set.yaml
--rw-r--r--   0        0        0    47765 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/functions_string.yaml
--rw-r--r--   0        0        0      683 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/type_variations.yaml
--rw-r--r--   0        0        0     1302 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/extensions/unknown.yaml
--rw-r--r--   0        0        0        0 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/__init__.py
--rw-r--r--   0        0        0     4478 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/conftest.py
--rw-r--r--   0        0        0    28698 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h01/tpc_h01.json
--rw-r--r--   0        0        0    33305 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h03/tpc_h03.json
--rw-r--r--   0        0        0    25303 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h04/tpc_h04.json
--rw-r--r--   0        0        0    49297 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h05/tpc_h05.json
--rw-r--r--   0        0        0    17098 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h06/tpc_h06.json
--rw-r--r--   0        0        0    61665 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h07/tpc_h07.json
--rw-r--r--   0        0        0    56538 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h090/tpc_h090.json
--rw-r--r--   0        0        0    57146 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h091/tpc_h091.json
--rw-r--r--   0        0        0    55708 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h092/tpc_h092.json
--rw-r--r--   0        0        0    39777 2024-02-06 22:27:38.891536 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h10/tpc_h10.json
--rw-r--r--   0        0        0    21846 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h110/tpc_h110.json
--rw-r--r--   0        0        0    21846 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h111/tpc_h111.json
--rw-r--r--   0        0        0    35211 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h12/tpc_h12.json
--rw-r--r--   0        0        0    16583 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h13/tpc_h13.json
--rw-r--r--   0        0        0    24196 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h18/tpc_h18.json
--rw-r--r--   0        0        0    87218 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h19/tpc_h19.json
--rw-r--r--   0        0        0    11811 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h20/tpc_h20.json
--rw-r--r--   0        0        0    79098 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h21/tpc_h21.json
--rw-r--r--   0        0        0    29170 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h220/tpc_h220.json
--rw-r--r--   0        0        0    29170 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h221/tpc_h221.json
--rw-r--r--   0        0        0    17966 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_compiler.py
--rw-r--r--   0        0        0    11251 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_extensions.py
--rw-r--r--   0        0        0    11005 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_literal.py
--rw-r--r--   0        0        0    21666 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_tpch.py
--rw-r--r--   0        0        0      175 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/conftest.py
--rw-r--r--   0        0        0     6086 2024-02-06 22:27:38.895537 ibis_substrait-3.2.0/ibis_substrait/tests/integration/test_pyarrow.py
--rw-r--r--   0        0        0     4709 2024-02-06 22:28:53.076445 ibis_substrait-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 ibis_substrait-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/LICENSE
+-rw-r--r--   0        0        0      951 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/README.md
+-rw-r--r--   0        0        0      147 2024-05-21 16:25:33.512016 ibis_substrait-3.2.1/ibis_substrait/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/compiler/__init__.py
+-rw-r--r--   0        0        0    11408 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/compiler/core.py
+-rw-r--r--   0        0        0     6127 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/compiler/mapping.py
+-rw-r--r--   0        0        0    47697 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/compiler/translate.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/extension_types.yaml
+-rw-r--r--   0        0        0      722 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_aggregate_approx.yaml
+-rw-r--r--   0        0        0      921 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_aggregate_generic.yaml
+-rw-r--r--   0        0        0    42855 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_arithmetic.yaml
+-rw-r--r--   0        0        0     4467 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_arithmetic_decimal.yaml
+-rw-r--r--   0        0        0     3252 2024-05-21 16:24:41.875584 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_boolean.yaml
+-rw-r--r--   0        0        0     4956 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_comparison.yaml
+-rw-r--r--   0        0        0     6238 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_datetime.yaml
+-rw-r--r--   0        0        0     4213 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_logarithmic.yaml
+-rw-r--r--   0        0        0    11507 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_rounding.yaml
+-rw-r--r--   0        0        0      733 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_set.yaml
+-rw-r--r--   0        0        0    47765 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/functions_string.yaml
+-rw-r--r--   0        0        0      683 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/type_variations.yaml
+-rw-r--r--   0        0        0     1302 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/extensions/unknown.yaml
+-rw-r--r--   0        0        0        0 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/__init__.py
+-rw-r--r--   0        0        0     4478 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/conftest.py
+-rw-r--r--   0        0        0    28698 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h01/tpc_h01.json
+-rw-r--r--   0        0        0    33305 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h03/tpc_h03.json
+-rw-r--r--   0        0        0    25303 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h04/tpc_h04.json
+-rw-r--r--   0        0        0    49297 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h05/tpc_h05.json
+-rw-r--r--   0        0        0    17098 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h06/tpc_h06.json
+-rw-r--r--   0        0        0    61665 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h07/tpc_h07.json
+-rw-r--r--   0        0        0    57146 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h09_1/tpc_h09_1.json
+-rw-r--r--   0        0        0    55708 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h09_2/tpc_h09_2.json
+-rw-r--r--   0        0        0    39777 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h10/tpc_h10.json
+-rw-r--r--   0        0        0    21846 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h11_0/tpc_h11_0.json
+-rw-r--r--   0        0        0    21846 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h11_1/tpc_h11_1.json
+-rw-r--r--   0        0        0    35211 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h12/tpc_h12.json
+-rw-r--r--   0        0        0    16583 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h13/tpc_h13.json
+-rw-r--r--   0        0        0    24196 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h18/tpc_h18.json
+-rw-r--r--   0        0        0    87218 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h19/tpc_h19.json
+-rw-r--r--   0        0        0    11811 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h20/tpc_h20.json
+-rw-r--r--   0        0        0    79098 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h21/tpc_h21.json
+-rw-r--r--   0        0        0    29170 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h22_0/tpc_h22_0.json
+-rw-r--r--   0        0        0    29170 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h22_1/tpc_h22_1.json
+-rw-r--r--   0        0        0    17966 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_compiler.py
+-rw-r--r--   0        0        0    11251 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_extensions.py
+-rw-r--r--   0        0        0    11005 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_literal.py
+-rw-r--r--   0        0        0    21308 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_tpch.py
+-rw-r--r--   0        0        0      175 2024-05-21 16:24:41.879585 ibis_substrait-3.2.1/ibis_substrait/tests/conftest.py
+-rw-r--r--   0        0        0     6086 2024-05-21 16:24:41.883585 ibis_substrait-3.2.1/ibis_substrait/tests/integration/test_pyarrow.py
+-rw-r--r--   0        0        0     4715 2024-05-21 16:25:36.124037 ibis_substrait-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 ibis_substrait-3.2.1/PKG-INFO
```

### Comparing `ibis_substrait-3.2.0/LICENSE` & `ibis_substrait-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/README.md` & `ibis_substrait-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/compiler/core.py` & `ibis_substrait-3.2.1/ibis_substrait/compiler/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         """Initialize the compiler.
 
         Parameters
         ----------
         udf_uri
             The extension URI to use for looking up registered UDFs, if any.
             This is highly backend dependent.
+
         """
         self.extension_uris: dict[str, ste.SimpleExtensionURI] = {}
         self.function_extensions: dict[
             str | tuple[Hashable, ...],
             ste.SimpleExtensionDeclaration.ExtensionFunction,
         ] = {}
         self.type_extensions: dict[
@@ -70,27 +71,28 @@
             Ibis operation to use to lookup desired substrait scalar function
 
         Returns
         -------
         ste.ExtensionsFunctionId
             This is a unique identifier for a given operation type, *argument
             types N-tuple.
+
         """
 
         op_name = IBIS_SUBSTRAIT_OP_MAPPING[type(op).__name__]
         sig_key = self.get_signature(op)
 
         extension_signature = f"{op_name}:{'_'.join(sig_key)}"
 
         try:
             function_extension = self.function_extensions[extension_signature]
         except KeyError:
-            function_extension = self.function_extensions[
-                extension_signature
-            ] = self.create_extension(op_name, sig_key)
+            function_extension = self.function_extensions[extension_signature] = (
+                self.create_extension(op_name, sig_key)
+            )
         return function_extension.function_anchor
 
     def get_signature(self, op: ops.Node) -> tuple[str, ...]:
         """Validate and upcast (if necessary) scalar function extension signature."""
 
         op_name = IBIS_SUBSTRAIT_OP_MAPPING[type(op).__name__]
 
@@ -174,14 +176,15 @@
             function definition site
         scalar_func
             The name of the scalar function
 
         Returns
         -------
         ste.SimpleExtensionDeclaration.ExtensionFunction
+
         """
         return ste.SimpleExtensionDeclaration.ExtensionFunction(
             extension_uri_reference=extension_uri.extension_uri_anchor,
             function_anchor=next(self.id_generator),
             name=scalar_func,
         )
 
@@ -192,14 +195,15 @@
         ----------
         uri
             The URI pointing to the extension function definition location
 
         Returns
         -------
         ste.SimpleExtensionURI
+
         """
         try:
             extension_uri = self.extension_uris[uri]
         except KeyError:
             extension_uri = self.extension_uris[uri] = ste.SimpleExtensionURI(
                 # by convention, extension URIs start at 1
                 extension_uri_anchor=len(self.extension_uris) + 1,
@@ -285,14 +289,15 @@
     [(None, int64)]
     >>> map_type = dt.parse("map<string, string>")
     >>> list(_get_fields(map_type))
     [(None, String(nullable=True)), (None, String(nullable=True))]
     >>> struct_type = dt.parse("struct<a: int64, b: map<int64, float64>>")
     >>> list(_get_fields(struct_type))  # doctest: +SKIP
     [('b', Map(key_type=int64, value_type=float64, nullable=True)), ('a', int64)]
+
     """
     if isinstance(dtype, dt.Array):
         yield None, dtype.value_type
     elif isinstance(dtype, dt.Map):
         yield None, dtype.value_type
         yield None, dtype.key_type
     elif isinstance(dtype, dt.Struct):
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/compiler/mapping.py` & `ibis_substrait-3.2.1/ibis_substrait/compiler/mapping.py`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/compiler/translate.py` & `ibis_substrait-3.2.1/ibis_substrait/compiler/translate.py`

 * *Files 0% similar despite different names*

```diff
@@ -786,14 +786,15 @@
     >>> t2 = ibis.table([("d", "string"), ("e", "map<string, float64>")], name="t2")
     >>> expr = t1.join(t2, t1.b == t2.d)
     >>> mapping = _get_child_relation_field_offsets(expr.op())
     >>> mapping[t1.op()]  # the first relation is always zero
     0
     >>> mapping[t2.op()]  # first relation has 3 fields, so the second starts at 3
     3
+
     """
     if isinstance(table, ops.Join):
         # Descend into the left and right tables to grab offsets from nested joins
         left_keys = _get_child_relation_field_offsets(table.left)
         right_keys = _get_child_relation_field_offsets(table.right)
         root_tables = [table.left, table.right]
         accum = [0, len(root_tables[0].schema)]
@@ -1448,17 +1449,17 @@
     # Explicitly register extension uri
     extension_uri = compiler.register_extension_uri(compiler.udf_uri)
 
     # Explicitly register extension function
     try:
         func_ext = compiler.function_extensions[udf_key]
     except KeyError:
-        func_ext = compiler.function_extensions[
-            udf_key
-        ] = compiler.create_extension_function(extension_uri, op.func.__name__)
+        func_ext = compiler.function_extensions[udf_key] = (
+            compiler.create_extension_function(extension_uri, op.func.__name__)
+        )
 
     return stalg.Expression(
         scalar_function=stalg.Expression.ScalarFunction(
             function_reference=func_ext.function_anchor,
             output_type=translate(op.return_type),
             arguments=[
                 stalg.FunctionArgument(
@@ -1521,17 +1522,19 @@
 @_upcast.register(ops.Repeat)
 @_upcast.register(ops.StringFind)
 @_upcast.register(ops.LPad)
 @_upcast.register(ops.RPad)
 def _upcast_string_op(op: string_op) -> string_op:
     # Substrait wants Int32 for all numeric args to string functions
     casted_args = [
-        ops.Cast(newop, to=dt.Int32())  # type: ignore
-        if isinstance(newop.output_dtype, dt.SignedInteger)
-        else newop
+        (
+            ops.Cast(newop, to=dt.Int32())  # type: ignore
+            if isinstance(newop.output_dtype, dt.SignedInteger)
+            else newop
+        )
         for newop in op.args
     ]
     return type(op)(*casted_args)
 
 
 @_upcast.register(ops.Round)
 def _upcast_round_digits(op: ops.Round) -> ops.Round:
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_aggregate_approx.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_aggregate_approx.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_aggregate_generic.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_aggregate_generic.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_arithmetic.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_arithmetic.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_arithmetic_decimal.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_arithmetic_decimal.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_boolean.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_boolean.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_comparison.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_comparison.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_datetime.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_datetime.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_logarithmic.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_logarithmic.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_rounding.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_rounding.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_set.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_set.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/functions_string.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/functions_string.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/type_variations.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/type_variations.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/extensions/unknown.yaml` & `ibis_substrait-3.2.1/ibis_substrait/extensions/unknown.yaml`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/conftest.py` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/conftest.py`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h01/tpc_h01.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h01/tpc_h01.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -702,11 +702,11 @@
                     "avg_disc",
                     "count_order"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h03/tpc_h03.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h03/tpc_h03.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -724,11 +724,11 @@
                     "o_shippriority",
                     "revenue"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h04/tpc_h04.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h04/tpc_h04.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -504,11 +504,11 @@
                     "o_orderpriority",
                     "order_count"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h05/tpc_h05.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h05/tpc_h05.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -1008,11 +1008,11 @@
                     "n_name",
                     "revenue"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h06/tpc_h06.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h06/tpc_h06.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -435,11 +435,11 @@
                 "names": [
                     "revenue"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h07/tpc_h07.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h07/tpc_h07.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -1230,11 +1230,11 @@
                     "l_year",
                     "revenue"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h090/tpc_h090.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h09_1/tpc_h09_1.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9408069428943453%*

 * *Differences: {"'extensionUris'": "{2: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml'}, "*

 * *                    "3: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml'}, "*

 * *                    "4: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml'}}",*

 * * "'extensions'": "{2: {'extensionFunction': {'name': 'subtr […]*

```diff
@@ -6,23 +6,23 @@
         },
         {
             "extensionUriAnchor": 2,
             "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_boolean.yaml"
         },
         {
             "extensionUriAnchor": 3,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml"
         },
         {
             "extensionUriAnchor": 4,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml"
         },
         {
             "extensionUriAnchor": 5,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml"
         }
     ],
     "extensions": [
         {
             "extensionFunction": {
                 "extensionUriReference": 1,
                 "functionAnchor": 1,
@@ -36,41 +36,41 @@
                 "name": "and:bool"
             }
         },
         {
             "extensionFunction": {
                 "extensionUriReference": 3,
                 "functionAnchor": 3,
-                "name": "like:str_str"
+                "name": "subtract:dec_dec"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 4,
+                "extensionUriReference": 3,
                 "functionAnchor": 4,
-                "name": "subtract:dec_dec"
+                "name": "multiply:dec_dec"
             }
         },
         {
             "extensionFunction": {
                 "extensionUriReference": 4,
                 "functionAnchor": 5,
-                "name": "multiply:dec_dec"
+                "name": "extract:date"
             }
         },
         {
             "extensionFunction": {
                 "extensionUriReference": 5,
                 "functionAnchor": 6,
-                "name": "extract:date"
+                "name": "like:str_str"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 4,
+                "extensionUriReference": 3,
                 "functionAnchor": 7,
                 "name": "sum:dec"
             }
         }
     ],
     "relations": [
         {
@@ -87,277 +87,273 @@
                                                     "directReference": {
                                                         "structField": {
                                                             "field": 2
                                                         }
                                                     },
                                                     "rootReference": {}
                                                 }
-                                            }
-                                        ]
-                                    },
-                                    {
-                                        "groupingExpressions": [
+                                            },
                                             {
                                                 "selection": {
                                                     "directReference": {
                                                         "structField": {
                                                             "field": 1
                                                         }
                                                     },
                                                     "rootReference": {}
                                                 }
                                             }
                                         ]
                                     }
                                 ],
                                 "input": {
-                                    "project": {
-                                        "common": {
-                                            "emit": {
-                                                "outputMapping": [
-                                                    50,
-                                                    51,
-                                                    52,
-                                                    53
-                                                ]
+                                    "filter": {
+                                        "condition": {
+                                            "scalarFunction": {
+                                                "arguments": [
+                                                    {
+                                                        "value": {
+                                                            "selection": {
+                                                                "directReference": {
+                                                                    "structField": {
+                                                                        "field": 3
+                                                                    }
+                                                                },
+                                                                "rootReference": {}
+                                                            }
+                                                        }
+                                                    },
+                                                    {
+                                                        "value": {
+                                                            "literal": {
+                                                                "string": "%GREEN%"
+                                                            }
+                                                        }
+                                                    }
+                                                ],
+                                                "functionReference": 6,
+                                                "outputType": {
+                                                    "bool": {
+                                                        "nullability": "NULLABILITY_NULLABLE"
+                                                    }
+                                                }
                                             }
                                         },
-                                        "expressions": [
-                                            {
-                                                "scalarFunction": {
-                                                    "arguments": [
-                                                        {
-                                                            "value": {
-                                                                "scalarFunction": {
-                                                                    "arguments": [
-                                                                        {
-                                                                            "value": {
-                                                                                "selection": {
-                                                                                    "directReference": {
-                                                                                        "structField": {
-                                                                                            "field": 5
+                                        "input": {
+                                            "project": {
+                                                "common": {
+                                                    "emit": {
+                                                        "outputMapping": [
+                                                            50,
+                                                            51,
+                                                            52,
+                                                            53
+                                                        ]
+                                                    }
+                                                },
+                                                "expressions": [
+                                                    {
+                                                        "scalarFunction": {
+                                                            "arguments": [
+                                                                {
+                                                                    "value": {
+                                                                        "scalarFunction": {
+                                                                            "arguments": [
+                                                                                {
+                                                                                    "value": {
+                                                                                        "selection": {
+                                                                                            "directReference": {
+                                                                                                "structField": {
+                                                                                                    "field": 5
+                                                                                                }
+                                                                                            },
+                                                                                            "rootReference": {}
                                                                                         }
-                                                                                    },
-                                                                                    "rootReference": {}
-                                                                                }
-                                                                            }
-                                                                        },
-                                                                        {
-                                                                            "value": {
-                                                                                "scalarFunction": {
-                                                                                    "arguments": [
-                                                                                        {
-                                                                                            "value": {
-                                                                                                "cast": {
-                                                                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                                                                    "input": {
-                                                                                                        "literal": {
-                                                                                                            "i8": 1
+                                                                                    }
+                                                                                },
+                                                                                {
+                                                                                    "value": {
+                                                                                        "scalarFunction": {
+                                                                                            "arguments": [
+                                                                                                {
+                                                                                                    "value": {
+                                                                                                        "cast": {
+                                                                                                            "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
+                                                                                                            "input": {
+                                                                                                                "literal": {
+                                                                                                                    "i8": 1
+                                                                                                                }
+                                                                                                            },
+                                                                                                            "type": {
+                                                                                                                "decimal": {
+                                                                                                                    "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                    "precision": 15,
+                                                                                                                    "scale": 2
+                                                                                                                }
+                                                                                                            }
                                                                                                         }
-                                                                                                    },
-                                                                                                    "type": {
-                                                                                                        "decimal": {
-                                                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                                                            "precision": 15,
-                                                                                                            "scale": 2
+                                                                                                    }
+                                                                                                },
+                                                                                                {
+                                                                                                    "value": {
+                                                                                                        "selection": {
+                                                                                                            "directReference": {
+                                                                                                                "structField": {
+                                                                                                                    "field": 6
+                                                                                                                }
+                                                                                                            },
+                                                                                                            "rootReference": {}
                                                                                                         }
                                                                                                     }
                                                                                                 }
+                                                                                            ],
+                                                                                            "functionReference": 3,
+                                                                                            "outputType": {
+                                                                                                "decimal": {
+                                                                                                    "nullability": "NULLABILITY_NULLABLE",
+                                                                                                    "precision": 16,
+                                                                                                    "scale": 2
+                                                                                                }
                                                                                             }
-                                                                                        },
-                                                                                        {
-                                                                                            "value": {
+                                                                                        }
+                                                                                    }
+                                                                                }
+                                                                            ],
+                                                                            "functionReference": 4,
+                                                                            "outputType": {
+                                                                                "decimal": {
+                                                                                    "nullability": "NULLABILITY_NULLABLE",
+                                                                                    "precision": 30,
+                                                                                    "scale": 4
+                                                                                }
+                                                                            }
+                                                                        }
+                                                                    }
+                                                                },
+                                                                {
+                                                                    "value": {
+                                                                        "scalarFunction": {
+                                                                            "arguments": [
+                                                                                {
+                                                                                    "value": {
+                                                                                        "cast": {
+                                                                                            "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
+                                                                                            "input": {
                                                                                                 "selection": {
                                                                                                     "directReference": {
                                                                                                         "structField": {
-                                                                                                            "field": 6
+                                                                                                            "field": 26
                                                                                                         }
                                                                                                     },
                                                                                                     "rootReference": {}
                                                                                                 }
+                                                                                            },
+                                                                                            "type": {
+                                                                                                "decimal": {
+                                                                                                    "nullability": "NULLABILITY_NULLABLE",
+                                                                                                    "precision": 15,
+                                                                                                    "scale": 2
+                                                                                                }
                                                                                             }
                                                                                         }
-                                                                                    ],
-                                                                                    "functionReference": 4,
-                                                                                    "outputType": {
-                                                                                        "decimal": {
-                                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                                            "precision": 16,
-                                                                                            "scale": 2
-                                                                                        }
                                                                                     }
-                                                                                }
-                                                                            }
-                                                                        }
-                                                                    ],
-                                                                    "functionReference": 5,
-                                                                    "outputType": {
-                                                                        "decimal": {
-                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                            "precision": 30,
-                                                                            "scale": 4
-                                                                        }
-                                                                    }
-                                                                }
-                                                            }
-                                                        },
-                                                        {
-                                                            "value": {
-                                                                "scalarFunction": {
-                                                                    "arguments": [
-                                                                        {
-                                                                            "value": {
-                                                                                "cast": {
-                                                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                                                    "input": {
+                                                                                },
+                                                                                {
+                                                                                    "value": {
                                                                                         "selection": {
                                                                                             "directReference": {
                                                                                                 "structField": {
-                                                                                                    "field": 26
+                                                                                                    "field": 4
                                                                                                 }
                                                                                             },
                                                                                             "rootReference": {}
                                                                                         }
-                                                                                    },
-                                                                                    "type": {
-                                                                                        "decimal": {
-                                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                                            "precision": 15,
-                                                                                            "scale": 2
-                                                                                        }
                                                                                     }
                                                                                 }
+                                                                            ],
+                                                                            "functionReference": 4,
+                                                                            "outputType": {
+                                                                                "decimal": {
+                                                                                    "nullability": "NULLABILITY_NULLABLE",
+                                                                                    "precision": 30,
+                                                                                    "scale": 4
+                                                                                }
                                                                             }
+                                                                        }
+                                                                    }
+                                                                }
+                                                            ],
+                                                            "functionReference": 3,
+                                                            "outputType": {
+                                                                "decimal": {
+                                                                    "nullability": "NULLABILITY_NULLABLE",
+                                                                    "precision": 31,
+                                                                    "scale": 4
+                                                                }
+                                                            }
+                                                        }
+                                                    },
+                                                    {
+                                                        "cast": {
+                                                            "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
+                                                            "input": {
+                                                                "scalarFunction": {
+                                                                    "arguments": [
+                                                                        {
+                                                                            "enum": "YEAR"
                                                                         },
                                                                         {
                                                                             "value": {
                                                                                 "selection": {
                                                                                     "directReference": {
                                                                                         "structField": {
-                                                                                            "field": 4
+                                                                                            "field": 41
                                                                                         }
                                                                                     },
                                                                                     "rootReference": {}
                                                                                 }
                                                                             }
                                                                         }
                                                                     ],
                                                                     "functionReference": 5,
                                                                     "outputType": {
-                                                                        "decimal": {
-                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                            "precision": 30,
-                                                                            "scale": 4
-                                                                        }
-                                                                    }
-                                                                }
-                                                            }
-                                                        }
-                                                    ],
-                                                    "functionReference": 4,
-                                                    "outputType": {
-                                                        "decimal": {
-                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                            "precision": 31,
-                                                            "scale": 4
-                                                        }
-                                                    }
-                                                }
-                                            },
-                                            {
-                                                "cast": {
-                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                    "input": {
-                                                        "scalarFunction": {
-                                                            "arguments": [
-                                                                {
-                                                                    "enum": "YEAR"
-                                                                },
-                                                                {
-                                                                    "value": {
-                                                                        "selection": {
-                                                                            "directReference": {
-                                                                                "structField": {
-                                                                                    "field": 41
-                                                                                }
-                                                                            },
-                                                                            "rootReference": {}
+                                                                        "i32": {
+                                                                            "nullability": "NULLABILITY_NULLABLE"
                                                                         }
                                                                     }
                                                                 }
-                                                            ],
-                                                            "functionReference": 6,
-                                                            "outputType": {
-                                                                "i32": {
+                                                            },
+                                                            "type": {
+                                                                "string": {
                                                                     "nullability": "NULLABILITY_NULLABLE"
                                                                 }
                                                             }
                                                         }
                                                     },
-                                                    "type": {
-                                                        "string": {
-                                                            "nullability": "NULLABILITY_NULLABLE"
-                                                        }
-                                                    }
-                                                }
-                                            },
-                                            {
-                                                "selection": {
-                                                    "directReference": {
-                                                        "structField": {
-                                                            "field": 47
-                                                        }
-                                                    },
-                                                    "rootReference": {}
-                                                }
-                                            },
-                                            {
-                                                "selection": {
-                                                    "directReference": {
-                                                        "structField": {
-                                                            "field": 29
+                                                    {
+                                                        "selection": {
+                                                            "directReference": {
+                                                                "structField": {
+                                                                    "field": 47
+                                                                }
+                                                            },
+                                                            "rootReference": {}
                                                         }
                                                     },
-                                                    "rootReference": {}
-                                                }
-                                            }
-                                        ],
-                                        "input": {
-                                            "filter": {
-                                                "condition": {
-                                                    "scalarFunction": {
-                                                        "arguments": [
-                                                            {
-                                                                "value": {
-                                                                    "selection": {
-                                                                        "directReference": {
-                                                                            "structField": {
-                                                                                "field": 29
-                                                                            }
-                                                                        },
-                                                                        "rootReference": {}
-                                                                    }
+                                                    {
+                                                        "selection": {
+                                                            "directReference": {
+                                                                "structField": {
+                                                                    "field": 29
                                                                 }
                                                             },
-                                                            {
-                                                                "value": {
-                                                                    "literal": {
-                                                                        "string": "%GREEN%"
-                                                                    }
-                                                                }
-                                                            }
-                                                        ],
-                                                        "functionReference": 3,
-                                                        "outputType": {
-                                                            "bool": {
-                                                                "nullability": "NULLABILITY_NULLABLE"
-                                                            }
+                                                            "rootReference": {}
                                                         }
                                                     }
-                                                },
+                                                ],
                                                 "input": {
                                                     "join": {
                                                         "expression": {
                                                             "scalarFunction": {
                                                                 "arguments": [
                                                                     {
                                                                         "value": {
@@ -1117,11 +1113,11 @@
                     "o_year",
                     "sum_profit"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h091/tpc_h091.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h09_2/tpc_h09_2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9409086681547619%*

 * *Differences: {"'extensionUris'": "{2: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml'}, "*

 * *                    "3: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml'}, "*

 * *                    "4: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml'}}",*

 * * "'extensions'": "{2: {'extensionFunction': {'name': 'like: […]*

```diff
@@ -6,23 +6,23 @@
         },
         {
             "extensionUriAnchor": 2,
             "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_boolean.yaml"
         },
         {
             "extensionUriAnchor": 3,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml"
         },
         {
             "extensionUriAnchor": 4,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml"
         },
         {
             "extensionUriAnchor": 5,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml"
         }
     ],
     "extensions": [
         {
             "extensionFunction": {
                 "extensionUriReference": 1,
                 "functionAnchor": 1,
@@ -36,41 +36,41 @@
                 "name": "and:bool"
             }
         },
         {
             "extensionFunction": {
                 "extensionUriReference": 3,
                 "functionAnchor": 3,
-                "name": "subtract:dec_dec"
+                "name": "like:str_str"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 3,
+                "extensionUriReference": 4,
                 "functionAnchor": 4,
-                "name": "multiply:dec_dec"
+                "name": "subtract:dec_dec"
             }
         },
         {
             "extensionFunction": {
                 "extensionUriReference": 4,
                 "functionAnchor": 5,
-                "name": "extract:date"
+                "name": "multiply:dec_dec"
             }
         },
         {
             "extensionFunction": {
                 "extensionUriReference": 5,
                 "functionAnchor": 6,
-                "name": "like:str_str"
+                "name": "extract:date"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 3,
+                "extensionUriReference": 4,
                 "functionAnchor": 7,
                 "name": "sum:dec"
             }
         }
     ],
     "relations": [
         {
@@ -102,258 +102,246 @@
                                                     "rootReference": {}
                                                 }
                                             }
                                         ]
                                     }
                                 ],
                                 "input": {
-                                    "filter": {
-                                        "condition": {
-                                            "scalarFunction": {
-                                                "arguments": [
-                                                    {
-                                                        "value": {
-                                                            "selection": {
-                                                                "directReference": {
-                                                                    "structField": {
-                                                                        "field": 3
-                                                                    }
-                                                                },
-                                                                "rootReference": {}
-                                                            }
-                                                        }
-                                                    },
-                                                    {
-                                                        "value": {
-                                                            "literal": {
-                                                                "string": "%GREEN%"
-                                                            }
-                                                        }
-                                                    }
-                                                ],
-                                                "functionReference": 6,
-                                                "outputType": {
-                                                    "bool": {
-                                                        "nullability": "NULLABILITY_NULLABLE"
-                                                    }
-                                                }
+                                    "project": {
+                                        "common": {
+                                            "emit": {
+                                                "outputMapping": [
+                                                    50,
+                                                    51,
+                                                    52,
+                                                    53
+                                                ]
                                             }
                                         },
-                                        "input": {
-                                            "project": {
-                                                "common": {
-                                                    "emit": {
-                                                        "outputMapping": [
-                                                            50,
-                                                            51,
-                                                            52,
-                                                            53
-                                                        ]
-                                                    }
-                                                },
-                                                "expressions": [
-                                                    {
-                                                        "scalarFunction": {
-                                                            "arguments": [
-                                                                {
-                                                                    "value": {
-                                                                        "scalarFunction": {
-                                                                            "arguments": [
-                                                                                {
-                                                                                    "value": {
-                                                                                        "selection": {
-                                                                                            "directReference": {
-                                                                                                "structField": {
-                                                                                                    "field": 5
-                                                                                                }
-                                                                                            },
-                                                                                            "rootReference": {}
+                                        "expressions": [
+                                            {
+                                                "scalarFunction": {
+                                                    "arguments": [
+                                                        {
+                                                            "value": {
+                                                                "scalarFunction": {
+                                                                    "arguments": [
+                                                                        {
+                                                                            "value": {
+                                                                                "selection": {
+                                                                                    "directReference": {
+                                                                                        "structField": {
+                                                                                            "field": 5
                                                                                         }
-                                                                                    }
-                                                                                },
-                                                                                {
-                                                                                    "value": {
-                                                                                        "scalarFunction": {
-                                                                                            "arguments": [
-                                                                                                {
-                                                                                                    "value": {
-                                                                                                        "cast": {
-                                                                                                            "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                                                                            "input": {
-                                                                                                                "literal": {
-                                                                                                                    "i8": 1
-                                                                                                                }
-                                                                                                            },
-                                                                                                            "type": {
-                                                                                                                "decimal": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                                    "precision": 15,
-                                                                                                                    "scale": 2
-                                                                                                                }
-                                                                                                            }
+                                                                                    },
+                                                                                    "rootReference": {}
+                                                                                }
+                                                                            }
+                                                                        },
+                                                                        {
+                                                                            "value": {
+                                                                                "scalarFunction": {
+                                                                                    "arguments": [
+                                                                                        {
+                                                                                            "value": {
+                                                                                                "cast": {
+                                                                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
+                                                                                                    "input": {
+                                                                                                        "literal": {
+                                                                                                            "i8": 1
                                                                                                         }
-                                                                                                    }
-                                                                                                },
-                                                                                                {
-                                                                                                    "value": {
-                                                                                                        "selection": {
-                                                                                                            "directReference": {
-                                                                                                                "structField": {
-                                                                                                                    "field": 6
-                                                                                                                }
-                                                                                                            },
-                                                                                                            "rootReference": {}
+                                                                                                    },
+                                                                                                    "type": {
+                                                                                                        "decimal": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                                                            "precision": 15,
+                                                                                                            "scale": 2
                                                                                                         }
                                                                                                     }
                                                                                                 }
-                                                                                            ],
-                                                                                            "functionReference": 3,
-                                                                                            "outputType": {
-                                                                                                "decimal": {
-                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                    "precision": 16,
-                                                                                                    "scale": 2
-                                                                                                }
                                                                                             }
-                                                                                        }
-                                                                                    }
-                                                                                }
-                                                                            ],
-                                                                            "functionReference": 4,
-                                                                            "outputType": {
-                                                                                "decimal": {
-                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                    "precision": 30,
-                                                                                    "scale": 4
-                                                                                }
-                                                                            }
-                                                                        }
-                                                                    }
-                                                                },
-                                                                {
-                                                                    "value": {
-                                                                        "scalarFunction": {
-                                                                            "arguments": [
-                                                                                {
-                                                                                    "value": {
-                                                                                        "cast": {
-                                                                                            "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                                                            "input": {
+                                                                                        },
+                                                                                        {
+                                                                                            "value": {
                                                                                                 "selection": {
                                                                                                     "directReference": {
                                                                                                         "structField": {
-                                                                                                            "field": 26
+                                                                                                            "field": 6
                                                                                                         }
                                                                                                     },
                                                                                                     "rootReference": {}
                                                                                                 }
-                                                                                            },
-                                                                                            "type": {
-                                                                                                "decimal": {
-                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                    "precision": 15,
-                                                                                                    "scale": 2
-                                                                                                }
                                                                                             }
                                                                                         }
-                                                                                    }
-                                                                                },
-                                                                                {
-                                                                                    "value": {
-                                                                                        "selection": {
-                                                                                            "directReference": {
-                                                                                                "structField": {
-                                                                                                    "field": 4
-                                                                                                }
-                                                                                            },
-                                                                                            "rootReference": {}
+                                                                                    ],
+                                                                                    "functionReference": 4,
+                                                                                    "outputType": {
+                                                                                        "decimal": {
+                                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                                            "precision": 16,
+                                                                                            "scale": 2
                                                                                         }
                                                                                     }
                                                                                 }
-                                                                            ],
-                                                                            "functionReference": 4,
-                                                                            "outputType": {
-                                                                                "decimal": {
-                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                    "precision": 30,
-                                                                                    "scale": 4
-                                                                                }
                                                                             }
                                                                         }
+                                                                    ],
+                                                                    "functionReference": 5,
+                                                                    "outputType": {
+                                                                        "decimal": {
+                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                            "precision": 30,
+                                                                            "scale": 4
+                                                                        }
                                                                     }
                                                                 }
-                                                            ],
-                                                            "functionReference": 3,
-                                                            "outputType": {
-                                                                "decimal": {
-                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                    "precision": 31,
-                                                                    "scale": 4
-                                                                }
                                                             }
-                                                        }
-                                                    },
-                                                    {
-                                                        "cast": {
-                                                            "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                            "input": {
+                                                        },
+                                                        {
+                                                            "value": {
                                                                 "scalarFunction": {
                                                                     "arguments": [
                                                                         {
-                                                                            "enum": "YEAR"
+                                                                            "value": {
+                                                                                "selection": {
+                                                                                    "directReference": {
+                                                                                        "structField": {
+                                                                                            "field": 26
+                                                                                        }
+                                                                                    },
+                                                                                    "rootReference": {}
+                                                                                }
+                                                                            }
                                                                         },
                                                                         {
                                                                             "value": {
                                                                                 "selection": {
                                                                                     "directReference": {
                                                                                         "structField": {
-                                                                                            "field": 41
+                                                                                            "field": 4
                                                                                         }
                                                                                     },
                                                                                     "rootReference": {}
                                                                                 }
                                                                             }
                                                                         }
                                                                     ],
                                                                     "functionReference": 5,
                                                                     "outputType": {
-                                                                        "i32": {
-                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                        "decimal": {
+                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                            "precision": 30,
+                                                                            "scale": 4
                                                                         }
                                                                     }
                                                                 }
-                                                            },
-                                                            "type": {
-                                                                "string": {
+                                                            }
+                                                        }
+                                                    ],
+                                                    "functionReference": 4,
+                                                    "outputType": {
+                                                        "decimal": {
+                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                            "precision": 31,
+                                                            "scale": 4
+                                                        }
+                                                    }
+                                                }
+                                            },
+                                            {
+                                                "cast": {
+                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
+                                                    "input": {
+                                                        "scalarFunction": {
+                                                            "arguments": [
+                                                                {
+                                                                    "enum": "YEAR"
+                                                                },
+                                                                {
+                                                                    "value": {
+                                                                        "selection": {
+                                                                            "directReference": {
+                                                                                "structField": {
+                                                                                    "field": 41
+                                                                                }
+                                                                            },
+                                                                            "rootReference": {}
+                                                                        }
+                                                                    }
+                                                                }
+                                                            ],
+                                                            "functionReference": 6,
+                                                            "outputType": {
+                                                                "i32": {
                                                                     "nullability": "NULLABILITY_NULLABLE"
                                                                 }
                                                             }
                                                         }
                                                     },
-                                                    {
-                                                        "selection": {
-                                                            "directReference": {
-                                                                "structField": {
-                                                                    "field": 47
-                                                                }
-                                                            },
-                                                            "rootReference": {}
+                                                    "type": {
+                                                        "string": {
+                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                        }
+                                                    }
+                                                }
+                                            },
+                                            {
+                                                "selection": {
+                                                    "directReference": {
+                                                        "structField": {
+                                                            "field": 47
                                                         }
                                                     },
-                                                    {
-                                                        "selection": {
-                                                            "directReference": {
-                                                                "structField": {
-                                                                    "field": 29
+                                                    "rootReference": {}
+                                                }
+                                            },
+                                            {
+                                                "selection": {
+                                                    "directReference": {
+                                                        "structField": {
+                                                            "field": 29
+                                                        }
+                                                    },
+                                                    "rootReference": {}
+                                                }
+                                            }
+                                        ],
+                                        "input": {
+                                            "filter": {
+                                                "condition": {
+                                                    "scalarFunction": {
+                                                        "arguments": [
+                                                            {
+                                                                "value": {
+                                                                    "selection": {
+                                                                        "directReference": {
+                                                                            "structField": {
+                                                                                "field": 29
+                                                                            }
+                                                                        },
+                                                                        "rootReference": {}
+                                                                    }
                                                                 }
                                                             },
-                                                            "rootReference": {}
+                                                            {
+                                                                "value": {
+                                                                    "literal": {
+                                                                        "string": "%GREEN%"
+                                                                    }
+                                                                }
+                                                            }
+                                                        ],
+                                                        "functionReference": 3,
+                                                        "outputType": {
+                                                            "bool": {
+                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                            }
                                                         }
                                                     }
-                                                ],
+                                                },
                                                 "input": {
                                                     "join": {
                                                         "expression": {
                                                             "scalarFunction": {
                                                                 "arguments": [
                                                                     {
                                                                         "value": {
@@ -1113,11 +1101,11 @@
                     "o_year",
                     "sum_profit"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h092/tpc_h092.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h21/tpc_h21.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8514880952380952%*

 * *Differences: {"'extensionUris'": "{2: {'uri': "*

 * *                    "'https://github.com/substrait-io/substrait/blob/main/extensions/functions_aggregate_generic.yaml'}, "*

 * *                    'delete: [4, 3]}',*

 * * "'extensions'": "{2: {'extensionFunction': {'extensionUriReference': 1, 'name': 'gt:any_any'}}, "*

 * *                 "3: {'extensionFunction': {'extensionUriReference': 1, 'name': "*

 * *                 "'not_equal:any_any'}}, 4: {'extensionFunction': {'extensionUriReference': 2, "*

 * *                 "'name': 'not:bool'} […]*

```diff
@@ -6,23 +6,15 @@
         },
         {
             "extensionUriAnchor": 2,
             "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_boolean.yaml"
         },
         {
             "extensionUriAnchor": 3,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_string.yaml"
-        },
-        {
-            "extensionUriAnchor": 4,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_arithmetic_decimal.yaml"
-        },
-        {
-            "extensionUriAnchor": 5,
-            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_datetime.yaml"
+            "uri": "https://github.com/substrait-io/substrait/blob/main/extensions/functions_aggregate_generic.yaml"
         }
     ],
     "extensions": [
         {
             "extensionFunction": {
                 "extensionUriReference": 1,
                 "functionAnchor": 1,
@@ -34,374 +26,848 @@
                 "extensionUriReference": 2,
                 "functionAnchor": 2,
                 "name": "and:bool"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 3,
+                "extensionUriReference": 1,
                 "functionAnchor": 3,
-                "name": "like:str_str"
+                "name": "gt:any_any"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 4,
+                "extensionUriReference": 1,
                 "functionAnchor": 4,
-                "name": "subtract:dec_dec"
+                "name": "not_equal:any_any"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 4,
+                "extensionUriReference": 2,
                 "functionAnchor": 5,
-                "name": "multiply:dec_dec"
+                "name": "not:bool"
             }
         },
         {
             "extensionFunction": {
-                "extensionUriReference": 5,
+                "extensionUriReference": 3,
                 "functionAnchor": 6,
-                "name": "extract:date"
-            }
-        },
-        {
-            "extensionFunction": {
-                "extensionUriReference": 4,
-                "functionAnchor": 7,
-                "name": "sum:dec"
+                "name": "count:any"
             }
         }
     ],
     "relations": [
         {
             "root": {
                 "input": {
-                    "sort": {
+                    "fetch": {
+                        "count": "100",
                         "input": {
-                            "aggregate": {
-                                "groupings": [
-                                    {
-                                        "groupingExpressions": [
-                                            {
-                                                "selection": {
-                                                    "directReference": {
-                                                        "structField": {
-                                                            "field": 2
-                                                        }
-                                                    },
-                                                    "rootReference": {}
-                                                }
-                                            },
+                            "sort": {
+                                "input": {
+                                    "aggregate": {
+                                        "groupings": [
                                             {
-                                                "selection": {
-                                                    "directReference": {
-                                                        "structField": {
-                                                            "field": 1
+                                                "groupingExpressions": [
+                                                    {
+                                                        "selection": {
+                                                            "directReference": {
+                                                                "structField": {
+                                                                    "field": 5
+                                                                }
+                                                            },
+                                                            "rootReference": {}
                                                         }
-                                                    },
-                                                    "rootReference": {}
-                                                }
-                                            }
-                                        ]
-                                    }
-                                ],
-                                "input": {
-                                    "project": {
-                                        "common": {
-                                            "emit": {
-                                                "outputMapping": [
-                                                    50,
-                                                    51,
-                                                    52,
-                                                    53
+                                                    }
                                                 ]
                                             }
-                                        },
-                                        "expressions": [
-                                            {
-                                                "scalarFunction": {
-                                                    "arguments": [
-                                                        {
-                                                            "value": {
-                                                                "scalarFunction": {
-                                                                    "arguments": [
-                                                                        {
-                                                                            "value": {
-                                                                                "selection": {
-                                                                                    "directReference": {
-                                                                                        "structField": {
-                                                                                            "field": 5
-                                                                                        }
-                                                                                    },
-                                                                                    "rootReference": {}
-                                                                                }
-                                                                            }
-                                                                        },
-                                                                        {
-                                                                            "value": {
-                                                                                "scalarFunction": {
-                                                                                    "arguments": [
-                                                                                        {
-                                                                                            "value": {
-                                                                                                "cast": {
-                                                                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                                                                    "input": {
-                                                                                                        "literal": {
-                                                                                                            "i8": 1
+                                        ],
+                                        "input": {
+                                            "filter": {
+                                                "condition": {
+                                                    "scalarFunction": {
+                                                        "arguments": [
+                                                            {
+                                                                "value": {
+                                                                    "scalarFunction": {
+                                                                        "arguments": [
+                                                                            {
+                                                                                "value": {
+                                                                                    "scalarFunction": {
+                                                                                        "arguments": [
+                                                                                            {
+                                                                                                "value": {
+                                                                                                    "scalarFunction": {
+                                                                                                        "arguments": [
+                                                                                                            {
+                                                                                                                "value": {
+                                                                                                                    "scalarFunction": {
+                                                                                                                        "arguments": [
+                                                                                                                            {
+                                                                                                                                "value": {
+                                                                                                                                    "selection": {
+                                                                                                                                        "directReference": {
+                                                                                                                                            "structField": {
+                                                                                                                                                "field": 1
+                                                                                                                                            }
+                                                                                                                                        },
+                                                                                                                                        "rootReference": {}
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            },
+                                                                                                                            {
+                                                                                                                                "value": {
+                                                                                                                                    "literal": {
+                                                                                                                                        "string": "F"
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            }
+                                                                                                                        ],
+                                                                                                                        "functionReference": 1,
+                                                                                                                        "outputType": {
+                                                                                                                            "bool": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    }
+                                                                                                                }
+                                                                                                            },
+                                                                                                            {
+                                                                                                                "value": {
+                                                                                                                    "scalarFunction": {
+                                                                                                                        "arguments": [
+                                                                                                                            {
+                                                                                                                                "value": {
+                                                                                                                                    "selection": {
+                                                                                                                                        "directReference": {
+                                                                                                                                            "structField": {
+                                                                                                                                                "field": 2
+                                                                                                                                            }
+                                                                                                                                        },
+                                                                                                                                        "rootReference": {}
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            },
+                                                                                                                            {
+                                                                                                                                "value": {
+                                                                                                                                    "selection": {
+                                                                                                                                        "directReference": {
+                                                                                                                                            "structField": {
+                                                                                                                                                "field": 3
+                                                                                                                                            }
+                                                                                                                                        },
+                                                                                                                                        "rootReference": {}
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            }
+                                                                                                                        ],
+                                                                                                                        "functionReference": 3,
+                                                                                                                        "outputType": {
+                                                                                                                            "bool": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    }
+                                                                                                                }
+                                                                                                            }
+                                                                                                        ],
+                                                                                                        "functionReference": 2,
+                                                                                                        "outputType": {
+                                                                                                            "bool": {
+                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                            }
                                                                                                         }
-                                                                                                    },
-                                                                                                    "type": {
-                                                                                                        "decimal": {
-                                                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                                                            "precision": 15,
-                                                                                                            "scale": 2
+                                                                                                    }
+                                                                                                }
+                                                                                            },
+                                                                                            {
+                                                                                                "value": {
+                                                                                                    "scalarFunction": {
+                                                                                                        "arguments": [
+                                                                                                            {
+                                                                                                                "value": {
+                                                                                                                    "selection": {
+                                                                                                                        "directReference": {
+                                                                                                                            "structField": {
+                                                                                                                                "field": 6
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        "rootReference": {}
+                                                                                                                    }
+                                                                                                                }
+                                                                                                            },
+                                                                                                            {
+                                                                                                                "value": {
+                                                                                                                    "literal": {
+                                                                                                                        "string": "SAUDI ARABIA"
+                                                                                                                    }
+                                                                                                                }
+                                                                                                            }
+                                                                                                        ],
+                                                                                                        "functionReference": 1,
+                                                                                                        "outputType": {
+                                                                                                            "bool": {
+                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                            }
                                                                                                         }
                                                                                                     }
                                                                                                 }
                                                                                             }
-                                                                                        },
-                                                                                        {
-                                                                                            "value": {
-                                                                                                "selection": {
-                                                                                                    "directReference": {
-                                                                                                        "structField": {
-                                                                                                            "field": 6
+                                                                                        ],
+                                                                                        "functionReference": 2,
+                                                                                        "outputType": {
+                                                                                            "bool": {
+                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                            }
+                                                                                        }
+                                                                                    }
+                                                                                }
+                                                                            },
+                                                                            {
+                                                                                "value": {
+                                                                                    "subquery": {
+                                                                                        "setPredicate": {
+                                                                                            "predicateOp": "PREDICATE_OP_EXISTS",
+                                                                                            "tuples": {
+                                                                                                "filter": {
+                                                                                                    "condition": {
+                                                                                                        "scalarFunction": {
+                                                                                                            "arguments": [
+                                                                                                                {
+                                                                                                                    "value": {
+                                                                                                                        "scalarFunction": {
+                                                                                                                            "arguments": [
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "selection": {
+                                                                                                                                            "directReference": {
+                                                                                                                                                "structField": {}
+                                                                                                                                            },
+                                                                                                                                            "rootReference": {}
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                },
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "selection": {
+                                                                                                                                            "directReference": {
+                                                                                                                                                "structField": {}
+                                                                                                                                            },
+                                                                                                                                            "rootReference": {}
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            ],
+                                                                                                                            "functionReference": 1,
+                                                                                                                            "outputType": {
+                                                                                                                                "bool": {
+                                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                                }
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    }
+                                                                                                                },
+                                                                                                                {
+                                                                                                                    "value": {
+                                                                                                                        "scalarFunction": {
+                                                                                                                            "arguments": [
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "selection": {
+                                                                                                                                            "directReference": {
+                                                                                                                                                "structField": {
+                                                                                                                                                    "field": 2
+                                                                                                                                                }
+                                                                                                                                            },
+                                                                                                                                            "rootReference": {}
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                },
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "selection": {
+                                                                                                                                            "directReference": {
+                                                                                                                                                "structField": {
+                                                                                                                                                    "field": 4
+                                                                                                                                                }
+                                                                                                                                            },
+                                                                                                                                            "rootReference": {}
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            ],
+                                                                                                                            "functionReference": 4,
+                                                                                                                            "outputType": {
+                                                                                                                                "bool": {
+                                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                                }
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    }
+                                                                                                                }
+                                                                                                            ],
+                                                                                                            "functionReference": 2,
+                                                                                                            "outputType": {
+                                                                                                                "bool": {
+                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                }
+                                                                                                            }
                                                                                                         }
                                                                                                     },
-                                                                                                    "rootReference": {}
+                                                                                                    "input": {
+                                                                                                        "read": {
+                                                                                                            "baseSchema": {
+                                                                                                                "names": [
+                                                                                                                    "l_orderkey",
+                                                                                                                    "l_partkey",
+                                                                                                                    "l_suppkey",
+                                                                                                                    "l_linenumber",
+                                                                                                                    "l_quantity",
+                                                                                                                    "l_extendedprice",
+                                                                                                                    "l_discount",
+                                                                                                                    "l_tax",
+                                                                                                                    "l_returnflag",
+                                                                                                                    "l_linestatus",
+                                                                                                                    "l_shipdate",
+                                                                                                                    "l_commitdate",
+                                                                                                                    "l_receiptdate",
+                                                                                                                    "l_shipinstruct",
+                                                                                                                    "l_shipmode",
+                                                                                                                    "l_comment"
+                                                                                                                ],
+                                                                                                                "struct": {
+                                                                                                                    "nullability": "NULLABILITY_REQUIRED",
+                                                                                                                    "types": [
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "date": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "date": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "date": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    ]
+                                                                                                                }
+                                                                                                            },
+                                                                                                            "common": {
+                                                                                                                "direct": {}
+                                                                                                            },
+                                                                                                            "namedTable": {
+                                                                                                                "names": [
+                                                                                                                    "lineitem"
+                                                                                                                ]
+                                                                                                            }
+                                                                                                        }
+                                                                                                    }
                                                                                                 }
                                                                                             }
                                                                                         }
-                                                                                    ],
-                                                                                    "functionReference": 4,
-                                                                                    "outputType": {
-                                                                                        "decimal": {
-                                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                                            "precision": 16,
-                                                                                            "scale": 2
-                                                                                        }
                                                                                     }
                                                                                 }
                                                                             }
-                                                                        }
-                                                                    ],
-                                                                    "functionReference": 5,
-                                                                    "outputType": {
-                                                                        "decimal": {
-                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                            "precision": 30,
-                                                                            "scale": 4
+                                                                        ],
+                                                                        "functionReference": 2,
+                                                                        "outputType": {
+                                                                            "bool": {
+                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                            }
                                                                         }
                                                                     }
                                                                 }
-                                                            }
-                                                        },
-                                                        {
-                                                            "value": {
-                                                                "scalarFunction": {
-                                                                    "arguments": [
-                                                                        {
-                                                                            "value": {
-                                                                                "selection": {
-                                                                                    "directReference": {
-                                                                                        "structField": {
-                                                                                            "field": 26
+                                                            },
+                                                            {
+                                                                "value": {
+                                                                    "scalarFunction": {
+                                                                        "arguments": [
+                                                                            {
+                                                                                "value": {
+                                                                                    "subquery": {
+                                                                                        "setPredicate": {
+                                                                                            "predicateOp": "PREDICATE_OP_EXISTS",
+                                                                                            "tuples": {
+                                                                                                "filter": {
+                                                                                                    "condition": {
+                                                                                                        "scalarFunction": {
+                                                                                                            "arguments": [
+                                                                                                                {
+                                                                                                                    "value": {
+                                                                                                                        "scalarFunction": {
+                                                                                                                            "arguments": [
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "scalarFunction": {
+                                                                                                                                            "arguments": [
+                                                                                                                                                {
+                                                                                                                                                    "value": {
+                                                                                                                                                        "selection": {
+                                                                                                                                                            "directReference": {
+                                                                                                                                                                "structField": {}
+                                                                                                                                                            },
+                                                                                                                                                            "rootReference": {}
+                                                                                                                                                        }
+                                                                                                                                                    }
+                                                                                                                                                },
+                                                                                                                                                {
+                                                                                                                                                    "value": {
+                                                                                                                                                        "selection": {
+                                                                                                                                                            "directReference": {
+                                                                                                                                                                "structField": {}
+                                                                                                                                                            },
+                                                                                                                                                            "rootReference": {}
+                                                                                                                                                        }
+                                                                                                                                                    }
+                                                                                                                                                }
+                                                                                                                                            ],
+                                                                                                                                            "functionReference": 1,
+                                                                                                                                            "outputType": {
+                                                                                                                                                "bool": {
+                                                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                                                }
+                                                                                                                                            }
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                },
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "scalarFunction": {
+                                                                                                                                            "arguments": [
+                                                                                                                                                {
+                                                                                                                                                    "value": {
+                                                                                                                                                        "selection": {
+                                                                                                                                                            "directReference": {
+                                                                                                                                                                "structField": {
+                                                                                                                                                                    "field": 2
+                                                                                                                                                                }
+                                                                                                                                                            },
+                                                                                                                                                            "rootReference": {}
+                                                                                                                                                        }
+                                                                                                                                                    }
+                                                                                                                                                },
+                                                                                                                                                {
+                                                                                                                                                    "value": {
+                                                                                                                                                        "selection": {
+                                                                                                                                                            "directReference": {
+                                                                                                                                                                "structField": {
+                                                                                                                                                                    "field": 4
+                                                                                                                                                                }
+                                                                                                                                                            },
+                                                                                                                                                            "rootReference": {}
+                                                                                                                                                        }
+                                                                                                                                                    }
+                                                                                                                                                }
+                                                                                                                                            ],
+                                                                                                                                            "functionReference": 4,
+                                                                                                                                            "outputType": {
+                                                                                                                                                "bool": {
+                                                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                                                }
+                                                                                                                                            }
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            ],
+                                                                                                                            "functionReference": 2,
+                                                                                                                            "outputType": {
+                                                                                                                                "bool": {
+                                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                                }
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    }
+                                                                                                                },
+                                                                                                                {
+                                                                                                                    "value": {
+                                                                                                                        "scalarFunction": {
+                                                                                                                            "arguments": [
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "selection": {
+                                                                                                                                            "directReference": {
+                                                                                                                                                "structField": {
+                                                                                                                                                    "field": 12
+                                                                                                                                                }
+                                                                                                                                            },
+                                                                                                                                            "rootReference": {}
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                },
+                                                                                                                                {
+                                                                                                                                    "value": {
+                                                                                                                                        "selection": {
+                                                                                                                                            "directReference": {
+                                                                                                                                                "structField": {
+                                                                                                                                                    "field": 11
+                                                                                                                                                }
+                                                                                                                                            },
+                                                                                                                                            "rootReference": {}
+                                                                                                                                        }
+                                                                                                                                    }
+                                                                                                                                }
+                                                                                                                            ],
+                                                                                                                            "functionReference": 3,
+                                                                                                                            "outputType": {
+                                                                                                                                "bool": {
+                                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                                }
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    }
+                                                                                                                }
+                                                                                                            ],
+                                                                                                            "functionReference": 2,
+                                                                                                            "outputType": {
+                                                                                                                "bool": {
+                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                }
+                                                                                                            }
+                                                                                                        }
+                                                                                                    },
+                                                                                                    "input": {
+                                                                                                        "read": {
+                                                                                                            "baseSchema": {
+                                                                                                                "names": [
+                                                                                                                    "l_orderkey",
+                                                                                                                    "l_partkey",
+                                                                                                                    "l_suppkey",
+                                                                                                                    "l_linenumber",
+                                                                                                                    "l_quantity",
+                                                                                                                    "l_extendedprice",
+                                                                                                                    "l_discount",
+                                                                                                                    "l_tax",
+                                                                                                                    "l_returnflag",
+                                                                                                                    "l_linestatus",
+                                                                                                                    "l_shipdate",
+                                                                                                                    "l_commitdate",
+                                                                                                                    "l_receiptdate",
+                                                                                                                    "l_shipinstruct",
+                                                                                                                    "l_shipmode",
+                                                                                                                    "l_comment"
+                                                                                                                ],
+                                                                                                                "struct": {
+                                                                                                                    "nullability": "NULLABILITY_REQUIRED",
+                                                                                                                    "types": [
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "i64": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "decimal": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE",
+                                                                                                                                "precision": 15,
+                                                                                                                                "scale": 2
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "date": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "date": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "date": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        },
+                                                                                                                        {
+                                                                                                                            "string": {
+                                                                                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                                                                                            }
+                                                                                                                        }
+                                                                                                                    ]
+                                                                                                                }
+                                                                                                            },
+                                                                                                            "common": {
+                                                                                                                "direct": {}
+                                                                                                            },
+                                                                                                            "namedTable": {
+                                                                                                                "names": [
+                                                                                                                    "lineitem"
+                                                                                                                ]
+                                                                                                            }
+                                                                                                        }
+                                                                                                    }
+                                                                                                }
+                                                                                            }
                                                                                         }
-                                                                                    },
-                                                                                    "rootReference": {}
+                                                                                    }
                                                                                 }
                                                                             }
-                                                                        },
-                                                                        {
-                                                                            "value": {
-                                                                                "selection": {
-                                                                                    "directReference": {
-                                                                                        "structField": {
-                                                                                            "field": 4
-                                                                                        }
-                                                                                    },
-                                                                                    "rootReference": {}
-                                                                                }
+                                                                        ],
+                                                                        "functionReference": 5,
+                                                                        "outputType": {
+                                                                            "bool": {
+                                                                                "nullability": "NULLABILITY_NULLABLE"
                                                                             }
                                                                         }
-                                                                    ],
-                                                                    "functionReference": 5,
-                                                                    "outputType": {
-                                                                        "decimal": {
-                                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                                            "precision": 30,
-                                                                            "scale": 4
-                                                                        }
                                                                     }
                                                                 }
                                                             }
-                                                        }
-                                                    ],
-                                                    "functionReference": 4,
-                                                    "outputType": {
-                                                        "decimal": {
-                                                            "nullability": "NULLABILITY_NULLABLE",
-                                                            "precision": 31,
-                                                            "scale": 4
+                                                        ],
+                                                        "functionReference": 2,
+                                                        "outputType": {
+                                                            "bool": {
+                                                                "nullability": "NULLABILITY_NULLABLE"
+                                                            }
                                                         }
                                                     }
-                                                }
-                                            },
-                                            {
-                                                "cast": {
-                                                    "failureBehavior": "FAILURE_BEHAVIOR_THROW_EXCEPTION",
-                                                    "input": {
-                                                        "scalarFunction": {
-                                                            "arguments": [
-                                                                {
-                                                                    "enum": "YEAR"
-                                                                },
-                                                                {
-                                                                    "value": {
-                                                                        "selection": {
-                                                                            "directReference": {
-                                                                                "structField": {
-                                                                                    "field": 41
-                                                                                }
-                                                                            },
-                                                                            "rootReference": {}
+                                                },
+                                                "input": {
+                                                    "project": {
+                                                        "common": {
+                                                            "emit": {
+                                                                "outputMapping": [
+                                                                    36,
+                                                                    37,
+                                                                    38,
+                                                                    39,
+                                                                    40,
+                                                                    41,
+                                                                    42
+                                                                ]
+                                                            }
+                                                        },
+                                                        "expressions": [
+                                                            {
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 7
                                                                         }
-                                                                    }
+                                                                    },
+                                                                    "rootReference": {}
                                                                 }
-                                                            ],
-                                                            "functionReference": 6,
-                                                            "outputType": {
-                                                                "i32": {
-                                                                    "nullability": "NULLABILITY_NULLABLE"
+                                                            },
+                                                            {
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 25
+                                                                        }
+                                                                    },
+                                                                    "rootReference": {}
                                                                 }
-                                                            }
-                                                        }
-                                                    },
-                                                    "type": {
-                                                        "string": {
-                                                            "nullability": "NULLABILITY_NULLABLE"
-                                                        }
-                                                    }
-                                                }
-                                            },
-                                            {
-                                                "selection": {
-                                                    "directReference": {
-                                                        "structField": {
-                                                            "field": 47
-                                                        }
-                                                    },
-                                                    "rootReference": {}
-                                                }
-                                            },
-                                            {
-                                                "selection": {
-                                                    "directReference": {
-                                                        "structField": {
-                                                            "field": 29
-                                                        }
-                                                    },
-                                                    "rootReference": {}
-                                                }
-                                            }
-                                        ],
-                                        "input": {
-                                            "filter": {
-                                                "condition": {
-                                                    "scalarFunction": {
-                                                        "arguments": [
+                                                            },
                                                             {
-                                                                "value": {
-                                                                    "selection": {
-                                                                        "directReference": {
-                                                                            "structField": {
-                                                                                "field": 29
-                                                                            }
-                                                                        },
-                                                                        "rootReference": {}
-                                                                    }
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 19
+                                                                        }
+                                                                    },
+                                                                    "rootReference": {}
                                                                 }
                                                             },
                                                             {
-                                                                "value": {
-                                                                    "literal": {
-                                                                        "string": "%GREEN%"
-                                                                    }
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 18
+                                                                        }
+                                                                    },
+                                                                    "rootReference": {}
                                                                 }
-                                                            }
-                                                        ],
-                                                        "functionReference": 3,
-                                                        "outputType": {
-                                                            "bool": {
-                                                                "nullability": "NULLABILITY_NULLABLE"
-                                                            }
-                                                        }
-                                                    }
-                                                },
-                                                "input": {
-                                                    "join": {
-                                                        "expression": {
-                                                            "scalarFunction": {
-                                                                "arguments": [
-                                                                    {
-                                                                        "value": {
-                                                                            "selection": {
-                                                                                "directReference": {
-                                                                                    "structField": {
-                                                                                        "field": 19
-                                                                                    }
-                                                                                },
-                                                                                "rootReference": {}
-                                                                            }
+                                                            },
+                                                            {
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 9
                                                                         }
                                                                     },
-                                                                    {
-                                                                        "value": {
-                                                                            "selection": {
-                                                                                "directReference": {
-                                                                                    "structField": {
-                                                                                        "field": 46
-                                                                                    }
-                                                                                },
-                                                                                "rootReference": {}
-                                                                            }
+                                                                    "rootReference": {}
+                                                                }
+                                                            },
+                                                            {
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 1
                                                                         }
-                                                                    }
-                                                                ],
-                                                                "functionReference": 1,
-                                                                "outputType": {
-                                                                    "bool": {
-                                                                        "nullability": "NULLABILITY_NULLABLE"
-                                                                    }
+                                                                    },
+                                                                    "rootReference": {}
+                                                                }
+                                                            },
+                                                            {
+                                                                "selection": {
+                                                                    "directReference": {
+                                                                        "structField": {
+                                                                            "field": 33
+                                                                        }
+                                                                    },
+                                                                    "rootReference": {}
                                                                 }
                                                             }
-                                                        },
-                                                        "left": {
+                                                        ],
+                                                        "input": {
                                                             "join": {
                                                                 "expression": {
                                                                     "scalarFunction": {
                                                                         "arguments": [
                                                                             {
                                                                                 "value": {
                                                                                     "selection": {
                                                                                         "directReference": {
                                                                                             "structField": {
-                                                                                                "field": 37
+                                                                                                "field": 3
                                                                                             }
                                                                                         },
                                                                                         "rootReference": {}
                                                                                     }
                                                                                 }
                                                                             },
                                                                             {
                                                                                 "value": {
                                                                                     "selection": {
                                                                                         "directReference": {
-                                                                                            "structField": {}
+                                                                                            "structField": {
+                                                                                                "field": 32
+                                                                                            }
                                                                                         },
                                                                                         "rootReference": {}
                                                                                     }
                                                                                 }
                                                                             }
                                                                         ],
                                                                         "functionReference": 1,
@@ -418,27 +884,27 @@
                                                                             "scalarFunction": {
                                                                                 "arguments": [
                                                                                     {
                                                                                         "value": {
                                                                                             "selection": {
                                                                                                 "directReference": {
                                                                                                     "structField": {
-                                                                                                        "field": 28
+                                                                                                        "field": 23
                                                                                                     }
                                                                                                 },
                                                                                                 "rootReference": {}
                                                                                             }
                                                                                         }
                                                                                     },
                                                                                     {
                                                                                         "value": {
                                                                                             "selection": {
                                                                                                 "directReference": {
                                                                                                     "structField": {
-                                                                                                        "field": 1
+                                                                                                        "field": 7
                                                                                                     }
                                                                                                 },
                                                                                                 "rootReference": {}
                                                                                             }
                                                                                         }
                                                                                     }
                                                                                 ],
@@ -453,441 +919,293 @@
                                                                         "left": {
                                                                             "join": {
                                                                                 "expression": {
                                                                                     "scalarFunction": {
                                                                                         "arguments": [
                                                                                             {
                                                                                                 "value": {
-                                                                                                    "scalarFunction": {
-                                                                                                        "arguments": [
-                                                                                                            {
-                                                                                                                "value": {
-                                                                                                                    "selection": {
-                                                                                                                        "directReference": {
-                                                                                                                            "structField": {
-                                                                                                                                "field": 24
-                                                                                                                            }
-                                                                                                                        },
-                                                                                                                        "rootReference": {}
-                                                                                                                    }
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "value": {
-                                                                                                                    "selection": {
-                                                                                                                        "directReference": {
-                                                                                                                            "structField": {
-                                                                                                                                "field": 2
-                                                                                                                            }
-                                                                                                                        },
-                                                                                                                        "rootReference": {}
-                                                                                                                    }
-                                                                                                                }
-                                                                                                            }
-                                                                                                        ],
-                                                                                                        "functionReference": 1,
-                                                                                                        "outputType": {
-                                                                                                            "bool": {
-                                                                                                                "nullability": "NULLABILITY_NULLABLE"
-                                                                                                            }
-                                                                                                        }
+                                                                                                    "selection": {
+                                                                                                        "directReference": {
+                                                                                                            "structField": {}
+                                                                                                        },
+                                                                                                        "rootReference": {}
                                                                                                     }
                                                                                                 }
                                                                                             },
                                                                                             {
                                                                                                 "value": {
-                                                                                                    "scalarFunction": {
-                                                                                                        "arguments": [
-                                                                                                            {
-                                                                                                                "value": {
-                                                                                                                    "selection": {
-                                                                                                                        "directReference": {
-                                                                                                                            "structField": {
-                                                                                                                                "field": 23
-                                                                                                                            }
-                                                                                                                        },
-                                                                                                                        "rootReference": {}
-                                                                                                                    }
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "value": {
-                                                                                                                    "selection": {
-                                                                                                                        "directReference": {
-                                                                                                                            "structField": {
-                                                                                                                                "field": 1
-                                                                                                                            }
-                                                                                                                        },
-                                                                                                                        "rootReference": {}
-                                                                                                                    }
-                                                                                                                }
+                                                                                                    "selection": {
+                                                                                                        "directReference": {
+                                                                                                            "structField": {
+                                                                                                                "field": 9
                                                                                                             }
-                                                                                                        ],
-                                                                                                        "functionReference": 1,
-                                                                                                        "outputType": {
-                                                                                                            "bool": {
-                                                                                                                "nullability": "NULLABILITY_NULLABLE"
-                                                                                                            }
-                                                                                                        }
+                                                                                                        },
+                                                                                                        "rootReference": {}
                                                                                                     }
                                                                                                 }
                                                                                             }
                                                                                         ],
-                                                                                        "functionReference": 2,
+                                                                                        "functionReference": 1,
                                                                                         "outputType": {
                                                                                             "bool": {
                                                                                                 "nullability": "NULLABILITY_NULLABLE"
                                                                                             }
                                                                                         }
                                                                                     }
                                                                                 },
                                                                                 "left": {
-                                                                                    "join": {
-                                                                                        "expression": {
-                                                                                            "scalarFunction": {
-                                                                                                "arguments": [
-                                                                                                    {
-                                                                                                        "value": {
-                                                                                                            "selection": {
-                                                                                                                "directReference": {
-                                                                                                                    "structField": {
-                                                                                                                        "field": 16
-                                                                                                                    }
-                                                                                                                },
-                                                                                                                "rootReference": {}
-                                                                                                            }
+                                                                                    "read": {
+                                                                                        "baseSchema": {
+                                                                                            "names": [
+                                                                                                "s_suppkey",
+                                                                                                "s_name",
+                                                                                                "s_address",
+                                                                                                "s_nationkey",
+                                                                                                "s_phone",
+                                                                                                "s_acctbal",
+                                                                                                "s_comment"
+                                                                                            ],
+                                                                                            "struct": {
+                                                                                                "nullability": "NULLABILITY_REQUIRED",
+                                                                                                "types": [
+                                                                                                    {
+                                                                                                        "i32": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED"
                                                                                                         }
                                                                                                     },
                                                                                                     {
-                                                                                                        "value": {
-                                                                                                            "selection": {
-                                                                                                                "directReference": {
-                                                                                                                    "structField": {
-                                                                                                                        "field": 2
-                                                                                                                    }
-                                                                                                                },
-                                                                                                                "rootReference": {}
-                                                                                                            }
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "i32": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "decimal": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED",
+                                                                                                            "precision": 15,
+                                                                                                            "scale": 2
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_REQUIRED"
                                                                                                         }
                                                                                                     }
-                                                                                                ],
-                                                                                                "functionReference": 1,
-                                                                                                "outputType": {
-                                                                                                    "bool": {
-                                                                                                        "nullability": "NULLABILITY_NULLABLE"
-                                                                                                    }
-                                                                                                }
-                                                                                            }
-                                                                                        },
-                                                                                        "left": {
-                                                                                            "read": {
-                                                                                                "baseSchema": {
-                                                                                                    "names": [
-                                                                                                        "l_orderkey",
-                                                                                                        "l_partkey",
-                                                                                                        "l_suppkey",
-                                                                                                        "l_linenumber",
-                                                                                                        "l_quantity",
-                                                                                                        "l_extendedprice",
-                                                                                                        "l_discount",
-                                                                                                        "l_tax",
-                                                                                                        "l_returnflag",
-                                                                                                        "l_linestatus",
-                                                                                                        "l_shipdate",
-                                                                                                        "l_commitdate",
-                                                                                                        "l_receiptdate",
-                                                                                                        "l_shipinstruct",
-                                                                                                        "l_shipmode",
-                                                                                                        "l_comment"
-                                                                                                    ],
-                                                                                                    "struct": {
-                                                                                                        "nullability": "NULLABILITY_REQUIRED",
-                                                                                                        "types": [
-                                                                                                            {
-                                                                                                                "i64": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "i64": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "i64": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "i64": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "decimal": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                                    "precision": 15,
-                                                                                                                    "scale": 2
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "decimal": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                                    "precision": 15,
-                                                                                                                    "scale": 2
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "decimal": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                                    "precision": 15,
-                                                                                                                    "scale": 2
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "decimal": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                                                                                    "precision": 15,
-                                                                                                                    "scale": 2
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "date": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "date": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "date": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_NULLABLE"
-                                                                                                                }
-                                                                                                            }
-                                                                                                        ]
-                                                                                                    }
-                                                                                                },
-                                                                                                "common": {
-                                                                                                    "direct": {}
-                                                                                                },
-                                                                                                "namedTable": {
-                                                                                                    "names": [
-                                                                                                        "lineitem"
-                                                                                                    ]
-                                                                                                }
+                                                                                                ]
                                                                                             }
                                                                                         },
-                                                                                        "right": {
-                                                                                            "read": {
-                                                                                                "baseSchema": {
-                                                                                                    "names": [
-                                                                                                        "s_suppkey",
-                                                                                                        "s_name",
-                                                                                                        "s_address",
-                                                                                                        "s_nationkey",
-                                                                                                        "s_phone",
-                                                                                                        "s_acctbal",
-                                                                                                        "s_comment"
-                                                                                                    ],
-                                                                                                    "struct": {
-                                                                                                        "nullability": "NULLABILITY_REQUIRED",
-                                                                                                        "types": [
-                                                                                                            {
-                                                                                                                "i32": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "i32": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "decimal": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED",
-                                                                                                                    "precision": 15,
-                                                                                                                    "scale": 2
-                                                                                                                }
-                                                                                                            },
-                                                                                                            {
-                                                                                                                "string": {
-                                                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                                                }
-                                                                                                            }
-                                                                                                        ]
-                                                                                                    }
-                                                                                                },
-                                                                                                "common": {
-                                                                                                    "direct": {}
-                                                                                                },
-                                                                                                "namedTable": {
-                                                                                                    "names": [
-                                                                                                        "supplier"
-                                                                                                    ]
-                                                                                                }
-                                                                                            }
+                                                                                        "common": {
+                                                                                            "direct": {}
                                                                                         },
-                                                                                        "type": "JOIN_TYPE_INNER"
+                                                                                        "namedTable": {
+                                                                                            "names": [
+                                                                                                "supplier"
+                                                                                            ]
+                                                                                        }
                                                                                     }
                                                                                 },
                                                                                 "right": {
                                                                                     "read": {
                                                                                         "baseSchema": {
                                                                                             "names": [
-                                                                                                "ps_partkey",
-                                                                                                "ps_suppkey",
-                                                                                                "ps_availqty",
-                                                                                                "ps_supplycost",
-                                                                                                "ps_comment"
+                                                                                                "l_orderkey",
+                                                                                                "l_partkey",
+                                                                                                "l_suppkey",
+                                                                                                "l_linenumber",
+                                                                                                "l_quantity",
+                                                                                                "l_extendedprice",
+                                                                                                "l_discount",
+                                                                                                "l_tax",
+                                                                                                "l_returnflag",
+                                                                                                "l_linestatus",
+                                                                                                "l_shipdate",
+                                                                                                "l_commitdate",
+                                                                                                "l_receiptdate",
+                                                                                                "l_shipinstruct",
+                                                                                                "l_shipmode",
+                                                                                                "l_comment"
                                                                                             ],
                                                                                             "struct": {
                                                                                                 "nullability": "NULLABILITY_REQUIRED",
                                                                                                 "types": [
                                                                                                     {
-                                                                                                        "i32": {
-                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        "i64": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
                                                                                                         }
                                                                                                     },
                                                                                                     {
-                                                                                                        "i32": {
-                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        "i64": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
                                                                                                         }
                                                                                                     },
                                                                                                     {
-                                                                                                        "i32": {
-                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                        "i64": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "i64": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
                                                                                                         }
                                                                                                     },
                                                                                                     {
                                                                                                         "decimal": {
-                                                                                                            "nullability": "NULLABILITY_REQUIRED",
+                                                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                                                            "precision": 15,
+                                                                                                            "scale": 2
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "decimal": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                                                            "precision": 15,
+                                                                                                            "scale": 2
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "decimal": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                                                            "precision": 15,
+                                                                                                            "scale": 2
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "decimal": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE",
                                                                                                             "precision": 15,
                                                                                                             "scale": 2
                                                                                                         }
                                                                                                     },
                                                                                                     {
                                                                                                         "string": {
-                                                                                                            "nullability": "NULLABILITY_REQUIRED"
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "date": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "date": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "date": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                                                                        }
+                                                                                                    },
+                                                                                                    {
+                                                                                                        "string": {
+                                                                                                            "nullability": "NULLABILITY_NULLABLE"
                                                                                                         }
                                                                                                     }
                                                                                                 ]
                                                                                             }
                                                                                         },
                                                                                         "common": {
                                                                                             "direct": {}
                                                                                         },
                                                                                         "namedTable": {
                                                                                             "names": [
-                                                                                                "partsupp"
+                                                                                                "lineitem"
                                                                                             ]
                                                                                         }
                                                                                     }
                                                                                 },
                                                                                 "type": "JOIN_TYPE_INNER"
                                                                             }
                                                                         },
                                                                         "right": {
                                                                             "read": {
                                                                                 "baseSchema": {
                                                                                     "names": [
-                                                                                        "p_partkey",
-                                                                                        "p_name",
-                                                                                        "p_mfgr",
-                                                                                        "p_brand",
-                                                                                        "p_type",
-                                                                                        "p_size",
-                                                                                        "p_container",
-                                                                                        "p_retailprice",
-                                                                                        "p_comment"
+                                                                                        "o_orderkey",
+                                                                                        "o_custkey",
+                                                                                        "o_orderstatus",
+                                                                                        "o_totalprice",
+                                                                                        "o_orderdate",
+                                                                                        "o_orderpriority",
+                                                                                        "o_clerk",
+                                                                                        "o_shippriority",
+                                                                                        "o_comment"
                                                                                     ],
                                                                                     "struct": {
                                                                                         "nullability": "NULLABILITY_REQUIRED",
                                                                                         "types": [
                                                                                             {
                                                                                                 "i32": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
-                                                                                                "string": {
+                                                                                                "i32": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
                                                                                                 "string": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
-                                                                                                "string": {
-                                                                                                    "nullability": "NULLABILITY_REQUIRED"
+                                                                                                "decimal": {
+                                                                                                    "nullability": "NULLABILITY_REQUIRED",
+                                                                                                    "precision": 15,
+                                                                                                    "scale": 2
                                                                                                 }
                                                                                             },
                                                                                             {
-                                                                                                "string": {
+                                                                                                "date": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
-                                                                                                "i32": {
+                                                                                                "string": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
                                                                                                 "string": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
-                                                                                                "decimal": {
-                                                                                                    "nullability": "NULLABILITY_REQUIRED",
-                                                                                                    "precision": 15,
-                                                                                                    "scale": 2
+                                                                                                "i32": {
+                                                                                                    "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             },
                                                                                             {
                                                                                                 "string": {
                                                                                                     "nullability": "NULLABILITY_REQUIRED"
                                                                                                 }
                                                                                             }
@@ -895,72 +1213,40 @@
                                                                                     }
                                                                                 },
                                                                                 "common": {
                                                                                     "direct": {}
                                                                                 },
                                                                                 "namedTable": {
                                                                                     "names": [
-                                                                                        "part"
+                                                                                        "orders"
                                                                                     ]
                                                                                 }
                                                                             }
                                                                         },
                                                                         "type": "JOIN_TYPE_INNER"
                                                                     }
                                                                 },
                                                                 "right": {
                                                                     "read": {
                                                                         "baseSchema": {
                                                                             "names": [
-                                                                                "o_orderkey",
-                                                                                "o_custkey",
-                                                                                "o_orderstatus",
-                                                                                "o_totalprice",
-                                                                                "o_orderdate",
-                                                                                "o_orderpriority",
-                                                                                "o_clerk",
-                                                                                "o_shippriority",
-                                                                                "o_comment"
+                                                                                "n_nationkey",
+                                                                                "n_name",
+                                                                                "n_regionkey",
+                                                                                "n_comment"
                                                                             ],
                                                                             "struct": {
                                                                                 "nullability": "NULLABILITY_REQUIRED",
                                                                                 "types": [
                                                                                     {
                                                                                         "i32": {
                                                                                             "nullability": "NULLABILITY_REQUIRED"
                                                                                         }
                                                                                     },
                                                                                     {
-                                                                                        "i32": {
-                                                                                            "nullability": "NULLABILITY_REQUIRED"
-                                                                                        }
-                                                                                    },
-                                                                                    {
-                                                                                        "string": {
-                                                                                            "nullability": "NULLABILITY_REQUIRED"
-                                                                                        }
-                                                                                    },
-                                                                                    {
-                                                                                        "decimal": {
-                                                                                            "nullability": "NULLABILITY_REQUIRED",
-                                                                                            "precision": 15,
-                                                                                            "scale": 2
-                                                                                        }
-                                                                                    },
-                                                                                    {
-                                                                                        "date": {
-                                                                                            "nullability": "NULLABILITY_REQUIRED"
-                                                                                        }
-                                                                                    },
-                                                                                    {
-                                                                                        "string": {
-                                                                                            "nullability": "NULLABILITY_REQUIRED"
-                                                                                        }
-                                                                                    },
-                                                                                    {
                                                                                         "string": {
                                                                                             "nullability": "NULLABILITY_REQUIRED"
                                                                                         }
                                                                                     },
                                                                                     {
                                                                                         "i32": {
                                                                                             "nullability": "NULLABILITY_REQUIRED"
@@ -975,137 +1261,76 @@
                                                                             }
                                                                         },
                                                                         "common": {
                                                                             "direct": {}
                                                                         },
                                                                         "namedTable": {
                                                                             "names": [
-                                                                                "orders"
+                                                                                "nation"
                                                                             ]
                                                                         }
                                                                     }
                                                                 },
                                                                 "type": "JOIN_TYPE_INNER"
                                                             }
-                                                        },
-                                                        "right": {
-                                                            "read": {
-                                                                "baseSchema": {
-                                                                    "names": [
-                                                                        "n_nationkey",
-                                                                        "n_name",
-                                                                        "n_regionkey",
-                                                                        "n_comment"
-                                                                    ],
-                                                                    "struct": {
-                                                                        "nullability": "NULLABILITY_REQUIRED",
-                                                                        "types": [
-                                                                            {
-                                                                                "i32": {
-                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                }
-                                                                            },
-                                                                            {
-                                                                                "string": {
-                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                }
-                                                                            },
-                                                                            {
-                                                                                "i32": {
-                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                }
-                                                                            },
-                                                                            {
-                                                                                "string": {
-                                                                                    "nullability": "NULLABILITY_REQUIRED"
-                                                                                }
-                                                                            }
-                                                                        ]
-                                                                    }
-                                                                },
-                                                                "common": {
-                                                                    "direct": {}
-                                                                },
-                                                                "namedTable": {
-                                                                    "names": [
-                                                                        "nation"
-                                                                    ]
-                                                                }
-                                                            }
-                                                        },
-                                                        "type": "JOIN_TYPE_INNER"
+                                                        }
                                                     }
                                                 }
                                             }
-                                        }
+                                        },
+                                        "measures": [
+                                            {
+                                                "measure": {
+                                                    "functionReference": 6,
+                                                    "outputType": {
+                                                        "i64": {
+                                                            "nullability": "NULLABILITY_NULLABLE"
+                                                        }
+                                                    },
+                                                    "phase": "AGGREGATION_PHASE_INITIAL_TO_RESULT"
+                                                }
+                                            }
+                                        ]
                                     }
                                 },
-                                "measures": [
+                                "sorts": [
                                     {
-                                        "measure": {
-                                            "arguments": [
-                                                {
-                                                    "value": {
-                                                        "selection": {
-                                                            "directReference": {
-                                                                "structField": {}
-                                                            },
-                                                            "rootReference": {}
-                                                        }
+                                        "direction": "SORT_DIRECTION_DESC_NULLS_FIRST",
+                                        "expr": {
+                                            "selection": {
+                                                "directReference": {
+                                                    "structField": {
+                                                        "field": 1
                                                     }
-                                                }
-                                            ],
-                                            "functionReference": 7,
-                                            "outputType": {
-                                                "decimal": {
-                                                    "nullability": "NULLABILITY_NULLABLE",
-                                                    "precision": 38,
-                                                    "scale": 4
-                                                }
-                                            },
-                                            "phase": "AGGREGATION_PHASE_INITIAL_TO_RESULT"
+                                                },
+                                                "rootReference": {}
+                                            }
                                         }
-                                    }
-                                ]
-                            }
-                        },
-                        "sorts": [
-                            {
-                                "direction": "SORT_DIRECTION_ASC_NULLS_FIRST",
-                                "expr": {
-                                    "selection": {
-                                        "directReference": {
-                                            "structField": {}
-                                        },
-                                        "rootReference": {}
-                                    }
-                                }
-                            },
-                            {
-                                "direction": "SORT_DIRECTION_DESC_NULLS_FIRST",
-                                "expr": {
-                                    "selection": {
-                                        "directReference": {
-                                            "structField": {
-                                                "field": 1
+                                    },
+                                    {
+                                        "direction": "SORT_DIRECTION_ASC_NULLS_FIRST",
+                                        "expr": {
+                                            "selection": {
+                                                "directReference": {
+                                                    "structField": {}
+                                                },
+                                                "rootReference": {}
                                             }
-                                        },
-                                        "rootReference": {}
+                                        }
                                     }
-                                }
+                                ]
                             }
-                        ]
+                        }
                     }
                 },
                 "names": [
-                    "nation",
-                    "o_year",
-                    "sum_profit"
+                    "s_name",
+                    "numwait"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h10/tpc_h10.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h10/tpc_h10.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -839,11 +839,11 @@
                     "c_comment",
                     "revenue"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h110/tpc_h110.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h11_1/tpc_h11_1.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9687499999080176%*

 * *Differences: {"'relations'": "{0: {'root': {'input': {'sort': {'input': {'filter': {'input': {'aggregate': "*

 * *                "{'measures': {0: {'measure': {'arguments': {0: {'value': {'scalarFunction': "*

 * *                "{'arguments': {1: {'value': {'cast': {'type': {'decimal': {'nullability': "*

 * *                "'NULLABILITY_NULLABLE'}}}}}}}}}}}}}}}}}}}}}}",*

 * * "'version'": "{'minorNumber': 44}"}*

```diff
@@ -443,15 +443,15 @@
                                                                                                 }
                                                                                             },
                                                                                             "rootReference": {}
                                                                                         }
                                                                                     },
                                                                                     "type": {
                                                                                         "decimal": {
-                                                                                            "nullability": "NULLABILITY_REQUIRED",
+                                                                                            "nullability": "NULLABILITY_NULLABLE",
                                                                                             "precision": 15,
                                                                                             "scale": 2
                                                                                         }
                                                                                     }
                                                                                 }
                                                                             }
                                                                         }
@@ -505,11 +505,11 @@
                     "ps_partkey",
                     "value"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h111/tpc_h111.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h11_0/tpc_h11_0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9687499999080176%*

 * *Differences: {"'relations'": "{0: {'root': {'input': {'sort': {'input': {'filter': {'input': {'aggregate': "*

 * *                "{'measures': {0: {'measure': {'arguments': {0: {'value': {'scalarFunction': "*

 * *                "{'arguments': {1: {'value': {'cast': {'type': {'decimal': {'nullability': "*

 * *                "'NULLABILITY_REQUIRED'}}}}}}}}}}}}}}}}}}}}}}",*

 * * "'version'": "{'minorNumber': 44}"}*

```diff
@@ -443,15 +443,15 @@
                                                                                                 }
                                                                                             },
                                                                                             "rootReference": {}
                                                                                         }
                                                                                     },
                                                                                     "type": {
                                                                                         "decimal": {
-                                                                                            "nullability": "NULLABILITY_NULLABLE",
+                                                                                            "nullability": "NULLABILITY_REQUIRED",
                                                                                             "precision": 15,
                                                                                             "scale": 2
                                                                                         }
                                                                                     }
                                                                                 }
                                                                             }
                                                                         }
@@ -505,11 +505,11 @@
                     "ps_partkey",
                     "value"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h12/tpc_h12.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h12/tpc_h12.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -770,11 +770,11 @@
                     "high_line_count",
                     "low_line_count"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h13/tpc_h13.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h13/tpc_h13.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -417,11 +417,11 @@
                     "c_count",
                     "custdist"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h18/tpc_h18.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h18/tpc_h18.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -541,11 +541,11 @@
                     "o_totalprice",
                     "sum_qty"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h19/tpc_h19.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h19/tpc_h19.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -1422,11 +1422,11 @@
                 "names": [
                     "revenue"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h20/tpc_h20.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h20/tpc_h20.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -309,11 +309,11 @@
                     "s_name",
                     "s_address"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h220/tpc_h220.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h22_0/tpc_h22_0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -613,11 +613,11 @@
                     "numcust",
                     "totacctbal"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h221/tpc_h221.json` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h22_1/tpc_h22_1.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "{'minorNumber': 44}"}*

```diff
@@ -613,11 +613,11 @@
                     "numcust",
                     "totacctbal"
                 ]
             }
         }
     ],
     "version": {
-        "minorNumber": 35,
+        "minorNumber": 44,
         "producer": "ibis-substrait"
     }
 }
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_compiler.py` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_compiler.py`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_extensions.py` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_extensions.py`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_literal.py` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_literal.py`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/compiler/test_tpch.py` & `ibis_substrait-3.2.1/ibis_substrait/tests/compiler/test_tpch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import date
 
 import ibis
 import pytest
 from google.protobuf import json_format
 from packaging import version
 from packaging.specifiers import SpecifierSet
-from pytest_lazyfixture import lazy_fixture
 
 
 def ibis_version(constraint: str, reason: str):
     """Run the test iff the Ibis version matches the constraint."""
     return pytest.mark.skipif(
         version.parse(ibis.__version__) not in SpecifierSet(constraint),
         reason=f"{reason} - ibis version: {ibis.__version__}, test versions: {constraint}",
@@ -621,113 +620,114 @@
     gq = custsale.group_by(custsale.cntrycode)
     outerq = gq.aggregate(numcust=custsale.count(), totacctbal=custsale.c_acctbal.sum())
 
     return outerq.order_by(outerq.cntrycode)
 
 
 TPC_H = [
-    lazy_fixture("tpc_h01"),
+    "tpc_h01",
     pytest.param(
-        lazy_fixture("tpc_h02"),
+        "tpc_h02",
         marks=pytest.mark.xfail(
             raises=NotImplementedError, reason="Correlated Subquery issues"
         ),
     ),
-    lazy_fixture("tpc_h03"),
-    lazy_fixture("tpc_h04"),
-    lazy_fixture("tpc_h05"),
-    lazy_fixture("tpc_h06"),
-    lazy_fixture("tpc_h07"),
+    "tpc_h03",
+    "tpc_h04",
+    "tpc_h05",
+    "tpc_h06",
+    "tpc_h07",
     pytest.param(
-        lazy_fixture("tpc_h08"),
+        "tpc_h08",
         marks=pytest.mark.xfail(
             raises=TypeError,
             reason="Aggregates need to be handled differently than they are",
         ),
     ),
     pytest.param(
-        lazy_fixture("tpc_h09"),
+        "tpc_h09",
         marks=ibis_version("<7.0,~=7.1.0", "Field ordering difference"),
     ),
     pytest.param(
-        lazy_fixture("tpc_h09"),
+        "tpc_h09",
         marks=ibis_version("~=7.0.0", "Field ordering difference"),
     ),
     pytest.param(
-        lazy_fixture("tpc_h09"),
+        "tpc_h09",
         marks=ibis_version(">=7.2", "7.2 adds a cast to int and dec multiplication"),
     ),
-    lazy_fixture("tpc_h10"),
+    "tpc_h10",
     pytest.param(
-        lazy_fixture("tpc_h11"),
+        "tpc_h11",
         marks=ibis_version("<7.2", "7.2 makes join output columns nullable"),
     ),
     pytest.param(
-        lazy_fixture("tpc_h11"),
+        "tpc_h11",
         marks=ibis_version(">=7.2", "7.2 makes join output columns nullable"),
     ),
-    lazy_fixture("tpc_h12"),
-    lazy_fixture("tpc_h13"),
+    "tpc_h12",
+    "tpc_h13",
     pytest.param(
-        lazy_fixture("tpc_h14"),
+        "tpc_h14",
         marks=pytest.mark.xfail(
             raises=TypeError,
             reason="protobuf error resulting subquery (cannot merge Expression and AggregateFunction)",
         ),
     ),
     pytest.param(
-        lazy_fixture("tpc_h15"),
+        "tpc_h15",
         marks=pytest.mark.xfail(
             raises=NotImplementedError, reason="Correlated Subquery issues"
         ),
     ),
     pytest.param(
-        lazy_fixture("tpc_h16"),
+        "tpc_h16",
         marks=pytest.mark.xfail(
             raises=ValueError, reason="countdistinct not handled correctly"
         ),
     ),
     pytest.param(
-        lazy_fixture("tpc_h17"),
+        "tpc_h17",
         marks=(
             pytest.mark.xfail(
                 raises=NotImplementedError,
                 reason="ibis.expr.operations.relations.Aggregation",
             ),
             ibis_version("<7.1", "Aggregation not implemented before 7.1"),
         ),
     ),
     pytest.param(
-        lazy_fixture("tpc_h17"),
+        "tpc_h17",
         marks=(
             pytest.mark.xfail(
                 raises=NotImplementedError,
                 reason="Filters on subqueries are unsupported",
             ),
             ibis_version(">=7.1", "Aggregation not implemented before 7.1"),
         ),
     ),
-    lazy_fixture("tpc_h18"),
-    lazy_fixture("tpc_h19"),
-    lazy_fixture("tpc_h20"),
-    lazy_fixture("tpc_h21"),
+    "tpc_h18",
+    "tpc_h19",
+    "tpc_h20",
+    "tpc_h21",
     pytest.param(
-        lazy_fixture("tpc_h22"),
+        "tpc_h22",
         marks=ibis_version("<7.1", "7.1 changes function order"),
     ),
     pytest.param(
-        lazy_fixture("tpc_h22"),
+        "tpc_h22",
         marks=ibis_version(">=7.1", "7.1 changes function order"),
     ),
 ]
 
 
 @pytest.mark.parametrize(
-    "query",
+    "fixture_name",
     TPC_H,
 )
-def test_compile(query, compiler, snapshot, request):
+def test_compile(fixture_name, compiler, snapshot, request):
+    query = request.getfixturevalue(fixture_name)
     plan = compiler.compile(query)
 
     snapshot.assert_match(
         json_format.MessageToJson(plan), f"{request.node.callspec.id}.json"
     )
```

### Comparing `ibis_substrait-3.2.0/ibis_substrait/tests/integration/test_pyarrow.py` & `ibis_substrait-3.2.1/ibis_substrait/tests/integration/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `ibis_substrait-3.2.0/pyproject.toml` & `ibis_substrait-3.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ibis-substrait"
-version = "3.2.0"
+version = "3.2.1"
 packages = [{ include = "ibis_substrait" }]
 homepage = "https://github.com/ibis-project/ibis-substrait"
 repository = "https://github.com/ibis-project/ibis-substrait"
 description = "Subtrait compiler for ibis"
 authors = ["Ibis Contributors"]
 maintainers = ["Ibis Contributors"]
 license = "Apache-2.0"
@@ -16,15 +16,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
-ibis-framework = ">=4"
+ibis-framework = ">=4,<9"
 packaging = ">=21.3"
 pyyaml = ">=5"
 substrait = ">=0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.0.0"
 duckdb = ">=0.8.1"
@@ -38,28 +38,31 @@
 mypy-protobuf = "^3.3.0"
 types-protobuf = "^3.20.1"
 types-pytz = ">=2022.0.0"
 types-pyyaml = ">=6.0.12.8"
 typing-extensions = ">=4"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.0.0"
+pytest = "^8.0.0"
 pytest-clarity = "^1.0.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-mock = "^3.6.1"
 pytest-randomly = "^3.10.1"
-pytest-lazy-fixture = "^0.6.3"
 pytz = "^2022.1"
 sqlalchemy = ">=1.4.48"
 pathspec = "0.12.1"
 pyarrow = ">=11.0.0"
 pytest-snapshot = "^0.9.0"
 
 [tool.ruff]
 line-length = 88
+respect-gitignore = true
+target-version = "py39"
+
+[tool.ruff.lint]
 select = [
   "B", # flake8-bugbear
   "BLE", # flake8-blind-except
   "C4", # comprehensions
   "D", # pydocstyle
   "E", # pycodestyle
   "F", # pyflakes
@@ -75,17 +78,15 @@
   "SIM", # flake8-simplify
   "T10", # flake8-debugger
   "T20", # flake8-print
   "TID", # flake8-tidy-imports
   "UP", # pyupgrade
   "W", # pycodestyle
   "YTT", # flake8-2020
-
 ]
-respect-gitignore = true
 ignore = [
   "B904", # raise from e or raise from None in exception handlers
   "C408", # dict(...) as literal
   "D100", # public module
   "D101", # public class
   "D102", # public method
   "D103", # public function
@@ -95,30 +96,30 @@
   "D107", # init
   "D202", # blank lines after function docstring
   "D203", # blank line before class docstring
   "D213", # Multi-line docstring summary should start at the second line
   "D402", # First line should not be the function's signature
   "E501",
   "E731",
+  "ISC001",
   "PGH003",
   "RET504",
   "RET505",
   "RET506",
   "RET507",
   "RET508",
   "SIM102", # nested ifs
   "SIM108", # convert everything to ternary operator
   "SIM114", # combine `if` branches
   "SIM117", # nested withs
   "SIM118", # remove .keys() calls from dictionaries
   "UP006", # use collections.deque instead of Deque for type annotation
 ]
-target-version = "py39"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*test*.py" = ["D"] # ignore all docstring lints in tests
 
 [tool.pytest.ini_options]
 xfail_strict = true
 addopts = [
   "--ignore=site-packages",
   "--ignore=dist-packages",
```

### Comparing `ibis_substrait-3.2.0/PKG-INFO` & `ibis_substrait-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-substrait
-Version: 3.2.0
+Version: 3.2.1
 Summary: Subtrait compiler for ibis
 Home-page: https://github.com/ibis-project/ibis-substrait
 License: Apache-2.0
 Author: Ibis Contributors
 Maintainer: Ibis Contributors
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: ibis-framework (>=4)
+Requires-Dist: ibis-framework (>=4,<9)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pyyaml (>=5)
 Requires-Dist: substrait (>=0.2.1)
 Project-URL: Repository, https://github.com/ibis-project/ibis-substrait
 Description-Content-Type: text/markdown
 
 # [Ibis](https://ibis-project.org) + [Substrait](https://substrait.io)
```

