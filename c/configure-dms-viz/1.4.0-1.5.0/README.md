# Comparing `tmp/configure_dms_viz-1.4.0.tar.gz` & `tmp/configure_dms_viz-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configure_dms_viz-1.4.0.tar", max compression
+gzip compressed data, was "configure_dms_viz-1.5.0.tar", max compression
```

## Comparing `configure_dms_viz-1.4.0.tar` & `configure_dms_viz-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/LICENSE
--rw-r--r--   0        0        0     9172 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/README.md
--rw-r--r--   0        0        0        0 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/configure_dms_viz/__init__.py
--rwxr-xr-x   0        0        0    41547 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/configure_dms_viz/configure_dms_viz.py
--rw-r--r--   0        0        0     8500 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/configure_dms_viz/pdb_utils.py
--rw-r--r--   0        0        0     1454 2024-05-17 20:09:26.922952 configure_dms_viz-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-21 20:26:18.710875 configure_dms_viz-1.5.0/LICENSE
+-rw-r--r--   0        0        0     9172 2024-05-21 20:26:18.710875 configure_dms_viz-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 20:26:18.710875 configure_dms_viz-1.5.0/configure_dms_viz/__init__.py
+-rwxr-xr-x   0        0        0    42697 2024-05-21 20:26:18.710875 configure_dms_viz-1.5.0/configure_dms_viz/configure_dms_viz.py
+-rw-r--r--   0        0        0     8500 2024-05-21 20:26:18.710875 configure_dms_viz-1.5.0/configure_dms_viz/pdb_utils.py
+-rw-r--r--   0        0        0     1454 2024-05-21 20:26:18.714875 configure_dms_viz-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10199 1970-01-01 00:00:00.000000 configure_dms_viz-1.5.0/PKG-INFO
```

### Comparing `configure_dms_viz-1.4.0/LICENSE` & `configure_dms_viz-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.4.0/README.md` & `configure_dms_viz-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.4.0/configure_dms_viz/configure_dms_viz.py` & `configure_dms_viz-1.5.0/configure_dms_viz/configure_dms_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,14 +367,16 @@
     alphabet="RKHDEQNSTYWFAILMVGPC-*",
     colors=None,
     negative_colors=None,
     check_pdb=True,
     exclude_amino_acids=None,
     description=None,
     title=None,
+    floor=None,
+    summary_stat=None,
 ):
     """Take site-level and mutation-level measurements and format into
     a dictionary that can be used to create a JSON file for the visualization.
 
     Parameters
     ---------
     mut_metric_df: pandas.DataFrame
@@ -415,14 +417,18 @@
         Check that the chains and wildtype residues are in the structure.
     exclude_amino_acids: list or None
         Amino acids that should be excluded from the summary statistics.
     description: str or None
         A short description of the dataset to show in the tool.
     title: str or None
         A short title to appear above the plot.
+    floor: bool or None
+        If True, the floor of the metric will be set to 0 by default.
+    summary_stat: str or None
+        The default summary statistic to display on the plot.
 
     Returns
     -------
     dict
         A dictionary containing a single dataset for visualization to convert into a JSON file.
     """
 
@@ -657,14 +663,26 @@
         metric_col = metric_name
 
     # Rename the condition column to the condition name
     if condition_name:
         mut_metric_df = mut_metric_df.rename(columns={condition_col: condition_name})
         condition_col = condition_name
 
+    # Check that the floor is a valid value
+    if floor is not None:
+        if not isinstance(floor, bool):
+            raise ValueError("The floor value must be a boolean.")
+
+    # Check that the summary statistic is a valid value
+    if summary_stat is not None:
+        if summary_stat not in ["sum", "mean", "median", "max", "min"]:
+            raise ValueError(
+                "The summary statistic must be one of 'sum', 'mean', 'median', 'max', or 'min'."
+            )
+
     # Check that the chains and wildtype residues are in the structure
     if check_pdb:
         if included_chains != "polymer":
             check_chains(get_structure(structure), included_chains.split(" "))
         # Check that the wildtype residues are in the structure
         perc_matching, perc_missing, count_matching, count_missing = (
             check_wildtype_residues(
@@ -703,14 +721,16 @@
         "filter_cols": filter_cols,
         "filter_limits": filter_limits,
         "heatmap_limits": heatmap_limits,
         "tooltip_cols": tooltip_cols,
         "excludedAminoAcids": exclude_amino_acids,
         "description": description,
         "title": title,
+        "floor": floor,
+        "summary_stat": summary_stat,
     }
 
     return experiment_dict
 
 
 # ============================== Command Line Interface ============================== #
 
@@ -896,14 +916,28 @@
 @click.option(
     "--title",
     type=str,
     required=False,
     default=None,
     help="A short title to appear above the plot.",
 )
+@click.option(
+    "--floor",
+    type=bool,
+    required=False,
+    default=None,
+    help="If True, the floor of the metric will be set to 0 by default.",
+)
+@click.option(
+    "--summary-stat",
+    type=str,
+    required=False,
+    default=None,
+    help="The default summary statistic to display on the plot.",
+)
 def format(
     input,
     sitemap,
     metric,
     condition,
     structure,
     name,
@@ -920,14 +954,16 @@
     alphabet,
     colors,
     negative_colors,
     check_pdb,
     exclude_amino_acids,
     description,
     title,
+    floor,
+    summary_stat,
 ):
     """Command line interface for creating a JSON file for visualizing protein data"""
     click.secho(
         message=f"\nFormatting data for visualization using the '{metric}' column from '{input}'...",
         fg="green",
     )
 
@@ -969,14 +1005,16 @@
         alphabet,
         colors,
         negative_colors,
         check_pdb,
         exclude_amino_acids,
         description,
         title,
+        floor,
+        summary_stat,
     )
 
     # Write the dictionary to a json file
     with open(output, "w") as f:
         json.dump({name: experiment_dict}, f)
 
     click.secho(
```

### Comparing `configure_dms_viz-1.4.0/configure_dms_viz/pdb_utils.py` & `configure_dms_viz-1.5.0/configure_dms_viz/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.4.0/pyproject.toml` & `configure_dms_viz-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configure-dms-viz"
-version = "1.4.0"
+version = "1.5.0"
 description = "Configure your data for visualization with dms-viz.github.io"
 authors = ["Will Hannon <hannonww@gmail.com>"]
 maintainers = ["Will Hannon <hannonww@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dms-viz"
 repository = "https://github.com/dms-viz/configure_dms_viz"
```

### Comparing `configure_dms_viz-1.4.0/PKG-INFO` & `configure_dms_viz-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configure-dms-viz
-Version: 1.4.0
+Version: 1.5.0
 Summary: Configure your data for visualization with dms-viz.github.io
 Home-page: https://github.com/dms-viz
 License: MIT
 Keywords: deep mutational scanning,interactive protein structure,dms-viz,dms,protein
 Author: Will Hannon
 Author-email: hannonww@gmail.com
 Maintainer: Will Hannon
```

