# Comparing `tmp/pypowerwall-0.8.5-py2.py3-none-any.whl.zip` & `tmp/pypowerwall-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,31 @@
-Zip file size: 62071 bytes, number of entries: 21
--rw-r--r--  2.0 unx    32843 b- defN 24-May-15 14:44 pypowerwall/__init__.py
--rw-r--r--  2.0 unx     5835 b- defN 24-May-15 14:43 pypowerwall/__main__.py
--rw-r--r--  2.0 unx     1889 b- defN 24-May-15 14:43 pypowerwall/aux.py
+Zip file size: 87264 bytes, number of entries: 29
+-rw-r--r--  2.0 unx    37170 b- defN 24-May-21 00:00 pypowerwall/__init__.py
+-rw-r--r--  2.0 unx     6434 b- defN 24-May-20 22:45 pypowerwall/__main__.py
 -rw-r--r--  2.0 unx      133 b- defN 24-Mar-30 06:29 pypowerwall/exceptions.py
 -rw-r--r--  2.0 unx     2897 b- defN 24-Apr-04 04:31 pypowerwall/pypowerwall_base.py
+-rw-r--r--  2.0 unx     1889 b- defN 24-May-20 22:45 pypowerwall/regex.py
 -rw-r--r--  2.0 unx     6718 b- defN 24-Mar-26 02:39 pypowerwall/scan.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:39 pypowerwall/cloud/__init__.py
 -rw-r--r--  2.0 unx      638 b- defN 24-Mar-26 02:39 pypowerwall/cloud/decorators.py
 -rw-r--r--  2.0 unx      242 b- defN 24-Mar-30 06:29 pypowerwall/cloud/exceptions.py
 -rw-r--r--  2.0 unx    18733 b- defN 24-Mar-26 02:39 pypowerwall/cloud/mock_data.py
 -rw-r--r--  2.0 unx    46441 b- defN 24-May-15 14:44 pypowerwall/cloud/pypowerwall_cloud.py
 -rw-r--r--  2.0 unx     4355 b- defN 24-Mar-26 02:39 pypowerwall/cloud/stubs.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 22:45 pypowerwall/fleetapi/__init__.py
+-rw-r--r--  2.0 unx     5747 b- defN 24-May-20 22:45 pypowerwall/fleetapi/__main__.py
+-rw-r--r--  2.0 unx      650 b- defN 24-May-20 22:45 pypowerwall/fleetapi/decorators.py
+-rw-r--r--  2.0 unx      254 b- defN 24-May-20 22:45 pypowerwall/fleetapi/exceptions.py
+-rw-r--r--  2.0 unx    31740 b- defN 24-May-20 23:50 pypowerwall/fleetapi/fleetapi.py
+-rw-r--r--  2.0 unx    18733 b- defN 24-May-20 22:45 pypowerwall/fleetapi/mock_data.py
+-rw-r--r--  2.0 unx    33528 b- defN 24-May-20 22:45 pypowerwall/fleetapi/pypowerwall_fleetapi.py
+-rw-r--r--  2.0 unx     4355 b- defN 24-May-20 22:45 pypowerwall/fleetapi/stubs.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-26 02:39 pypowerwall/local/__init__.py
 -rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 02:39 pypowerwall/local/exceptions.py
--rw-r--r--  2.0 unx    20404 b- defN 24-May-15 14:43 pypowerwall/local/pypowerwall_local.py
+-rw-r--r--  2.0 unx    20463 b- defN 24-May-20 22:45 pypowerwall/local/pypowerwall_local.py
 -rw-r--r--  2.0 unx    71273 b- defN 24-Mar-26 02:39 pypowerwall/local/tesla_pb2.py
--rw-r--r--  2.0 unx     1066 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    41728 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1766 b- defN 24-May-15 14:46 pypowerwall-0.8.5.dist-info/RECORD
-21 files, 257175 bytes uncompressed, 59191 bytes compressed:  77.0%
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-21 00:13 pypowerwall-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    44205 b- defN 24-May-21 00:13 pypowerwall-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-21 00:13 pypowerwall-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-21 00:13 pypowerwall-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2492 b- defN 24-May-21 00:13 pypowerwall-0.9.0.dist-info/RECORD
+29 files, 360370 bytes uncompressed, 83232 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pypowerwall/__init__.py
 Comment: 
 
 Filename: pypowerwall/__main__.py
 Comment: 
 
-Filename: pypowerwall/aux.py
-Comment: 
-
 Filename: pypowerwall/exceptions.py
 Comment: 
 
 Filename: pypowerwall/pypowerwall_base.py
 Comment: 
 
+Filename: pypowerwall/regex.py
+Comment: 
+
 Filename: pypowerwall/scan.py
 Comment: 
 
 Filename: pypowerwall/cloud/__init__.py
 Comment: 
 
 Filename: pypowerwall/cloud/decorators.py
@@ -30,35 +30,59 @@
 
 Filename: pypowerwall/cloud/pypowerwall_cloud.py
 Comment: 
 
 Filename: pypowerwall/cloud/stubs.py
 Comment: 
 
+Filename: pypowerwall/fleetapi/__init__.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/__main__.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/decorators.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/exceptions.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/fleetapi.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/mock_data.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/pypowerwall_fleetapi.py
+Comment: 
+
+Filename: pypowerwall/fleetapi/stubs.py
+Comment: 
+
 Filename: pypowerwall/local/__init__.py
 Comment: 
 
 Filename: pypowerwall/local/exceptions.py
 Comment: 
 
 Filename: pypowerwall/local/pypowerwall_local.py
 Comment: 
 
 Filename: pypowerwall/local/tesla_pb2.py
 Comment: 
 
-Filename: pypowerwall-0.8.5.dist-info/LICENSE
+Filename: pypowerwall-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pypowerwall-0.8.5.dist-info/METADATA
+Filename: pypowerwall-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pypowerwall-0.8.5.dist-info/WHEEL
+Filename: pypowerwall-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pypowerwall-0.8.5.dist-info/top_level.txt
+Filename: pypowerwall-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pypowerwall-0.8.5.dist-info/RECORD
+Filename: pypowerwall-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pypowerwall/__init__.py

```diff
@@ -29,14 +29,17 @@
     poolmaxsize = 10          # Pool max size for http connection re-use (persistent
                                 connections disabled if zero)
     cloudmode = False         # If True, use Tesla cloud for data (default is False)
     siteid = None             # If cloudmode is True, use this siteid (default is None)
     authpath = ""             # Path to cloud auth and site files (default current directory)
     authmode = "cookie"       # "cookie" (default) or "token" - use cookie or bearer token for auth
     cachefile = ".powerwall"  # Path to cache file (default current directory)
+    fleetapi = False          # If True, use Tesla FleetAPI for data (default is False)
+    auth_path = ""            # Path to configfile (default current directory)
+    auto_select = False       # If True, select the best available mode to connect (default is False)
     
  Functions 
     poll(api, json, force)    # Return data from Powerwall api (dict if json=True, bypass cache force=True)
     post(api, payload, json)  # Send payload to Powerwall api (dict if json=True)
     level()                   # Return battery power level percentage
     power()                   # Return power data returned as dictionary
     site(verbose)             # Return site sensor data (W or raw JSON if verbose=True)
@@ -61,48 +64,50 @@
                               #     - "numeric": -1 (Syncing), 0 (DOWN), 1 (UP)
     is_connected()            # Returns True if able to connect and login to Powerwall
     get_reserve(scale)        # Get Battery Reserve Percentage
     get_mode()                # Get Current Battery Operation Mode
     set_reserve(level)        # Set Battery Reserve Percentage
     set_mode(mode)            # Set Current Battery Operation Mode
     get_time_remaining()      # Get the backup time remaining on the battery
-
     set_operation(level, mode, json)        # Set Battery Reserve Percentage and/or Operation Mode
 
  Requirements
     This module requires the following modules: requests, protobuf, teslapy
     pip install requests protobuf teslapy
 """
 import json
 import logging
 import os.path
 import sys
 from json import JSONDecodeError
 from typing import Union, Optional
+import time
 
 # noinspection PyPackageRequirements
 import urllib3
 
-from pypowerwall.aux import HOST_REGEX, IPV4_6_REGEX, EMAIL_REGEX
+from pypowerwall.regex import HOST_REGEX, IPV4_6_REGEX, EMAIL_REGEX
 from pypowerwall.exceptions import PyPowerwallInvalidConfigurationParameter, InvalidBatteryReserveLevelException
 from pypowerwall.cloud.pypowerwall_cloud import PyPowerwallCloud
 from pypowerwall.local.pypowerwall_local import PyPowerwallLocal
+from pypowerwall.fleetapi.pypowerwall_fleetapi import PyPowerwallFleetAPI
 from pypowerwall.pypowerwall_base import parse_version, PyPowerwallBase
+from pypowerwall.fleetapi.fleetapi import CONFIGFILE
+from pypowerwall.cloud.pypowerwall_cloud import AUTHFILE
 
 urllib3.disable_warnings()  # Disable SSL warnings
 
-version_tuple = (0, 8, 5)
+version_tuple = (0, 9, 0)
 version = __version__ = '%d.%d.%d' % version_tuple
 __author__ = 'jasonacox'
 
 log = logging.getLogger(__name__)
 log.debug('%s version %s', __name__, __version__)
 log.debug('Python %s on %s', sys.version, sys.platform)
 
-
 def set_debug(toggle=True, color=True):
     """Enable verbose logging"""
     if toggle:
         if color:
             logging.basicConfig(format='\x1b[31;1m%(levelname)s:%(message)s\x1b[0m', level=logging.DEBUG)
         else:
             logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
@@ -111,15 +116,16 @@
     else:
         log.setLevel(logging.NOTSET)
 
 
 class Powerwall(object):
     def __init__(self, host="", password="", email="nobody@nowhere.com",
                  timezone="America/Los_Angeles", pwcacheexpire=5, timeout=5, poolmaxsize=10,
-                 cloudmode=False, siteid=None, authpath="", authmode="cookie", cachefile=".powerwall"):
+                 cloudmode=False, siteid=None, authpath="", authmode="cookie", cachefile=".powerwall",
+                 fleetapi=False, auto_select=False, retry_modes=False):
         """
         Represents a Tesla Energy Gateway Powerwall device.
 
         Args:
             host        = Hostname or IP address of Powerwall (e.g. 10.0.1.99)
             password    = Customer password set up on Powerwall gateway
             email       = Customer email 
@@ -129,53 +135,126 @@
             timeout      = Seconds for the timeout on http requests
             poolmaxsize  = Pool max size for http connection re-use (persistent connections disabled if zero)
             cloudmode    = If True, use Tesla cloud for data (default is False)
             siteid       = If cloudmode is True, use this siteid (default is None)  
             authpath     = Path to cloud auth and site cache files (default current directory)
             authmode     = "cookie" (default) or "token" - use cookie or bearer token for authorization
             cachefile    = Path to cache file (default current directory)
+            fleetapi     = If True, use Tesla FleetAPI for data (default is False)
+            auto_select  = If True, select the best available mode to connect (default is False)
+            retry_modes  = If True, retry connection to Powerwall
         """
 
         # Attributes
         self.cachefile = cachefile  # Stores auth session information
         self.host = host
         self.password = password
         self.email = email
         self.timezone = timezone
         self.timeout = timeout  # 5s timeout for http calls
         self.poolmaxsize = poolmaxsize  # pool max size for http connection re-use
         self.auth = {}  # caches auth cookies
         self.token = None  # caches bearer token
-        self.pwcachetime = {}  # holds the cached data timestamps for api
-        self.pwcache = {}  # holds the cached data for api
         self.pwcacheexpire = pwcacheexpire  # seconds to expire cache
         self.cloudmode = cloudmode  # cloud mode or local mode (default)
         self.siteid = siteid  # siteid for cloud mode
         self.authpath = os.path.expanduser(authpath)  # path to auth and site cache files
         self.authmode = authmode  # cookie or token
         self.pwcooldown = 0  # rate limit cooldown time - pause api calls
         self.vitals_api = True  # vitals api is available for local mode
         self.client: PyPowerwallBase
+        self.fleetapi = fleetapi
+        self.retry_modes = retry_modes
 
         # Make certain assumptions here
         if not self.host:
             self.cloudmode = True
+        elif not self.cloudmode and not self.fleetapi:
+            self.mode = "local"
+        else:
+            self.mode = "unknown"
+
+        # Auto select mode if requested
+        if auto_select:
+            if self.host and not self.cloudmode and not self.fleetapi:
+                log.debug("Auto selecting local mode")
+                self.cloudmode = self.fleetapi = False
+                self.mode = "local"
+            elif os.path.exists(os.path.join(self.authpath, CONFIGFILE)):
+                log.debug("Auto selecting FleetAPI Mode")
+                self.cloudmode = self.fleetapi = True
+                self.mode = "fleetapi"
+            elif os.path.exists(os.path.join(self.authpath, AUTHFILE)):
+                if not self.email or self.email == "nobody@nowhere.com":
+                    with open(authpath + AUTHFILE, 'r') as file:
+                        auth = json.load(file)
+                    self.email = list(auth.keys())[0]
+                self.cloudmode = True
+                self.fleetapi = False     
+                self.mode = "cloud"       
+                log.debug("Auto selecting Cloud Mode (email: %s)" % self.email)    
+            else:
+                log.error("Auto Select Failed: Unable to use local, cloud or fleetapi mode.")
 
         # Validate provided parameters
         self._validate_init_configuration()
 
-        # Check for cloud mode
-        if self.cloudmode:
-            self.client = PyPowerwallCloud(self.email, self.pwcacheexpire, self.timeout, self.siteid, self.authpath)
-            # Check to see if we can connect to the cloud
-        else:
-            self.client = PyPowerwallLocal(self.host, self.password, self.email, self.timezone, self.timeout,
-                                           self.pwcacheexpire, self.poolmaxsize, self.authmode, self.cachefile)
+        # Connect to Powerwall
+        self.connect(self.retry_modes)
+    
+    def connect(self, retry=False):
+        """
+        Connect to Tesla Energy Gateway Powerwall
 
-        self.client.authenticate()
+        Args:
+            retry = If True, retry connection to Powerwall
+        """
+        if self.mode == "unknown":
+            log.error("Unable to determine mode to connect.")
+            return
+        count = 0
+        while count < 3:
+            count += 1
+            if retry and count == 3:
+                log.error("Failed to connect to Powerwall with all modes. Waiting 30s to retry.")
+                time.sleep(30)
+                count = 0
+            if self.mode == "local":
+                try:
+                    self.client = PyPowerwallLocal(self.host, self.password, self.email, self.timezone, self.timeout,
+                                               self.pwcacheexpire, self.poolmaxsize, self.authmode, self.cachefile)
+                    self.client.authenticate()
+                    self.cloudmode = self.fleetapi = False
+                    break
+                except Exception as exc:
+                    log.error(f"Failed to connect using Local mode: {exc} - trying fleetapi mode.")
+                    self.mode = "fleetapi"
+                    continue
+            if self.mode == "fleetapi":
+                try:
+                    self.client = PyPowerwallFleetAPI(self.email, self.pwcacheexpire, self.timeout, self.siteid,
+                                                    self.authpath)
+                    self.client.authenticate()
+                    self.cloudmode = self.fleetapi = True
+                    break
+                except Exception as exc:
+                    log.error(f"Failed to connect using FleetAPI mode: {exc} - trying cloud mode.")
+                    self.mode = "cloud"
+                    continue
+            if self.mode == "cloud":
+                try:
+                    self.client = PyPowerwallCloud(self.email, self.pwcacheexpire, self.timeout, self.siteid, self.authpath)
+                    self.client.authenticate()
+                    self.cloudmode = True
+                    self.fleetapi = False
+                    break
+                except Exception as exc:
+                    log.error(f"Failed to connect using Cloud mode: {exc} - trying fleetapi mode.")
+                    self.mode = "local"
+                    continue
 
     def is_connected(self):
         """
         Attempt connection with Tesla Energy Gateway
         
         Return True if able to successfully connect and login to Powerwall
         """
@@ -736,29 +815,35 @@
                 not isinstance(self.host, str) or
                 (not IPV4_6_REGEX.match(self.host) and not HOST_REGEX.match(self.host))
         )):
             raise PyPowerwallInvalidConfigurationParameter(f"Invalid powerwall host: '{self.host}'. Must be in the "
                                                            f"form of IP address or a valid form of a hostname or FQDN.")
 
         # If cloud mode requested, check appropriate parameters
-        if self.cloudmode:
+        if self.cloudmode and not self.fleetapi:
             # Ensure email is set and syntactically correct
             if not self.email or not isinstance(self.email, str) or not EMAIL_REGEX.match(self.email):
                 raise PyPowerwallInvalidConfigurationParameter(f"A valid email address is required to run in "
                                                                f"cloud mode: '{self.email}' did not pass validation.")
 
             # Ensure we can write to the provided authpath
             dirname = self.authpath
             if not dirname:
                 log.debug("No authpath provided, using current directory.")
                 dirname = '.'
             self._check_if_dir_is_writable(dirname, "authpath")
-        # If local mode, check appropriate parameters, too
+        elif self.fleetapi:
+            # Ensure we can write to the configfile
+            self.configfile = os.path.join(self.authpath, CONFIGFILE)
+            if os.access(self.configfile, os.W_OK):
+                log.debug(f"Config file '{self.configfile}' is writable.")
+            else:
+                raise PyPowerwallInvalidConfigurationParameter(f"Config file '{self.configfile}' is not writable.")
         else:
-            # Ensure we can create a cachefile
+            # If local mode, check appropriate parameters, and ensure we can write to the provided cachefile
             dirname = os.path.dirname(self.cachefile)
             if not dirname:
                 log.debug("No cachefile provided, using current directory.")
                 dirname = '.'
             self._check_if_dir_is_writable(dirname, "cachefile")
 
     @staticmethod
```

## pypowerwall/__main__.py

```diff
@@ -13,18 +13,19 @@
 
 import argparse
 import os
 import sys
 import json
 
 # Modules
-from pypowerwall import version
+from pypowerwall import version, set_debug
+from pypowerwall.cloud.pypowerwall_cloud import AUTHFILE
+from pypowerwall.fleetapi.fleetapi import CONFIGFILE
 
 # Global Variables
-AUTHFILE = ".pypowerwall.auth"
 authpath = os.getenv("PW_AUTH_PATH", "")
 
 timeout = 1.0
 hosts = 30
 state = 0
 color = True
 ip = None
@@ -34,14 +35,16 @@
 p = argparse.ArgumentParser(prog="PyPowerwall", description=f"PyPowerwall Module v{version}")
 subparsers = p.add_subparsers(dest="command", title='commands (run <command> -h to see usage information)',
                               required=True)
 
 setup_args = subparsers.add_parser("setup", help='Setup Tesla Login for Cloud Mode access')
 setup_args.add_argument("-email", type=str, default=email, help="Email address for Tesla Login.")
 
+setup_args = subparsers.add_parser("fleetapi", help='Setup Tesla FleetAPI for Cloud Mode access')
+
 scan_args = subparsers.add_parser("scan", help='Scan local network for Powerwall gateway')
 scan_args.add_argument("-timeout", type=float, default=timeout,
                        help=f"Seconds to wait per host [Default={timeout:.1f}]")
 scan_args.add_argument("-nocolor", action="store_true", default=not color,
                        help="Disable color text output.")
 scan_args.add_argument("-ip", type=str, default=ip, help="IP address within network to scan.")
 scan_args.add_argument("-hosts", type=int, default=hosts,
@@ -57,58 +60,77 @@
 
 get_mode_args = subparsers.add_parser("get", help='Get Powerwall Settings and Power Levels')
 get_mode_args.add_argument("-format", type=str, default="text",
                             help="Output format: text, json, csv")
 
 version_args = subparsers.add_parser("version", help='Print version information')
 
+# Add a global debug flag
+p.add_argument("-debug", action="store_true", default=False, help="Enable debug output")
+
 if len(sys.argv) == 1:
     p.print_help(sys.stderr)
     sys.exit(1)
 
 # parse args
 args = p.parse_args()
 command = args.command
 
+# Set Debug Mode
+if args.debug:
+    set_debug(True)
+
 # Cloud Mode Setup
 if command == 'setup':
     from pypowerwall import PyPowerwallCloud
 
     email = args.email
     print("pyPowerwall [%s] - Cloud Mode Setup\n" % version)
     # Run Setup
     c = PyPowerwallCloud(None, authpath=authpath)
     if c.setup(email):
-        print("Setup Complete. Auth file %s ready to use." % AUTHFILE)
+        print(f"Setup Complete. Auth file {c.authfile} ready to use.")
     else:
         print("ERROR: Failed to setup Tesla Cloud Mode")
         exit(1)
+# FleetAPI Mode Setup
+elif command == 'fleetapi':
+    from pypowerwall import PyPowerwallFleetAPI
+
+    print("pyPowerwall [%s] - FleetAPI Mode Setup\n" % version)
+    # Run Setup
+    c = PyPowerwallFleetAPI(None, authpath=authpath)
+    if c.setup():
+        print(f"Setup Complete. Config file {c.configfile} ready to use.")
+    else:
+        print("Setup Aborted.")
+        exit(1)
 # Run Scan
 elif command == 'scan':
     from pypowerwall import scan
 
     print("pyPowerwall [%s] - Scanner\n" % version)
     color = not args.nocolor
     ip = args.ip
     hosts = args.hosts
     timeout = args.timeout
     scan.scan(color, timeout, hosts, ip)
 # Set Powerwall Mode
 elif command == 'set':
+    # If no arguments, print usage
+    if not args.mode and not args.reserve and not args.current:
+        print("usage: pypowerwall set [-h] [-mode MODE] [-reserve RESERVE] [-current]")
+        exit(1)
     import pypowerwall
     print("pyPowerwall [%s] - Set Powerwall Mode and Power Levels\n" % version)
-    # Load email from auth file
-    auth_file = authpath + AUTHFILE
-    if not os.path.exists(auth_file):
-        print("ERROR: Auth file %s not found. Run 'setup' to create." % auth_file)
+    # Determine which cloud mode to use
+    pw = pypowerwall.Powerwall(auto_select=True, host="", authpath=authpath)
+    if not pw.client:
+        print("ERROR: FleetAPI and Cloud access are not configured. Run 'fleetapi' or 'setup' to create.")
         exit(1)
-    with open(auth_file, 'r') as file:
-        auth = json.load(file)
-    email = list(auth.keys())[0]
-    pw = pypowerwall.Powerwall(email=email, host="", authpath=authpath)
     if args.mode:
         mode = args.mode.lower()
         if mode not in ['self_consumption', 'backup', 'autonomous']:
             print("ERROR: Invalid Mode [%s] - must be one of self_consumption, backup, or autonomous" % mode)
             exit(1)
         print("Setting Powerwall Mode to %s" % mode)
         pw.set_mode(mode)
@@ -120,24 +142,18 @@
         current = float(pw.level())
         print("Setting Powerwall Reserve to Current Charge Level %s" % current)
         pw.set_reserve(current)
 # Get Powerwall Mode
 elif command == 'get':
     import pypowerwall
     # Load email from auth file
-    auth_file = authpath + AUTHFILE
-    if not os.path.exists(auth_file):
-        print("ERROR: Auth file %s not found. Run 'setup' to create." % auth_file)
-        exit(1)
-    with open(auth_file, 'r') as file:
-        auth = json.load(file)
-    email = list(auth.keys())[0]
-    pw = pypowerwall.Powerwall(email=email, host="", authpath=authpath)
+    pw = pypowerwall.Powerwall(auto_select=True, host="", authpath=authpath)
     output = {
         'site': pw.site_name(),
+        'site_id': pw.client.fleet.site_id,
         'din': pw.din(),
         'mode': pw.get_mode(),
         'reserve': pw.get_reserve(),
         'current': pw.level(),
         'grid': pw.grid(),
         'home': pw.home(),
         'battery': pw.battery(),
```

## pypowerwall/local/pypowerwall_local.py

```diff
@@ -26,14 +26,15 @@
         self.authmode = authmode  # cookie or token
         self.timeout = timeout
         self.timezone = timezone
 
         self.session = None
         self.pwcachetime = {}  # holds the cached data timestamps for api
         self.pwcacheexpire = pwcacheexpire  # seconds to expire cache
+        self.pwcache = {}  # holds the cached data for api
         self.pwcooldown = 0  # rate limit cooldown time - pause api calls
         self.vitals_api = True  # vitals api is available for local mode
 
     def authenticate(self):
         log.debug('Tesla local mode enabled')
         if self.poolmaxsize > 0:
             # Create session object for http connection re-use
```

## Comparing `pypowerwall/aux.py` & `pypowerwall/regex.py`

 * *Files identical despite different names*

## Comparing `pypowerwall-0.8.5.dist-info/LICENSE` & `pypowerwall-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pypowerwall-0.8.5.dist-info/METADATA` & `pypowerwall-0.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypowerwall
-Version: 0.8.5
+Version: 0.9.0
 Summary: Python module to access Tesla Energy Gateway for Powerwall and solar power data
 Home-page: https://github.com/jasonacox/pypowerwall
 Author: Jason Cox
 Author-email: jason@jasonacox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,39 +29,63 @@
 
 This python module can be used to monitor and control Tesla Energy Powerwalls. It uses a single class (`Powerwall`) and simple functions to fetch energy data and
 poll API endpoints on the Gateway.  
 
 pyPowerwall will cache the authentication headers and API call responses to help reduce the number of calls made to the Gateway (useful if you are polling the Powerwall frequently for trending data).
 
 * Works with Tesla Energy Gateways - Powerwall and Powerwall+
-* Simple access through easy to use functions using customer credentials
+* Access provided via Local Gateway API, Tesla FleetAPI (official), and Tesla Owners API (unofficial).
 * Will cache authentication to reduce load on Powerwall Gateway
-* Will cache responses to limit number of calls to Powerwall Gateway (optional/user definable)
+* Will cache responses to limit number of calls to Powerwall Gateway or Cloud (optional/user definable) 
 * Will re-use http connections to Powerwall Gateway for reduced load and faster response times
-* Easy access to decoded binary device vitals (/api/devices/vitals in JSON format)
-* Provides solar string data for Powerwall+ systems
-
-NOTE: This module requires that you (or your installer) have set up *Customer Login* credentials
-on your Powerwall Gateway.
+* Provides solar string data for Powerwall+ systems.
 
 ## Setup
 
 You can clone this repo or install the package with pip.  Once installed, pyPowerwall can scan your local network to find th IP address of your Tesla Powerwall Gateway.
 
 ```bash
 # Install pyPowerwall
 python3 -m pip install pypowerwall
 
-# Scan Network for Powerwalls
+# Option 1 - LOCAL MODE - Scan Network for Powerwalls
 python3 -m pypowerwall scan
 
-# (optional) Setup to use Tesla Owners cloud API
+# Option 2 - FLEETAPI MODE - Setup to use the official Tesla FleetAPI - See notes below.
+python3 -m pypowerwal fleetapi
+
+# Option 3 - CLOUD MODE -  Setup to use Tesla Owners cloud API
 python3 -m pypowerwall setup
 ```
 
+### Local Setup - Option 1
+
+The Tesla Powerwall, Powerwall 2 and Powerwall+ have a local LAN based API that you can use to monitor your Powerwall. It requires that you (or your installer) have the IP address (see scan above) and set up *Customer Login* credentials on your Powerwall Gateway. That is all that is needed to connect. Unfortunately, Powerwall 3 does not have a local API but you can access it via the cloud (options 2 and 3).
+
+### FleetAPI Setup - Option 2
+
+FleetAPI is the official Tesla API for accessing your Tesla products. This setup has some additional setup requirements that you will be prompted to do:
+
+Step 1 - Tesla Partner Account - Sign in to Tesla Developer Portal and make an App Access Request: See [Tesla App Access Request](https://developer.tesla.com/request) - During this process, you will need to set up and remember the following account settings: 
+
+   * CLIENT_ID - This will be provided to you by Tesla when your request is approved.
+   * CLIENT_SECRET - Same as above.
+   * DOMAIN - The domain name of a website your own and control.
+   * REDIRECT_URI - This is the URL that Tesla will direct you to after you authenticate. This landing URL (on your website) will extract the GET variable `code`, which is a one-time use authorization code needed during the pyPowerwall setup. You can use [index.html](./tools/fleetapi/index.html) on your site and update REDIRECT_URI with that url. Alternatively, you can just copy the URL from the 404 page during the authorization process (the code is in the URL).
+
+Step 2 - Run the [create_pem_key.py](./tools/fleetapi/create_pem_key.py) script and place the **public** key on your website at the URL: https://{DOMAIN}/.well-known/appspecific/com.tesla.3p.public-key.pem
+
+Step 3 - Run `python3 -m pypowerwal fleetapi` - The credentials and tokens will be stored in the `.pypowerwall.fleetapi` file.
+
+### Cloud Mode - Option 3
+
+The unofficial Tesla Owners API allows FleetAPI access (option 2) without having to set up a website and PEM key. Follow the directions given to you by running `python3 -m pypowerwall setup`. The credentials and site_id will be stored in `.pypowerwall.auth` and `.pypowerwall.site`.
+
+### FreeBSD Install
+
 FreeBSD users can install from ports or pkg [FreshPorts](https://www.freshports.org/net-mgmt/py-pypowerwall):
 
 Via pkg:
 ```bash
 # pkg install net-mgmt/py-pypowerwall
 ```
 
@@ -79,28 +103,31 @@
 
 ```python
     import pypowerwall
 
     # Optional: Turn on Debug Mode
     # pypowerwall.set_debug(True)
 
-    # Local Mode - Credentials for your Powerwall - Customer Login
-    password='password'
-    email='email@example.com'
+    # Option 1 - LOCAL MODE - Credentials for your Powerwall - Customer Login
+    password="password"
+    email="email@example.com"
     host = "10.0.1.123"               # Address of your Powerwall Gateway
     timezone = "America/Los_Angeles"  # Your local timezone
 
-    # (Optional) Cloud Mode - Requires Setup
-    password = ""
+    # Option 2 - FLEETAPI MODE - Requires Setup
+    host = password = email = ""
+    timezone = "America/Los_Angeles" 
+
+    # Option 3 - CLOUD MODE - Requires Setup
+    host = password = ""
     email='email@example.com'
-    host = ""
-    timezone = "America/Los_Angeles"  # Your local timezone
+    timezone = "America/Los_Angeles"
  
-    # Connect to Powerwall
-    pw = pypowerwall.Powerwall(host,password,email,timezone)
+    # Connect to Powerwall - auto_select mode (local, fleetapi, cloud)
+    pw = pypowerwall.Powerwall(host,password,email,timezone,auto_select=True)
 
     # Some System Info
     print("Site Name: %s - Firmware: %s - DIN: %s" % (pw.site_name(), pw.version(), pw.din()))
     print("System Uptime: %s\n" % pw.uptime())
 
     # Pull Sensor Power Data
     grid = pw.grid()
@@ -129,35 +156,38 @@
 
     # Display String Data
     print("String Data: %r\n" % pw.strings())
 
 ```
 
 ### pyPowerwall Module Class and Functions 
+
 ```
  set_debug(True, color=True)
 
  Classes
     Powerwall(host, password, email, timezone, pwcacheexpire, timeout, poolmaxsize, 
-              cloudmode, siteid, authpath, authmode, cachefile)
+               cloudmode, siteid, authpath, authmode, cachefile, fleetapi, auto_select)
 
  Parameters
     host                      # Hostname or IP of the Tesla gateway
     password                  # Customer password for gateway
     email                     # (required) Customer email for gateway / cloud
     timezone                  # Desired timezone
     pwcacheexpire = 5         # Set API cache timeout in seconds
     timeout = 5               # Timeout for HTTPS calls in seconds
     poolmaxsize = 10          # Pool max size for http connection re-use (persistent
                                 connections disabled if zero)
     cloudmode = False         # If True, use Tesla cloud for data (default is False)
-    siteid                    # If cloudmode is True, use this siteid (default is None)  
-    authpath                  # Path to cloud auth and site cache files (default is "")
+    siteid = None             # If cloudmode is True, use this siteid (default is None)
+    authpath = ""             # Path to cloud auth and site files (default current directory)
     authmode = "cookie"       # "cookie" (default) or "token" - use cookie or bearer token for auth
     cachefile = ".powerwall"  # Path to cache file (default current directory)
+    fleetapi = False          # If True, use Tesla FleetAPI for data (default is False)
+    auto_select = False       # If True, select the best available mode to connect (default is False)
 
  Functions 
     poll(api, json, force)    # Return data from Powerwall api (dict if json=True, bypass cache force=True)
     post(api, payload, json)  # Send payload to Powerwall api (dict if json=True)
     level()                   # Return battery power level percentage
     power()                   # Return power data returned as dictionary
     site(verbose)             # Return site sensor data (W or raw JSON if verbose=True)
@@ -172,29 +202,25 @@
     uptime()                  # Return uptime - string hms format
     version()                 # Return system version
     status(param)             # Return status (JSON) or individual param
     site_name()               # Return site name
     temps()                   # Return Powerwall Temperatures
     alerts()                  # Return array of Alerts from devices
     system_status(json)       # Returns the system status
-    battery_blocks(json)      # Returns battery specific information merged from 
-                              # system_status() and vitals()
-    grid_status(type)         # Return the power grid status, type ="string" (default),
-                              # "json", or "numeric":
+    battery_blocks(json)      # Returns battery specific information merged from system_status() and vitals()
+    grid_status(type)         # Return the power grid status, type ="string" (default), "json", or "numeric"
                               #     - "string": "UP", "DOWN", "SYNCING"
                               #     - "numeric": -1 (Syncing), 0 (DOWN), 1 (UP)
-    is_connected()            # Returns True if able to connect to Powerwall
+    is_connected()            # Returns True if able to connect and login to Powerwall
     get_reserve(scale)        # Get Battery Reserve Percentage
     get_mode()                # Get Current Battery Operation Mode
-    set_reserve(level)        # Set Battery Reserve Percentage (only cloud mode)
-    set_mode(mode)            # Set Current Battery Operation Mode (only cloud mode)
+    set_reserve(level)        # Set Battery Reserve Percentage
+    set_mode(mode)            # Set Current Battery Operation Mode
     get_time_remaining()      # Get the backup time remaining on the battery
-
-    set_operation(level, mode, json)        # Set Battery Reserve Percentage and/or Operation Mode
-    
+    set_operation(level, mode, json)  # Set Battery Reserve Percentage and/or Operation Mode
 ```
 
 ## Tools
 
 The following are some useful tools based on pypowerwall:
 
 * [Powerwall Proxy](proxy) - Use this caching proxy to handle authentication to the Powerwall Gateway and make basic read-only API calls to /api/meters/aggregates (power metrics), /api/system_status/soe (battery level) and many [others](https://github.com/jasonacox/pypowerwall/blob/main/proxy/HELP.md). This is useful for metrics gathering tools like telegraf to pull metrics without needing to authenticate. Because pyPowerwall is designed to cache the auth and high frequency API calls, this will also reduce the load on the Gateway and prevent crash/restart issues that can happen if too many session are created on the Gateway.
```

## Comparing `pypowerwall-0.8.5.dist-info/RECORD` & `pypowerwall-0.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-pypowerwall/__init__.py,sha256=zptASN1StYU71e9z9hSviBxeKMxq4dh0mmxNWabbXIk,32843
-pypowerwall/__main__.py,sha256=yDDWrUHvdk_jy5JUOqHYWNgGyTsBaL9j8DqQQtoE080,5835
-pypowerwall/aux.py,sha256=9VR4d4q163AdQQ4ELHLUYEH-RDOr-490cNZiGZFXlXM,1889
+pypowerwall/__init__.py,sha256=3U-2oGFMRFGCDoheALz1bi445foXZSBDA2ymQ_6ucvg,37170
+pypowerwall/__main__.py,sha256=-sFOtMlKeGkk0DXU3y0suPCMNzVF_WipU5ayZlJJT34,6434
 pypowerwall/exceptions.py,sha256=D2TxwF42_quXoVr7CSQ1ifhSms_eHBJnFwy9l-bdtB0,133
 pypowerwall/pypowerwall_base.py,sha256=HKTNQQ59QfqtZtqYBe5rSkB8qyfZq9WPOwywzFvK7bs,2897
+pypowerwall/regex.py,sha256=9VR4d4q163AdQQ4ELHLUYEH-RDOr-490cNZiGZFXlXM,1889
 pypowerwall/scan.py,sha256=DM9CxQLceu0bmyPaH8fNRdLgkS3oe4ata_78eObSNn8,6718
 pypowerwall/cloud/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pypowerwall/cloud/decorators.py,sha256=aDwS9G-g7B8Md0dPPucHVd5mIdvrGKlz8typC-YHBCU,638
 pypowerwall/cloud/exceptions.py,sha256=tBSq0cUJvINmTMIcaq53iceSOmh-7hntqHIRCG6PEL0,242
 pypowerwall/cloud/mock_data.py,sha256=8CLdxyAhMY5I-tYsxUqcjGHth4T5NJkqvm-V6GUIAXM,18733
 pypowerwall/cloud/pypowerwall_cloud.py,sha256=DYu7C1KTd8kyNy-tTSwML_wvvkypjRIOmNAPU5vU4EQ,46441
 pypowerwall/cloud/stubs.py,sha256=JQXgAONPzJSuK7_N55ODBOHAMpm_CfZ4YYmJFbJEWvg,4355
+pypowerwall/fleetapi/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pypowerwall/fleetapi/__main__.py,sha256=MUN8z4p6hdQJ5Ko9Zu1L-qxENyiS_xjEgfD-3dyP1w8,5747
+pypowerwall/fleetapi/decorators.py,sha256=GWP392gJX5ENY3siVKlZsnFnZyynM8DwT5D5eZbSER0,650
+pypowerwall/fleetapi/exceptions.py,sha256=lHUVK_z1apfnjsvsR9maxtJ5y72eKrTu4U0cwAlbFBI,254
+pypowerwall/fleetapi/fleetapi.py,sha256=jJBzsGj1eNVM1tFpW2Nn06If0Quiy0-bhwzXEDq45F4,31740
+pypowerwall/fleetapi/mock_data.py,sha256=8CLdxyAhMY5I-tYsxUqcjGHth4T5NJkqvm-V6GUIAXM,18733
+pypowerwall/fleetapi/pypowerwall_fleetapi.py,sha256=ljaKDXC-ow3JPZu3N73X403mjJYX13fQ4dqT8jEwEDA,33528
+pypowerwall/fleetapi/stubs.py,sha256=JQXgAONPzJSuK7_N55ODBOHAMpm_CfZ4YYmJFbJEWvg,4355
 pypowerwall/local/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pypowerwall/local/exceptions.py,sha256=JRm141HHbwKSkdeIWttOrniQTeehGJ3Zo6Fg9KH4Scc,92
-pypowerwall/local/pypowerwall_local.py,sha256=4DcdxnJT7e2SxDgYqXhWOlZUvM1bGEiGfGOEuyGfZ68,20404
+pypowerwall/local/pypowerwall_local.py,sha256=cxB--lok75GPgDdU8_tp9HOxNdZLN-ZlX6stjbqvEvY,20463
 pypowerwall/local/tesla_pb2.py,sha256=l3faEX13xLWbWh6KRtbyCClK3zXpyN0LY6y3kM3Dpp8,71273
-pypowerwall-0.8.5.dist-info/LICENSE,sha256=9cu5S_JpsnnwkV5ZWabxJwmoObWpOncMZaKdYe9vrH0,1066
-pypowerwall-0.8.5.dist-info/METADATA,sha256=oIAuIoazgdrAk028Qx19RqQMeGRgCc2hJheWgN5LRm4,41728
-pypowerwall-0.8.5.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-pypowerwall-0.8.5.dist-info/top_level.txt,sha256=xAKahe-O0UjzTWlyxF1oHIZuAXkioYNTlC32ttXxjaM,12
-pypowerwall-0.8.5.dist-info/RECORD,,
+pypowerwall-0.9.0.dist-info/LICENSE,sha256=9cu5S_JpsnnwkV5ZWabxJwmoObWpOncMZaKdYe9vrH0,1066
+pypowerwall-0.9.0.dist-info/METADATA,sha256=we_9OiLthlT_DLJzbDmTTrI1NPilFL0uEttBLCquLsw,44205
+pypowerwall-0.9.0.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+pypowerwall-0.9.0.dist-info/top_level.txt,sha256=xAKahe-O0UjzTWlyxF1oHIZuAXkioYNTlC32ttXxjaM,12
+pypowerwall-0.9.0.dist-info/RECORD,,
```

