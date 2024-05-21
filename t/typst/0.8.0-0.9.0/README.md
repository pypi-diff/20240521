# Comparing `tmp/typst-0.8.0.tar.gz` & `tmp/typst-0.9.0.tar.gz`

## Comparing `typst-0.8.0.tar` & `typst-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 typst-0.8.0/Cargo.toml
--rw-r--r--   0     1001      127     3443 2023-09-14 13:10:01.000000 typst-0.8.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      692 2023-09-14 13:10:01.000000 typst-0.8.0/.gitignore
--rw-r--r--   0     1001      127     9723 2023-09-14 13:10:01.000000 typst-0.8.0/LICENSE
--rw-r--r--   0     1001      127      690 2023-09-14 13:10:01.000000 typst-0.8.0/README.md
--rw-r--r--   0     1001      127      419 2023-09-14 13:10:01.000000 typst-0.8.0/pyproject.toml
--rw-r--r--   0     1001      127       74 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/__init__.py
--rw-r--r--   0     1001      127     1071 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/__init__.pyi
--rw-r--r--   0     1001      127   331992 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
--rw-r--r--   0     1001      127   253580 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
--rw-r--r--   0     1001      127   251932 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
--rw-r--r--   0     1001      127   340712 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/DejaVuSansMono.ttf
--rw-r--r--   0     1001      127   806856 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/LinLibertine_R.ttf
--rw-r--r--   0     1001      127   748600 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/LinLibertine_RB.ttf
--rw-r--r--   0     1001      127   533532 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/LinLibertine_RBI.ttf
--rw-r--r--   0     1001      127   721340 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/LinLibertine_RI.ttf
--rw-r--r--   0     1001      127   499128 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/NewCM10-Bold.otf
--rw-r--r--   0     1001      127   445800 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/NewCM10-BoldItalic.otf
--rw-r--r--   0     1001      127   464808 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/NewCM10-Italic.otf
--rw-r--r--   0     1001      127   547508 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/NewCM10-Regular.otf
--rw-r--r--   0     1001      127  2161432 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/NewCMMath-Book.otf
--rw-r--r--   0     1001      127  1229208 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/fonts/NewCMMath-Regular.otf
--rw-r--r--   0     1001      127        1 2023-09-14 13:10:01.000000 typst-0.8.0/python/typst/py.typed
--rw-r--r--   0     1001      127     4662 2023-09-14 13:10:01.000000 typst-0.8.0/src/compiler.rs
--rw-r--r--   0     1001      127     2670 2023-09-14 13:10:01.000000 typst-0.8.0/src/download.rs
--rw-r--r--   0     1001      127     4304 2023-09-14 13:10:01.000000 typst-0.8.0/src/fonts.rs
--rw-r--r--   0     1001      127     2961 2023-09-14 13:10:01.000000 typst-0.8.0/src/lib.rs
--rw-r--r--   0     1001      127     1897 2023-09-14 13:10:01.000000 typst-0.8.0/src/package.rs
--rw-r--r--   0     1001      127     8290 2023-09-14 13:10:01.000000 typst-0.8.0/src/world.rs
--rw-r--r--   0     1001      127    75333 2023-09-14 13:10:01.000000 typst-0.8.0/Cargo.lock
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 typst-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1205 1970-01-01 00:00:00.000000 typst-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      127     3549 2023-11-18 05:47:04.000000 typst-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      692 2023-11-18 05:47:04.000000 typst-0.9.0/.gitignore
+-rw-r--r--   0     1001      127     9723 2023-11-18 05:47:04.000000 typst-0.9.0/LICENSE
+-rw-r--r--   0     1001      127      690 2023-11-18 05:47:04.000000 typst-0.9.0/README.md
+-rw-r--r--   0     1001      127       74 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/__init__.py
+-rw-r--r--   0     1001      127     1071 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/__init__.pyi
+-rw-r--r--   0     1001      127   331992 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0     1001      127   253580 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf
+-rw-r--r--   0     1001      127   251932 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf
+-rw-r--r--   0     1001      127   340712 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0     1001      127   806856 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/LinLibertine_R.ttf
+-rw-r--r--   0     1001      127   748600 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/LinLibertine_RB.ttf
+-rw-r--r--   0     1001      127   533532 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/LinLibertine_RBI.ttf
+-rw-r--r--   0     1001      127   721340 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/LinLibertine_RI.ttf
+-rw-r--r--   0     1001      127   499128 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/NewCM10-Bold.otf
+-rw-r--r--   0     1001      127   445800 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/NewCM10-BoldItalic.otf
+-rw-r--r--   0     1001      127   464808 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/NewCM10-Italic.otf
+-rw-r--r--   0     1001      127   547508 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/NewCM10-Regular.otf
+-rw-r--r--   0     1001      127  2161432 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/NewCMMath-Book.otf
+-rw-r--r--   0     1001      127  1229208 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/fonts/NewCMMath-Regular.otf
+-rw-r--r--   0     1001      127        1 2023-11-18 05:47:04.000000 typst-0.9.0/python/typst/py.typed
+-rw-r--r--   0     1001      127     5170 2023-11-18 05:47:04.000000 typst-0.9.0/src/compiler.rs
+-rw-r--r--   0     1001      127     2670 2023-11-18 05:47:04.000000 typst-0.9.0/src/download.rs
+-rw-r--r--   0     1001      127     2416 2023-11-18 05:47:04.000000 typst-0.9.0/src/fonts.rs
+-rw-r--r--   0     1001      127     3057 2023-11-18 05:47:04.000000 typst-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127     1897 2023-11-18 05:47:04.000000 typst-0.9.0/src/package.rs
+-rw-r--r--   0     1001      127    10339 2023-11-18 05:47:04.000000 typst-0.9.0/src/world.rs
+-rw-r--r--   0     1001      127    74900 2023-11-18 05:47:04.000000 typst-0.9.0/Cargo.lock
+-rw-r--r--   0     1001      127      481 2023-11-18 05:47:04.000000 typst-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 typst-0.9.0/PKG-INFO
```

### Comparing `typst-0.8.0/Cargo.toml` & `typst-0.9.0/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typst-py"
-version = "0.8.0"
+version = "0.9.0"
 edition = "2021"
 description = "Python binding to typst"
 license = "Apache-2.0"
 repository = "https://github.com/messense/typst-py"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
@@ -15,30 +15,31 @@
 chrono = { version = "0.4.24", default-features = false, features = [
     "clock",
     "std",
 ] }
 codespan-reporting = "0.11"
 comemo = "0.3"
 dirs = "5"
-ecow = "0.1.1"
+ecow = "0.2"
 env_proxy = "0.4"
+filetime = "0.2.22"
 flate2 = "1"
-memmap2 = "0.7"
-pathdiff = "0.1"
-pyo3 = { version = "0.19.0", features = ["abi3-py37"] }
+fontdb = "0.15.0"
+pathdiff = "0.2"
+pyo3 = { version = "0.20.0", features = ["abi3-py37"] }
 same-file = "1"
 siphasher = "1.0"
 tar = "0.4"
-typst = { git = "https://github.com/typst/typst.git", tag = "v0.8.0" }
-typst-library = { git = "https://github.com/typst/typst.git", tag = "v0.8.0" }
+typst = { git = "https://github.com/typst/typst.git", tag = "v0.9.0" }
+typst-library = { git = "https://github.com/typst/typst.git", tag = "v0.9.0" }
 ureq = { version = "2", default-features = false, features = [
     "gzip",
     "socks-proxy",
 ] }
-walkdir = "2"
+walkdir = "2.4.0"
 
 [target.'cfg(target_os = "linux")'.dependencies]
 openssl = { version = "0.10", optional = true }
 
 [features]
 default = ["rustls"]
 rustls = ["ureq/tls"]
```

### Comparing `typst-0.8.0/.github/workflows/CI.yml` & `typst-0.9.0/.github/workflows/CI.yml`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         env:
           # Make psm compile, see https://github.com/rust-lang/stacker/issues/79
           CFLAGS_s390x_unknown_linux_gnu: "-march=z10"
+          # Workaround ring 0.17 build issue
+          CFLAGS_aarch64_unknown_linux_gnu: "-D__ARM_ARCH=8"
         with:
           target: ${{ matrix.target }}
           args: --release --out dist ${{ matrix.extra-build-args || '' }}
           sccache: 'true'
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
```

### Comparing `typst-0.8.0/.gitignore` & `typst-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/LICENSE` & `typst-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/README.md` & `typst-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/__init__.pyi` & `typst-0.9.0/python/typst/__init__.pyi`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/DejaVuSansMono-Bold.ttf` & `typst-0.9.0/python/typst/fonts/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf` & `typst-0.9.0/python/typst/fonts/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf` & `typst-0.9.0/python/typst/fonts/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/DejaVuSansMono.ttf` & `typst-0.9.0/python/typst/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/LinLibertine_R.ttf` & `typst-0.9.0/python/typst/fonts/LinLibertine_R.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/LinLibertine_RB.ttf` & `typst-0.9.0/python/typst/fonts/LinLibertine_RB.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/LinLibertine_RBI.ttf` & `typst-0.9.0/python/typst/fonts/LinLibertine_RBI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/LinLibertine_RI.ttf` & `typst-0.9.0/python/typst/fonts/LinLibertine_RI.ttf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/NewCM10-Bold.otf` & `typst-0.9.0/python/typst/fonts/NewCM10-Bold.otf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/NewCM10-BoldItalic.otf` & `typst-0.9.0/python/typst/fonts/NewCM10-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/NewCM10-Italic.otf` & `typst-0.9.0/python/typst/fonts/NewCM10-Italic.otf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/NewCM10-Regular.otf` & `typst-0.9.0/python/typst/fonts/NewCM10-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/NewCMMath-Book.otf` & `typst-0.9.0/python/typst/fonts/NewCMMath-Book.otf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/python/typst/fonts/NewCMMath-Regular.otf` & `typst-0.9.0/python/typst/fonts/NewCMMath-Regular.otf`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/src/compiler.rs` & `typst-0.9.0/src/compiler.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+use chrono::{Datelike, Timelike};
 use codespan_reporting::diagnostic::{Diagnostic, Label};
 use codespan_reporting::term::{self, termcolor};
 use typst::diag::{Severity, SourceDiagnostic, StrResult};
 use typst::doc::Document;
-use typst::eval::{eco_format, Tracer};
+use typst::eval::{eco_format, Datetime, Tracer};
 use typst::syntax::{FileId, Source, Span};
 use typst::{World, WorldExt};
 
 use crate::world::SystemWorld;
 
 type CodespanResult<T> = Result<T, CodespanError>;
 type CodespanError = codespan_reporting::files::Error;
@@ -19,27 +20,41 @@
 
         let mut tracer = Tracer::default();
         let result = typst::compile(self, &mut tracer);
         let warnings = tracer.warnings();
 
         match result {
             // Export the PDF / PNG.
-            Ok(document) => Ok(export_pdf(&document)?),
+            Ok(document) => Ok(export_pdf(&document, self)?),
             Err(errors) => Err(format_diagnostics(self, &errors, &warnings).unwrap().into()),
         }
     }
 }
 
 /// Export to a PDF.
 #[inline]
-fn export_pdf(document: &Document) -> StrResult<Vec<u8>> {
-    let buffer = typst::export::pdf(document);
+fn export_pdf(document: &Document, world: &SystemWorld) -> StrResult<Vec<u8>> {
+    let ident = world.input().to_string_lossy();
+    let buffer = typst::export::pdf(document, Some(&ident), now());
     Ok(buffer)
 }
 
+/// Get the current date and time in UTC.
+fn now() -> Option<Datetime> {
+    let now = chrono::Local::now().naive_utc();
+    Datetime::from_ymd_hms(
+        now.year(),
+        now.month().try_into().ok()?,
+        now.day().try_into().ok()?,
+        now.hour().try_into().ok()?,
+        now.minute().try_into().ok()?,
+        now.second().try_into().ok()?,
+    )
+}
+
 /// Format diagnostic messages.\
 pub fn format_diagnostics(
     world: &SystemWorld,
     errors: &[SourceDiagnostic],
     warnings: &[SourceDiagnostic],
 ) -> Result<String, codespan_reporting::files::Error> {
     let mut w = termcolor::Buffer::no_color();
```

### Comparing `typst-0.8.0/src/download.rs` & `typst-0.9.0/src/download.rs`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/src/lib.rs` & `typst-0.9.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 mod compiler;
 mod download;
 mod fonts;
 mod package;
 mod world;
 
 fn resources_path(py: Python<'_>, package: &str) -> PyResult<PathBuf> {
-    let resources = py.import("importlib.resources")?;
+    let resources = match py.import("importlib.resources") {
+        Ok(module) => module,
+        Err(_) => py.import("importlib_resources")?,
+    };
     let files = resources.call_method1("files", (package,))?;
     let files = resources.call_method1("as_file", (files,))?;
     let path = files.call_method0("__enter__")?; // enter python context manager
     match path.extract() {
         Ok(path) => {
             let none = py.None();
             files.call_method1("__exit__", (&none, &none, &none))?;
```

### Comparing `typst-0.8.0/src/package.rs` & `typst-0.9.0/src/package.rs`

 * *Files identical despite different names*

### Comparing `typst-0.8.0/src/world.rs` & `typst-0.9.0/src/world.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-use std::cell::{OnceCell, RefCell, RefMut};
+use std::cell::{Cell, OnceCell, RefCell, RefMut};
 use std::collections::HashMap;
 use std::fs;
 use std::hash::Hash;
 use std::path::{Path, PathBuf};
 
 use chrono::{DateTime, Datelike, Local};
 use comemo::Prehashed;
+use filetime::FileTime;
 use same_file::Handle;
 use siphasher::sip128::{Hasher128, SipHasher13};
 use typst::diag::{FileError, FileResult, StrResult};
-use typst::eval::{Bytes, Datetime, Library};
+use typst::eval::{eco_format, Bytes, Datetime, Library};
 use typst::font::{Font, FontBook};
 use typst::syntax::{FileId, Source, VirtualPath};
 use typst::World;
 
 use crate::fonts::{FontSearcher, FontSlot};
 use crate::package::prepare_package;
 
 /// A world that provides access to the operating system.
 pub struct SystemWorld {
     /// The working directory.
     workdir: Option<PathBuf>,
+    /// The canonical path to the input file.
+    input: PathBuf,
     /// The root relative to which absolute paths are resolved.
     root: PathBuf,
     /// The input path.
     main: FileId,
     /// Typst's standard library.
     library: Prehashed<Library>,
     /// Metadata about discovered fonts.
@@ -32,15 +35,15 @@
     /// Locations of and storage for lazily loaded fonts.
     fonts: Vec<FontSlot>,
     /// Maps package-path combinations to canonical hashes. All package-path
     /// combinations that point to the same file are mapped to the same hash. To
     /// be used in conjunction with `paths`.
     hashes: RefCell<HashMap<FileId, FileResult<PathHash>>>,
     /// Maps canonical path hashes to source files and buffers.
-    paths: RefCell<HashMap<PathHash, PathSlot>>,
+    slots: RefCell<HashMap<PathHash, PathSlot>>,
     /// The current datetime if requested. This is stored here to ensure it is
     /// always the same within one compilation. Reset between compilations.
     now: OnceCell<DateTime<Local>>,
 }
 
 impl World for SystemWorld {
     fn library(&self) -> &Prehashed<Library> {
@@ -108,23 +111,18 @@
                 // access. Note: It can still escape via symlinks.
                 system_path = id.vpath().resolve(root).ok_or(FileError::AccessDenied)?;
 
                 PathHash::new(&system_path)
             })
             .clone()?;
 
-        Ok(RefMut::map(self.paths.borrow_mut(), |paths| {
-            paths.entry(hash).or_insert_with(|| PathSlot {
-                id,
-                // This will only trigger if the `or_insert_with` above also
-                // triggered.
-                system_path,
-                source: OnceCell::new(),
-                buffer: OnceCell::new(),
-            })
+        Ok(RefMut::map(self.slots.borrow_mut(), |paths| {
+            paths
+                .entry(hash)
+                .or_insert_with(|| PathSlot::new(id, system_path))
         }))
     }
 
     /// The id of the main source file.
     pub fn main(&self) -> FileId {
         self.main
     }
@@ -138,18 +136,25 @@
     pub fn workdir(&self) -> &Path {
         self.workdir.as_deref().unwrap_or(Path::new("."))
     }
 
     /// Reset the compilation state in preparation of a new compilation.
     pub fn reset(&mut self) {
         self.hashes.borrow_mut().clear();
-        self.paths.borrow_mut().clear();
+        for slot in self.slots.borrow_mut().values_mut() {
+            slot.reset();
+        }
         self.now.take();
     }
 
+    /// Return the canonical path to the input file.
+    pub fn input(&self) -> &PathBuf {
+        &self.input
+    }
+
     /// Lookup a source file by id.
     #[track_caller]
     pub fn lookup(&self, id: FileId) -> Source {
         self.source(id)
             .expect("file id does not point to any source file")
     }
 }
@@ -179,68 +184,138 @@
     pub fn font_files(mut self, font_files: Vec<PathBuf>) -> Self {
         self.font_files = font_files;
         self
     }
 
     pub fn build(self) -> StrResult<SystemWorld> {
         let mut searcher = FontSearcher::new();
-        searcher.search(&self.font_paths);
-
-        for path in self.font_files {
-            searcher.search_file(path);
-        }
+        searcher.search(&self.font_paths, &self.font_files);
 
+        let input = self.main.canonicalize().map_err(|_| {
+            eco_format!("input file not found (searched at {})", self.main.display())
+        })?;
         // Resolve the virtual path of the main file within the project root.
         let main_path = VirtualPath::within_root(&self.main, &self.root)
             .ok_or("input file must be contained in project root")?;
 
         let world = SystemWorld {
             workdir: std::env::current_dir().ok(),
+            input,
             root: self.root,
             main: FileId::new(None, main_path),
             library: Prehashed::new(typst_library::build()),
             book: Prehashed::new(searcher.book),
             fonts: searcher.fonts,
             hashes: RefCell::default(),
-            paths: RefCell::default(),
+            slots: RefCell::default(),
             now: OnceCell::new(),
         };
         Ok(world)
     }
 }
 
 /// Holds canonical data for all paths pointing to the same entity.
 ///
 /// Both fields can be populated if the file is both imported and read().
 struct PathSlot {
     /// The slot's canonical file id.
     id: FileId,
     /// The slot's path on the system.
-    system_path: PathBuf,
-    /// The lazily loaded source file for a path hash.
-    source: OnceCell<FileResult<Source>>,
-    /// The lazily loaded buffer for a path hash.
-    buffer: OnceCell<FileResult<Bytes>>,
+    path: PathBuf,
+    /// The lazily loaded and incrementally updated source file.
+    source: SlotCell<Source>,
+    /// The lazily loaded raw byte buffer.
+    file: SlotCell<Bytes>,
 }
 
 impl PathSlot {
+    /// Create a new path slot.
+    fn new(id: FileId, path: PathBuf) -> Self {
+        Self {
+            id,
+            path,
+            file: SlotCell::new(),
+            source: SlotCell::new(),
+        }
+    }
+
+    /// Marks the file as not yet accessed in preparation of the next
+    /// compilation.
+    fn reset(&self) {
+        self.source.reset();
+        self.file.reset();
+    }
+
     fn source(&self) -> FileResult<Source> {
-        self.source
-            .get_or_init(|| {
-                let buf = read(&self.system_path)?;
-                let text = decode_utf8(buf)?;
-                Ok(Source::new(self.id, text))
-            })
-            .clone()
+        self.source.get_or_init(&self.path, |data, prev| {
+            let text = decode_utf8(&data)?;
+            if let Some(mut prev) = prev {
+                prev.replace(text);
+                Ok(prev)
+            } else {
+                Ok(Source::new(self.id, text.into()))
+            }
+        })
     }
 
     fn file(&self) -> FileResult<Bytes> {
-        self.buffer
-            .get_or_init(|| read(&self.system_path).map(Bytes::from))
-            .clone()
+        self.file.get_or_init(&self.path, |data, _| Ok(data.into()))
+    }
+}
+
+/// Lazily processes data for a file.
+struct SlotCell<T> {
+    data: RefCell<Option<FileResult<T>>>,
+    refreshed: Cell<FileTime>,
+    accessed: Cell<bool>,
+}
+
+impl<T: Clone> SlotCell<T> {
+    /// Creates a new, empty cell.
+    fn new() -> Self {
+        Self {
+            data: RefCell::new(None),
+            refreshed: Cell::new(FileTime::zero()),
+            accessed: Cell::new(false),
+        }
+    }
+
+    /// Marks the cell as not yet accessed in preparation of the next
+    /// compilation.
+    fn reset(&self) {
+        self.accessed.set(false);
+    }
+
+    /// Gets the contents of the cell or initialize them.
+    fn get_or_init(
+        &self,
+        path: &Path,
+        f: impl FnOnce(Vec<u8>, Option<T>) -> FileResult<T>,
+    ) -> FileResult<T> {
+        let mut borrow = self.data.borrow_mut();
+        if let Some(data) = &*borrow {
+            if self.accessed.replace(true) || self.current(path) {
+                return data.clone();
+            }
+        }
+
+        self.accessed.set(true);
+        self.refreshed.set(FileTime::now());
+        let prev = borrow.take().and_then(Result::ok);
+        let value = read(path).and_then(|data| f(data, prev));
+        *borrow = Some(value.clone());
+        value
+    }
+
+    /// Whether the cell contents are still up to date with the file system.
+    fn current(&self, path: &Path) -> bool {
+        fs::metadata(path).map_or(false, |meta| {
+            let modified = FileTime::from_last_modification_time(&meta);
+            modified < self.refreshed.get()
+        })
     }
 }
 
 /// A hash that is the same for all paths pointing to the same entity.
 #[derive(Debug, Copy, Clone, Eq, PartialEq, Hash)]
 struct PathHash(u128);
 
@@ -261,16 +336,13 @@
         Err(FileError::IsDirectory)
     } else {
         fs::read(path).map_err(f)
     }
 }
 
 /// Decode UTF-8 with an optional BOM.
-fn decode_utf8(buf: Vec<u8>) -> FileResult<String> {
-    Ok(if buf.starts_with(b"\xef\xbb\xbf") {
-        // Remove UTF-8 BOM.
-        std::str::from_utf8(&buf[3..])?.into()
-    } else {
-        // Assume UTF-8.
-        String::from_utf8(buf)?
-    })
+fn decode_utf8(buf: &[u8]) -> FileResult<&str> {
+    // Remove UTF-8 BOM.
+    Ok(std::str::from_utf8(
+        buf.strip_prefix(b"\xef\xbb\xbf").unwrap_or(buf),
+    )?)
 }
```

### Comparing `typst-0.8.0/Cargo.lock` & `typst-0.9.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,29 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "ahash"
+version = "0.7.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a824f2aa7e75a0c98c5a504fceb80649e9c35265d44525b5f94de4771a395cd"
+dependencies = [
+ "getrandom",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
 name = "aho-corasick"
-version = "1.0.5"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c378d78423fdad8089616f827526ee33c19f2fddbd5de1629152c9593ba4783"
+checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -29,14 +40,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "approx"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
 [[package]]
 name = "arrayvec"
@@ -54,25 +74,24 @@
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
 name = "base64"
-version = "0.21.4"
+version = "0.21.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ba43ea6f343b788c8764558649e08df62f86c6ef251fdaeb1ffd010a9ae50a2"
+checksum = "35636a1494ede3b646cc98f74f8e62c773a38a659ebc777a2cf26b9b74171df9"
 
 [[package]]
 name = "biblatex"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc9fd60378277e44cd400ec5f35e768ce0d5a63d8d18ac7b1a9231196251dae5"
+checksum = "2e41df82f0d1c4919d946bb0c7c3d179b6071246243d308a1bdee6cfecee3bc7"
 dependencies = [
- "chrono",
  "numerals",
  "paste",
  "strum",
  "unicode-normalization",
  "unscanny",
 ]
 
@@ -97,51 +116,79 @@
 [[package]]
 name = "bit-vec"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
 
 [[package]]
-name = "bit_field"
-version = "0.10.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc827186963e592360843fb5ba4b973e145841266c1357f7180c43526f2e5b61"
-
-[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4682ae6287fcf752ecaabbfcc7b6f9b72aa33933dc23a554d853aea8eea8635"
+checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
 name = "bumpalo"
-version = "3.13.0"
+version = "3.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+
+[[package]]
+name = "bytecheck"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
+dependencies = [
+ "bytecheck_derive",
+ "ptr_meta",
+ "simdutf8",
+]
+
+[[package]]
+name = "bytecheck_derive"
+version = "0.6.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a7ec4c6f261935ad534c0c22dbef2201b45918860eb1c574b972bd213a76af61"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
 
 [[package]]
 name = "bytemuck"
 version = "1.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
 
 [[package]]
 name = "byteorder"
-version = "1.4.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "cc"
 version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
 dependencies = [
@@ -170,17 +217,17 @@
 name = "chinese-variant"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aeea139b89efab957972956e5d3e4efb66a6c261f726abf6911040cc8ef700f7"
 
 [[package]]
 name = "chrono"
-version = "0.4.30"
+version = "0.4.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "defd4e7873dbddba6c7c91e199c7fcb946abc4a6a4ac3195400bcfb01b5de877"
+checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
  "windows-targets",
 ]
 
@@ -204,15 +251,25 @@
 [[package]]
 name = "ciborium-ll"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
- "half 1.8.2",
+ "half",
+]
+
+[[package]]
+name = "citationberg"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c857faf24e89710f105b623c174508070a9e11e056a749f251ca4c56f59ad88"
+dependencies = [
+ "quick-xml 0.28.2",
+ "serde",
 ]
 
 [[package]]
 name = "cobs"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67ba02a97a2bd10f4b59b25c7973101c79642302776489e030cd13cdab09ed15"
@@ -267,103 +324,66 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
-name = "crc32fast"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "crossbeam-channel"
-version = "0.5.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
-dependencies = [
- "cfg-if",
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-deque"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
-dependencies = [
- "cfg-if",
- "crossbeam-epoch",
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-epoch"
-version = "0.9.15"
+name = "core_maths"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "e3b02505ccb8c50b0aa21ace0fc08c3e53adebd4e58caa18a36152803c7709a3"
 dependencies = [
- "autocfg",
- "cfg-if",
- "crossbeam-utils",
- "memoffset",
- "scopeguard",
+ "libm",
 ]
 
 [[package]]
-name = "crossbeam-utils"
-version = "0.8.16"
+name = "crc32fast"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
+checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "crunchy"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
-
-[[package]]
 name = "csv"
-version = "1.2.2"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
+checksum = "ac574ff4d437a7b5ad237ef331c17ccca63c46479e5b5453eb8e10bb99a759fe"
 dependencies = [
  "csv-core",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "csv-core"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "data-url"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d7439c3735f405729d52c3fbbe4de140eaf938a1fe47d227c27f8254d4302a5"
+checksum = "41b319d1b62ffbd002e057f36bebd1f42b9f97927c9577461d855f3513c4289f"
 
 [[package]]
 name = "deranged"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2696e8a945f658fd14dc3b87242e6b80cd0f36ff04ea560fa39082368847946"
+checksum = "0f32d04922c60427da6f9fef14d042d9edddef64cb9d4ce0d64d0685fbeb1fd3"
+dependencies = [
+ "powerfmt",
+]
 
 [[package]]
 name = "dirs"
 version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
 dependencies = [
@@ -386,49 +406,49 @@
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
 
 [[package]]
 name = "ecow"
-version = "0.1.2"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d1990d053cf6edf3f030682dba3b0eb65ef01fabb2686072765d8a17d6728e8"
+checksum = "e6ea5e3f9cda726431da9d1a8d5a29785d544b31e98e1ca7a210906244002e02"
 dependencies = [
  "serde",
 ]
 
 [[package]]
-name = "either"
-version = "1.9.0"
+name = "embedded-io"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "ef1a6892d9eef45c8fa6b9e0086428a2cca8491aca8f787c534a3d6d0bcb3ced"
 
 [[package]]
 name = "enum-ordinalize"
-version = "3.1.13"
+version = "3.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4f76552f53cefc9a7f64987c3701b99d982f7690606fd67de1d09712fbf52f1"
+checksum = "1bf1fa3f06bbff1ea5b1a9c7b14aa992a39657db60a2759457328d7e058f49ee"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "env_proxy"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a5019be18538406a43b5419a5501461f0c8b49ea7dfda0cfc32f4e51fc44be1"
@@ -441,70 +461,49 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.3"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "136526188508e25c6fef639d7927dfb3e0e3084488bf202267829cf7fc23dbdd"
+checksum = "f258a7194e7f7c2a7837a8913aeab7fd8c383457034fa20ce4dd3dcb813e8eb8"
 dependencies = [
- "errno-dragonfly",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
-dependencies = [
- "cc",
- "libc",
-]
-
-[[package]]
-name = "exr"
-version = "1.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1e481eb11a482815d3e9d618db8c42a93207134662873809335a92327440c18"
-dependencies = [
- "bit_field",
- "flume",
- "half 2.2.1",
- "lebe",
- "miniz_oxide",
- "rayon-core",
- "smallvec",
- "zune-inflate",
-]
-
-[[package]]
 name = "fancy-regex"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b95f7c0680e4142284cf8b22c14a476e87d61b004a3a0861872b32ef7ead40a2"
 dependencies = [
  "bit-set",
  "regex",
 ]
 
 [[package]]
+name = "fast-srgb8"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd2e7510819d6fbf51a5545c8f922716ecfb14df168a3242f7d33e0239efe6a1"
+
+[[package]]
 name = "fastrand"
-version = "2.0.0"
+version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6999dc1837253364c2ebb0704ba97994bd874e8f195d665c50b7548f6ea92764"
+checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
 
 [[package]]
 name = "fdeflate"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+checksum = "64d6dafc854908ff5da46ff3f8f473c6984119a2876a383a860246dd7841a868"
 dependencies = [
  "simd-adler32",
 ]
 
 [[package]]
 name = "filetime"
 version = "0.2.22"
@@ -515,57 +514,55 @@
  "libc",
  "redox_syscall 0.3.5",
  "windows-sys",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6c98ee8095e9d1dcbf2fcc6d95acccb90d1c81db1e44725c6a984b1dbdfb010"
+checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "float-cmp"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
 
 [[package]]
-name = "flume"
-version = "0.10.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
-dependencies = [
- "futures-core",
- "futures-sink",
- "nanorand",
- "pin-project",
- "spin 0.9.8",
-]
-
-[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "fontconfig-parser"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "674e258f4b5d2dcd63888c01c68413c51f565e8af99d2f7701c7b81d79ef41c4"
+dependencies = [
+ "roxmltree",
+]
+
+[[package]]
 name = "fontdb"
-version = "0.14.1"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af8d8cbea8f21307d7e84bca254772981296f058a1d36b461bf4d83a7499fc9e"
+checksum = "020e203f177c0fb250fb19455a252e838d2bbbce1f80f25ecc42402aafa8cd38"
 dependencies = [
+ "fontconfig-parser",
  "log",
+ "memmap2",
  "slotmap",
  "tinyvec",
- "ttf-parser 0.19.2",
+ "ttf-parser",
 ]
 
 [[package]]
 name = "foreign-types"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
@@ -585,36 +582,28 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
-name = "futures-core"
-version = "0.3.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
-
-[[package]]
-name = "futures-sink"
-version = "0.3.28"
+name = "funty"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "fe9006bed769170c11f845cf00c7c1e9092aeb3f268e007c3e760ac68008070f"
 dependencies = [
  "cfg-if",
- "js-sys",
  "libc",
  "wasi",
- "wasm-bindgen",
 ]
 
 [[package]]
 name = "gif"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
@@ -626,311 +615,305 @@
 [[package]]
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
-name = "half"
-version = "2.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
-dependencies = [
- "crunchy",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+dependencies = [
+ "ahash",
+]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.0"
+version = "0.14.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
 
 [[package]]
 name = "hayagriva"
-version = "0.3.2"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065e90e53aa502be868a307f58ca6b46e31143641e809047c689de75619d8cea"
+checksum = "c5af3d464a6b5ae882f15fe1da4e696fd96b77fee78ded933e0ad81d1d87cbc5"
 dependencies = [
  "biblatex",
- "chrono",
- "isolang",
- "lazy_static",
- "linked-hash-map",
+ "ciborium",
+ "citationberg",
+ "indexmap",
+ "numerals",
  "paste",
- "regex",
- "strum",
+ "rkyv",
+ "serde",
+ "serde_yaml",
  "thiserror",
  "unic-langid",
  "unicode-segmentation",
+ "unscanny",
  "url",
- "yaml-rust",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
-name = "hermit-abi"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
-
-[[package]]
 name = "hypher"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "723e315d77ea8aa1aedf53ad979ff0e763cfa2a1b3403248e427ae052f403cad"
+checksum = "94bf16dd62ea2bec617a6f8a3e1ba03107311783069a647787ac689d1f35321e"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.57"
+version = "0.1.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+checksum = "8326b86b6cff230b97d0d312a6c40a60726df3332e721f72a1b035f451663b20"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows",
+ "windows-core",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "icu_collections"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef8302d8dfd6044d3ddb3f807a5ef3d7bbca9a574959c6d6e4dc39aa7012d0d5"
+checksum = "137d96353afc8544d437e8a99eceb10ab291352699573b0de5b08bda38c78c60"
 dependencies = [
  "displaydoc",
  "serde",
  "yoke",
  "zerofrom",
  "zerovec",
 ]
 
 [[package]]
 name = "icu_locid"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3003f85dccfc0e238ff567693248c59153a46f4e6125ba4020b973cef4d1d335"
+checksum = "5c0aa2536adc14c07e2a521e95512b75ed8ef832f0fdf9299d4a0a45d2be2a9d"
 dependencies = [
  "displaydoc",
  "litemap",
  "tinystr",
  "writeable",
  "zerovec",
 ]
 
 [[package]]
+name = "icu_locid_transform"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57c17d8f6524fdca4471101dd71f0a132eb6382b5d6d7f2970441cb25f6f435a"
+dependencies = [
+ "displaydoc",
+ "icu_locid",
+ "icu_locid_transform_data",
+ "icu_provider",
+ "tinystr",
+ "zerovec",
+]
+
+[[package]]
+name = "icu_locid_transform_data"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "545c6c3e8bf9580e2dafee8de6f9ec14826aaf359787789c7724f1f85f47d3dc"
+
+[[package]]
 name = "icu_properties"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce0e1aa26851f16c9e04412a5911c86b7f8768dac8f8d4c5f1c568a7e5d7a434"
+checksum = "976e296217453af983efa25f287a4c1da04b9a63bf1ed63719455068e4453eb5"
 dependencies = [
  "displaydoc",
  "icu_collections",
+ "icu_locid_transform",
+ "icu_properties_data",
  "icu_provider",
  "serde",
  "tinystr",
  "zerovec",
 ]
 
 [[package]]
+name = "icu_properties_data"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f6a86c0e384532b06b6c104814f9c1b13bcd5b64409001c0d05713a1f3529d99"
+
+[[package]]
 name = "icu_provider"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8dc312a7b6148f7dfe098047ae2494d12d4034f48ade58d4f353000db376e305"
+checksum = "ba58e782287eb6950247abbf11719f83f5d4e4a5c1f2cd490d30a334bc47c2f4"
 dependencies = [
  "displaydoc",
  "icu_locid",
  "icu_provider_macros",
  "postcard",
  "serde",
  "stable_deref_trait",
+ "tinystr",
  "writeable",
  "yoke",
  "zerofrom",
  "zerovec",
 ]
 
 [[package]]
 name = "icu_provider_adapters"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4ae1e2bd0c41728b77e7c46e9afdec5e2127d1eedacc684724667d50c126bd3"
+checksum = "a229f978260da7c3aabb68cb7dc7316589936680570fe55e50fdd3f97711a4dd"
 dependencies = [
  "icu_locid",
+ "icu_locid_transform",
  "icu_provider",
  "tinystr",
- "yoke",
  "zerovec",
 ]
 
 [[package]]
 name = "icu_provider_blob"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd364c9a01f791a4bc04a74cf2a1d01d9f6926a40fd5ae1c28004e1e70d8338b"
+checksum = "4a7202cddda672db167c6352719959e9b01cb1ca576d32fa79103f61b5a73601"
 dependencies = [
  "icu_provider",
  "postcard",
  "serde",
  "writeable",
- "yoke",
+ "zerotrie",
  "zerovec",
 ]
 
 [[package]]
 name = "icu_provider_macros"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b728b9421e93eff1d9f8681101b78fa745e0748c95c655c83f337044a7e10"
+checksum = "d2abdd3a62551e8337af119c5899e600ca0c88ec8f23a46c60ba216c803dcf1a"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "icu_segmenter"
-version = "1.2.1"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3300a7b6bf187be98a57264ad094f11f2e062c2e8263132af010ff522ee5495"
+checksum = "b2dc1e8f4ba33a6a4956770ac5c08570f255d6605519fb3a859a0c0a270a2f8f"
 dependencies = [
+ "core_maths",
  "displaydoc",
  "icu_collections",
  "icu_locid",
  "icu_provider",
- "num-traits",
+ "icu_segmenter_data",
  "serde",
  "utf8_iter",
  "zerovec",
 ]
 
 [[package]]
+name = "icu_segmenter_data"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3673d6698dcffce08cfe8fc5da3c11c3f2c663d5d6137fd58ab2cbf44235ab46"
+
+[[package]]
 name = "idna"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
-name = "if_chain"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb56e1aa765b4b4f3aadfab769793b7087bb03a4ea4920644a6d238e2df5b9ed"
-
-[[package]]
 name = "image"
 version = "0.24.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f3dfdbdd72063086ff443e297b61695500514b1e41095b6fb9a5ab48a70a711"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
- "exr",
  "gif",
  "jpeg-decoder",
  "num-rational",
  "num-traits",
  "png",
- "qoi",
- "tiff",
 ]
 
 [[package]]
 name = "imagesize"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d73f573d8e8d63e6d5020011d3255b28c3ba85d6cf870a07184ed23de9284"
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
-dependencies = [
- "autocfg",
- "hashbrown 0.12.3",
-]
-
-[[package]]
-name = "indexmap"
-version = "2.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.0",
+ "hashbrown 0.14.2",
  "serde",
 ]
 
 [[package]]
 name = "indexmap-nostd"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e04e2fd2b8188ea827b32ef11de88377086d690286ab35747ef7f9bf3ccb590"
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "isolang"
-version = "2.3.0"
+version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f80f221db1bc708b71128757b9396727c04de86968081e18e89b0575e03be071"
-dependencies = [
- "phf",
-]
+checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
 name = "itoa"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
-dependencies = [
- "rayon",
-]
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "54c0c35952f67de54bb584e9fd912b3023117cbafc0a77d8f3dee1fb5f572fe8"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kurbo"
 version = "0.9.5"
@@ -943,30 +926,35 @@
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
-name = "lebe"
-version = "0.5.2"
+name = "libc"
+version = "0.2.150"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
+checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
 
 [[package]]
-name = "libc"
-version = "0.2.148"
+name = "libm"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cdc71e17332e86d2e1d38c1f99edcb6288ee11b815fb1a4b049eaa2114d369b"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
-name = "libm"
-version = "0.2.7"
+name = "libredox"
+version = "0.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+dependencies = [
+ "bitflags 2.4.1",
+ "libc",
+ "redox_syscall 0.4.1",
+]
 
 [[package]]
 name = "line-wrap"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f30344350a2a51da54c1d53be93fade8a237e545dbcc4bdbe635413f2117cab9"
 dependencies = [
@@ -977,61 +965,64 @@
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.7"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a9bad9f94746442c783ca431b22403b519cd7fbeed0533fdd6328b2f2212128"
+checksum = "969488b55f8ac402214f3f5fd243ebb7206cf82de60d3172994707a4bcc2b829"
 
 [[package]]
 name = "lipsum"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c5e9ef2d2ad6fe67a59ace27c203c8d3a71d195532ee82e3bbe0d5f9a9ca541"
 dependencies = [
  "rand",
  "rand_chacha",
 ]
 
 [[package]]
 name = "litemap"
-version = "0.7.0"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a04a5b2b6f54acba899926491d0a6c59d98012938ca2ab5befb281c034e8f94"
+checksum = "f9d642685b028806386b2b6e75685faadd3eb65a85fff7df711ce18446a422da"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
 
 [[package]]
 name = "memchr"
-version = "2.6.3"
+version = "2.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f232d6ef707e1956a43342693d2a31e72989554d58299d7a88738cc95b0d35c"
+checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
 
 [[package]]
 name = "memmap2"
-version = "0.7.1"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
+checksum = "43a5a03cefb0d953ec0be133036f14e109412fa594edc2f77227249db66cc3ed"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
@@ -1048,23 +1039,14 @@
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
-name = "nanorand"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
-dependencies = [
- "getrandom",
-]
-
-[[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
 dependencies = [
  "lazy_static",
  "libc",
@@ -1108,60 +1090,40 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
+checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
 dependencies = [
  "autocfg",
- "libm",
-]
-
-[[package]]
-name = "num_cpus"
-version = "1.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
-dependencies = [
- "hermit-abi",
- "libc",
 ]
 
 [[package]]
 name = "numerals"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e25be21376a772d15f97ae789845340a9651d3c4246ff5ebb6a2b35f9c37bd31"
 
 [[package]]
-name = "oklab"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "467e40ada50d13bab19019e3707862b5076ca15841f31ee1474c40397c1b9f11"
-dependencies = [
- "rgb",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "openssl"
-version = "0.10.57"
+version = "0.10.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bac25ee399abb46215765b1cb35bc0212377e58a061560d8b29b024fd0430e7c"
+checksum = "7a257ad03cd8fb16ad4172fedf8094451e1af1c4b70097636ef2eac9a5f0cc33"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags 2.4.1",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -1170,37 +1132,37 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "300.1.3+3.1.2"
+version = "300.1.6+3.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd2c101a165fff9935e34def4669595ab1c7847943c42be86e21503e482be107"
+checksum = "439fac53e092cd7442a3660c85dde4643ab3b5bd39040912388dcdabf6b88085"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.93"
+version = "0.9.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db4d56a4c0478783083cfafcc42493dd4a981d41669da64b4572a2a089b51b1d"
+checksum = "40a4130519a360279579c2053038317e40eff64d13fd3f004f9e1b72b8a6aaf9"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
@@ -1208,140 +1170,126 @@
 [[package]]
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
+name = "palette"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2e2f34147767aa758aa649415b50a69eeb46a67f9dc7db8011eeb3d84b351dc"
+dependencies = [
+ "approx",
+ "fast-srgb8",
+ "libm",
+ "palette_derive",
+]
+
+[[package]]
+name = "palette_derive"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b7db010ec5ff3d4385e4f133916faacd9dad0f6a09394c92d825b3aed310fa0a"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.39",
+]
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.3.5",
+ "redox_syscall 0.4.1",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pathdiff"
-version = "0.1.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3bf70094d203e07844da868b634207e71bfab254fe713171fae9a6e751ccf31"
+checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
 name = "pdf-writer"
-version = "0.8.1"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d77bc47c8968aa63f86a7e6693e270a6cbd1e3b784c364f1711a0ddecc71447"
+checksum = "644b654f2de28457bf1e25a4905a76a563d1128a33ce60cf042f721f6818feaf"
 dependencies = [
  "bitflags 1.3.2",
  "itoa",
+ "memchr",
  "ryu",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
-name = "phf"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
-dependencies = [
- "phf_shared",
-]
-
-[[package]]
-name = "phf_shared"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90fcb95eef784c2ac79119d1dd819e162b5da872ce6f3c3abe1e8ca1c082f72b"
-dependencies = [
- "siphasher 0.3.11",
-]
-
-[[package]]
 name = "pico-args"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5be167a7af36ee22fe3115051bc51f6e6c7054c9348e28deb4f49bd6f705a315"
 
 [[package]]
-name = "pin-project"
-version = "1.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fda4ed1c6c173e3fc7a83629421152e01d7b1f9b7f65fb301e490e8cfc656422"
-dependencies = [
- "pin-project-internal",
-]
-
-[[package]]
-name = "pin-project-internal"
-version = "1.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4359fd9c9171ec6e8c62926d6faaf553a8dc3f64e1507e76da7911b4f6a04405"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.33",
-]
-
-[[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pixglyph"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f67591f21f6668e63c1cd85adab066ac8a92bc7b962668dd8042197a6e4b8f8f"
 dependencies = [
- "ttf-parser 0.19.2",
+ "ttf-parser",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plist"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdc0001cfea3db57a2e24bc0d818e9e20e554b5f97fabb9bc231dc240269ae06"
+checksum = "e5699cc8a63d1aa2b1ee8e12b9ad70ac790d65788cd36101fa37f87ea46c4cef"
 dependencies = [
  "base64",
- "indexmap 1.9.3",
+ "indexmap",
  "line-wrap",
- "quick-xml",
+ "quick-xml 0.31.0",
  "serde",
  "time",
 ]
 
 [[package]]
 name = "png"
 version = "0.17.10"
@@ -1353,134 +1301,169 @@
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "postcard"
-version = "1.0.7"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d534c6e61df1c7166e636ca612d9820d486fe96ddad37f7abc671517b297488e"
+checksum = "a55c51ee6c0db07e68448e336cf8ea4131a620edefebf9893e759b2d793420f8"
 dependencies = [
  "cobs",
+ "embedded-io",
  "serde",
 ]
 
 [[package]]
+name = "powerfmt"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.67"
+version = "1.0.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d433d9f1a3e8c1263d9456598b16fec66f4acc9a74dacffd35c7bb09b3a1328"
+checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
+name = "ptr_meta"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0738ccf7ea06b608c10564b31debd4f5bc5e197fc8bfe088f68ae5ce81e7a4f1"
+dependencies = [
+ "ptr_meta_derive",
+]
+
+[[package]]
+name = "ptr_meta_derive"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "16b845dbfca988fa33db069c0e230574d15a3088f147a87b64c7589eb662c9ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "dac53072f717aa1bfa4db832b39de8c875b7c7af4f4a6fe93cdbf9264cf8383b"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "7774b5a8282bd4f25f803b1f0d945120be959a36c72e08e7cd031c792fdfd424"
 dependencies = [
+ "heck",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.39",
 ]
 
 [[package]]
-name = "qoi"
-version = "0.4.1"
+name = "quick-xml"
+version = "0.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
+checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
 dependencies = [
- "bytemuck",
+ "memchr",
+ "serde",
 ]
 
 [[package]]
 name = "quick-xml"
-version = "0.29.0"
+version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81b9228215d82c7b61490fec1de287136b5de6f5700f6e58ea9ad61a7964ca51"
+checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "rand_core",
 ]
@@ -1498,213 +1481,223 @@
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 
 [[package]]
-name = "rayon"
-version = "1.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
-dependencies = [
- "either",
- "rayon-core",
-]
-
-[[package]]
-name = "rayon-core"
-version = "1.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
-dependencies = [
- "crossbeam-channel",
- "crossbeam-deque",
- "crossbeam-utils",
- "num_cpus",
-]
-
-[[package]]
 name = "rctree"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b42e27ef78c35d3998403c1d26f3efd9e135d3e5121b0a4845cc5cc27547f4f"
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
 dependencies = [
  "getrandom",
- "redox_syscall 0.2.16",
+ "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.5"
+version = "1.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "697061221ea1b4a94a624f67d0ae2bfe4e22b8a17b6a192afb11046542cc8c47"
+checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
- "regex-syntax",
+ "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.8"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2f401f4955220693b56f8ec66ee9c78abffd8d1c4f23dc41a23839eb88f0795"
+checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.8.2",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
 
 [[package]]
+name = "regex-syntax"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+
+[[package]]
+name = "rend"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2571463863a6bd50c32f94402933f03457a3fbaf697a707c5be741e459f08fd"
+dependencies = [
+ "bytecheck",
+]
+
+[[package]]
 name = "resvg"
-version = "0.35.0"
+version = "0.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6554f47c38eca56827eea7f285c2a3018b4e12e0e195cc105833c008be338f1"
+checksum = "cc7980f653f9a7db31acff916a262c3b78c562919263edea29bf41a056e20497"
 dependencies = [
  "gif",
  "jpeg-decoder",
  "log",
  "pico-args",
  "png",
  "rgb",
  "svgtypes",
  "tiny-skia",
  "usvg",
 ]
 
 [[package]]
 name = "rgb"
-version = "0.8.36"
+version = "0.8.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20ec2d3e3fc7a92ced357df9cebd5a10b6fb2aa1ee797bf7e9ce2f17dffc8f59"
+checksum = "05aaa8004b64fd573fc9d002f4e632d51ad4f026c2b5ba95fcb6c2f32c2c47d8"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "ring"
-version = "0.16.20"
+version = "0.17.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
+checksum = "fb0205304757e5d899b9c2e448b867ffd03ae7f988002e47cd24954391394d0b"
 dependencies = [
  "cc",
+ "getrandom",
  "libc",
- "once_cell",
- "spin 0.5.2",
+ "spin",
  "untrusted",
- "web-sys",
- "winapi",
+ "windows-sys",
+]
+
+[[package]]
+name = "rkyv"
+version = "0.7.42"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0200c8230b013893c0b2d6213d6ec64ed2b9be2e0e016682b7224ff82cff5c58"
+dependencies = [
+ "bitvec",
+ "bytecheck",
+ "hashbrown 0.12.3",
+ "ptr_meta",
+ "rend",
+ "rkyv_derive",
+ "seahash",
+ "tinyvec",
+ "uuid",
+]
+
+[[package]]
+name = "rkyv_derive"
+version = "0.7.42"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2e06b915b5c230a17d7a736d1e2e63ee753c256a8614ef3f5147b13a4f5541d"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "roxmltree"
-version = "0.18.0"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8f595a457b6b8c6cda66a48503e92ee8d19342f905948f29c383200ec9eb1d8"
+checksum = "862340e351ce1b271a378ec53f304a5558f7db87f3769dc655a8f6ecbb68b302"
 dependencies = [
  "xmlparser",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.13"
+version = "0.38.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7db8590df6dfcd144d22afd1b83b36c21a18d7cbc1dc4bb5295a8712e9eb662"
+checksum = "9ad981d6c340a49cdc40a1028d9c6084ec7e9fa33fcb839cab656a267071e234"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags 2.4.1",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.7"
+version = "0.21.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd8d6c9f025a446bc4d18ad9632e69aec8f287aa84499ee335599fabd20c3fd8"
+checksum = "629648aced5775d558af50b2b4c7b02983a04b312126d45eeead26e7caa498b9"
 dependencies = [
  "log",
  "ring",
- "rustls-webpki 0.101.5",
+ "rustls-webpki",
  "sct",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.100.3"
+version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f6a5fc258f1c1276dfe3016516945546e2d5383911efc0fc4f1cdc5df3a4ae3"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
-name = "rustls-webpki"
-version = "0.101.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45a27e3b59326c16e23d30aeb7a36a24cc0d29e71d68ff611cdfb4a01d013bed"
+checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "rustybuzz"
-version = "0.7.0"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "162bdf42e261bee271b3957691018634488084ef577dddeb6420a9684cab2a6a"
+checksum = "71cd15fef9112a1f94ac64b58d1e4628192631ad6af4dc69997f995459c874e7"
 dependencies = [
  "bitflags 1.3.2",
  "bytemuck",
  "smallvec",
- "ttf-parser 0.18.1",
+ "ttf-parser",
  "unicode-bidi-mirroring",
  "unicode-ccc",
- "unicode-general-category",
+ "unicode-properties",
  "unicode-script",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1738,23 +1731,29 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "sct"
-version = "0.7.0"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
+checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
+name = "seahash"
+version = "4.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
+
+[[package]]
 name = "security-framework"
 version = "2.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
@@ -1771,72 +1770,78 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.192"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "bca2a08484b285dcb282d0f67b26cadc0df8b19f8c12502c13d966bf9482f001"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.192"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "d6c7207fbec9faa48073f3e3074cbe553af6ea512d7c21ba46e434e70ea9fbc1"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.107"
+version = "1.0.108"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b420ce6e3d8bd882e9b243c6eed35dbc9a6110c9769e74b584e0d68d1f20c65"
+checksum = "3d1c7e3eac408d115102c4c24ad393e0821bb3a5df4d506a80f85f7a742a526b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96426c9936fd7a0124915f9185ea1d20aa9445cc9821142f0a73bc9207a2e186"
+checksum = "12022b835073e5b11e90a14f86838ceb1c8fb0325b72416845c487ac0fa95e80"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.25"
+version = "0.9.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a49e178e4452f45cb61d0cd8cebc1b0fafd3e41929e996cef79aa3aca91f574"
+checksum = "3cc7a1570e38322cfe4154732e5110f887ea57e22b76f4bfd32b5bdd3368666c"
 dependencies = [
- "indexmap 2.0.0",
+ "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "simd-adler32"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d66dc143e6b11c1eddc06d5c423cfc97062865baf299914ab64caa38182078fe"
 
 [[package]]
+name = "simdutf8"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
+
+[[package]]
 name = "simplecss"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a11be7c62927d9427e9f40f3444d5499d868648e2edbc4e2116de69e7ec0e89d"
 dependencies = [
  "log",
 ]
@@ -1860,43 +1865,34 @@
 checksum = "e1e08e261d0e8f5c43123b7adf3e4ca1690d655377ac93a03b2c9d3e98de1342"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.0"
+version = "1.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
+checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
 
 [[package]]
 name = "socks"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0c3dbbd9ae980613c6dd8e28a9407b50509d3803b57624d5dfe8315218cd58b"
 dependencies = [
  "byteorder",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "spin"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
-
-[[package]]
-name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
-dependencies = [
- "lock_api",
-]
 
 [[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
@@ -1948,29 +1944,29 @@
 name = "subsetter"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09eab8a83bff89ba2200bd4c59be45c7c787f988431b936099a5a266c957f2f9"
 
 [[package]]
 name = "svg2pdf"
-version = "0.7.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c267ce43e1b46631a121481ae2d7dc00dda163d486f0f600be772bbe24d6037"
+checksum = "363c5346967da04bf3ebb3d8bafa7f52c53c810167047904df1960eac3fc08b7"
 dependencies = [
  "image",
  "miniz_oxide",
  "pdf-writer",
  "usvg",
 ]
 
 [[package]]
 name = "svgtypes"
-version = "0.11.0"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed4b0611e7f3277f68c0fa18e385d9e2d26923691379690039548f867cef02a7"
+checksum = "d71499ff2d42f59d26edb21369a308ede691421f79ebc0f001e2b1fd3a7c9e52"
 dependencies = [
  "kurbo",
  "siphasher 0.3.11",
 ]
 
 [[package]]
 name = "syn"
@@ -1981,32 +1977,32 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.33"
+version = "2.0.39"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9caece70c63bfba29ec2fed841a09851b14a235c60010fa4de58089b6c025668"
+checksum = "23e78b90f2fcf45d3e842032ce32e3f2d1545ba6636271dcbf24fa306d87be7a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "synstructure"
-version = "0.12.6"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
+checksum = "285ba80e733fac80aa4270fbcdf83772a79b80aa35c97075320abfee4a915b06"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.39",
  "unicode-xid",
 ]
 
 [[package]]
 name = "syntect"
 version = "5.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2015,151 +2011,147 @@
  "bincode",
  "bitflags 1.3.2",
  "fancy-regex",
  "flate2",
  "fnv",
  "once_cell",
  "plist",
- "regex-syntax",
+ "regex-syntax 0.7.5",
  "serde",
  "serde_json",
  "thiserror",
  "walkdir",
  "yaml-rust",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "tar"
 version = "0.4.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b16afcea1f22891c49a00c751c7b63b2233284064f11a200fc624137c51e2ddb"
 dependencies = [
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.11"
+version = "0.12.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
 
 [[package]]
 name = "tempfile"
-version = "3.8.0"
+version = "3.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb94d2f3cc536af71caac6b6fcebf65860b347e7ce0cc9ebe8f70d3e521054ef"
+checksum = "7ef1adac450ad7f4b3c28589471ade84f25f731a7a0fe30d71dfa9f60fd808e5"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall 0.3.5",
+ "redox_syscall 0.4.1",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "ff1bc3d3f05aff0403e8ac0d92ced918ec05b666a43f83297ccef5bea8a3d449"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.48"
+version = "1.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d6d7a740b8a666a7e828dd00da9c0dc290dff53154ea77ac109281de90589b7"
+checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.48"
+version = "1.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49922ecae66cc8a249b77e68d1d0623c1b2c514f0060c27cdc68bd62a1219d35"
+checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.33",
-]
-
-[[package]]
-name = "tiff"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d172b0f4d3fba17ba89811858b9d3d97f928aece846475bbda076ca46736211"
-dependencies = [
- "flate2",
- "jpeg-decoder",
- "weezl",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6bb557fd245c28e6411aa56b6403c689ad95061f50e4be16c274e70a17e48"
+checksum = "c4a34ab300f2dee6e562c10a046fc05e358b29f9bf92277f30c3c8d82275f6f5"
 dependencies = [
  "deranged",
  "itoa",
+ "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a942f44339478ef67935ab2bbaec2fb0322496cf3cbe84b261e06ac3814c572"
+checksum = "4ad70d68dba9e1f8aceda7aa6711965dfec1cac869f311a51bd08b3a2ccbce20"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tiny-skia"
-version = "0.10.0"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7db11798945fa5c3e5490c794ccca7c6de86d3afdd54b4eb324109939c6f37bc"
+checksum = "3b72a92a05db376db09fe6d50b7948d106011761c05a6a45e23e17ee9b556222"
 dependencies = [
  "arrayref",
  "arrayvec",
  "bytemuck",
  "cfg-if",
  "log",
  "png",
  "tiny-skia-path",
 ]
 
 [[package]]
 name = "tiny-skia-path"
-version = "0.10.0"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f60aa35c89ac2687ace1a2556eaaea68e8c0d47408a2e3e7f5c98a489e7281c"
+checksum = "6ac3865b9708fc7e1961a65c3a4fa55e984272f33092d3c859929f887fceb647"
 dependencies = [
  "arrayref",
  "bytemuck",
  "strict-num",
 ]
 
 [[package]]
 name = "tinystr"
-version = "0.7.1"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ac3f5b6856e931e15e07b478e98c8045239829a65f9156d4fa7e7788197a5ef"
+checksum = "83c02bf3c538ab32ba913408224323915f4ef9a6d61c0e85d493f355921c0ece"
 dependencies = [
  "displaydoc",
  "serde",
  "zerovec",
 ]
 
 [[package]]
@@ -2175,115 +2167,108 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
-version = "0.8.0"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c226a7bba6d859b63c92c4b4fe69c5b6b72d0cb897dbc8e6012298e6154cb56e"
+checksum = "a1a195ec8c9da26928f773888e0742ca3ca1040c6cd859c919c9f59c1954ab35"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.3"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cda73e2f1397b1262d6dfdcef8aafae14d1de7748d66822d3bfeeb6d03e5e4b"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ff63e60a958cefbb518ae1fd6566af80d9d4be430a33f3723dfc47d1d411d95"
+checksum = "d34d383cd00a163b4a5b85053df514d45bc330f6de7737edfe0a93311d1eaa03"
 dependencies = [
- "indexmap 2.0.0",
+ "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.26"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "ttf-parser"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0609f771ad9c6155384897e1df4d948e692667cc0588548b68eb44d052b27633"
-
-[[package]]
-name = "ttf-parser"
 version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49d64318d8311fc2668e48b63969f4343e0a85c4a109aa8460d6672e364b8bd1"
 
 [[package]]
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typst"
-version = "0.8.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.8.0#360cc9b9570f263d52530b98d0c93523e7bdb100"
+version = "0.9.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.9.0#7bb4f6df44086b4c1120b227f7ae963e6c2ad5ab"
 dependencies = [
  "base64",
- "bitflags 2.4.0",
+ "bitflags 2.4.1",
  "bytemuck",
  "comemo",
  "ecow",
  "flate2",
  "fontdb",
- "if_chain",
  "image",
- "indexmap 2.0.0",
+ "indexmap",
+ "kurbo",
  "log",
  "miniz_oxide",
- "oklab",
  "once_cell",
+ "palette",
  "pdf-writer",
  "pixglyph",
  "regex",
  "resvg",
  "roxmltree",
  "rustybuzz",
  "serde",
@@ -2291,15 +2276,15 @@
  "stacker",
  "subsetter",
  "svg2pdf",
  "time",
  "tiny-skia",
  "toml",
  "tracing",
- "ttf-parser 0.19.2",
+ "ttf-parser",
  "typst-macros",
  "typst-syntax",
  "unicode-ident",
  "unicode-math-class",
  "unicode-properties",
  "unicode-segmentation",
  "unscanny",
@@ -2308,91 +2293,93 @@
  "xmlparser",
  "xmlwriter",
  "xmp-writer",
 ]
 
 [[package]]
 name = "typst-library"
-version = "0.8.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.8.0#360cc9b9570f263d52530b98d0c93523e7bdb100"
+version = "0.9.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.9.0#7bb4f6df44086b4c1120b227f7ae963e6c2ad5ab"
 dependencies = [
  "az",
  "chinese-number",
  "ciborium",
  "comemo",
  "csv",
  "ecow",
  "hayagriva",
  "hypher",
  "icu_properties",
  "icu_provider",
  "icu_provider_adapters",
  "icu_provider_blob",
  "icu_segmenter",
+ "indexmap",
  "kurbo",
  "lipsum",
  "log",
  "once_cell",
  "roxmltree",
  "rustybuzz",
  "serde_json",
  "serde_yaml",
  "smallvec",
  "syntect",
  "time",
  "toml",
  "tracing",
- "ttf-parser 0.19.2",
+ "ttf-parser",
  "typed-arena",
  "typst",
  "unicode-bidi",
  "unicode-math-class",
  "unicode-script",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "typst-macros"
-version = "0.8.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.8.0#360cc9b9570f263d52530b98d0c93523e7bdb100"
+version = "0.9.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.9.0#7bb4f6df44086b4c1120b227f7ae963e6c2ad5ab"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
 ]
 
 [[package]]
 name = "typst-py"
-version = "0.8.0"
+version = "0.9.0"
 dependencies = [
  "chrono",
  "codespan-reporting",
  "comemo",
  "dirs",
  "ecow",
  "env_proxy",
+ "filetime",
  "flate2",
- "memmap2",
+ "fontdb",
  "openssl",
  "pathdiff",
  "pyo3",
  "same-file",
  "siphasher 1.0.0",
  "tar",
  "typst",
  "typst-library",
  "ureq",
  "walkdir",
 ]
 
 [[package]]
 name = "typst-syntax"
-version = "0.8.0"
-source = "git+https://github.com/typst/typst.git?tag=v0.8.0#360cc9b9570f263d52530b98d0c93523e7bdb100"
+version = "0.9.0"
+source = "git+https://github.com/typst/typst.git?tag=v0.9.0#7bb4f6df44086b4c1120b227f7ae963e6c2ad5ab"
 dependencies = [
  "comemo",
  "ecow",
  "once_cell",
  "serde",
  "tracing",
  "unicode-ident",
@@ -2412,14 +2399,15 @@
 
 [[package]]
 name = "unic-langid-impl"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e35bfd2f2b8796545b55d7d3fd3e89a0613f68a0d1c8bc28cb7ff96b411a35ff"
 dependencies = [
+ "serde",
  "tinystr",
 ]
 
 [[package]]
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2434,20 +2422,14 @@
 [[package]]
 name = "unicode-ccc"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc2520efa644f8268dce4dcd3050eaa7fc044fca03961e9998ac7e2e92b77cf1"
 
 [[package]]
-name = "unicode-general-category"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2281c8c1d221438e373249e065ca4989c4c36952c211ff21a0ee91c44a3869e7"
-
-[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-math-class"
@@ -2486,29 +2468,29 @@
 name = "unicode-vo"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1d386ff53b415b7fe27b50bb44679e2cc4660272694b7b6f3326d8480823a94"
 
 [[package]]
 name = "unicode-width"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "unsafe-libyaml"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28467d3e1d3c6586d8f25fa243f544f5800fec42d97032474e17222c2b75cfa"
 
@@ -2516,67 +2498,68 @@
 name = "unscanny"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9df2af067a7953e9c3831320f35c1cc0600c30d44d9f7a12b01db1cd88d6b47"
 
 [[package]]
 name = "untrusted"
-version = "0.7.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
+checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.7.1"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b11c96ac7ee530603dcdf68ed1557050f374ce55a5a07193ebf8cbc9f8927e9"
+checksum = "f5ccd538d4a604753ebc2f17cd9946e89b77bf87f6a8e2309667c6f2e87855e3"
 dependencies = [
  "base64",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
- "rustls-webpki 0.100.3",
+ "rustls-webpki",
  "socks",
  "url",
  "webpki-roots",
 ]
 
 [[package]]
 name = "url"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "143b538f18257fac9cad154828a57c6bf5157e1aa604d4816b5995bf6de87ae5"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
+ "serde",
 ]
 
 [[package]]
 name = "usvg"
-version = "0.35.0"
+version = "0.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d09ddfb0d93bf84824c09336d32e42f80961a9d1680832eb24fdf249ce11e6"
+checksum = "c51daa774fe9ee5efcf7b4fec13019b8119cda764d9a8b5b06df02bb1445c656"
 dependencies = [
  "base64",
  "log",
  "pico-args",
  "usvg-parser",
  "usvg-text-layout",
  "usvg-tree",
  "xmlwriter",
 ]
 
 [[package]]
 name = "usvg-parser"
-version = "0.35.0"
+version = "0.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d19bf93d230813599927d88557014e0908ecc3531666d47c634c6838bc8db408"
+checksum = "45c88a5ffaa338f0e978ecf3d4e00d8f9f493e29bed0752e1a808a1db16afc40"
 dependencies = [
  "data-url",
  "flate2",
  "imagesize",
  "kurbo",
  "log",
  "roxmltree",
@@ -2584,47 +2567,53 @@
  "siphasher 0.3.11",
  "svgtypes",
  "usvg-tree",
 ]
 
 [[package]]
 name = "usvg-text-layout"
-version = "0.35.0"
+version = "0.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "035044604e89652c0a2959b8b356946997a52649ba6cade45928c2842376feb4"
+checksum = "4d2374378cb7a3fb8f33894e0fdb8625e1bbc4f25312db8d91f862130b541593"
 dependencies = [
  "fontdb",
  "kurbo",
  "log",
  "rustybuzz",
  "unicode-bidi",
  "unicode-script",
  "unicode-vo",
  "usvg-tree",
 ]
 
 [[package]]
 name = "usvg-tree"
-version = "0.35.0"
+version = "0.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7939a7e4ed21cadb5d311d6339730681c3e24c3e81d60065be80e485d3fc8b92"
+checksum = "6cacb0c5edeaf3e80e5afcf5b0d4004cc1d36318befc9a7c6606507e5d0f4062"
 dependencies = [
  "rctree",
  "strict-num",
  "svgtypes",
  "tiny-skia-path",
 ]
 
 [[package]]
 name = "utf8_iter"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64a8922555b9500e3d865caed19330172cd67cbf82203f1a3311d8c305cc9f33"
 
 [[package]]
+name = "uuid"
+version = "1.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ad59a7560b41a70d191093a945f0b87bc1deeda46fb237479708a1d6b6cdfc"
+
+[[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "version_check"
@@ -2646,74 +2635,74 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "7daec296f25a1bae309c0cd5c29c4b260e510e6d813c286b19eaadf409d40fce"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "e397f4664c0e4e428e8313a469aaa58310d302159845980fd23b0f22a847f217"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "5961017b3b08ad5f3fe39f1e79877f8ee7c23c5e5fd5eb80de95abc41f1f16b2"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "c5353b8dab669f5e10f5bd76df26a9360c748f054f862ff5f3f8aae0c7fb3907"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.33",
+ "syn 2.0.39",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "0d046c5d029ba91a1ed14da14dca44b68bf2f124cfbaf741c54151fdb3e0750b"
 
 [[package]]
 name = "wasmi"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f341edb80021141d4ae6468cbeefc50798716a347d4085c3811900049ea8945"
 dependencies = [
  "smallvec",
- "spin 0.9.8",
+ "spin",
  "wasmi_arena",
  "wasmi_core",
  "wasmparser-nostd",
 ]
 
 [[package]]
 name = "wasmi_arena"
@@ -2739,31 +2728,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9157cab83003221bfd385833ab587a039f5d6fa7304854042ba358a3b09e0724"
 dependencies = [
  "indexmap-nostd",
 ]
 
 [[package]]
-name = "web-sys"
-version = "0.3.64"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
-dependencies = [
- "js-sys",
- "wasm-bindgen",
-]
-
-[[package]]
 name = "webpki-roots"
-version = "0.23.1"
+version = "0.25.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b03058f88386e5ff5310d9111d53f48b17d732b401aeb83a8d5190f2ac459338"
-dependencies = [
- "rustls-webpki 0.100.3",
-]
+checksum = "14247bb57be4f377dfb94c72830b8ce8fc6beac03cf4bf7b9732eadd414123fc"
 
 [[package]]
 name = "weezl"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
 
@@ -2781,32 +2757,32 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows"
-version = "0.48.0"
+name = "windows-core"
+version = "0.51.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+checksum = "f1f8cf84f35d2db49a46868f947758c7a1138116f7fac3bc844f43ade1292e64"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
@@ -2871,133 +2847,144 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "winnow"
-version = "0.5.15"
+version = "0.5.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c2e3184b9c4e92ad5167ca73039d0c42476302ab603e2fec4487511f38ccefc"
+checksum = "829846f3e3db426d4cee4510841b71a8e58aa2a76b1132579487ae430ccd9c7b"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "writeable"
-version = "0.5.2"
+version = "0.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dad7bb64b8ef9c0aa27b6da38b452b0ee9fd82beaf276a87dd796fb55cbae14e"
+
+[[package]]
+name = "wyz"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60e49e42bdb1d5dc76f4cd78102f8f0714d32edfa3efb82286eb0f0b1fc0da0f"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
 
 [[package]]
 name = "xattr"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4686009f71ff3e5c4dbcf1a282d0a44db3f021ba69350cd42086b3e5f1c6985"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "xmlparser"
-version = "0.13.5"
+version = "0.13.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d25c75bf9ea12c4040a97f829154768bbbce366287e2dc044af160cd79a13fd"
+checksum = "66fee0b777b0f5ac1c69bb06d361268faafa61cd4682ae064a171c16c433e9e4"
 
 [[package]]
 name = "xmlwriter"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec7a2a501ed189703dba8b08142f057e887dfc4b2cc4db2d343ac6376ba3e0b9"
 
 [[package]]
 name = "xmp-writer"
-version = "0.1.0"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9fd742bbbb930fc972b28bf66b7546dfbc7bb9a4c7924299df0ae6a5641fcadf"
+checksum = "4543ba138f64a94b19e1e9c66c165bca7e03d470e1c066cb76ea279d9d0e1989"
 
 [[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
 
 [[package]]
 name = "yoke"
-version = "0.7.1"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1848075a23a28f9773498ee9a0f2cf58fcbad4f8c0ccf84a210ab33c6ae495de"
+checksum = "65e71b2e4f287f467794c671e2b8f8a5f3716b3c829079a1c44740148eff07e4"
 dependencies = [
  "serde",
  "stable_deref_trait",
  "yoke-derive",
  "zerofrom",
 ]
 
 [[package]]
 name = "yoke-derive"
-version = "0.7.1"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af46c169923ed7516eef0aa32b56d2651b229f57458ebe46b49ddd6efef5b7a2"
+checksum = "9e6936f0cce458098a201c245a11bef556c6a0181129c7034d10d76d1ec3a2b8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.39",
  "synstructure",
 ]
 
 [[package]]
 name = "zerofrom"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df54d76c3251de27615dfcce21e636c172dafb2549cd7fd93e21c66f6ca6bea2"
+checksum = "655b0814c5c0b19ade497851070c640773304939a6c0fd5f5fb43da0696d05b7"
 dependencies = [
  "zerofrom-derive",
 ]
 
 [[package]]
 name = "zerofrom-derive"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4eae7c1f7d4b8eafce526bc0771449ddc2f250881ae31c50d22c032b5a1c499"
+checksum = "e6a647510471d372f2e6c2e6b7219e44d8c574d24fdc11c610a61455782f18c3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.39",
  "synstructure",
 ]
 
 [[package]]
+name = "zerotrie"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d0594125a0574fb93059c92c588ab209cc036a23d1baeb3410fa9181bea551a0"
+dependencies = [
+ "displaydoc",
+ "litemap",
+ "serde",
+ "zerovec",
+]
+
+[[package]]
 name = "zerovec"
-version = "0.9.4"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "198f54134cd865f437820aa3b43d0ad518af4e68ee161b444cdd15d8e567c8ea"
+checksum = "eff4439ae91fb5c72b8abc12f3f2dbf51bd27e6eadb9f8a5bc8898dddb0e27ea"
 dependencies = [
  "serde",
  "yoke",
  "zerofrom",
  "zerovec-derive",
 ]
 
 [[package]]
 name = "zerovec-derive"
-version = "0.9.4"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "486558732d5dde10d0f8cb2936507c1bb21bc539d924c949baf5f36a58e51bac"
+checksum = "7b4e5997cbf58990550ef1f0e5124a05e47e1ebd33a84af25739be6031a62c20"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
- "synstructure",
-]
-
-[[package]]
-name = "zune-inflate"
-version = "0.2.54"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73ab332fe2f6680068f3582b16a24f90ad7096d5d39b974d1c0aff0125116f02"
-dependencies = [
- "simd-adler32",
+ "syn 2.0.39",
 ]
```

### Comparing `typst-0.8.0/PKG-INFO` & `typst-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: typst
-Version: 0.8.0
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: importlib-resources ; python_version < '3.9'
 License-File: LICENSE
 Summary: Python binding to typst
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/messense/typst-py
```

