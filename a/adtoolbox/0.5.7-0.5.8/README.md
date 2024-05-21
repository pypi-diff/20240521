# Comparing `tmp/adtoolbox-0.5.7.tar.gz` & `tmp/adtoolbox-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.5.7.tar", max compression
+gzip compressed data, was "adtoolbox-0.5.8.tar", max compression
```

## Comparing `adtoolbox-0.5.7.tar` & `adtoolbox-0.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      988 2024-05-09 04:21:15.185160 adtoolbox-0.5.7/README.md
--rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.7/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.7/adtoolbox/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.7/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.7/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.7/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.7/adtoolbox/cli.py
--rw-r--r--   0        0        0    16613 2024-05-15 15:55:16.214048 adtoolbox-0.5.7/adtoolbox/configs.py
--rw-r--r--   0        0        0   109451 2024-05-15 17:41:17.396046 adtoolbox-0.5.7/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.7/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.7/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.7/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.7/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.7/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0      864 2024-05-15 19:39:10.537774 adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0      920 2024-05-15 19:45:02.263654 adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.7/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.7/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.7/adtoolbox/tables.py
--rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.7/adtoolbox/utils.py
--rw-r--r--   0        0        0      748 2024-05-15 19:52:55.322828 adtoolbox-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     4420 2024-05-15 19:53:04.395268 adtoolbox-0.5.7/setup.py
--rw-r--r--   0        0        0     1961 2024-05-15 19:53:04.395592 adtoolbox-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      988 2024-05-09 04:21:15.185160 adtoolbox-0.5.8/README.md
+-rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.8/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.8/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.8/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.8/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.8/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.8/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16660 2024-05-20 16:45:36.910045 adtoolbox-0.5.8/adtoolbox/configs.py
+-rw-r--r--   0        0        0   110142 2024-05-21 19:48:16.265314 adtoolbox-0.5.8/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.8/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.8/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.8/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.8/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.8/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0      864 2024-05-15 19:39:10.537774 adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0      920 2024-05-15 19:45:02.263654 adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.8/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.8/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.8/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15972 2024-05-20 19:34:44.781887 adtoolbox-0.5.8/adtoolbox/utils.py
+-rw-r--r--   0        0        0      768 2024-05-21 20:34:26.806580 adtoolbox-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     4448 2024-05-21 20:34:36.616119 adtoolbox-0.5.8/setup.py
+-rw-r--r--   0        0        0     2003 2024-05-21 20:34:36.616315 adtoolbox-0.5.8/PKG-INFO
```

### Comparing `adtoolbox-0.5.7/README.md` & `adtoolbox-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/.DS_Store` & `adtoolbox-0.5.8/adtoolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/__init__.py` & `adtoolbox-0.5.8/adtoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/adm.py` & `adtoolbox-0.5.8/adtoolbox/adm.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/bio_struct.py` & `adtoolbox-0.5.8/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/cli.py` & `adtoolbox-0.5.8/adtoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/configs.py` & `adtoolbox-0.5.8/adtoolbox/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from adtoolbox import Main_Dir,PKG_DATA
+from adtoolbox import Main_Dir, PKG_DATA
 import pathlib
 import rich
 import json
 import warnings
 
 """
 This module contains all the paths to the files and directories used in the program.
@@ -12,29 +12,30 @@
 
 
 RXN_DB = os.path.join(Main_Dir, "Database", "Reaction_Metadata.csv")
 
 Seed_RXN_DB = os.path.join(Main_Dir, "Database", "reactions.json")
 Seed_COMPOUNDS_DB = os.path.join(Main_Dir, "Database", "compounds.json")
 
-ADTOOLBOX_CONTAINERS={
-	'docker_x86':"parsaghadermazi/adtoolbox:x86",
-	'docker_arm64':"parsaghadermazi/adtoolbox:arm64",
-	'singularity_x86':"docker://parsaghadermazi/adtoolbox:x86",
-	'singularity_arm64':"docker://parsaghadermazi/adtoolbox:arm64"}
-
-E_ADM_2_REMOTE={
-	"model_parameters":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_model_parameters.json",
-	"base_parameters":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_base_parameters.json",
-	"initial_conditions":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_initial_conditions.json",
-	"inlet_conditions":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_inlet_conditions.json",
-	"reactions":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_reactions.json",
-	"species":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_species.json"
-			}
-E_ADM_2_LOCAL={
+ADTOOLBOX_CONTAINERS = {
+    'docker_x86': "parsaghadermazi/adtoolbox:x86",
+    'docker_arm64': "parsaghadermazi/adtoolbox:arm64",
+    'singularity_x86': "docker://parsaghadermazi/adtoolbox:x86",
+    'singularity_arm64': "docker://parsaghadermazi/adtoolbox:arm64"}
+
+E_ADM_2_REMOTE = {
+   "model_parameters": "https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_model_parameters.json",
+   "base_parameters": "https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_base_parameters.json",
+   "initial_conditions": "https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_initial_conditions.json",
+   "inlet_conditions": "https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_inlet_conditions.json",
+   "reactions": "https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_reactions.json",
+   "species": "https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/e_adm_2/e_adm_2_species.json"
+                 }
+
+E_ADM_2_LOCAL = {
 	"model_parameters":os.path.join(Main_Dir, "Database","ADM_Parameters","e_adm_2_model_parameters.json"),
 	"base_parameters":os.path.join(Main_Dir, "Database","ADM_Parameters","e_adm_2_base_parameters.json"),
 	"initial_conditions":os.path.join(Main_Dir, "Database","ADM_Parameters","e_adm_2_initial_conditions.json"),
 	"inlet_conditions":os.path.join(Main_Dir, "Database","ADM_Parameters","e_adm_2_inlet_conditions.json"),
 	"reactions":os.path.join(Main_Dir, "Database","ADM_Parameters","e_adm_2_reactions.json"),
 	"species":os.path.join(Main_Dir, "Database","ADM_Parameters","e_adm_2_species.json"),	
 }
@@ -219,15 +220,15 @@
             bit_score=40,
             e_value=10**-5,
             qiime2_docker_image="quay.io/qiime2/core:2022.2",
             qiime2_singularity_image="docker://quay.io/qiime2/core:2022.2",
             qiime2_paired_end_bash_str=os.path.join(PKG_DATA,"qiime_template_paired.txt"),
             qiime2_single_end_bash_str=os.path.join(PKG_DATA,"qiime_template_single.txt"),
 			qiime_classifier_db=Database().qiime_classifier_db,
-			adm_mapping=Database().adm_microbial_groups_mapping,
+			adm_mapping=E_ADM_MICROBIAL_GROUPS_MAPPING,
 			qiime2_p_trunc_len:tuple[int,int]=("250","250"),
              ):
 		self.k = amplicon2genome_k
 		self.vsearch_similarity = vsearch_similarity
 		self.align_to_gtdb_outputs_dir = align_to_gtdb_outputs_dir
 		self.amplicon2genome_db = amplicon2genome_db
 		self.qiime_outputs_dir = qiime_outputs_dir
```

### Comparing `adtoolbox-0.5.7/adtoolbox/core.py` & `adtoolbox-0.5.8/adtoolbox/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                    fasta_to_dict,
                    extract_zipped_file,
                    needs_repair,
                    create_mmseqs_database,
                    index_mmseqs_db,
                    mmseqs_search,
                    mmseqs_result_db_to_tsv) 
+import polars as pl
 # import doctest
 # doctest.testmod(verbose=True, optionflags=doctest.ELLIPSIS)
 
             
 @dataclass
 class Experiment:
     """
@@ -1648,15 +1649,15 @@
         
         Args:
             save (bool, optional): Whether to save the json file or not. Defaults to True.
         """
         matches = os.path.join(alignment_dir,'matches.blast')
         aligned=pd.read_table(matches,header=None,delimiter='\t')
         aligned.drop_duplicates(0,inplace=True)
-        aligned[1]=aligned[1].apply(lambda x: ("".join(x.split('_')[1:])).split("~")[0])
+        aligned[1]=aligned[1].apply(lambda x: ("_".join(x.split('_')[1:])).split("~")[0])
         alignment_dict=dict(zip(aligned[0],aligned[1]))
 
         
         return alignment_dict
     
     
     def download_genome(self,identifier:str,output_dir:str,container:str="None")-> str:
@@ -1868,19 +1869,22 @@
         Args:
             alignment_file (str): The address of the alignment file.
         
         Returns:
             dict: A dictionary of EC numbers and their counts.
 
         """
-        alignment_table = pd.read_table(alignment_file,sep='\t')
-        alignment_table = alignment_table[(alignment_table['evalue']<self.config.e_value)&(alignment_table['bits']>self.config.bit_score)]
-        alignment_table["target"]=alignment_table["target"].apply(lambda x:x.split("|")[1])
-        ec_counts=alignment_table["target"].value_counts().to_dict()
-        return ec_counts
+        df=(pl.scan_csv(alignment_file, separator='\t',) 
+        .filter((pl.col("evalue") < self.config.e_value)&(pl.col("bits") >self.config.bit_score))
+        .with_columns((pl.col("target").str.split_exact("|",1).struct[1].alias("EC")))
+        .unique(["query","EC"],keep="first")
+        .groupby("EC")
+        .count()
+        ).collect(streaming=True)
+        return pd.DataFrame(df.to_dicts()).set_index("EC").to_dict()["count"]
     
     def get_cod_from_ec_counts(self,ec_counts:dict)->dict:
         """This function takes a json file that comtains ec counts and converts it to ADM microbial agents counts.
         Required Configs:
             config.adm_mapping : A dictionary that maps ADM reactions to ADM microbial agents.
             ---------
             config.csv_reaction_db : The address of the reaction database of ADToolbox.
@@ -2014,15 +2018,22 @@
             fasterq_dump_script+=f"\nfasterq-dump {sra_file} -O {acc_folder} --split-files"
             fasterq_dump_script+=f"\nrm {sra_file}"
             
             prefetch_script+=fasterq_dump_script
  
         
         elif container=="docker":
-            warn("Docker is not supported yet")
+            prefetch_script=f"""#!/bin/bash\n"""
+            prefetch_script+=f"docker run -v {target_dir}:{target_dir} {self.config.adtoolbox_docker} prefetch {accession} -O {target_dir}\n"
+            acc_folder=pathlib.Path(target_dir)/accession
+            fasterq_dump_script=""
+            sra_file=acc_folder/(accession+".sra")
+            fasterq_dump_script+=f"docker run -v {target_dir}:{target_dir} {self.config.adtoolbox_docker} fasterq-dump {sra_file} -O {acc_folder} --split-files\n"
+            fasterq_dump_script+=f"docker run -v {target_dir}:{target_dir} {self.config.adtoolbox_docker} rm {sra_file}"
+            prefetch_script+=fasterq_dump_script
        
         sample_metadata=utils.get_sample_metadata_from_accession(accession)      
             
         
         return prefetch_script,sample_metadata
```

### Comparing `adtoolbox-0.5.7/adtoolbox/metagenomics_report.py` & `adtoolbox-0.5.8/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/optimize.py` & `adtoolbox-0.5.8/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pipeline.py` & `adtoolbox-0.5.8/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.5.8/adtoolbox/pkg_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pkg_data/README.md` & `adtoolbox-0.5.8/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/stats.py` & `adtoolbox-0.5.8/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/tables.py` & `adtoolbox-0.5.8/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.7/adtoolbox/utils.py` & `adtoolbox-0.5.8/adtoolbox/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,37 +45,38 @@
 
 
 
 
 
 
 
-def wrap_for_slurm(command:str,run:bool,save:bool,config:configs.Utils())->str:
+def wrap_for_slurm(command:str,jobname:str,run:bool,save:bool,config:configs.Utils)->str:
     """
     This is a function that wraps a bash script in a slurm script.
     All resource allocation configuration is obtained from config argument
     Args:
         command: bash command to run in python string format
         run: if True, the slurm script is executed
+        jobname: the name of the job to be submitted
         save: if True, the slurm script is saved to the path specified in config
         config: Configs.Utils object that detemines the template form and slurm options
     
     Returns:
         The slurm script as a string
     """
     with open(config.slurm_template,'r') as f:
         slurm_template = f.read()
     
     command = command.replace("#!/bin/bash","") 
     slurm_script = slurm_template.replace("<command>",command)
-    slurm_script = slurm_script.replace("<sample_name>",config.slurm_job_name)
+    slurm_script = slurm_script.replace("<sample_name>",jobname)
     slurm_script = slurm_script.replace("<wall_time>",config.slurm_wall_time)
     slurm_script = slurm_script.replace("<executer>",config.slurm_executer)
-    slurm_script = slurm_script.replace("<job_name>",config.slurm_job_name)
-    slurm_script = slurm_script.replace("<sample_outlog>",config.slurm_outlog)
+    slurm_script = slurm_script.replace("<job_name>",jobname)
+    slurm_script = slurm_script.replace("<sample_outlog>",jobname)
     slurm_script = slurm_script.replace("<memory>",config.slurm_memory)
     slurm_script = slurm_script.replace("<cpus>",config.slurm_cpus)
     
     if save:
         with open(config.slurm_save_dir,'w') as f:
             f.write(slurm_script)
 
@@ -136,30 +137,31 @@
         script=f"singularity exec -B {input_file}:{input_file} {configs.adtoolbox_singularity} gzip -d {input_file}"
         
     elif container =="docker":
         script=f"docker run -v {input_file}:{input_file} {configs.adtoolbox_docker} gzip -d {input_file}"
         
     return script,
 
+
 def generate_batch_script(
-    generator_function:callable,
-    number_of_batches:int,
-    input_series:list[list],
-    input_var:list[str],
-    container:str="None",
-    save:Union[str,None]=None,
-    run:bool=False,
-    header:str="#!/bin/bash\n",
-    **kwargs)->tuple:
+    generator_function: callable,
+    number_of_batches: int,
+    input_series: list[list],
+    input_var: list[str],
+    container: str = "None",
+    save: Union[str, None] = None,
+    run: bool = False,
+    header: str = "#!/bin/bash\n",
+    **kwargs) -> tuple:
     """
     This is a general function that generates an iterable of bash scripts for running a function
     that creates a bash script on an iterable of inputs.
     
     """
-    batch_size = len(list(zip(*input_series)))//number_of_batches+1
+    batch_size = len(list(zip(*input_series)))//number_of_batches
     batches=[]
     for i in range(len(input_series)):
         batches.append([input_series[i][j:j+batch_size] for j in range(0,len(input_series[i]),batch_size)])
     scripts=[]
     
     for inputs in zip(*batches):
         script=header
```

### Comparing `adtoolbox-0.5.7/pyproject.toml` & `adtoolbox-0.5.8/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.5.7"
+version = "0.5.8"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
@@ -15,14 +15,15 @@
 rich = "^12.4.4"
 scipy = "^1.8.1"
 sympy = "^1.10.1"
 matplotlib = "^3.5.2"
 dash-escher = "^0.0.4"
 openbox = "^0.7.17"
 dash-bootstrap-components = "^1.3.1"
+polars = "^0.20.27"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `adtoolbox-0.5.7/setup.py` & `adtoolbox-0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,25 +62,26 @@
  'dash-escher>=0.0.4,<0.0.5',
  'dash>=2.4.1,<3.0.0',
  'matplotlib>=3.5.2,<4.0.0',
  'numpy>=1.22.4,<2.0.0',
  'openbox>=0.7.17,<0.8.0',
  'pandas>=1.4.2,<2.0.0',
  'plotly>=5.8.0,<6.0.0',
+ 'polars>=0.20.27,<0.21.0',
  'requests>=2.27.1,<3.0.0',
  'rich>=12.4.4,<13.0.0',
  'scipy>=1.8.1,<2.0.0',
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.5.7',
+    'version': '0.5.8',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
     'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)\n\n***NOTE***:Binder implementations don\'t offer escher map functionalities yet.\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `adtoolbox-0.5.7/PKG-INFO` & `adtoolbox-0.5.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.5.7
+Version: 0.5.8
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Requires-Dist: dash-bootstrap-components (>=1.3.1,<2.0.0)
 Requires-Dist: dash-escher (>=0.0.4,<0.0.5)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: openbox (>=0.7.17,<0.8.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: plotly (>=5.8.0,<6.0.0)
+Requires-Dist: polars (>=0.20.27,<0.21.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: sympy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Toolbox Overview
```

