# Comparing `tmp/rormula-0.1.5.tar.gz` & `tmp/rormula-0.1.6.tar.gz`

## Comparing `rormula-0.1.5.tar` & `rormula-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0     1001      127      165 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/Cargo.toml
--rw-r--r--   0     1001      127        6 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/.gitignore
--rw-r--r--   0     1001      127     4474 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/array.rs
--rw-r--r--   0     1001      127    12246 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/expression/expr_arithmetic.rs
--rw-r--r--   0     1001      127    10877 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/expression/expr_wilkinson.rs
--rw-r--r--   0     1001      127      211 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/expression/mod.rs
--rw-r--r--   0     1001      127     3272 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/expression/ops_common.rs
--rw-r--r--   0     1001      127     1577 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/expression/value.rs
--rw-r--r--   0     1001      127       66 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/lib.rs
--rw-r--r--   0     1001      127     1232 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/src/result.rs
--rw-r--r--   0     1001      127     3434 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula-rs/tests/test_rormula.rs
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 rormula-0.1.5/rormula/Cargo.toml
--rw-r--r--   0     1001      127        6 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/.gitignore
--rw-r--r--   0     1001      127      548 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/README-pypi.md
--rw-r--r--   0     1001      127     2719 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/benches/benchmark.rs
--rw-r--r--   0     1001      127       50 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/requirements-dev.txt
--rw-r--r--   0     1001      127     2781 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/rormula/__init__.py
--rw-r--r--   0     1001      127      764 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/rormula/rormula.pyi
--rw-r--r--   0     1001      127     8227 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/test/__init__.py
--rw-r--r--   0     1001      127     2452 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/test/test_arithmetic.py
--rw-r--r--   0     1001      127     1178 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/test/test_meta.py
--rw-r--r--   0     1001      127     6060 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/test/test_wilkinson.py
--rw-r--r--   0     1001      127    28690 2024-02-15 10:44:22.000000 rormula-0.1.5/Cargo.lock
--rw-r--r--   0        0        0       64 1970-01-01 00:00:00.000000 rormula-0.1.5/Cargo.toml
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 rormula-0.1.5/pyproject.toml
--rw-r--r--   0     1001      127      764 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/rormula.pyi
--rw-r--r--   0     1001      127     2781 2024-02-15 10:44:22.000000 rormula-0.1.5/rormula/__init__.py
--rw-r--r--   0     1001      127      548 2024-02-15 10:44:22.000000 rormula-0.1.5/README-pypi.md
--rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 rormula-0.1.5/PKG-INFO
+-rw-r--r--   0     1001      127      165 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/Cargo.toml
+-rw-r--r--   0     1001      127        6 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/.gitignore
+-rw-r--r--   0     1001      127     4474 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/array.rs
+-rw-r--r--   0     1001      127    12246 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/expression/expr_arithmetic.rs
+-rw-r--r--   0     1001      127    10877 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/expression/expr_wilkinson.rs
+-rw-r--r--   0     1001      127      211 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      127     3272 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/expression/ops_common.rs
+-rw-r--r--   0     1001      127     1481 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/expression/value.rs
+-rw-r--r--   0     1001      127       66 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/lib.rs
+-rw-r--r--   0     1001      127     1232 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/src/result.rs
+-rw-r--r--   0     1001      127     3434 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula-rs/tests/test_rormula.rs
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 rormula-0.1.6/rormula/Cargo.toml
+-rw-r--r--   0     1001      127        6 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/.gitignore
+-rw-r--r--   0     1001      127      548 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/README-pypi.md
+-rw-r--r--   0     1001      127     2751 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/benches/benchmark.rs
+-rw-r--r--   0     1001      127       50 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/requirements-dev.txt
+-rw-r--r--   0     1001      127     2781 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/rormula/__init__.py
+-rw-r--r--   0     1001      127      764 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/rormula/rormula.pyi
+-rw-r--r--   0     1001      127     8749 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/test/__init__.py
+-rw-r--r--   0     1001      127     2471 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/test/test_arithmetic.py
+-rw-r--r--   0     1001      127     1178 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/test/test_meta.py
+-rw-r--r--   0     1001      127     6301 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/test/test_wilkinson.py
+-rw-r--r--   0     1001      127    31439 2024-05-21 20:30:00.000000 rormula-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0       64 1970-01-01 00:00:00.000000 rormula-0.1.6/Cargo.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 rormula-0.1.6/pyproject.toml
+-rw-r--r--   0     1001      127     2781 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/__init__.py
+-rw-r--r--   0     1001      127      764 2024-05-21 20:30:00.000000 rormula-0.1.6/rormula/rormula.pyi
+-rw-r--r--   0     1001      127      548 2024-05-21 20:30:00.000000 rormula-0.1.6/README-pypi.md
+-rw-r--r--   0        0        0     1135 1970-01-01 00:00:00.000000 rormula-0.1.6/PKG-INFO
```

### Comparing `rormula-0.1.5/rormula-rs/src/array.rs` & `rormula-0.1.6/rormula-rs/src/array.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula-rs/src/expression/expr_arithmetic.rs` & `rormula-0.1.6/rormula-rs/src/expression/expr_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula-rs/src/expression/expr_wilkinson.rs` & `rormula-0.1.6/rormula-rs/src/expression/expr_wilkinson.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula-rs/src/expression/ops_common.rs` & `rormula-0.1.6/rormula-rs/src/expression/ops_common.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula-rs/src/expression/value.rs` & `rormula-0.1.6/rormula-rs/src/expression/value.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 use std::str::FromStr;
 
 use crate::{array::Array2d, result::RoErr, roerr};
 
 #[derive(Clone, Debug, PartialEq)]
 pub enum Value {
-    /// Vec<String> are the names of the columns, i.e., the resulting names of the new features
     Array(Array2d),
     RowInds(Vec<usize>),
     /// String is the name of the categorical
     Cats(Vec<String>),
     Scalar(f64),
     /// String is the error message
     Error(String),
```

### Comparing `rormula-0.1.5/rormula-rs/src/result.rs` & `rormula-0.1.6/rormula-rs/src/result.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula-rs/tests/test_rormula.rs` & `rormula-0.1.6/rormula-rs/tests/test_rormula.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula/Cargo.toml` & `rormula-0.1.6/rormula/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [package]
 name = "rormula"
-version = "0.1.5"
+version = "0.1.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "rormula"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.20.2", features = ["generate-import-lib"] }
-numpy = "0.20.0"
+pyo3 = { version = "0.21.2", features = ["generate-import-lib"] }
+numpy = "0.21.0"
 rormula-rs = { path = "../rormula-rs" }
 
 # The extension module needs to be a feature due to
 # https://pyo3.rs/v0.20.0/faq.html#i-cant-run-cargo-test-or-i-cant-build-in-a-cargo-workspace-im-having-linker-issues-like-symbol-not-found-or-undefined-reference-to-_pyexc_systemerror
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
+print_timings = ["rormula-rs/print_timings"]
 
 [dev-dependencies]
 criterion = { version = "0.5.1", features = ["html_reports"] }
-which = "5.0.0"
+which = "6.0.1"
 
 [[bench]]
 name = "benchmark"
 harness = false
```

### Comparing `rormula-0.1.5/rormula/README-pypi.md` & `rormula-0.1.6/rormula/README-pypi.md`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula/benches/benchmark.rs` & `rormula-0.1.6/rormula/benches/benchmark.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 //! On Windows with Conda the Benchmarks might not work due to
 //! https://github.com/ContinuumIO/anaconda-issues/issues/11439,
 //! see https://github.com/PyO3/pyo3/issues/1554
 
 use criterion::{black_box, criterion_group, criterion_main, Criterion};
+use numpy::PyArrayMethods;
 use numpy::{
     ndarray::{concatenate, Array1, Array2, Axis},
     pyo3::Python,
     PyArray2, PyReadonlyArray2,
 };
 use pyo3::PyResult;
 use rormula_rs::array::Array2d;
 use std::mem;
-
 pub fn initialize_python() -> PyResult<()> {
     pyo3::prepare_freethreaded_python();
     Ok(())
 }
 
 fn from_pyarray_nd(pyarray: &PyReadonlyArray2<f64>) -> Array2<f64> {
     pyarray.to_owned_array()
@@ -45,15 +45,15 @@
 
     mem::take(arr1)
 }
 
 fn criterion_benchmark(c: &mut Criterion) {
     initialize_python().unwrap();
     Python::with_gil(|py| {
-        let pyarray = PyArray2::<f64>::zeros(py, (500000, 3), false);
+        let pyarray = PyArray2::<f64>::zeros_bound(py, (500000, 3), false);
         let readonly = pyarray.readonly();
         c.bench_function("create nd", |b| {
             b.iter(|| from_pyarray_nd(black_box(&readonly)))
         });
         c.bench_function("create array", |b| {
             b.iter(|| from_pyarray(black_box(&readonly)))
         });
```

### Comparing `rormula-0.1.5/rormula/rormula/__init__.py` & `rormula-0.1.6/rormula/rormula/__init__.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula/rormula/rormula.pyi` & `rormula-0.1.6/rormula/rormula/rormula.pyi`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula/src/lib.rs` & `rormula-0.1.6/rormula/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 use numpy::{
     ndarray::{s, Array2, ArrayView1},
     IntoPyArray, PyArray2, PyReadonlyArray2,
 };
 use pyo3::{
     exceptions::{PyTypeError, PyValueError},
     prelude::*,
+    types::PyList,
 };
 pub use rormula_rs::exmex::prelude::*;
 pub use rormula_rs::exmex::ExError;
 use rormula_rs::expression::{ExprColCount, ExprNames, ExprWilkinson, NameValue, Value};
 use rormula_rs::result::RoErr;
 use rormula_rs::{array::Array2d, expression::ExprArithmetic};
 
 fn ex_to_pyerr(e: ExError) -> PyErr {
     PyTypeError::new_err(e.msg().to_string())
 }
 fn ro_to_pyerr(e: RoErr) -> PyErr {
     PyValueError::new_err(e.msg().to_string())
 }
 
+fn find_col(cols: &Bound<'_, PyList>, needle: &str) -> Option<usize> {
+    cols.iter().position(|num_name| {
+        let num_name = num_name.extract::<&str>();
+        if let Ok(num_name) = num_name {
+            num_name == needle
+        } else {
+            false
+        }
+    })
+}
+
 #[pyfunction]
 fn eval_arithmetic<'py>(
     py: Python<'py>,
     ror: &Arithmetic,
     numerical_data: PyReadonlyArray2<f64>,
-    numerical_cols: Vec<&'py str>,
-) -> PyResult<&'py PyArray2<f64>> {
+    numerical_cols: &Bound<'py, PyList>,
+) -> PyResult<Bound<'py, PyArray2<f64>>> {
     let numerical_data = numerical_data.as_array();
     let vars = ror
         .expr
         .var_names()
         .iter()
-        .map(|vn| {
-            if let Some(num_idx) = numerical_cols.iter().position(|num_name| vn == num_name) {
+        .map(|vn: &String| {
+            if let Some(num_idx) = find_col(numerical_cols, vn) {
                 let s: ArrayView1<'_, f64> = numerical_data.slice(s![.., num_idx]);
                 let n_rows = s.dim();
                 Ok(Value::Array(
                     Array2d::from_iter(s.into_iter(), n_rows, 1).map_err(ro_to_pyerr)?,
                 ))
             } else {
                 Err(PyValueError::new_err(format!(
@@ -58,76 +70,84 @@
             Value::Array(a) => {
                 let mut pya = Array2::<f64>::ones([a.n_rows, a.n_cols]);
                 for col in 0..a.n_cols {
                     for row in 0..a.n_rows {
                         pya[(row, col)] = a.get(row, col);
                     }
                 }
-                let res = pya.into_pyarray(py);
+                let res = pya.into_pyarray_bound(py);
 
                 Ok(res)
             }
             Value::RowInds(row_inds) => {
                 let mut pya = Array2::<f64>::ones([row_inds.len(), 1]);
                 for row in 0..row_inds.len() {
                     pya[(row, 0)] = row_inds[row] as f64;
                 }
-                let res = pya.into_pyarray(py);
+                let res = pya.into_pyarray_bound(py);
                 Ok(res)
             }
-            Value::Scalar(s) => Ok(Array2::<f64>::from_elem((1, 1), s).into_pyarray(py)),
+            Value::Scalar(s) => Ok(Array2::<f64>::from_elem((1, 1), s).into_pyarray_bound(py)),
             Value::Cats(_) => Err(PyValueError::new_err("result cannot be cat".to_string())),
             Value::Error(e) => Err(PyValueError::new_err(format!("computation failed, {e:?}"))),
         }
     }
 }
+
+type WilkonsonReturnType<'py> = (Option<Vec<String>>, Bound<'py, PyArray2<f64>>);
+
 #[pyfunction]
 fn eval_wilkinson<'py>(
     py: Python<'py>,
     ror: &Wilkinson,
     numerical_data: PyReadonlyArray2<f64>,
-    numerical_cols: Vec<&'py str>,
+    numerical_cols: &Bound<'py, PyList>,
     cat_data: PyReadonlyArray2<PyObject>,
-    cat_cols: Vec<&'py str>,
+    cat_cols: &Bound<'py, PyList>,
     skip_names: bool,
-) -> PyResult<(Option<Vec<String>>, &'py PyArray2<f64>)> {
+) -> PyResult<WilkonsonReturnType<'py>> {
     let numerical_data = numerical_data.as_array();
     let cat_data = cat_data.as_array();
     let vars = ror
         .expr
         .var_names()
         .iter()
         .map(|vn| {
-            if let Some(num_idx) = numerical_cols.iter().position(|num_name| vn == num_name) {
+            if let Some(num_idx) = find_col(numerical_cols, vn) {
                 let s: ArrayView1<'_, f64> = numerical_data.slice(s![.., num_idx]);
                 let n_rows = s.dim();
                 let names = if skip_names {
                     None
                 } else {
-                    Some(NameValue::Array(vec![numerical_cols[num_idx].to_string()]))
+                    Some(NameValue::Array(vec![numerical_cols
+                        .get_item(num_idx)?
+                        .extract::<String>()?]))
                 };
                 Ok((
                     names,
                     Value::Array(
                         Array2d::from_iter(s.into_iter(), n_rows, 1).map_err(ro_to_pyerr)?,
                     ),
                 ))
-            } else if let Some(cat_idx) = cat_cols.iter().position(|cat_name| vn == cat_name) {
+            } else if let Some(cat_idx) = find_col(cat_cols, vn) {
                 let col: ArrayView1<'_, Py<PyAny>> = cat_data.slice(s![.., cat_idx]);
                 let col = col
                     .iter()
                     .map(|s: &pyo3::Py<pyo3::PyAny>| Ok(s.extract::<&str>(py)?.to_string()))
                     .collect::<PyResult<Vec<_>>>()?;
                 let x = Value::Cats(col);
                 let feature_name = if skip_names {
                     None
                 } else {
                     Some(
-                        NameValue::cats_from_value(cat_cols[cat_idx].to_string(), x.clone())
-                            .unwrap(),
+                        NameValue::cats_from_value(
+                            cat_cols.get_item(cat_idx)?.extract::<String>()?,
+                            x.clone(),
+                        )
+                        .unwrap(),
                     )
                 };
                 Ok((feature_name, x))
             } else {
                 Err(PyValueError::new_err(format!(
                     "did not find Variable {vn} in the data"
                 )))
@@ -169,15 +189,15 @@
                 };
                 let mut pya = Array2::<f64>::ones([a.n_rows, a.n_cols + 1]);
                 for col in 0..a.n_cols {
                     for row in 0..a.n_rows {
                         pya[(row, col + 1)] = a.get(row, col);
                     }
                 }
-                let res = pya.into_pyarray(py);
+                let res = pya.into_pyarray_bound(py);
 
                 Ok((names, res))
             }
             Value::Cats(_) => Err(PyValueError::new_err("result cannot be cat".to_string())),
             Value::RowInds(_) => Err(PyValueError::new_err(
                 "result cannot be row indices".to_string(),
             )),
@@ -214,15 +234,15 @@
         expr: ExprWilkinson::parse(s).map_err(ex_to_pyerr)?,
         expr_names: ExprNames::parse(s).map_err(ex_to_pyerr)?,
         expr_count: ExprColCount::parse(s).map_err(ex_to_pyerr)?,
     })
 }
 
 #[pymodule]
-fn rormula(_py: Python, m: &PyModule) -> PyResult<()> {
+fn rormula(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(parse_wilkinson, m)?)?;
     m.add_function(wrap_pyfunction!(eval_wilkinson, m)?)?;
     m.add_function(wrap_pyfunction!(parse_arithmetic, m)?)?;
     m.add_function(wrap_pyfunction!(eval_arithmetic, m)?)?;
     m.add_class::<Wilkinson>()?;
     m.add_class::<Arithmetic>()?;
     Ok(())
```

### Comparing `rormula-0.1.5/rormula/test/test_arithmetic.py` & `rormula-0.1.6/rormula/test/test_arithmetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,29 @@
     s = "((first_var|{second.var}==5.0) - (first_var|{second.var}==2.5)) / 4.0"
     data[7, :] = 5.0
     df = pd.DataFrame(data=data[:10, :2], columns=["first_var", "second.var"])
     rormula = Arithmetic(s, "reduced")
     res = rormula.eval_asdf(df)
     assert np.allclose(res.to_numpy().item(), (5.0 - 2.5) / 4.0)
 
+
 def test_scalar_scalar():
     name = "test_scalar"
     data = np.random.random((100, 6)) * 1000
     df = pd.DataFrame(
         data=data, columns=["alpha", "beta", "gamma", "delta", "epsilon", "phi"]
     )
     s = "5/3 * alpha / beta * (0.2 / 200.0 / (29.22+gamma+epsilon+phi) / 1000)"
     rormula = Arithmetic(s, name)
     res = rormula.eval_asdf(df)
     ref = df.eval(s)
     np.allclose(res[name].to_numpy(), ref.values)
     s = "5/3"
     rormula = Arithmetic(s, name)
     res = rormula.eval_asdf(df)
-    ref = df.eval(s)    
+    ref = df.eval(s)
     np.allclose(res[name].to_numpy(), ref)
 
 
 if __name__ == "__main__":
+    test_arithmetic()
     test_scalar_scalar()
```

### Comparing `rormula-0.1.5/rormula/test/test_meta.py` & `rormula-0.1.6/rormula/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula/test/test_wilkinson.py` & `rormula-0.1.6/rormula/test/test_wilkinson.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,20 +105,23 @@
 
 
 def timing_and_test(data, formula_str):
     rormula = Wilkinson(formula_str)
     # keeping data numerical and categorical data separated is faster
     separated_data = ror.separate_num_cat(data)
     M_r = timing(partial(rormula.eval, data=separated_data), "Rormula")
+    M_r_asdf = timing(partial(rormula.eval_asdf, data=data), "Rormula asdf")
 
     assert M_r is not None
+    assert M_r_asdf is not None
     names, M_r = M_r
     if len(names) == 0:
         return
     M_r = pd.DataFrame(data=M_r, columns=names)
+    assert np.allclose(M_r, M_r_asdf)
     formula = formulaic.Formula(formula_str.replace("^", "**"))
     M_f = timing(partial(formula.get_model_matrix, data=data), "Formulaic")
 
     assert M_f is not None
     assert np.allclose(cast(pd.Series, M_f["e:f"]), M_r["e:f"])
     assert np.allclose(cast(pd.Series, M_f["f"]), M_r["f"])
     assert np.allclose(cast(pd.Series, M_f["c:d"]), M_r["c:d"])
@@ -182,8 +185,11 @@
     rormula = Wilkinson("alpha + beta + alpha:gamma")
     names, mm = rormula.eval(separated_data)
     assert names == ["Intercept", "alpha", "beta", "alpha:gamma"]
     assert mm.shape == (100, 4)
 
 
 if __name__ == "__main__":
-    test_small_numerical()
+    print("- test just numerical")
+    test_numerical()
+    print("- test numerical and categorical")
+    test_num_cat()
```

### Comparing `rormula-0.1.5/Cargo.lock` & `rormula-0.1.6/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -194,33 +194,33 @@
 checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "errno"
-version = "0.3.5"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3e13f66a2f95e32a39eaa81f6b95d42878ca0e1db0c7543723dfe12557e860"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "exmex"
-version = "0.19.0"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00ba02c553b1567daf3831b357b48c72e56ea159c0d7d4cb2ce8b1ba4cb4ea58"
+checksum = "b3d756a702ec06bb080cf553645cfec9adcc78c054ddb0a3436636f812d3553e"
 dependencies = [
  "lazy_static",
  "num",
  "regex",
  "smallvec",
 ]
 
@@ -249,19 +249,19 @@
 name = "hermit-abi"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
 
 [[package]]
 name = "home"
-version = "0.5.5"
+version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
+checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
@@ -305,23 +305,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.149"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a08173bc88b7955d1b3145aa561539096c421ac8debde8cbc3612ec635fee29b"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.10"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2479e8c062e40bf0066ffa0bc823de0a9368974af99c9f6df941d2c231e03f"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -468,17 +468,17 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -545,80 +545,88 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9a81d2759aae1dae668f783c308bc5c8ebd191ff4184aaa1b37f65a6ae5a56f"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset 0.9.0",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "python3-dll-a",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
 name = "python3-dll-a"
 version = "0.2.6"
@@ -672,77 +680,77 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "rormula"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "criterion",
  "numpy",
  "pyo3",
  "rormula-rs",
  "which",
 ]
 
 [[package]]
 name = "rormula-rs"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "exmex",
  "numpy",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.20"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67ce50cb2e16c2903e30d1cbccfd8387a74b9d4c938b6a4c5ec6cc7556f7a8a0"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.4.1",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
@@ -791,17 +799,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
@@ -921,23 +929,22 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
-version = "5.0.0"
+version = "6.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bf3ea8596f3a0dd5980b46430f2058dfe2c36a27ccfbb1845d6fbfcd9ba6e14"
+checksum = "8211e4f58a2b2805adfbefbc07bab82958fc91e3836339b1ab7ae32465dce0d7"
 dependencies = [
  "either",
  "home",
- "once_cell",
  "rustix",
- "windows-sys 0.48.0",
+ "winsafe",
 ]
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
@@ -982,14 +989,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -1012,89 +1028,159 @@
  "windows_i686_msvc 0.48.5",
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
+name = "windows-targets"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
+]
+
+[[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+
+[[package]]
+name = "winsafe"
+version = "0.0.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d135d17ab770252ad95e9a872d365cf3090e3be864a34ab46f48555993efc904"
```

### Comparing `rormula-0.1.5/pyproject.toml` & `rormula-0.1.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rormula"
 requires-python = ">=3.7"
-version = "0.1.5"
+version = "0.1.6"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = ["pandas"]
 license = {text = "BSD-3-Clause"}
 description = "Formula parser and evaluator for Wilkinson notation"
@@ -21,9 +21,9 @@
 [project.urls]
 repository = "https://github.com/basf/rormula"
 homepage = "https://github.com/basf/rormula"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "rormula/Cargo.toml"
-[tool.ruff]
+[tool.ruff.lint]
 ignore = ["E731"]
```

### Comparing `rormula-0.1.5/rormula/rormula.pyi` & `rormula-0.1.6/rormula/rormula.pyi`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/rormula/__init__.py` & `rormula-0.1.6/rormula/__init__.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/README-pypi.md` & `rormula-0.1.6/README-pypi.md`

 * *Files identical despite different names*

### Comparing `rormula-0.1.5/PKG-INFO` & `rormula-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rormula
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: pandas
 Summary: Formula parser and evaluator for Wilkinson notation
 Keywords: design of experiments,Wilkinson,parser,eval,doe
 Author-email: Behrang Shafei <behrang.shafei@basf.com>
 License: BSD-3-Clause
```

