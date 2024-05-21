# Comparing `tmp/ansar_connect-0.1.250.tar.gz` & `tmp/ansar_connect-0.1.251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.250.tar", last modified: Sun May 19 15:10:19 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.251.tar", last modified: Mon May 20 23:59:06 2024, max compression
```

## Comparing `ansar_connect-0.1.250.tar` & `ansar_connect-0.1.251.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 15:10:19.827104 ansar_connect-0.1.250/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.250/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-19 15:10:19.827104 ansar_connect-0.1.250/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.250/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-15 01:33:06.000000 ansar_connect-0.1.250/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-19 15:10:19.827104 ansar_connect-0.1.250/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-15 01:32:55.000000 ansar_connect-0.1.250/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 15:10:19.823104 ansar_connect-0.1.250/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 15:10:19.823104 ansar_connect-0.1.250/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 15:10:19.827104 ansar_connect-0.1.250/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.250/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.250/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.250/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.250/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 15:10:19.827104 ansar_connect-0.1.250/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-19 15:10:16.000000 ansar_connect-0.1.250/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.250/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88788 2024-05-18 21:19:19.000000 ansar_connect-0.1.250/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.250/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.250/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.250/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15675 2024-05-19 00:14:47.000000 ansar_connect-0.1.250/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.250/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.250/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.250/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9680 2024-05-18 21:34:58.000000 ansar_connect-0.1.250/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.250/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34066 2024-05-19 15:06:41.000000 ansar_connect-0.1.250/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.250/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42061 2024-05-18 21:24:11.000000 ansar_connect-0.1.250/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.250/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.250/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.250/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.250/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-19 15:10:19.827104 ansar_connect-0.1.250/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-19 15:10:19.000000 ansar_connect-0.1.250/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-19 15:10:19.000000 ansar_connect-0.1.250/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-19 15:10:19.000000 ansar_connect-0.1.250/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-19 15:10:19.000000 ansar_connect-0.1.250/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-19 15:10:19.000000 ansar_connect-0.1.250/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-19 15:10:19.000000 ansar_connect-0.1.250/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-20 23:59:06.032530 ansar_connect-0.1.251/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.251/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-20 23:59:06.032530 ansar_connect-0.1.251/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.251/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-15 01:33:06.000000 ansar_connect-0.1.251/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-20 23:59:06.032530 ansar_connect-0.1.251/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-15 01:32:55.000000 ansar_connect-0.1.251/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-20 23:59:06.028530 ansar_connect-0.1.251/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-20 23:59:06.028530 ansar_connect-0.1.251/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-20 23:59:06.032530 ansar_connect-0.1.251/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.251/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.251/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.251/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.251/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-20 23:59:06.032530 ansar_connect-0.1.251/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-20 23:59:02.000000 ansar_connect-0.1.251/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.251/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88788 2024-05-18 21:19:19.000000 ansar_connect-0.1.251/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.251/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.251/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.251/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.251/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.251/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.251/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.251/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9680 2024-05-18 21:34:58.000000 ansar_connect-0.1.251/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.251/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.251/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.251/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42334 2024-05-19 21:19:26.000000 ansar_connect-0.1.251/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.251/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.251/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.251/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.251/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-20 23:59:06.032530 ansar_connect-0.1.251/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-20 23:59:06.000000 ansar_connect-0.1.251/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-20 23:59:06.000000 ansar_connect-0.1.251/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-20 23:59:06.000000 ansar_connect-0.1.251/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-20 23:59:06.000000 ansar_connect-0.1.251/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-20 23:59:06.000000 ansar_connect-0.1.251/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-20 23:59:06.000000 ansar_connect-0.1.251/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.250/LICENSE` & `ansar_connect-0.1.251/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/PKG-INFO` & `ansar_connect-0.1.251/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.250
+Version: 0.1.251
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.250/README.md` & `ansar_connect-0.1.251/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/pyproject.toml` & `ansar_connect-0.1.251/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/setup.py` & `ansar_connect-0.1.251/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.251/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.251/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.251/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.251/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/__init__.py` & `ansar_connect-0.1.251/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 957e2dfb1cf2245fcdfdfb69213e95935aa8e5d4
-Version: 0.1.249 (2024-05-20@03:10:16+NZST)
+Commit: 79378ded8fe6d6ff359bb878e4475472c108d301
+Version: 0.1.250 (2024-05-21@11:59:02+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.250/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.251/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/directory.py` & `ansar_connect-0.1.251/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.251/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.251/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/group_if.py` & `ansar_connect-0.1.251/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/grouping.py` & `ansar_connect-0.1.251/src/ansar/connect/grouping.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 		:type get_ready: float
 		:param session: object to be created at Ready state, or None
 		:type session: CreateFrame
 		:param resident_code: facilitate a series of sessions
 		:type resident_code: bool
 		:param until_stopped: a flag passed to AddressGroup
 		:type until_stopped: bool
-		:rtype: an ansar address
+		:rtype: ansar address
 		"""
 		for k in self.member_frame.keys():
 			setattr(self, k, None)	# Fill with blanks.
 		a = owner.create(AddressGroup, self.member_frame, session=session, resident_code=resident_code, get_ready=get_ready, until_stopped=until_stopped)
 		return a
 
 	def update(self, message):
@@ -79,14 +79,21 @@
 		:rtype: None
 		"""
 		if message.key in self.member_frame:
 			setattr(self, message.key, message.address)
 
 # Runtime image.
 class GroupUpdate(object):
+	"""A group notification, an address was acquired or lost.
+
+	:param key: name of the address
+	:type key: str
+	:param address: new address or None
+	:type address: ansar address
+	"""
 	def __init__(self, key=None, address=None):
 		self.key = key
 		self.address = address
 
 UPDATE_GROUP_SCHEMA = {
 	'key': ar.Unicode(),
 	'address': ar.Address(),
```

### Comparing `ansar_connect-0.1.250/src/ansar/connect/moving.py` & `ansar_connect-0.1.251/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/networking.py` & `ansar_connect-0.1.251/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.251/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/node.py` & `ansar_connect-0.1.251/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.251/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/procedure.py` & `ansar_connect-0.1.251/src/ansar/connect/procedure.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 	hb = open_home(home)
 
 	# if not hb.role_exists(group_role):
 	#	e = ar.Failed(group_exists=(f'group "{group}" not found', None))
 	#	raise ar.Incomplete(e)
 	# TBD - auto-create or not.
 	settings = GroupSettings()
-	hr = hb.open_role(group_role, settings, None, ar.NodeProperties())
+	hr = hb.open_role(group_role, settings, None, ar.NodeProperties(executable='ansar-group'))
 
 	_, running = role_status(self, hb, [group_role])
 	if running:
 		e = ar.Failed(group_running=(f'group "{group}" is already running', None))
 		raise ar.Incomplete(e)
 
 	settings = hr.role_settings[2]				# From the group.
@@ -390,15 +390,15 @@
 
 	_, running = role_status(self, hb, [group_role])
 	if running:
 		e = ar.Failed(group_running=(f'group "{group}" is already running', None))
 		raise ar.Incomplete(e)
 
 	settings = GroupSettings()
-	hr = hb.open_role(group_role, settings, None, ar.NodeProperties())
+	hr = hb.open_role(group_role, settings, None, ar.NodeProperties(executable='ansar-group'))
 
 	settings = hr.role_settings[2]				# From the group.
 	connect_above = settings.connect_above
 	accept_below = ar.LocalPort(0)				# Disabled.
 
 	a = self.create(ar.ServiceDirectory, ar.ScopeOfService.GROUP, connect_above, accept_below)
 	self.assign(a, None)
@@ -571,14 +571,15 @@
 		self.send(ar.Close(), session)
 		self.select(ar.Closed, ar.Stop)
 
 def login_read(self, login_token, session, account):
 	read = LoginRead(login_token=login_token,
 		login_id=account.login_id)
 	fill_form(self, read)
+	self.console(f'login-id: {read.login_id}')
 	self.send(read, session)
 	m = self.select(LoginPage, ar.Faulted, ar.Abandoned, ar.Stop)
 	if isinstance(m, LoginPage):
 		output_login(m, account)
 	elif isinstance(m, ar.Faulted):
 		return m
 	elif isinstance(m, ar.Abandoned):
```

### Comparing `ansar_connect-0.1.250/src/ansar/connect/product.py` & `ansar_connect-0.1.251/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/socketry.py` & `ansar_connect-0.1.251/src/ansar/connect/socketry.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,14 +693,23 @@
 #
 #
 class INITIAL: pass
 class PENDING: pass
 class NORMAL: pass
 
 class SocketProxy(ar.Point, ar.StateMachine):
+	"""Local representation of an object at remote end of a network connection.
+
+	:param s: associated network connection
+	:type s: socket descriptor
+	:param channel: async socket loop
+	:type channel: internal
+	:param stream: associated buffering
+	:type stream: internal
+	"""
 	def __init__(self, s, channel, stream):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
 		self.s = s
 		self.channel = channel
 		self.stream = stream
```

### Comparing `ansar_connect-0.1.250/src/ansar/connect/standard.py` & `ansar_connect-0.1.251/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/transporting.py` & `ansar_connect-0.1.251/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.251/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar/connect/wan.py` & `ansar_connect-0.1.251/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.250/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.251/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.250
+Version: 0.1.251
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.250/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.251/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

