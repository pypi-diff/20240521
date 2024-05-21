# Comparing `tmp/boss_runs-0.1.0.tar.gz` & `tmp/boss_runs-0.1.1.tar.gz`

## Comparing `boss_runs-0.1.0.tar` & `boss_runs-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 boss_runs-0.1.0/.gitattributes
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 boss_runs-0.1.0/.gitmodules
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/BOSS.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/__init__.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/_cli_base.py
--rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/batch.py
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/config.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/core.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/dependencies.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/live.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/mapper.py
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/paf.py
--rw-r--r--   0        0        0    20816 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/readfish_boss.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/readlengthdist.py
--rw-r--r--   0        0        0    16675 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/sampler.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/aeons/__init__.py
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/aeons/core.py
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/aeons/kmer.py
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/aeons/repeats.py
--rw-r--r--   0        0        0    59481 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/aeons/sequences.py
--rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/aeons/simulation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/__init__.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/abundance_tracker.py
--rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/core.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/readstartdist.py
--rw-r--r--   0        0        0    12557 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/reference.py
--rw-r--r--   0        0        0    33447 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/sequences.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 boss_runs-0.1.0/boss/runs/simulation.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boss_runs-0.1.0/scripts/check_manager_connection.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 boss_runs-0.1.0/scripts/mappy_index_fasta.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 boss_runs-0.1.0/scripts/prepare_simulation_data.smk
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 boss_runs-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 boss_runs-0.1.0/LICENSE
--rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 boss_runs-0.1.0/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 boss_runs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 boss_runs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 boss_runs-0.1.1/.directory
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 boss_runs-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 boss_runs-0.1.1/.gitmodules
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/BOSS.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/__init__.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/_cli_base.py
+-rw-r--r--   0        0        0    10546 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/batch.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/config.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/core.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/dependencies.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/live.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/mapper.py
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/paf.py
+-rw-r--r--   0        0        0    20816 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/readfish_boss.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/readlengthdist.py
+-rw-r--r--   0        0        0    16675 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/sampler.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/aeons/__init__.py
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/aeons/core.py
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/aeons/kmer.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/aeons/repeats.py
+-rw-r--r--   0        0        0    59481 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/aeons/sequences.py
+-rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/aeons/simulation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/__init__.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/abundance_tracker.py
+-rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/core.py
+-rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/readstartdist.py
+-rw-r--r--   0        0        0    12557 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/reference.py
+-rw-r--r--   0        0        0    33447 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/sequences.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 boss_runs-0.1.1/boss/runs/simulation.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 boss_runs-0.1.1/scripts/check_manager_connection.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 boss_runs-0.1.1/scripts/mappy_index_fasta.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 boss_runs-0.1.1/scripts/prepare_simulation_data.smk
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 boss_runs-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 boss_runs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8494 2020-02-02 00:00:00.000000 boss_runs-0.1.1/README.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 boss_runs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 boss_runs-0.1.1/PKG-INFO
```

### Comparing `boss_runs-0.1.0/boss/BOSS.py` & `boss_runs-0.1.1/boss/BOSS.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/_cli_base.py` & `boss_runs-0.1.1/boss/_cli_base.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/batch.py` & `boss_runs-0.1.1/boss/batch.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/config.py` & `boss_runs-0.1.1/boss/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         ref = ""                        # reference file (fasta or None). Not specifying a file switches to AEONS
         mmi = ""                        # index of reference (will be built if ref is given but not mmi)
         
         [live]
         device = "TEST"                 # position on sequencer
         host = "localhost"              # host of sequencing device
         port = 9502                     # port of sequencing device
-        data_wait = 100                 # wait for X Mb data before first update
-        prom = false
+        data_wait = 100                 # wait for X Mb of data before first update
+        prom = false                    # switch for using a PromethION flowcell (experimental)
 
         [optional]
         reject_refs = ""                # comma-separated list of headers in reference from which to always reject
         ploidy = 1                      # 1 or 2
         lowcov = 10                     # target coverage for assemblies
         temperature = 60                # max updates during which to consider fragments (higher number might decrease update speeds)
         min_seq_len = 2500              # min sequence length used during contig reconstruction
```

### Comparing `boss_runs-0.1.0/boss/core.py` & `boss_runs-0.1.1/boss/core.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/dependencies.py` & `boss_runs-0.1.1/boss/dependencies.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/live.py` & `boss_runs-0.1.1/boss/live.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/mapper.py` & `boss_runs-0.1.1/boss/mapper.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/paf.py` & `boss_runs-0.1.1/boss/paf.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/readfish_boss.py` & `boss_runs-0.1.1/boss/readfish_boss.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/readlengthdist.py` & `boss_runs-0.1.1/boss/readlengthdist.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/sampler.py` & `boss_runs-0.1.1/boss/sampler.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/utils.py` & `boss_runs-0.1.1/boss/utils.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/aeons/core.py` & `boss_runs-0.1.1/boss/aeons/core.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/aeons/kmer.py` & `boss_runs-0.1.1/boss/aeons/kmer.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/aeons/repeats.py` & `boss_runs-0.1.1/boss/aeons/repeats.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/aeons/sequences.py` & `boss_runs-0.1.1/boss/aeons/sequences.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/aeons/simulation.py` & `boss_runs-0.1.1/boss/aeons/simulation.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/runs/abundance_tracker.py` & `boss_runs-0.1.1/boss/runs/abundance_tracker.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/runs/core.py` & `boss_runs-0.1.1/boss/runs/core.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/runs/readstartdist.py` & `boss_runs-0.1.1/boss/runs/readstartdist.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/runs/reference.py` & `boss_runs-0.1.1/boss/runs/reference.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/runs/sequences.py` & `boss_runs-0.1.1/boss/runs/sequences.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/boss/runs/simulation.py` & `boss_runs-0.1.1/boss/runs/simulation.py`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/scripts/prepare_simulation_data.smk` & `boss_runs-0.1.1/scripts/prepare_simulation_data.smk`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/.gitignore` & `boss_runs-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/LICENSE` & `boss_runs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `boss_runs-0.1.0/README.md` & `boss_runs-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# <img src=doc/BR_logo.png width="500" />
+# <img src=doc/BR_logo.png width="350" />
 
 
 *B*enefit-*O*ptimising *S*hort-term *S*trategies for *R*ead*U*ntil *N*anopore *S*equencing
 
 
 BOSS* strategies allow for dynamic, adaptive sampling during nanopore sequencing. New data is periodically ingested to 
 generate updated decision strategies in order to maximise the information gain during the sequencing experiment.
 [Readfish](https://github.com/LooseLab/readfish) is launched to run alongside and communicates the rejection signals 
 to the sequencing machine. 
 
+
 The method is described in this [article](https://doi.org/10.1038/s41587-022-01580-z)
 
 
 
+
 <p align="center">
 	<img src=doc/BR_flowchart.png width="500" />
 </p>
 
 
 
 
@@ -33,17 +35,15 @@
 
 Recommended way of installing our software is in a conda/mamba environment. 
 These commands will create an environment and install BOSS* alongside the necessary dependencies. 
 
 
 ```shell
 mamba create -n boss python=3.10 pip gfatools minimap2 miniasm && mamba activate boss   
-pip install dist/boss_runs-0.1.0-py3-none-any.whl
-
-pip install dist/boss_runs-0.1.0-py3-none-any.whl --force-reinstall --no-deps
+pip install boss_runs
 ```
 
 
 
 ## Usage
 
 BOSS* can be used in different ways depending on the aim of the sequencing experiment.
@@ -69,15 +69,16 @@
 [optional]
 reject_refs = ""                # comma-separated list of headers in reference from which to always reject
 ploidy = 1                      # 1 or 2
 ```
 
 
 By default, all whole genome(s) included in the input fasta file are considered of interest at the beginning of the experiment. 
-It is possible to reject all reads from specific sequences in a fasta file. For this, provide fasta headers of the reference file, e.g.: `--reject_refs 1,2,3,X,Y,MT`
+It is possible to reject all reads from specific sequences in a fasta file. 
+For this, provide fasta headers of the reference file, e.g.: `--reject_refs 1,2,3,X,Y,MT`
 
 
 
 ### Configuring readfish
 
 A separate toml file needs to be given to BOSS that contains the configuration of readfish (according to [their instructions](https://github.com/LooseLab/readfish/blob/main/docs/toml.md))
 
@@ -128,57 +129,46 @@
 
 
 
 ### Starting BOSS*
 
 After sequencing has started launch BOSS* with:
 
-```
-./BOSS.py --toml path/to/toml --toml_readfish path/to/readfish/toml
+```shell
+boss --toml path/to/toml --toml_readfish path/to/readfish/toml
 ```
 
 
 BOSS* will initialise and start to periodically generate new decision strategies from the sequencing reads deposited by the sequencer.
 If readfish is configured properly, the strategies will be reloaded automatically.
 This triggers a message in readfish's logfile similar to: `Reloaded strategies for X sequences`.
 
-When enough data is collected, BOSS-RUNS can be stopped by a keyboard interrupt (Ctrl+C).
+When enough data is collected, BOSS* can be stopped by a keyboard interrupt (Ctrl+C).
 
 
 
 ## Testing
 
 
 It is highly recommended to follow the [walkthrough provided in the readfish repository](https://github.com/LooseLab/readfish/tree/main?tab=readme-ov-file#testing)
 to set up a playback experiment and test the functionality and interplay of the software and sequencing machine.
 
-As soon as playback is running, BOSS* can be executed using these toml files:
+As soon as playback is running, BOSS* can be executed using toml files located in `tests/config`:
 
-TODO
-```
---ref /data/Homo_sapiens.GRCh38.dna_sm.primary_assembly.fa
---ref_idx /data/Homo_sapiens.GRCh38.dna_sm.primary_assembly.fa.mmi 
---reject_refs 1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,21,22,X,Y,MT 
+
+```shell
+boss --toml tests/config/boss_ch20.toml --toml_readfish tests/config/boss_ch20_readfish.toml
 ``` 
               
+This configures targeting of chromosome 20 with continuously updated decision strategies.
+Let the playback sequencing run for a few minutes, then verify that the setup works:
 
-`../BOSS.py --toml ./config/`
-
-
-This configures targeting of chromosome 20 and to continuously updated decision strategies
-
-
-Let the playback sequencing run for a few minutes.
-
+1) `readfish` is rejecting reads from all chromosomes, except for #20. For this, look at the observed read lengths:
 
-Then there are 2 things to verify that the setup works:
-
-1) `readfish` is rejecting reads from all chromosomes, except for #20. For this, we look at the observed read lengths:
-
-`readfish summary readfish_test.toml /path/to/sequencing/output/fastq_pass/`
+`readfish summary tests/config/boss_ch20_readfish.toml /path/to/sequencing/output/fastq_pass/`
 
 
 Check that the mean read length for the enriched chromosome is larger than for the remaining chromosomes.   
 (In this example the read lengths of depleted chromosomes are still rather long due to slow base calling) 
 
 
 
@@ -205,53 +195,51 @@
      6     656  1013424  231  118194   5819   1545     599   7268
      7    1026   932717  185   66384   2972    909     563    914
      8     906  1133194  210  162732   5930   1251     564   2210
      9    1046  1533653  200  248867   9656   1466     552   8059
     MT      19   143721  591   16467   6140   7564    6809  13257
      X    1515  1490398  199  132776   4652    984     526   1014
      Y       9     6531  427    1895    475    726     517    628
-
 ```
 
 
 2) `readfish` is using dynamically updated decision strategies
 
-for this, we can simply grep the log-file of `readfish` for all reloading events of updated strategies.
+for this, grep the log-file of `readfish` for all reloading events of updated strategies.
 
-```
+```shell 
 grep "Reloaded" readfish.log
-```
-
-This should produce an output similar to this, showing the periodic updates:
-
-
-```
-TODO
+#2024-03-06 17:06:39,179 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:07:07,994 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:07:37,818 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:08:38,902 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:09:07,365 readfish.targets Reloaded strategies for 24 sequences
+# ...
 ```
 
 
-
-
 ## Issues, questions, suggestions ...
 
 Please use the issue tracker in this repository to get in touch!
+Notes for development and code organisation can be found in `doc/developer_noted.md` 
 
 
 ## Citation
 
 
 ```
 @article{weilgunyDynamicAdaptiveSampling2023,
   title = {Dynamic, adaptive sampling during nanopore sequencing using {{Bayesian}} experimental design},
   author = {Weilguny, Lukas and De Maio, Nicola and Munro, Rory and Manser, Charlotte and Birney, Ewan and Loose, Matthew and Goldman, Nick},
   year = {2023},
   journal = {Nature Biotechnology},
   publisher = {{Nature Publishing Group}},
   doi = {10.1038/s41587-022-01580-z}
 }
+
 ```
 
 
 ## License
 
 Licensed under GPLv3
```

### Comparing `boss_runs-0.1.0/pyproject.toml` & `boss_runs-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 [project]
 name = "boss_runs"
 description = "Dynamic, adaptive sampling during nanopore sequencing"
 dynamic = ["version"]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
-    "readfish[all]",
+    "readfish[all]==2023.1.1",
     "Bottleneck~=1.3.7",
     "scipy~=1.12.0",
     "numba~=0.59.0",
 ]
 
 
+[project.urls]
+homepage = "https://github.com/goldman-gp-ebi/BOSS-RUNS/"
+
+
 [project.optional-dependencies]
 dev = [
     "pytest~=8.0.0",
     "pytest-cov~=4.1.0",
     "pytest-timeout~=2.2.0",
 ]
```

### Comparing `boss_runs-0.1.0/PKG-INFO` & `boss_runs-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: boss_runs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic, adaptive sampling during nanopore sequencing
+Project-URL: homepage, https://github.com/goldman-gp-ebi/BOSS-RUNS/
 License-File: LICENSE
 Requires-Python: >=3.10
 Requires-Dist: bottleneck~=1.3.7
 Requires-Dist: numba~=0.59.0
-Requires-Dist: readfish[all]
+Requires-Dist: readfish[all]==2023.1.1
 Requires-Dist: scipy~=1.12.0
 Provides-Extra: dev
 Requires-Dist: pytest-cov~=4.1.0; extra == 'dev'
 Requires-Dist: pytest-timeout~=2.2.0; extra == 'dev'
 Requires-Dist: pytest~=8.0.0; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# <img src=doc/BR_logo.png width="500" />
+# <img src=doc/BR_logo.png width="350" />
 
 
 *B*enefit-*O*ptimising *S*hort-term *S*trategies for *R*ead*U*ntil *N*anopore *S*equencing
 
 
 BOSS* strategies allow for dynamic, adaptive sampling during nanopore sequencing. New data is periodically ingested to 
 generate updated decision strategies in order to maximise the information gain during the sequencing experiment.
 [Readfish](https://github.com/LooseLab/readfish) is launched to run alongside and communicates the rejection signals 
 to the sequencing machine. 
 
+
 The method is described in this [article](https://doi.org/10.1038/s41587-022-01580-z)
 
 
 
+
 <p align="center">
 	<img src=doc/BR_flowchart.png width="500" />
 </p>
 
 
 
 
@@ -49,17 +52,15 @@
 
 Recommended way of installing our software is in a conda/mamba environment. 
 These commands will create an environment and install BOSS* alongside the necessary dependencies. 
 
 
 ```shell
 mamba create -n boss python=3.10 pip gfatools minimap2 miniasm && mamba activate boss   
-pip install dist/boss_runs-0.1.0-py3-none-any.whl
-
-pip install dist/boss_runs-0.1.0-py3-none-any.whl --force-reinstall --no-deps
+pip install boss_runs
 ```
 
 
 
 ## Usage
 
 BOSS* can be used in different ways depending on the aim of the sequencing experiment.
@@ -85,15 +86,16 @@
 [optional]
 reject_refs = ""                # comma-separated list of headers in reference from which to always reject
 ploidy = 1                      # 1 or 2
 ```
 
 
 By default, all whole genome(s) included in the input fasta file are considered of interest at the beginning of the experiment. 
-It is possible to reject all reads from specific sequences in a fasta file. For this, provide fasta headers of the reference file, e.g.: `--reject_refs 1,2,3,X,Y,MT`
+It is possible to reject all reads from specific sequences in a fasta file. 
+For this, provide fasta headers of the reference file, e.g.: `--reject_refs 1,2,3,X,Y,MT`
 
 
 
 ### Configuring readfish
 
 A separate toml file needs to be given to BOSS that contains the configuration of readfish (according to [their instructions](https://github.com/LooseLab/readfish/blob/main/docs/toml.md))
 
@@ -144,57 +146,46 @@
 
 
 
 ### Starting BOSS*
 
 After sequencing has started launch BOSS* with:
 
-```
-./BOSS.py --toml path/to/toml --toml_readfish path/to/readfish/toml
+```shell
+boss --toml path/to/toml --toml_readfish path/to/readfish/toml
 ```
 
 
 BOSS* will initialise and start to periodically generate new decision strategies from the sequencing reads deposited by the sequencer.
 If readfish is configured properly, the strategies will be reloaded automatically.
 This triggers a message in readfish's logfile similar to: `Reloaded strategies for X sequences`.
 
-When enough data is collected, BOSS-RUNS can be stopped by a keyboard interrupt (Ctrl+C).
+When enough data is collected, BOSS* can be stopped by a keyboard interrupt (Ctrl+C).
 
 
 
 ## Testing
 
 
 It is highly recommended to follow the [walkthrough provided in the readfish repository](https://github.com/LooseLab/readfish/tree/main?tab=readme-ov-file#testing)
 to set up a playback experiment and test the functionality and interplay of the software and sequencing machine.
 
-As soon as playback is running, BOSS* can be executed using these toml files:
+As soon as playback is running, BOSS* can be executed using toml files located in `tests/config`:
 
-TODO
-```
---ref /data/Homo_sapiens.GRCh38.dna_sm.primary_assembly.fa
---ref_idx /data/Homo_sapiens.GRCh38.dna_sm.primary_assembly.fa.mmi 
---reject_refs 1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,21,22,X,Y,MT 
+
+```shell
+boss --toml tests/config/boss_ch20.toml --toml_readfish tests/config/boss_ch20_readfish.toml
 ``` 
               
+This configures targeting of chromosome 20 with continuously updated decision strategies.
+Let the playback sequencing run for a few minutes, then verify that the setup works:
 
-`../BOSS.py --toml ./config/`
-
-
-This configures targeting of chromosome 20 and to continuously updated decision strategies
-
-
-Let the playback sequencing run for a few minutes.
-
+1) `readfish` is rejecting reads from all chromosomes, except for #20. For this, look at the observed read lengths:
 
-Then there are 2 things to verify that the setup works:
-
-1) `readfish` is rejecting reads from all chromosomes, except for #20. For this, we look at the observed read lengths:
-
-`readfish summary readfish_test.toml /path/to/sequencing/output/fastq_pass/`
+`readfish summary tests/config/boss_ch20_readfish.toml /path/to/sequencing/output/fastq_pass/`
 
 
 Check that the mean read length for the enriched chromosome is larger than for the remaining chromosomes.   
 (In this example the read lengths of depleted chromosomes are still rather long due to slow base calling) 
 
 
 
@@ -221,53 +212,51 @@
      6     656  1013424  231  118194   5819   1545     599   7268
      7    1026   932717  185   66384   2972    909     563    914
      8     906  1133194  210  162732   5930   1251     564   2210
      9    1046  1533653  200  248867   9656   1466     552   8059
     MT      19   143721  591   16467   6140   7564    6809  13257
      X    1515  1490398  199  132776   4652    984     526   1014
      Y       9     6531  427    1895    475    726     517    628
-
 ```
 
 
 2) `readfish` is using dynamically updated decision strategies
 
-for this, we can simply grep the log-file of `readfish` for all reloading events of updated strategies.
+for this, grep the log-file of `readfish` for all reloading events of updated strategies.
 
-```
+```shell 
 grep "Reloaded" readfish.log
-```
-
-This should produce an output similar to this, showing the periodic updates:
-
-
-```
-TODO
+#2024-03-06 17:06:39,179 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:07:07,994 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:07:37,818 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:08:38,902 readfish.targets Reloaded strategies for 24 sequences
+#2024-03-06 17:09:07,365 readfish.targets Reloaded strategies for 24 sequences
+# ...
 ```
 
 
-
-
 ## Issues, questions, suggestions ...
 
 Please use the issue tracker in this repository to get in touch!
+Notes for development and code organisation can be found in `doc/developer_noted.md` 
 
 
 ## Citation
 
 
 ```
 @article{weilgunyDynamicAdaptiveSampling2023,
   title = {Dynamic, adaptive sampling during nanopore sequencing using {{Bayesian}} experimental design},
   author = {Weilguny, Lukas and De Maio, Nicola and Munro, Rory and Manser, Charlotte and Birney, Ewan and Loose, Matthew and Goldman, Nick},
   year = {2023},
   journal = {Nature Biotechnology},
   publisher = {{Nature Publishing Group}},
   doi = {10.1038/s41587-022-01580-z}
 }
+
 ```
 
 
 ## License
 
 Licensed under GPLv3
```

