# Comparing `tmp/poseidon_rna-0.3.tar.gz` & `tmp/poseidon_rna-0.4.tar.gz`

## Comparing `poseidon_rna-0.3.tar` & `poseidon_rna-0.4.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.3/src/poseidonrna/__init__.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 poseidon_rna-0.3/src/poseidonrna/poseidonrna.py
--rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.3/test/full__average.ct
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.3/test/full__average.db
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.3/test/full__average__varna-color.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.3/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 poseidon_rna-0.3/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 poseidon_rna-0.3/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.4/src/poseidonrna/__init__.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 poseidon_rna-0.4/src/poseidonrna/poseidonrna.py
+-rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/full__average.ct
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/full__average.db
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/full__average__varna-color.txt
+-rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/Structures/a580__full.png
+-rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/Structures/a580__full.svg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.4/README.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 poseidon_rna-0.4/pyproject.toml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 poseidon_rna-0.4/PKG-INFO
```

### Comparing `poseidon_rna-0.3/src/poseidonrna/poseidonrna.py` & `poseidon_rna-0.4/src/poseidonrna/poseidonrna.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,33 +121,32 @@
 
             #Adds new node for each base and relevant connected edges
             conGraphStep(G,struc[x],'',colors[x+1])
 
         
     return G
 
-def plotGraph(G,name,color,node_size,bases,**kwargs):
+def plotGraph(G,name,color,node_size,bases,view,**kwargs):
 
     args = dict(kwargs.items())
 
+    plt.rcParams["figure.figsize"] = (15,15)
+
     try:
         pos = args['pos']
         
     except:
         pos = nx.kamada_kawai_layout(G)
 
-    plt.rcParams["figure.figsize"] = (15,15)
-
     if color == None:
         
         nx.draw(G,pos,with_labels=False,node_size = node_size)
 
     else:
         node_colors = [G.nodes[n]['color'] for n in G.nodes]
-        pos = nx.kamada_kawai_layout(G)
         nx.draw(G,pos,with_labels=False,node_size = node_size,node_color=node_colors,cmap=sns.color_palette("viridis", as_cmap=True))
 
     if bases == True:
         #Label nodes with base
         labels = nx.get_node_attributes(G, 'base')
         nx.draw_networkx_labels(G, pos, labels)
 
@@ -184,15 +183,15 @@
         
     except:
         prefix = '#'
 
     #plot color default:none
     try:
         color = args['color']
-        color_type = 'varna'#args['color_type']
+        color_type = 'varna'
     except:
         color = None
         color_type = None
 
     #plot bases default:false
     try:
         bases = args['bases']
@@ -203,60 +202,66 @@
     try:
         node_size = args['node_size']
     except:
         node_size = 10
 
     #view graph default:10
     try:
-        node_size = args['view']
+        view = args['view']
     except:
-        node_size = False
+        view = False
 
 
-    graphs = []
     #read in file if dot-bracket
     if filename[-2:]=='db':
     
         names,seqs,pairs = read_db_structures(filename)
 
-        if num_strucs == 'all':
-            num_strucs = len(pairs)
-            
-        for x in range(num_strucs):
-            G = create_db_graph(seqs[x],pairs[x],newcolors)
-            graphs.append(G)
-
-
     #read in file if connectivity table
     elif filename[-2:] == 'ct':
         
-        names, strucs = read_ct_structures(filename,prefix)
-
-        if num_strucs == 'all':
-            num_strucs = len(strucs)
-        
-        for x in range(num_strucs):
-            G = create_ct_graph(strucs[x],'',newcolors)
-            graphs.append(G)
+        names, seqs = read_ct_structures(filename,prefix)
 
     #read in colors from varna file
     if color_type == 'varna':
         with open(color, 'r') as file:
             # Read the lines
             colors = file.readlines()
         newcolors = [0.25]
         for x in range(len(colors)):
             newcolors.append((float(colors[x][:-2])+1)/2)
         file.close()
 
     else:
         newcolors = np.zeros(len(seqs[0])+1)
 
+
+    graphs = []
+    
+    if filename[-2:]=='db':
+        
+        if num_strucs == 'all':
+            num_strucs = len(pairs)
+            
+        for x in range(num_strucs):
+            G = create_db_graph(seqs[x],pairs[x],newcolors)
+            graphs.append(G)
+
+
+    elif filename[-2:] == 'ct':
+
+        if num_strucs == 'all':
+            num_strucs = len(seqs)
+        
+        for x in range(num_strucs):
+            G = create_ct_graph(seqs[x],'',newcolors)
+            graphs.append(G)
+
     
     positions = []
     for x in range(num_strucs):
 
-        pos = plotGraph(graphs[x],names[x],color,node_size,bases)
+        pos = plotGraph(graphs[x],names[x],color,node_size,bases,view)
         
         positions.append(pos)
 
     return
```

### Comparing `poseidon_rna-0.3/test/full__average.ct` & `poseidon_rna-0.4/test/full__average.ct`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.3/test/full__average.db` & `poseidon_rna-0.4/test/full__average.db`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.3/test/full__average__varna-color.txt` & `poseidon_rna-0.4/test/full__average__varna-color.txt`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.3/pyproject.toml` & `poseidon_rna-0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "poseidon-rna"
 authors = [
     {name="Adam Sychla"},
 ]
-description = "Structure Ensemble Inference by Sequencing, Mutation Identification, and Clustering of RNA (SEISMIC-RNA)"
+description = "Plotting RNA using Kamada-Kawai Graph Plotting Algorithm"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "GPL-3.0-only"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `poseidon_rna-0.3/PKG-INFO` & `poseidon_rna-0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: poseidon-rna
-Version: 0.3
-Summary: Structure Ensemble Inference by Sequencing, Mutation Identification, and Clustering of RNA (SEISMIC-RNA)
+Version: 0.4
+Summary: Plotting RNA using Kamada-Kawai Graph Plotting Algorithm
 Project-URL: Homepage, https://github.com/rouskinlab/poseidon-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/poseidon-rna/issues
 Author: Adam Sychla
 License: GPL-3.0-only
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

