# Comparing `tmp/azizkitten-11.1.2.tar.gz` & `tmp/azizkitten-11.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azizkitten-11.1.2.tar", last modified: Mon May 20 17:14:28 2024, max compression
+gzip compressed data, was "azizkitten-11.1.3.tar", last modified: Tue May 21 18:28:59 2024, max compression
```

## Comparing `azizkitten-11.1.2.tar` & `azizkitten-11.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 17:14:28.139589 azizkitten-11.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-20 17:14:28.124585 azizkitten-11.1.2/AzizKitten/
--rw-rw-rw-   0        0        0      956 2024-05-16 18:30:48.000000 azizkitten-11.1.2/AzizKitten/__init__.py
--rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.2/AzizKitten/acos.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.2/AzizKitten/acot.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.2/AzizKitten/acsc.py
--rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/among_us.py
--rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.2/AzizKitten/asec.py
--rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.2/AzizKitten/asin.py
--rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.2/AzizKitten/atan.py
--rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/bin_rep.py
--rw-rw-rw-   0        0        0     2128 2024-05-16 17:14:20.000000 azizkitten-11.1.2/AzizKitten/cbrt.py
--rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.2/AzizKitten/constants.py
--rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.2/AzizKitten/cos.py
--rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.2/AzizKitten/cosh.py
--rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.2/AzizKitten/cot.py
--rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.2/AzizKitten/coth.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.2/AzizKitten/csc.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.2/AzizKitten/csch.py
--rw-rw-rw-   0        0        0     2312 2024-05-20 17:12:54.000000 azizkitten-11.1.2/AzizKitten/cubic.py
--rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.1.2/AzizKitten/degrees.py
--rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.2/AzizKitten/exp.py
--rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.2/AzizKitten/factorial.py
--rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.2/AzizKitten/floor.py
--rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.2/AzizKitten/gcd.py
--rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.2/AzizKitten/integrate.py
--rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.2/AzizKitten/lcm.py
--rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.2/AzizKitten/limit.py
--rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.2/AzizKitten/ln.py
--rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.2/AzizKitten/log.py
--rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/ment_calc.py
--rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.2/AzizKitten/mystery.py
--rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.2/AzizKitten/quad.py
--rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.1.2/AzizKitten/radians.py
--rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.2/AzizKitten/sec.py
--rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.2/AzizKitten/sech.py
--rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.2/AzizKitten/sin.py
--rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.2/AzizKitten/sinh.py
--rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.2/AzizKitten/sqrt.py
--rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.2/AzizKitten/tan.py
--rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.2/AzizKitten/tanh.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:14:28.136585 azizkitten-11.1.2/AzizKitten.egg-info/
--rw-rw-rw-   0        0        0      785 2024-05-20 17:14:27.000000 azizkitten-11.1.2/AzizKitten.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      961 2024-05-20 17:14:28.000000 azizkitten-11.1.2/AzizKitten.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 17:14:27.000000 azizkitten-11.1.2/AzizKitten.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 17:14:27.000000 azizkitten-11.1.2/AzizKitten.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.2/LICENSE
--rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      785 2024-05-20 17:14:28.138602 azizkitten-11.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.2/README.md
--rw-rw-rw-   0        0        0      673 2024-05-20 17:13:36.000000 azizkitten-11.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 17:14:28.140588 azizkitten-11.1.2/setup.cfg
--rw-rw-rw-   0        0        0      708 2024-05-20 17:13:44.000000 azizkitten-11.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:28:59.236242 azizkitten-11.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-21 18:28:59.224152 azizkitten-11.1.3/AzizKitten/
+-rw-rw-rw-   0        0        0      956 2024-05-16 18:30:48.000000 azizkitten-11.1.3/AzizKitten/__init__.py
+-rw-rw-rw-   0        0        0      199 2024-02-06 13:32:20.000000 azizkitten-11.1.3/AzizKitten/acos.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:34:15.000000 azizkitten-11.1.3/AzizKitten/acot.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:55.000000 azizkitten-11.1.3/AzizKitten/acsc.py
+-rw-rw-rw-   0        0        0    19953 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/among_us.py
+-rw-rw-rw-   0        0        0       64 2024-02-06 13:33:33.000000 azizkitten-11.1.3/AzizKitten/asec.py
+-rw-rw-rw-   0        0        0      406 2024-02-06 13:31:30.000000 azizkitten-11.1.3/AzizKitten/asin.py
+-rw-rw-rw-   0        0        0      141 2024-05-16 17:14:01.000000 azizkitten-11.1.3/AzizKitten/atan.py
+-rw-rw-rw-   0        0        0      409 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/bin_rep.py
+-rw-rw-rw-   0        0        0     2226 2024-05-20 18:59:59.000000 azizkitten-11.1.3/AzizKitten/cbrt.py
+-rw-rw-rw-   0        0        0      199 2024-05-16 17:28:31.000000 azizkitten-11.1.3/AzizKitten/constants.py
+-rw-rw-rw-   0        0        0      306 2024-05-16 17:14:09.000000 azizkitten-11.1.3/AzizKitten/cos.py
+-rw-rw-rw-   0        0        0       71 2024-02-09 14:35:45.000000 azizkitten-11.1.3/AzizKitten/cosh.py
+-rw-rw-rw-   0        0        0      168 2024-02-24 15:38:52.000000 azizkitten-11.1.3/AzizKitten/cot.py
+-rw-rw-rw-   0        0        0       96 2024-02-24 15:39:19.000000 azizkitten-11.1.3/AzizKitten/coth.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:26:25.000000 azizkitten-11.1.3/AzizKitten/csc.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:42:18.000000 azizkitten-11.1.3/AzizKitten/csch.py
+-rw-rw-rw-   0        0        0     2799 2024-05-21 18:27:50.000000 azizkitten-11.1.3/AzizKitten/cubic.py
+-rw-rw-rw-   0        0        0       67 2024-05-16 18:30:33.000000 azizkitten-11.1.3/AzizKitten/degrees.py
+-rw-rw-rw-   0        0        0       60 2024-02-06 13:34:42.000000 azizkitten-11.1.3/AzizKitten/exp.py
+-rw-rw-rw-   0        0        0      506 2024-05-14 18:00:41.000000 azizkitten-11.1.3/AzizKitten/factorial.py
+-rw-rw-rw-   0        0        0      135 2024-02-10 09:32:39.000000 azizkitten-11.1.3/AzizKitten/floor.py
+-rw-rw-rw-   0        0        0       81 2024-02-07 12:42:22.000000 azizkitten-11.1.3/AzizKitten/gcd.py
+-rw-rw-rw-   0        0        0      605 2024-05-14 17:51:40.000000 azizkitten-11.1.3/AzizKitten/integrate.py
+-rw-rw-rw-   0        0        0       82 2024-02-07 12:42:13.000000 azizkitten-11.1.3/AzizKitten/lcm.py
+-rw-rw-rw-   0        0        0     1485 2024-02-10 11:22:50.000000 azizkitten-11.1.3/AzizKitten/limit.py
+-rw-rw-rw-   0        0        0      516 2024-05-14 17:38:20.000000 azizkitten-11.1.3/AzizKitten/ln.py
+-rw-rw-rw-   0        0        0       74 2024-02-06 13:22:15.000000 azizkitten-11.1.3/AzizKitten/log.py
+-rw-rw-rw-   0        0        0     2249 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/ment_calc.py
+-rw-rw-rw-   0        0        0     6268 2024-02-06 12:37:23.000000 azizkitten-11.1.3/AzizKitten/mystery.py
+-rw-rw-rw-   0        0        0      560 2024-05-16 17:14:04.000000 azizkitten-11.1.3/AzizKitten/quad.py
+-rw-rw-rw-   0        0        0       69 2024-05-16 18:30:59.000000 azizkitten-11.1.3/AzizKitten/radians.py
+-rw-rw-rw-   0        0        0      139 2024-02-06 13:30:00.000000 azizkitten-11.1.3/AzizKitten/sec.py
+-rw-rw-rw-   0        0        0       62 2024-02-09 14:41:44.000000 azizkitten-11.1.3/AzizKitten/sech.py
+-rw-rw-rw-   0        0        0      310 2024-05-16 17:14:11.000000 azizkitten-11.1.3/AzizKitten/sin.py
+-rw-rw-rw-   0        0        0       71 2024-02-10 11:23:11.000000 azizkitten-11.1.3/AzizKitten/sinh.py
+-rw-rw-rw-   0        0        0      114 2024-05-14 17:41:04.000000 azizkitten-11.1.3/AzizKitten/sqrt.py
+-rw-rw-rw-   0        0        0      169 2024-02-06 13:30:05.000000 azizkitten-11.1.3/AzizKitten/tan.py
+-rw-rw-rw-   0        0        0       96 2024-02-09 14:36:37.000000 azizkitten-11.1.3/AzizKitten/tanh.py
+drwxrwxrwx   0        0        0        0 2024-05-21 18:28:59.234243 azizkitten-11.1.3/AzizKitten.egg-info/
+-rw-rw-rw-   0        0        0      785 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 18:28:59.000000 azizkitten-11.1.3/AzizKitten.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1055 2024-02-06 12:37:22.000000 azizkitten-11.1.3/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-02-06 12:37:22.000000 azizkitten-11.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      785 2024-05-21 18:28:59.235255 azizkitten-11.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2024-02-06 12:37:22.000000 azizkitten-11.1.3/README.md
+-rw-rw-rw-   0        0        0      673 2024-05-21 18:28:20.000000 azizkitten-11.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 18:28:59.236242 azizkitten-11.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      708 2024-05-21 18:28:23.000000 azizkitten-11.1.3/setup.py
```

### Comparing `azizkitten-11.1.2/AzizKitten/__init__.py` & `azizkitten-11.1.3/AzizKitten/__init__.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/among_us.py` & `azizkitten-11.1.3/AzizKitten/among_us.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/cbrt.py` & `azizkitten-11.1.3/AzizKitten/cbrt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 def cbrt(x):
-    from .cos import cos
-    from .sin import sin
     from .constants import pi
     from .sqrt import sqrt
     from .atan import atan
+    from .exp import exp
     if type(x) is complex:
         a = x.real
         b = x.imag
         if a != 0:
             r = sqrt(a**2+b**2)
-            theta = atan(b/a)
+            if a > 0 and b > 0:
+                theta = atan(b/a)
+            elif a > 0 and b < 0:
+                theta = 2*pi-atan(-b/a)
+            elif a < 0 and b > 0:
+                theta = pi - atan(b/-a)
+            elif a < 0 and b < 0:
+                theta = pi + atan(-b/-a)
+            elif a > 0 and b == 0:
+                theta = 0
+            else:
+                theta = 3*pi
             low = 0.0
             high = max(1.0, r)
             epsilon = 0.00000000000001
             while True:
                 mid = (low + high)/2
                 mid_cubed = mid * mid * mid
 
                 if abs(mid_cubed-r) < epsilon:
                     cubed_r = mid
                     break
                 elif mid_cubed < r:
                     low = mid
                 else:
                     high = mid
-            sqrt1 = cubed_r * (cos((-pi-theta)/3)-sin((-pi-theta)/3)*1j)
-            sqrt2 = cubed_r * (cos((pi-theta)/3)-sin((pi-theta)/3)*1j)
-            sqrt3 = -cubed_r * (cos((theta)/3)+sin((theta)/3)*1j)
-            if sqrt1.real > sqrt2.real and sqrt1.real > sqrt3.real:
-                return sqrt1
-            elif sqrt2.real > sqrt1.real and sqrt2.real > sqrt3.real:
-                return sqrt2
-            return sqrt3 
+            principal_root = cubed_r * exp(theta*1j/3)
+            if abs(principal_root.imag) < 1e-8:
+                return principal_root.real
+            return principal_root
             
         if b >= 0:
             low = 0.0
             high = max(1.0, b)
         else:
             low = min(-1.0, b)
             high = 0.0
@@ -68,8 +74,8 @@
         mid_cubed = mid * mid * mid
 
         if abs(mid_cubed - x) < epsilon:
             return mid
         elif mid_cubed < x:
             low = mid
         else:
-            high = mid
+            high = mid
```

### Comparing `azizkitten-11.1.2/AzizKitten/cubic.py` & `azizkitten-11.1.3/AzizKitten/cubic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 def cubic(a,b,c,d):
     from .cbrt import cbrt
     from .sqrt import sqrt
     from .quad import quad
     if a == 0:
         raise ValueError("value of 'a' must be different to 0.")
-    if d == 0:
-        quad(a,b,c)
-        cubic.x1, cubic.x2, cubic.x3 = 0, quad.x1, quad.x2
-    elif a+b+c+d == 0:
+    if a+b+c+d == 0:
         A = a
         B = b+a
         C = -d
         quad(A,B,C)
         cubic.x1, cubic.x2, cubic.x3 = 1, quad.x1, quad.x2
     elif -a+b-c+d == 0:
         A = a
         B = b-a
         C = d
         quad(A,B,C)
         cubic.x1, cubic.x2, cubic.x3 = -1, quad.x1, quad.x2
     else:
         p = (3*a*c-b**2)/(3*a**2)
         q = (2*b**3-9*a*b*c+27*a**2*d)/(27*a**3)
-        cubic.x1 = cbrt(-q/2+sqrt(q**2/4+p**3/27))+cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
-        cubic.x2 = (-1+sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1-sqrt(-3))/2*cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
-        cubic.x3 = (-1-sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1+sqrt(-3))/2*cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
+        if type(-q/2+sqrt(q**2/4+p**3/27)) is complex:
+            cubic.x1 = cbrt(-q/2+sqrt(q**2/4+p**3/27))+(cbrt(-q/2+sqrt(q**2/4+p**3/27))).real-1j*(cbrt(-q/2+sqrt(q**2/4+p**3/27))).imag-b/(3*a)
+            cubic.x2 = (-1+sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1-sqrt(-3))/2*((cbrt(-q/2+sqrt(q**2/4+p**3/27))).real-1j*(cbrt(-q/2+sqrt(q**2/4+p**3/27))).imag)-b/(3*a)
+            cubic.x3 = (-1-sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1+sqrt(-3))/2*((cbrt(-q/2+sqrt(q**2/4+p**3/27))).real-1j*(cbrt(-q/2+sqrt(q**2/4+p**3/27))).imag)-b/(3*a)
+        else:
+            cubic.x1 = cbrt(-q/2+sqrt(q**2/4+p**3/27))+cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
+            cubic.x2 = (-1+sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1-sqrt(-3))/2*cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
+            cubic.x3 = (-1-sqrt(-3))/2*cbrt(-q/2+sqrt(q**2/4+p**3/27))+(-1+sqrt(-3))/2*cbrt(-q/2-sqrt(q**2/4+p**3/27))-b/(3*a)
     if type(cubic.x1) is complex:
         if abs(cubic.x1.imag) < 1e-6:
             cubic.x1 = cubic.x1.real+0j
         if abs(cubic.x1.real) < 1e-6:
             cubic.x1 = 0+cubic.x1.imag*1j
         if cubic.x1.imag == 0:
             cubic.x1 = cubic.x1.real
```

### Comparing `azizkitten-11.1.2/AzizKitten/integrate.py` & `azizkitten-11.1.3/AzizKitten/integrate.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/limit.py` & `azizkitten-11.1.3/AzizKitten/limit.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/ln.py` & `azizkitten-11.1.3/AzizKitten/ln.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/ment_calc.py` & `azizkitten-11.1.3/AzizKitten/ment_calc.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/mystery.py` & `azizkitten-11.1.3/AzizKitten/mystery.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten/quad.py` & `azizkitten-11.1.3/AzizKitten/quad.py`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/AzizKitten.egg-info/PKG-INFO` & `azizkitten-11.1.3/AzizKitten.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.1.2
+Version: 11.1.3
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azizkitten-11.1.2/AzizKitten.egg-info/SOURCES.txt` & `azizkitten-11.1.3/AzizKitten.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/LICENSE` & `azizkitten-11.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azizkitten-11.1.2/PKG-INFO` & `azizkitten-11.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AzizKitten
-Version: 11.1.2
+Version: 11.1.3
 Summary: AzizOmrane's own Python package
 Author: AzizKitten
 Author-email: AzizKitten <azizprv43@gmail.com>
 Project-URL: AboutMe, https://azizkitten.github.io
 Project-URL: Documentation, https://azizkitten.github.io/python
 Project-URL: Bug Tracker, https://github.com/AzizKitten/azizkitten.github.io/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `azizkitten-11.1.2/pyproject.toml` & `azizkitten-11.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AzizKitten"
-version = "11.1.2"
+version = "11.1.3"
 authors = [
   { name="AzizKitten", email="azizprv43@gmail.com" },
 ]
 description = "AzizOmrane's own Python package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `azizkitten-11.1.2/setup.py` & `azizkitten-11.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AzizKitten",
-    version="11.1.2",
+    version="11.1.3",
     packages=find_packages(),
     include_package_data=True,
     author="AzizKitten",
     author_email="azizprv43@gmail.com",
     description="AzizOmrane's own python library",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

