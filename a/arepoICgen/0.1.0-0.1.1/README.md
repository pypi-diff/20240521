# Comparing `tmp/arepoicgen-0.1.0.tar.gz` & `tmp/arepoicgen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arepoicgen-0.1.0.tar", last modified: Tue May 21 14:14:13 2024, max compression
+gzip compressed data, was "arepoicgen-0.1.1.tar", last modified: Tue May 21 17:08:30 2024, max compression
```

## Comparing `arepoicgen-0.1.0.tar` & `arepoicgen-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:14:13.657345 arepoicgen-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 14:14:13.657345 arepoicgen-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 14:14:13.657345 arepoicgen-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:14:13.653345 arepoicgen-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:14:13.657345 arepoicgen-0.1.0/src/arepoICgen/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/arepoOut.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/boxCreation.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/densityPerturbations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/generateICs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/lowDensityPadding.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/massAndEnergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/shapeTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-05-21 14:14:09.000000 arepoicgen-0.1.0/src/arepoICgen/turbulence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:14:13.657345 arepoicgen-0.1.0/src/arepoICgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 14:14:13.000000 arepoicgen-0.1.0/src/arepoICgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 14:14:13.000000 arepoicgen-0.1.0/src/arepoICgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:14:13.000000 arepoicgen-0.1.0/src/arepoICgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 14:14:13.000000 arepoicgen-0.1.0/src/arepoICgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:08:30.616999 arepoicgen-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-21 17:08:30.616999 arepoicgen-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 17:08:30.620999 arepoicgen-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:08:30.616999 arepoicgen-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:08:30.616999 arepoicgen-0.1.1/src/arepoICgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/arepoOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/boxCreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/densityPerturbations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/generateICs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/lowDensityPadding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/massAndEnergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/shapeTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-05-21 17:08:24.000000 arepoicgen-0.1.1/src/arepoICgen/turbulence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:08:30.616999 arepoicgen-0.1.1/src/arepoICgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-21 17:08:30.000000 arepoicgen-0.1.1/src/arepoICgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 17:08:30.000000 arepoicgen-0.1.1/src/arepoICgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:08:30.000000 arepoicgen-0.1.1/src/arepoICgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 17:08:30.000000 arepoicgen-0.1.1/src/arepoICgen.egg-info/top_level.txt
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/arepoOut.py` & `arepoicgen-0.1.1/src/arepoICgen/arepoOut.py`

 * *Files identical despite different names*

### Comparing `arepoicgen-0.1.0/src/arepoICgen/boxCreation.py` & `arepoicgen-0.1.1/src/arepoICgen/boxCreation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,107 @@
 # Needed libraries
 import numpy as np
 from random import random
 from numba import jit
 
+# Compiled loop to speed things up, this is slow in normal python for large ngas
 @jit(nopython=True)
-def tripleLoop(nx, ny, nz, pos, xmin, ymin, zmin, spacing, ngas):
-    # Looping through every particle and assigning its position
+def tripleLoop(nx, ny, nz, pos, spacing):
     npart = 0
     for i in range(0, nx):
        for j in range(0, ny):
             for k in range(0, nz):
                 # Assigning positions 
-                pos[0][npart] = xmin + (0.5 * spacing) + (i * spacing)
-                pos[1][npart] = ymin + (0.5 * spacing) + (j * spacing)
-                pos[2][npart] = zmin + (0.5 * spacing) + (k * spacing)
+                pos[0][npart] = (0.5 * spacing) + (i * spacing)
+                pos[1][npart] = (0.5 * spacing) + (j * spacing)
+                pos[2][npart] = (0.5 * spacing) + (k * spacing)
 
                 # Adding to counter
                 npart += 1
     return pos
 
 # Code to create particles in a box grid
-def boxGrid(ngas, bounds):
+def boxGrid(ngas, lengths, verbose=False):
     # Unpacking bounds
-    xmin = bounds[0]
-    xmax = bounds[1]
-    ymin = bounds[2]
-    ymax = bounds[3]
-    zmin = bounds[4]
-    zmax = bounds[5]
+    xLength = lengths[0]
+    yLength = lengths[1]
+    zLength = lengths[2]
 
     # Calculating the box volume
-    volume = (xmax-xmin) * (ymax-ymin) * (zmax-zmin)
-
-    # Printing the volume
-    print("Desired Volume: {:.2e}".format(volume))
+    volume = xLength * yLength * zLength
 
     # Determining average particle spacing
     spacing = (volume / ngas)**(1./3.)
 
     # Finding the number of grid points for each dimension
-    nx = np.int64((xmax-xmin)/spacing)
-    ny = np.int64((ymax-ymin)/spacing)
-    nz = np.int64((zmax-zmin)/spacing)
+    nx = np.int64(xLength/spacing)
+    ny = np.int64(yLength/spacing)
+    nz = np.int64(zLength/spacing)
 
     # Resetting the number of gas particles to the rounded version 
     ngas = nx * ny * nz
 
-    # Printing information
-    print("Number of points in each dimension: %s, %s, %s" % (nx, ny, nz))
-    print("New number of particles: %s" % ngas)
-    print("Spacing between points: {:.2f}".format(spacing))
-
     # Creating arrays for the particles
     pos = np.zeros((3, ngas), dtype=np.float64)
 
     # Looping through every particle and assigning its position
-    pos = tripleLoop(nx, ny, nz, pos, xmin, ymin, zmin, spacing, ngas)
+    pos = tripleLoop(nx, ny, nz, pos, spacing)
 
     # Setting the max dimensions to the maximum particle positions 
     xmin = np.min(pos[0])
     xmax = np.max(pos[0])
     ymin = np.min(pos[1])
     ymax = np.max(pos[1])
     zmin = np.min(pos[2])
     zmax = np.max(pos[2]) 
 
-    # Printing the new limits
-    print("New X Limits: {:.2f} - {:.2f}".format(xmin, xmax))
-    print("New Y Limits: {:.2f} - {:.2f}".format(ymin, ymax))
-    print("New Z Limits: {:.2f} - {:.2f}".format(zmin, zmax))
-
     # Calculating an updated volume using these
     volume = (xmax-xmin) * (ymax-ymin) * (zmax-zmin)
 
-    # Printing the volume
-    print("Box Grid Volume: {:.2e}".format(volume))
+    if verbose:
+        print("Number of points in each dimension: %s, %s, %s" % (nx, ny, nz))
+        print("New number of particles: %s" % ngas)
+        print("Spacing between points: {:.2f}".format(spacing))
+
+        print("New X Limits: {:.2f} - {:.2f}".format(xmin, xmax))
+        print("New Y Limits: {:.2f} - {:.2f}".format(ymin, ymax))
+        print("New Z Limits: {:.2f} - {:.2f}".format(zmin, zmax))
+
+        print("Box Grid Volume: {:.2e}".format(volume))
 
-    return pos, ngas, [xmin, xmax, ymin, ymax, zmin, zmax], volume
+    return pos, ngas, volume
 
 # Code to allocate particle positions randomly
-def boxRandom(ngas, bounds):
+def boxRandom(ngas, lengths, verbose=False):
     # Unpacking bounds
-    xmin = bounds[0]
-    xmax = bounds[1]
-    ymin = bounds[2]
-    ymax = bounds[3]
-    zmin = bounds[4]
-    zmax = bounds[5]
+    xLength = lengths[0]
+    yLength = lengths[1]
+    zLength = lengths[2]
     
     # Creating the particle array
     pos = np.zeros((3, int(ngas)), dtype=np.float64)
 
     # Calculating volume
-    volume = (xmax-xmin) * (ymax-ymin) * (zmax-zmin)
+    volume = xLength * yLength * zLength
 
     # Looping through the list of particles
     for i in range(ngas):
-        pos[0][i] = xmin + (xmax - xmin) * random()
-        pos[1][i] = ymin + (ymax - ymin) * random()
-        pos[2][i] = zmin + (zmax - zmin) * random()
+        pos[0][i] = xLength * random()
+        pos[1][i] = yLength * random()
+        pos[2][i] = zLength * random()
 
     return pos, volume
 
-def sphereRandom(ngas, radius):
+def sphereRandom(ngas, radius, verbose=False):
     # Creating particle array
     pos = np.zeros((3, ngas))
 
     # Calculating volume
     volume = (radius**3) *  (4. * np.pi) / 3.
 
-    # Printing values
-    print("Spherical Volume: {:.2e}".format(volume))
-
     # Allocating positions
     i = 0
     while i < ngas:
         x = -radius + 2. * radius * random()    
         y = -radius + 2. * radius * random()
         z = -radius + 2. * radius * random()
         r = np.sqrt(x**2 + y**2 + z**2)
@@ -136,15 +122,19 @@
     xmin = np.min(pos[0])
     xmax = np.max(pos[0])
     ymin = np.min(pos[1])
     ymax = np.max(pos[1])
     zmin = np.min(pos[2])
     zmax = np.max(pos[2]) 
 
-    # Printing the new limits
-    print("New X Limits: {:.2f} - {:.2f}".format(xmin, xmax))
-    print("New Y Limits: {:.2f} - {:.2f}".format(ymin, ymax))
-    print("New Z Limits: {:.2f} - {:.2f}".format(zmin, zmax))
+    if verbose:
+        # Printing values
+        print("Spherical Volume: {:.2e}".format(volume))
+
+        # Printing the new limits
+        print("New X Limits: {:.2f} - {:.2f}".format(xmin, xmax))
+        print("New Y Limits: {:.2f} - {:.2f}".format(ymin, ymax))
+        print("New Z Limits: {:.2f} - {:.2f}".format(zmin, zmax))
 
     return pos, volume
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/densityPerturbations.py` & `arepoicgen-0.1.1/src/arepoICgen/densityPerturbations.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,13 @@
         y = yCom - pos[1,i]
 
         # Work out the angle 
         phi = np.arctan2(y, x)
 
         # Work out what the mass should be here
         mass[i] = mass[i] * (1 + 0.5 * np.cos(2*phi))
-        
-    print("Boss-Bodenheimer Density Perturbation Applied")
 
     return pos, mass
 
 def densityGradient(pos, mass, lowerDensity=0.66, upperDensity=1.33):
     distance = pos[0] + np.max(pos[0])
     return lowerDensity * mass + (upperDensity-lowerDensity) * mass * (distance/np.max(distance))
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/lowDensityPadding.py` & `arepoicgen-0.1.1/src/arepoICgen/lowDensityPadding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Importing libraries
 import numpy as np
 from random import random 
 
 # Generic function for the padding
-def padGeneric(ngas, pos, vels, pMass, pIDs, pEnergy, volume, boxDims, gridType, tempFactor, paddingPercent=0.02, padDensity=0.01):
+def padGeneric(ngas, pos, vels, pMass, pIDs, pEnergy, volume, boxDims, gridType, tempFactor, paddingPercent=0.02, padDensity=0.01, verbose=False):
     # Use 2% of the number of particles to pad the box 
     nPaddingParticles = int(paddingPercent * ngas)
     print("Padding the box with %s new particles" % nPaddingParticles)
 
     # Create new arrays that are long enough for all the particles
     newPos = np.zeros((3, nPaddingParticles), dtype=np.float64)
     newVels = np.zeros((3, nPaddingParticles), dtype=np.float64)
@@ -55,18 +55,19 @@
     cloudMass = np.sum(pMass)
     cloudDensity = cloudMass / cloudVolume
     cloudDimensions = [xmin, xmax, ymin, ymax, zmin, zmax]
     cloudCentre = [xcom, ycom, zcom]
     cloudRadius = np.max([(xmax-xmin)/2, (ymax-ymin)/2, (zmax-zmin)/2])
 
     pc = 3.09e18
-    print("Cloud Density of {:.2e}".format(cloudDensity))
-    print("Cloud Centre at {:.2f},{:.2f},{:.2f}".format(xcom/pc, ycom/pc, zcom/pc))
-    print("Cloud has Dimensions: {:.2f}-{:.2f},{:.2f}-{:.2f},{:.2f}-{:.2f}".format(cloudDimensions[0]/pc, cloudDimensions[1]/pc, cloudDimensions[2]/pc, cloudDimensions[3]/pc, cloudDimensions[4]/pc, cloudDimensions[5]/pc))
-    print("Box has Dimensions: {:.2f}-{:.2f},{:.2f}-{:.2f},{:.2f}-{:.2f}".format(minDimensionX/pc, maxDimensionX/pc, minDimensionY/pc, maxDimensionY/pc, minDimensionZ/pc, maxDimensionZ/pc))
+    if verbose:
+        print("Cloud Density of {:.2e}".format(cloudDensity))
+        print("Cloud Centre at {:.2f},{:.2f},{:.2f}".format(xcom/pc, ycom/pc, zcom/pc))
+        print("Cloud has Dimensions: {:.2f}-{:.2f},{:.2f}-{:.2f},{:.2f}-{:.2f}".format(cloudDimensions[0]/pc, cloudDimensions[1]/pc, cloudDimensions[2]/pc, cloudDimensions[3]/pc, cloudDimensions[4]/pc, cloudDimensions[5]/pc))
+        print("Box has Dimensions: {:.2f}-{:.2f},{:.2f}-{:.2f},{:.2f}-{:.2f}".format(minDimensionX/pc, maxDimensionX/pc, minDimensionY/pc, maxDimensionY/pc, minDimensionZ/pc, maxDimensionZ/pc))
 
     # Setting the density of the particles within the cloud to this
     pRho = pRho * cloudDensity
 
     # Calculating mass of the particles we'll pad with 
     newParticleMass = (padDensity * cloudDensity) * (cloudVolume) / nPaddingParticles
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/massAndEnergy.py` & `arepoicgen-0.1.1/src/arepoICgen/massAndEnergy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # Importing libraries
 import numpy as np
 
 # Constants
 gasConstant = 8.31
 
 # Defining mass of the particles 
-def masses(ngas, totalMass):
+def masses(ngas, totalMass, verbose=False):
     # Calculate mass of each particle 
     particleMass = totalMass / ngas
 
     # Set array of particle masses
     pMass = np.ones(ngas, dtype=np.float64) * particleMass
 
-    # Printing the mass
-    print("Total desired mass: %s" % totalMass)
-    print("Initial particle mass: {:.5f}".format(particleMass))
+    if verbose:
+        # Printing the mass
+        print("Total desired mass: %s" % totalMass)
+        print("Initial particle mass: {:.5f}".format(particleMass))
 
     return pMass
 
 # Defining energy of the particles
-def thermalEnergy(ngas, temperature, mu):
+def thermalEnergy(ngas, temperature, mu, verbose=False):
     # Calculating internal energy
     energy = (3./2.) * temperature * gasConstant / mu 
 
     # Calculating a sound speed
     cs = np.sqrt(energy * 2./3.)
 
     # Allocating this energy to each particle
     pEnergy = np.ones(ngas, dtype=np.float64) * energy
 
-    # Printing values
-    print("Initial particle energy: {:.2f}".format(energy))
-    print("Initial sound speed: {:.2f}".format(cs))
+    if verbose:
+        # Printing values
+        print("Initial particle energy: {:.2f}".format(energy))
+        print("Initial sound speed: {:.2f}".format(cs))
 
-    return pEnergy, cs
+    return pEnergy
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/rotation.py` & `arepoicgen-0.1.1/src/arepoICgen/rotation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Importing libraries
 import numpy as np
 
 # Function to add solid body rotation
-def addRotation(pos, pMass, vels, beta):
+def addRotation(pos, pMass, vels, beta, verbose=False):
     # Find the centre of mass of the body
     mtot = np.sum(pMass) 
     xcom = np.sum(pMass * pos[0]) / mtot
     ycom = np.sum(pMass * pos[1]) / mtot
     zcom = np.sum(pMass * pos[2]) / mtot
 
     # Working out rmax of the sphere
@@ -25,11 +25,12 @@
     # Working out gravitational potential energy
     eGrav = (6.67e-8) * (3./5.) * (mtot**2) / rMax
  
     # Working out the rotational energy
     momentOfInteria = (2/5) * mtot * rMax**2
     eRot = (1/2) * momentOfInteria * omega**2
 
-    # Reporting the deviation from the desired beta value
-    print("Difference from desired beta: {:.2f}%".format(abs(100*(beta-eRot/eGrav)/beta)))
+    if verbose:
+        # Reporting the deviation from the desired beta value
+        print("Difference from desired beta: {:.2f}%".format(abs(100*(beta-eRot/eGrav)/beta)))
 
     return vels
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/shapeTypes.py` & `arepoicgen-0.1.1/src/arepoICgen/shapeTypes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,44 @@
 # Needed libraries
 import numpy as np
 
 # Function for a spherical cloud
-def sphericalCloud(pos, cloudSize, ngas, bounds):
-    # Getting the min and max positions
-    xmin = bounds[0]
-    xmax = bounds[1]
-    ymin = bounds[2]
-    ymax = bounds[3]
-    zmin = bounds[4]
-    zmax = bounds[5]
-
-    # Getting box sizes
-    dx = xmax - xmin
-    dy = ymax - ymin
-    dz = zmax - zmin
-
-    # Finding the radius of the central sphere
-    radius = np.abs(np.min([dx/2, dy/2, dz/2]))
-
-    # Fiding the central point
-    xcom = xmin + dx/2
-    ycom = ymin + dy/2
-    zcom = zmin + dz/2
-
+def sphericalCloud(pos, radius, ngas, verbose=False):
     # Only keeping the particles within the spherical region
     newPos = np.zeros((3, ngas), dtype=np.float64)
     ngasNew = 0
 
     for i in range(ngas):
         # Distance of each particle from centre
-        r = np.sqrt((pos[0,i] - xcom)**2 + (pos[1,i] - ycom)**2 + (pos[2,i] - zcom)**2)
+        r = np.sqrt((pos[0,i] - radius)**2 + (pos[1,i] - radius)**2 + (pos[2,i] - radius)**2)
 
         # Check if within sphere
         if r <= radius:
             # Assign new positions
-            newPos[0,ngasNew] = pos[0,i] - xcom
-            newPos[1,ngasNew] = pos[1,i] - ycom
-            newPos[2,ngasNew] = pos[2,i] - zcom
+            newPos[0,ngasNew] = pos[0,i] - radius
+            newPos[1,ngasNew] = pos[1,i] - radius
+            newPos[2,ngasNew] = pos[2,i] - radius
 
             # Update the number of particles inside the sphere
             ngasNew += 1
 
-    # Printing the change in particles
-    print("Number originally in box: %s" % ngas)
-    print("Number left in sphere: %s" % ngasNew)
-
     # Reallocating the position array
     pos = np.zeros((3, ngasNew), dtype=np.float64)
     pos[0] = newPos[0,0:ngasNew]
     pos[1] = newPos[1,0:ngasNew]
     pos[2] = newPos[2,0:ngasNew]
 
-    # Scaling the cloud to the desired size
-    pos = pos * (cloudSize/radius)
-
     # Checking the size etc
     xmin = np.min(pos[0])
     xmax = np.max(pos[0])
     ymin = np.min(pos[1])
     ymax = np.max(pos[1])
     zmin = np.min(pos[2])
     zmax = np.max(pos[2])
 
-    # Printing the new limits
-    print("Sphere X Limits: {:.2f} - {:.2f}".format(xmin, xmax))
-    print("Sphere Y Limits: {:.2f} - {:.2f}".format(ymin, ymax))
-    print("Sphere Z Limits: {:.2f} - {:.2f}".format(zmin, zmax))
-
     # Getting box sizes
     dx = xmax - xmin
     dy = ymax - ymin
     dz = zmax - zmin
 
     # Finding the radius of the central sphere
     radius = np.abs(np.min([dx/2, dy/2, dz/2]))
@@ -80,67 +47,77 @@
     xcom = xmin + dx/2
     ycom = ymin + dy/2
     zcom = zmin + dz/2
     
     # Calculating the volume
     volume = (4. * np.pi /3.) * radius**3
 
-    # Printing sphere information
-    print("Radius of the sphere: {:.2f}".format(radius))
-    print("Sphere COM: {:.2f},{:.2f},{:.2f}".format(xcom, ycom, zcom))
-    print("Sphere volume: {:.2e}".format(volume))
+    if verbose:
+        # Printing the change in particles
+        print("Number originally in box: %s" % ngas)
+        print("Number left in sphere: %s" % ngasNew)
+
+        # Printing the new limits
+        print("Sphere X Limits: {:.2f} - {:.2f}".format(xmin, xmax))
+        print("Sphere Y Limits: {:.2f} - {:.2f}".format(ymin, ymax))
+        print("Sphere Z Limits: {:.2f} - {:.2f}".format(zmin, zmax))
+
+        # Printing sphere information
+        print("Radius of the sphere: {:.2f}".format(radius))
+        print("Sphere COM: {:.2f},{:.2f},{:.2f}".format(xcom, ycom, zcom))
+        print("Sphere volume: {:.2e}".format(volume))
 
     return ngasNew, pos, volume
 
 # Function for an ellipsodial cloud
-def ellipsoidalCloud(ellipseLengths, ngas):
+def ellipsoidalCloud(lengths, ngas, verbose="False"):
     # Generate array for positions
     pos = np.zeros((3, ngas), dtype=np.float64)
 
     # Calculate radii bounds
-    xx = ellipseLengths[0]**2
-    yy = ellipseLengths[1]**2
-    zz = ellipseLengths[2]**2
+    xx = lengths[0]**2
+    yy = lengths[1]**2
+    zz = lengths[2]**2
 
     # Generate points on an ellipse
     i = 0
     while i < ngas:
         # Generate the x, y and z coordinates of the points
-        x = -ellipseLengths[0] + 2 * ellipseLengths[0] * np.random.random()
-        y = -ellipseLengths[1] + 2 * ellipseLengths[1] * np.random.random()
-        z = -ellipseLengths[2] + 2 * ellipseLengths[2] * np.random.random()
+        x = -lengths[0] + 2 * lengths[0] * np.random.random()
+        y = -lengths[1] + 2 * lengths[1] * np.random.random()
+        z = -lengths[2] + 2 * lengths[2] * np.random.random()
 
         # Check we've the right length
         if (x*x/xx + y*y/yy + z*z/zz) <= 1: 
             pos[0,i] = x
             pos[1,i] = y
             pos[2,i] = z
             i += 1
 
     # Work out volume
-    volume = (np.pi * 4/3) * (ellipseLengths[0] * ellipseLengths[1] * ellipseLengths[2])
+    volume = (np.pi * 4/3) * (lengths[0] * lengths[1] * lengths[2])
 
     return pos, volume
 
-def cylindricalCloud(ngas, radius, length):
+def cylindricalCloud(ngas, radius, lengths, verbose="False"):
     # Setup the positions arrays
     pos = np.zeros((3, ngas), dtype=np.float64)
 
     # Generate points of the cylnder
     i = 0
     while i < ngas:
         # Generate x (cylinder axis), y and z points of the cylinder
-        x = -0.5 * length + length * np.random.random()
+        x = -0.5 * lengths[0] + lengths[0] * np.random.random()
         y = - radius + 2 * radius * np.random.random()
         z = - radius + 2 * radius * np.random.random()
 
         # Check inside the cylinder
         if np.sqrt(y*y + z*z) <= radius:
             pos[0,i] = x
             pos[1,i] = y
             pos[2,i] = z
             i += 1
 
     # Work out volume
-    volume = np.pi * radius**2 * length
+    volume = np.pi * radius**2 * lengths[0]
     
     return pos, volume
```

### Comparing `arepoicgen-0.1.0/src/arepoICgen/turbulence.py` & `arepoicgen-0.1.1/src/arepoICgen/turbulence.py`

 * *Files identical despite different names*

