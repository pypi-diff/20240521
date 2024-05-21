# Comparing `tmp/VASP2KP-1.1.3.tar.gz` & `tmp/VASP2KP-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VASP2KP-1.1.3.tar", last modified: Tue Apr 16 10:48:40 2024, max compression
+gzip compressed data, was "VASP2KP-1.1.4.tar", last modified: Tue May 21 07:03:40 2024, max compression
```

## Comparing `VASP2KP-1.1.3.tar` & `VASP2KP-1.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-16 10:48:40.839028 VASP2KP-1.1.3/
--rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.3/LICENSE.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-16 10:48:40.838780 VASP2KP-1.1.3/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.3/README.md
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-16 10:48:40.837091 VASP2KP-1.1.3/VASP2KP/
--rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.3/VASP2KP/__init__.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.3/VASP2KP/_get_kp_Zeeman.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.3/VASP2KP/_numeric_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    52731 2024-04-16 10:22:04.000000 VASP2KP-1.1.3/VASP2KP/_read_data.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    91234 2024-04-13 14:23:44.000000 VASP2KP-1.1.3/VASP2KP/_standard_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.3/VASP2KP/_transform_matrix.py
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-16 10:48:40.838487 VASP2KP-1.1.3/VASP2KP.egg-info/
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/SOURCES.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/dependency_links.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/not-zip-safe
--rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/requires.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/top_level.txt
--rwxrwxrwx   0 shengzhang   (501) staff       (20)     8664 2024-04-16 10:47:09.000000 VASP2KP-1.1.3/mat2kp
--rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-04-16 10:48:40.839083 VASP2KP-1.1.3/setup.cfg
--rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-04-16 10:47:33.000000 VASP2KP-1.1.3/setup.py
--rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.3/vasp2mat.5.3-patch-1.0.1.sh
--rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.3/vasp2mat.6.4-patch-1.0.1.sh
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-21 07:03:40.152186 VASP2KP-1.1.4/
+-rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.4/LICENSE.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-05-21 07:03:40.151936 VASP2KP-1.1.4/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.4/README.md
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-21 07:03:40.150195 VASP2KP-1.1.4/VASP2KP/
+-rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.4/VASP2KP/__init__.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.4/VASP2KP/_get_kp_Zeeman.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.4/VASP2KP/_numeric_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    52754 2024-05-20 16:00:24.000000 VASP2KP-1.1.4/VASP2KP/_read_data.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    91476 2024-05-21 07:00:58.000000 VASP2KP-1.1.4/VASP2KP/_standard_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.4/VASP2KP/_transform_matrix.py
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-21 07:03:40.151666 VASP2KP-1.1.4/VASP2KP.egg-info/
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/SOURCES.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/dependency_links.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-16 10:48:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/not-zip-safe
+-rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/requires.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/top_level.txt
+-rwxrwxrwx   0 shengzhang   (501) staff       (20)     9688 2024-04-18 02:00:28.000000 VASP2KP-1.1.4/mat2kp
+-rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-05-21 07:03:40.152245 VASP2KP-1.1.4/setup.cfg
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-05-21 07:03:24.000000 VASP2KP-1.1.4/setup.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.4/vasp2mat.5.3-patch-1.0.1.sh
+-rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.4/vasp2mat.6.4-patch-1.0.1.sh
```

### Comparing `VASP2KP-1.1.3/LICENSE.txt` & `VASP2KP-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/PKG-INFO` & `VASP2KP-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.3
+Version: 1.1.4
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.3/README.md` & `VASP2KP-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/VASP2KP/__init__.py` & `VASP2KP-1.1.4/VASP2KP/__init__.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/VASP2KP/_get_kp_Zeeman.py` & `VASP2KP-1.1.4/VASP2KP/_get_kp_Zeeman.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/VASP2KP/_numeric_kp.py` & `VASP2KP-1.1.4/VASP2KP/_numeric_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/VASP2KP/_read_data.py` & `VASP2KP-1.1.4/VASP2KP/_read_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,15 @@
     try:
         file = open(os.path.join(folder_path,"MAT_Pi.m"),'r')
     except:
         try:
             file = open(os.path.join(folder_path,"MAT_pi.m",'r'))
         except:
             print("ERROR: Cannot fild the file 'MAT_Pi.m'!")
+            sys.exit()
     file.readline()
     file.readline()
     kpoints = file.readline().strip().split(' ')
     file.close()
     
     while '' in kpoints:
         kpoints.remove('')
```

### Comparing `VASP2KP-1.1.3/VASP2KP/_standard_kp.py` & `VASP2KP-1.1.4/VASP2KP/_standard_kp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1069,31 +1069,32 @@
     if print_flag != 0:
         print('\n==========  Result of Zeeman\'s coupling  ==========')
     
     # fixing the bug in kdotp-generator
     try:
         warnings.filterwarnings("ignore", category=DeprecationWarning)
         np.complex
-        warnings.resetwarnings()
+        warnings.filterwarnings('default')
         
     except:
-        warnings.resetwarnings()
+        warnings.filterwarnings('default')
         np.complex = np.complex128
         
     # use kdotp-generator to generate the analytical Zeeman's coupling based on invariant theory
-    
+    warnings.filterwarnings("ignore", category=DeprecationWarning)
     kpmodel, irrep_expr_basis, irrep_repr_basis = kp.symmetric_hamiltonian(
                 sym_ops,
                 kp_variable = 'B',
                 order = [1],
                 repr_basis = 'pauli',
                 msg_num = msg_num,
                 kvec = kvec
             )   
-    
+    warnings.filterwarnings('default')
+
     if print_flag == 2:
         sys.stdout = outfile
         
     else:
         sys.stdout = save_stdout
      
     # removal of duplicates
@@ -1689,38 +1690,39 @@
     coe_sym = []
     coe_sym_ = []
     
     # fixing the bug in kdotp-generator
     try:
         warnings.filterwarnings("ignore", category=DeprecationWarning)
         np.complex
-        warnings.resetwarnings()
+        warnings.filterwarnings('default')
         
     except:
-        warnings.resetwarnings()
+        warnings.filterwarnings('default')
         np.complex = np.complex128
     
     for order in order_list:
         
         # Redirect the output stream to the log file 
         # the function kp.symmetric_hamiltonian will output some information
         sys.stdout = logging
         
         print('\n==========  Result of order = %s  =========='%(str(order)))
         
         # use kdotp-generator to generate the analytical kp hamiltonian based on invariant theory
+        warnings.filterwarnings("ignore", category=DeprecationWarning)
         kpmodel, irrep_expr_basis, irrep_repr_basis = kp.symmetric_hamiltonian(
                 sym_ops,
                 kp_variable = 'k',
                 order = order,
                 repr_basis = 'pauli',
                 msg_num = msg_num,
                 kvec = kvec
             )
-        
+        warnings.filterwarnings('default')
             
         
         if print_flag == 2:
             sys.stdout = outfile
             
         else:
             sys.stdout = save_stdout
```

### Comparing `VASP2KP-1.1.3/VASP2KP/_transform_matrix.py` & `VASP2KP-1.1.4/VASP2KP/_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/VASP2KP.egg-info/PKG-INFO` & `VASP2KP-1.1.4/VASP2KP.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.3
+Version: 1.1.4
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.3/mat2kp` & `VASP2KP-1.1.4/mat2kp`

 * *Files 7% similar despite different names*

```diff
@@ -83,17 +83,29 @@
                 line = line.replace(line[start:end],string)
         
         input_list.append(line)
     
     input_inf = '\n'.join(input_list)
 
 
-
+try:
 # execute
-exec(input_inf)
+    exec(input_inf)
+except ValueError as ve:
+    if str(ve) == 'mismatched dimensions':
+        print("ERROR: At least one matrices in 'Symmetry' is not square matrix! Please check and rewrite it!")
+        sys.exit()
+    else:
+        print("An exception occurred:", ve)
+        print("ERROR: There are some typos in mat2kp.in. Please check!")
+        sys.exit()
+except Exception as e:
+    print("An exception occurred:", e)
+    print("ERROR: There are some typos in mat2kp.in. Please check!")
+    sys.exit()
 
 locals_key = list(locals().keys())
 locals_key_low = []
 
 for i in range(len(locals_key)):
     locals_key_low.append(locals_key[i].lower())
 
@@ -229,18 +241,26 @@
     if no_vasp_kp:
         result_kp, result_Zeeman = \
         get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log, repr_split = repr_split)
     
     else:
         result_kp, result_Zeeman = \
         get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc, repr_split = repr_split)
-
-except:
+# except ValueError as ve:
+#     if ve == 'mismatched dimensions':
+#         print("ERROR: At least one matrices in 'Symmetry' is not square matrix! Please check and rewrite it!")
+#     else:
+#         print("An exception occurred:", ve)
+#         print("The program unexpectedly encountered an error. We kindly ask you to send us a screenshot of the error and the input files. Email: zhangsheng221@mails.ucas.ac.cn/wzj@iphy.ac.cn")
+#         sys.exit()
+    
+except Exception as e:
+    print("An exception occurred:", e)
     print("The program unexpectedly encountered an error. We kindly ask you to send us a screenshot of the error and the input files. Email: zhangsheng221@mails.ucas.ac.cn/wzj@iphy.ac.cn")
-
+    sys.exit()
 else:
     print("Congratulations! The computation of VASP2KP has finished!!!")
 
 
 if gfactor == 1 and (not no_vasp_kp) and mathematica_flag:
     mathematica_file = open("kp-Zeeman.nb",'w')
     mathematica_file.write(r'Clear["Global`*"];')
```

### Comparing `VASP2KP-1.1.3/setup.py` & `VASP2KP-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 README = """A tool for computing k.p effective Hamiltonians and Zeeman's coupling under given symmetry constraints from VASP calculations."""
 
 
 setup(name='VASP2KP',
       python_requires=">=3.6",
-      version = "1.1.3",
+      version = "1.1.4",
       long_description=README,
       install_requires=[
         'sympy', 'numpy', 'scipy', 'kdotp_generator'
         ],
       packages=['VASP2KP'],
       author = 'Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang',
       author_email='zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn',
```

### Comparing `VASP2KP-1.1.3/vasp2mat.5.3-patch-1.0.1.sh` & `VASP2KP-1.1.4/vasp2mat.5.3-patch-1.0.1.sh`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.3/vasp2mat.6.4-patch-1.0.1.sh` & `VASP2KP-1.1.4/vasp2mat.6.4-patch-1.0.1.sh`

 * *Files identical despite different names*

