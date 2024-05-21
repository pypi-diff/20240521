# Comparing `tmp/qontrol-1.1.19.tar.gz` & `tmp/qontrol-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qontrol-1.1.19.tar", last modified: Tue May 21 08:33:46 2024, max compression
+gzip compressed data, was "qontrol-1.1.7.tar", last modified: Thu Aug 31 14:29:20 2023, max compression
```

## Comparing `qontrol-1.1.19.tar` & `qontrol-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:33:46.257866 qontrol-1.1.19/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-21 08:33:35.000000 qontrol-1.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 08:33:35.000000 qontrol-1.1.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-21 08:33:46.257866 qontrol-1.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-21 08:33:35.000000 qontrol-1.1.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:33:46.257866 qontrol-1.1.19/qontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-21 08:33:46.000000 qontrol-1.1.19/qontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-21 08:33:46.000000 qontrol-1.1.19/qontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:33:46.000000 qontrol-1.1.19/qontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 08:33:46.000000 qontrol-1.1.19/qontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 08:33:46.000000 qontrol-1.1.19/qontrol.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    57188 2024-05-21 08:33:35.000000 qontrol-1.1.19/qontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:33:46.257866 qontrol-1.1.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-21 08:33:35.000000 qontrol-1.1.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 14:29:20.836743 qontrol-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (999)     1059 2023-08-31 14:29:07.000000 qontrol-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)       33 2023-08-31 14:29:07.000000 qontrol-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     3588 2023-08-31 14:29:20.836743 qontrol-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     3284 2023-08-31 14:29:07.000000 qontrol-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)     2037 2023-08-31 14:29:07.000000 qontrol-1.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 14:29:20.836743 qontrol-1.1.7/qontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3588 2023-08-31 14:29:20.000000 qontrol-1.1.7/qontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      214 2023-08-31 14:29:20.000000 qontrol-1.1.7/qontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 14:29:20.000000 qontrol-1.1.7/qontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        9 2023-08-31 14:29:20.000000 qontrol-1.1.7/qontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-31 14:29:20.000000 qontrol-1.1.7/qontrol.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (999)    57003 2023-08-31 14:29:07.000000 qontrol-1.1.7/qontrol.py
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-31 14:29:20.836743 qontrol-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)      813 2023-08-31 14:29:07.000000 qontrol-1.1.7/setup.py
```

### Comparing `qontrol-1.1.19/LICENSE` & `qontrol-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qontrol-1.1.19/PKG-INFO` & `qontrol-1.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: qontrol
-Version: 1.1.19
+Version: 1.1.7
 Summary: Python Library for interfacing with Qontrol integrated optics control hardware.
 Home-page: https://github.com/takeqontrol/api
 Author: Qontrol
 Author-email: support@qontrol.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyserial
 
 # Qontrol API
 
 Integrated photonic devices need large-scale, precise electronic control. We can provide the precision and power you need, at a scale only limited by your ambition. Let’s take photonics into the future.
  See [our website](https://qontrol.co.uk/) for more details!
 
 Python Library for interfacing with **Qontrol** integrated optics control hardware. This module lets you control Qontrol hardware modules, natively in Python. It provides
```

### Comparing `qontrol-1.1.19/README.md` & `qontrol-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `qontrol-1.1.19/qontrol.egg-info/PKG-INFO` & `qontrol-1.1.7/qontrol.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: qontrol
-Version: 1.1.19
+Version: 1.1.7
 Summary: Python Library for interfacing with Qontrol integrated optics control hardware.
 Home-page: https://github.com/takeqontrol/api
 Author: Qontrol
 Author-email: support@qontrol.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyserial
 
 # Qontrol API
 
 Integrated photonic devices need large-scale, precise electronic control. We can provide the precision and power you need, at a scale only limited by your ambition. Let’s take photonics into the future.
  See [our website](https://qontrol.co.uk/) for more details!
 
 Python Library for interfacing with **Qontrol** integrated optics control hardware. This module lets you control Qontrol hardware modules, natively in Python. It provides
```

### Comparing `qontrol-1.1.19/qontrol.py` & `qontrol-1.1.7/qontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import serial, re, time
 from collections import deque as fifo
 from random import shuffle
 from serial.tools import list_ports
 import sys
 import os
 
-__version__ = "1.1.19"
+__version__ = "1.1.7"
 
 COMMON_ERRORS = {
 	0:'Unknown error.',
 	3:'Power error.',
 	4:'Calibration error.',
 	5:'Output error.',
 	10:'Unrecognised command.',
@@ -50,15 +50,14 @@
 	20:'Interlock triggered on channel {ch}.'}
 
 
 CMD_CODES = {'V':0x00, 'I':0x01, 'VMAX':0x02, 'IMAX':0x03, 'VCAL':0x04, 'ICAL':0x05, 'VERR':0x06, 'IERR':0x07, 'VIP':0x0A, 'SR':0x0B, 'PDI':0x0C, 'PDP':0x0D, 'PDR':0x0E, 'GAIN':0x0F, 'VFULL':0x20, 'IFULL':0x21, 'NCHAN':0x22, 'FIRMWARE':0x23, 'ID':0x24, 'LIFETIME':0x25, 'NVM':0x26, 'LOG':0x27, 'QUIET':0x28, 'LED':0x31, 'NUP':0x32, 'ADCT':0x33, 'ADCN':0x34, 'CCFN':0x35, 'INTEST':0x36, 'OK':0x37, 'DIGSUP':0x38, 'HELP':0x41, 'SAFE':0x42, 'ROCOM':0x43}
 
 DEVICE_PROPERTIES = {
 		'Q8iv':{'VFULL':12.0,'IFULL':24.0}, 
-		'Q8a':{'VFULL':12.0,'IFULL':100.0}, 
 		'Q8b':{'VFULL':12.0,'IFULL':83.333333}, 
 		'Q8bi':{'VFULL':12.0,'IFULL':100},
 		'M2':{'VFULL':8458.0,'IFULL':1375.0,'XFULL':8388352.0}}
 
 	
 RESPONSE_OK = 'OK\n'
 ERROR_FORMAT = '[A-Za-z]{1,3}(\d+):(\d+)'
@@ -733,15 +732,14 @@
 class _ChannelVector(object):
 	"""
 	List class with fixed length but mutable (typed) elements, with hooks.
 	"""
 	
 	def __init__(self, base_list, valid_types=(int,float), set_handle=None, get_handle=None):
 		self.list = base_list
-		self.n_ch = len(self.list)
 		self.valid_types = valid_types
 		try:
 			len(self.valid_types)
 		except:
 			raise AttributeError("valid_types must be iterable.")
 		self.set_handle = set_handle
 		self.get_handle = get_handle
@@ -775,21 +773,17 @@
 			if isinstance(value,list):
 				if len(ks) != len(value):
 					raise AttributeError('Attempt to set {0} channels of output to list of length {1}. Lengths must match.'.format(len(ks), len(values)))
 				vs = value
 			else:
 				vs = [value] * len(ks)
 			
-			for i,k in enumerate(ks):
-				self[k] = vs[i]
+			for k in ks:
+				self[k] = vs[k]
 		else:
-			# set_handle doesn't recognise -1 as the last element
-			# so we need to update the key
-			key = self.n_ch - 1 if key == -1 else key
-
 			# Handle normal key
 			if self.set_handle is not None:
 				self.set_handle (key, value)
 			self.list[key] = value
 		
 	
 	def __iter__(self):
@@ -804,22 +798,21 @@
 class QXOutput(Qontroller):
 	"""
 	Output module class. Provides channel vectors for voltage (v), current (i), 
 	maximum voltage (vmax), and maximum current (imax).
 	
 	Compatible modules:
 	- Q8iv
-	- Q8a
 	- Q8b
 	"""
 	
 	error_desc_dict = {**COMMON_ERRORS, **Qx_ERRORS}
 
 	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
+		super(type(self), self).__init__(*args, **kwargs)
 		
 		self.n_chs = 0
 		self.v_full = 0
 		self.i_full = 0
 		self.v = None				# Channel voltages (direct access)
 		self.i = None				# Channel currents (direct access)
 		self.vmax = None			# Channel voltages (direct access)
@@ -1010,15 +1003,15 @@
 	Compatible modules:
 	- M2
 	"""
 	
 	error_desc_dict = {**COMMON_ERRORS, **Mx_ERRORS}
 	
 	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
+		super(type(self), self).__init__(*args, **kwargs)
 
 		self.n_chs = 0
 		self.v_full = 0
 		self.i_full = 0
 		self.x_full = 0
 		self.v = None				# Channel voltages (direct access)
 		self.x = None				# Channel positions (direct access)
@@ -1313,15 +1306,15 @@
 	Compatible modules:
 	- S8i
 	"""
 	
 	error_desc_dict = {**COMMON_ERRORS, **Qx_ERRORS}
 
 	def __init__(self, *args, **kwargs):
-		super().__init__(*args, **kwargs)
+		super(type(self), self).__init__(*args, **kwargs)
 		
 		self.n_chs = 0
 		self.i_full = 0
 		self.i = None				# Channel currents (direct access)
 		self.gain = None			# Channel gain settings (direct access)
 		self.binary_mode = False	# Communicate in binary
```

