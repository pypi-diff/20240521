# Comparing `tmp/aggPy-0.1.5.tar.gz` & `tmp/aggpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggPy-0.1.5.tar", last modified: Wed Mar 13 16:23:02 2024, max compression
+gzip compressed data, was "aggpy-0.1.8.tar", last modified: Tue May 21 15:20:39 2024, max compression
```

## Comparing `aggPy-0.1.5.tar` & `aggpy-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 nvascone (241113) campus    (1313)        0 2024-03-13 16:23:02.000000 aggPy-0.1.5/
--rw-r--r--   0 nvascone (241113) campus    (1313)     1023 2024-03-12 22:20:05.000000 aggPy-0.1.5/LICENSE.txt
--rw-r--r--   0 nvascone (241113) campus    (1313)     1469 2024-03-13 16:23:02.000000 aggPy-0.1.5/PKG-INFO
--rw-r--r--   0 nvascone (241113) campus    (1313)     2306 2024-03-12 22:07:30.000000 aggPy-0.1.5/README.md
-drwxr-xr-x   0 nvascone (241113) campus    (1313)        0 2024-03-13 16:23:02.000000 aggPy-0.1.5/aggPy/
--rw-r--r--   0 nvascone (241113) campus    (1313)     2322 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/MDHbondMain.py
--rw-r--r--   0 nvascone (241113) campus    (1313)      528 2024-03-13 16:22:52.000000 aggPy-0.1.5/aggPy/__init__.py
--rw-r--r--   0 nvascone (241113) campus    (1313)      689 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/atom_map.py
--rw-r--r--   0 nvascone (241113) campus    (1313)     2407 2024-03-13 16:22:12.000000 aggPy-0.1.5/aggPy/frequency.py
--rw-r--r--   0 nvascone (241113) campus    (1313)     1839 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/initial_analysis.py
--rw-r--r--   0 nvascone (241113) campus    (1313)     3170 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/jsonreader.py
--rw-r--r--   0 nvascone (241113) campus    (1313)     2303 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/network2.py
--rw-r--r--   0 nvascone (241113) campus    (1313)     1667 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/timeCorr.py
--rw-r--r--   0 nvascone (241113) campus    (1313)     1932 2024-03-12 21:57:15.000000 aggPy-0.1.5/aggPy/workup.py
-drwxr-xr-x   0 nvascone (241113) campus    (1313)        0 2024-03-13 16:23:02.000000 aggPy-0.1.5/aggPy.egg-info/
--rw-r--r--   0 nvascone (241113) campus    (1313)     1469 2024-03-13 16:23:01.000000 aggPy-0.1.5/aggPy.egg-info/PKG-INFO
--rw-r--r--   0 nvascone (241113) campus    (1313)      358 2024-03-13 16:23:01.000000 aggPy-0.1.5/aggPy.egg-info/SOURCES.txt
--rw-r--r--   0 nvascone (241113) campus    (1313)        1 2024-03-13 16:23:01.000000 aggPy-0.1.5/aggPy.egg-info/dependency_links.txt
--rw-r--r--   0 nvascone (241113) campus    (1313)       17 2024-03-13 16:23:01.000000 aggPy-0.1.5/aggPy.egg-info/requires.txt
--rw-r--r--   0 nvascone (241113) campus    (1313)        6 2024-03-13 16:23:01.000000 aggPy-0.1.5/aggPy.egg-info/top_level.txt
--rw-r--r--   0 nvascone (241113) campus    (1313)       79 2024-03-13 16:23:02.000000 aggPy-0.1.5/setup.cfg
--rw-r--r--   0 nvascone (241113) campus    (1313)     1625 2024-03-13 16:22:39.000000 aggPy-0.1.5/setup.py
+drwxr-xr-x   0 nvascone (241113) campus    (1313)        0 2024-05-21 15:20:39.000000 aggpy-0.1.8/
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     1023 2024-05-21 15:16:59.000000 aggpy-0.1.8/LICENSE.txt
+-rw-r--r--   0 nvascone (241113) campus    (1313)     1488 2024-05-21 15:20:39.000000 aggpy-0.1.8/PKG-INFO
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)      912 2024-05-21 15:16:59.000000 aggpy-0.1.8/README.md
+drwxr-xr-x   0 nvascone (241113) campus    (1313)        0 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy/
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     2263 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/MDHbondMain.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)      528 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/__init__.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)      689 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/atom_map.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     2361 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/frequency.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     1821 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/initial_analysis.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     3170 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/jsonreader.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     2304 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/network2.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     1667 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/timeCorr.py
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     1974 2024-05-21 15:16:59.000000 aggpy-0.1.8/aggPy/workup.py
+drwxr-xr-x   0 nvascone (241113) campus    (1313)        0 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy.egg-info/
+-rw-r--r--   0 nvascone (241113) campus    (1313)     1488 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy.egg-info/PKG-INFO
+-rw-r--r--   0 nvascone (241113) campus    (1313)      358 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy.egg-info/SOURCES.txt
+-rw-r--r--   0 nvascone (241113) campus    (1313)        1 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy.egg-info/dependency_links.txt
+-rw-r--r--   0 nvascone (241113) campus    (1313)       17 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy.egg-info/requires.txt
+-rw-r--r--   0 nvascone (241113) campus    (1313)        6 2024-05-21 15:20:39.000000 aggpy-0.1.8/aggPy.egg-info/top_level.txt
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)       79 2024-05-21 15:20:39.000000 aggpy-0.1.8/setup.cfg
+-rwxr-xr-x   0 nvascone (241113) campus    (1313)     1625 2024-05-21 15:16:59.000000 aggpy-0.1.8/setup.py
```

### Comparing `aggPy-0.1.5/LICENSE.txt` & `aggpy-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aggPy-0.1.5/PKG-INFO` & `aggpy-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: aggPy
-Version: 0.1.5
+Version: 0.1.8
 Summary: Calculating aggregation with MDanalysis tools
 Home-page: https://github.com/Corcellilab/Phosphates/tree/main/aggPy
 Author: Noah Vasconez
 Author-email: nvascone@nd.edu
 License: Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. "
         " THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
-
-UNKNOWN
-
+Requires-Dist: MDAnalysis
+Requires-Dist: numpy
```

### Comparing `aggPy-0.1.5/aggPy/MDHbondMain.py` & `aggpy-0.1.8/aggPy/MDHbondMain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import MDAnalysis as mda
 import numpy as np
 import aggPy.network2   
 
-def hbond(topology=[],donors=[],hydrogens=[],acceptors=[],HbondParm=[],box=[],pre_allo=[],mol_delim='resid',XYZ=[False]):
+def hbond(topology=[],donors=[],hydrogens=[],acceptors=[],HbondParm=[],box=[],pre_allo=[],XYZ=[False]):
     if XYZ[0] == True:
         xyz_string = ''
         atom_map = XYZ[1]
         XYZfilename = XYZ[2]
         num_atoms = 0
 
     dist = mda.lib.distances.distance_array(hydrogens.positions,acceptors.positions,
             box=box,result=pre_allo)
     index = np.column_stack(np.where((dist >= HbondParm[0]) & (dist <= HbondParm[1])))
 
     output = {'Distance':[],'Angle':[],'Network':[]}
     for i in index:
-        if getattr(hydrogens[i[0]], mol_delim) != getattr(acceptors[i[1]], mol_delim):
+        if hydrogens[i[0]].resid != acceptors[i[1]].resid:
             hydrogen = hydrogens[i[0]]
             acceptor = acceptors[i[1]]
             distance = dist[i[0]][i[1]]
             bonded = hydrogen.bonds[0]
-            h_bond_atom = bonded[0]
+            h_bond_atom = bonded.partner(hydrogen)
             angle = (mda.lib.distances.calc_angles(h_bond_atom.position,hydrogen.position,acceptor.position,
                 box=box))         #radians
             if angle > HbondParm[2]:
                 output['Distance'].append(distance)
                 output['Angle'].append(angle)
                 output['Network'].append((hydrogen.resid,acceptor.resid))
 
             if XYZ[0] == True:
-                rez = [getattr(h_bond_atom, mol_delim), getattr(acceptor, mol_delim)]
+                rez = [h_bond_atom.resid, acceptor.resid]
                 for i in range(0,len(rez)):
                     rez_h = rez[i]
                     num_atoms += len(topology[rez_h])
                     for atom in topology[rez_h]:
                         symbol = atom_map[atom.type]
                         pos = atom.position
                         xyz_string += f'{symbol} {pos[0]} {pos[1]} {pos[2]}\n'
```

### Comparing `aggPy-0.1.5/aggPy/__init__.py` & `aggpy-0.1.8/aggPy/__init__.py`

 * *Files identical despite different names*

### Comparing `aggPy-0.1.5/aggPy/atom_map.py` & `aggpy-0.1.8/aggPy/atom_map.py`

 * *Files identical despite different names*

### Comparing `aggPy-0.1.5/aggPy/frequency.py` & `aggpy-0.1.8/aggPy/frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
             topology = self.topology,
             donors = self.donors,
             hydrogens = self.hydrogens,
             acceptors = self.acceptors,
             HbondParm = self.HbondParm,
             box = self.box,
             pre_allo = self.pre_allo,
-            mol_delim = self.mol_deliminator,
             XYZ = [eval(self.XYZ[0]), self.atom_map, f'{self.XYZ[1].strip()}.xyz']
         )
         
         if self.run_length == 'n':
             self.length = int((self.end_frame - self.start_frame / self.frame_dt))
             hbonds.run(start=self.start_frame, stop=self.end_frame, step=self.frame_dt)
         else:
```

### Comparing `aggPy-0.1.5/aggPy/initial_analysis.py` & `aggpy-0.1.8/aggPy/initial_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     pre_allo = np.zeros([len(hydrogens),len(acceptors)])
 
     print(f'Total atoms: {len(u.atoms)}')
     print(f'{len(hydrogens)} hydrogens of type {set(hydrogens.types)} found')
     print(f'{len(acceptors)} acceptors type {set(acceptors.types)} found')
     print(f'{len(donors)} donors type {set(donors.types)} found')
 
-    topology = u.atoms.groupby(f'{self.mol_deliminator}s') 
+    topology = u.atoms.groupby('resids') 
 
     self.universe = u
     self.box = box
     self.hydrogens = hydrogens
     self.donors = donors
     self.acceptors = acceptors
     self.pre_allo = pre_allo
```

### Comparing `aggPy-0.1.5/aggPy/jsonreader.py` & `aggpy-0.1.8/aggPy/jsonreader.py`

 * *Files identical despite different names*

### Comparing `aggPy-0.1.5/aggPy/network2.py` & `aggpy-0.1.8/aggPy/network2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def dij(adj_list, visited, node, result, key):
     visited.add(node)
     result[key].append(node)
     for neighbor in adj_list[node]:
         if neighbor not in visited:
             dij(adj_list, visited, neighbor, result, key)
 
-def connectivity(data,nodes):
+def connectivity(data, nodes):
     data = np.tril(data)
     z = np.nonzero(data)
     agg_tuple = [tuple((row,col)) for row, col in zip(z[1],z[0])]
 
     adj_list = {k: [] for k in range(len(data))}
     for x, y in agg_tuple:
         try:
```

### Comparing `aggPy-0.1.5/aggPy/timeCorr.py` & `aggpy-0.1.8/aggPy/timeCorr.py`

 * *Files identical despite different names*

### Comparing `aggPy-0.1.5/aggPy/workup.py` & `aggpy-0.1.8/aggPy/workup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,24 @@
             except AttributeError: print('Attr Error')
         return v0
     else:
         print('Variable format not dict or list')
 
 #########
 def average(self, variable):
-    agg = self.aggregate(variable)
+    agg = self.aggregate(self, variable)
     T = type(getattr(self.result0, variable))
     if T == dict:
         for k,v in agg.items():
             agg[k] = v/self.length
     elif T == list:
         agg = sum(agg) / self.length
 
     setattr(self, f'{variable}Avg', agg)
+    return agg
 
 #########
 def std_dev(self, variable, bin_width=1):
     cn_group = {}
     for i in range(0, self.length):
         for k in getattr(getattr(self, f'result{i}'), variable).keys():
             try: cn_group[k].append(getattr(getattr(self, f'result{i}'), variable)[k])
@@ -51,11 +52,12 @@
             x = np.mean(cn_group[k][t:t+bin_width])
             bin_values.append(x)
         bin_values = np.array(bin_values)
         bin_values[np.isnan(bin_values)] = 0
         trj_stdev[k] = np.std(bin_values)
 
     setattr(self, f'{variable}Stdev', trj_stdev)
+    return trj_stdev
 
 ##########
```

### Comparing `aggPy-0.1.5/aggPy.egg-info/PKG-INFO` & `aggpy-0.1.8/aggPy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: aggPy
-Version: 0.1.5
+Version: 0.1.8
 Summary: Calculating aggregation with MDanalysis tools
 Home-page: https://github.com/Corcellilab/Phosphates/tree/main/aggPy
 Author: Noah Vasconez
 Author-email: nvascone@nd.edu
 License: Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. "
         " THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
-
-UNKNOWN
-
+Requires-Dist: MDAnalysis
+Requires-Dist: numpy
```

### Comparing `aggPy-0.1.5/setup.py` & `aggpy-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
         name='aggPy',
-        version='0.1.5',
+        version='0.1.8',
         description='Calculating aggregation with MDanalysis tools',
         url='https://github.com/Corcellilab/Phosphates/tree/main/aggPy',
         author='Noah Vasconez',
         author_email='nvascone@nd.edu',
         license= 'Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. "\n" THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.',
     packages=['aggPy'],
     install_requires=['MDAnalysis',
```

