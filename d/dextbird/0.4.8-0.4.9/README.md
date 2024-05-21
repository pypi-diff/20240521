# Comparing `tmp/dextbird-0.4.8.tar.gz` & `tmp/dextbird-0.4.9.tar.gz`

## Comparing `dextbird-0.4.8.tar` & `dextbird-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 dextbird-0.4.8/Cargo.toml
--rw-r--r--   0     1001      127      387 2024-04-04 18:18:24.000000 dextbird-0.4.8/.bashrc
--rw-r--r--   0     1001      127     1367 2024-04-04 18:18:24.000000 dextbird-0.4.8/.github/workflows/docs.yml
--rw-r--r--   0     1001      127     2030 2024-04-04 18:18:24.000000 dextbird-0.4.8/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1025 2024-04-04 18:18:24.000000 dextbird-0.4.8/.github/workflows/test.yml
--rw-r--r--   0     1001      127      713 2024-04-04 18:18:24.000000 dextbird-0.4.8/.gitignore
--rw-r--r--   0     1001      127     1065 2024-04-04 18:18:24.000000 dextbird-0.4.8/LICENSE
--rw-r--r--   0     1001      127     1392 2024-04-04 18:18:24.000000 dextbird-0.4.8/README.md
--rw-r--r--   0     1001      127       67 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/__init__.py
--rw-r--r--   0     1001      127     1314 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/core.pyi
--rw-r--r--   0     1001      127      759 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/plug.py
--rw-r--r--   0     1001      127     2633 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/voice_client.py
--rw-r--r--   0     1001      127     1310 2024-04-04 18:18:24.000000 dextbird-0.4.8/examples/basic.py
--rw-r--r--   0     1001      127      107 2024-04-04 18:18:24.000000 dextbird-0.4.8/renovate.json
--rw-r--r--   0     1001      127 15660281 2024-04-04 18:18:24.000000 dextbird-0.4.8/result.txt
--rw-r--r--   0     1001      127     7151 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/core.rs
--rw-r--r--   0     1001      127      320 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/lib.rs
--rw-r--r--   0     1001      127     2376 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/track.rs
--rw-r--r--   0     1001      127     1401 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/update_voice_state.rs
--rw-r--r--   0     1001      127       49 2024-04-04 18:18:24.000000 dextbird-0.4.8/test.sh
--rw-r--r--   0     1001      127     1561 2024-04-04 18:18:24.000000 dextbird-0.4.8/tests/test_simple.py
--rw-r--r--   0     1001      127    73821 2024-04-04 18:18:28.000000 dextbird-0.4.8/Cargo.lock
--rw-r--r--   0     1001      127      814 2024-04-04 18:18:24.000000 dextbird-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 dextbird-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 dextbird-0.4.9/Cargo.toml
+-rw-r--r--   0     1001      127      387 2024-05-21 20:53:38.000000 dextbird-0.4.9/.bashrc
+-rw-r--r--   0     1001      127       66 2024-05-21 20:53:38.000000 dextbird-0.4.9/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     1308 2024-05-21 20:53:38.000000 dextbird-0.4.9/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127     2030 2024-05-21 20:53:38.000000 dextbird-0.4.9/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1025 2024-05-21 20:53:38.000000 dextbird-0.4.9/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      713 2024-05-21 20:53:38.000000 dextbird-0.4.9/.gitignore
+-rw-r--r--   0     1001      127     1065 2024-05-21 20:53:38.000000 dextbird-0.4.9/LICENSE
+-rw-r--r--   0     1001      127     1405 2024-05-21 20:53:38.000000 dextbird-0.4.9/README.md
+-rw-r--r--   0     1001      127       67 2024-05-21 20:53:38.000000 dextbird-0.4.9/dextbird/__init__.py
+-rw-r--r--   0     1001      127     1314 2024-05-21 20:53:38.000000 dextbird-0.4.9/dextbird/core.pyi
+-rw-r--r--   0     1001      127      759 2024-05-21 20:53:38.000000 dextbird-0.4.9/dextbird/plug.py
+-rw-r--r--   0     1001      127     2633 2024-05-21 20:53:38.000000 dextbird-0.4.9/dextbird/voice_client.py
+-rw-r--r--   0     1001      127     1310 2024-05-21 20:53:38.000000 dextbird-0.4.9/examples/basic.py
+-rw-r--r--   0     1001      127      107 2024-05-21 20:53:38.000000 dextbird-0.4.9/renovate.json
+-rw-r--r--   0     1001      127     7151 2024-05-21 20:53:38.000000 dextbird-0.4.9/src/core.rs
+-rw-r--r--   0     1001      127      320 2024-05-21 20:53:38.000000 dextbird-0.4.9/src/lib.rs
+-rw-r--r--   0     1001      127     2376 2024-05-21 20:53:38.000000 dextbird-0.4.9/src/track.rs
+-rw-r--r--   0     1001      127     1401 2024-05-21 20:53:38.000000 dextbird-0.4.9/src/update_voice_state.rs
+-rw-r--r--   0     1001      127     1615 2024-05-21 20:53:38.000000 dextbird-0.4.9/tests/test_simple.py
+-rw-r--r--   0     1001      127    74040 2024-05-21 20:53:41.000000 dextbird-0.4.9/Cargo.lock
+-rw-r--r--   0     1001      127      831 2024-05-21 20:53:38.000000 dextbird-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 dextbird-0.4.9/PKG-INFO
```

### Comparing `dextbird-0.4.8/Cargo.toml` & `dextbird-0.4.9/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "dextbird"
-version = "0.4.8"
+version = "0.4.9"
 description = "Discord extensions voice library made with rust"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dextbird"
 crate-type = ["cdylib"]
 
 [dependencies]
 async-dropper = { version = "0.3.1", features = ["tokio", "simple"] }
-async-trait = "0.1.79"
+async-trait = "0.1.80"
 log = "0.4.21"
 pyo3 = "0.20.3"
 pyo3-asyncio = { version = "0.20.0", features = ["tokio-runtime"] }
 reqwest = { version = "0.11.7", default-features = false, features = ["rustls-tls"] }
 songbird = { version = "0.4.1", features = ["driver"] }
 symphonia = { version = "0.5.4", features = ["aac", "mp3", "isomp4", "alac"] }
 tokio = { version = "1.37.0", features = ["sync"] }
```

### Comparing `dextbird-0.4.8/.github/workflows/docs.yml` & `dextbird-0.4.9/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,47 +4,48 @@
   push:
     branches: ["main", "develop"]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
-      - name: Checkout
-        uses: actions/checkout@v4
-      - name: Setup Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: '3.11'
-      - uses: actions/cache@v4
-        with:
-          path: |
-            ~/.cargo/bin/
-            ~/.cargo/registry/index/
-            ~/.cargo/registry/cache/
-            ~/.cargo/git/db/
-            target/
-          key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.toml') }}
-      - name: Install rust
-        run: curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
-      - name: Install requirements
-        run: |
-          pip install maturin pdoc3 discord.py
-          maturin build -o dist && pip install dist/*.whl
-      - name: Build document
-        run: cd dist && pdoc dextbird --html -o docs
-      - name: Upload artifact
-        uses: actions/upload-pages-artifact@v3
-        with:
-          path: ./dist/docs/dextbird
+    - name: Checkout
+      uses: actions/checkout@v4
+    - name: Setup Python
+      uses: actions/setup-python@v5
+      with:
+        python-version: '3.11'
+    - uses: actions/cache@v4
+      with:
+        path: |
+          ~/.cargo/bin/
+          ~/.cargo/registry/index/
+          ~/.cargo/registry/cache/
+          ~/.cargo/git/db/
+          target/
+        key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.toml') }}
+    - name: Install rust
+      run: curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
+    - name: Install requirements
+      run: |
+        pip install maturin pdoc3 discord.py
+        maturin build -o dist && pip install dist/*.whl
+    - name: Build document
+      run: cd dist && pdoc dextbird --html -o docs
+    - name: Upload artifact
+      uses: actions/upload-pages-artifact@v3
+      with:
+        path: ./dist/docs/dextbird
+
   deploy:
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     permissions:
       pages: write
       id-token: write
     runs-on: ubuntu-latest
     needs: build
     steps:
-      - name: Deploy to GitHub Pages
-        id: deployment
-        uses: actions/deploy-pages@v4
+    - name: Deploy to GitHub Pages
+      id: deployment
+      uses: actions/deploy-pages@v4
```

### Comparing `dextbird-0.4.8/.github/workflows/release.yml` & `dextbird-0.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/.github/workflows/test.yml` & `dextbird-0.4.9/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   pull_request:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.12"]
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install rust
       run: curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
```

### Comparing `dextbird-0.4.8/.gitignore` & `dextbird-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/LICENSE` & `dextbird-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/README.md` & `dextbird-0.4.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # discord-ext-songbird
 [![Test songbird](https://github.com/tuna2134/discord-ext-songbird/actions/workflows/test.yml/badge.svg)](https://github.com/tuna2134/discord-ext-songbird/actions/workflows/test.yml)
 
-Songbird is rust voice manager.
+Songbird is voice client which made by Rust.
 
 This library is wrapping songbird for discord.py.
 
 [Document](https://tuna2134.dev/discord-ext-songbird/)
 
-## support
+## Support
 Only macos and linux.
 
 If you are using linux, we are only support this python version.
 3.8.10+, 3.9.5+, 3.10.0+
 
 ### Why I am not supporting windows?
 It's too hard for me.
```

### Comparing `dextbird-0.4.8/dextbird/core.pyi` & `dextbird-0.4.9/dextbird/core.pyi`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/dextbird/plug.py` & `dextbird-0.4.9/dextbird/plug.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/dextbird/voice_client.py` & `dextbird-0.4.9/dextbird/voice_client.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/examples/basic.py` & `dextbird-0.4.9/examples/basic.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/src/core.rs` & `dextbird-0.4.9/src/core.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/src/track.rs` & `dextbird-0.4.9/src/track.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/src/update_voice_state.rs` & `dextbird-0.4.9/src/update_voice_state.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.8/tests/test_simple.py` & `dextbird-0.4.9/tests/test_simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 import logging
 import random
 
 
 MUSICS = [
     "https://youtu.be/fE9trKOuT3Q",
     "https://youtu.be/TG2IgWOjtwU",
-    "https://youtu.be/yL1LYf-S2Q0"
+    "https://youtu.be/yL1LYf-S2Q0",
+    "https://youtu.be/foRefp4MlOI",  # Arika - blan_
 ]
 
 
 client = discord.Client(intents=discord.Intents.all())
 logger = logging.getLogger()
```

### Comparing `dextbird-0.4.8/Cargo.lock` & `dextbird-0.4.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a35cf17a37761f1c88b8e770b5956820fe84c12854165b6f930c604ea186e47e"
 dependencies = [
  "async-trait",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
  "tokio",
 ]
 
 [[package]]
 name = "async-dropper-simple"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -108,21 +108,21 @@
  "futures",
  "pin-project",
  "tokio",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.79"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "audiopus"
 version = "0.3.0-rc.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ab55eb0e56d7c6de3d59f544e5db122d7725ec33be6a276ee8241f3be6473955"
@@ -139,17 +139,17 @@
  "cmake",
  "log",
  "pkg-config",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -193,23 +193,23 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -217,34 +217,34 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
@@ -286,35 +286,35 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.12"
+version = "0.5.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
+checksum = "33480d6946193aa8033910124896ca395333cae7e2d1113d1fef6c3272217df2"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
@@ -349,17 +349,17 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.5.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+checksum = "e8566979429cf69b49a5c740c60791108e86440e8be149bbea4fe54d2c32d6e2"
 
 [[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
@@ -376,15 +376,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dextbird"
-version = "0.4.8"
+version = "0.4.9"
 dependencies = [
  "async-dropper",
  "async-trait",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
@@ -411,17 +411,17 @@
 dependencies = [
  "pnet_macros",
  "pnet_macros_support",
 ]
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
@@ -432,17 +432,17 @@
 name = "extended"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af9673d8203fcb076b19dfd17e38b3d4ae9f44959416ea532ce72415a6020365"
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
@@ -523,15 +523,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -582,17 +582,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -620,17 +620,17 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -714,15 +714,15 @@
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
  "http 0.2.12",
  "hyper",
- "rustls 0.21.10",
+ "rustls 0.21.12",
  "tokio",
  "tokio-rustls 0.24.1",
 ]
 
 [[package]]
 name = "iana-time-zone"
 version = "0.1.60"
@@ -806,23 +806,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -883,17 +883,17 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -934,17 +934,17 @@
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-conv"
 version = "0.1.0"
@@ -958,17 +958,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1019,33 +1019,33 @@
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -1063,15 +1063,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -1102,15 +1102,15 @@
 version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "688b17499eee04a0408aca0aa5cba5fc86401d7216de8a63fdf7a4c227871804"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pnet_macros_support"
 version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eea925b72f4bd37f8eab0f221bbe4c78b63498350c983ffa9dd4bcde7e030f56"
@@ -1154,17 +1154,17 @@
 checksum = "9df7f93fd637f083201473dab4fee2db4c429d32e55e3299980ab3957ab916a0"
 dependencies = [
  "num-integer",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -1221,35 +1221,35 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1287,19 +1287,19 @@
 checksum = "953d9f7e5cdd80963547b456251296efc2626ed4e3cbf36c869d9564e0220571"
 dependencies = [
  "rustfft",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -1362,15 +1362,15 @@
  "js-sys",
  "log",
  "mime",
  "mime_guess",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.10",
+ "rustls 0.21.12",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
@@ -1435,17 +1435,17 @@
  "num-integer",
  "num-traits",
  "realfft",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
@@ -1477,34 +1477,34 @@
  "ring 0.16.20",
  "sct",
  "webpki",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring 0.17.8",
  "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring 0.17.8",
  "rustls-pki-types",
- "rustls-webpki 0.102.2",
+ "rustls-webpki 0.102.4",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-native-certs"
 version = "0.6.3"
@@ -1524,44 +1524,44 @@
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
  "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring 0.17.8",
  "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "ff448f7e92e913c4b7d4c6d8e4540a1724b319b4152b8aef6d4cf8339712b33e"
 dependencies = [
  "ring 0.17.8",
  "rustls-pki-types",
  "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
 name = "rusty_pool"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ed36cdb20de66d89a17ea04b8883fc7a386f2cf877aaedca5005583ce4876ff"
 dependencies = [
@@ -1570,17 +1570,17 @@
  "futures-channel",
  "futures-executor",
  "num_cpus",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "salsa20"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97a22f5af31f73a954c10289c93e8a50cc23d971e80ee446f1f6f7137a088213"
 dependencies = [
@@ -1626,46 +1626,46 @@
 dependencies = [
  "serde",
  "zeroize",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-aux"
 version = "4.5.0"
@@ -1685,43 +1685,43 @@
 dependencies = [
  "ordered-float",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.18"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
+checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
@@ -1790,17 +1790,17 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
@@ -1814,17 +1814,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "songbird"
@@ -2100,17 +2100,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2144,47 +2144,47 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -2195,17 +2195,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
@@ -2244,15 +2244,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.23.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
@@ -2264,25 +2264,25 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.10",
+ "rustls 0.21.12",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
 dependencies = [
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-tungstenite"
 version = "0.18.0"
@@ -2303,34 +2303,33 @@
 name = "tokio-tungstenite"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c83b561d025642014097b66e6c1bb422783339e0909e4429cde4749d1990bc38"
 dependencies = [
  "futures-util",
  "log",
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pki-types",
  "tokio",
  "tokio-rustls 0.25.0",
  "tungstenite 0.21.0",
  "webpki-roots 0.26.1",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
@@ -2351,15 +2350,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -2453,15 +2452,15 @@
  "byteorder",
  "bytes",
  "data-encoding",
  "http 1.1.0",
  "httparse",
  "log",
  "rand",
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pki-types",
  "sha1",
  "thiserror",
  "url",
  "utf-8",
 ]
 
@@ -2649,15 +2648,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2683,15 +2682,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.65",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2779,15 +2778,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -2797,15 +2796,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2817,110 +2816,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
```

### Comparing `dextbird-0.4.8/pyproject.toml` & `dextbird-0.4.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 name = "dextbird"
 version = "v0.1.0"
 description = "dextbird poetry description"
 authors = ["tuna2134"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-yt-dlp = "^2024.3.10"
+yt-dlp = "^2024.4.9"
+pytest = "^8.2.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.0.0"
-pytest-asyncio = "^0.23.0"
-python-dotenv = "^1.0.0"
+pytest = "^8.2.1"
+pytest-asyncio = "^0.23.7"
+python-dotenv = "^1.0.1"
 discord-py = "^2.3.2"
-maturin = {extras = ["patchelf"], version = "^1.2.3"}
-black = "^24.0.0"
-pyright = "^1.1.326"
+maturin = {extras = ["patchelf"], version = "^1.5.1"}
+black = "^24.4.2"
+pyright = "^1.1.363"
 pdoc3 = "^0.10.0"
 jishaku = "^2.5.2"
 
 [build-system]
 requires = ["maturin>=1.2,<2.0"]
 build-backend = "maturin"
```

### Comparing `dextbird-0.4.8/PKG-INFO` & `dextbird-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.3
 Name: dextbird
-Version: 0.4.8
+Version: 0.4.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Discord extensions voice library made with rust
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # discord-ext-songbird
 [![Test songbird](https://github.com/tuna2134/discord-ext-songbird/actions/workflows/test.yml/badge.svg)](https://github.com/tuna2134/discord-ext-songbird/actions/workflows/test.yml)
 
-Songbird is rust voice manager.
+Songbird is voice client which made by Rust.
 
 This library is wrapping songbird for discord.py.
 
 [Document](https://tuna2134.dev/discord-ext-songbird/)
 
-## support
+## Support
 Only macos and linux.
 
 If you are using linux, we are only support this python version.
 3.8.10+, 3.9.5+, 3.10.0+
 
 ### Why I am not supporting windows?
 It's too hard for me.
```

