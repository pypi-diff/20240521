# Comparing `tmp/asknews-0.6.5-py3-none-any.whl.zip` & `tmp/asknews-0.6.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 23891 bytes, number of entries: 24
+Zip file size: 23882 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 asknews_sdk/__init__.py
 -rw-r--r--  2.0 unx      415 b- defN 80-Jan-01 00:00 asknews_sdk/api/__init__.py
 -rw-r--r--  2.0 unx     4569 b- defN 80-Jan-01 00:00 asknews_sdk/api/analytics.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 asknews_sdk/api/base.py
 -rw-r--r--  2.0 unx     8720 b- defN 80-Jan-01 00:00 asknews_sdk/api/chat.py
 -rw-r--r--  2.0 unx    13821 b- defN 80-Jan-01 00:00 asknews_sdk/api/news.py
 -rw-r--r--  2.0 unx    11238 b- defN 80-Jan-01 00:00 asknews_sdk/api/stories.py
 -rw-r--r--  2.0 unx    16134 b- defN 80-Jan-01 00:00 asknews_sdk/client.py
 -rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 asknews_sdk/dto/__init__.py
 -rw-r--r--  2.0 unx     4040 b- defN 80-Jan-01 00:00 asknews_sdk/dto/base.py
 -rw-r--r--  2.0 unx     4530 b- defN 80-Jan-01 00:00 asknews_sdk/dto/chat.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 asknews_sdk/dto/error.py
--rw-r--r--  2.0 unx     1321 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
+-rw-r--r--  2.0 unx     1306 b- defN 80-Jan-01 00:00 asknews_sdk/dto/news.py
 -rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 asknews_sdk/dto/sentiment.py
 -rw-r--r--  2.0 unx     6970 b- defN 80-Jan-01 00:00 asknews_sdk/dto/stories.py
 -rw-r--r--  2.0 unx     1451 b- defN 80-Jan-01 00:00 asknews_sdk/errors.py
 -rw-r--r--  2.0 unx     6339 b- defN 80-Jan-01 00:00 asknews_sdk/sdk.py
 -rw-r--r--  2.0 unx     5396 b- defN 80-Jan-01 00:00 asknews_sdk/security.py
 -rw-r--r--  2.0 unx     1614 b- defN 80-Jan-01 00:00 asknews_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 asknews_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.5.dist-info/RECORD
-24 files, 95287 bytes uncompressed, 20857 bytes compressed:  78.1%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 asknews-0.6.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3233 b- defN 80-Jan-01 00:00 asknews-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 asknews-0.6.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1901 b- defN 16-Jan-01 00:00 asknews-0.6.6.dist-info/RECORD
+24 files, 95272 bytes uncompressed, 20848 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -54,20 +54,20 @@
 
 Filename: asknews_sdk/utils.py
 Comment: 
 
 Filename: asknews_sdk/version.py
 Comment: 
 
-Filename: asknews-0.6.5.dist-info/LICENSE
+Filename: asknews-0.6.6.dist-info/LICENSE
 Comment: 
 
-Filename: asknews-0.6.5.dist-info/METADATA
+Filename: asknews-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: asknews-0.6.5.dist-info/WHEEL
+Filename: asknews-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: asknews-0.6.5.dist-info/RECORD
+Filename: asknews-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asknews_sdk/dto/news.py

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Dict, List, Optional
 
-from pydantic import AwareDatetime, BaseModel, Field, RootModel
+from pydantic import BaseModel, Field, RootModel
 from typing_extensions import Annotated
 from datetime import datetime
 
 from asknews_sdk.dto.base import Article, BaseSchema
 
 
 class SearchResponseDictItem(Article):
```

## Comparing `asknews-0.6.5.dist-info/LICENSE` & `asknews-0.6.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `asknews-0.6.5.dist-info/METADATA` & `asknews-0.6.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asknews
-Version: 0.6.5
+Version: 0.6.6
 Summary: Python SDK for AskNews
 Home-page: https://github.com/emergentmethods/asknews-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `asknews-0.6.5.dist-info/RECORD` & `asknews-0.6.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 asknews_sdk/api/news.py,sha256=iTFsb7nf2d3mwJqE55CPCGFbUGcVgwRzGsrSAOoiNV8,13821
 asknews_sdk/api/stories.py,sha256=ESsisljMV0WCpKGoSWMVDHIbYz4HIX5WPfl7MdWdfeg,11238
 asknews_sdk/client.py,sha256=A7irft6UAXEIA8OTC2-EOfp7HSREiT09WAZ7g53iAVM,16134
 asknews_sdk/dto/__init__.py,sha256=dECq34FclMMDeF8Fq62TTngjillmysK8yht2DTOdqHM,677
 asknews_sdk/dto/base.py,sha256=XMozNP4mCiTubVWeQNGdPEzutHtc_y18lTrEfuLbkv4,4040
 asknews_sdk/dto/chat.py,sha256=U76lXLM27LXAxGeMFzbBp9rr5Wi5epXr3H6-2jyZhfc,4530
 asknews_sdk/dto/error.py,sha256=fAJutRBtFzSLcJuZYgTDZtv7-T3p6WBGqk3ky3K481c,674
-asknews_sdk/dto/news.py,sha256=JMFLjtqFCNTlA1Mb1SN2AEQBmC3BPml0U6jWH2--6Rg,1321
+asknews_sdk/dto/news.py,sha256=NheGNwrVXQFkvQ8XuaPmno5x4Fhym0YLtG_IzLgIULQ,1306
 asknews_sdk/dto/sentiment.py,sha256=8UhtmYw9jxwcZ1aw9300g-UE0WEIdo5JmgWbPLR-58w,596
 asknews_sdk/dto/stories.py,sha256=f3QLBnKATwOL0dYpNLzr_WXds_YlAMcjQFGx9Hfe_wY,6970
 asknews_sdk/errors.py,sha256=2J6fihHeAL1ny7bdGAoEOazaRibosU3N4IFDBlO9vHk,1451
 asknews_sdk/sdk.py,sha256=EMQeZLuPeAWlV8yLbiefY_C7UuG-1pFDp7GwKJ0rsn4,6339
 asknews_sdk/security.py,sha256=mXVyc4_5KE2j-t5fS3IKewUfmCJZLCPbfcXMJJpLzIk,5396
 asknews_sdk/utils.py,sha256=tM7ga0MZGDA4YheH4dyZ6xxVVexMkzTMz0f6ttP6pwU,1614
 asknews_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-asknews-0.6.5.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-asknews-0.6.5.dist-info/METADATA,sha256=JTti8FcWB-7VkwpAmYF52v4gbBAH7q5TnR7KhtDN0Fw,3233
-asknews-0.6.5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-asknews-0.6.5.dist-info/RECORD,,
+asknews-0.6.6.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+asknews-0.6.6.dist-info/METADATA,sha256=dQiDhBULqldu60GZU94EFdbWFWr7Ziz9bhD9a9rkeEk,3233
+asknews-0.6.6.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+asknews-0.6.6.dist-info/RECORD,,
```

