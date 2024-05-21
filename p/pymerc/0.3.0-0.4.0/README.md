# Comparing `tmp/pymerc-0.3.0.tar.gz` & `tmp/pymerc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymerc-0.3.0.tar", max compression
+gzip compressed data, was "pymerc-0.4.0.tar", max compression
```

## Comparing `pymerc-0.3.0.tar` & `pymerc-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
--rw-r--r--   0        0        0     1096 2024-05-17 15:32:57.829331 pymerc-0.3.0/README.md
--rw-r--r--   0        0        0      381 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/base.py
--rw-r--r--   0        0        0      571 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/map.py
--rw-r--r--   0        0        0      264 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/common.py
--rw-r--r--   0        0        0      594 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/map.py
--rw-r--r--   0        0        0     2003 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/player.py
--rw-r--r--   0        0        0     2466 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/static.py
--rw-r--r--   0        0        0     3285 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/towns.py
--rw-r--r--   0        0        0      481 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/player.py
--rw-r--r--   0        0        0     2204 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/static.py
--rw-r--r--   0        0        0     1828 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/towns.py
--rw-r--r--   0        0        0     1282 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/client.py
--rw-r--r--   0        0        0     1585 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/util/towns.py
--rw-r--r--   0        0        0      761 2024-05-17 15:32:57.829331 pymerc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 pymerc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-21 04:48:12.666119 pymerc-0.4.0/README.md
+-rw-r--r--   0        0        0      381 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/base.py
+-rw-r--r--   0        0        0     1225 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/buildings.py
+-rw-r--r--   0        0        0      640 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/businesses.py
+-rw-r--r--   0        0        0      571 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/map.py
+-rw-r--r--   0        0        0     1279 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/buildings.py
+-rw-r--r--   0        0        0      855 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/businesses.py
+-rw-r--r--   0        0        0    18770 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/common.py
+-rw-r--r--   0        0        0      593 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/map.py
+-rw-r--r--   0        0        0     1396 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/player.py
+-rw-r--r--   0        0        0     2692 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/static.py
+-rw-r--r--   0        0        0     3131 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/towns.py
+-rw-r--r--   0        0        0      483 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/player.py
+-rw-r--r--   0        0        0     2210 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/static.py
+-rw-r--r--   0        0        0     1830 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/towns.py
+-rw-r--r--   0        0        0     5022 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/client.py
+-rw-r--r--   0        0        0      107 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/exceptions.py
+-rw-r--r--   0        0        0     2416 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/game/building.py
+-rw-r--r--   0        0        0     2020 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/game/player.py
+-rw-r--r--   0        0        0     3607 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/game/town.py
+-rw-r--r--   0        0        0      599 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/util/data.py
+-rw-r--r--   0        0        0     1602 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/util/towns.py
+-rw-r--r--   0        0        0      777 2024-05-21 04:48:12.666119 pymerc-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 pymerc-0.4.0/PKG-INFO
```

### Comparing `pymerc-0.3.0/README.md` & `pymerc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymerc-0.3.0/pymerc/api/map.py` & `pymerc-0.4.0/pymerc/api/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.3.0/pymerc/api/models/map.py` & `pymerc-0.4.0/pymerc/api/models/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,7 @@
         size (int): The size of the region.
     """
 
     id: int
     name: str
     center: Center
     size: int
-
```

### Comparing `pymerc-0.3.0/pymerc/api/models/static.py` & `pymerc-0.4.0/pymerc/api/models/static.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,112 @@
 from __future__ import annotations
 
 from typing import Optional
 from pydantic import BaseModel, Field
 
+from pymerc.api.models import common
+
 
 class Building(BaseModel):
     """Represents a building in the game."""
-    type: str
+
+    type: common.BuildingType
     supports_boost: Optional[bool] = False
     requires: BuildingRequirements
     construction: Optional[BuildingConstruction] = None
     upgrades: Optional[list[BuildingUpgrade]] = []
 
 
 class BuildingRequirements(BaseModel):
     """Represents the requirements for a building."""
+
     fertility: Optional[TileRequirement] = None
     forest: Optional[TileRequirement] = None
-    climate: Optional[str] = None
+    climate: Optional[common.Climate] = None
 
 
 class TileRequirement(BaseModel):
     """Represents a requirement for a tile."""
+
     min: Optional[int] = None
     max: Optional[int] = None
 
 
 class BuildingRequirement(BaseModel):
     """Represents a requirement for a building."""
+
     center: Optional[bool] = False
-    climate: Optional[str] = None
+    climate: Optional[common.Climate] = None
     min: Optional[int] = None
-    resource: Optional[str] = None
+    resource: Optional[common.Item] = None
+
 
 class BuildingConstruction(BaseModel):
     """Represents the construction requirements for a building."""
+
     range: Optional[int] = None
     size: Optional[int] = None
     discount: Optional[int] = None
     time: int
-    materials: dict[str, int]
+    materials: dict[common.Item, int]
+
 
 class BuildingUpgrade(BaseModel):
     """Represents an upgrade for a building."""
-    type: str
+
+    type: common.BuildingUpgradeType
     construction: BuildingConstruction
 
+
 class Recipe(BaseModel):
     """Represents a recipe for a product in the game."""
-    name: str
+
+    name: common.Recipe
     tier: int
-    building: str
+    building: common.BuildingType
     size: int
-    product_class: Optional[str] = Field(alias='class', default=None)
+    product_class: Optional[common.Skill] = Field(alias="class", default=None)
     points: Optional[float] = None
     inputs: Optional[list[Ingredient]] = []
     outputs: Optional[list[Ingredient]] = []
 
 
 class Ingredient(BaseModel):
     """Represents an ingredient in a recipe."""
-    product: str
+
+    product: common.Item
     amount: float
 
+
 class Transport(BaseModel):
     """Represents a transport in the game."""
-    type: str
+
+    type: common.Transport
     category: int
     tier: int
     capacity: int
     speed: int
     journey_duration: int
     effective_days: int
-    operating_costs: dict[str, float]
+    operating_costs: dict[common.Item, float]
     catches: Optional[str] = None
     fishing_range: Optional[int] = None
 
+
 class Item(BaseModel):
     """Represents an item in the game."""
-    name: str
-    type: str
+
+    name: common.Item
+    type: common.ItemType
     unit: str
     weight: Optional[float] = None
     tier: int
-    classes: Optional[list[str]] = []
+    classes: Optional[list[common.Skill]] = []
     price: ItemPrice
 
+
 class ItemPrice(BaseModel):
     """Represents the price of an item in the game."""
+
     low: float
     typical: float
-    high: float
+    high: float
```

### Comparing `pymerc-0.3.0/pymerc/api/models/towns.py` & `pymerc-0.4.0/pymerc/api/models/towns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,113 +1,115 @@
 from __future__ import annotations
 
 from pydantic import BaseModel, Field
 from typing import Optional
 
-from pymerc.api.models.common import Location
+from pymerc.api.models import common
+
 
 class Town(BaseModel):
     """Represents a town in the game."""
 
     id: str
     name: str
-    location: Location
+    location: common.Location
     region: int
     capital: bool
 
 
 class TownData(BaseModel):
     """Represents the data for a town in the game."""
+
     id: str
     name: str
-    location: Location
+    location: common.Location
     region: int
     center_ids: list[int]
     domain: dict[str, TownDomain]
     household_ids: list[str]
     commoners: TownCommoners
     government: TownGovernment
     church: TownChurch
     navigation_zones: dict[int, int]
     culture: TownCulture
 
 
 class TownDomain(BaseModel):
     """Represents a domain in a town."""
+
     owner_id: Optional[str] = None
     structure: Optional[TownDomainStructure] = None
     ask_price: Optional[str] = None
 
 
 class TownDomainStructure(BaseModel):
     """Represents a structure in a town domain."""
+
     id: str
-    type: str
+    type: common.BuildingType
     tags: Optional[list[str]] = []
 
 
-class TownStrucure(BaseModel):
-    """Represents a structure in a town."""
-    id: int
-    type: str
-    size: Optional[int] = 0
-    owner_id: str
-    location: Location
-    land: Optional[list[Location]] = []
-
-
 class TownCommoners(BaseModel):
     """Represents the commoners in a town."""
+
     account_id: str
     count: int
     migration: float
     sustenance: list[TownDemandCategory]
 
 
 class TownDemandCategory(BaseModel):
     """Represents a category of demands in a town."""
+
     name: str
     products: list[TownDemand]
 
 
 class TownDemand(BaseModel):
     """Represents a demand in a town."""
-    product: str
+
+    product: common.Item
     bonus: int
     desire: int
     request: int
     result: int
 
 
 class TownGovernment(BaseModel):
     """Represents the government in a town."""
+
     account_id: str
     demands: list[TownDemand]
     taxes_collected: TownGovernmentTaxes
 
 
 class TownGovernmentTaxes(BaseModel):
     """Represents the taxes collected by the government in a town."""
+
     land_tax: float
     structure_tax: float
     ferry_fees: float
 
 
 class TownChurch(BaseModel):
     """Represents the church in a town."""
+
     project_ids: Optional[list[str]] = []
 
 
 class TownCulture(BaseModel):
     """Represents the culture in a town."""
+
     special_market_pressure: Optional[dict[int, float]] = {}
 
 
 class TownMarket(BaseModel):
     """Represents the market in a town."""
+
     markets: dict[str, TownMarketItem]
     ts: int = Field(alias="_ts")
 
 
 class TownMarketItem(BaseModel):
     """Represents the market data for a single item in a town."""
 
@@ -123,20 +125,20 @@
     ask_volume_10: Optional[int] = 0
 
 
 class TownMarketItemDetails(BaseModel):
     """Represents the market data for a single item in a town."""
 
     id: int
-    product: str
-    asset: str
+    product: common.Item
+    asset: common.Item
     currency: str
     bids: list[ItemOrder]
     asks: list[ItemOrder]
     data: TownMarketItem
 
 
 class ItemOrder(BaseModel):
     """Represents an order for an item in the market."""
 
     volume: int
-    price: float
+    price: float
```

### Comparing `pymerc-0.3.0/pymerc/api/static.py` & `pymerc-0.4.0/pymerc/api/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from typing import Any
 
 from pydantic import TypeAdapter
 
 from pymerc.api.base import BaseAPI
 from pymerc.api.models import static
 
-BASE_URL="https://play.mercatorio.io/static/js/"
-ROOT_URL="https://play.mercatorio.io/"
+BASE_URL = "https://play.mercatorio.io/static/js/"
+ROOT_URL = "https://play.mercatorio.io/"
+
 
 class StaticAPI(BaseAPI):
     """A class for interacting with the static data from the game."""
 
     async def get_buildings(self) -> list[static.Building]:
         """Get the buildings from the game.
 
@@ -65,8 +66,8 @@
         """
         response = await self.client.get(ROOT_URL)
         pattern = r"src=\"\/static\/js\/(.*?)\">"
         filename = re.search(pattern, response.text).group(1)
 
         response = await self.client.get(BASE_URL + filename)
         pattern = r"JSON\.parse\('(.*?)'\)"
-        return json.loads(re.search(pattern, response.text).group(1).replace("\\", ""))
+        return json.loads(re.search(pattern, response.text).group(1).replace("\\", ""))
```

### Comparing `pymerc-0.3.0/pymerc/api/towns.py` & `pymerc-0.4.0/pymerc/api/towns.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pydantic import TypeAdapter
 
 from pymerc.api.base import BaseAPI
 from pymerc.api.models import towns
 
 BASE_URL = "https://play.mercatorio.io/api/towns"
 
+
 class TownsAPI(BaseAPI):
     """A class for interacting with the towns API endpoint."""
 
     async def init_cache(self):
         pass
 
     async def get_all(self) -> list[towns.Town]:
@@ -52,8 +53,8 @@
             town_id (int): The ID of the town
             item (str): The item to get the overview for
 
         Returns:
             TownMarketItemDetails: The market overview for the town
         """
         response = await self.client.get(f"{BASE_URL}/{town_id}/markets/{item}")
-        return towns.TownMarketItemDetails.model_validate(response.json())
+        return towns.TownMarketItemDetails.model_validate(response.json())
```

### Comparing `pymerc-0.3.0/pymerc/util/towns.py` & `pymerc-0.4.0/pymerc/util/towns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 
 from pymerc.api.models.towns import TownData
 from pymerc.client import Client
 
+
 def calculate_town_satisfaction(data: TownData):
     """Calculate the satisfaction of a town.
 
     Args:
         data (TownData): The data for the town
 
     Returns:
@@ -14,14 +15,15 @@
     """
     demands = sum([category.products for category in data.commoners.sustenance], [])
     desire_total = sum(demand.desire for demand in demands)
     result_total = sum(demand.result for demand in demands)
 
     return math.ceil((result_total / desire_total) * 100)
 
+
 async def get_towns_market_data(client: Client):
     """Get the market data for all towns.
 
     Args:
         client (Client): The client to use for the request
 
     Returns:
@@ -40,15 +42,18 @@
 
     Args:
         data (TownData): The data for the town
 
     Returns:
         int: The sum of the structures in the town
     """
-    return len([domain for domain in data.domain.values() if domain.structure is not None])
+    return len(
+        [domain for domain in data.domain.values() if domain.structure is not None]
+    )
+
 
 def sum_town_taxes(data: TownData):
     """Sum the taxes collected by a town.
 
     Args:
         data (TownData): The data for the town
```

### Comparing `pymerc-0.3.0/pyproject.toml` & `pymerc-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymerc"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Python library for interacting with the Mercatorio browser based game"
 authors = ["Joshua Gilman <joshuagilman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jmgilman/pymerc"
 keywords = ["mercatorio", "python", "library", "game"]
 packages = [{ include = "pymerc" }]
@@ -19,11 +19,12 @@
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.24.0"
 pytest = "^8.2.0"
 pytest-asyncio = "^0.23.6"
 python-dotenv = "^1.0.1"
 pytest-subtests = "^0.12.1"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pymerc-0.3.0/PKG-INFO` & `pymerc-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymerc
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for interacting with the Mercatorio browser based game
 Home-page: https://github.com/jmgilman/pymerc
 License: MIT
 Keywords: mercatorio,python,library,game
 Author: Joshua Gilman
 Author-email: joshuagilman@gmail.com
 Requires-Python: >=3.11,<4.0
```

