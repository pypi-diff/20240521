# Comparing `tmp/nanoCEM-0.0.5.9.tar.gz` & `tmp/nanoCEM-0.0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoCEM-0.0.5.9.tar", last modified: Mon May 13 03:58:27 2024, max compression
+gzip compressed data, was "nanoCEM-0.0.6.0.tar", last modified: Tue May 21 03:07:43 2024, max compression
```

## Comparing `nanoCEM-0.0.5.9.tar` & `nanoCEM-0.0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2024-04-30 05:56:15.000000 nanoCEM-0.0.5.9/LICENSE
--rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-04-30 05:56:15.000000 nanoCEM-0.0.5.9/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15657 2024-04-30 05:57:13.000000 nanoCEM-0.0.5.9/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3973 2024-05-03 02:57:20.000000 nanoCEM-0.0.5.9/nanoCEM/alignment_magnifier
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    14799 2024-05-13 03:24:07.000000 nanoCEM-0.0.5.9/nanoCEM/cem_utils.py
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10833 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3597 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/machine_learning_trainer.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_f5c_eventalign.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_move_table.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-04-30 05:56:16.000000 nanoCEM-0.0.5.9/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/nanoCEM.egg-info/
--rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      545 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-05-13 03:58:27.000000 nanoCEM-0.0.5.9/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-05-13 03:58:27.013821 nanoCEM-0.0.5.9/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-05-13 03:57:30.000000 nanoCEM-0.0.5.9/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-21 03:07:43.925960 nanoCEM-0.0.6.0/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2024-04-30 05:56:15.000000 nanoCEM-0.0.6.0/LICENSE
+-rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-21 03:07:43.924960 nanoCEM-0.0.6.0/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-04-30 05:56:15.000000 nanoCEM-0.0.6.0/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-21 03:07:43.924960 nanoCEM-0.0.6.0/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15657 2024-04-30 05:57:13.000000 nanoCEM-0.0.6.0/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3973 2024-05-03 02:57:20.000000 nanoCEM-0.0.6.0/nanoCEM/alignment_magnifier
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    14865 2024-05-21 03:07:40.000000 nanoCEM-0.0.6.0/nanoCEM/cem_utils.py
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10833 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3597 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/machine_learning_trainer.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_f5c_eventalign.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_move_table.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-21 03:07:43.924960 nanoCEM-0.0.6.0/nanoCEM.egg-info/
+-rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      545 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-05-21 03:07:43.925960 nanoCEM-0.0.6.0/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-05-21 03:03:56.000000 nanoCEM-0.0.6.0/setup.py
```

### Comparing `nanoCEM-0.0.5.9/LICENSE` & `nanoCEM-0.0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/PKG-INFO` & `nanoCEM-0.0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.9
+Version: 0.0.6.0
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.9 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.6.0 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.5.9/README.md` & `nanoCEM-0.0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.6.0/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/alignment_magnifier` & `nanoCEM-0.0.6.0/nanoCEM/alignment_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/cem_utils.py` & `nanoCEM-0.0.6.0/nanoCEM/cem_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 base_shift_dict ={
     'r9RNA+': -1,
     'r9RNA-': -3,
     'r9DNA+': -2,
     'r9DNA-': -3,
     'r10DNA+': -6,
     'r10DNA-': -2,
-    'rna004RNA+': -2,
-    'rna004RNA-': -6,
+    'rna004RNA+': -3,
+    'rna004RNA-': -5,
 }
 
 def caculate_base_shift_size(kmer_model,strand):
     def is_odd(number):
         if number % 2 == 0:
             return False
         else:
@@ -98,14 +98,16 @@
 
     if subsample_ratio < 1:
         new_bam = '.'.join(fastq_file.split('.')[:-1]) + '_sub.bam'
         cmds = "samtools view -hbS -s " +str(subsample_ratio) +' ' + bam_file +' > ' + new_bam
         print(cmds)
         run_cmd(cmds)
         bam_file = new_bam
+        cmds = 'samtools index ' + bam_file
+        run_cmd(cmds)
 
     if not os.path.exists(bam_file+'.bai'):
         cmds = 'samtools index ' + bam_file
         run_cmd(cmds)
 
     new_fastq_file = '.'.join(bam_file.split('.')[:-1]) + '.fastq'
     if not os.path.exists(new_fastq_file):
```

### Comparing `nanoCEM-0.0.5.9/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.6.0/nanoCEM/current_events_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.6.0/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/machine_learning_trainer.py` & `nanoCEM-0.0.6.0/nanoCEM/machine_learning_trainer.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/normalization.py` & `nanoCEM-0.0.6.0/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/plot.py` & `nanoCEM-0.0.6.0/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/read_f5c_eventalign.py` & `nanoCEM-0.0.6.0/nanoCEM/read_f5c_eventalign.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.6.0/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/read_move_table.py` & `nanoCEM-0.0.6.0/nanoCEM/read_move_table.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.6.0/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.6.0/nanoCEM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.9
+Version: 0.0.6.0
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.9 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.6.0 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.5.9/nanoCEM.egg-info/SOURCES.txt` & `nanoCEM-0.0.6.0/nanoCEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.9/setup.py` & `nanoCEM-0.0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.5.9",
+    version="0.0.6.0",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

