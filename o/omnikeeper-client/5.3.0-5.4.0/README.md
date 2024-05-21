# Comparing `tmp/omnikeeper_client-5.3.0-py3-none-any.whl.zip` & `tmp/omnikeeper_client-5.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 21084 bytes, number of entries: 16
--rw-r--r--  2.0 unx     1265 b- defN 24-May-08 06:45 omnikeeper_client/__init__.py
+Zip file size: 22626 bytes, number of entries: 17
+-rw-r--r--  2.0 unx     1344 b- defN 24-May-21 09:11 omnikeeper_client/__init__.py
 -rw-r--r--  2.0 unx     1984 b- defN 24-Mar-14 11:13 omnikeeper_client/apiclient.py
 -rw-r--r--  2.0 unx     5040 b- defN 24-Feb-06 12:05 omnikeeper_client/ci.py
 -rw-r--r--  2.0 unx     3796 b- defN 24-Apr-04 07:13 omnikeeper_client/dataframes.py
+-rw-r--r--  2.0 unx     1080 b- defN 24-May-21 09:14 omnikeeper_client/issues.py
 -rw-r--r--  2.0 unx     3232 b- defN 24-Feb-06 12:05 omnikeeper_client/layer.py
 -rw-r--r--  2.0 unx     2765 b- defN 24-Apr-05 10:02 omnikeeper_client/pyd.py
 -rw-r--r--  2.0 unx    10639 b- defN 24-Apr-04 07:14 omnikeeper_client/simple_traits.py
 -rw-r--r--  2.0 unx     4574 b- defN 24-Apr-04 07:13 omnikeeper_client/trait.py
--rw-r--r--  2.0 unx    21202 b- defN 24-May-16 10:22 omnikeeper_client/traitentities.py
+-rw-r--r--  2.0 unx    24876 b- defN 24-May-21 09:14 omnikeeper_client/traitentities.py
 -rw-r--r--  2.0 unx     5262 b- defN 24-Feb-06 12:05 omnikeeper_client/typing.py
 -rw-r--r--  2.0 unx      917 b- defN 24-Feb-06 12:05 omnikeeper_client/util.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      572 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1373 b- defN 24-May-16 10:25 omnikeeper_client-5.3.0.dist-info/RECORD
-16 files, 74088 bytes uncompressed, 18810 bytes compressed:  74.6%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-21 09:15 omnikeeper_client-5.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      572 b- defN 24-May-21 09:15 omnikeeper_client-5.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 09:15 omnikeeper_client-5.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-21 09:15 omnikeeper_client-5.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1457 b- defN 24-May-21 09:15 omnikeeper_client-5.4.0.dist-info/RECORD
+17 files, 79005 bytes uncompressed, 20222 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: omnikeeper_client/ci.py
 Comment: 
 
 Filename: omnikeeper_client/dataframes.py
 Comment: 
 
+Filename: omnikeeper_client/issues.py
+Comment: 
+
 Filename: omnikeeper_client/layer.py
 Comment: 
 
 Filename: omnikeeper_client/pyd.py
 Comment: 
 
 Filename: omnikeeper_client/simple_traits.py
@@ -27,23 +30,23 @@
 
 Filename: omnikeeper_client/typing.py
 Comment: 
 
 Filename: omnikeeper_client/util.py
 Comment: 
 
-Filename: omnikeeper_client-5.3.0.dist-info/LICENSE
+Filename: omnikeeper_client-5.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: omnikeeper_client-5.3.0.dist-info/METADATA
+Filename: omnikeeper_client-5.4.0.dist-info/METADATA
 Comment: 
 
-Filename: omnikeeper_client-5.3.0.dist-info/WHEEL
+Filename: omnikeeper_client-5.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: omnikeeper_client-5.3.0.dist-info/top_level.txt
+Filename: omnikeeper_client-5.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: omnikeeper_client-5.3.0.dist-info/RECORD
+Filename: omnikeeper_client-5.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnikeeper_client/__init__.py

```diff
@@ -44,14 +44,16 @@
     get_latest_trait_change,
     get_all_traitentities,
     get_all_traitentity_relations,
     set_traitentity_relations,
     bulk_replace_trait_entities,
     bulk_replace_trait_entities_by_filter,
     bulk_replace_traitentity_relations,
+    OKEntityList,
+    OKRelationList
 )
 
 from .dataframes import (
     get_all_traitentities_dataframe,
     bulk_replace_trait_entities_dataframe,
     bulk_replace_trait_entities_by_filter_dataframe,
 )
@@ -59,8 +61,12 @@
 from .pyd import (
     SerializableUUID,
     AttributeName,
     AttributeOptional,
     TypeHint,
     get_all_traitentities_pydantic,
     bulk_replace_trait_entities_pydantic
+)
+
+from .issues import (
+    OKIssueList,
 )
```

## omnikeeper_client/traitentities.py

```diff
@@ -1,15 +1,15 @@
 from gql import gql
 import graphql
 from graphql import GraphQLType
 from gql.dsl import DSLQuery, DSLVariableDefinitions, DSLSchema, dsl_gql
 from dateutil import parser
 import datetime
 import omnikeeper_client as okc
-from typing import List, Dict, Any
+from typing import List, Dict, Any, Self
 import uuid
 from typing import (
     List,
 )
 
 
 def _is_relation_field(type: GraphQLType) -> bool:
@@ -593,7 +593,88 @@
     Returns
     -------
     bool 
         True if the update is successful, False otherwise
     """
     result = _bulk_replace_trait_entities(ok_api_client, trait_id, input, write_layer, read_layers)
     return result
+
+class OKEntityList:
+    def __init__(self, ok_list: List[Dict[str, Any]]):
+        self.ok_list = ok_list
+        self.ciid_lookup_table = {str(v['ciid']): index for index, v in enumerate(ok_list)}
+
+    def update_or_add_via_ciid(self, item: Dict[str, Any], ciid: str) -> int:
+        item['__keep'] = True
+        index = self.ciid_lookup_table.get(ciid, None)
+        if index is not None:
+            # ci exists in the data already -> update
+            self.ok_list[index].update(item)
+            return index
+        else:
+            # ci does not exist yet -> add
+            item['ciid'] = ciid
+            self.ok_list.append(item)
+            self.ciid_lookup_table[ciid] = len(self.ok_list) - 1
+            return index
+    
+    def get_final_list(self) -> List[Dict[str, Any]]:
+        return [{k: v for k, v in d.items() if k != '__keep'} for d in self.ok_list if '__keep' in d]
+
+class OKRelationList:
+    def __init__(self, ok_list: List[Dict[str, Any]]):
+        self.ok_list = ok_list
+        self.lookup_table = {str(v['base_ciid']): index for index, v in enumerate(ok_list)}
+
+    def add_or_update(self, base_ciid: str, related_ciids: List[str], merge_strategy_related_ciids: str = 'replace'):
+        related_ciids_non_duplicates = list(set(related_ciids)) # NOTE: list(set(...)) ensures uniqueness
+        item = { 'base_ciid': base_ciid, 'related_ciids': related_ciids_non_duplicates, '__keep': True}
+        index = self.lookup_table.get(base_ciid, None)
+        if index is not None:
+            # give caller the choice on how to merge related_ciids
+            if merge_strategy_related_ciids == 'replace':
+                # simply replace existing related_ciids dictionary with new dictionary
+                self.ok_list[index].update(item)
+            elif merge_strategy_related_ciids == 'merge':
+                exsting_related_ciids = self.ok_list[index]['related_ciids']
+                new_related_ciids = item['related_ciids']
+                final_related_ciids = list(set(exsting_related_ciids + new_related_ciids)) # NOTE: list(set(...)) ensures uniqueness
+                item['related_ciids'] = final_related_ciids
+                self.ok_list[index].update(item)
+                pass
+            else:
+                raise Exception(f"Unknown value for merge_strategy_related_ciids: {merge_strategy_related_ciids}")
+        else:
+            self.ok_list.append(item)
+            self.lookup_table[base_ciid] = len(self.ok_list) - 1
+
+    def build_inverse_list(self) -> Self:
+        tmp = dict()
+        for d in self.ok_list:
+            for r in d['related_ciids']:
+                existing = tmp.get(r, None)
+                if existing is None:
+                    tmp[r] = [d['base_ciid']]
+                else:
+                    existing.append(d['base_ciid'])
+        
+        final_list = [{'base_ciid': k, 'related_ciids': v} for k, v in tmp.items()]
+        return OKRelationList(final_list)
+
+    def get_related_ciids(self, base_ciid: str, default = []) -> List[str]:
+        index = self.lookup_table.get(base_ciid, None)
+        if index is None:
+            return default
+        return self.ok_list[index]["related_ciids"]
+    
+    def get_relevant_ciids(self) -> List[str]:
+        return [d['base_ciid'] for d in self.ok_list]
+    
+    def get_final_list(self) -> List[Dict[str, Any]]:
+        tmp = [{k: v for k, v in d.items() if k != '__keep'} for d in self.ok_list if '__keep' in d]
+
+        # HACK, TODO: rework client library to not have to rewrite keys
+        for d in tmp:
+            d['baseCIID'] = d.pop('base_ciid')
+            d['relatedCIIDs'] = d.pop('related_ciids')
+
+        return tmp
```

## Comparing `omnikeeper_client-5.3.0.dist-info/LICENSE` & `omnikeeper_client-5.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `omnikeeper_client-5.3.0.dist-info/METADATA` & `omnikeeper_client-5.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnikeeper-client
-Version: 5.3.0
+Version: 5.4.0
 Summary: Python library containing helper functions for implementing omnikeeper clients
 Home-page: UNKNOWN
 Author: Maximilian Csuk
 License: Apache 2.0
 Platform: UNKNOWN
 License-File: LICENSE
 Requires-Dist: appengine-python-standard ~=1.1
```

## Comparing `omnikeeper_client-5.3.0.dist-info/RECORD` & `omnikeeper_client-5.4.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-omnikeeper_client/__init__.py,sha256=JAZEDxX9hU1cOoXnz9yarIJMroHteueGYOIVZHVuKkw,1265
+omnikeeper_client/__init__.py,sha256=OG6WLJCy_eYyqi8a3cJPmOCR8-sW_0FBUFq-gtp-ZVw,1344
 omnikeeper_client/apiclient.py,sha256=X2NMaqM23pGLmDFDV2ueJnJzGdUEjz1WLrVvlWkYaGA,1984
 omnikeeper_client/ci.py,sha256=hXYsfDbMNvIy32CbStar1ade3ifH6VTL4VjxF9ICy1I,5040
 omnikeeper_client/dataframes.py,sha256=1G-k_IhPejA1UpR0_JYzLSgEBkVymD24gWNpWC5aHC0,3796
+omnikeeper_client/issues.py,sha256=APnn2Li0spekUj3ygZe2bnYmo2x9fr_eybhl6jNYueI,1080
 omnikeeper_client/layer.py,sha256=To0INBUjgOiIuwwcMRo3wdT1mIbwcm-cVjJ4Lqh0SwI,3232
 omnikeeper_client/pyd.py,sha256=8AQVtMzxz2tkDP8z-0MCLA0meLOxmtEMBHQxI_f6Uwk,2765
 omnikeeper_client/simple_traits.py,sha256=yduQQKL93hUOBe6NQBBHchrtC8qr-kl8BU29b5cnbls,10639
 omnikeeper_client/trait.py,sha256=mPn46R2Aj5x1F6us_Z5VQ2iXf2pYQW9osSgItcQ8L5Q,4574
-omnikeeper_client/traitentities.py,sha256=avlwArYgTl_pe26lCmmC8cxU1GXWqEE7bvwD8n5xExM,21202
+omnikeeper_client/traitentities.py,sha256=ecjnzHKSzLf8GFNOFC3n4XN6riv7tX5FNIJ0L0ZBTbE,24876
 omnikeeper_client/typing.py,sha256=dLzATV6Ez3VhPMEGdnsLKkZNS1aFgfURYbRKHiAGEFE,5262
 omnikeeper_client/util.py,sha256=Htf_rrlvd6usJ-ONWOU1l0Bz_CnisjQrlRzNODppiZg,917
-omnikeeper_client-5.3.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-omnikeeper_client-5.3.0.dist-info/METADATA,sha256=Alum_tThOsen-sJbejPRFZe1bbJthiym0oF2MfrYUrw,572
-omnikeeper_client-5.3.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-omnikeeper_client-5.3.0.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
-omnikeeper_client-5.3.0.dist-info/RECORD,,
+omnikeeper_client-5.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+omnikeeper_client-5.4.0.dist-info/METADATA,sha256=Dw7GpDifMFjB2Nnet7fmZwfhqlXEW-5Rqda66urpruo,572
+omnikeeper_client-5.4.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+omnikeeper_client-5.4.0.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
+omnikeeper_client-5.4.0.dist-info/RECORD,,
```

