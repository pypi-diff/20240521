# Comparing `tmp/pulpy-1.8.1.tar.gz` & `tmp/pulpy-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulpy-1.8.1.tar", last modified: Fri Feb 16 22:30:43 2024, max compression
+gzip compressed data, was "pulpy-1.8.2.tar", last modified: Tue May 21 20:07:00 2024, max compression
```

## Comparing `pulpy-1.8.1.tar` & `pulpy-1.8.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:30:43.437698 pulpy-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-16 22:30:34.000000 pulpy-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-16 22:30:43.437698 pulpy-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-16 22:30:34.000000 pulpy-1.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:30:43.429698 pulpy-1.8.1/pulpy/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:30:43.433698 pulpy-1.8.1/pulpy/grad/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/grad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/grad/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/grad/waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/linop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:30:43.433698 pulpy-1.8.1/pulpy/rf/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/adiabatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/b1sel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/multiband.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/optcont.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/ptx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    29753 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/slr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/rf/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/verse.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 22:30:34.000000 pulpy-1.8.1/pulpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:30:43.437698 pulpy-1.8.1/pulpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-16 22:30:43.000000 pulpy-1.8.1/pulpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-16 22:30:43.000000 pulpy-1.8.1/pulpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 22:30:43.000000 pulpy-1.8.1/pulpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-16 22:30:43.000000 pulpy-1.8.1/pulpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-02-16 22:30:34.000000 pulpy-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-16 22:30:43.437698 pulpy-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-16 22:30:34.000000 pulpy-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 22:30:43.433698 pulpy-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-16 22:30:34.000000 pulpy-1.8.1/tests/test_linop.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-16 22:30:34.000000 pulpy-1.8.1/tests/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-16 22:30:34.000000 pulpy-1.8.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:07:00.983848 pulpy-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34357 2024-05-21 20:06:56.000000 pulpy-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-21 20:07:00.983848 pulpy-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-21 20:06:56.000000 pulpy-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-21 20:06:56.000000 pulpy-1.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:07:00.979848 pulpy-1.8.2/pulpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:07:00.979848 pulpy-1.8.2/pulpy/grad/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/grad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/grad/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/grad/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/linop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:07:00.979848 pulpy-1.8.2/pulpy/rf/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/adiabatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/b1sel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/multiband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/optcont.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/ptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29761 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/slr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/rf/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/verse.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 20:06:56.000000 pulpy-1.8.2/pulpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:07:00.983848 pulpy-1.8.2/pulpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-21 20:07:00.000000 pulpy-1.8.2/pulpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-21 20:07:00.000000 pulpy-1.8.2/pulpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:07:00.000000 pulpy-1.8.2/pulpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 20:07:00.000000 pulpy-1.8.2/pulpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-21 20:06:56.000000 pulpy-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-21 20:07:00.983848 pulpy-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 20:06:56.000000 pulpy-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:07:00.979848 pulpy-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-21 20:06:56.000000 pulpy-1.8.2/tests/test_linop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-21 20:06:56.000000 pulpy-1.8.2/tests/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 20:06:56.000000 pulpy-1.8.2/tests/test_version.py
```

### Comparing `pulpy-1.8.1/pulpy/__init__.py` & `pulpy-1.8.2/pulpy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/grad/optim.py` & `pulpy-1.8.2/pulpy/grad/optim.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/grad/waveform.py` & `pulpy-1.8.2/pulpy/grad/waveform.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/io.py` & `pulpy-1.8.2/pulpy/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = ["signa", "ge_rf_params", "philips_rf_params", "siemens_rf"]
 
 
 def siemens_rf(
     pulse, rfbw, rfdurms, pulsename, minslice=0.5, maxslice=320.0, comment=None
 ):
-    """Write a .pta text file for Siemens PulseTool.
+    """Write a .pta text file for Siemens PulseTool. 
 
     Args:
         pulse (array): complex-valued RF pulse array with maximum of 4096
             points.
         rfbw (float): bandwidth of RF pulse in Hz
         rfdurms (float): duration of RF pulse in ms
         pulsename (string): '<FamilyName>.<PulseName>', e.g. 'Sigpy.SincPulse'
```

### Comparing `pulpy-1.8.1/pulpy/linop.py` & `pulpy-1.8.2/pulpy/linop.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/__init__.py` & `pulpy-1.8.2/pulpy/rf/__init__.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/adiabatic.py` & `pulpy-1.8.2/pulpy/rf/adiabatic.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/b1sel.py` & `pulpy-1.8.2/pulpy/rf/b1sel.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/multiband.py` & `pulpy-1.8.2/pulpy/rf/multiband.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/optcont.py` & `pulpy-1.8.2/pulpy/rf/optcont.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/ptx.py` & `pulpy-1.8.2/pulpy/rf/ptx.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/shim.py` & `pulpy-1.8.2/pulpy/rf/shim.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/rf/slr.py` & `pulpy-1.8.2/pulpy/rf/slr.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,15 +767,15 @@
     # calculate beta filter response
     B = sp.fft(b[:, 0], norm=None)
 
     if win_fact < z_pad_fact:
         win_len = (win_fact - 1) * n
         npad = n * z_pad_fact - win_fact * n
         # blackman window?
-        window = signal.blackman(int((win_fact - 1) * n))
+        window = signal.windows.blackman(int((win_fact - 1) * n))
         # split in half; stick N ones in the middle
         window = np.concatenate(
             (
                 window[0 : int(win_len / 2)],
                 np.ones(n),
                 window[int(win_len / 2) :],
             )
```

### Comparing `pulpy-1.8.1/pulpy/rf/util.py` & `pulpy-1.8.2/pulpy/rf/util.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy/sim.py` & `pulpy-1.8.2/pulpy/sim.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,22 +110,24 @@
             bt = bv * a + xp.conj(av) * b
             a = at
             b = bt
 
         return a, b
 
 
-def abrm_hp(rf, gamgdt, xx, dom0dt=0):
+def abrm_hp(rf, gamgdt, xx, dom0dt=0, b1=None):
     r"""1D RF pulse simulation, with non-simultaneous RF + gradient rotations.
 
     Args:
         rf (array): rf pulse samples in radians.
-        gamdt (array): gradient samples in radians/(units of xx).
+        gamgdt (array): gradient samples in radians/(units of xx).
         xx (array): spatial locations.
-        dom0dt (float): off-resonance phase in radians.
+        dom0dt (array): off-resonance phase in radians.
+        b1 (array): B1 at each spatial location, for each channel in rf.
+            b1 * rf should have units of radians
 
     Returns:
         2-element tuple containing
 
         - **a** (*array*): SLR alpha parameter.
         - **b** (*array*): SLR beta parameter.
 
@@ -134,31 +136,38 @@
         'Parameter Relations for the Shinnar-LeRoux Selective Excitation
         Pulse Design Algorithm'.
         IEEE Transactions on Medical Imaging, Vol 10, No 1, 53-65.
     """
 
     device = backend.get_device(rf)
     xp = device.xp
+
+    if b1 is None:
+        rf = rf.flatten()
+
     with device:
-        Ns = xp.shape(xx)
-        Ns = Ns[0]  # Ns: # of spatial locs
-        Nt = xp.shape(gamgdt)
-        Nt = Nt[0]  # Nt: # time points
+        Ns = xx.shape[0]  # Ns: # of spatial locs
+        Nt = gamgdt.shape[0]  # Nt: # time points
 
         a = xp.ones((Ns,))
         b = xp.zeros((Ns,))
 
         for ii in xp.arange(Nt):
             # apply phase accural
             z = xp.exp(-1j * (xx * gamgdt[ii,] + dom0dt))
             b = b * z
 
             # apply rf
-            C = xp.cos(xp.abs(rf[ii]) / 2)
-            S = 1j * xp.exp(1j * xp.angle(rf[ii])) * xp.sin(xp.abs(rf[ii]) / 2)
+            if b1 is None:
+                C = xp.cos(xp.abs(rf[ii]) / 2)
+                S = 1j * xp.exp(1j * xp.angle(rf[ii])) * xp.sin(xp.abs(rf[ii]) / 2)
+            else:
+                b1rf = b1 @ rf[:, ii]
+                C = xp.cos(xp.abs(b1rf) / 2)
+                S = 1j * xp.exp(1j * xp.angle(b1rf)) * xp.sin(xp.abs(b1rf) / 2)
             at = a * C - b * xp.conj(S)
             bt = a * S + b * C
 
             a = at
             b = bt
 
         z = xp.exp(1j / 2 * (xx * xp.sum(gamgdt, axis=0) + Nt * dom0dt))
```

### Comparing `pulpy-1.8.1/pulpy/verse.py` & `pulpy-1.8.2/pulpy/verse.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/pulpy.egg-info/SOURCES.txt` & `pulpy-1.8.2/pulpy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 pulpy/__init__.py
 pulpy/io.py
 pulpy/linop.py
```

### Comparing `pulpy-1.8.1/pyproject.toml` & `pulpy-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>61.0"]
 build-backend ="setuptools.build_meta"
 
 [project]
 name = "pulpy"
-version = "1.8.1"
+version = "1.8.2"
 authors = [
   { name="Jonathan Martin", email="jonathan.bach.martin@vumc.org" },
 ]
 description = "PulPy-Pulses in Python. A package for MRI/NMR RF pulse design"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pulpy-1.8.1/tests/test_linop.py` & `pulpy-1.8.2/tests/test_linop.py`

 * *Files identical despite different names*

### Comparing `pulpy-1.8.1/tests/test_sim.py` & `pulpy-1.8.2/tests/test_sim.py`

 * *Files identical despite different names*

