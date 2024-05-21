# Comparing `tmp/lpath-md-1.0.1.tar.gz` & `tmp/lpath_md-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpath-md-1.0.1.tar", last modified: Fri Mar  1 18:24:13 2024, max compression
+gzip compressed data, was "lpath_md-1.0.2.tar", last modified: Tue May 21 19:37:22 2024, max compression
```

## Comparing `lpath-md-1.0.1.tar` & `lpath_md-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 18:24:13.172120 lpath-md-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-01 18:24:08.000000 lpath-md-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-01 18:24:08.000000 lpath-md-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-01 18:24:08.000000 lpath-md-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-01 18:24:13.172120 lpath-md-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-03-01 18:24:08.000000 lpath-md-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 18:24:13.172120 lpath-md-1.0.1/lpath/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    37078 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 18:24:13.168120 lpath-md-1.0.1/lpath/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 18:24:13.172120 lpath-md-1.0.1/lpath/data/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/data/styles/default.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/extloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44451 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/extract.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/lpath.py
--rw-r--r--   0 runner    (1001) docker     (127)    35980 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 18:24:13.172120 lpath-md-1.0.1/lpath/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/test_discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/test_lpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-01 18:24:08.000000 lpath-md-1.0.1/lpath/tests/test_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 18:24:13.172120 lpath-md-1.0.1/lpath_md.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath_md.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath_md.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath_md.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath_md.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 18:24:12.000000 lpath-md-1.0.1/lpath_md.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath_md.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 18:24:13.000000 lpath-md-1.0.1/lpath_md.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-01 18:24:08.000000 lpath-md-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-01 18:24:13.176120 lpath-md-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.082848 lpath_md-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 19:37:17.000000 lpath_md-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-21 19:37:17.000000 lpath_md-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-21 19:37:17.000000 lpath_md-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-21 19:37:22.082848 lpath_md-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-21 19:37:17.000000 lpath_md-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37269 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.074848 lpath_md-1.0.2/lpath/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath/data/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/data/styles/default.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/extloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44451 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/extract.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3669 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/lpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36321 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_lpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-21 19:37:17.000000 lpath_md-1.0.2/lpath/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:37:22.078848 lpath_md-1.0.2/lpath_md.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:37:21.000000 lpath_md-1.0.2/lpath_md.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 19:37:22.000000 lpath_md-1.0.2/lpath_md.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-21 19:37:17.000000 lpath_md-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-21 19:37:22.082848 lpath_md-1.0.2/setup.cfg
```

### Comparing `lpath-md-1.0.1/CODE_OF_CONDUCT.md` & `lpath_md-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/LICENSE` & `lpath_md-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/PKG-INFO` & `lpath_md-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpath-md
-Version: 1.0.1
+Version: 1.0.2
 Summary: A user-friendly, Python tool for clustering pathways from molecular dynamics simulations.
 Author-email: Anthony Bogetti <atb43@pitt.edu>, Jeremy Leung <jml230@pitt.edu>, Lillian Chong <lchong@pitt.edu>
 Maintainer-email: Jeremy Leung <jml230@pitt.edu>
 License: MIT
 Project-URL: Source, https://github.com/chonglab-pitt/lpath/
 Project-URL: Documentation, https://lpath.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lpath-md-1.0.1/README.md` & `lpath_md-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/_logger.py` & `lpath_md-1.0.2/lpath/_logger.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/argparser.py` & `lpath_md-1.0.2/lpath/argparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -534,14 +534,16 @@
                          action='store_true', help=argparse.SUPPRESS)
     plot_io.add_argument('--plots-hide', '-pth', '--dendrogram-hide', '-pdh', '--dendro-hide', '-dh',
                          dest='dendrogram_show', action='store_false',
                          help='Do not show dendrogram. Overrides ``--dendrogram-show``.')
     plot_io.add_argument('--n-clusters', '-nc', '--num-clusters', dest='num_clusters', type=check_positive,
                          help='For cases where you know in advance how many clusters you want for '
                               'the hierarchical clustering.')
+    plot_io.add_argument('--timeout', '-pto', '--plot-timeout', dest='plot_timeout', type=check_non_neg,
+                         default=None, help='Timeout (in seconds) for asking input.')
 
     # plot_io.add_argument('--plot-regen-cl', '-rcl', '--plot-regenerate-cluster-labels', dest='regen_cl',
     #                      action='store_true',
     #                      help='Option to regenerate new cluster labels after relabeling. ``--plot-cluster-labels`` '
     #                           'options can be left empty if this is called.')
     plot_io.add_argument('--relabel', '-prl', '--plot-relabel-method', '--plot-relabel-method', dest='relabel_method',
                          default='relabel_identity', type=str,
```

### Comparing `lpath-md-1.0.1/lpath/discretize.py` & `lpath_md-1.0.2/lpath/discretize.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/extloader.py` & `lpath_md-1.0.2/lpath/extloader.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/extract.py` & `lpath_md-1.0.2/lpath/extract.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/io.py` & `lpath_md-1.0.2/lpath/io.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/lpath.py` & `lpath_md-1.0.2/lpath/lpath.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/match.py` & `lpath_md-1.0.2/lpath/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,15 +936,15 @@
                     if (n_iter, n_seg) not in exclusive_set:
                         h5file[f"iterations/iter_{n_iter:>08}/seg_index"]["weight", n_seg] = 0
 
     with open(representative_file, 'w') as f:
         f.writelines(representative_list)
 
 
-def determine_rerun(z, out_path='plots', mpl_colors=default_dendrogram_colors, ax=None):
+def determine_rerun(z, out_path='plots', mpl_colors=default_dendrogram_colors, ax=None, timeout=None):
     """
     Asks if you want to regenerate the dendrogram.
 
     Parameters
     ----------
     z : numpy.ndarray
         A numpy.ndarray from sch.linkage.
@@ -953,52 +953,64 @@
         Path to output plots.
 
     mpl_colors : list or default_dendrogram_colors
         A list of colors for coloring the dendrogram.
 
     ax : matplotlib.Axes, Default: None
         Matplotlib.Axes object to be inherited.
+
+    timeout : int, default: 30
+        Input timeout in seconds.
+
     """
+    if timeout is None:
+        timeout = 30
+
     while True:
         try:
             ans = timedinput('Do you want to regenerate the graph with a new threshold (y/[n])?\n',
-                             timeout=60, default='N')
+                             timeout=timeout, default='N')
             if ans == 'y' or ans == 'Y':
                 ans2 = timedinput('What new threshold would you like?\n', timeout=15, default=0.5)
                 try:
                     ax = visualize(z, out_path=out_path, threshold=float(ans2),
                                    show_fig=True, mpl_colors=mpl_colors, ax=ax)
                     return ax
                 except ValueError:
-                    determine_rerun(z, out_path=out_path, mpl_colors=mpl_colors, ax=ax)
+                    determine_rerun(z, out_path=out_path, mpl_colors=mpl_colors, ax=ax, timeout=timeout)
             elif ans == 'n' or ans == 'N' or ans == '':
                 return None
             else:
                 log.warning("Invalid input.\n")
         except KeyboardInterrupt:
             sys.exit(0)
 
 
-def ask_number_clusters(num_clusters=None):
+def ask_number_clusters(num_clusters=None, timeout=None):
     """
     Asks how many clusters you want to separate the trajectories into.
 
     """
+    if timeout is None:
+        timeout = 15
+
     if not num_clusters:
         while True:
             try:
                 ans = timedinput('How many clusters would you like to separate the pathways into?\n',
-                                 timeout=15, default=2)
+                                 timeout=timeout, default=2)
                 try:
                     ans = int(ans)
                     return ans
                 except ValueError:
                     log.warning("Invalid input.\n")
             except KeyboardInterrupt:
                 sys.exit(0)
+    else:
+        return num_clusters
 
 
 def report_statistics(n_clusters, cluster_labels, weights, segid_status=False):
     """
     Report statistics about the final clusters.
 
     Parameters
@@ -1090,17 +1102,18 @@
 
     log.debug(f'Generated distance matrix.')
 
     # Visualize the Dendrogram and determine how clusters used to group successful trajectories
     z = calc_linkage(dist_matrix)
     ax = visualize(z, threshold=arguments.dendrogram_threshold, out_path=arguments.out_path,
                    show_fig=arguments.dendrogram_show, mpl_colors=arguments.mpl_colors)
-    ax = determine_rerun(z, out_path=arguments.out_path, mpl_colors=arguments.mpl_colors, ax=ax)
+    ax = determine_rerun(z, out_path=arguments.out_path, mpl_colors=arguments.mpl_colors, ax=ax,
+                         timeout=arguments.plot_timeout)
 
-    n_clusters = ask_number_clusters(arguments.num_clusters)
+    n_clusters = ask_number_clusters(arguments.num_clusters, timeout=arguments.plot_timeout)
     cluster_labels = hcluster(z, n_clusters)
 
     # Report statistics
     if arguments.stats:
         log.debug('Reporting statistics')
         if arguments.reassign_method == 'reassign_segid':
             segid_status = True
```

### Comparing `lpath-md-1.0.1/lpath/plot.py` & `lpath_md-1.0.2/lpath/plot.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/tests/conftest.py` & `lpath_md-1.0.2/lpath/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/tests/test_argparser.py` & `lpath_md-1.0.2/lpath/tests/test_argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         See if returned objects are legit.
 
         """
         output, _ = create_ref_parser
 
         assert isinstance(output, argparse.ArgumentParser)
         # Need to change as number of options increase
-        assert len(output._actions) == 66
+        assert len(output._actions) == 67
 
     def test_common_arguments(self, create_ref_parser):
         """
         Test to see if common args are in the parser.
 
         """
         output, test_output = create_ref_parser
@@ -176,11 +176,11 @@
     def test_plot_arguments(self, create_ref_parser):
         """
         Test to see if plot args are in the parser.
 
         """
         output, test_output = create_ref_parser
         test_input = ['-ipl', '-icl', '-pdF', '-pod', '-sty', '-mpl', '-col', '-pdt', '-pds',
-                      '-pdh', '-nc', '-prl']
+                      '-pdh', '-nc', '-prl', '-pto']
 
         for option in test_input:
             assert option in test_output
```

### Comparing `lpath-md-1.0.1/lpath/tests/test_extract.py` & `lpath_md-1.0.2/lpath/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath/tests/test_match.py` & `lpath_md-1.0.2/lpath/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/lpath_md.egg-info/PKG-INFO` & `lpath_md-1.0.2/lpath_md.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpath-md
-Version: 1.0.1
+Version: 1.0.2
 Summary: A user-friendly, Python tool for clustering pathways from molecular dynamics simulations.
 Author-email: Anthony Bogetti <atb43@pitt.edu>, Jeremy Leung <jml230@pitt.edu>, Lillian Chong <lchong@pitt.edu>
 Maintainer-email: Jeremy Leung <jml230@pitt.edu>
 License: MIT
 Project-URL: Source, https://github.com/chonglab-pitt/lpath/
 Project-URL: Documentation, https://lpath.readthedocs.io/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lpath-md-1.0.1/lpath_md.egg-info/SOURCES.txt` & `lpath_md-1.0.2/lpath_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lpath-md-1.0.1/pyproject.toml` & `lpath_md-1.0.2/pyproject.toml`

 * *Files identical despite different names*

