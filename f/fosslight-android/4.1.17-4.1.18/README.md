# Comparing `tmp/fosslight_android-4.1.17.tar.gz` & `tmp/fosslight_android-4.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fosslight_android-4.1.17.tar", last modified: Mon Apr  8 04:33:54 2024, max compression
+gzip compressed data, was "fosslight_android-4.1.18.tar", last modified: Tue May 21 11:18:35 2024, max compression
```

## Comparing `fosslight_android-4.1.17.tar` & `fosslight_android-4.1.18.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1557 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.457349 fosslight_android-4.1.17/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/src/fosslight_android/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_binary_db_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_src_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/_write_excel.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33530 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/android_binary_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/check_notice_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/check_package_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/src/fosslight_android/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   146753 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/resources/aosp_repository.json
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 04:33:45.000000 fosslight_android-4.1.17/src/fosslight_android/resources/module_license.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:33:54.461349 fosslight_android-4.1.17/src/fosslight_android.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 04:33:54.000000 fosslight_android-4.1.17/src/fosslight_android.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:35.414314 fosslight_android-4.1.18/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-21 11:18:35.414314 fosslight_android-4.1.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:18:35.414314 fosslight_android-4.1.18/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1557 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:35.410314 fosslight_android-4.1.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:35.410314 fosslight_android-4.1.18/src/fosslight_android/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/_binary_db_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/_src_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/_write_excel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33760 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/android_binary_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/check_notice_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/check_package_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:35.414314 fosslight_android-4.1.18/src/fosslight_android/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   146753 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/resources/aosp_repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 11:18:21.000000 fosslight_android-4.1.18/src/fosslight_android/resources/module_license.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:35.414314 fosslight_android-4.1.18/src/fosslight_android.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-21 11:18:35.000000 fosslight_android-4.1.18/src/fosslight_android.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 11:18:35.000000 fosslight_android-4.1.18/src/fosslight_android.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:18:35.000000 fosslight_android-4.1.18/src/fosslight_android.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 11:18:35.000000 fosslight_android-4.1.18/src/fosslight_android.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 11:18:35.000000 fosslight_android-4.1.18/src/fosslight_android.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 11:18:35.000000 fosslight_android-4.1.18/src/fosslight_android.egg-info/top_level.txt
```

### Comparing `fosslight_android-4.1.17/LICENSE` & `fosslight_android-4.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/PKG-INFO` & `fosslight_android-4.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_android
-Version: 4.1.17
+Version: 4.1.18
 Summary: FOSSLight Android Scanner
 Home-page: https://github.com/fosslight/fosslight_android_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_android_scanner
 Description: <!--
         # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

### Comparing `fosslight_android-4.1.17/README.md` & `fosslight_android-4.1.18/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/setup.py` & `fosslight_android-4.1.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 
 if __name__ == "__main__":
     setup(
         name='fosslight_android',
-        version='4.1.17',
+        version='4.1.18',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Android Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_android-4.1.17/src/fosslight_android/_binary_db_controller.py` & `fosslight_android-4.1.18/src/fosslight_android/_binary_db_controller.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/_common.py` & `fosslight_android-4.1.18/src/fosslight_android/_common.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/_help.py` & `fosslight_android-4.1.18/src/fosslight_android/_help.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         Mandatory
             -s <android_source_path>\t   Path to analyze
             -a <build_log_file_name>\t   The file must be located in the android source path.
 
         Optional
             -h\t\t\t\t   Print help message
             -m\t\t\t\t   Analyze the source code for the path where the license could not be found.
+            -e <path1> <path2..>\t   Path to exclude from source analysis.
             -p\t\t\t\t   Check files that should not be included in the Packaging file.
             -f\t\t\t\t   Print result of Find Command for binary that can not find Source Code Path.
             -t\t\t\t\t   Collect NOTICE for binaries that are not added to NOTICE.html.
             -d\t\t\t\t   Divide needtoadd-notice.html by binary.
             -i\t\t\t\t   Disable the function to automatically convert OSS names based on AOSP.
             -r <result.txt>\t\t   result.txt file with a list of binaries to remove."""
```

### Comparing `fosslight_android-4.1.17/src/fosslight_android/_src_analysis.py` & `fosslight_android-4.1.18/src/fosslight_android/_src_analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,35 +9,44 @@
 from ._common import CONST_NULL
 from fosslight_util.constant import LOGGER_NAME
 
 logger = logging.getLogger(LOGGER_NAME)
 ANALYSIS_OUTPUT_DIR = "source_analyzed"
 
 
-def find_item_to_analyze(bin_info, output_path, start_time=""):
-    logger.info("* START TO ANALYZE SOURCE")
+def find_item_to_analyze(bin_info, output_path, start_time="", path_to_exclude=[]):
     path_list_to_analyze = {}
     for item in bin_info:
         try:
             source_path = item.source_code_path
             item_license = item.license
             if item_license == CONST_NULL and source_path != CONST_NULL:
                 path_list_to_analyze[source_path] = ""
         except Exception as error:
             logger.debug(f"Find_item_to_analyze:{error}")
 
-    logger.info(f"|--Source analysis begins for {len(path_list_to_analyze)} paths.")
-    idx = 0
+    source_analysis_path = [path for path in path_list_to_analyze.keys() if path not in path_to_exclude]
+    logger.info(f"|--Source analysis for {len(source_analysis_path)} paths.")
+    for path in source_analysis_path:
+        file_array = [len(files) for r, d, files in os.walk(path)]
+        files = sum(file_array)
+        logger.info(f"{path}, File Count:{files}")
+
     output_dir = os.path.join(output_path, f"{ANALYSIS_OUTPUT_DIR}_{start_time}")
-    for source_path in path_list_to_analyze.keys():
+
+    logger.info("------------------------------")
+    logger.info("* START TO ANALYZE SOURCE *")
+    idx = 0
+    for source_path in source_analysis_path:
         try:
             idx += 1
-            logger.info(f"|---{idx} {source_path}")
-            license = run_src_analysis(source_path, start_time, output_dir)
-            path_list_to_analyze[source_path] = license
+            if os.path.isdir(source_path):
+                logger.info(f"({idx}){source_path}")
+                license = run_src_analysis(source_path, start_time, output_dir)
+                path_list_to_analyze[source_path] = license
         except Exception as error:
             logger.debug(f"Failed to run src analysis:{error}")
 
     for analyzed_path, analyzed_license in path_list_to_analyze.items():
         try:
             for item in bin_info:
                 source_path = item.source_code_path
```

### Comparing `fosslight_android-4.1.17/src/fosslight_android/_util.py` & `fosslight_android-4.1.18/src/fosslight_android/_util.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/_write_excel.py` & `fosslight_android-4.1.18/src/fosslight_android/_write_excel.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/android_binary_analysis.py` & `fosslight_android-4.1.18/src/fosslight_android/android_binary_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,14 +757,15 @@
     find_empty_path = False
     _create_additial_notice = False
     notice_check_ok = False
     base_binary_txt = ""
     auto_fill_oss_name = True
     _NOTICE_CHECKLIST_TYPE = False
     analyze_source = False
+    path_to_exclude = []
 
     num_cores = multiprocessing.cpu_count() - 1
     if num_cores < 1:
         num_cores = 1
 
     python_script_dir = os.getcwd()
     now = datetime.now().strftime('%y%m%d_%H%M')
@@ -784,14 +785,15 @@
     parser.add_argument('-c', '--check', type=str, required=False)
     parser.add_argument('-a', '--android', type=str, required=False)
     parser.add_argument('-f', '--find', action='store_true', required=False)
     parser.add_argument('-i', '--ignore', action='store_true', required=False)
     parser.add_argument('-p', '--packaging', type=str, required=False)
     parser.add_argument('-d', '--divide', type=str, required=False)
     parser.add_argument('-r', '--remove', type=str, required=False)
+    parser.add_argument('-e', '--exclude', nargs="*", required=False, default=[])
 
     args = parser.parse_args()
     if args.help:
         print_help_msg()
     if args.version:
         print_version(PKG_NAME)
     if args.source:  # android source path
@@ -809,14 +811,16 @@
         notice_check_ok = (args.check == "ok" or args.check == "OK")
     if args.android:
         ANDROID_LOG_FILE_NAME = args.android
     if args.find:  # Execute "find" command when source path is not found.
         find_empty_path = True
     if args.ignore:  # Disable the function to automatically convert OSS names based on AOSP.
         auto_fill_oss_name = False
+    if args.exclude:  # Path to exclude from source code analysis.
+        path_to_exclude = args.exclude
 
     logger, result_log = init_log(log_txt_file, True, logging.INFO, logging.DEBUG, PKG_NAME)
 
     if args.packaging:
         check_packaging_files(args.packaging)
         return
     if args.divide:
@@ -846,15 +850,15 @@
 
     set_checksum_tlsh_and_get_oss_from_db_after_remove_duplication(remove_list_file)
 
     if auto_fill_oss_name:
         set_oss_name_by_repository()
     if analyze_source:
         from ._src_analysis import find_item_to_analyze
-        final_bin_info = find_item_to_analyze(final_bin_info, python_script_dir, now)
+        final_bin_info = find_item_to_analyze(final_bin_info, python_script_dir, now, path_to_exclude)
 
     write_result_to_txt_and_excel(result_excel_file, final_bin_info, result_txt_file)
     result_log["Output FOSSLight Report"] = result_excel_file
     result_log["Output result text file"] = result_txt_file
 
     if _create_additial_notice:
         create_additional_notice(final_bin_info, python_script_dir)
```

### Comparing `fosslight_android-4.1.17/src/fosslight_android/check_notice_file.py` & `fosslight_android-4.1.18/src/fosslight_android/check_notice_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/check_package_file.py` & `fosslight_android-4.1.18/src/fosslight_android/check_package_file.py`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/resources/aosp_repository.json` & `fosslight_android-4.1.18/src/fosslight_android/resources/aosp_repository.json`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android/resources/module_license.json` & `fosslight_android-4.1.18/src/fosslight_android/resources/module_license.json`

 * *Files identical despite different names*

### Comparing `fosslight_android-4.1.17/src/fosslight_android.egg-info/PKG-INFO` & `fosslight_android-4.1.18/src/fosslight_android.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-android
-Version: 4.1.17
+Version: 4.1.18
 Summary: FOSSLight Android Scanner
 Home-page: https://github.com/fosslight/fosslight_android_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_android_scanner
 Description: <!--
         # SPDX-FileCopyrightText: Copyright 2023 LG Electronics Inc.
```

### Comparing `fosslight_android-4.1.17/src/fosslight_android.egg-info/SOURCES.txt` & `fosslight_android-4.1.18/src/fosslight_android.egg-info/SOURCES.txt`

 * *Files identical despite different names*

