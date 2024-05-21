# Comparing `tmp/bayesian_average-0.1.7.tar.gz` & `tmp/bayesian_average-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian_average-0.1.7.tar", last modified: Sat May  4 11:23:01 2024, max compression
+gzip compressed data, was "bayesian_average-0.2.1.tar", last modified: Tue May 21 07:43:58 2024, max compression
```

## Comparing `bayesian_average-0.1.7.tar` & `bayesian_average-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-04 11:23:01.098336 bayesian_average-0.1.7/
--rw-rw-r--   0 martino    (501) staff       (20)     1274 2024-03-28 16:44:26.000000 bayesian_average-0.1.7/LICENSE.txt
--rw-r--r--   0 martino    (501) staff       (20)     4156 2024-05-04 11:23:01.098100 bayesian_average-0.1.7/PKG-INFO
--rw-r--r--   0 martino    (501) staff       (20)     3955 2024-05-04 11:16:11.000000 bayesian_average-0.1.7/README.md
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-04 11:23:01.097133 bayesian_average-0.1.7/bayesian_average/
--rw-r--r--   0 martino    (501) staff       (20)      993 2024-05-04 11:01:49.000000 bayesian_average-0.1.7/bayesian_average/__init__.py
--rw-r--r--   0 martino    (501) staff       (20)       21 2024-05-04 11:02:49.000000 bayesian_average-0.1.7/bayesian_average/_version.py
--rw-r--r--   0 martino    (501) staff       (20)     6467 2024-05-02 08:29:12.000000 bayesian_average-0.1.7/bayesian_average/average.py
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-04 11:23:01.097874 bayesian_average-0.1.7/bayesian_average.egg-info/
--rw-r--r--   0 martino    (501) staff       (20)     4156 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/PKG-INFO
--rw-r--r--   0 martino    (501) staff       (20)      276 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/SOURCES.txt
--rw-r--r--   0 martino    (501) staff       (20)        1 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/dependency_links.txt
--rw-r--r--   0 martino    (501) staff       (20)       17 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/top_level.txt
--rw-r--r--   0 martino    (501) staff       (20)       38 2024-05-04 11:23:01.098387 bayesian_average-0.1.7/setup.cfg
--rw-r--r--   0 martino    (501) staff       (20)      622 2024-05-04 11:22:52.000000 bayesian_average-0.1.7/setup.py
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-21 07:43:58.799442 bayesian_average-0.2.1/
+-rw-rw-r--   0 martino    (501) staff       (20)     1274 2024-03-28 16:44:26.000000 bayesian_average-0.2.1/LICENSE.txt
+-rw-r--r--   0 martino    (501) staff       (20)     5623 2024-05-21 07:43:58.799241 bayesian_average-0.2.1/PKG-INFO
+-rw-r--r--   0 martino    (501) staff       (20)     5422 2024-05-15 21:36:25.000000 bayesian_average-0.2.1/README.md
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-21 07:43:58.798334 bayesian_average-0.2.1/bayesian_average/
+-rw-r--r--   0 martino    (501) staff       (20)     1219 2024-05-15 15:15:35.000000 bayesian_average-0.2.1/bayesian_average/__init__.py
+-rw-r--r--   0 martino    (501) staff       (20)       21 2024-05-13 07:58:43.000000 bayesian_average-0.2.1/bayesian_average/_version.py
+-rw-r--r--   0 martino    (501) staff       (20)     8890 2024-05-16 04:57:51.000000 bayesian_average-0.2.1/bayesian_average/average.py
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-21 07:43:58.799046 bayesian_average-0.2.1/bayesian_average.egg-info/
+-rw-r--r--   0 martino    (501) staff       (20)     5623 2024-05-21 07:43:58.000000 bayesian_average-0.2.1/bayesian_average.egg-info/PKG-INFO
+-rw-r--r--   0 martino    (501) staff       (20)      276 2024-05-21 07:43:58.000000 bayesian_average-0.2.1/bayesian_average.egg-info/SOURCES.txt
+-rw-r--r--   0 martino    (501) staff       (20)        1 2024-05-21 07:43:58.000000 bayesian_average-0.2.1/bayesian_average.egg-info/dependency_links.txt
+-rw-r--r--   0 martino    (501) staff       (20)       17 2024-05-21 07:43:58.000000 bayesian_average-0.2.1/bayesian_average.egg-info/top_level.txt
+-rw-r--r--   0 martino    (501) staff       (20)       38 2024-05-21 07:43:58.799478 bayesian_average-0.2.1/setup.cfg
+-rw-r--r--   0 martino    (501) staff       (20)      622 2024-05-04 11:22:52.000000 bayesian_average-0.2.1/setup.py
```

### Comparing `bayesian_average-0.1.7/LICENSE.txt` & `bayesian_average-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bayesian_average-0.1.7/PKG-INFO` & `bayesian_average-0.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: bayesian_average
-Version: 0.1.7
+Version: 0.2.1
 Summary: __doc__
 Author: Marleen Maxton, Martino Trassinelli
 License: X11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Bayesian average
 
 ### Version:
-0.1.7
+0.2.0
 
 ### Authors
 Martino Trassinelli\
 CNRS, Institute of NanoSciences of Paris\
-email: trassinelli AT insp.jussieu.fr\
-email: m.trassinelli AT gmail.com
+emails: trassinelli AT cnrs.fr, m.trassinelli AT gmail.com
 
 Marleen Maxton\
 Max Planck Institute Heidelberg\
-email:
 
 ### Homepage
 https://github.com/martinit18/bayesian_average
 
 
 ### License
 Type: X11, see `LICENCE.txt`
@@ -41,47 +39,79 @@
 It is obtained by the marginalization on $\sigma'$, this result in a modified probability distribution for each $x_i$ that still depens on $\sigma_i$.
 Two different priors are proposed for $\sigma'$: the non-informative Jeffreys' prior $p(\sigma') \propto 1/ \sigma'$ (more precisely its limit, see Ref.[1]), and a modified version of it $p(\sigma') \propto 1/ (\sigma')^2$ proposed in Ref.[2].
 
 For both priors, the weighted average and its associated uncertainty are obtained numerically using `basinhopping` minimisation algorithm.
 
 In addition, the standard (inverse-variance) weighted average is also available for possible comparisons.
 
+## How to install it
+
+In your terminal, run
+```
+pip install bayesian_average
+```
+
 ## How to use it
-For the calculation of the Jeffreys' weighted average (see below for other averages)
+For the calculation of the weighted average just type in your python shell
 ```
 import bayesian_average as ba
-ba.jwa(data,sigma)
+ba.average(data,sigma)
 ```
 where `data` is a ntuple of data and `sigma` is the associated uncertainty of the same dimension.
+The default average mode is the one assuming a Jeffreys' prior `jeffreys`. 
+The other available are the `conservative`, `standard`, `birge`, which can be speficied by the keyword `mode`, like
+```
+ba.average(data,sigma, mode='conservative')
+```
+Details on the different method are presented below.
+
 The typical output is
 ```
 (6.6742395674538315, 9.74833292573106e-5)
 ```
-where the first number is the weighted average and the second one is the estimated final uncertainty 
+where the first number is the weighted average and the second one is the estimated final uncertainty.
+
+
+To plot the resulting probability distribution, the final weighted average and the input data:
+```
+ba.plot_average(data,sigma)
+```
+The default mode present the Jeffreys' vinal weighted average value and the associated distribution in log-scale. 
+To select other choices of weighted averages, take out the associated data point, normalise the associated distribution and/or plot them linerarly, additional options are available, like
 
-To plot the resulting probability distribution, the final weighted average and the input data (optionally)
 ```
-ba.plot_average(data,sigma,jwa_val=True,plot_data=True)
+ba.plot_average(data,sigma,jeffreys_val=True,jeffreys_like=True,plot_data=True,)
 ```
-The option `jwa_val=True` is on on as default. `plot_data=True` show the input data in addition.
+The option `xxx_val=True` display the value of the final weighted average of the `xxx` method. \
+`xxx_like=True` display the value of the final likelihood distribution (in log-scale by default). \
+`plot_data=True` show the input data in addition.
 
 ## Details of the vailable weighted averages
 
-- `jwa`: **Jeffreys weighted average** (main average, RECOMENDED, see Ref.[1]).\
+- `jeffreys`: **Jeffreys weighted average** (default average, RECOMENDED, see Ref.[1]).\
     The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to $1/\sigma'$.
     Because of the non-normalisability of the final probability distribution, this weighted average results 
     correspond to the  limit case with prior bounds $[\sigma, \sigma_\mathrm{max}]$ with $\sigma_\mathrm{max} \to \infty$ and where $\sigma$ is the value provided by the user.
     The final probability distribution is, however not a proper probability distribution.
-- `cwa`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
+- `cons`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
     The priors of the real uncertainty value are proportional to $\sigma/(\sigma')^2$, where $\sigma$ is the value provided by the user.
     The bounds of the prior are $[\sigma, \sigma_\mathrm{max}]$.
     This is a modified and normalisable version of the non-informative Jeffeys' prior.
-- `wa`: **Standard weighted average**\
+- `standard`: **Standard weighted average**\
     The standard inverse-variance weighted average useful for comparisons.
-
+- `birge`: **Standard weighted average corrected with the Birge ratio**\
+    The uncertainty of the final average is enanched by a factor proportional to the $\chi^2$ of the data and the weighted average if $\chi^2 > 1$, following Ref.[3].
 
 
 
 ## Refere articles:
 [1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* \
-[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
+[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press\
+[3]	R. T. Birge, *The Calculation of Errors by the Method of Least Squares*, Phys. Rev. **40**, 207 (1932)
+
+## Version history
+
+- 0.2: rearrangement of the average function(s),
+Birge ratio added
+- 0.1.5: First version aviable in github with documentation
+- 0.0.1: First version published in pypi with conservative, jeffreys' and standard weighted averages
```

### Comparing `bayesian_average-0.1.7/README.md` & `bayesian_average-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # Bayesian average
 
 ### Version:
-0.1.7
+0.2.0
 
 ### Authors
 Martino Trassinelli\
 CNRS, Institute of NanoSciences of Paris\
-email: trassinelli AT insp.jussieu.fr\
-email: m.trassinelli AT gmail.com
+emails: trassinelli AT cnrs.fr, m.trassinelli AT gmail.com
 
 Marleen Maxton\
 Max Planck Institute Heidelberg\
-email:
 
 ### Homepage
 https://github.com/martinit18/bayesian_average
 
 
 ### License
 Type: X11, see `LICENCE.txt`
@@ -32,47 +30,79 @@
 It is obtained by the marginalization on $\sigma'$, this result in a modified probability distribution for each $x_i$ that still depens on $\sigma_i$.
 Two different priors are proposed for $\sigma'$: the non-informative Jeffreys' prior $p(\sigma') \propto 1/ \sigma'$ (more precisely its limit, see Ref.[1]), and a modified version of it $p(\sigma') \propto 1/ (\sigma')^2$ proposed in Ref.[2].
 
 For both priors, the weighted average and its associated uncertainty are obtained numerically using `basinhopping` minimisation algorithm.
 
 In addition, the standard (inverse-variance) weighted average is also available for possible comparisons.
 
+## How to install it
+
+In your terminal, run
+```
+pip install bayesian_average
+```
+
 ## How to use it
-For the calculation of the Jeffreys' weighted average (see below for other averages)
+For the calculation of the weighted average just type in your python shell
 ```
 import bayesian_average as ba
-ba.jwa(data,sigma)
+ba.average(data,sigma)
 ```
 where `data` is a ntuple of data and `sigma` is the associated uncertainty of the same dimension.
+The default average mode is the one assuming a Jeffreys' prior `jeffreys`. 
+The other available are the `conservative`, `standard`, `birge`, which can be speficied by the keyword `mode`, like
+```
+ba.average(data,sigma, mode='conservative')
+```
+Details on the different method are presented below.
+
 The typical output is
 ```
 (6.6742395674538315, 9.74833292573106e-5)
 ```
-where the first number is the weighted average and the second one is the estimated final uncertainty 
+where the first number is the weighted average and the second one is the estimated final uncertainty.
+
+
+To plot the resulting probability distribution, the final weighted average and the input data:
+```
+ba.plot_average(data,sigma)
+```
+The default mode present the Jeffreys' vinal weighted average value and the associated distribution in log-scale. 
+To select other choices of weighted averages, take out the associated data point, normalise the associated distribution and/or plot them linerarly, additional options are available, like
 
-To plot the resulting probability distribution, the final weighted average and the input data (optionally)
 ```
-ba.plot_average(data,sigma,jwa_val=True,plot_data=True)
+ba.plot_average(data,sigma,jeffreys_val=True,jeffreys_like=True,plot_data=True,)
 ```
-The option `jwa_val=True` is on on as default. `plot_data=True` show the input data in addition.
+The option `xxx_val=True` display the value of the final weighted average of the `xxx` method. \
+`xxx_like=True` display the value of the final likelihood distribution (in log-scale by default). \
+`plot_data=True` show the input data in addition.
 
 ## Details of the vailable weighted averages
 
-- `jwa`: **Jeffreys weighted average** (main average, RECOMENDED, see Ref.[1]).\
+- `jeffreys`: **Jeffreys weighted average** (default average, RECOMENDED, see Ref.[1]).\
     The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to $1/\sigma'$.
     Because of the non-normalisability of the final probability distribution, this weighted average results 
     correspond to the  limit case with prior bounds $[\sigma, \sigma_\mathrm{max}]$ with $\sigma_\mathrm{max} \to \infty$ and where $\sigma$ is the value provided by the user.
     The final probability distribution is, however not a proper probability distribution.
-- `cwa`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
+- `cons`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
     The priors of the real uncertainty value are proportional to $\sigma/(\sigma')^2$, where $\sigma$ is the value provided by the user.
     The bounds of the prior are $[\sigma, \sigma_\mathrm{max}]$.
     This is a modified and normalisable version of the non-informative Jeffeys' prior.
-- `wa`: **Standard weighted average**\
+- `standard`: **Standard weighted average**\
     The standard inverse-variance weighted average useful for comparisons.
-
+- `birge`: **Standard weighted average corrected with the Birge ratio**\
+    The uncertainty of the final average is enanched by a factor proportional to the $\chi^2$ of the data and the weighted average if $\chi^2 > 1$, following Ref.[3].
 
 
 
 ## Refere articles:
 [1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* \
-[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
+[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press\
+[3]	R. T. Birge, *The Calculation of Errors by the Method of Least Squares*, Phys. Rev. **40**, 207 (1932)
+
+## Version history
+
+- 0.2: rearrangement of the average function(s),
+Birge ratio added
+- 0.1.5: First version aviable in github with documentation
+- 0.0.1: First version published in pypi with conservative, jeffreys' and standard weighted averages
```

### Comparing `bayesian_average-0.1.7/bayesian_average/__init__.py` & `bayesian_average-0.2.1/bayesian_average/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from .average import jwa, cwa, wa, plot_average
+from .average import average, plot_average
 from ._version import __version__
 
 __doc__="""
 Python package to calculate the weighted average with Bayesian methods.
 The proposed weighted average is particularly adapted to inconsistent
 data and/or for the presence of outliers, which can both false the 
 results of standard methods.
 For each data point, a normal disrtribution is considered with the 
 provided sigma value taken as lower bound for the *real* possibly 
 larger uncertainty sigma' and marginalizing on its possible values.
-A non-informative Jeffreys' prior is considered for sigma' as default (`jwa').
-In addition, a modified Jeffreys' prior from Sivia 2004 (`cwa`) and the 
-standard weigted average (`wa`) are proposed.
+A non-informative Jeffreys' prior is considered for sigma' as default (`jeffreys').
+In addition, a modified Jeffreys' prior from Sivia 2004 (`cons`), the 
+standard weigted average (`standard`) based on inverse-invariance 
+and the standard weighted average uncertainty corrected by the Birge 
+(`birge`) ratio are proposed.
 
 References:
 [1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* \
-[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
+[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press\
+[3] R.T. Birge, *The Calculation of Errors by the Method of Least Squares*, Phys. Rev. **40**, 207 (1932)
 
 
 """
```

### Comparing `bayesian_average-0.1.7/bayesian_average/average.py` & `bayesian_average-0.2.1/bayesian_average/average.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,179 @@
 import numpy as np
 from sympy import log, exp, diff, lambdify, sqrt, pi, erf
 from sympy.abc import mu
 from scipy.optimize import basinhopping
-from matplotlib.pyplot import errorbar, legend, ylabel, show, axvline, plot, gca
+from matplotlib.pyplot import errorbar, legend, ylabel, show, axvline, axvspan, plot, gca
+from sys import exit
 
+linestyle = {"markeredgewidth":1, "elinewidth":1, "capsize":2,"markersize":2}
 
-def wa(data, sigma):
-    """
-    Standard invariance inverse weighted average.
-    Attention! In this case the scattering of the data is not included in the final uncertainty
-    """
-    weights = 1 / np.array(sigma)**2
-    av_value = np.average(data, weights = weights) #find minima of negative loglikelihood
-    sig_value = 1/np.sqrt(np.sum(weights)) #calculate sigma        
-    return av_value, sig_value
+############################################################################################
 
-def cwa(data, sigma):    
+def average(data, sigma, mode = 'jeffreys'):
     """
-    Conservative weighted average proposed by Sivia in 2004 (see references in README file).
-    The priors of the real uncertainty value are proportional to sigma_0/sigma^2, where sigma_0 is the value provided by the user
-    The bounds of the prior are [sigma_0, infinite].
-    This is a modified and normalisable version of the non-informative Jeffeys' prior.
-    """
-    loglike = np.sum([log((1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)]) #loglikelihood function
-    ddloglike = diff(loglike, mu, 2) #second derivative
-    negloglike = lambdify(mu, -loglike)
-    av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
-    sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)) #calculate sigma        
-    return av_value, sig_value
+    Weighted average from the inputs
+    - data, an array of values
+    - sigma, the corresponding associated error bars
 
-def jwa(data, sigma):    
-    """
-    Jeffreys weighted average proposed by Trassinelli and Maxton in 2024 (see references in README file).
+    
+    Different type of average are available and can be select with 'mode' option.
+    The available ones are:
+
+    - 'jeffreys' (default): Jeffreys weighted average proposed by Trassinelli and Maxton in 2024 (see references in README file).
     The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to 1/sigma'.
     Because of the non-normalisability of the final probability distribution, this weighted average results 
     correspond to the  limit case with prior bounds [sigma, sigma_max] with sigma_max -> infinite. 
     The final probability distribution is, however not a proper probability distribution.
+    
+    - 'cons': Conservative weighted average proposed by Sivia in 2004 (see references in README file).
+    The priors of the real uncertainty value are proportional to sigma_0/sigma^2, where sigma_0 is the value provided by the user
+    The bounds of the prior are [sigma_0, infinite].
+    This is a modified and normalisable version of the non-informative Jeffeys' prior.
+
+    - 'standard': Standard invariance-inverse weighted average.
+    Attention! In this case the scattering of the data is not included in the final uncertainty.
+
+    - 'birge': Standard invariance-inverse weighted average with uncertainty corrected by the Birge ratio.
     """
-    loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
-    ddloglike = diff(loglike, mu, 2) #second derivative
-    negloglike = lambdify(mu, -loglike)
-    av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
-    sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)).evalf() #calculate sigma        
+    
+    # Check the data size
+    if np.size(data) != np.size(sigma):
+        exit('The dimension of the two input arrays are different. Please change it.')
+        
+    # Select the type of average
+    if mode  == 'standard' or mode == 'birge':
+        weights = 1 / np.array(sigma)**2
+        av_value = np.average(data, weights = weights) #find minima of negative loglikelihood
+        sig_value = 1/np.sqrt(np.sum(weights)) #calculate sigma    
+        if mode == 'birge':
+            chi2 = 0.
+            for i in range(np.size(data)):
+                chi2 = ( data[i] - av_value )**2 / sigma[i]**2 + chi2
+                #print((data[i] - av_value)/sigma[i], chi2)
+            birge_ratio = sqrt (chi2 / ( np.size(data) - 1))
+            print('Birge ratio = ', birge_ratio)
+            if birge_ratio > 1.: sig_value = sig_value * birge_ratio
+    elif mode == 'jeffreys' or mode == 'cons':
+        if mode == 'jeffreys':
+            loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) 
+                              for x_temp, s_temp in zip(data, sigma)])
+        elif mode == 'cons':
+            loglike = np.sum([log((1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) 
+                              for x_temp, s_temp in zip(data, sigma)]) #loglikelihood function
+        ddloglike = diff(loglike, mu, 2) #second derivative
+        negloglike = lambdify(mu, -loglike)
+        av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
+        sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)).evalf() #calculate sigma 
+    else:
+        exit('Please enter a valid average mode')
+    
     return av_value, sig_value
 
-def plot_average(data, sigma, plot_data = False, wa_val = False, cwa_val = False, jwa_val = True, 
-                 wa_loglike = False, cwa_loglike = False, jwa_loglike = True, 
-                 legendon = True, showon = False, normalize = False):
+#####################################################################################################
+
+def plot_average(data, sigma, plot_data = False, 
+                 jeffreys_val = True, cons_val = False, standard_val = False, 
+                 jeffreys_like = True, cons_like = False, standard_like = False, 
+                 legendon = True, showon = False, linear = False, normalize = False):
     """
     This is the main plot function of the library.
 
     Three weighted average are available:
-        - wa: standard weigted average
-        - jwa: Jeffreys weighted average
-        - cwa: conservative weighted average
+        - 'jeffreys': Jeffreys weighted average
+        - 'cons': conservative weighted average
+        - 'standard': standard inverse-variance weigted average
 
     Please select the items you want to plot.
-    xxx indicates wa, jwa or cwa.
         - plot_data: plot the input data with the input errorbar
         - xxx_val: plot the weighted average and the corresponding uncertainty
         - xxx_like: plot the corresponding likelihood
 
-    To have normalised curves of likelihood put `normalize=True'
+    with 'xxx' equal one of the available weighted average type listed above.
+
+    To have normalised curves of likelihood put 'normalize = True'
+
+    To have likelihood values in linear scale, put 'linear = True'
+
+    To take out the legend, put 'legendon = False'
+
+    In case the graph does not show up, try the option 'showon = True'
 
     """
 
-    if not (plot_data or wa_val or cwa_val or jwa_val or wa_loglike or cwa_loglike or jwa_loglike):
-        print("Please enter at least one thing that you want to plot.")
+    if not (plot_data or standard_val or cons_val or jeffreys_val 
+            or standard_like or cons_like or jeffreys_like):
+        exit("Please enter at least one thing that you want to plot.")
     else:
-        x_plot = np.linspace(min(np.array(data) - np.array(sigma)), max(np.array(data) + np.array(sigma)),100)
-        if cwa_val:
-            cwa_av, cwa_sig = cwa(data, sigma)
+        x_plot = np.linspace(min(np.array(data) - np.array(sigma)), max(np.array(data) + np.array(sigma)),400)
+        x_step = x_plot[1] - x_plot[0]
+        if jeffreys_val:
+            jeff_av, jeff_sig = average(data, sigma, mode = 'jeffreys')
+            print("Jeffreys weighted average:", jeff_av, "+-", jeff_sig)
+            axvspan(jeff_av - jeff_sig, jeff_av + jeff_sig, facecolor = "b", alpha=0.2)
+            axvline(jeff_av, c = "b", label = "Jeffreys average")
+            axvline(jeff_av - jeff_sig, c='b', ls = "--")
+            axvline(jeff_av + jeff_sig, c='b', ls = "--")
+        if cons_val:
+            cwa_av, cwa_sig = average(data, sigma, mode = 'cons')
             print("Conservative weighted average:", cwa_av, "+-", cwa_sig)
-            axvline(cwa_av, c = "b", label = "Conservative weighted average")
-            axvline(cwa_av - cwa_sig, c='b', ls = "--")
-            axvline(cwa_av + cwa_sig, c='b', ls = "--")
-        if cwa_loglike:
-            loglike = np.sum([log(sqrt(2 / pi) * s_temp * (1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)])
-            loglike_lam = lambdify(mu, loglike)
-            y_plot = loglike_lam(x_plot)
-            if normalize:
-                y_plot = (y_plot - min(y_plot))
-                y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'dodgerblue', label = "Conservative final likelihood")
-        if wa_val:
-            wa_av, wa_sig = wa(data, sigma)
+            axvspan(cwa_av - cwa_sig, cwa_av + cwa_sig, facecolor = "g", alpha=0.2)
+            axvline(cwa_av, c = "g", label = "Conservative average")
+            axvline(cwa_av - cwa_sig, c='g', ls = "--")
+            axvline(cwa_av + cwa_sig, c='g', ls = "--")
+        if standard_val:
+            wa_av, wa_sig = average(data, sigma, mode = 'standard')
             print("Standard weighted average:", wa_av, "+-", wa_sig)
-            axvline(wa_av, c = "r", label = "Standard weighted average")
+            axvspan(wa_av - wa_sig, wa_av + wa_sig, facecolor = "r", alpha=0.2)
+            axvline(wa_av, c = "r", label = "Standard average")
             axvline(wa_av - wa_sig, c='r', ls = "--")
             axvline(wa_av + wa_sig, c='r', ls = "--")
-        if wa_loglike:
-            loglike = np.sum([log(1/(s_temp * sqrt(2 * pi)) * exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) for x_temp, s_temp in zip(data, sigma)])
+        if jeffreys_like:
+            loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
             loglike_lam = lambdify(mu, loglike)
-            y_plot = loglike_lam(x_plot)
+            if linear:
+                y_plot = np.exp(loglike_lam(x_plot))
+            else:
+                y_plot = loglike_lam(x_plot)
             if normalize:
                 y_plot = (y_plot - min(y_plot))
-                y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'orange', label = "Standard likelihood")
-        if jwa_val:
-            jeff_av, jeff_sig = jwa(data, sigma)
-            print("Jeffreys weighted average:", jeff_av, "+-", jeff_sig)
-            axvline(jeff_av, c = "g", label = "Jeffreys final likelihood")
-            axvline(jeff_av - jeff_sig, c='g', ls = "--")
-            axvline(jeff_av + jeff_sig, c='g', ls = "--")
-        if jwa_loglike:
-            loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
+                y_plot = y_plot / np.sum(y_plot) / x_step
+            plot(x_plot, y_plot, c = 'dodgerblue', label = "Jeffreys likelihood")
+        if cons_like:
+            loglike = np.sum([log(sqrt(2 / pi) * s_temp * (1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)])
+            loglike_lam = lambdify(mu, loglike)
+            if linear:
+                y_plot = np.exp(loglike_lam(x_plot))
+            else:
+                y_plot = loglike_lam(x_plot)
+            if normalize:
+                y_plot = (y_plot - min(y_plot))
+                y_plot = y_plot / np.sum(y_plot) / x_step
+            plot(x_plot, y_plot, c = 'lime', label = "Conservative likelihood")
+        if standard_like:
+            loglike = np.sum([log(1/(s_temp * sqrt(2 * pi)) * exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) for x_temp, s_temp in zip(data, sigma)])
             loglike_lam = lambdify(mu, loglike)
-            y_plot = loglike_lam(x_plot)
+            if linear:
+                y_plot = np.exp(loglike_lam(x_plot))
+            else:
+                y_plot = loglike_lam(x_plot)
             if normalize:
                 y_plot = (y_plot - min(y_plot))
-                y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'lime', label = "Jeffreys weighted average")
+                y_plot = y_plot / np.sum(y_plot) / x_step
+            plot(x_plot, y_plot, c = 'brown', label = "Standard likelihood")
         if plot_data:
             y_min, y_max = gca().get_ylim()
             y_dist = y_max - y_min
             y_data = np.linspace(y_min + 0.2 * y_dist, y_min + 0.8 * y_dist, len(data))
-            errorbar(data, y_data, xerr = sigma, ls = "", capsize = 3, marker = ".", label = "data", c = "k")
-        if legendon: legend()
+            errorbar(data, y_data, xerr = sigma, label = "data", c = "k", fmt='.k',ecolor='k',mec='k',ls = "",**linestyle)
+        if legendon: legend(fontsize=10)
         if normalize:
-            ylabel("normalized log-likelihood")
+            if linear:
+                ylabel("Normalized likelihood")
+            else:
+                ylabel("Normalized log-likelihood")
         else:
-            ylabel("log-likelihood")
+            if linear:
+                ylabel("Likelihood")
+            else:
+                ylabel("Log-likelihood")
         if showon: show()
```

### Comparing `bayesian_average-0.1.7/bayesian_average.egg-info/PKG-INFO` & `bayesian_average-0.2.1/bayesian_average.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: bayesian_average
-Version: 0.1.7
+Version: 0.2.1
 Summary: __doc__
 Author: Marleen Maxton, Martino Trassinelli
 License: X11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Bayesian average
 
 ### Version:
-0.1.7
+0.2.0
 
 ### Authors
 Martino Trassinelli\
 CNRS, Institute of NanoSciences of Paris\
-email: trassinelli AT insp.jussieu.fr\
-email: m.trassinelli AT gmail.com
+emails: trassinelli AT cnrs.fr, m.trassinelli AT gmail.com
 
 Marleen Maxton\
 Max Planck Institute Heidelberg\
-email:
 
 ### Homepage
 https://github.com/martinit18/bayesian_average
 
 
 ### License
 Type: X11, see `LICENCE.txt`
@@ -41,47 +39,79 @@
 It is obtained by the marginalization on $\sigma'$, this result in a modified probability distribution for each $x_i$ that still depens on $\sigma_i$.
 Two different priors are proposed for $\sigma'$: the non-informative Jeffreys' prior $p(\sigma') \propto 1/ \sigma'$ (more precisely its limit, see Ref.[1]), and a modified version of it $p(\sigma') \propto 1/ (\sigma')^2$ proposed in Ref.[2].
 
 For both priors, the weighted average and its associated uncertainty are obtained numerically using `basinhopping` minimisation algorithm.
 
 In addition, the standard (inverse-variance) weighted average is also available for possible comparisons.
 
+## How to install it
+
+In your terminal, run
+```
+pip install bayesian_average
+```
+
 ## How to use it
-For the calculation of the Jeffreys' weighted average (see below for other averages)
+For the calculation of the weighted average just type in your python shell
 ```
 import bayesian_average as ba
-ba.jwa(data,sigma)
+ba.average(data,sigma)
 ```
 where `data` is a ntuple of data and `sigma` is the associated uncertainty of the same dimension.
+The default average mode is the one assuming a Jeffreys' prior `jeffreys`. 
+The other available are the `conservative`, `standard`, `birge`, which can be speficied by the keyword `mode`, like
+```
+ba.average(data,sigma, mode='conservative')
+```
+Details on the different method are presented below.
+
 The typical output is
 ```
 (6.6742395674538315, 9.74833292573106e-5)
 ```
-where the first number is the weighted average and the second one is the estimated final uncertainty 
+where the first number is the weighted average and the second one is the estimated final uncertainty.
+
+
+To plot the resulting probability distribution, the final weighted average and the input data:
+```
+ba.plot_average(data,sigma)
+```
+The default mode present the Jeffreys' vinal weighted average value and the associated distribution in log-scale. 
+To select other choices of weighted averages, take out the associated data point, normalise the associated distribution and/or plot them linerarly, additional options are available, like
 
-To plot the resulting probability distribution, the final weighted average and the input data (optionally)
 ```
-ba.plot_average(data,sigma,jwa_val=True,plot_data=True)
+ba.plot_average(data,sigma,jeffreys_val=True,jeffreys_like=True,plot_data=True,)
 ```
-The option `jwa_val=True` is on on as default. `plot_data=True` show the input data in addition.
+The option `xxx_val=True` display the value of the final weighted average of the `xxx` method. \
+`xxx_like=True` display the value of the final likelihood distribution (in log-scale by default). \
+`plot_data=True` show the input data in addition.
 
 ## Details of the vailable weighted averages
 
-- `jwa`: **Jeffreys weighted average** (main average, RECOMENDED, see Ref.[1]).\
+- `jeffreys`: **Jeffreys weighted average** (default average, RECOMENDED, see Ref.[1]).\
     The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to $1/\sigma'$.
     Because of the non-normalisability of the final probability distribution, this weighted average results 
     correspond to the  limit case with prior bounds $[\sigma, \sigma_\mathrm{max}]$ with $\sigma_\mathrm{max} \to \infty$ and where $\sigma$ is the value provided by the user.
     The final probability distribution is, however not a proper probability distribution.
-- `cwa`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
+- `cons`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
     The priors of the real uncertainty value are proportional to $\sigma/(\sigma')^2$, where $\sigma$ is the value provided by the user.
     The bounds of the prior are $[\sigma, \sigma_\mathrm{max}]$.
     This is a modified and normalisable version of the non-informative Jeffeys' prior.
-- `wa`: **Standard weighted average**\
+- `standard`: **Standard weighted average**\
     The standard inverse-variance weighted average useful for comparisons.
-
+- `birge`: **Standard weighted average corrected with the Birge ratio**\
+    The uncertainty of the final average is enanched by a factor proportional to the $\chi^2$ of the data and the weighted average if $\chi^2 > 1$, following Ref.[3].
 
 
 
 ## Refere articles:
 [1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* \
-[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
+[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press\
+[3]	R. T. Birge, *The Calculation of Errors by the Method of Least Squares*, Phys. Rev. **40**, 207 (1932)
+
+## Version history
+
+- 0.2: rearrangement of the average function(s),
+Birge ratio added
+- 0.1.5: First version aviable in github with documentation
+- 0.0.1: First version published in pypi with conservative, jeffreys' and standard weighted averages
```

### Comparing `bayesian_average-0.1.7/setup.py` & `bayesian_average-0.2.1/setup.py`

 * *Files identical despite different names*

