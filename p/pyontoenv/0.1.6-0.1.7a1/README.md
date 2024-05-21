# Comparing `tmp/pyontoenv-0.1.6.tar.gz` & `tmp/pyontoenv-0.1.7a1.tar.gz`

## Comparing `pyontoenv-0.1.6.tar` & `pyontoenv-0.1.7a1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0     1001      127      776 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/Cargo.toml
--rw-r--r--   0     1001      127     5324 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/config.rs
--rw-r--r--   0     1001      127     2180 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/consts.rs
--rw-r--r--   0     1001      127     3267 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/doctor.rs
--rw-r--r--   0     1001      127      350 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/errors.rs
--rw-r--r--   0     1001      127    38576 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/lib.rs
--rw-r--r--   0     1001      127    13633 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/ontology.rs
--rw-r--r--   0     1001      127     3521 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/policy.rs
--rw-r--r--   0     1001      127     4646 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/transform.rs
--rw-r--r--   0     1001      127     6428 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/src/util.rs
--rw-r--r--   0     1001      127  1689944 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model
--rw-r--r--   0     1001      127      321 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.n3
--rw-r--r--   0     1001      127      537 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.nt
--rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.ttl
--rw-r--r--   0     1001      127      789 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/model.xml
--rw-r--r--   0     1001      127      909 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   146214 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0     1001      127    30521 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   163975 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0     1001      127  1323794 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127    17472 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127  1456008 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127   104496 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0     1001      127  1255550 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0     1001      127    44502 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0     1001      127    81761 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/rec.ttl
--rw-r--r--   0     1001      127     4069 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/recimports.ttl
--rw-r--r--   0     1001      127    11876 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0     1001      127     1160 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/data2/ont4.ttl
--rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model
--rw-r--r--   0     1001      127      321 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.n3
--rw-r--r--   0     1001      127      537 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.nt
--rw-r--r--   0     1001      127     1248 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.ttl
--rw-r--r--   0     1001      127      789 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/fileendings/model.xml
--rw-r--r--   0     1001      127  1689944 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0     1001      127     1160 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0     1001      127     1135 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0     1001      127     1129 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/python/Cargo.toml
--rw-r--r--   0     1001      127     2886 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/.gitignore
--rw-r--r--   0     1001      127      731 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/README.md
--rw-r--r--   0     1001      127       71 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/build.rs
--rw-r--r--   0     1001      127     5241 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/poetry.lock
--rw-r--r--   0     1001      127       71 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/requirements.dev.txt
--rw-r--r--   0     1001      127    14479 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/src/lib.rs
--rw-r--r--   0     1001      127      694 2024-04-29 19:45:48.000000 pyontoenv-0.1.6/python/test.py
--rw-r--r--   0     1001      127    73218 2024-04-29 19:46:26.000000 pyontoenv-0.1.6/Cargo.lock
--rw-r--r--   0        0        0     1005 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 pyontoenv-0.1.6/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/Cargo.toml
+-rw-r--r--   0     1001      127     5324 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/errors.rs
+-rw-r--r--   0     1001      127    38662 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/lib.rs
+-rw-r--r--   0     1001      127    13633 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6428 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/util.rs
+-rw-r--r--   0     1001      127  1689944 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model
+-rw-r--r--   0     1001      127      321 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.xml
+-rw-r--r--   0     1001      127      909 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    81761 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/ref-schema.ttl
+-rw-r--r--   0     1001      127     1160 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont4.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.xml
+-rw-r--r--   0     1001      127  1689944 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127     1160 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/README.md
+-rw-r--r--   0     1001      127       71 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14445 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/test.py
+-rw-r--r--   0     1001      127    73227 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/PKG-INFO
```

### Comparing `pyontoenv-0.1.6/lib/Cargo.toml` & `pyontoenv-0.1.7a1/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/config.rs` & `pyontoenv-0.1.7a1/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/consts.rs` & `pyontoenv-0.1.7a1/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/doctor.rs` & `pyontoenv-0.1.7a1/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/lib.rs` & `pyontoenv-0.1.7a1/lib/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 pub mod ontology;
 pub mod policy;
 #[macro_use]
 pub mod util;
 pub mod transform;
 
 use crate::config::Config;
-use crate::consts::{IMPORTS, ONTOLOGY, PREFIXES, TYPE};
 use crate::doctor::{Doctor, DuplicateOntology, OntologyDeclaration};
 use crate::ontology::{GraphIdentifier, Ontology, OntologyLocation};
 use anyhow::Result;
 use chrono::prelude::*;
 use log::{debug, error, info, warn};
 use oxigraph::model::{
-    Dataset, Graph, GraphName, NamedNode, NamedNodeRef, NamedOrBlankNode, Quad, QuadRef, SubjectRef,
+    Dataset, Graph, GraphName, NamedNode, NamedNodeRef, NamedOrBlankNode, QuadRef, SubjectRef,
 };
 use oxigraph::store::Store;
 use petgraph::graph::{Graph as DiGraph, NodeIndex};
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::collections::{HashSet, VecDeque};
 use std::io::{BufReader, Write};
@@ -94,14 +93,15 @@
     }
 
     // TODO: add a read-only version? make this thread-safe?
     fn store(&self) -> Result<Store> {
         let ontoenv_dir = self.config.root.join(".ontoenv");
         std::fs::create_dir_all(&ontoenv_dir)?;
         Store::open(ontoenv_dir.join("store.db"))
+            .or_else(|_| Store::open_read_only(ontoenv_dir.join("store.db")))
             .map_err(|e| anyhow::anyhow!("Could not open store: {}", e))
     }
 
     pub fn new_readonly(config: Config) -> Result<Self> {
         // create the store in the root/.ontoenv/store.db directory
         let store = Store::open_secondary(config.root.join(".ontoenv/store.db"))?;
         Ok(Self {
@@ -831,15 +831,15 @@
     // https://docs.rs/tempdir/latest/tempdir/struct.TempDir.html#method.close)
     fn teardown(_dir: TempDir) {}
 
     #[test]
     fn test_ontoenv_scans() -> Result<()> {
         let dir = setup("data2")?;
         let cfg = default_config(&dir);
-        let mut env = OntoEnv::new(cfg)?;
+        let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         teardown(dir);
         Ok(())
     }
 
     #[test]
@@ -848,15 +848,15 @@
         let cfg = Config::new_with_default_matches(
             dir.path().into(),
             Some([dir.path().into()]),
             false,
             false,
             true,
         )?;
-        let mut env = OntoEnv::new(cfg)?;
+        let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         teardown(dir);
         Ok(())
     }
 
     #[test]
@@ -868,27 +868,27 @@
             &["*.n3"],
             &[""],
             false,
             false,
             true,
             "default".to_string(),
         )?;
-        let mut env = OntoEnv::new(cfg1)?;
+        let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 1);
         assert_eq!(env.num_triples()?, 5);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_update() -> Result<()> {
         let dir = setup("data2")?;
         let cfg = default_config(&dir);
-        let mut env = OntoEnv::new(cfg)?;
+        let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         let old_num_triples = env.num_triples()?;
         assert_eq!(env.num_graphs(), 4);
 
         // updating again shouldn't add anything
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
@@ -910,15 +910,15 @@
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_retrieval_by_name() -> Result<()> {
         let dir = setup("data2")?;
         let cfg = default_config(&dir);
-        let mut env = OntoEnv::new(cfg)?;
+        let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
 
         let ont1 = NamedNodeRef::new("urn:ont1")?;
         let ont = env
             .get_ontology_by_name(ont1)
             .ok_or(anyhow::anyhow!("Ontology not found"))?;
         assert_eq!(ont.imports.len(), 2);
@@ -927,15 +927,15 @@
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_retrieval_by_location() -> Result<()> {
         let dir = setup("data2")?;
         let cfg = default_config(&dir);
-        let mut env = OntoEnv::new(cfg)?;
+        let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
 
         let ont1_path = dir.path().join("ont1.ttl");
         let loc = OntologyLocation::from_str(
             ont1_path
                 .to_str()
                 .ok_or(anyhow::anyhow!("Failed to convert to string"))?,
@@ -952,15 +952,15 @@
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_load() -> Result<()> {
         let dir = setup("data2")?;
         let cfg = default_config(&dir);
-        let mut env = OntoEnv::new(cfg)?;
+        let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         env.save_to_directory()?;
         // drop env
         env.close();
 
         // reload env
@@ -971,15 +971,15 @@
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_add() -> Result<()> {
         let dir = setup("updates")?;
         let cfg1 = default_config_with_subdir(&dir, "v1");
-        let mut env = OntoEnv::new(cfg1)?;
+        let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         let ont_path = dir.path().join("v2/ont5.ttl");
         let loc = OntologyLocation::from_str(
             ont_path
                 .to_str()
@@ -991,15 +991,15 @@
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_detect_updates() -> Result<()> {
         let dir = setup("updates")?;
         let cfg1 = default_config_with_subdir(&dir, "v1");
-        let mut env = OntoEnv::new(cfg1)?;
+        let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         // copy files from dir/v2 to dir/v1
         let base_dir = Path::new("tests/").join("updates").join("v2");
         for entry in walkdir::WalkDir::new(&base_dir) {
             let entry = entry?;
@@ -1016,15 +1016,15 @@
         Ok(())
     }
 
     #[test]
     fn test_check_for_updates() -> Result<()> {
         let dir = setup("updates")?;
         let cfg1 = default_config_with_subdir(&dir, "v1");
-        let mut env = OntoEnv::new(cfg1)?;
+        let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         // copy files from dir/v2 to dir/v1
         let base_dir = Path::new("tests/").join("updates").join("v2");
         for entry in walkdir::WalkDir::new(&base_dir) {
             let entry = entry?;
```

### Comparing `pyontoenv-0.1.6/lib/src/ontology.rs` & `pyontoenv-0.1.7a1/lib/src/ontology.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/policy.rs` & `pyontoenv-0.1.7a1/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/transform.rs` & `pyontoenv-0.1.7a1/lib/src/transform.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/src/util.rs` & `pyontoenv-0.1.7a1/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/model` & `pyontoenv-0.1.7a1/lib/tests/data/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/model.nt` & `pyontoenv-0.1.7a1/lib/tests/data/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/model.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/model.xml` & `pyontoenv-0.1.7a1/lib/tests/data/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.7a1/lib/tests/data/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.7a1/lib/tests/data2/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.7a1/lib/tests/data2/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.7a1/lib/tests/data2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.7a1/lib/tests/data2/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/fileendings/model` & `pyontoenv-0.1.7a1/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.7a1/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.7a1/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.7a1/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.7a1/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.7a1/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.7a1/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/python/Cargo.toml` & `pyontoenv-0.1.7a1/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/python/.github/workflows/CI.yml` & `pyontoenv-0.1.7a1/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/python/.gitignore` & `pyontoenv-0.1.7a1/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/python/README.md` & `pyontoenv-0.1.7a1/python/README.md`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/python/poetry.lock` & `pyontoenv-0.1.7a1/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/python/src/lib.rs` & `pyontoenv-0.1.7a1/python/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use ::ontoenv as ontoenvrs;
 use ::ontoenv::consts::{ONTOLOGY, TYPE};
 use ::ontoenv::ontology::OntologyLocation;
 use ::ontoenv::transform;
 use anyhow::Error;
-use oxigraph::model::{BlankNode, Literal, NamedNode, NamedNodeRef, Term, SubjectRef};
+use oxigraph::model::{BlankNode, Literal, NamedNode, Term, SubjectRef};
 use pyo3::{
     prelude::*,
-    types::{PyBool, PyString, PyTuple, IntoPyDict},
+    types::{PyString, PyTuple, IntoPyDict},
 };
 use std::borrow::Borrow;
 use std::path::{Path, PathBuf};
 use std::sync::Once;
 
 static INIT: Once = Once::new();
 
@@ -140,20 +140,20 @@
                 Some(
                     search_directories
                         .iter()
                         .map(|s| s.to_string().into())
                         .collect::<Vec<PathBuf>>(),
                 ),
                 includes
-                    .unwrap_or_else(|| vec![])
+                    .unwrap_or_default()
                     .iter()
                     .map(|s| s.to_string())
                     .collect::<Vec<_>>(),
                 excludes
-                    .unwrap_or_else(|| vec![])
+                    .unwrap_or_default()
                     .iter()
                     .map(|s| s.to_string())
                     .collect::<Vec<_>>(),
                 require_ontology_names,
                 strict,
                 offline,
                 resolution_policy.to_string(),
```

### Comparing `pyontoenv-0.1.6/python/test.py` & `pyontoenv-0.1.7a1/python/test.py`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.6/Cargo.lock` & `pyontoenv-0.1.7a1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.6"
+version = "0.1.7-a1"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1401,15 +1401,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.6"
+version = "0.1.7-a1"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1719,15 +1719,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.6"
+version = "0.1.7-a1"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.6/Cargo.toml` & `pyontoenv-0.1.7a1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.6"
+version = "0.1.7-a1"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
@@ -27,8 +27,8 @@
 glob = "0.3.1"
 chrono = { version = "0.4.33", features = ["serde"] }
 petgraph = { version = "0.6.4", features = ["serde-1"] }
 clap = { version = "4.4.18", features = ["derive"] }
 derive_builder = "0.13.0"
 oxigraph = "0.3.22"
 
-ontoenv = { version = "0.1.4-alpha6", path = "lib" }
+ontoenv = { version = "0.1.7-a1", path = "lib" }
```

### Comparing `pyontoenv-0.1.6/pyproject.toml` & `pyontoenv-0.1.7a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pyontoenv"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.6"
+version = "0.1.7a1"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 rdflib = "^7.0.0"
 
 [tool.poetry.group.dev.dependencies]
 maturin = "^1.5.0"
```

### Comparing `pyontoenv-0.1.6/PKG-INFO` & `pyontoenv-0.1.7a1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.6
+Version: 0.1.7a1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
 License: BSD-3-Clause
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/gtfierro/ontoenv-rs
 
 # PyOntoenv
 
 ## Installation
```

