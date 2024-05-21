# Comparing `tmp/betwatch-1.3.0.tar.gz` & `tmp/betwatch-1.3.1.tar.gz`

## Comparing `betwatch-1.3.0.tar` & `betwatch-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 betwatch-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 betwatch-1.3.0/requirements-dev.lock
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 betwatch-1.3.0/requirements.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-1.3.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/__about__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/__init__.py
--rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/client.py
--rw-r--r--   0        0        0    32194 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/client_async.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/exceptions.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/filters.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/markets.py
--rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.3.0/betwatch/types/updates.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_race_prices.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_races.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_races_async.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/get_races_async_lightweight.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/subscriptions.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 betwatch-1.3.0/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_race.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_race_async.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_races.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 betwatch-1.3.0/tests/test_subscribe_race_updates.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 betwatch-1.3.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.3.0/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 betwatch-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 betwatch-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 betwatch-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 betwatch-1.3.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 betwatch-1.3.1/requirements.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-1.3.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/__about__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/__init__.py
+-rw-r--r--   0        0        0    13690 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/client.py
+-rw-r--r--   0        0        0    34976 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/client_async.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/exceptions.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12404 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.3.1/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/get_races.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/get_races_async.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/get_races_async_lightweight.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/subscriptions.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 betwatch-1.3.1/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/test_get_race.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/test_get_races.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 betwatch-1.3.1/tests/test_subscribe_race_updates.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 betwatch-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.3.1/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 betwatch-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 betwatch-1.3.1/PKG-INFO
```

### Comparing `betwatch-1.3.0/requirements-dev.lock` & `betwatch-1.3.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/requirements.lock` & `betwatch-1.3.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/.github/workflows/test.yml` & `betwatch-1.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/betwatch/__init__.py` & `betwatch-1.3.1/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/betwatch/client.py` & `betwatch-1.3.1/betwatch/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from betwatch.__about__ import __version__
 from betwatch.exceptions import APIKeyNotSetError
 from betwatch.queries import (
     MUTATION_UPDATE_USER_EVENT_DATA,
     QUERY_GET_LAST_SUCCESSFUL_PRICE_UPDATE,
     query_get_race,
+    query_get_race_from_bookmaker_market,
     query_get_races,
 )
 from betwatch.types import Bookmaker, Race, RaceProjection
 from betwatch.types.filters import RacesFilter
 from betwatch.types.updates import SelectionData
 
 log = logging.getLogger(__name__)
@@ -245,14 +246,52 @@
         query = query_get_race(projection)
 
         if parse_result:
             return self._get_race_by_id(race_id, query, parse_result=True)
         else:
             return self._get_race_by_id(race_id, query, parse_result=False)
 
+    @overload
+    def get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        projection: Optional[RaceProjection] = None,
+        parse_result: Literal[True] = True,
+    ) -> Union[Race, None]:
+        ...
+
+    @overload
+    def get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        projection: Optional[RaceProjection] = None,
+        parse_result: Literal[True] = True,
+    ) -> Union[Dict, None]:
+        ...
+
+    def get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        projection: Optional[RaceProjection] = None,
+        parse_result: bool = True,
+    ) -> Union[Race, Dict, None]:
+        # handle defaults
+        if not projection:
+            projection = RaceProjection(markets=True)
+        query = query_get_race_from_bookmaker_market(projection)
+
+        if parse_result:
+            return self._get_race_from_bookmaker_market(
+                market_id, query, parse_result=True
+            )
+        else:
+            return self._get_race_from_bookmaker_market(
+                market_id, query, parse_result=False
+            )
+
     def get_races_today(
         self, projection: Optional[RaceProjection] = None
     ) -> List[Race]:
         """Get all races for today."""
         today = datetime.now()
         tomorrow = datetime.now() + timedelta(days=0)
         return self.get_races_between_dates(today, tomorrow, projection)
@@ -292,14 +331,53 @@
         if result.get("race"):
             if parse_result:
                 return typedload.load(result["race"], Race)
             else:
                 return result["race"]
         return None
 
+    @overload
+    def _get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        query: DocumentNode,
+        parse_result: Literal[True] = True,
+    ) -> Union[Race, None]:
+        ...
+
+    @overload
+    def _get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        query: DocumentNode,
+        parse_result: Literal[False] = False,
+    ) -> Union[Dict, None]:
+        ...
+
+    @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
+    def _get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        query: DocumentNode,
+        parse_result: bool = True,
+    ) -> Union[Race, Dict, None]:
+        log.info(f"Getting race from bookmaker market (market_id={market_id})")
+
+        variables = {
+            "id": market_id,
+        }
+        result = self._gql_client.execute(query, variable_values=variables)
+
+        if result.get("raceFromBookmakerMarket"):
+            if parse_result:
+                return typedload.load(result["raceFromBookmakerMarket"], Race)
+            else:
+                return result["raceFromBookmakerMarket"]
+        return None
+
     def update_event_data(
         self, race_id: str, column_name: str, data: List[SelectionData]
     ):
         """
         Updates event data for a given race ID.
 
         Args:
```

### Comparing `betwatch-1.3.0/betwatch/client_async.py` & `betwatch-1.3.1/betwatch/client_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from betwatch.exceptions import APIKeyNotSetError
 from betwatch.queries import (
     MUTATION_UPDATE_USER_EVENT_DATA,
     QUERY_GET_LAST_SUCCESSFUL_PRICE_UPDATE,
     SUBSCRIPTION_BETFAIR_UPDATES,
     SUBSCRIPTION_RACES_UPDATES,
     query_get_race,
+    query_get_race_from_bookmaker_market,
     query_get_races,
     subscription_race_price_updates,
 )
 from betwatch.types import (
     BetfairMarket,
     Bookmaker,
     BookmakerMarket,
@@ -450,14 +451,60 @@
             projection = RaceProjection(markets=True)
         query = query_get_race(projection)
         if parse_result:
             return await self._get_race_by_id(race_id, query, parse_result=True)
         else:
             return await self._get_race_by_id(race_id, query, parse_result=False)
 
+    @overload
+    async def get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        projection: Optional[RaceProjection] = None,
+        parse_result: Literal[True] = True,
+    ) -> Union[Race, None]:
+        ...
+
+    @overload
+    async def get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        projection: Optional[RaceProjection] = None,
+        parse_result: Literal[False] = False,
+    ) -> Union[Race, None]:
+        ...
+
+    async def get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        projection: Optional[RaceProjection] = None,
+        parse_result: bool = True,
+    ) -> Union[Race, Dict, None]:
+        """Get all details of a specific race by id.
+
+        Args:
+            race_id (str): The id of a race. This can be obtained from the `get_races` method.
+            projection (RaceProjection, optional): The fields to return. Defaults to RaceProjection(markets=True).
+
+        Returns:
+            Union[Race, None]: The race object or None if the race is not found.
+        """
+        # set defaults
+        if not projection:
+            projection = RaceProjection(markets=True)
+        query = query_get_race_from_bookmaker_market(projection)
+        if parse_result:
+            return await self._get_race_from_bookmaker_market(
+                market_id, query, parse_result=True
+            )
+        else:
+            return await self._get_race_from_bookmaker_market(
+                market_id, query, parse_result=False
+            )
+
     async def _monitor(self):
         """Monitor the subscription tasks and restart them if they fail"""
         log.debug("Starting subscription monitor")
         while True:
             try:
                 await asyncio.sleep(1)
                 for d in [
@@ -809,14 +856,54 @@
         if result.get("race"):
             if parse_result:
                 return typedload.load(result["race"], Race)
             else:
                 return result["race"]
         return None
 
+    @overload
+    async def _get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        query: DocumentNode,
+        parse_result: Literal[True] = True,
+    ) -> Union[Race, None]:
+        ...
+
+    @overload
+    async def _get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        query: DocumentNode,
+        parse_result: Literal[False] = False,
+    ) -> Union[Dict, None]:
+        ...
+
+    @backoff.on_exception(backoff.expo, Exception, max_time=60, max_tries=5)
+    async def _get_race_from_bookmaker_market(
+        self,
+        market_id: str,
+        query: DocumentNode,
+        parse_result: bool = False,
+    ) -> Union[Race, Dict, None]:
+        log.info(f"Getting race from bookmaker market (id={market_id})")
+        session = await self._setup_http_session()
+        variables = {
+            "id": market_id,
+        }
+
+        result = await session.execute(query, variable_values=variables)
+
+        if result.get("raceFromBookmakerMarket"):
+            if parse_result:
+                return typedload.load(result["raceFromBookmakerMarket"], Race)
+            else:
+                return result["raceFromBookmakerMarket"]
+        return None
+
     async def update_event_data(
         self, race_id: str, column_name: str, data: List[SelectionData]
     ):
         """
         Updates event data for a given race ID.
 
         Args:
```

### Comparing `betwatch-1.3.0/betwatch/queries.py` & `betwatch-1.3.1/betwatch/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,28 @@
         + """
         }
     }
     """
     )
 
 
+def query_get_race_from_bookmaker_market(projection: RaceProjection) -> DocumentNode:
+    return gql(
+        """
+    query GetRaceFromBookmakerMarket($id: ID!) {
+        raceFromBookmakerMarket(id: $id) {
+         """
+        + get_race_query(projection)
+        + """
+        }
+    }
+    """
+    )
+
+
 QUERY_GET_LAST_SUCCESSFUL_PRICE_UPDATE = gql(
     """
     query GetRace($id: ID!) {
         race(id: $id) {
             id
             status
             links {
```

### Comparing `betwatch-1.3.0/betwatch/types/bookmakers.py` & `betwatch-1.3.1/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/betwatch/types/filters.py` & `betwatch-1.3.1/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/betwatch/types/markets.py` & `betwatch-1.3.1/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/betwatch/types/race.py` & `betwatch-1.3.1/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/get_race_prices.py` & `betwatch-1.3.1/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/get_race_prices_async.py` & `betwatch-1.3.1/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/get_races.py` & `betwatch-1.3.1/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/get_races_async.py` & `betwatch-1.3.1/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/get_races_async_lightweight.py` & `betwatch-1.3.1/examples/get_races_async_lightweight.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/subscriptions.py` & `betwatch-1.3.1/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/examples/update_rated_prices.py` & `betwatch-1.3.1/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/tests/test_get_races.py` & `betwatch-1.3.1/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/tests/test_get_races_async.py` & `betwatch-1.3.1/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/tests/test_subscribe_race_updates.py` & `betwatch-1.3.1/tests/test_subscribe_race_updates.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/.gitignore` & `betwatch-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/LICENSE.txt` & `betwatch-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/README.md` & `betwatch-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.0/pyproject.toml` & `betwatch-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "betwatch"
-version = "1.3.0"
+version = "1.3.1"
 description = 'A Python package for interacting with the Betwatch.com API'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["betwatch", "betting", "sports", "api", "sdk"]
 authors = [{ name = "Jamie Watts", email = "jamie@betwatch.com" }]
 classifiers = [
```

### Comparing `betwatch-1.3.0/PKG-INFO` & `betwatch-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: betwatch
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-Expression: MIT
```

