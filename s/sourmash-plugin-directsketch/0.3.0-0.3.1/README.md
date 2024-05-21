# Comparing `tmp/sourmash_plugin_directsketch-0.3.0.tar.gz` & `tmp/sourmash_plugin_directsketch-0.3.1.tar.gz`

## Comparing `sourmash_plugin_directsketch-0.3.0.tar` & `sourmash_plugin_directsketch-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.3.0/Cargo.toml
--rw-r--r--   0      501       20      405 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.3.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1421 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.3.0/.github/workflows/build-test.yml
--rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.3.0/.gitignore
--rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.0/LICENSE
--rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.3.0/Makefile
--rw-r--r--   0      501       20     4103 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/README.md
--rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.3.0/environment.yml
--rw-r--r--   0      501       20    26384 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/src/directsketch.rs
--rw-r--r--   0      501       20     2367 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/src/lib.rs
--rw-r--r--   0      501       20     4892 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/src/python/sourmash_plugin_directsketch/__init__.py
--rw-r--r--   0      501       20    11467 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/src/utils.rs
--rw-r--r--   0      501       20      410 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.3.0/tests/conftest.py
--rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.0/tests/sourmash_tst_utils.py
--rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/.notempty
--rw-r--r--   0      501       20    18550 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000175535.1.sig.gz
--rw-r--r--   0      501       20    35505 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000193795.2.sig.gz
--rw-r--r--   0      501       20    23022 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000961135.2.protein.sig.gz
--rw-r--r--   0      501       20    30635 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000961135.2.sig.gz
--rw-r--r--   0      501       20      221 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc-cols.csv
--rw-r--r--   0      501       20      115 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc-version.csv
--rw-r--r--   0      501       20      386 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc-with-ftppath.csv
--rw-r--r--   0      501       20      219 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.0/tests/test-data/acc.csv
--rw-r--r--   0      501       20    17370 2024-05-13 23:02:21.000000 sourmash_plugin_directsketch-0.3.0/tests/test_gbsketch.py
--rw-r--r--   0      501       20    63405 2024-05-13 23:04:06.000000 sourmash_plugin_directsketch-0.3.0/Cargo.lock
--rw-r--r--   0      501       20      966 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.3.1/Cargo.toml
+-rw-r--r--   0      501       20      405 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.3.1/.github/dependabot.yml
+-rw-r--r--   0      501       20     1421 2024-05-09 18:23:54.000000 sourmash_plugin_directsketch-0.3.1/.github/workflows/build-test.yml
+-rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.3.1/.gitignore
+-rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.1/LICENSE
+-rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.3.1/Makefile
+-rw-r--r--   0      501       20     7461 2024-05-21 07:00:48.000000 sourmash_plugin_directsketch-0.3.1/README.md
+-rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.3.1/environment.yml
+-rw-r--r--   0      501       20    36600 2024-05-21 07:00:57.000000 sourmash_plugin_directsketch-0.3.1/src/directsketch.rs
+-rw-r--r--   0      501       20     3065 2024-05-21 07:00:42.000000 sourmash_plugin_directsketch-0.3.1/src/lib.rs
+-rw-r--r--   0      501       20     8127 2024-05-21 07:00:42.000000 sourmash_plugin_directsketch-0.3.1/src/python/sourmash_plugin_directsketch/__init__.py
+-rw-r--r--   0      501       20    12132 2024-05-21 07:00:42.000000 sourmash_plugin_directsketch-0.3.1/src/utils.rs
+-rw-r--r--   0      501       20      410 2024-05-09 18:23:51.000000 sourmash_plugin_directsketch-0.3.1/tests/conftest.py
+-rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.1/tests/sourmash_tst_utils.py
+-rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/.notempty
+-rw-r--r--   0      501       20    18550 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000175535.1.sig.gz
+-rw-r--r--   0      501       20    35505 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000193795.2.sig.gz
+-rw-r--r--   0      501       20    23022 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000961135.2.protein.sig.gz
+-rw-r--r--   0      501       20    30635 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000961135.2.sig.gz
+-rw-r--r--   0      501       20      221 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/acc-cols.csv
+-rw-r--r--   0      501       20      944 2024-05-21 07:00:42.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/acc-url.csv
+-rw-r--r--   0      501       20      115 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/acc-version.csv
+-rw-r--r--   0      501       20      386 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/acc-with-ftppath.csv
+-rw-r--r--   0      501       20      219 2024-05-13 22:18:01.000000 sourmash_plugin_directsketch-0.3.1/tests/test-data/acc.csv
+-rw-r--r--   0      501       20    18184 2024-05-21 07:00:42.000000 sourmash_plugin_directsketch-0.3.1/tests/test_gbsketch.py
+-rw-r--r--   0      501       20    13420 2024-05-21 07:00:57.000000 sourmash_plugin_directsketch-0.3.1/tests/test_urlsketch.py
+-rw-r--r--   0      501       20    63405 2024-05-21 07:05:26.000000 sourmash_plugin_directsketch-0.3.1/Cargo.lock
+-rw-r--r--   0      501       20     1033 2024-05-21 07:00:42.000000 sourmash_plugin_directsketch-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8131 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.3.1/PKG-INFO
```

### Comparing `sourmash_plugin_directsketch-0.3.0/Cargo.toml` & `sourmash_plugin_directsketch-0.3.1/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 
 [package]
 name = "sourmash_plugin_directsketch"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 
 [lib]
 name = "sourmash_plugin_directsketch"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21.2", features = ["extension-module", "anyhow"] }
 rayon = "1.10.0"
-serde = { version = "1.0.201", features = ["derive"] }
+serde = { version = "1.0.202", features = ["derive"] }
 sourmash = { version = "0.13.1"}
 serde_json = "1.0.117"
 niffler = "2.4.0"
 needletail = "0.5.1"
 #zip = { version = "0.6", default-features = false, features = ["deflate"] }
 async_zip={version="0.0.17", features=["full"]}
 simple-error = "0.3.0"
-anyhow = "1.0.83"
-camino = "1.1.6"
+anyhow = "1.0.86"
+camino = "1.1.7"
 csv = "1.3.0"
 reqwest = { version = "0.12.4", features = ["json", "stream"] }
 tokio = { version = "1.37.0", features = ["full"] }
 tokio-util = "0.7.11"
 regex = "1.10.4"
 chrono = "0.4.32"
 lazy_static = "1.4.0"
```

### Comparing `sourmash_plugin_directsketch-0.3.0/.github/workflows/build-test.yml` & `sourmash_plugin_directsketch-0.3.1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/.gitignore` & `sourmash_plugin_directsketch-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/LICENSE` & `sourmash_plugin_directsketch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/src/directsketch.rs` & `sourmash_plugin_directsketch-0.3.1/src/directsketch.rs`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 
 use pyo3::prelude::*;
 
 use sourmash::manifest::{Manifest, Record};
 use sourmash::signature::Signature;
 
 use crate::utils::{
-    build_siginfo, load_gbassembly_info, parse_params_str, GBAssemblyData, GenBankFileType,
+    build_siginfo, load_accession_info, load_gbassembly_info, parse_params_str, AccessionData,
+    GBAssemblyData, GenBankFileType, InputMolType,
 };
 use reqwest::Url;
 
 async fn find_genome_directory(
     client: &Client,
     db: &str,
     number_path: &str,
@@ -237,20 +238,22 @@
         Result::<Vec<Signature>, anyhow::Error>::Ok(sigs)
     })
     .await?
 }
 pub struct FailedDownload {
     accession: String,
     name: String,
-    url: Option<Url>,
     moltype: String,
+    md5sum: Option<String>,
+    download_filename: Option<String>,
+    url: Option<Url>,
 }
 
 #[allow(clippy::too_many_arguments)]
-async fn dl_sketch_accession(
+async fn dl_sketch_assembly_accession(
     client: &Client,
     accinfo: GBAssemblyData,
     location: &PathBuf,
     retry: Option<u32>,
     keep_fastas: bool,
     dna_sigs: Vec<Signature>,
     prot_sigs: Vec<Signature>,
@@ -271,25 +274,29 @@
             Ok(result) => result,
             Err(_err) => {
                 // Add accession to failed downloads with each moltype
                 if !proteomes_only {
                     let failed_download_dna = FailedDownload {
                         accession: accession.clone(),
                         name: name.clone(),
-                        url: None,
                         moltype: "dna".to_string(),
+                        md5sum: None,
+                        download_filename: None,
+                        url: None,
                     };
                     failed.push(failed_download_dna);
                 }
                 if !genomes_only {
                     let failed_download_protein = FailedDownload {
                         accession: accession.clone(),
                         name: name.clone(),
-                        url: None,
                         moltype: "protein".to_string(),
+                        md5sum: None,
+                        download_filename: None,
+                        url: None,
                     };
                     failed.push(failed_download_protein);
                 }
 
                 return Ok((sigs, failed));
             }
         };
@@ -312,32 +319,34 @@
     } else if proteomes_only {
         file_types = vec![GenBankFileType::Protein];
     }
 
     for file_type in &file_types {
         let url = file_type.url(&base_url, &full_name);
         let expected_md5 = checksums.get(&file_type.server_filename(&full_name));
+        let file_name = file_type.filename_to_write(&accession);
         let data =
             match download_with_retry(client, &url, expected_md5.map(|x| x.as_str()), retry_count)
                 .await
             {
                 Ok(data) => data,
                 Err(_err) => {
                     // here --> keep track of accession errors + filetype
                     let failed_download = FailedDownload {
                         accession: accession.clone(),
                         name: name.clone(),
-                        url: Some(url),
                         moltype: file_type.moltype(),
+                        md5sum: expected_md5.map(|x| x.to_string()),
+                        download_filename: Some(file_name),
+                        url: Some(url),
                     };
                     failed.push(failed_download);
                     continue;
                 }
             };
-        let file_name = file_type.filename_to_write(&accession);
 
         if keep_fastas {
             let path = location.join(&file_name);
             fs::write(&path, &data).context("Failed to write data to file")?;
         }
         if !download_only {
             // sketch data
@@ -368,14 +377,93 @@
             };
         }
     }
 
     Ok((sigs, failed))
 }
 
+#[allow(clippy::too_many_arguments)]
+async fn dl_sketch_url(
+    client: &Client,
+    accinfo: AccessionData,
+    location: &PathBuf,
+    retry: Option<u32>,
+    _keep_fastas: bool,
+    dna_sigs: Vec<Signature>,
+    prot_sigs: Vec<Signature>,
+    _genomes_only: bool,
+    _proteomes_only: bool,
+    download_only: bool,
+) -> Result<(Vec<Signature>, Vec<FailedDownload>)> {
+    let retry_count = retry.unwrap_or(3); // Default retry count
+    let mut sigs = Vec::<Signature>::new();
+    let mut failed = Vec::<FailedDownload>::new();
+
+    let name = accinfo.name;
+    let accession = accinfo.accession;
+    let url = accinfo.url;
+    let expected_md5 = accinfo.expected_md5sum;
+    let download_filename = accinfo.download_filename;
+    let moltype = accinfo.moltype;
+
+    match download_with_retry(client, &url, expected_md5.as_deref(), retry_count)
+        .await
+        .ok()
+    {
+        Some(data) => {
+            // check keep_fastas instead??
+            if let Some(ref download_filename) = download_filename {
+                let path = location.join(download_filename);
+                fs::write(path, &data).context("Failed to write data to file")?;
+            }
+            if !download_only {
+                let filename = download_filename.clone().unwrap_or("".to_string());
+                // sketch data
+                match moltype {
+                    InputMolType::Dna => sigs.extend(
+                        sketch_data(
+                            name.clone(),
+                            filename.clone(),
+                            data,
+                            dna_sigs.clone(),
+                            "dna".to_string(),
+                        )
+                        .await?,
+                    ),
+                    InputMolType::Protein => {
+                        sigs.extend(
+                            sketch_data(
+                                name.clone(),
+                                filename.clone(),
+                                data,
+                                prot_sigs.clone(),
+                                "protein".to_string(),
+                            )
+                            .await?,
+                        );
+                    }
+                };
+            }
+        }
+        None => {
+            let failed_download = FailedDownload {
+                accession: accession.clone(),
+                name: name.clone(),
+                moltype: moltype.to_string(),
+                md5sum: expected_md5.map(|x| x.to_string()),
+                download_filename,
+                url: Some(url),
+            };
+            failed.push(failed_download);
+        }
+    }
+
+    Ok((sigs, failed))
+}
+
 async fn write_sig(
     sig: &Signature,
     md5sum_occurrences: &mut HashMap<String, usize>,
     manifest_rows: &mut Vec<Record>,
     zip_writer: &mut ZipFileWriter<Compat<tokio::fs::File>>,
 ) -> Result<()> {
     let md5sum_str = sig.md5sum();
@@ -510,28 +598,41 @@
 ) -> tokio::task::JoinHandle<()> {
     tokio::spawn(async move {
         match File::create(&failed_csv).await {
             Ok(file) => {
                 let mut writer = BufWriter::new(file);
 
                 // Attempt to write CSV headers
-                if let Err(e) = writer.write_all(b"accession,name,moltype,url\n").await {
+                if let Err(e) = writer
+                    .write_all(b"accession,name,moltype,md5sum,download_filename,url\n")
+                    .await
+                {
                     let error = Error::new(e).context("Failed to write headers");
                     let _ = error_sender.send(error).await;
                     return; // Exit the task early after reporting the error
                 }
 
                 while let Some(FailedDownload {
                     accession,
                     name,
-                    moltype,
+                    md5sum,
+                    download_filename,
                     url,
+                    moltype,
                 }) = recv_failed.recv().await
                 {
-                    let record = format!("{},{},{},{:?}\n", accession, name, moltype, url);
+                    let record = format!(
+                        "{},{},{},{},{},{}\n",
+                        accession,
+                        name,
+                        moltype,
+                        md5sum.unwrap_or("".to_string()),
+                        download_filename.unwrap_or("".to_string()),
+                        url.map(|u| u.to_string()).unwrap_or("".to_string())
+                    );
                     // Attempt to write each record
                     if let Err(e) = writer.write_all(record.as_bytes()).await {
                         let error = Error::new(e).context("Failed to write record");
                         let _ = error_sender.send(error).await;
                         continue; // Optionally continue to try to write next records
                     }
                 }
@@ -564,15 +665,15 @@
             }
         }
     })
 }
 
 #[tokio::main]
 #[allow(clippy::too_many_arguments)]
-pub async fn download_and_sketch(
+pub async fn gbsketch(
     py: Python,
     input_csv: String,
     param_str: String,
     failed_csv: String,
     retry_times: u32,
     fasta_location: String,
     keep_fastas: bool,
@@ -634,14 +735,188 @@
     let prot_sig_templates = build_siginfo(&params_vec, "protein");
 
     let mut genomes_only = genomes_only;
     let mut proteomes_only = proteomes_only;
 
     // Check if dna_sig_templates is empty and not keep_fastas
     if dna_sig_templates.is_empty() && !keep_fastas {
+        eprintln!("No DNA signature templates provided, and --keep-fasta is not set.");
+        proteomes_only = true;
+    }
+    // Check if protein_sig_templates is empty and not keep_fastas
+    if prot_sig_templates.is_empty() && !keep_fastas {
+        eprintln!("No protein signature templates provided, and --keep-fasta is not set.");
+        genomes_only = true;
+    }
+    if genomes_only {
+        if !download_only {
+            eprintln!("Downloading and sketching genomes only.");
+        } else {
+            eprintln!("Downloading genomes only.");
+        }
+    } else if proteomes_only {
+        if !download_only {
+            eprintln!("Downloading and sketching proteomes only.");
+        } else {
+            eprintln!("Downloading proteomes only.");
+        }
+    }
+
+    // report every 1 percent (or every 1, whichever is larger)
+    let reporting_threshold = std::cmp::max(n_accs / 100, 1);
+
+    for (i, accinfo) in accession_info.into_iter().enumerate() {
+        py.check_signals()?; // If interrupted, return an Err automatically
+        let semaphore_clone = Arc::clone(&semaphore);
+        let client_clone = Arc::clone(&client);
+        let send_sigs = send_sigs.clone();
+        let send_failed = send_failed.clone();
+        let download_path_clone = download_path.clone(); // Clone the path for each task
+        let send_errors = error_sender.clone();
+
+        let dna_sigs = dna_sig_templates.clone();
+        let prot_sigs = prot_sig_templates.clone();
+
+        tokio::spawn(async move {
+            let _permit = semaphore_clone.acquire().await;
+            // progress report when the permit is available and processing begins
+            if (i + 1) % reporting_threshold == 0 {
+                let percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
+                println!(
+                    "Starting accession {}/{} ({}%)",
+                    (i + 1),
+                    n_accs,
+                    percent_processed
+                );
+            }
+            // Perform download and sketch
+            let result = dl_sketch_assembly_accession(
+                &client_clone,
+                accinfo.clone(),
+                &download_path_clone,
+                Some(retry_times),
+                keep_fastas,
+                dna_sigs,
+                prot_sigs,
+                genomes_only,
+                proteomes_only,
+                download_only,
+            )
+            .await;
+            match result {
+                Ok((sigs, failed_downloads)) => {
+                    if !sigs.is_empty() {
+                        if let Err(e) = send_sigs.send(sigs).await {
+                            eprintln!("Failed to send signatures: {}", e);
+                            let _ = send_errors.send(e.into()).await; // Send the error through the channel
+                        }
+                    }
+                    for fail in failed_downloads {
+                        if let Err(e) = send_failed.send(fail).await {
+                            eprintln!("Failed to send failed download info: {}", e);
+                            let _ = send_errors.send(e.into()).await; // Send the error through the channel
+                        }
+                    }
+                }
+                Err(e) => {
+                    let _ = send_errors.send(e).await;
+                }
+            }
+            drop(send_errors);
+        });
+    }
+    // drop senders as we're done sending data
+    drop(send_sigs);
+    drop(send_failed);
+    drop(error_sender);
+    // Wait for all tasks to complete
+    for handle in handles {
+        if let Err(e) = handle.await {
+            eprintln!("Handle join error: {}.", e);
+        }
+    }
+    // since the only critical error is not having written any sigs
+    // check this here at end. Bail if we wrote expected sigs but wrote none.
+    if critical_error_flag.load(Ordering::SeqCst) & !download_only {
+        bail!("No signatures written, exiting.");
+    }
+
+    Ok(())
+}
+
+#[tokio::main]
+#[allow(clippy::too_many_arguments)]
+pub async fn urlsketch(
+    py: Python,
+    input_csv: String,
+    param_str: String,
+    failed_csv: String,
+    retry_times: u32,
+    fasta_location: String,
+    keep_fastas: bool,
+    download_only: bool,
+    output_sigs: Option<String>,
+) -> Result<(), anyhow::Error> {
+    // if sig output provided but doesn't end in zip, bail
+    if let Some(ref output_sigs) = output_sigs {
+        if Path::new(&output_sigs)
+            .extension()
+            .map_or(true, |ext| ext != "zip")
+        {
+            bail!("Output must be a zip file.");
+        }
+    }
+    // set up fasta download path
+    let download_path = PathBuf::from(fasta_location);
+    if !download_path.exists() {
+        create_dir_all(&download_path)?;
+    }
+
+    // create channels. buffer size here is 4 b/c we can do 3 downloads simultaneously
+    let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::<Vec<Signature>>(4);
+    let (send_failed, recv_failed) = tokio::sync::mpsc::channel::<FailedDownload>(4);
+    // Error channel for handling task errors
+    let (error_sender, error_receiver) = tokio::sync::mpsc::channel::<anyhow::Error>(1);
+
+    // Set up collector/writing tasks
+    let mut handles = Vec::new();
+    let sig_handle = sigwriter_handle(recv_sigs, output_sigs, error_sender.clone());
+    let failures_handle = failures_handle(failed_csv, recv_failed, error_sender.clone());
+    let critical_error_flag = Arc::new(AtomicBool::new(false));
+    let error_handle = error_handler(error_receiver, critical_error_flag.clone());
+    handles.push(sig_handle);
+    handles.push(failures_handle);
+    handles.push(error_handle);
+
+    // Worker tasks
+    let semaphore = Arc::new(Semaphore::new(3)); // Limiting concurrent downloads
+    let client = Arc::new(Client::new());
+
+    // Open the file containing the accessions synchronously
+    let (accession_info, n_accs) = load_accession_info(input_csv, keep_fastas)?;
+    if n_accs == 0 {
+        bail!("No accessions to download and sketch.")
+    }
+
+    // parse param string into params_vec, print error if fail
+    let param_result = parse_params_str(param_str);
+    let params_vec = match param_result {
+        Ok(params) => params,
+        Err(e) => {
+            bail!("Failed to parse params string: {}", e);
+        }
+    };
+    let dna_sig_templates = build_siginfo(&params_vec, "DNA");
+    let prot_sig_templates = build_siginfo(&params_vec, "protein");
+
+    let mut genomes_only = false;
+    let mut proteomes_only = false;
+
+    // Check if dna_sig_templates is empty and not keep_fastas
+    if dna_sig_templates.is_empty() && !keep_fastas {
         eprintln!("No DNA signature templates provided, and --keep-fastas is not set.");
         proteomes_only = true;
     }
     // Check if protein_sig_templates is empty and not keep_fastas
     if prot_sig_templates.is_empty() && !keep_fastas {
         eprintln!("No protein signature templates provided, and --keep-fastas is not set.");
         genomes_only = true;
@@ -684,15 +959,15 @@
                     "Starting accession {}/{} ({}%)",
                     (i + 1),
                     n_accs,
                     percent_processed
                 );
             }
             // Perform download and sketch
-            let result = dl_sketch_accession(
+            let result = dl_sketch_url(
                 &client_clone,
                 accinfo.clone(),
                 &download_path_clone,
                 Some(retry_times),
                 keep_fastas,
                 dna_sigs,
                 prot_sigs,
```

#### html2text {}

```diff
@@ -3,19 +3,20 @@
 ZipEntryBuilder}; use camino::Utf8PathBuf as PathBuf; use chrono::Utc; use
 needletail::parse_fastx_reader; use regex::Regex; use reqwest::Client; use
 std::collections::HashMap; use std::fs::{self, create_dir_all}; use std::io::
 Cursor; use std::path::Path; use std::sync::atomic::{AtomicBool, Ordering}; use
 std::sync::Arc; use tokio::fs::File; use tokio::io::{AsyncWriteExt, BufWriter};
 use tokio::sync::Semaphore; use tokio_util::compat::Compat; use pyo3::prelude::
 *; use sourmash::manifest::{Manifest, Record}; use sourmash::signature::
-Signature; use crate::utils::{ build_siginfo, load_gbassembly_info,
-parse_params_str, GBAssemblyData, GenBankFileType, }; use reqwest::Url; async
-fn find_genome_directory( client: &Client, db: &str, number_path: &str,
-accession: &str, acc_number: &str, version: &str, ) -> Result<(Url, String)>
-{ let base_url = format!( "https://ftp.ncbi.nlm.nih.gov/genomes/all/{}/{}", db,
+Signature; use crate::utils::{ build_siginfo, load_accession_info,
+load_gbassembly_info, parse_params_str, AccessionData, GBAssemblyData,
+GenBankFileType, InputMolType, }; use reqwest::Url; async fn
+find_genome_directory( client: &Client, db: &str, number_path: &str, accession:
+&str, acc_number: &str, version: &str, ) -> Result<(Url, String)> { let
+base_url = format!( "https://ftp.ncbi.nlm.nih.gov/genomes/all/{}/{}", db,
 number_path ); let directory_response = client.get(&base_url).send().await?; if
 !directory_response.status().is_success() { return Err(anyhow!( "Failed to open
 genome directory: HTTP {}, {}", directory_response.status(), directory_response
 .status() .canonical_reason() .unwrap_or("Unknown reason") )); } let text =
 directory_response.text().await?; let link_regex = Regex::new(r#"
 +)/""#)?; for cap in link_regex.captures_iter(&text) { let name = ∩[1]; // Use
 acc numerical identifier and version as expected pattern let expected_pattern =
@@ -71,53 +72,78 @@
 record")?; sigs.iter_mut().for_each(|sig| { if !set_name { sig.set_name(&name);
 sig.set_filename(&filename); }; if moltype == "protein" { sig.add_protein
 (&record.seq()) .expect("Failed to add protein"); } else { sig.add_sequence
 (&record.seq(), true) .expect("Failed to add sequence"); // if not force,
 panics with 'N' in dna sequence } }); if !set_name { set_name = true; } }
 Result::
 Signature>, anyhow::Error>::Ok(sigs) }) .await? } pub struct FailedDownload
-{ accession: String, name: String, url: Option, moltype: String, } #[allow
-(clippy::too_many_arguments)] async fn dl_sketch_accession( client: &Client,
-accinfo: GBAssemblyData, location: &PathBuf, retry: Option, keep_fastas: bool,
-dna_sigs: Vec, prot_sigs: Vec, genomes_only: bool, proteomes_only: bool,
-download_only: bool, ) -> Result<(Vec, Vec)> { let retry_count =
-retry.unwrap_or(3); // Default retry count let mut sigs = Vec::::new(); let mut
-failed = Vec::::new(); let name = accinfo.name; let accession =
-accinfo.accession; // keep track of any accessions for which we fail to find
-URLs let (base_url, full_name) = match fetch_genbank_filename(client,
-accession.as_str(), accinfo.url).await { Ok(result) => result, Err(_err) => { /
-/ Add accession to failed downloads with each moltype if !proteomes_only { let
-failed_download_dna = FailedDownload { accession: accession.clone(), name:
-name.clone(), url: None, moltype: "dna".to_string(), }; failed.push
+{ accession: String, name: String, moltype: String, md5sum: Option,
+download_filename: Option, url: Option, } #[allow(clippy::too_many_arguments)]
+async fn dl_sketch_assembly_accession( client: &Client, accinfo:
+GBAssemblyData, location: &PathBuf, retry: Option, keep_fastas: bool, dna_sigs:
+Vec, prot_sigs: Vec, genomes_only: bool, proteomes_only: bool, download_only:
+bool, ) -> Result<(Vec, Vec)> { let retry_count = retry.unwrap_or(3); /
+/ Default retry count let mut sigs = Vec::::new(); let mut failed = Vec::::new
+(); let name = accinfo.name; let accession = accinfo.accession; // keep track
+of any accessions for which we fail to find URLs let (base_url, full_name) =
+match fetch_genbank_filename(client, accession.as_str(), accinfo.url).await
+{ Ok(result) => result, Err(_err) => { // Add accession to failed downloads
+with each moltype if !proteomes_only { let failed_download_dna = FailedDownload
+{ accession: accession.clone(), name: name.clone(), moltype: "dna".to_string(),
+md5sum: None, download_filename: None, url: None, }; failed.push
 (failed_download_dna); } if !genomes_only { let failed_download_protein =
-FailedDownload { accession: accession.clone(), name: name.clone(), url: None,
-moltype: "protein".to_string(), }; failed.push(failed_download_protein); }
-return Ok((sigs, failed)); } }; let md5sum_url = GenBankFileType::Checksum.url
-(&base_url, &full_name); let checksums = match download_and_parse_md5(client,
-&md5sum_url).await { Ok(cs) => cs, Err(e) => { return Err(e); } }; let mut
-file_types = vec![ GenBankFileType::Genomic, GenBankFileType::Protein, /
-/ GenBankFileType::AssemblyReport, ]; if genomes_only { file_types = vec!
-[GenBankFileType::Genomic]; } else if proteomes_only { file_types = vec!
-[GenBankFileType::Protein]; } for file_type in &file_types { let url =
-file_type.url(&base_url, &full_name); let expected_md5 = checksums.get
-(&file_type.server_filename(&full_name)); let data = match download_with_retry
-(client, &url, expected_md5.map(|x| x.as_str()), retry_count) .await { Ok(data)
-=> data, Err(_err) => { // here --> keep track of accession errors + filetype
-let failed_download = FailedDownload { accession: accession.clone(), name:
-name.clone(), url: Some(url), moltype: file_type.moltype(), }; failed.push
-(failed_download); continue; } }; let file_name = file_type.filename_to_write
-(&accession); if keep_fastas { let path = location.join(&file_name); fs::write
-(&path, &data).context("Failed to write data to file")?; } if !download_only
-{ // sketch data match file_type { GenBankFileType::Genomic => sigs.extend
+FailedDownload { accession: accession.clone(), name: name.clone(), moltype:
+"protein".to_string(), md5sum: None, download_filename: None, url: None, };
+failed.push(failed_download_protein); } return Ok((sigs, failed)); } }; let
+md5sum_url = GenBankFileType::Checksum.url(&base_url, &full_name); let
+checksums = match download_and_parse_md5(client, &md5sum_url).await { Ok(cs) =>
+cs, Err(e) => { return Err(e); } }; let mut file_types = vec!
+[ GenBankFileType::Genomic, GenBankFileType::Protein, // GenBankFileType::
+AssemblyReport, ]; if genomes_only { file_types = vec![GenBankFileType::
+Genomic]; } else if proteomes_only { file_types = vec![GenBankFileType::
+Protein]; } for file_type in &file_types { let url = file_type.url(&base_url,
+&full_name); let expected_md5 = checksums.get(&file_type.server_filename
+(&full_name)); let file_name = file_type.filename_to_write(&accession); let
+data = match download_with_retry(client, &url, expected_md5.map(|x| x.as_str
+()), retry_count) .await { Ok(data) => data, Err(_err) => { // here --> keep
+track of accession errors + filetype let failed_download = FailedDownload
+{ accession: accession.clone(), name: name.clone(), moltype: file_type.moltype
+(), md5sum: expected_md5.map(|x| x.to_string()), download_filename: Some
+(file_name), url: Some(url), }; failed.push(failed_download); continue; } }; if
+keep_fastas { let path = location.join(&file_name); fs::write(&path,
+&data).context("Failed to write data to file")?; } if !download_only { /
+/ sketch data match file_type { GenBankFileType::Genomic => sigs.extend
 ( sketch_data( name.clone(), file_name.clone(), data, dna_sigs.clone(),
 "dna".to_string(), ) .await?, ), GenBankFileType::Protein => { sigs.extend
 ( sketch_data( name.clone(), file_name.clone(), data, prot_sigs.clone(),
 "protein".to_string(), ) .await?, ); } _ => {} // Do nothing for other file
-types }; } } Ok((sigs, failed)) } async fn write_sig( sig: &Signature,
-md5sum_occurrences: &mut HashMap
+types }; } } Ok((sigs, failed)) } #[allow(clippy::too_many_arguments)] async fn
+dl_sketch_url( client: &Client, accinfo: AccessionData, location: &PathBuf,
+retry: Option, _keep_fastas: bool, dna_sigs: Vec, prot_sigs: Vec,
+_genomes_only: bool, _proteomes_only: bool, download_only: bool, ) -> Result<
+(Vec, Vec)> { let retry_count = retry.unwrap_or(3); // Default retry count let
+mut sigs = Vec::::new(); let mut failed = Vec::::new(); let name =
+accinfo.name; let accession = accinfo.accession; let url = accinfo.url; let
+expected_md5 = accinfo.expected_md5sum; let download_filename =
+accinfo.download_filename; let moltype = accinfo.moltype; match
+download_with_retry(client, &url, expected_md5.as_deref(), retry_count) .await
+.ok() { Some(data) => { // check keep_fastas instead?? if let Some(ref
+download_filename) = download_filename { let path = location.join
+(download_filename); fs::write(path, &data).context("Failed to write data to
+file")?; } if !download_only { let filename = download_filename.clone
+().unwrap_or("".to_string()); // sketch data match moltype { InputMolType::Dna
+=> sigs.extend( sketch_data( name.clone(), filename.clone(), data,
+dna_sigs.clone(), "dna".to_string(), ) .await?, ), InputMolType::Protein =>
+{ sigs.extend( sketch_data( name.clone(), filename.clone(), data,
+prot_sigs.clone(), "protein".to_string(), ) .await?, ); } }; } } None => { let
+failed_download = FailedDownload { accession: accession.clone(), name:
+name.clone(), moltype: moltype.to_string(), md5sum: expected_md5.map(|x|
+x.to_string()), download_filename, url: Some(url), }; failed.push
+(failed_download); } } Ok((sigs, failed)) } async fn write_sig( sig:
+&Signature, md5sum_occurrences: &mut HashMap
  usize>, manifest_rows: &mut Vec, zip_writer: &mut ZipFileWriter
 tokio::fs::File>>, ) -> Result<()> { let md5sum_str = sig.md5sum(); let count =
 md5sum_occurrences.entry(md5sum_str.clone()).or_insert(0); *count += 1; let
 sig_filename = if *count > 1 { format!("signatures/{}_{}.sig.gz", md5sum_str,
 count) } else { format!("signatures/{}.sig.gz", md5sum_str) }; let records: Vec
 = Record::from_sig(sig, &sig_filename); manifest_rows.extend(records); let
 wrapped_sig = vec![sig.clone()]; let json_bytes = serde_json::to_vec
@@ -162,37 +188,40 @@
 error_sender.send(error).await; // Send error about no signatures written } }
 drop(error_sender); // should be dropped automatically as it goes out of scope,
 but just in case }) } pub fn failures_handle( failed_csv: String, mut
 recv_failed: tokio::sync::mpsc::Receiver, error_sender: tokio::sync::mpsc::
 Sender, // Additional parameter for error channel ) -> tokio::task::JoinHandle<
 ()> { tokio::spawn(async move { match File::create(&failed_csv).await { Ok
 (file) => { let mut writer = BufWriter::new(file); // Attempt to write CSV
-headers if let Err(e) = writer.write_all(b"accession,name,moltype,url\n").await
-{ let error = Error::new(e).context("Failed to write headers"); let _ =
-error_sender.send(error).await; return; // Exit the task early after reporting
-the error } while let Some(FailedDownload { accession, name, moltype, url, }) =
-recv_failed.recv().await { let record = format!("{},{},{},{:?}\n", accession,
-name, moltype, url); // Attempt to write each record if let Err(e) =
-writer.write_all(record.as_bytes()).await { let error = Error::new(e).context
+headers if let Err(e) = writer .write_all
+(b"accession,name,moltype,md5sum,download_filename,url\n") .await { let error =
+Error::new(e).context("Failed to write headers"); let _ = error_sender.send
+(error).await; return; // Exit the task early after reporting the error } while
+let Some(FailedDownload { accession, name, md5sum, download_filename, url,
+moltype, }) = recv_failed.recv().await { let record = format!( "{},{},{},{},{},
+{}\n", accession, name, moltype, md5sum.unwrap_or("".to_string()),
+download_filename.unwrap_or("".to_string()), url.map(|u| u.to_string
+()).unwrap_or("".to_string()) ); // Attempt to write each record if let Err(e)
+= writer.write_all(record.as_bytes()).await { let error = Error::new(e).context
 ("Failed to write record"); let _ = error_sender.send(error).await; continue; /
 / Optionally continue to try to write next records } } // Attempt to flush the
 writer if let Err(e) = writer.flush().await { let error = Error::new(e).context
 ("Failed to flush writer"); let _ = error_sender.send(error).await; } } Err(e)
 => { let error = Error::new(e).context("Failed to create file"); let _ =
 error_sender.send(error).await; } } drop(error_sender); }) } pub fn
 error_handler( mut recv_errors: tokio::sync::mpsc::Receiver, error_flag: Arc, )
 -> tokio::task::JoinHandle<()> { tokio::spawn(async move { while let Some
 (error) = recv_errors.recv().await { eprintln!("Error: {}", error); if
 error.to_string().contains("No signatures written") { error_flag.store(true,
 Ordering::SeqCst); break; } } }) } #[tokio::main] #[allow(clippy::
-too_many_arguments)] pub async fn download_and_sketch( py: Python, input_csv:
-String, param_str: String, failed_csv: String, retry_times: u32,
-fasta_location: String, keep_fastas: bool, genomes_only: bool, proteomes_only:
-bool, download_only: bool, output_sigs: Option, ) -> Result<(), anyhow::Error>
-{ // if sig output provided but doesn't end in zip, bail if let Some(ref
+too_many_arguments)] pub async fn gbsketch( py: Python, input_csv: String,
+param_str: String, failed_csv: String, retry_times: u32, fasta_location:
+String, keep_fastas: bool, genomes_only: bool, proteomes_only: bool,
+download_only: bool, output_sigs: Option, ) -> Result<(), anyhow::Error> { /
+/ if sig output provided but doesn't end in zip, bail if let Some(ref
 output_sigs) = output_sigs { if Path::new(&output_sigs) .extension() .map_or
 (true, |ext| ext != "zip") { bail!("Output must be a zip file."); } } // set up
 fasta download path let download_path = PathBuf::from(fasta_location); if
 !download_path.exists() { create_dir_all(&download_path)?; } // create
 channels. buffer size here is 4 b/c we can do 3 downloads simultaneously let
 (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::
 Signature>>(4); let (send_failed, recv_failed) = tokio::sync::mpsc::channel::
@@ -212,18 +241,18 @@
 fail let param_result = parse_params_str(param_str); let params_vec = match
 param_result { Ok(params) => params, Err(e) => { bail!("Failed to parse params
 string: {}", e); } }; let dna_sig_templates = build_siginfo(&params_vec,
 "DNA"); let prot_sig_templates = build_siginfo(&params_vec, "protein"); let mut
 genomes_only = genomes_only; let mut proteomes_only = proteomes_only; // Check
 if dna_sig_templates is empty and not keep_fastas if dna_sig_templates.is_empty
 () && !keep_fastas { eprintln!("No DNA signature templates provided, and --
-keep-fastas is not set."); proteomes_only = true; } // Check if
+keep-fasta is not set."); proteomes_only = true; } // Check if
 protein_sig_templates is empty and not keep_fastas if
 prot_sig_templates.is_empty() && !keep_fastas { eprintln!("No protein signature
-templates provided, and --keep-fastas is not set."); genomes_only = true; } if
+templates provided, and --keep-fasta is not set."); genomes_only = true; } if
 genomes_only { if !download_only { eprintln!("Downloading and sketching genomes
 only."); } else { eprintln!("Downloading genomes only."); } } else if
 proteomes_only { if !download_only { eprintln!("Downloading and sketching
 proteomes only."); } else { eprintln!("Downloading proteomes only."); } } /
 / report every 1 percent (or every 1, whichever is larger) let
 reporting_threshold = std::cmp::max(n_accs / 100, 1); for (i, accinfo) in
 accession_info.into_iter().enumerate() { py.check_signals()?; // If
@@ -233,15 +262,15 @@
 download_path_clone = download_path.clone(); // Clone the path for each task
 let send_errors = error_sender.clone(); let dna_sigs = dna_sig_templates.clone
 (); let prot_sigs = prot_sig_templates.clone(); tokio::spawn(async move { let
 _permit = semaphore_clone.acquire().await; // progress report when the permit
 is available and processing begins if (i + 1) % reporting_threshold == 0 { let
 percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
 println!( "Starting accession {}/{} ({}%)", (i + 1), n_accs, percent_processed
-); } // Perform download and sketch let result = dl_sketch_accession
+); } // Perform download and sketch let result = dl_sketch_assembly_accession
 ( &client_clone, accinfo.clone(), &download_path_clone, Some(retry_times),
 keep_fastas, dna_sigs, prot_sigs, genomes_only, proteomes_only, download_only,
 ) .await; match result { Ok((sigs, failed_downloads)) => { if !sigs.is_empty()
 { if let Err(e) = send_sigs.send(sigs).await { eprintln!("Failed to send
 signatures: {}", e); let _ = send_errors.send(e.into()).await; // Send the
 error through the channel } } for fail in failed_downloads { if let Err(e) =
 send_failed.send(fail).await { eprintln!("Failed to send failed download info:
@@ -249,8 +278,78 @@
 the channel } } } Err(e) => { let _ = send_errors.send(e).await; } } drop
 (send_errors); }); } // drop senders as we're done sending data drop
 (send_sigs); drop(send_failed); drop(error_sender); // Wait for all tasks to
 complete for handle in handles { if let Err(e) = handle.await { eprintln!
 ("Handle join error: {}.", e); } } // since the only critical error is not
 having written any sigs // check this here at end. Bail if we wrote expected
 sigs but wrote none. if critical_error_flag.load(Ordering::SeqCst) &
-!download_only { bail!("No signatures written, exiting."); } Ok(()) }
+!download_only { bail!("No signatures written, exiting."); } Ok(()) } #[tokio::
+main] #[allow(clippy::too_many_arguments)] pub async fn urlsketch( py: Python,
+input_csv: String, param_str: String, failed_csv: String, retry_times: u32,
+fasta_location: String, keep_fastas: bool, download_only: bool, output_sigs:
+Option, ) -> Result<(), anyhow::Error> { // if sig output provided but doesn't
+end in zip, bail if let Some(ref output_sigs) = output_sigs { if Path::new
+(&output_sigs) .extension() .map_or(true, |ext| ext != "zip") { bail!("Output
+must be a zip file."); } } // set up fasta download path let download_path =
+PathBuf::from(fasta_location); if !download_path.exists() { create_dir_all
+(&download_path)?; } // create channels. buffer size here is 4 b/c we can do 3
+downloads simultaneously let (send_sigs, recv_sigs) = tokio::sync::mpsc::
+channel::
+Signature>>(4); let (send_failed, recv_failed) = tokio::sync::mpsc::channel::
+(4); // Error channel for handling task errors let (error_sender,
+error_receiver) = tokio::sync::mpsc::channel::(1); // Set up collector/writing
+tasks let mut handles = Vec::new(); let sig_handle = sigwriter_handle
+(recv_sigs, output_sigs, error_sender.clone()); let failures_handle =
+failures_handle(failed_csv, recv_failed, error_sender.clone()); let
+critical_error_flag = Arc::new(AtomicBool::new(false)); let error_handle =
+error_handler(error_receiver, critical_error_flag.clone()); handles.push
+(sig_handle); handles.push(failures_handle); handles.push(error_handle); /
+/ Worker tasks let semaphore = Arc::new(Semaphore::new(3)); // Limiting
+concurrent downloads let client = Arc::new(Client::new()); // Open the file
+containing the accessions synchronously let (accession_info, n_accs) =
+load_accession_info(input_csv, keep_fastas)?; if n_accs == 0 { bail!("No
+accessions to download and sketch.") } // parse param string into params_vec,
+print error if fail let param_result = parse_params_str(param_str); let
+params_vec = match param_result { Ok(params) => params, Err(e) => { bail!
+("Failed to parse params string: {}", e); } }; let dna_sig_templates =
+build_siginfo(&params_vec, "DNA"); let prot_sig_templates = build_siginfo
+(&params_vec, "protein"); let mut genomes_only = false; let mut proteomes_only
+= false; // Check if dna_sig_templates is empty and not keep_fastas if
+dna_sig_templates.is_empty() && !keep_fastas { eprintln!("No DNA signature
+templates provided, and --keep-fastas is not set."); proteomes_only = true; } /
+/ Check if protein_sig_templates is empty and not keep_fastas if
+prot_sig_templates.is_empty() && !keep_fastas { eprintln!("No protein signature
+templates provided, and --keep-fastas is not set."); genomes_only = true; } if
+genomes_only { if !download_only { eprintln!("Downloading and sketching genomes
+only."); } else { eprintln!("Downloading genomes only."); } } else if
+proteomes_only { if !download_only { eprintln!("Downloading and sketching
+proteomes only."); } else { eprintln!("Downloading proteomes only."); } } /
+/ report every 1 percent (or every 1, whichever is larger) let
+reporting_threshold = std::cmp::max(n_accs / 100, 1); for (i, accinfo) in
+accession_info.into_iter().enumerate() { py.check_signals()?; // If
+interrupted, return an Err automatically let semaphore_clone = Arc::clone
+(&semaphore); let client_clone = Arc::clone(&client); let send_sigs =
+send_sigs.clone(); let send_failed = send_failed.clone(); let
+download_path_clone = download_path.clone(); // Clone the path for each task
+let send_errors = error_sender.clone(); let dna_sigs = dna_sig_templates.clone
+(); let prot_sigs = prot_sig_templates.clone(); tokio::spawn(async move { let
+_permit = semaphore_clone.acquire().await; // progress report when the permit
+is available and processing begins if (i + 1) % reporting_threshold == 0 { let
+percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
+println!( "Starting accession {}/{} ({}%)", (i + 1), n_accs, percent_processed
+); } // Perform download and sketch let result = dl_sketch_url( &client_clone,
+accinfo.clone(), &download_path_clone, Some(retry_times), keep_fastas,
+dna_sigs, prot_sigs, genomes_only, proteomes_only, download_only, ) .await;
+match result { Ok((sigs, failed_downloads)) => { if !sigs.is_empty() { if let
+Err(e) = send_sigs.send(sigs).await { eprintln!("Failed to send signatures:
+{}", e); let _ = send_errors.send(e.into()).await; // Send the error through
+the channel } } for fail in failed_downloads { if let Err(e) = send_failed.send
+(fail).await { eprintln!("Failed to send failed download info: {}", e); let _ =
+send_errors.send(e.into()).await; // Send the error through the channel } } }
+Err(e) => { let _ = send_errors.send(e).await; } } drop(send_errors); }); } /
+/ drop senders as we're done sending data drop(send_sigs); drop(send_failed);
+drop(error_sender); // Wait for all tasks to complete for handle in handles
+{ if let Err(e) = handle.await { eprintln!("Handle join error: {}.", e); } } /
+/ since the only critical error is not having written any sigs // check this
+here at end. Bail if we wrote expected sigs but wrote none. if
+critical_error_flag.load(Ordering::SeqCst) & !download_only { bail!("No
+signatures written, exiting."); } Ok(()) }
```

### Comparing `sourmash_plugin_directsketch-0.3.0/src/lib.rs` & `sourmash_plugin_directsketch-0.3.1/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     fasta_location: String,
     keep_fastas: bool,
     genomes_only: bool,
     proteomes_only: bool,
     download_only: bool,
     output_sigs: Option<String>,
 ) -> anyhow::Result<u8> {
-    match directsketch::download_and_sketch(
+    match directsketch::gbsketch(
         py,
         input_csv,
         param_str,
         failed_csv,
         retry_times,
         fasta_location,
         keep_fastas,
@@ -79,13 +79,46 @@
         Err(e) => {
             eprintln!("Error: {e}");
             Ok(1)
         }
     }
 }
 
+#[pyfunction]
+#[allow(clippy::too_many_arguments)]
+fn do_urlsketch(
+    py: Python,
+    input_csv: String,
+    param_str: String,
+    failed_csv: String,
+    retry_times: u32,
+    fasta_location: String,
+    keep_fastas: bool,
+    download_only: bool,
+    output_sigs: Option<String>,
+) -> anyhow::Result<u8> {
+    match directsketch::urlsketch(
+        py,
+        input_csv,
+        param_str,
+        failed_csv,
+        retry_times,
+        fasta_location,
+        keep_fastas,
+        download_only,
+        output_sigs,
+    ) {
+        Ok(_) => Ok(0),
+        Err(e) => {
+            eprintln!("Error: {e}");
+            Ok(1)
+        }
+    }
+}
+
 #[pymodule]
 fn sourmash_plugin_directsketch(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(do_gbsketch, m)?)?;
+    m.add_function(wrap_pyfunction!(do_urlsketch, m)?)?;
     m.add_function(wrap_pyfunction!(set_tokio_thread_pool, m)?)?;
     Ok(())
 }
```

### Comparing `sourmash_plugin_directsketch-0.3.0/src/python/sourmash_plugin_directsketch/__init__.py` & `sourmash_plugin_directsketch-0.3.1/src/python/sourmash_plugin_directsketch/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self, p):
         super().__init__(p)
         p.add_argument('input_csv', help="a txt file or csv file containing accessions in the first column")
         p.add_argument('-o', '--output', default=None,
                        help='output zip file for the signatures')
         p.add_argument('-f', '--fastas',
                        help='Write fastas here', default = '.')
-        p.add_argument('-k', '--keep-fastas', action='store_true',
+        p.add_argument('-k', '--keep-fasta', action='store_true',
                        help="write FASTA files in addition to sketching. Default: do not write FASTA files")
         p.add_argument('--download-only', help='just download genomes; do not sketch', action='store_true')
         p.add_argument('--failed',help='csv of failed accessions and download links (should be mostly protein).')
         p.add_argument('-p', '--param-string', action='append', type=str, default=[],
                           help='parameter string for sketching (default: k=31,scaled=1000)')
         p.add_argument('-c', '--cores', default=0, type=int,
                        help='number of cores to use (default is all available)')
@@ -60,43 +60,108 @@
 
     def main(self, args):
         print_version()
         if not args.param_string:
             args.param_string = ["k=31,scaled=1000"]
         notify(f"params: {args.param_string}")
 
-        if args.download_only and not args.keep_fastas:
-            notify("Error: '--download-only' requires '--keep-fastas'.")
+        if args.download_only and not args.keep_fasta:
+            notify("Error: '--download-only' requires '--keep-fasta'.")
             sys.exit(-1)
         if args.output is None and not args.download_only:
             notify("Error: output signature zipfile is required if not using '--download-only'.")
             sys.exit(-1)
 
         # convert to a single string for easier rust handling
         args.param_string = "_".join(args.param_string)
         # lowercase the param string
         args.param_string = args.param_string.lower()
 
         num_threads = set_thread_pool(args.cores)
 
-        notify(f"downloading and sketching all accessions in '{args.input_csv} using {num_threads} threads")
+        notify(f"downloading and sketching all accessions in '{args.input_csv} using {args.retry_times} retries and {num_threads} threads")
 
         super().main(args)
         status = sourmash_plugin_directsketch.do_gbsketch(args.input_csv,
                                                            args.param_string,
                                                            args.failed,
                                                            args.retry_times,
                                                            args.fastas,
-                                                           args.keep_fastas,
+                                                           args.keep_fasta,
                                                            args.genomes_only,
                                                            args.proteomes_only,
                                                            args.download_only,
                                                            args.output)
         
         if status == 0:
             notify("...gbsketch is done!")
             if args.output is not None:
                 notify(f"Sigs in '{args.output}'.")
-            if args.keep_fastas:
+            if args.keep_fasta:
+                notify(f"FASTAs in '{args.fastas}'.")
+
+        return status
+
+
+class Download_and_Sketch_Url(CommandLinePlugin):
+    command = 'urlsketch'
+    description = 'download and sketch GenBank assembly datasets'
+
+    def __init__(self, p):
+        super().__init__(p)
+        p.add_argument('input_csv', help="a txt file or csv file containing accessions in the first column")
+        p.add_argument('-o', '--output', default=None,
+                       help='output zip file for the signatures')
+        p.add_argument('-f', '--fastas',
+                       help='Write fastas here', default = '.')
+        p.add_argument('-k', '--keep-fasta', '--keep-fastq', action='store_true',
+                       help="write FASTA/Q files in addition to sketching. Default: do not write FASTA files")
+        p.add_argument('--download-only', help='just download genomes; do not sketch', action='store_true')
+        p.add_argument('--failed',help='csv of failed accessions and download links (should be mostly protein).')
+        p.add_argument('-p', '--param-string', action='append', type=str, default=[],
+                          help='parameter string for sketching (default: k=31,scaled=1000)')
+        p.add_argument('-c', '--cores', default=0, type=int,
+                       help='number of cores to use (default is all available)')
+        p.add_argument('-r', '--retry-times', default=1, type=int,
+                       help='number of times to retry failed downloads')
+
+
+    def main(self, args):
+        print_version()
+        if not args.param_string:
+            args.param_string = ["k=31,scaled=1000"]
+        notify(f"params: {args.param_string}")
+
+        if args.download_only and not args.keep_fasta:
+            notify("Error: '--download-only' requires '--keep-fasta'.")
+            sys.exit(-1)
+        if args.output is None and not args.download_only:
+            notify("Error: output signature zipfile is required if not using '--download-only'.")
+            sys.exit(-1)
+
+        # convert to a single string for easier rust handling
+        args.param_string = "_".join(args.param_string)
+        # lowercase the param string
+        args.param_string = args.param_string.lower()
+
+        num_threads = set_thread_pool(args.cores)
+
+        notify(f"downloading and sketching all accessions in '{args.input_csv} using {num_threads} threads")
+
+        super().main(args)
+        status = sourmash_plugin_directsketch.do_urlsketch(args.input_csv,
+                                                           args.param_string,
+                                                           args.failed,
+                                                           args.retry_times,
+                                                           args.fastas,
+                                                           args.keep_fasta,
+                                                           args.download_only,
+                                                           args.output)
+        
+        if status == 0:
+            notify("...gbsketch is done!")
+            if args.output is not None:
+                notify(f"Sigs in '{args.output}'.")
+            if args.keep_fasta:
                 notify(f"FASTAs in '{args.fastas}'.")
 
         return status
```

### Comparing `sourmash_plugin_directsketch-0.3.0/src/utils.rs` & `sourmash_plugin_directsketch-0.3.1/src/utils.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 use anyhow::{anyhow, Result};
 use reqwest::Url;
 use sourmash::cmd::ComputeParameters;
 use sourmash::signature::Signature;
+use std::fmt;
 use std::hash::Hash;
 use std::hash::Hasher;
 
 #[derive(Clone)]
 pub enum InputMolType {
     Dna,
     Protein,
 }
 
+impl InputMolType {}
+
+impl fmt::Display for InputMolType {
+    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
+        match self {
+            InputMolType::Dna => write!(f, "dna"),
+            InputMolType::Protein => write!(f, "protein"),
+        }
+    }
+}
+
 impl std::str::FromStr for InputMolType {
     type Err = ();
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         match s.to_lowercase().as_str() {
             "dna" => Ok(InputMolType::Dna),
             "protein" => Ok(InputMolType::Protein),
@@ -73,17 +85,18 @@
     }
 }
 #[allow(dead_code)]
 #[derive(Clone)]
 pub struct AccessionData {
     pub accession: String,
     pub name: String,
-    pub input_moltype: InputMolType,
+    pub moltype: InputMolType,
     pub url: reqwest::Url,
-    pub md5sum: Option<String>,
+    pub expected_md5sum: Option<String>,
+    pub download_filename: Option<String>, // need to require this if --keep-fastas are used
 }
 
 #[derive(Clone)]
 pub struct GBAssemblyData {
     pub accession: String,
     pub name: String,
     pub url: Option<reqwest::Url>,
@@ -156,27 +169,36 @@
         "Loaded {} rows (including {} rows with valid URL).",
         row_count, url_count
     );
 
     Ok((results, row_count))
 }
 
-#[allow(dead_code)]
-pub fn load_accession_info(input_csv: String) -> Result<(Vec<AccessionData>, usize)> {
+pub fn load_accession_info(
+    input_csv: String,
+    keep_fasta: bool,
+) -> Result<(Vec<AccessionData>, usize)> {
     let mut results = Vec::new();
     let mut row_count = 0;
     let mut processed_rows = std::collections::HashSet::new();
     let mut duplicate_count = 0;
     let mut md5sum_count = 0; // Counter for entries with MD5sum
                               // to do - maybe use HashSet for accessions too to avoid incomplete dupes
     let mut rdr = csv::Reader::from_path(input_csv)?;
 
     // Check column names
     let header = rdr.headers()?;
-    let expected_header = vec!["accession", "name", "input_moltype", "url", "md5sum"];
+    let expected_header = vec![
+        "accession",
+        "name",
+        "moltype",
+        "md5sum",
+        "download_filename",
+        "url",
+    ];
     if header != expected_header {
         return Err(anyhow!(
             "Invalid column names in CSV file. Columns should be: {:?}",
             expected_header
         ));
     }
 
@@ -195,46 +217,50 @@
             .get(0)
             .ok_or_else(|| anyhow!("Missing 'accession' field"))?
             .to_string();
         let name = record
             .get(1)
             .ok_or_else(|| anyhow!("Missing 'name' field"))?
             .to_string();
-        let input_moltype = record
+        let moltype = record
             .get(2)
-            .ok_or_else(|| anyhow!("Missing 'input_moltype' field"))?
+            .ok_or_else(|| anyhow!("Missing 'moltype' field"))?
             .parse::<InputMolType>()
-            .map_err(|_| anyhow!("Invalid 'input_moltype' value"))?;
+            .map_err(|_| anyhow!("Invalid 'moltype' value"))?;
+        let expected_md5sum = record.get(3).map(|s| s.to_string());
+        let download_filename = record.get(4).map(|s| s.to_string());
+        if keep_fasta && download_filename.is_none() {
+            return Err(anyhow!("Missing 'download_filename' field"));
+        }
         let url = record
-            .get(3)
+            .get(5)
             .ok_or_else(|| anyhow!("Missing 'url' field"))?
             .split(',')
             .filter_map(|s| {
                 if s.starts_with("http://") || s.starts_with("https://") || s.starts_with("ftp://")
                 {
                     reqwest::Url::parse(s).ok()
                 } else {
                     None
                 }
             })
             .next()
             .ok_or_else(|| anyhow!("Invalid 'url' value"))?;
-        let md5sum = record.get(4).map(|s| s.to_string());
-
         // count entries with url and md5sum
-        if md5sum.is_some() {
+        if expected_md5sum.is_some() {
             md5sum_count += 1;
         }
         // store accession data
         results.push(AccessionData {
-            accession: acc.to_string(),
-            name: name.to_string(),
-            input_moltype,
+            accession: acc,
+            name,
+            moltype,
             url,
-            md5sum,
+            expected_md5sum,
+            download_filename,
         });
     }
 
     // Print warning if there were duplicated rows.
     if duplicate_count > 0 {
         println!("Warning: {} duplicated rows were skipped.", duplicate_count);
     }
```

### Comparing `sourmash_plugin_directsketch-0.3.0/tests/sourmash_tst_utils.py` & `sourmash_plugin_directsketch-0.3.1/tests/sourmash_tst_utils.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000175535.1.sig.gz` & `sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000175535.1.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000193795.2.sig.gz` & `sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000193795.2.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000961135.2.protein.sig.gz` & `sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000961135.2.protein.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/tests/test-data/GCA_000961135.2.sig.gz` & `sourmash_plugin_directsketch-0.3.1/tests/test-data/GCA_000961135.2.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.3.0/tests/test_gbsketch.py` & `sourmash_plugin_directsketch-0.3.1/tests/test_gbsketch.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,26 @@
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             if sig.minhash.moltype == 'DNA':
                 assert sig.md5sum() == ss2.md5sum()
             else:
                 assert sig.md5sum() == ss3.md5sum()
+    assert os.path.exists(failed)
+    with open(failed, 'r') as failF:
+        fail_lines = failF.readlines()
+        print(fail_lines)
+        assert len(fail_lines) == 2
+        assert fail_lines[0] == "accession,name,moltype,md5sum,download_filename,url\n"
+        acc, name, moltype, md5sum, download_filename, url = fail_lines[1].strip().split(',')
+        assert acc == "GCA_000175535.1"
+        assert name == "GCA_000175535.1 Chlamydia muridarum MopnTet14 (agent of mouse pneumonitis) strain=MopnTet14"
+        assert moltype == "protein"
+        assert download_filename == "GCA_000175535.1_protein.faa.gz"
+        assert url == "https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/175/535/GCA_000175535.1_ASM17553v1/GCA_000175535.1_ASM17553v1_protein.faa.gz"
 
 
 def test_gbsketch_simple_url(runtmp):
     acc_csv = get_test_data('acc-with-ftppath.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
@@ -173,15 +185,15 @@
     for sig in sigs:
         if 'GCA_000175535.1' in sig.name:
             assert sig.name == ss1.name
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             assert sig.md5sum() == ss2.md5sum()
-    assert 'No protein signature templates provided, and --keep-fastas is not set.' in captured.err
+    assert 'No protein signature templates provided, and --keep-fasta is not set.' in captured.err
     assert 'Downloading and sketching genomes only.' in captured.err
 
 
 def test_gbsketch_proteomes_only_via_params(runtmp, capfd):
     acc_csv = get_test_data('acc.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
@@ -202,15 +214,15 @@
     sigs = list(idx.signatures())
     captured = capfd.readouterr()
 
     assert len(sigs) == 1
     for sig in sigs:
         assert 'GCA_000961135.2' in sig.name
         assert sig.md5sum() == ss3.md5sum()
-    assert 'No DNA signature templates provided, and --keep-fastas is not set.' in captured.err
+    assert 'No DNA signature templates provided, and --keep-fasta is not set.' in captured.err
     assert 'Downloading and sketching proteomes only.' in captured.err
 
 
 def test_gbsketch_save_fastas(runtmp):
     acc_csv = get_test_data('acc.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
@@ -222,15 +234,15 @@
     sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
     # why does this need ksize =30 and not ksize = 10!???
     ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
 
     runtmp.sourmash('scripts', 'gbsketch', acc_csv, '-o', output,
-                    '--failed', failed, '-r', '1', '--fastas', out_dir, '--keep-fastas',
+                    '--failed', failed, '-r', '1', '--fastas', out_dir, '--keep-fasta',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
 
     assert os.path.exists(output)
     assert not runtmp.last_result.out # stdout should be empty
     fa_files = os.listdir(out_dir)
     assert set(fa_files) == set(['GCA_000175535.1_genomic.fna.gz', 'GCA_000961135.2_protein.faa.gz', 'GCA_000961135.2_genomic.fna.gz'])
 
@@ -261,23 +273,23 @@
     sig3 = get_test_data('GCA_000961135.2.protein.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
     ss2 = sourmash.load_one_signature(sig2, ksize=31)
     # why does this need ksize =30 and not ksize = 10!???
     ss3 = sourmash.load_one_signature(sig3, ksize=30, select_moltype='protein')
 
     runtmp.sourmash('scripts', 'gbsketch', acc_csv, '--download-only',
-                    '--failed', failed, '-r', '1', '--fastas', out_dir, '--keep-fastas',
+                    '--failed', failed, '-r', '1', '--fastas', out_dir, '--keep-fasta',
                     '--param-str', "dna,k=31,scaled=1000", '-p', "protein,k=10,scaled=200")
 
     assert not runtmp.last_result.out # stdout should be empty
     fa_files = os.listdir(out_dir)
     assert set(fa_files) == set(['GCA_000175535.1_genomic.fna.gz', 'GCA_000961135.2_protein.faa.gz', 'GCA_000961135.2_genomic.fna.gz'])
     captured = capfd.readouterr()
     assert "Failed to send signatures: channel closed" not in captured.err
-   
+
 
 def test_gbsketch_bad_acc(runtmp):
     acc_csv = get_test_data('acc.csv')
     acc_mod = runtmp.output('acc_mod.csv')
     with open(acc_csv, 'r') as inF, open(acc_mod, 'w') as outF:
         lines = inF.readlines()
         for line in lines:
@@ -331,15 +343,15 @@
             assert sig.md5sum() == ss1.md5sum()
         elif 'GCA_000961135.2' in sig.name:
             assert sig.name == ss2.name
             if sig.minhash.moltype == 'DNA':
                 assert sig.md5sum() == ss2.md5sum()
             else:
                 assert sig.md5sum() == ss3.md5sum()
-    
+
 
 def test_gbsketch_missing_accfile(runtmp, capfd):
     acc_csv = runtmp.output('acc1.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
     with pytest.raises(utils.SourmashCommandFailed):
@@ -393,14 +405,15 @@
     captured = capfd.readouterr()
     print(captured.out)
     print(captured.err)
     assert "Error: No signatures written, exiting." in captured.err
 
 
 def test_gbsketch_version_bug(runtmp):
+    # test for bug where we didn't check version correctly
     acc_csv = get_test_data('acc-version.csv')
     output = runtmp.output('simple.zip')
     failed = runtmp.output('failed.csv')
 
     sig1 = get_test_data('GCA_000193795.2.sig.gz')
     ss1 = sourmash.load_one_signature(sig1, ksize=31)
```

### Comparing `sourmash_plugin_directsketch-0.3.0/Cargo.lock` & `sourmash_plugin_directsketch-0.3.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.83"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
@@ -215,17 +215,17 @@
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
 name = "camino"
-version = "1.1.6"
+version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c59e92b5a388f549b863a7bea62612c09f24c8393560709a54558a9abdfb3b9c"
+checksum = "e0ec6b951b160caa93cc0c7b209e5a3bff7aae9062213451ac99493cd844c239"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cc"
 version = "1.0.95"
@@ -1663,26 +1663,26 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.201"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.201"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -1811,15 +1811,15 @@
  "vec-collections",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "sourmash_plugin_directsketch"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "anyhow",
  "async_zip",
  "camino",
  "chrono",
  "csv",
  "futures",
```

### Comparing `sourmash_plugin_directsketch-0.3.0/pyproject.toml` & `sourmash_plugin_directsketch-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 [build-system]
 requires = ["maturin>=1.4.0,<2"]
 build-backend = "maturin"
 
 [project.entry-points."sourmash.cli_script"]
 gbsketch = "sourmash_plugin_directsketch:Download_and_Sketch_Assemblies"
+urlsketch = "sourmash_plugin_directsketch:Download_and_Sketch_Url"
 
 [project.optional-dependencies]
 test = [
   "pytest>=6.2.4,<8.3.0",
   "pytest-cov>=2.12,<6.0",
   "pytest-xdist",
 ]
```

### Comparing `sourmash_plugin_directsketch-0.3.0/PKG-INFO` & `sourmash_plugin_directsketch-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sourmash_plugin_directsketch
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: sourmash >=4.8.5, <5
 Requires-Dist: pytest >=6.2.4, <8.3.0 ; extra == 'test'
 Requires-Dist: pytest-cov >=2.12, <6.0 ; extra == 'test'
 Requires-Dist: pytest-xdist ; extra == 'test'
@@ -14,29 +14,36 @@
 Author: N. Tessa Pierce-Ward
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # sourmash_plugin_directsketch
 
 [![PyPI](https://img.shields.io/pypi/v/sourmash_plugin_directsketch)](https://pypi.org/project/sourmash_plugin_directsketch/)
+[![DOI](https://zenodo.org/badge/792101561.svg)](https://zenodo.org/doi/10.5281/zenodo.11165725)
 
 
-tl;dr - download and sketch NCBI Assembly Datasets by accession
+tl;dr - download and sketch data directly
 
 ## About
 
-This plugin is an attempt to improve database generation by downloading assemblies, checking md5sum, and sketching to a sourmash zipfile. FASTA files can also be saved if desired. It's quite fast, but still very much at alpha level. Here be dragons.
+Commands:
+
+- `gbsketch` - download and sketch NCBI Assembly Datasets by accession
+- `urlsketch` - download and sketch directly from a url
+
+This plugin is an attempt to improve sourmash database generation by downloading files, checking md5sum if provided or accessible, and sketching to a sourmash zipfile. FASTA files can also be saved if desired. It's quite fast, but still very much at alpha level. Here be dragons.
 
 ## Installation
 
 ```
 pip install sourmash_plugin_directsketch
 ```
 
-## Usage
+## `gbsketch`
+download and sketch NCBI Assembly Datasets by accession
 
 ### Create an input file
 
 First, create a file, e.g. `acc.csv` with GenBank identifiers and sketch names.
 ```
 accession,name,ftp_path
 GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-45,
@@ -55,48 +62,100 @@
 - example `ftp_path`: [https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/036/600/915/GCA_036600915.1_ASM3660091v1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/036/600/915/GCA_036600915.1_ASM3660091v1)
 - bacteria assembly summary file: [https://ftp.ncbi.nih.gov/genomes/genbank/bacteria/assembly_summary.txt](https://ftp.ncbi.nih.gov/genomes/genbank/bacteria/assembly_summary.txt)
 
 ### Run:
 
 To run the test accession file at `tests/test-data/acc.csv`, run:
 ```
-sourmash scripts gbsketch tests/test-data/acc.csv -o test.zip -f out_fastas -k --failed test.failed.csv -p dna,k=21,k=31,scaled=1000,abund -p protein,k=10,scaled=100,abund -r 1
+sourmash scripts gbsketch tests/test-data/acc.csv -o test-gbsketch.zip -f out_fastas -k --failed test.failed.csv -p dna,k=21,k=31,scaled=1000,abund -p protein,k=10,scaled=100,abund -r 1
 ```
 
 Full Usage:
 
 ```
-usage:  gbsketch [-h] [-q] [-d] -o OUTPUT [-f FASTAS] [-k] [--download-only] [--failed FAILED] [-p PARAM_STRING] [-c CORES]
-                 [-r RETRY_TIMES] [-g | -m]
-                 input_csv
+usage:  gbsketch [-h] [-q] [-d] [-o OUTPUT] [-f FASTAS] [-k] [--download-only] [--failed FAILED] [-p PARAM_STRING] [-c CORES] [-r RETRY_TIMES] [-g | -m] input_csv
 
 download and sketch GenBank assembly datasets
 
 positional arguments:
   input_csv             a txt file or csv file containing accessions in the first column
 
 options:
   -h, --help            show this help message and exit
   -q, --quiet           suppress non-error output
   -d, --debug           provide debugging output
   -o OUTPUT, --output OUTPUT
                         output zip file for the signatures
   -f FASTAS, --fastas FASTAS
                         Write fastas here
-  -k, --keep-fastas     write FASTA files in addition to sketching. Default: do not write FASTA files
+  -k, --keep-fasta      write FASTA files in addition to sketching. Default: do not write FASTA files
   --download-only       just download genomes; do not sketch
   --failed FAILED       csv of failed accessions and download links (should be mostly protein).
   -p PARAM_STRING, --param-string PARAM_STRING
                         parameter string for sketching (default: k=31,scaled=1000)
   -c CORES, --cores CORES
                         number of cores to use (default is all available)
   -r RETRY_TIMES, --retry-times RETRY_TIMES
                         number of times to retry failed downloads
   -g, --genomes-only    just download and sketch genome (DNA) files
-  -m, --proteomes-only  just download and sketch proteome (protein) files
+```
+
+## `urlsketch`
+download and sketch directly from a url
+### Create an input file
+
+First, create a file, e.g. `acc-url.csv` with identifiers, sketch names, and other required info.
+```
+accession,name,moltype,md5sum,download_filename,url
+GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-454,dna,47b9fb20c51f0552b87db5d44d5d4566,GCA_000961135.2_genomic.urlsketch.fna.gz,https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/961/135/GCA_000961135.2_ASM96113v2/GCA_000961135.2_ASM96113v2_genomic.fna.gz
+GCA_000961135.2,GCA_000961135.2 Candidatus Aramenus sulfurataquae isolate AZ1-454,protein,fb7920fb8f3cf5d6ab9b6b754a5976a4,GCA_000961135.2_protein.urlsketch.faa.gz,https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/961/135/GCA_000961135.2_ASM96113v2/GCA_000961135.2_ASM96113v2_protein.faa.gz
+GCA_000175535.1,GCA_000175535.1 Chlamydia muridarum MopnTet14 (agent of mouse pneumonitis) strain=MopnTet14,dna,a1a8f1c6dc56999c73fe298871c963d1,GCA_000175535.1_genomic.urlsketch.fna.gz,https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/175/535/GCA_000175535.1_ASM17553v1/GCA_000175535.1_ASM17553v1_genomic.fna.gz
+```
+> Six columns must be present:
+> - `accession` - an accession or unique identifier. Ideally no spaces.
+> - `name` - full name for the sketch.
+> - `moltype` - is the file 'dna' or 'protein'?
+> - `md5sum` - expected md5sum (optional, will be checked after download if provided)
+> - `download_filename` - filename for FASTA download. Required if `--keep-fastas`, but useful for signatures, too (saved in sig data).
+> - `url` - direct link for the file
+
+### Run:
+
+To run the test accession file at `tests/test-data/acc-url.csv`, run:
+```
+sourmash scripts urlsketch tests/test-data/acc-url.csv -o test-urlsketch.zip -f out_fastas -k --failed test.failed.csv -p dna,k=21,k=31,scaled=1000,abund -p protein,k=10,scaled=100,abund -r 1
+```
+
+Full Usage:
+```
+usage:  urlsketch [-h] [-q] [-d] [-o OUTPUT] [-f FASTAS] [-k] [--download-only] [--failed FAILED] [-p PARAM_STRING] [-c CORES] [-r RETRY_TIMES] input_csv
+
+download and sketch GenBank assembly datasets
+
+positional arguments:
+  input_csv             a txt file or csv file containing accessions in the first column
+
+options:
+  -h, --help            show this help message and exit
+  -q, --quiet           suppress non-error output
+  -d, --debug           provide debugging output
+  -o OUTPUT, --output OUTPUT
+                        output zip file for the signatures
+  -f FASTAS, --fastas FASTAS
+                        Write fastas here
+  -k, --keep-fasta, --keep-fastq
+                        write FASTA/Q files in addition to sketching. Default: do not write FASTA files
+  --download-only       just download genomes; do not sketch
+  --failed FAILED       csv of failed accessions and download links (should be mostly protein).
+  -p PARAM_STRING, --param-string PARAM_STRING
+                        parameter string for sketching (default: k=31,scaled=1000)
+  -c CORES, --cores CORES
+                        number of cores to use (default is all available)
+  -r RETRY_TIMES, --retry-times RETRY_TIMES
+                        number of times to retry failed downloads
 ```
 
 ## Code of Conduct
 
 This project is under the [sourmash Code of Conduct](https://github.com/sourmash-bio/sourmash/blob/latest/CODE_OF_CONDUCT.rst).
 
 ## Support
```

