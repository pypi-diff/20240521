# Comparing `tmp/vbpy-2.0.7.tar.gz` & `tmp/vbpy-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.0.7.tar", last modified: Fri May 17 02:21:35 2024, max compression
+gzip compressed data, was "vbpy-2.0.8.tar", last modified: Tue May 21 07:54:37 2024, max compression
```

## Comparing `vbpy-2.0.7.tar` & `vbpy-2.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 02:21:35.680000 vbpy-2.0.7/
--rw-rw-rw-   0        0        0      122 2024-05-17 02:21:36.000000 vbpy-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-17 02:21:36.000000 vbpy-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-17 02:21:32.000000 vbpy-2.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:21:35.720000 vbpy-2.0.7/vbpy/
--rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.7/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.7/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0    18573 2024-05-17 02:21:14.000000 vbpy-2.0.7/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.7/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-17 02:21:35.760000 vbpy-2.0.7/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-17 02:21:36.000000 vbpy-2.0.7/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-17 02:21:36.000000 vbpy-2.0.7/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 02:21:36.000000 vbpy-2.0.7/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-17 02:21:36.000000 vbpy-2.0.7/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 07:54:37.680000 vbpy-2.0.8/
+-rw-rw-rw-   0        0        0      122 2024-05-21 07:54:38.000000 vbpy-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-21 07:54:38.000000 vbpy-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-21 07:53:58.000000 vbpy-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:54:37.710000 vbpy-2.0.8/vbpy/
+-rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.8/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.8/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0    17970 2024-05-21 07:53:50.000000 vbpy-2.0.8/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.8/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:54:37.750000 vbpy-2.0.8/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.0.7/setup.py` & `vbpy-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.0.7',
+    version='2.0.8',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.0.7/vbpy/combine_data_file.py` & `vbpy-2.0.8/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.0.7/vbpy/load_claim_auto_file.py` & `vbpy-2.0.8/vbpy/load_claim_auto_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,22 +255,14 @@
                     #     SO_HSBT = index
                     #     STBT = row['STBT']
 
                     #     df.loc[df['SO_HSBT'] == SO_HSBT, ['STBT']] = STBT
 
                     # print(f"Step 3 - Adjust for Internal Insurance\n   -Removed {(_nrows_bf3 - df.shape[0]):,.0f} Rows\n   -Change in Tot Claims = {(_clms_bf3 - df['STBT'].sum()):,.0f} ({((_clms_bf3 - df['STBT'].sum())/_clms_bf3*100):,.0f}%)")
 
-                       
-                        
-                    """ FILTER OUT TEST ROWS """
-                    print("--------------------------------------------------------------------------\nFiltering Test Rows:")
-                    rows_b4 = df.shape[0]
-                    claims_b4 = df['STBT'].sum()
-                    df = df[~(df['NGAY_TT_BT'].isna() & (df['STBT'] <= 1000))]  
-                    print(f"   Removed {(rows_b4 - df.shape[0]):,.0f} Rows\n   Change in Tot Claims = {(claims_b4 - df['STBT'].sum()):,.0f} ({((claims_b4 - df['STBT'].sum())/claims_b4*100):,.0f}%)")
                         
                     
                     """ REMOVE ROWs WITH MISSING EFF DATE """
                     print("--------------------------------------------------------------------------\nRemoving Rows Missing NGAY_HL:")    
                     rows_b4 = df.shape[0]    
                     df = df[df['NGAY_HL'].notna()]
                     print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
```

### Comparing `vbpy-2.0.7/vbpy/load_revenue_auto_file.py` & `vbpy-2.0.8/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

