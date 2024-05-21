# Comparing `tmp/asknews-0.6.4-py3-none-any.whl.zip` & `tmp/asknews-0.6.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 23849 bytes, number of entries: 24
+Zip file size: 23891 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4569 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     8720 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
--rw-r--r--  2.0 unx    13803 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
+-rw-r--r--  2.0 unx    13821 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
 -rw-r--r--  2.0 unx    11238 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    16134 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
--rw-r--r--  2.0 unx     4006 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
+-rw-r--r--  2.0 unx     4040 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     4530 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
--rw-r--r--  2.0 unx     1296 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
+-rw-r--r--  2.0 unx     1321 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
--rw-r--r--  2.0 unx     6920 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
+-rw-r--r--  2.0 unx     6970 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1451 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6339 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5396 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.4.dist-info/RECORD
-24 files, 95160 bytes uncompressed, 20815 bytes compressed:  78.1%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.5.dist-info/RECORD
+24 files, 95287 bytes uncompressed, 20857 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.6.4.dist-info/LICENSE
+Filename: asknews-0.6.5.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.6.4.dist-info/METADATA
+Filename: asknews-0.6.5.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.6.4.dist-info/WHEEL
+Filename: asknews-0.6.5.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.6.4.dist-info/RECORD
+Filename: asknews-0.6.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/api/news.py

```diff
@@ -323,15 +323,16 @@
         :type metric: str
         :param sampling: The sampling.
         :type sampling: str
         :return: The source report response.
         :rtype: SourceReportResponse
         """
         response = await self.client.request(
-            endpoint="/v1/stories/sources",
+            method="GET",
+            endpoint="/v1/sources",
             query={
                 "n_points": n_points,
                 "start_timestamp": start_timestamp,
                 "end_timestamp": end_timestamp,
                 "metric": metric,
                 "sampling": sampling,
             },
```

## asknews_sdk/dto/base.py

```diff
@@ -61,16 +61,18 @@
     language: Annotated[str, Field(title="Language")]
     pub_date: Annotated[AwareDatetime, Field(title="Pub Date")]
     summary: Annotated[str, Field(title="Summary")]
     title: Annotated[str, Field(title="Title")]
     sentiment: Annotated[int, Field(title="Sentiment")]
     medoid_distance: Annotated[Optional[float], Field(title="Medoid Distance")] = None
     markdown_citation: Annotated[Optional[str], Field("", title="Markdown Citation")]
-    provocative: Annotated[str, Field(title="A measure of how provocative this story update is.")]
+    provocative: Annotated[
+        str, Field(title="A measure of how provocative this story update is.")
+    ] = "low"
     reporting_voice: Annotated[
         str, Field(title="The reporting voice of the article.")
-    ]
+    ] = "Unknown"
 
 
 class PingResponse(BaseSchema):
     app: Annotated[str, Field(title="App")]
     version: Annotated[str, Field(title="Version")]
```

## asknews_sdk/dto/news.py

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Dict, List, Optional
 
 from pydantic import AwareDatetime, BaseModel, Field, RootModel
 from typing_extensions import Annotated
+from datetime import datetime
 
 from asknews_sdk.dto.base import Article, BaseSchema
 
 
 class SearchResponseDictItem(Article):
     as_string_key: Annotated[str, Field(title="As String Key")]
 
@@ -17,15 +18,15 @@
         Optional[List[SearchResponseDictItem]], Field(None, title="As Dicts")
     ]
     as_string: Annotated[Optional[str], Field(None, title="As String")]
     offset: Annotated[Optional[int], Field(None, title="Offset")]
 
 
 class SourceReportItem(BaseModel):
-    bson_date: Annotated[AwareDatetime, Field(title="Bson Date")]
+    bson_date: Annotated[datetime, Field(title="Bson Date")]
     n_bucket: Annotated[int, Field(title="N Bucket")]
     n_selected: Annotated[int, Field(title="N Selected")]
     bucket_counts: Annotated[Dict[str, int], Field(title="Bucket Counts")]
     selected_counts: Annotated[Dict[str, int], Field(title="Selected Counts")]
     bucket_pct: Annotated[Dict[str, float], Field(title="Bucket Pct")]
     selected_pct: Annotated[Dict[str, float], Field(title="Selected Pct")]
```

## asknews_sdk/dto/stories.py

```diff
@@ -92,21 +92,24 @@
     keywords: Annotated[List[str], Field(title="Keywords")]
     intra_cluster_statistics: IntraClusterStatistics
     silhouette_score: Annotated[Dict[str, Any], Field(title="Silhouette Score")]
     article_ids: Annotated[List[UUID], Field(title="Article Ids")]
     countries: Annotated[Dict[str, int], Field(title="Countries")]
     markdown_citations: Annotated[List[str], Field(title="Markdown Citations")]
     confidence: Annotated[Optional[float], Field(0.0, title="Confidence")]
-    provocative: Annotated[str, Field(title="A measure of how provocative this story update is.")]
+    provocative: Annotated[
+        str, Field(title="A measure of how provocative this story update is.")
+    ] = "low"
     reporting_voice: Annotated[
         str,
         Field(
-            title="An overview of the reporting voice for the articles comprising this story update."
-        )
-    ]
+            title="An overview of the reporting voice for the articles "
+            "comprising this story update."
+        ),
+    ] = "Unknown"
 
 
 class StoryResponse(BaseSchema):
     uuid: Annotated[UUID, Field(title="Uuid")]
     categories: Annotated[List[str], Field(title="Categories")]
     countries: Annotated[Dict[str, int], Field(title="Countries")]
     countries_pct: Annotated[Dict[str, float], Field(title="Countries Pct")]
```

## Comparing `asknews-0.6.4.dist-info/LICENSE` & `asknews-0.6.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.6.4.dist-info/METADATA` & `asknews-0.6.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python SDK for AskNews
 Home-page: https://github.com/emergentmethods/asknews-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.6.4.dist-info/RECORD` & `asknews-0.6.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 asknews_sdk/__init__.py,sha256=TSiiLJIi3INZrbhvrqaXBSAG4MuX5e-Hz7VQstvTOWM,262
 asknews_sdk/api/__init__.py,sha256=1pNfLO6CSeU2bapA-l_oyUQhW2bgavSQUdQcWqjzwno,415
 asknews_sdk/api/analytics.py,sha256=XrH5U5GYXJ5RRTQNVkWYnL-HOD-6yLm6HmNNVWKczxQ,4569
 asknews_sdk/api/base.py,sha256=6w20VMcj9wuMIZLSy_ajbGbMs-cHWbyN7easFpNb8Cg,203
 asknews_sdk/api/chat.py,sha256=7EbwsFKwwmT8Q-7HanDaWrNO8p1bBt565uBHpAH91ao,8720
-asknews_sdk/api/news.py,sha256=BPYIxLL-_ep1x4Bg8iDLIy2kiDDxv_bHblsNTzDtgC0,13803
+asknews_sdk/api/news.py,sha256=iTFsb7nf2d3mwJqE55CPCGFbUGcVgwRzGsrSAOoiNV8,13821
 asknews_sdk/api/stories.py,sha256=ESsisljMV0WCpKGoSWMVDHIbYz4HIX5WPfl7MdWdfeg,11238
 asknews_sdk/client.py,sha256=A7irft6UAXEIA8OTC2-EOfp7HSREiT09WAZ7g53iAVM,16134
 asknews_sdk/dto/__init__.py,sha256=dECq34FclMMDeF8Fq62TTngjillmysK8yht2DTOdqHM,677
-asknews_sdk/dto/base.py,sha256=shI4ozTHIf_zTU3McvhmtESGcwLKDruC_syRm97dSFM,4006
+asknews_sdk/dto/base.py,sha256=XMozNP4mCiTubVWeQNGdPEzutHtc_y18lTrEfuLbkv4,4040
 asknews_sdk/dto/chat.py,sha256=U76lXLM27LXAxGeMFzbBp9rr5Wi5epXr3H6-2jyZhfc,4530
 asknews_sdk/dto/error.py,sha256=fAJutRBtFzSLcJuZYgTDZtv7-T3p6WBGqk3ky3K481c,674
-asknews_sdk/dto/news.py,sha256=aq9H-lU3LOPbTgPXT_j_7HlCHx-y1aNdPuwD9a6icVo,1296
+asknews_sdk/dto/news.py,sha256=JMFLjtqFCNTlA1Mb1SN2AEQBmC3BPml0U6jWH2--6Rg,1321
 asknews_sdk/dto/sentiment.py,sha256=8UhtmYw9jxwcZ1aw9300g-UE0WEIdo5JmgWbPLR-58w,596
-asknews_sdk/dto/stories.py,sha256=AxeMe1oPtHIWRnX_ilbVNVAUoP5gUo6dWXAomAPRErg,6920
+asknews_sdk/dto/stories.py,sha256=f3QLBnKATwOL0dYpNLzr_WXds_YlAMcjQFGx9Hfe_wY,6970
 asknews_sdk/errors.py,sha256=2J6fihHeAL1ny7bdGAoEOazaRibosU3N4IFDBlO9vHk,1451
 asknews_sdk/sdk.py,sha256=EMQeZLuPeAWlV8yLbiefY_C7UuG-1pFDp7GwKJ0rsn4,6339
 asknews_sdk/security.py,sha256=mXVyc4_5KE2j-t5fS3IKewUfmCJZLCPbfcXMJJpLzIk,5396
 asknews_sdk/utils.py,sha256=tM7ga0MZGDA4YheH4dyZ6xxVVexMkzTMz0f6ttP6pwU,1614
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.6.4.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.6.4.dist-info/METADATA,sha256=fLyEibclzxqK7rZRaHKy8EbxtdXCz-iTDhsIqHBmkEY,3233
-asknews-0.6.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.6.4.dist-info/RECORD,,
+asknews-0.6.5.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.6.5.dist-info/METADATA,sha256=JTti8FcWB-7VkwpAmYF52v4gbBAH7q5TnR7KhtDN0Fw,3233
+asknews-0.6.5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.6.5.dist-info/RECORD,,
```

