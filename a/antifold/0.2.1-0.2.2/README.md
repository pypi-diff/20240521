# Comparing `tmp/antifold-0.2.1.tar.gz` & `tmp/antifold-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antifold-0.2.1.tar", last modified: Tue May 21 16:14:59 2024, max compression
+gzip compressed data, was "antifold-0.2.2.tar", last modified: Tue May 21 16:36:13 2024, max compression
```

## Comparing `antifold-0.2.1.tar` & `antifold-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.997236 antifold-0.2.1/
--rw-r--r--   0 maghoi     (502) staff       (20)     1512 2024-05-13 11:41:55.000000 antifold-0.2.1/LICENSE
--rw-r--r--   0 maghoi     (502) staff       (20)       24 2024-05-21 14:41:16.000000 antifold-0.2.1/MANIFEST.in
--rw-r--r--   0 maghoi     (502) staff       (20)    11944 2024-05-21 16:14:58.996816 antifold-0.2.1/PKG-INFO
--rw-r--r--   0 maghoi     (502) staff       (20)    11465 2024-05-21 16:13:33.000000 antifold-0.2.1/README.md
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.975656 antifold-0.2.1/antifold/
--rw-r--r--   0 maghoi     (502) staff       (20)        0 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/__init__.py
--rw-r--r--   0 maghoi     (502) staff       (20)    26394 2024-05-21 15:01:46.000000 antifold-0.2.1/antifold/antiscripts.py
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.987221 antifold-0.2.1/antifold/esm/
--rw-r--r--   0 maghoi     (502) staff       (20)      238 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/__init__.py
--rw-r--r--   0 maghoi     (502) staff       (20)      371 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/constants.py
--rw-r--r--   0 maghoi     (502) staff       (20)    17438 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/data.py
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.995991 antifold-0.2.1/antifold/esm/inverse_folding/
--rw-r--r--   0 maghoi     (502) staff       (20)      231 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/__init__.py
--rw-r--r--   0 maghoi     (502) staff       (20)    14800 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/features.py
--rw-r--r--   0 maghoi     (502) staff       (20)     1790 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_encoder.py
--rw-r--r--   0 maghoi     (502) staff       (20)    18774 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_modules.py
--rw-r--r--   0 maghoi     (502) staff       (20)     5140 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer.py
--rw-r--r--   0 maghoi     (502) staff       (20)     7232 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer_encoder.py
--rw-r--r--   0 maghoi     (502) staff       (20)     2966 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/gvp_utils.py
--rw-r--r--   0 maghoi     (502) staff       (20)     6113 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/multichain_util.py
--rw-r--r--   0 maghoi     (502) staff       (20)     7569 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/transformer_decoder.py
--rw-r--r--   0 maghoi     (502) staff       (20)    10679 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/transformer_layer.py
--rw-r--r--   0 maghoi     (502) staff       (20)    11715 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/inverse_folding/util.py
--rw-r--r--   0 maghoi     (502) staff       (20)     1883 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/modules.py
--rw-r--r--   0 maghoi     (502) staff       (20)    20748 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/multihead_attention.py
--rw-r--r--   0 maghoi     (502) staff       (20)    14213 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/pretrained.py
--rw-r--r--   0 maghoi     (502) staff       (20)     2785 2024-05-13 11:41:55.000000 antifold-0.2.1/antifold/esm/rotary_embedding.py
--rwxr-xr-x   0 maghoi     (502) staff       (20)    13995 2024-05-21 14:18:58.000000 antifold-0.2.1/antifold/esm_multichain_util_custom.py
--rwxr-xr-x   0 maghoi     (502) staff       (20)    21670 2024-05-21 14:18:54.000000 antifold-0.2.1/antifold/esm_util_custom.py
--rwxr-xr-x   0 maghoi     (502) staff       (20)     9255 2024-05-21 14:18:58.000000 antifold-0.2.1/antifold/if1_dataset.py
--rw-r--r--   0 maghoi     (502) staff       (20)    15248 2024-05-21 15:06:53.000000 antifold-0.2.1/antifold/main.py
-drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:14:58.979258 antifold-0.2.1/antifold.egg-info/
--rw-r--r--   0 maghoi     (502) staff       (20)    11944 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/PKG-INFO
--rw-r--r--   0 maghoi     (502) staff       (20)     1062 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/SOURCES.txt
--rw-r--r--   0 maghoi     (502) staff       (20)        1 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/dependency_links.txt
--rw-r--r--   0 maghoi     (502) staff       (20)       94 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/requires.txt
--rw-r--r--   0 maghoi     (502) staff       (20)        9 2024-05-21 16:14:58.000000 antifold-0.2.1/antifold.egg-info/top_level.txt
--rw-r--r--   0 maghoi     (502) staff       (20)       94 2024-05-13 11:41:55.000000 antifold-0.2.1/requirements.txt
--rw-r--r--   0 maghoi     (502) staff       (20)       38 2024-05-21 16:14:58.997435 antifold-0.2.1/setup.cfg
--rw-r--r--   0 maghoi     (502) staff       (20)      938 2024-05-21 15:09:28.000000 antifold-0.2.1/setup.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:36:13.042080 antifold-0.2.2/
+-rw-r--r--   0 maghoi     (502) staff       (20)     1512 2024-05-13 11:41:55.000000 antifold-0.2.2/LICENSE
+-rw-r--r--   0 maghoi     (502) staff       (20)       24 2024-05-21 14:41:16.000000 antifold-0.2.2/MANIFEST.in
+-rw-r--r--   0 maghoi     (502) staff       (20)    11970 2024-05-21 16:36:12.999278 antifold-0.2.2/PKG-INFO
+-rw-r--r--   0 maghoi     (502) staff       (20)    11491 2024-05-21 16:26:29.000000 antifold-0.2.2/README.md
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:36:12.959416 antifold-0.2.2/antifold/
+-rw-r--r--   0 maghoi     (502) staff       (20)        0 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/__init__.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    26387 2024-05-21 16:35:02.000000 antifold-0.2.2/antifold/antiscripts.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:36:12.969781 antifold-0.2.2/antifold/esm/
+-rw-r--r--   0 maghoi     (502) staff       (20)      238 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/__init__.py
+-rw-r--r--   0 maghoi     (502) staff       (20)      371 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/constants.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    17438 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/data.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:36:12.998507 antifold-0.2.2/antifold/esm/inverse_folding/
+-rw-r--r--   0 maghoi     (502) staff       (20)      231 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/__init__.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    14800 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/features.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     1790 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/gvp_encoder.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    18774 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/gvp_modules.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     5140 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/gvp_transformer.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     7232 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/gvp_transformer_encoder.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     2966 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/gvp_utils.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     6113 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/multichain_util.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     7569 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/transformer_decoder.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    10679 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/transformer_layer.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    11715 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/inverse_folding/util.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     1883 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/modules.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    20748 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/multihead_attention.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    14213 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/pretrained.py
+-rw-r--r--   0 maghoi     (502) staff       (20)     2785 2024-05-13 11:41:55.000000 antifold-0.2.2/antifold/esm/rotary_embedding.py
+-rwxr-xr-x   0 maghoi     (502) staff       (20)    13995 2024-05-21 14:18:58.000000 antifold-0.2.2/antifold/esm_multichain_util_custom.py
+-rwxr-xr-x   0 maghoi     (502) staff       (20)    21670 2024-05-21 14:18:54.000000 antifold-0.2.2/antifold/esm_util_custom.py
+-rwxr-xr-x   0 maghoi     (502) staff       (20)     9255 2024-05-21 14:18:58.000000 antifold-0.2.2/antifold/if1_dataset.py
+-rw-r--r--   0 maghoi     (502) staff       (20)    15248 2024-05-21 15:06:53.000000 antifold-0.2.2/antifold/main.py
+drwxr-xr-x   0 maghoi     (502) staff       (20)        0 2024-05-21 16:36:12.961638 antifold-0.2.2/antifold.egg-info/
+-rw-r--r--   0 maghoi     (502) staff       (20)    11970 2024-05-21 16:36:12.000000 antifold-0.2.2/antifold.egg-info/PKG-INFO
+-rw-r--r--   0 maghoi     (502) staff       (20)     1062 2024-05-21 16:36:12.000000 antifold-0.2.2/antifold.egg-info/SOURCES.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)        1 2024-05-21 16:36:12.000000 antifold-0.2.2/antifold.egg-info/dependency_links.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)       79 2024-05-21 16:36:12.000000 antifold-0.2.2/antifold.egg-info/requires.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)        9 2024-05-21 16:36:12.000000 antifold-0.2.2/antifold.egg-info/top_level.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)       79 2024-05-21 16:25:22.000000 antifold-0.2.2/requirements.txt
+-rw-r--r--   0 maghoi     (502) staff       (20)       38 2024-05-21 16:36:13.042350 antifold-0.2.2/setup.cfg
+-rw-r--r--   0 maghoi     (502) staff       (20)      938 2024-05-21 16:30:49.000000 antifold-0.2.2/setup.py
```

### Comparing `antifold-0.2.1/LICENSE` & `antifold-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/PKG-INFO` & `antifold-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antifold
-Version: 0.2.1
+Version: 0.2.2
 Summary: Inverse folding of antibodies
 Home-page: https://github.com/oxpig/AntiFold/
 Author: Magnus Haraldson Høie & Alissa Hummer
 Author-email: maghoi@dtu.dk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
@@ -28,37 +28,36 @@
 ## Webserver
 
 To try AntiFold without installing it, please see our OPIG webserver:
 [https://opig.stats.ox.ac.uk/webapps/antifold/](https://opig.stats.ox.ac.uk/webapps/antifold/)
 
 ## Install and run AntiFold
 
-
-### Install AntiFold with pip (CPU)
+#### Install AntiFold with pip (CPU)
 ```bash
 conda create --name antifold python=3.10 -y && activate antifold
 pip install antifold
 ```
 
-### Install AntiFold with pip (GPU)
+#### Install AntiFold with pip (GPU)
 ```bash
 conda create --name antifold python=3.10 -y && activate antifold
 conda install -c conda-forge pytorch-gpu
 pip install antifold
 ```
 
-### Download and install from Github source (latest release)
+#### Download and install from Github source (latest release)
 ```bash
 # Download code and model
 git clone https://github.com/oxpig/AntiFold && cd AntiFold
 conda create --name antifold python=3.10 -y && conda activate antifold
 pip install .
 ```
 
-### Run AntiFold (inverse-folding probabilities, sample sequences)
+#### Run AntiFold (inverse-folding probabilities, sample sequences)
 ```bash
 # Run AntiFold on single PDB/CIF file
 # Nb: Assumes first chain heavy, second chain light
 python antifold/main.py \
     --pdb_file data/pdbs/6y1l_imgt.pdb
 
 # Run AntiFold on an antibody-antigen complex
@@ -89,18 +88,20 @@
 
 # Run all chains with ESM-IF1
 python antifold/main.py \
     --pdb_dir data/pdbs \
     --esm_if1_mode
 ```
 
-## Example notebook
+## Jupyter notebook
 Notebook: <a href="https://github.com/oxpig/AntiFold/blob/master/notebook.ipynb">notebook.ipynb</a>
 
 ```python
+!pip install antifold
+
 import antifold
 import antifold.main
 
 # Load model
 model = antifold.main.load_model()
 
 # PDB directory
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: antifold Version: 0.2.1 Summary: Inverse folding of
+Metadata-Version: 2.1 Name: antifold Version: 0.2.2 Summary: Inverse folding of
 antibodies Home-page: https://github.com/oxpig/AntiFold/ Author: Magnus
 Haraldson HÃ¸ie & Alissa Hummer Author-email: maghoi@dtu.dk Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
 License-File: LICENSE AntiFold ============================== AntiFold predicts
 sequences which fit into an input antibody variable domain structure. The tool
@@ -14,39 +14,39 @@
 webserver](https://opig.stats.ox.ac.uk/webapps/antifold/) - Colab (outdated):
 [![Open In Colab](images/colab-badge.svg)](https://colab.research.google.com/
 drive/1TTfgjoZx3mzF5u4e9b4Un9Y7b_rqXc_4) - Model: [model.pt](https://
 opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt) - License: [BSD 3-
 Clause](https://opig.stats.ox.ac.uk/data/downloads/AntiFold/LICENSE) ##
 Webserver To try AntiFold without installing it, please see our OPIG webserver:
 [https://opig.stats.ox.ac.uk/webapps/antifold/](https://opig.stats.ox.ac.uk/
-webapps/antifold/) ## Install and run AntiFold ### Install AntiFold with pip
+webapps/antifold/) ## Install and run AntiFold #### Install AntiFold with pip
 (CPU) ```bash conda create --name antifold python=3.10 -y && activate antifold
-pip install antifold ``` ### Install AntiFold with pip (GPU) ```bash conda
+pip install antifold ``` #### Install AntiFold with pip (GPU) ```bash conda
 create --name antifold python=3.10 -y && activate antifold conda install -
-c conda-forge pytorch-gpu pip install antifold ``` ### Download and install
+c conda-forge pytorch-gpu pip install antifold ``` #### Download and install
 from Github source (latest release) ```bash # Download code and model git clone
 https://github.com/oxpig/AntiFold && cd AntiFold conda create --name antifold
-python=3.10 -y && conda activate antifold pip install . ``` ### Run AntiFold
+python=3.10 -y && conda activate antifold pip install . ``` #### Run AntiFold
 (inverse-folding probabilities, sample sequences) ```bash # Run AntiFold on
 single PDB/CIF file # Nb: Assumes first chain heavy, second chain light python
 antifold/main.py \ --pdb_file data/pdbs/6y1l_imgt.pdb # Run AntiFold on an
 antibody-antigen complex python antifold/main.py \ --pdb_file data/
 antibody_antigen/3hfm.pdb \ --heavy_chain H \ --light_chain L \ --antigen_chain
 Y # Run AntiFold on a folder of PDB/CIFs # Nb: Assumes first chain heavy,
 second light python antifold/main.py \ --pdb_dir data/pdbs # Specify chains to
 run in a CSV file (e.g. antibody-antigen complex) python antifold/main.py \ --
 pdb_dir data/antibody_antigen \ --pdbs_csv data/antibody_antigen.csv # Sample
 sequences 10x python antifold/main.py \ --pdb_file data/pdbs/6y1l_imgt.pdb \ --
 heavy_chain H \ --light_chain L \ --num_seq_per_target 10 \ --sampling_temp
 "0.2" \ --regions "CDR1 CDR2 CDR3" # Run all chains with ESM-IF1 python
-antifold/main.py \ --pdb_dir data/pdbs \ --esm_if1_mode ``` ## Example notebook
-Notebook: _n_o_t_e_b_o_o_k_._i_p_y_n_b ```python import antifold import antifold.main # Load
-model model = antifold.main.load_model() # PDB directory pdb_dir = "data/pdbs"
-# Assumes first chain heavy, second chain light pdbs_csv =
-antifold.main.generate_pdbs_csv(pdb_dir, max_chains=2) # Sample from PDBs
+antifold/main.py \ --pdb_dir data/pdbs \ --esm_if1_mode ``` ## Jupyter notebook
+Notebook: _n_o_t_e_b_o_o_k_._i_p_y_n_b ```python !pip install antifold import antifold import
+antifold.main # Load model model = antifold.main.load_model() # PDB directory
+pdb_dir = "data/pdbs" # Assumes first chain heavy, second chain light pdbs_csv
+= antifold.main.generate_pdbs_csv(pdb_dir, max_chains=2) # Sample from PDBs
 df_logits_list = antifold.main.get_pdbs_logits( model=model,
 pdbs_csv_or_dataframe=pdbs_csv, pdb_dir=pdb_dir, ) # Output log probabilites
 df_logits_list[0] ``` ## Input parameters Required parameters: ```text Input
 PDBs should be antibody variable domain structures (IMGT positions 1-128). If
 no chains are specified, the first two chains will be assumed to be heavy
 light. If custom_chain_mode is set, all (10) chains will be run. - Option 1:
 PDB file (--pdb_file). We recommend specifying heavy and light chain (--
```

### Comparing `antifold-0.2.1/README.md` & `antifold-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,37 +14,36 @@
 ## Webserver
 
 To try AntiFold without installing it, please see our OPIG webserver:
 [https://opig.stats.ox.ac.uk/webapps/antifold/](https://opig.stats.ox.ac.uk/webapps/antifold/)
 
 ## Install and run AntiFold
 
-
-### Install AntiFold with pip (CPU)
+#### Install AntiFold with pip (CPU)
 ```bash
 conda create --name antifold python=3.10 -y && activate antifold
 pip install antifold
 ```
 
-### Install AntiFold with pip (GPU)
+#### Install AntiFold with pip (GPU)
 ```bash
 conda create --name antifold python=3.10 -y && activate antifold
 conda install -c conda-forge pytorch-gpu
 pip install antifold
 ```
 
-### Download and install from Github source (latest release)
+#### Download and install from Github source (latest release)
 ```bash
 # Download code and model
 git clone https://github.com/oxpig/AntiFold && cd AntiFold
 conda create --name antifold python=3.10 -y && conda activate antifold
 pip install .
 ```
 
-### Run AntiFold (inverse-folding probabilities, sample sequences)
+#### Run AntiFold (inverse-folding probabilities, sample sequences)
 ```bash
 # Run AntiFold on single PDB/CIF file
 # Nb: Assumes first chain heavy, second chain light
 python antifold/main.py \
     --pdb_file data/pdbs/6y1l_imgt.pdb
 
 # Run AntiFold on an antibody-antigen complex
@@ -75,18 +74,20 @@
 
 # Run all chains with ESM-IF1
 python antifold/main.py \
     --pdb_dir data/pdbs \
     --esm_if1_mode
 ```
 
-## Example notebook
+## Jupyter notebook
 Notebook: <a href="https://github.com/oxpig/AntiFold/blob/master/notebook.ipynb">notebook.ipynb</a>
 
 ```python
+!pip install antifold
+
 import antifold
 import antifold.main
 
 # Load model
 model = antifold.main.load_model()
 
 # PDB directory
```

#### html2text {}

```diff
@@ -8,39 +8,39 @@
 opig.stats.ox.ac.uk/webapps/antifold/) - Colab (outdated): [![Open In Colab]
 (images/colab-badge.svg)](https://colab.research.google.com/drive/
 1TTfgjoZx3mzF5u4e9b4Un9Y7b_rqXc_4) - Model: [model.pt](https://
 opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt) - License: [BSD 3-
 Clause](https://opig.stats.ox.ac.uk/data/downloads/AntiFold/LICENSE) ##
 Webserver To try AntiFold without installing it, please see our OPIG webserver:
 [https://opig.stats.ox.ac.uk/webapps/antifold/](https://opig.stats.ox.ac.uk/
-webapps/antifold/) ## Install and run AntiFold ### Install AntiFold with pip
+webapps/antifold/) ## Install and run AntiFold #### Install AntiFold with pip
 (CPU) ```bash conda create --name antifold python=3.10 -y && activate antifold
-pip install antifold ``` ### Install AntiFold with pip (GPU) ```bash conda
+pip install antifold ``` #### Install AntiFold with pip (GPU) ```bash conda
 create --name antifold python=3.10 -y && activate antifold conda install -
-c conda-forge pytorch-gpu pip install antifold ``` ### Download and install
+c conda-forge pytorch-gpu pip install antifold ``` #### Download and install
 from Github source (latest release) ```bash # Download code and model git clone
 https://github.com/oxpig/AntiFold && cd AntiFold conda create --name antifold
-python=3.10 -y && conda activate antifold pip install . ``` ### Run AntiFold
+python=3.10 -y && conda activate antifold pip install . ``` #### Run AntiFold
 (inverse-folding probabilities, sample sequences) ```bash # Run AntiFold on
 single PDB/CIF file # Nb: Assumes first chain heavy, second chain light python
 antifold/main.py \ --pdb_file data/pdbs/6y1l_imgt.pdb # Run AntiFold on an
 antibody-antigen complex python antifold/main.py \ --pdb_file data/
 antibody_antigen/3hfm.pdb \ --heavy_chain H \ --light_chain L \ --antigen_chain
 Y # Run AntiFold on a folder of PDB/CIFs # Nb: Assumes first chain heavy,
 second light python antifold/main.py \ --pdb_dir data/pdbs # Specify chains to
 run in a CSV file (e.g. antibody-antigen complex) python antifold/main.py \ --
 pdb_dir data/antibody_antigen \ --pdbs_csv data/antibody_antigen.csv # Sample
 sequences 10x python antifold/main.py \ --pdb_file data/pdbs/6y1l_imgt.pdb \ --
 heavy_chain H \ --light_chain L \ --num_seq_per_target 10 \ --sampling_temp
 "0.2" \ --regions "CDR1 CDR2 CDR3" # Run all chains with ESM-IF1 python
-antifold/main.py \ --pdb_dir data/pdbs \ --esm_if1_mode ``` ## Example notebook
-Notebook: _n_o_t_e_b_o_o_k_._i_p_y_n_b ```python import antifold import antifold.main # Load
-model model = antifold.main.load_model() # PDB directory pdb_dir = "data/pdbs"
-# Assumes first chain heavy, second chain light pdbs_csv =
-antifold.main.generate_pdbs_csv(pdb_dir, max_chains=2) # Sample from PDBs
+antifold/main.py \ --pdb_dir data/pdbs \ --esm_if1_mode ``` ## Jupyter notebook
+Notebook: _n_o_t_e_b_o_o_k_._i_p_y_n_b ```python !pip install antifold import antifold import
+antifold.main # Load model model = antifold.main.load_model() # PDB directory
+pdb_dir = "data/pdbs" # Assumes first chain heavy, second chain light pdbs_csv
+= antifold.main.generate_pdbs_csv(pdb_dir, max_chains=2) # Sample from PDBs
 df_logits_list = antifold.main.get_pdbs_logits( model=model,
 pdbs_csv_or_dataframe=pdbs_csv, pdb_dir=pdb_dir, ) # Output log probabilites
 df_logits_list[0] ``` ## Input parameters Required parameters: ```text Input
 PDBs should be antibody variable domain structures (IMGT positions 1-128). If
 no chains are specified, the first two chains will be assumed to be heavy
 light. If custom_chain_mode is set, all (10) chains will be run. - Option 1:
 PDB file (--pdb_file). We recommend specifying heavy and light chain (--
```

### Comparing `antifold-0.2.1/antifold/antiscripts.py` & `antifold-0.2.2/antifold/antiscripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     model_path = f"{root_dir}/models/model.pt"
 
     if not os.path.exists(model_path):
         log.warning(
             f"Downloading AntiFold model weights to models/model.pt from https://opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt"
         )
         url = "https://opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt"
-        filename = "models/model.pt"
+        filename = model_path
         urllib.request.urlretrieve(url, filename)
 
     if not os.path.exists(model_path) and not checkpoint_path == "ESM-IF1":
         raise Exception(
             f"Unable to find model weights. File does not exist: {checkpoint_path}"
         )
```

### Comparing `antifold-0.2.1/antifold/esm/data.py` & `antifold-0.2.2/antifold/esm/data.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/features.py` & `antifold-0.2.2/antifold/esm/inverse_folding/features.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/gvp_encoder.py` & `antifold-0.2.2/antifold/esm/inverse_folding/gvp_encoder.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/gvp_modules.py` & `antifold-0.2.2/antifold/esm/inverse_folding/gvp_modules.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer.py` & `antifold-0.2.2/antifold/esm/inverse_folding/gvp_transformer.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/gvp_transformer_encoder.py` & `antifold-0.2.2/antifold/esm/inverse_folding/gvp_transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/gvp_utils.py` & `antifold-0.2.2/antifold/esm/inverse_folding/gvp_utils.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/multichain_util.py` & `antifold-0.2.2/antifold/esm/inverse_folding/multichain_util.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/transformer_decoder.py` & `antifold-0.2.2/antifold/esm/inverse_folding/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/transformer_layer.py` & `antifold-0.2.2/antifold/esm/inverse_folding/transformer_layer.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/inverse_folding/util.py` & `antifold-0.2.2/antifold/esm/inverse_folding/util.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/modules.py` & `antifold-0.2.2/antifold/esm/modules.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/multihead_attention.py` & `antifold-0.2.2/antifold/esm/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/pretrained.py` & `antifold-0.2.2/antifold/esm/pretrained.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm/rotary_embedding.py` & `antifold-0.2.2/antifold/esm/rotary_embedding.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm_multichain_util_custom.py` & `antifold-0.2.2/antifold/esm_multichain_util_custom.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/esm_util_custom.py` & `antifold-0.2.2/antifold/esm_util_custom.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/if1_dataset.py` & `antifold-0.2.2/antifold/if1_dataset.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold/main.py` & `antifold-0.2.2/antifold/main.py`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/antifold.egg-info/PKG-INFO` & `antifold-0.2.2/antifold.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antifold
-Version: 0.2.1
+Version: 0.2.2
 Summary: Inverse folding of antibodies
 Home-page: https://github.com/oxpig/AntiFold/
 Author: Magnus Haraldson Høie & Alissa Hummer
 Author-email: maghoi@dtu.dk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
@@ -28,37 +28,36 @@
 ## Webserver
 
 To try AntiFold without installing it, please see our OPIG webserver:
 [https://opig.stats.ox.ac.uk/webapps/antifold/](https://opig.stats.ox.ac.uk/webapps/antifold/)
 
 ## Install and run AntiFold
 
-
-### Install AntiFold with pip (CPU)
+#### Install AntiFold with pip (CPU)
 ```bash
 conda create --name antifold python=3.10 -y && activate antifold
 pip install antifold
 ```
 
-### Install AntiFold with pip (GPU)
+#### Install AntiFold with pip (GPU)
 ```bash
 conda create --name antifold python=3.10 -y && activate antifold
 conda install -c conda-forge pytorch-gpu
 pip install antifold
 ```
 
-### Download and install from Github source (latest release)
+#### Download and install from Github source (latest release)
 ```bash
 # Download code and model
 git clone https://github.com/oxpig/AntiFold && cd AntiFold
 conda create --name antifold python=3.10 -y && conda activate antifold
 pip install .
 ```
 
-### Run AntiFold (inverse-folding probabilities, sample sequences)
+#### Run AntiFold (inverse-folding probabilities, sample sequences)
 ```bash
 # Run AntiFold on single PDB/CIF file
 # Nb: Assumes first chain heavy, second chain light
 python antifold/main.py \
     --pdb_file data/pdbs/6y1l_imgt.pdb
 
 # Run AntiFold on an antibody-antigen complex
@@ -89,18 +88,20 @@
 
 # Run all chains with ESM-IF1
 python antifold/main.py \
     --pdb_dir data/pdbs \
     --esm_if1_mode
 ```
 
-## Example notebook
+## Jupyter notebook
 Notebook: <a href="https://github.com/oxpig/AntiFold/blob/master/notebook.ipynb">notebook.ipynb</a>
 
 ```python
+!pip install antifold
+
 import antifold
 import antifold.main
 
 # Load model
 model = antifold.main.load_model()
 
 # PDB directory
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: antifold Version: 0.2.1 Summary: Inverse folding of
+Metadata-Version: 2.1 Name: antifold Version: 0.2.2 Summary: Inverse folding of
 antibodies Home-page: https://github.com/oxpig/AntiFold/ Author: Magnus
 Haraldson HÃ¸ie & Alissa Hummer Author-email: maghoi@dtu.dk Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Science/Research Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3.10 Description-Content-Type: text/markdown
 License-File: LICENSE AntiFold ============================== AntiFold predicts
 sequences which fit into an input antibody variable domain structure. The tool
@@ -14,39 +14,39 @@
 webserver](https://opig.stats.ox.ac.uk/webapps/antifold/) - Colab (outdated):
 [![Open In Colab](images/colab-badge.svg)](https://colab.research.google.com/
 drive/1TTfgjoZx3mzF5u4e9b4Un9Y7b_rqXc_4) - Model: [model.pt](https://
 opig.stats.ox.ac.uk/data/downloads/AntiFold/models/model.pt) - License: [BSD 3-
 Clause](https://opig.stats.ox.ac.uk/data/downloads/AntiFold/LICENSE) ##
 Webserver To try AntiFold without installing it, please see our OPIG webserver:
 [https://opig.stats.ox.ac.uk/webapps/antifold/](https://opig.stats.ox.ac.uk/
-webapps/antifold/) ## Install and run AntiFold ### Install AntiFold with pip
+webapps/antifold/) ## Install and run AntiFold #### Install AntiFold with pip
 (CPU) ```bash conda create --name antifold python=3.10 -y && activate antifold
-pip install antifold ``` ### Install AntiFold with pip (GPU) ```bash conda
+pip install antifold ``` #### Install AntiFold with pip (GPU) ```bash conda
 create --name antifold python=3.10 -y && activate antifold conda install -
-c conda-forge pytorch-gpu pip install antifold ``` ### Download and install
+c conda-forge pytorch-gpu pip install antifold ``` #### Download and install
 from Github source (latest release) ```bash # Download code and model git clone
 https://github.com/oxpig/AntiFold && cd AntiFold conda create --name antifold
-python=3.10 -y && conda activate antifold pip install . ``` ### Run AntiFold
+python=3.10 -y && conda activate antifold pip install . ``` #### Run AntiFold
 (inverse-folding probabilities, sample sequences) ```bash # Run AntiFold on
 single PDB/CIF file # Nb: Assumes first chain heavy, second chain light python
 antifold/main.py \ --pdb_file data/pdbs/6y1l_imgt.pdb # Run AntiFold on an
 antibody-antigen complex python antifold/main.py \ --pdb_file data/
 antibody_antigen/3hfm.pdb \ --heavy_chain H \ --light_chain L \ --antigen_chain
 Y # Run AntiFold on a folder of PDB/CIFs # Nb: Assumes first chain heavy,
 second light python antifold/main.py \ --pdb_dir data/pdbs # Specify chains to
 run in a CSV file (e.g. antibody-antigen complex) python antifold/main.py \ --
 pdb_dir data/antibody_antigen \ --pdbs_csv data/antibody_antigen.csv # Sample
 sequences 10x python antifold/main.py \ --pdb_file data/pdbs/6y1l_imgt.pdb \ --
 heavy_chain H \ --light_chain L \ --num_seq_per_target 10 \ --sampling_temp
 "0.2" \ --regions "CDR1 CDR2 CDR3" # Run all chains with ESM-IF1 python
-antifold/main.py \ --pdb_dir data/pdbs \ --esm_if1_mode ``` ## Example notebook
-Notebook: _n_o_t_e_b_o_o_k_._i_p_y_n_b ```python import antifold import antifold.main # Load
-model model = antifold.main.load_model() # PDB directory pdb_dir = "data/pdbs"
-# Assumes first chain heavy, second chain light pdbs_csv =
-antifold.main.generate_pdbs_csv(pdb_dir, max_chains=2) # Sample from PDBs
+antifold/main.py \ --pdb_dir data/pdbs \ --esm_if1_mode ``` ## Jupyter notebook
+Notebook: _n_o_t_e_b_o_o_k_._i_p_y_n_b ```python !pip install antifold import antifold import
+antifold.main # Load model model = antifold.main.load_model() # PDB directory
+pdb_dir = "data/pdbs" # Assumes first chain heavy, second chain light pdbs_csv
+= antifold.main.generate_pdbs_csv(pdb_dir, max_chains=2) # Sample from PDBs
 df_logits_list = antifold.main.get_pdbs_logits( model=model,
 pdbs_csv_or_dataframe=pdbs_csv, pdb_dir=pdb_dir, ) # Output log probabilites
 df_logits_list[0] ``` ## Input parameters Required parameters: ```text Input
 PDBs should be antibody variable domain structures (IMGT positions 1-128). If
 no chains are specified, the first two chains will be assumed to be heavy
 light. If custom_chain_mode is set, all (10) chains will be run. - Option 1:
 PDB file (--pdb_file). We recommend specifying heavy and light chain (--
```

### Comparing `antifold-0.2.1/antifold.egg-info/SOURCES.txt` & `antifold-0.2.2/antifold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antifold-0.2.1/setup.py` & `antifold-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(
     name="antifold",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     description="Inverse folding of antibodies",
     url="https://github.com/oxpig/AntiFold/",
     author="Magnus Haraldson Høie & Alissa Hummer",
     author_email="maghoi@dtu.dk",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

