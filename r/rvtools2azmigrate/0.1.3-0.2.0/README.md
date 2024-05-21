# Comparing `tmp/rvtools2azmigrate-0.1.3.tar.gz` & `tmp/rvtools2azmigrate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvtools2azmigrate-0.1.3.tar", last modified: Wed Oct 11 07:35:45 2023, max compression
+gzip compressed data, was "rvtools2azmigrate-0.2.0.tar", last modified: Tue May 21 09:44:37 2024, max compression
```

## Comparing `rvtools2azmigrate-0.1.3.tar` & `rvtools2azmigrate-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:35:45.273632 rvtools2azmigrate-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-10-11 07:35:45.273632 rvtools2azmigrate-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:35:45.273632 rvtools2azmigrate-0.1.3/rvtools2azmigrate/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2891 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate/azmigrate_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate/convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2723 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate/rvtools_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:35:45.273632 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-11 07:35:45.000000 rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 07:35:45.273632 rvtools2azmigrate-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2023-10-11 07:35:33.000000 rvtools2azmigrate-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:44:37.414137 rvtools2azmigrate-0.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/AUTHORS.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-21 09:44:37.414137 rvtools2azmigrate-0.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:44:37.414137 rvtools2azmigrate-0.2.0/rvtools2azmigrate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      107 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2972 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate/azmigrate_vm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2131 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6559 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate/convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2723 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate/rvtools_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:44:37.414137 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 09:44:37.000000 rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      411 2024-05-21 09:44:37.414137 rvtools2azmigrate-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1644 2024-05-21 09:44:27.000000 rvtools2azmigrate-0.2.0/setup.py
```

### Comparing `rvtools2azmigrate-0.1.3/LICENSE` & `rvtools2azmigrate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rvtools2azmigrate-0.1.3/PKG-INFO` & `rvtools2azmigrate-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvtools2azmigrate
-Version: 0.1.3
+Version: 0.2.0
 Summary: Convert an RVTools export to an Azure Migrate CSV inventory file
 Home-page: https://github.com/lrivallain/rvtools2azmigrate
 Author: Ludovic Rivallain
 License: MIT license
 Keywords: rvtools2azmigrate
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -91,14 +91,15 @@
 Convert RVTools file to Azure Migrate format
 
 Options:
   -i, --rvtools PATH  RVTools input file  [required]
   -o, --output PATH   Ouptut file  [required]
   --anonymized        Anonymize the output file by replacing VM names with UUIDs
   --filter-off-vms    Filter the powered-off VMs
+  --filter-out TEXT   Filter out VMs based on the provided patterns (contains + case-insensitive)
   --help              Show this message and exit.
 ```
 
 ### Examples
 
 #### Anonymized
 
@@ -113,16 +114,35 @@
 ```bash
 rvtools2azmigrate convert -i rvtools.xlsx -o azuremigrate.csv --filter-off-vms
 ```
 
 This will provide a CSV file to be imported in Azure Migrate manual discovery section. Powered-Off VMs will not be exported to the CSV file.
 
 
+#### Filter out VMs based on naming
+
+It is possible to specify a list of patterns to filter out VMs based on their name.
+
+```bash
+rvtools2azmigrate convert -i rvtools.xlsx -o azuremigrate.csv \
+  --filter-out pattern1 \
+  --filter-out pattern2 \
+  --filter-out pattern3
+```
+
+This will provide a CSV file to be imported in Azure Migrate manual discovery section. VMs with one of the pattern in their name will be filtered out and not part of the exported file.
+
+
 # History
 
+## 0.2.0 (2024-05-21)
+
+* Feat: Use python-slugify to generate VM names
+* Feat: Filter out VMs based on name with `--filter-out pattern1 --filter-out pattern2`
+
 ## 0.1.3 (2023-10-11)
 
 * Fix #2: Incorrect output if RV Tools input has a VM name with spaces in it
 
 ## 0.1.2 (2023-02-16)
 
 * Fix import issue when used as installed module
```

### Comparing `rvtools2azmigrate-0.1.3/README.md` & `rvtools2azmigrate-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 Convert RVTools file to Azure Migrate format
 
 Options:
   -i, --rvtools PATH  RVTools input file  [required]
   -o, --output PATH   Ouptut file  [required]
   --anonymized        Anonymize the output file by replacing VM names with UUIDs
   --filter-off-vms    Filter the powered-off VMs
+  --filter-out TEXT   Filter out VMs based on the provided patterns (contains + case-insensitive)
   --help              Show this message and exit.
 ```
 
 ### Examples
 
 #### Anonymized
 
@@ -91,7 +92,21 @@
 #### Filter off VMs
 
 ```bash
 rvtools2azmigrate convert -i rvtools.xlsx -o azuremigrate.csv --filter-off-vms
 ```
 
 This will provide a CSV file to be imported in Azure Migrate manual discovery section. Powered-Off VMs will not be exported to the CSV file.
+
+
+#### Filter out VMs based on naming
+
+It is possible to specify a list of patterns to filter out VMs based on their name.
+
+```bash
+rvtools2azmigrate convert -i rvtools.xlsx -o azuremigrate.csv \
+  --filter-out pattern1 \
+  --filter-out pattern2 \
+  --filter-out pattern3
+```
+
+This will provide a CSV file to be imported in Azure Migrate manual discovery section. VMs with one of the pattern in their name will be filtered out and not part of the exported file.
```

### Comparing `rvtools2azmigrate-0.1.3/rvtools2azmigrate/azmigrate_vm.py` & `rvtools2azmigrate-0.2.0/rvtools2azmigrate/azmigrate_vm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """AzMigrateVM class definition
 """
 
 import logging
 
+from slugify import slugify
+
 log = logging.getLogger(__name__)
 
 
 class AzMigrateVM:
     """Class to represent a VM in Azure Migrate import format"""
 
     def __init__(
@@ -19,15 +21,16 @@
             cores (int): Number of CPU cores for the server
             memory (int): Memory allocated to the server (MB)
             os (str): OS name
             architecture (str): Architecture of the OS
             boot_type (str): Boot type of the server
             disk1_size (int): Disk size of the server (GB)
         """
-        self.server_name = server_name.replace(' ', '-').replace('_', '-').replace('.', '-').replace(',', '-')
+        # slugify the server name to avoid special characters and limit the length
+        self.server_name = slugify(server_name, lowercase=False, max_length=25)
         self.cores = cores
         self.memory = memory
         self.os = os
         self.architecture = architecture
         self.boot_type = boot_type
         self.disk1_size = disk1_size
```

### Comparing `rvtools2azmigrate-0.1.3/rvtools2azmigrate/cli.py` & `rvtools2azmigrate-0.2.0/rvtools2azmigrate/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,41 +22,49 @@
         handlers=[RichHandler()],
     )
     click.echo("RVTools to Azure Migrate converter")
     log.debug(f"Debug mode is {'on' if debug else 'off'}")
     return 0
 
 
-@cli.command()  # @cli, not @click!
+@cli.command()
 @click.option(
     "-i",
     "--rvtools",
     help="RVTools input file",
     required=True,
     type=click.Path(exists=True),
 )
-@click.option("-o", "--output", help="Ouptut file", required=True, type=click.Path(exists=False))
+@click.option("-o", "--output", help="Output file", required=True, type=click.Path(exists=False))
 @click.option(
     "--anonymized",
     default=False,
     is_flag=True,
     help="Anonymize the output file by replacing VM names with UUIDs",
 )
 @click.option(
     "--filter-off-vms",
     default=False,
     is_flag=True,
     help="Filter the powered-off VMs",
 )
-def convert(rvtools: str, output: str, anonymized: bool, filter_off_vms: bool):
+@click.option(
+    "--filter-out",
+    default=[],
+    multiple=True,
+    help="Filter out VMs based on the provided patterns (contains + case-insensitive)",
+)
+def convert(rvtools: str, output: str, anonymized: bool, filter_off_vms: bool, filter_out: list[str]):
     """Convert RVTools file to Azure Migrate format"""
     log.info("Starting RVTools file conversion to Azure Migrate format...")
     log.debug(f"Input file: {click.format_filename(rvtools)}")
     log.debug(f"Output file: {click.format_filename(output)}")
     log.debug(f"Anonymized: {anonymized}")
     log.debug(f"Filter powered-off VMs: {filter_off_vms}")
-    convert_rvtools_to_azmigrate(rvtools=rvtools, output=output, anonymized=anonymized, filter_off_vms=filter_off_vms)
+    if filter_out:
+        log.debug(f"Filter VMs with following patterns: {", ".join(filter_out)}")
+    convert_rvtools_to_azmigrate(rvtools=rvtools, output=output, anonymized=anonymized, filter_off_vms=filter_off_vms, filter_out=filter_out)
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(cli())  # pragma: no cover
```

### Comparing `rvtools2azmigrate-0.1.3/rvtools2azmigrate/convert.py` & `rvtools2azmigrate-0.2.0/rvtools2azmigrate/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,29 +24,34 @@
     for column_cell in ws.iter_cols(1, ws.max_column):  # iterate column cell
         if column_cell[0].value == column_name:  # check for your column
             return [data.value for data in column_cell[1:]]  # iterate your column
     log.warning(f"Column {column_name} not found")
     return None
 
 
-def get_rvtools_vms(rvtools_data: dict, anonymized: bool, filter_off_vms: bool) -> list():
+def get_rvtools_vms(rvtools_data: dict, anonymized: bool, filter_off_vms: bool, filter_out: list[str]) -> list():
     """Get a list of RvToolsVM objects based on the RVTools data
 
     Args:
         rvtools_data (dict): RVTools data as a dict
         anonymized (bool): Anonymize the output data ?
         filter_off_vms (bool): Filter the powered-off VMs
+        filter_out (list): List of VM naming patterns to filter out (contains)
 
     Returns:
         list(): List of RvToolsVM objects
     """
     rvtools_vms = []
     nb_vms = len(rvtools_data["vms_name"])
-    vm_name_already_used = []
     for i in range(nb_vms):
+        # Filtering out VMs based on provided patterns
+        for fout_pattern in filter_out:
+            if fout_pattern.lower() in rvtools_data["vms_name"][i].lower():
+                log.debug(f"Filtered out VM {rvtools_data['vms_name'][i]} based on pattern {fout_pattern}")
+                break
         rv_vm = RvToolsVM(
             is_anonymized=anonymized,
             name=rvtools_data["vms_name"][i],
             power_state=rvtools_data["power_states"][i],
             cores=rvtools_data["cores"][i],
             memory=rvtools_data["memory"][i],
             os_config=rvtools_data["os_config"][i],
@@ -129,28 +134,29 @@
         "dns_name": get_column_data_by_name(ws, column_name="DNS Name"),
         "uuid": get_column_data_by_name(ws, column_name="VM UUID"),
         "firmware": get_column_data_by_name(ws, column_name="Firmware"),
         "is_mib": is_mib,
     }
 
 
-def convert_rvtools_to_azmigrate(rvtools: str, output: str, anonymized: bool, filter_off_vms: bool):
+def convert_rvtools_to_azmigrate(rvtools: str, output: str, anonymized: bool, filter_off_vms: bool, filter_out: list[str]):
     """Convert RVTools file to Azure Migrate format
 
     Args:
         rvtools (str): Input file in RVTools format
         output (str): Output file in Azure Migrate CSV format
         anonymized (bool): Anonymize VM names
         filter_off_vms (bool): Filter the powered-off VMs
+        filter_out (list): List of VM naming patterns to filter out (contains)
     """
     # Read data from RVTools file
     rvtools_data = parse_rvtools_data(rvtools)
     log.info(f"We have found {len(rvtools_data['vms_name'])} VMs in the file {rvtools}")
 
     # Create a list of VMs
-    rvtools_vms = get_rvtools_vms(rvtools_data, anonymized, filter_off_vms)
+    rvtools_vms = get_rvtools_vms(rvtools_data, anonymized, filter_off_vms, filter_out)
     log.info(f"VM data set from RVtools was built successfully")
 
     # Export VMs to an AZ migrate CSV file
     write_azmigrate_file(rvtools_vms, output)
     log.info(f"File {output} created successfully with {len(rvtools_vms)} VMs")
     return 0
```

### Comparing `rvtools2azmigrate-0.1.3/rvtools2azmigrate/rvtools_vm.py` & `rvtools2azmigrate-0.2.0/rvtools2azmigrate/rvtools_vm.py`

 * *Files identical despite different names*

### Comparing `rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/PKG-INFO` & `rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvtools2azmigrate
-Version: 0.1.3
+Version: 0.2.0
 Summary: Convert an RVTools export to an Azure Migrate CSV inventory file
 Home-page: https://github.com/lrivallain/rvtools2azmigrate
 Author: Ludovic Rivallain
 License: MIT license
 Keywords: rvtools2azmigrate
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -91,14 +91,15 @@
 Convert RVTools file to Azure Migrate format
 
 Options:
   -i, --rvtools PATH  RVTools input file  [required]
   -o, --output PATH   Ouptut file  [required]
   --anonymized        Anonymize the output file by replacing VM names with UUIDs
   --filter-off-vms    Filter the powered-off VMs
+  --filter-out TEXT   Filter out VMs based on the provided patterns (contains + case-insensitive)
   --help              Show this message and exit.
 ```
 
 ### Examples
 
 #### Anonymized
 
@@ -113,16 +114,35 @@
 ```bash
 rvtools2azmigrate convert -i rvtools.xlsx -o azuremigrate.csv --filter-off-vms
 ```
 
 This will provide a CSV file to be imported in Azure Migrate manual discovery section. Powered-Off VMs will not be exported to the CSV file.
 
 
+#### Filter out VMs based on naming
+
+It is possible to specify a list of patterns to filter out VMs based on their name.
+
+```bash
+rvtools2azmigrate convert -i rvtools.xlsx -o azuremigrate.csv \
+  --filter-out pattern1 \
+  --filter-out pattern2 \
+  --filter-out pattern3
+```
+
+This will provide a CSV file to be imported in Azure Migrate manual discovery section. VMs with one of the pattern in their name will be filtered out and not part of the exported file.
+
+
 # History
 
+## 0.2.0 (2024-05-21)
+
+* Feat: Use python-slugify to generate VM names
+* Feat: Filter out VMs based on name with `--filter-out pattern1 --filter-out pattern2`
+
 ## 0.1.3 (2023-10-11)
 
 * Fix #2: Incorrect output if RV Tools input has a VM name with spaces in it
 
 ## 0.1.2 (2023-02-16)
 
 * Fix import issue when used as installed module
```

### Comparing `rvtools2azmigrate-0.1.3/rvtools2azmigrate.egg-info/SOURCES.txt` & `rvtools2azmigrate-0.2.0/rvtools2azmigrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rvtools2azmigrate-0.1.3/setup.py` & `rvtools2azmigrate-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     history = history_file.read()
 
 requirements = [
     "coloredlogs",
     "Click",
     "openpyxl",
     "rich",
+    "python-slugify",
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 description = "Convert an RVTools export to an Azure Migrate CSV inventory file"
@@ -51,10 +52,10 @@
     include_package_data=True,
     keywords="rvtools2azmigrate",
     name="rvtools2azmigrate",
     packages=find_packages(include=["rvtools2azmigrate", "rvtools2azmigrate.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/lrivallain/rvtools2azmigrate",
-    version="0.1.3",
+    version="0.2.0",
     zip_safe=False,
 )
```

