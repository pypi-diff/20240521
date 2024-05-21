# Comparing `tmp/STEP.py-2.8.tar.gz` & `tmp/STEP.py-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STEP.py-2.8.tar", last modified: Tue Sep 12 00:56:24 2023, max compression
+gzip compressed data, was "STEP.py-2.9.tar", last modified: Mon Sep 18 08:39:40 2023, max compression
```

## Comparing `STEP.py-2.8.tar` & `STEP.py-2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-09-12 00:56:24.818853 STEP.py-2.8/
--rw-r--r--   0 dave       (501) staff       (20)     1068 2023-08-01 01:10:57.000000 STEP.py-2.8/LICENSE.txt
--rw-r--r--   0 dave       (501) staff       (20)     6610 2023-09-12 00:56:24.819065 STEP.py-2.8/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     6314 2023-08-01 01:10:57.000000 STEP.py-2.8/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-09-12 00:56:24.767317 STEP.py-2.8/STEP/
--rwxr-xr-x   0 dave       (501) staff       (20)     1317 2022-04-21 05:05:19.000000 STEP.py-2.8/STEP/Cleaner.py
--rwxr-xr-x   0 dave       (501) staff       (20)    41946 2023-09-12 00:41:58.000000 STEP.py-2.8/STEP/REST.py
--rwxr-xr-x   0 dave       (501) staff       (20)    14931 2023-03-10 02:02:08.000000 STEP.py-2.8/STEP/SOAP.py
--rwxr-xr-x   0 dave       (501) staff       (20)    11053 2022-04-21 05:05:19.000000 STEP.py-2.8/STEP/XML.py
--rwxr-xr-x   0 dave       (501) staff       (20)  3190837 2023-09-12 00:53:02.000000 STEP.py-2.8/STEP/XSD.py
--rwxr-xr-x   0 dave       (501) staff       (20)        0 2023-03-10 02:02:08.000000 STEP.py-2.8/STEP/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-09-12 00:56:24.778602 STEP.py-2.8/STEP.py.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)     6610 2023-09-12 00:56:24.000000 STEP.py-2.8/STEP.py.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      379 2023-09-12 00:56:24.000000 STEP.py-2.8/STEP.py.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-09-12 00:56:24.000000 STEP.py-2.8/STEP.py.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)      117 2023-09-12 00:56:24.000000 STEP.py-2.8/STEP.py.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)        5 2023-09-12 00:56:24.000000 STEP.py-2.8/STEP.py.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-09-12 00:56:24.807855 STEP.py-2.8/bin/
--rwxr-xr-x   0 dave       (501) staff       (20)      187 2023-09-12 00:45:46.000000 STEP.py-2.8/bin/excel2step.py
--rwxr-xr-x   0 dave       (501) staff       (20)      287 2022-07-26 22:14:49.000000 STEP.py-2.8/bin/step.rest.py
--rwxr-xr-x   0 dave       (501) staff       (20)      716 2022-07-26 22:16:51.000000 STEP.py-2.8/bin/step.soap.py
--rwxr-xr-x   0 dave       (501) staff       (20)    19193 2023-04-06 01:08:13.000000 STEP.py-2.8/bin/step2uml.py
--rwxr-xr-x   0 dave       (501) staff       (20)    16469 2023-03-10 02:02:08.000000 STEP.py-2.8/bin/uml2step.py
--rw-r--r--   0 dave       (501) staff       (20)       79 2023-09-12 00:56:24.821402 STEP.py-2.8/setup.cfg
--rwxr-xr-x   0 dave       (501) staff       (20)      980 2023-09-12 00:51:23.000000 STEP.py-2.8/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-09-12 00:56:24.818013 STEP.py-2.8/test/
--rwxr-xr-x   0 dave       (501) staff       (20)    10118 2022-09-01 05:43:58.000000 STEP.py-2.8/test/test_rest.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-09-18 08:39:40.544394 STEP.py-2.9/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1068 2022-09-28 02:37:16.000000 STEP.py-2.9/LICENSE.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6610 2023-09-18 08:39:40.545394 STEP.py-2.9/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6314 2022-09-28 02:37:16.000000 STEP.py-2.9/README.md
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-09-18 08:39:40.527393 STEP.py-2.9/STEP/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1317 2022-04-21 05:05:19.000000 STEP.py-2.9/STEP/Cleaner.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    42972 2023-09-18 08:33:20.000000 STEP.py-2.9/STEP/REST.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    12322 2023-09-18 08:36:22.000000 STEP.py-2.9/STEP/SOAP.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    11014 2023-09-18 08:24:48.000000 STEP.py-2.9/STEP/XML.py
+-rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)  3190837 2023-09-13 01:31:12.000000 STEP.py-2.9/STEP/XSD.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)        0 2022-09-28 02:37:16.000000 STEP.py-2.9/STEP/__init__.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-09-18 08:39:40.534394 STEP.py-2.9/STEP.py.egg-info/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6610 2023-09-18 08:39:40.000000 STEP.py-2.9/STEP.py.egg-info/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      379 2023-09-18 08:39:40.000000 STEP.py-2.9/STEP.py.egg-info/SOURCES.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2023-09-18 08:39:40.000000 STEP.py-2.9/STEP.py.egg-info/dependency_links.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      117 2023-09-18 08:39:40.000000 STEP.py-2.9/STEP.py.egg-info/requires.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        5 2023-09-18 08:39:40.000000 STEP.py-2.9/STEP.py.egg-info/top_level.txt
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-09-18 08:39:40.542394 STEP.py-2.9/bin/
+-rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)      187 2023-09-13 01:31:12.000000 STEP.py-2.9/bin/excel2step.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      287 2022-07-26 22:14:49.000000 STEP.py-2.9/bin/step.rest.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      716 2022-07-26 22:16:51.000000 STEP.py-2.9/bin/step.soap.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    19193 2023-03-22 04:38:13.000000 STEP.py-2.9/bin/step2uml.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    16469 2022-07-19 06:08:05.000000 STEP.py-2.9/bin/uml2step.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-09-18 08:39:40.545394 STEP.py-2.9/setup.cfg
+-rwxr-xr-x   0 eddo8    (197610) eddo8    (197610)      980 2023-09-18 08:25:34.000000 STEP.py-2.9/setup.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-09-18 08:39:40.543395 STEP.py-2.9/test/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    10118 2022-09-01 05:43:58.000000 STEP.py-2.9/test/test_rest.py
```

### Comparing `STEP.py-2.8/LICENSE.txt` & `STEP.py-2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/PKG-INFO` & `STEP.py-2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: STEP.py
-Version: 2.8
+Version: 2.9
 Home-page: https://github.com/eddo888/STEP.py
-Download-URL: https://github.com/eddo888/STEP.py/archive/2.8.tar.gz
+Download-URL: https://github.com/eddo888/STEP.py/archive/2.9.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # STEP.py
```

### Comparing `STEP.py-2.8/README.md` & `STEP.py-2.9/README.md`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/STEP/Cleaner.py` & `STEP.py-2.9/STEP/Cleaner.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/STEP/REST.py` & `STEP.py-2.9/STEP/REST.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 from datetime import datetime
 from io import StringIO, BytesIO
 from dotmap import DotMap
 
 from Perdy.parser import doParse, printXML
 from Perdy.pretty import prettyPrint
 from Argumental.Argue import Argue
-from Spanners.Squirrel import Squirrel
 
 args = Argue()
-squirrel = Squirrel()
 
 dts = '%Y-%m-%dT%H:%M:%S'
 
 #====================================================================================================
 node_types = {
 	'P': 'product',
 	'E': 'entity',
@@ -48,15 +46,15 @@
 	@args.property(short='H', default='http://host')
 	def hostname(self): return
 
 	@args.property(short='U', default='stepsys')
 	def username(self): return
 
 	@args.property(short='P')
-	def password(self): return squirrel.get('stibo:%s:%s'%(self.hostname, self.username))
+	def password(self): return
 
 	@args.property(short='v', flag=True)
 	def verbose(self): return
 
 	@args.property(short='x', flag=True, help='output in xml')
 	def asXML(self): return
 
@@ -563,26 +561,29 @@
 		except:
 			return result
 
 
 	#________________________________________________________________________________________________
 	@args.operation(help='set values of product by id')
 	@args.parameter(name='id', help='the ID of product')
-	@args.parameter(name='attributeID', help='the ID of product')
-	@args.parameter(name='value', help='the ID of product')
-	def update(self, id, attributeID, value):
+	@args.parameter(name='attributeID', help='the ID of attribute')
+	@args.parameter(name='value', help='the actual value')
+	@args.parameter(name='unit', short='u', help='unit of measure')
+	def update(self, id, attributeID, value, unit=None):
 		headers={
 			"accept": "application/json",
 			"Content-Type": "application/json",
 		}
 		payload={
 			"value": {
 				"value":value
 			}
 		}
+		if unit:
+			payload['value']['unit'] = unit
 		result = super().put('%s/%s/values/%s'%(
 			self.base, id, attributeID), body=json.dumps(payload), headers=headers
 		)
 		return json.loads(result)
 
 
 	#________________________________________________________________________________________________
@@ -649,20 +650,33 @@
 
 
 	#________________________________________________________________________________________________
 	@args.operation(help='update values of entity by id')
 	@args.parameter(name='id', help='the ID of entity')
 	@args.parameter(name='name', help='attribute ID')
 	@args.parameter(name='value', help='attribute Value')
-	def update(self, id, name, value):
-		body = json.dumps(dict(value=dict(value=value)))
-		headers = { 'Content-Type' : 'application/json' }
-		return super().put('%s/%s/values/%s'%(self.base, id, name), body=body, headers=headers)
+	@args.parameter(name='unit', short='u', help='unit of measure')
+	def update(self, id, attributeID, value, unit=None):
+		headers={
+			"accept": "application/json",
+			"Content-Type": "application/json",
+		}
+		payload={
+			"value": {
+				"value":value
+			}
+		}
+		if unit:
+			payload['value']['unit'] = unit
+		result = super().put('%s/%s/values/%s'%(
+			self.base, id, attributeID), body=json.dumps(payload), headers=headers
+		)
+		return json.loads(result)
+
 
-	
 	#________________________________________________________________________________________________
 	@args.operation(help='search for entities')
 	@args.parameter(name='below_id', help='the ID of entity to search within')
 	@args.parameter(name='conditionType', choices=['name'], default='name', help='the type of confidition')
 	@args.parameter(name='operator', choices=['eq','exists','like','neq'], default='eq', help='comparison choices')
 	@args.parameter(name='queryString', help='string to search for')
 	def search(self, below_id, conditionType, operator, queryString):
@@ -765,14 +779,38 @@
 	
 	#________________________________________________________________________________________________
 	@args.operation(help='get values of classification by id')
 	@args.parameter(name='id', help='the ID of classification')
 	def values(self, id):
 		return super().get('%s/%s/values'%(self.base,id))
 	
+	#________________________________________________________________________________________________
+	@args.operation(help='set values of classification by id')
+	@args.parameter(name='id', help='the ID of classification')
+	@args.parameter(name='attributeID', help='the ID of attribute')
+	@args.parameter(name='value', help='the actual value')
+	@args.parameter(name='unit', short='u', help='unit of measure')
+	def update(self, id, attributeID, value, unit=None):
+		headers={
+			"accept": "application/json",
+			"Content-Type": "application/json",
+		}
+		payload={
+			"value": {
+				"value":value
+			}
+		}
+		if unit:
+			payload['value']['unit'] = unit
+		result = super().put('%s/%s/values/%s'%(
+			self.base, id, attributeID), body=json.dumps(payload), headers=headers
+		)
+		return json.loads(result)
+
+
 
 #====================================================================================================
 @args.command(name='endpoints')
 class Endpoints(STEP):
 
 	base = 'integrationendpoints'
```

### Comparing `STEP.py-2.8/STEP/SOAP.py` & `STEP.py-2.9/STEP/SOAP.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 from suds.client import Client
 from suds.sax.text import Text
 from suds.wsse import Security, UsernameToken
 from suds.xsd.sxbasic import Complex
 from dotmap import DotMap
 
 from Argumental.Argue import Argue
-from Spanners.Squirrel import Squirrel
 from Perdy.pretty import prettyPrint
 from Baubles.Logger import Logger
 
 args = Argue()
-squirrel = Squirrel()
 logger = Logger()
 
 def quietly():
 	for name in [
 		'boto3.resources.action',
 		'boto3.resources.factory',
 		'botocore.auth',
@@ -69,22 +67,19 @@
 	@args.property(short='w', default='StepWS/stepws?wsdl')
 	def wsdlpath(self): return
 
 	@args.property(short='u', default='stepsys')
 	def username(self): return
 
 	@args.property(short='p')
-	def password(self):
-		return squirrel.get('%s:%s'%(self.hostname, self.username))
-	
+	def password(self): return 
 
 	@args.property(short='v', flag=True)
 	def verbose(self): return False
 
-	#.............................................................
 	def __init__(self, hostname=None, wsdlpath=None, username=None, password=None, verbose=False):
 		if hostname: self.hostname = hostname
 		if wsdlpath: self.wsdlpath = wsdlpath
 		if username: self.username = username
 		if password: self.password = password
 		if verbose:  self.verbose  = verbose
 		
@@ -102,61 +97,55 @@
 		self._types = dict(map(lambda x: 
 			(x[0].name, x[0]), self.client.sd[0].types
 		))
 		
 		return
 
 
-	#.............................................................
 	@args.operation
 	def service(self):
 		print(self.client)
 
 
-	#.............................................................
 	def createAccessControl(self):
 		request = self.client.factory.create('ns1:accessContext')
 		request.userName = self.username
 		request.password = self.password
 		return request
 	
 
-	#.............................................................
 	@args.operation
 	def directory(self):
 		'''
 		print out the client specification
 		'''
 		return sorted(self.client.sd[0].service.ports[0].methods.keys())
 	
 
-	#.............................................................
 	@args.operation
 	def types(self):
 		'''
 		print out the client types
 		'''
 		return sorted(self._types.keys())
 		
 
-	#.............................................................
 	def typo(self, part):
 		name = str(part[0].name)
 		if name not in self._types.keys():
 			name = '%sType'%name
 		if name not in self._types.keys():
 			return name
 		t = self._types[name]
 		d = dict()
 		if isinstance(t, Complex):
 			d[t.name] = map(self.typo, t.children())
 		return d
 		
 
-	#.............................................................
 	@args.operation
 	def describe(self, name):
 		'''
 		describe a method
 		'''
 		method = self.client.sd[0].service.ports[0].methods[name]
 		result = {
@@ -172,84 +161,80 @@
 				)
 			)
 		}
 		#print method.soap
 		return(result)
 			
 
-	#.............................................................
 	@args.operation
 	def dummy(self, name):
 		'''
 		describe a method
 		'''
 		request = self.createAccessControl()
 		return self.client.service.dummy(request,name)
 
 
-	#.............................................................
 	@args.operation
 	def getWorkspaces(self):
 		response = self.client.service.getWorkspaces(self.username,self.password)
 		return response
 
 
-	#.............................................................
+	@args.operation
+	def getContexts(self):
+		response = self.client.service.getContexts(self.username,self.password)
+		return response
+
+
 	@args.operation
 	def approve(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.approve(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getBaseProduct(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getBaseProduct(request, nodeURL)
 		return response
 		
 
-	#.............................................................
 	@args.operation
 	def createProduct(self, productID, name, objectTypeURL, parentURL, beforeURL=None):
 		request = self.createAccessControl()
 		response = self.client.service.createProduct(request,productID, name, objectTypeURL, parentURL, beforeURL) 
 		return response
 													 
-	#.............................................................
 	@args.operation
 	def createClassification(self, classificationID, name, objectTypeURL, parentURL, beforeURL=None):
 		request = self.createAccessControl()
 		response = self.client.service.createClassification(request, classificationID, name, objectTypeURL, parentURL, beforeURL) 
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getClassifications(self, nodeURL):
 		request = self.createAccessControl()
 		return self.client.service.getClassifications(request, nodeURL)
 		
 
-	#.............................................................
 	@args.operation
 	def addClassification(self, nodeURL, classificationURL):
 		request = self.createAccessControl()
 		return self.client.service.addClassification(request, nodeURL, classificationURL)
 		
 
-	#.............................................................
 	@args.operation
 	def getAttributeDetails(self, nodeURL):
 		request = self.createAccessControl()
 		return self.client.service.getAttributeDetails(request, nodeURL)
 		
 
-	#.............................................................
 	@args.operation
 	@args.parameter(name='urls', short='u', flag=True, help='show attribute urls')
 	@args.parameter(name='useNames', short='n', flag=True, help='use attribute name not id')
 	@args.parameter(name='ignoreNulls', short='i', flag=True)
 	def getValues(self, nodeURL, urls=False, useNames=False, ignoreNulls=False):
 		request = self.createAccessControl()
 		response = self.client.service.getValues(request, nodeURL)
@@ -266,15 +251,14 @@
 			elif useNames:
 				values[value['attributeTtitle']] = v
 			else:
 				values[value['attributeURL'].split('=')[1]] = v
 		return values
 
 
-	#.............................................................
 	@args.operation
 	@args.parameter(name='nameEqValues', short='e', nargs='*', metavar='name=value', help='name is the attribute id')
 	def setValues(self, nodeURL, nameEqValues=[]):
 		request = self.createAccessControl()
 		ns1_values = list()
 		for nameEqValue in nameEqValues:
 			parts = nameEqValue.split('=')
@@ -288,197 +272,174 @@
 			ns1_values.append(ns1_value)
 
 			#print(dir(ns1_value))
 		response = self.client.service.setValues(request, nodeURL, ns1_values)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getName(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getName(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	@args.parameter(name='caseSensitive', short='i', flag=True)
 	@args.parameter(name='sort', short='s', flag=True)
 	@args.parameter(name='offset', type=int, default=0)
 	@args.parameter(name='maxCount', type=int, default=100)
 	def queryById(self, queryString, caseSensitive=False, sort=False, offset=0, maxCount=100):
 		request = self.createAccessControl()
 		response = self.client.service.queryById(request, queryString, caseSensitive, sort, offset, maxCount)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	@args.parameter(name='caseSensitive', flag=True)
 	@args.parameter(name='offset', type=int, default=0)
 	@args.parameter(name='maxCount', type=int, default=100)
 	def queryByAttribute(self, attributeID, attributeValue, caseSensitive=False, offset=0, maxCount=100):
 		request = self.createAccessControl()
 		response = self.client.service.queryByAttribute(request, 'step://attribute?id=%s'%attributeID, attributeValue, caseSensitive, offset, maxCount)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getNodeDetails(self, nodeURL):
 		request = self.createAccessControl()
 		return self.client.service.getNodeDetails(request, nodeURL)
 		
 
-	#.............................................................
 	@args.operation
 	def moveNode(self, nodeURL, oldParentURL, newParentURL):
 		request = self.createAccessControl()
 		response = self.client.service.moveNode(request, nodeURL, oldParentURL, newParentURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def setName(self, nodeURL, name=None):
 		request = self.createAccessControl()
 		response = self.client.service.setName(request, nodeURL, name)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getChildren(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getChildren(request, nodeURL)
 		return response
 		
 
-	#.............................................................
 	@args.operation
 	def getGroups(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getGroups(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getUsers(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getUsers(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getUserInfo(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getUserInfo(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getValidChildTypes(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getValidChildTypes(request, nodeURL)
 		return response
 		
 
-	#.............................................................
 	@args.operation
 	def getPath(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getPath(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getReferenceTypes(self):
 		request = self.createAccessControl()
 		response = self.client.service.getReferenceTypes(request)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def createReference(self, ownerURL, targetURL, referenceType):
 		request = self.createAccessControl()
 		response = self.client.service.createReference(request, ownerURL, targetURL, referenceType)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getReferences(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.getReferences(request, nodeURL)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def deleteNode(self, nodeURL):
 		request = self.createAccessControl()
 		response = self.client.service.deleteNode(request, nodeURL)
 		return response
 	
 
-	#.............................................................
 	@args.operation
 	def getTasks(self, nodeURL, workflowID):
 		request = self.createAccessControl()
 		response = self.client.service.getTasks(request, nodeURL, workflowID)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getWorkflowProcesses(self, workflowID):
 		request = self.createAccessControl()
 		response = self.client.service.getWorkflowProcesses(request, workflowID)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getWorkflowProcessDetail(self, processTemplateIdType, processIdType):
 		request = self.createAccessControl()
 		response = self.client.service.getWorkflowProcessDetail(request, processTemplateIdType, processIdType)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def startWorkflow(self, nodeID, workflowID, message):
 		request = self.createAccessControl()
 		response = self.client.service.startWorkflow(request, nodeID, workflowID, message)
 		return response
 
 
-	#.............................................................
 	@args.operation
 	def getLOVValueIDs(self,nodeID):
 		request = self.createAccessControl()
 		response = self.client.service.getLOVValueIDs(request,nodeID)
 		return response
 
-	#.............................................................
 	@args.operation
 	@args.parameter(name='templateID', choices=['Inbound', 'Outbound', 'Importer', 'Exporter', 'StateflowDeadline'])
 	def getBackgoundProcesses(self, templateID):
 		request = self.createAccessControl()
 		response = self.client.service.getBackgroundProcesses(request, templateID)
 		return response
 
 
-#_________________________________________________________________
 def render(node):
 	#sys.stderr.write('%s[%s]\n'%(node,type(node)))
 	if type(node) in [Text]:
 		return '%s'%node
 	if type(node) == list: 
 		return list(map(render, node))
 	if hasattr(node, '__dict__'):
```

### Comparing `STEP.py-2.8/STEP/XML.py` & `STEP.py-2.9/STEP/XML.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from collections import namedtuple, OrderedDict
 from openpyxl import load_workbook
 
 from GoldenChild.xpath import *
 from Perdy.pyxbext import directory
 from Perdy.parser import printXML
 from Spanners.IdentityCache import IdentityCache
-from Spanners.Squirrel import Squirrel
 from Argumental.Argue import Argue
 
 from STEP.XSD import *
 
 args = Argue()
 
 #_________________________________________________________________
```

### Comparing `STEP.py-2.8/STEP/XSD.py` & `STEP.py-2.9/STEP/XSD.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/STEP.py.egg-info/PKG-INFO` & `STEP.py-2.9/STEP.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: STEP.py
-Version: 2.8
+Version: 2.9
 Home-page: https://github.com/eddo888/STEP.py
-Download-URL: https://github.com/eddo888/STEP.py/archive/2.8.tar.gz
+Download-URL: https://github.com/eddo888/STEP.py/archive/2.9.tar.gz
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # STEP.py
```

### Comparing `STEP.py-2.8/bin/step.soap.py` & `STEP.py-2.9/bin/step.soap.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/bin/step2uml.py` & `STEP.py-2.9/bin/step2uml.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/bin/uml2step.py` & `STEP.py-2.9/bin/uml2step.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.8/setup.py` & `STEP.py-2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
 	long_description = input.read()
 
 name='STEP.py'
 user='eddo888'
-version='2.8'
+version='2.9'
 
 setup(
 	name=name,
 	version=version,
 	license='MIT',
 	long_description=long_description,
 	long_description_content_type="text/markdown",
```

### Comparing `STEP.py-2.8/test/test_rest.py` & `STEP.py-2.9/test/test_rest.py`

 * *Files identical despite different names*

