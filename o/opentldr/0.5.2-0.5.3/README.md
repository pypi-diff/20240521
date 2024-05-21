# Comparing `tmp/opentldr-0.5.2.tar.gz` & `tmp/opentldr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.5.2.tar", last modified: Mon May 20 01:47:41 2024, max compression
+gzip compressed data, was "opentldr-0.5.3.tar", last modified: Tue May 21 13:51:58 2024, max compression
```

## Comparing `opentldr-0.5.2.tar` & `opentldr-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.262182 opentldr-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 01:47:36.000000 opentldr-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:36.000000 opentldr-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-20 01:47:41.262182 opentldr-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-20 01:47:36.000000 opentldr-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 01:47:36.000000 opentldr-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 01:47:41.262182 opentldr-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.254182 opentldr-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.258182 opentldr-0.5.2/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/FileSystemDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    34618 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 01:47:36.000000 opentldr-0.5.2/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.262182 opentldr-0.5.2/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 01:47:41.000000 opentldr-0.5.2/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 01:47:41.262182 opentldr-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-20 01:47:36.000000 opentldr-0.5.2/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.714570 opentldr-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 13:51:49.000000 opentldr-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:49.000000 opentldr-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-21 13:51:58.714570 opentldr-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-21 13:51:49.000000 opentldr-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 13:51:49.000000 opentldr-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:51:58.714570 opentldr-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.706570 opentldr-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.710570 opentldr-0.5.3/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37262 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.714570 opentldr-0.5.3/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.714570 opentldr-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_workflow.py
```

### Comparing `opentldr-0.5.2/LICENSE` & `opentldr-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/PKG-INFO` & `opentldr-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.2
+Version: 0.5.3
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.2/README.md` & `opentldr-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/pyproject.toml` & `opentldr-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.5.2/src/opentldr/AbstractDataRepo.py` & `opentldr-0.5.3/src/opentldr/AbstractDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr/DataRepo.py` & `opentldr-0.5.3/src/opentldr/DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr/DataRepoJson.py` & `opentldr-0.5.3/src/opentldr/DataRepoJson.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr/Domain.py` & `opentldr-0.5.3/src/opentldr/Domain.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr/FileSystemDataRepo.py` & `opentldr-0.5.3/src/opentldr/FileSystemDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr/KnowledgeGraph.py` & `opentldr-0.5.3/src/opentldr/KnowledgeGraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -413,25 +413,34 @@
 
     def update_source(self, node:Source) -> Source:
         '''
         Updates the KG with changes to a Source's properties.
         '''
         return node.save()
     
-    def delete_source(self, node:Source):
+    def delete_source(self, source:Source):
         '''
-        Removes the passed Source node and the edges connected to it.
+        Removes the passed Source node, its content nodes, and the edges connected to it.
         '''
-        self.cypher_query("MATCH (n:Source) WHERE n.uid=$uid DETACH DELETE n", params={"uid": node.uid})
+        for c in self.get_content_by_source(source):
+            self.delete_content(c)
+        return self.delete_source_by_uid(source.uid)
    
+    def delete_source_by_uid(self, uid:str):
+        return self.cypher_query("""
+            MATCH (s:Source) WHERE s.uid=$uid
+            DETACH DELETE s""",
+            params={"uid": uid})
+
     def delete_all_sources(self):
         '''
-        Removes all of the Sources and the edges connected to them.
+        Removes all of the Sources, their content, and the edges connected to them.
         '''
-        self.cypher_query("MATCH (n:Source) DETACH DELETE n")
+        for s in self.get_all_sources():
+            self.delete_source(s)
 
     # -----------------
     # Content Nodes - contain article content and link to their Source
     # -----------------
 
     def add_content(self, source:Source, type:str, url:str, date:datetime.date, title:str, text:str) -> Content:
         content = Content.nodes.get_or_none(url=url)
@@ -457,23 +466,47 @@
         return content
 
     def get_content_by_date(self,date:datetime.date) -> list[Content]:
         content = Content.nodes.get_or_none(date=date)
         return content
 
     def get_content_by_source(self,source:Source) -> list[Content]:
-        return source.get_content()
+        return self.get_content_by_source_uid(source.uid)
+
+    def get_content_by_source_uid(self, uid: str) -> list[Content]:
+        return self.cypher_query("""
+            MATCH (s:Source) WHERE s.uid=$uid
+            MATCH (c:Content)
+            MATCH (c)-[y:IS_FROM]->(s)
+            RETURN c """,
+            "c", params={"uid": uid})
 
     def get_content_by_recommendation(self,recommendation:Recommendation) -> list[Content]:
-        return recommendation.get_content()
+        return recommendation.get_recommends()
 
     def get_all_content(self) -> list[Content]:
         content = Content.nodes
         return content
 
+    def delete_content(self, content:Content):
+        for e in self.get_entities_by_content(content):
+            self.delete_entity(e)
+        return self.delete_content_by_uid(content.uid)
+
+    def delete_content_by_uid(self, uid:str):
+        return self.cypher_query('''
+            MATCH (c:Content) WHERE c.uid=$uid
+            DETACH DELETE c ''',
+            params={"uid": uid})
+
+    def delete_all_content(self):
+        for c in self.get_all_content():
+            self.delete_content(c)
+
+
     # -----------------
     # Active Data / Entity
     # -----------------
 
     def add_entity(self, content:Content, text:str, type:str ) -> Entity:
         entity=Entity(text=text,type=type).save()
         entity.mentioned_in.connect(content)
@@ -493,27 +526,49 @@
     def get_entities_by_content(self,content:Content) -> list[Entity]:
         return self.cypher_query("""
             MATCH (c:Content) WHERE c.uid=$content_uid
             MATCH (e:Entity)
             MATCH (e)-[y:MENTIONED_IN]->(c)
             RETURN e """,
             "e", params={"content_uid": content.uid})
+    
+    def get_entities_by_content_uid(self,uid:str) -> list[Entity]:
+        return self.cypher_query("""
+            MATCH (c:Content) WHERE c.uid=$content_uid
+            MATCH (e:Entity)
+            MATCH (e)-[y:MENTIONED_IN]->(c)
+            RETURN e """,
+            "e", params={"content_uid": uid})
 
     def get_entities_by_request(self,request:Request) -> list[Entity]:
         return self.cypher_query("""
             MATCH (r:Request) WHERE r.uid=$request_uid
             MATCH (e:Entity)
             MATCH (e)-[y:MENTIONED_IN]->(r)
             RETURN e """,
             "e", params={"request_uid": request.uid})
 
     def get_all_entities(self) -> list[Entity]:
         entities = Entity.nodes
         return entities
 
+    def delete_entity(self, node:Entity):
+        return self.delete_entity_by_uid(node.uid)
+
+    def delete_entity_by_uid(self, uid:str):
+        return self.cypher_query("""
+            MATCH (e:Entity) WHERE e.uid=$uid
+            DETACH DELETE e """,
+            params={"uid": uid})
+
+    def delete_all_entities(self):
+        return self.cypher_query("""
+            MATCH (e:Entity)
+            DETACH DELETE e """)
+
     # -----------------
     # Requests API
     # -----------------
 
     # -----------------
     # Users
     # -----------------
@@ -536,14 +591,30 @@
         user = User.nodes.get_or_none(name=name)
         return user
     
     def get_all_users(self) -> list[User]:
         users = User.nodes
         return users
 
+    def delete_user(self, user:User):
+        for r in self.get_requests_by_user(user):
+            self.delete_request(r)
+        return self.delete_user_by_uid(user.uid)
+
+    def delete_user_by_uid(self, uid:str):
+        return self.cypher_query("""
+            MATCH (u:User) WHERE u.uid=$uid
+            DETACH DELETE u""",
+            params={"uid": uid})
+
+    def delete_all_users(self):
+        for u in self.get_all_users():
+            self.delete_user(u)
+
+
     # -----------------
     # Requests
     # -----------------
 
     def add_request(self, title:str, text:str, user:User) -> Request:
         request = Request.nodes.get_or_none(title=title)
         if request is None or request.requested_by.single().uid != user.uid:
@@ -575,36 +646,36 @@
             "q", params={"title": title})
 
     def get_all_requests(self) -> list[Request]:
         requests = Request.nodes
         return requests
 
     def delete_request(self,request:Request):
-        return self.delete_entities_by_request_uid(request.uid)
+        for e in self.get_entities_by_request(request):
+            self.delete_entity(e)
+        return self.delete_request_by_uid(request.uid)
     
-    def delete_request_by_uid(self,request_uid:str):
-        self.delete_entities_by_request_uid(request_uid)
-        return self.cypher_query("""
+    def delete_request_by_uid(self,uid:str):
+        return self.cypher_query('''
             MATCH (r:Request) WHERE r.uid=$uid
-            DETACH DELETE (r) """, params={'uid':request_uid})
-    
-    def delete_entities_by_request_uid(self,request_uid:str):
-        return self.cypher_query("""
-            MATCH (r:Request) WHERE r.uid=$uid
-            MATCH (e:Entity)
-            MATCH (e)-[y:MENTIONED_IN]->(r)
-            DETACH DELETE (e)""", params={'uid':request_uid})
+            DETACH DELETE r ''',
+            params={"uid": uid})
     
+    def delete_all_requests(self):
+        for r in self.get_all_requests():
+            self.delete_request(r)
+   
     def get_requests_by_tldr_entry(self,entry:TldrEntry) -> Request: 
         return self.cypher_query_one("""
             MATCH (e:TldrEntry) WHERE e.uid=$uid
             MATCH (t:Tldr)
             MATCH (q:Request)
-            MATCH (e)<-[x:CONTAINS]-(t)-[y:RESPONSE_TO]->(r)
+            MATCH (e)<-[x:CONTAINS]-(t)-[y:RESPONSE_TO]->(q)
             RETURN q ""","q", params={'uid': entry.uid})
+    
 
     # -----------------
     # Workflow Products API
     # -----------------
 
     # -----------------
     # Recommendations
@@ -652,15 +723,15 @@
     def get_all_recommendations(self) -> list[Recommendation]:
         recommendations = Recommendation.nodes
         return recommendations
 
     def delete_recommendation(self, recommendation:Recommendation):
         recommendation.delete()
     
-    def delete_all_recommendations(self):
+    def delete_all_recommendations(self): 
         self.cypher_query("MATCH (r:Recommendation) DETACH DELETE (r)")
          
     # -----------------
     # Summaries
     # -----------------
 
     def add_summary(self, text:str, content:Content, recommendation:Recommendation=None) -> Summary:
@@ -706,14 +777,20 @@
             RETURN s """,
             "s", params={"recommendation_id": recommendation.uid})
 
     def get_all_summary(self) -> list[Summary]:
         summary = Summary.nodes
         return summary
     
+    def delete_summary(self, summary:Summary):
+        summary.delete()
+    
+    def delete_all_summaries(self): 
+        self.cypher_query("MATCH (s:Summary) DETACH DELETE (s)")
+    
     # -----------------
     # Tldr
     # -----------------
 
     def add_tldr(self, request: Request, date: datetime.date) -> Tldr:
         tldr = self.get_tldr(request, date)
         if tldr is None:
@@ -887,9 +964,19 @@
                 "content_id": content.uid,
                 "request_id": request.uid})
 
     def get_all_evalkeys(self) -> list[EvalKey]:
         evalkeys = EvalKey.nodes
         return evalkeys
 
+    def delete_evalkey(self, evalKey:EvalKey):
+        return self.delete_evalkey_by_uid(evalKey.uid)
+
+    def delete_evalkey_by_uid(self, uid:str):
+        return self.cypher_query("""
+            MATCH (k:EvalKey) WHERE k.uid=$uid
+            DETACH DELETE k""",
+            params={"uid": uid})
+
     def delete_all_evalkeys(self):
-        self.cypher_query("MATCH (r:EvalKey) DETACH DELETE (r)")
+        for k in self.get_all_evalkeys():
+            self.delete_evalkey(k)
```

### Comparing `opentldr-0.5.2/src/opentldr/S3DataRepo.py` & `opentldr-0.5.3/src/opentldr/S3DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr/Workflow.py` & `opentldr-0.5.3/src/opentldr/Workflow.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.5.3/src/opentldr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.2
+Version: 0.5.3
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.2/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.5.3/src/opentldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/tests/test_knowledgegraph.py` & `opentldr-0.5.3/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.2/tests/test_workflow.py` & `opentldr-0.5.3/tests/test_workflow.py`

 * *Files identical despite different names*

