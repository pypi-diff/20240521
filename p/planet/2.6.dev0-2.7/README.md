# Comparing `tmp/planet-2.6.dev0.tar.gz` & `tmp/planet-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-qffvu8xp/planet-2.6.dev0.tar", last modified: Mon Apr  8 22:07:10 2024, max compression
+gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-w0l3qrjp/planet-2.7.tar", last modified: Tue May 21 17:55:11 2024, max compression
```

## Comparing `planet-2.6.dev0.tar` & `planet-2.7.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-08 22:06:43.000000 planet-2.6.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 22:07:10.000000 planet-2.6.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-08 22:06:43.000000 planet-2.6.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/data/
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/Feature.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/orders_product_bundle_2023-02-24.json
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/order_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28493 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/subscription_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 22:07:10.000000 planet-2.6.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-08 22:06:43.000000 planet-2.6.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-21 17:54:54.000000 planet-2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-21 17:55:11.000000 planet-2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-21 17:54:54.000000 planet-2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-21 17:54:54.000000 planet-2.7/planet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 17:54:54.000000 planet-2.7/planet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-21 17:54:54.000000 planet-2.7/planet/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22507 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-21 17:54:54.000000 planet-2.7/planet/cli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23066 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-21 17:54:54.000000 planet-2.7/planet/clients/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-21 17:54:54.000000 planet-2.7/planet/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-21 17:54:54.000000 planet-2.7/planet/data/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-21 17:54:54.000000 planet-2.7/planet/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-05-21 17:54:54.000000 planet-2.7/planet/data/orders_product_bundle_2023-02-24.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-05-21 17:54:54.000000 planet-2.7/planet/data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-21 17:54:54.000000 planet-2.7/planet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-21 17:54:54.000000 planet-2.7/planet/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-21 17:54:54.000000 planet-2.7/planet/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-21 17:54:54.000000 planet-2.7/planet/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-21 17:54:54.000000 planet-2.7/planet/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19209 2024-05-21 17:54:54.000000 planet-2.7/planet/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-21 17:54:54.000000 planet-2.7/planet/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-21 17:54:54.000000 planet-2.7/planet/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28579 2024-05-21 17:54:54.000000 planet-2.7/planet/subscription_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 17:55:11.000000 planet-2.7/planet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 17:55:11.000000 planet-2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-21 17:54:54.000000 planet-2.7/setup.py
```

### Comparing `planet-2.6.dev0/LICENSE` & `planet-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/PKG-INFO` & `planet-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.6.dev0
+Version: 2.7
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.6.dev0/README.md` & `planet-2.7/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/__init__.py` & `planet-2.7/planet/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/auth.py` & `planet-2.7/planet/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/auth.py` & `planet-2.7/planet/cli/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/cli.py` & `planet-2.7/planet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/cmds.py` & `planet-2.7/planet/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/collect.py` & `planet-2.7/planet/cli/collect.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/data.py` & `planet-2.7/planet/cli/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """The Planet Data CLI."""
 from typing import List, Optional
 from contextlib import asynccontextmanager
 from pathlib import Path
-
 import click
 
 from planet.reporting import AssetStatusBar
 from planet import data_filter, DataClient, exceptions
 from planet.clients.data import (SEARCH_SORT,
                                  LIST_SEARCH_TYPE,
                                  LIST_SEARCH_TYPE_DEFAULT,
@@ -33,14 +32,15 @@
                           SpecificationException)
 
 from . import types
 from .cmds import coro, translate_exceptions
 from .io import echo_json
 from .options import limit, pretty
 from .session import CliSession
+from .validators import check_geom
 
 valid_item_string = "Valid entries for ITEM_TYPES: " + "|".join(
     get_data_item_types())
 
 
 @asynccontextmanager
 async def data_client(ctx):
@@ -277,27 +277,28 @@
 @data.command(epilog=valid_item_string)  # type: ignore
 @click.pass_context
 @translate_exceptions
 @coro
 @click.argument("item_types",
                 type=types.CommaSeparatedString(),
                 callback=check_item_types)
+@click.option("--geom", type=types.Geometry(), callback=check_geom)
 @click.option('--filter',
               type=types.JSON(),
               help="""Apply specified filter to search. Can be a json string,
               filename, or '-' for stdin.""")
 @limit
 @click.option('--name', type=str, help='Name of the saved search.')
 @click.option('--sort',
               type=click.Choice(SEARCH_SORT),
               default=SEARCH_SORT_DEFAULT,
               show_default=True,
               help='Field and direction to order results by.')
 @pretty
-async def search(ctx, item_types, filter, limit, name, sort, pretty):
+async def search(ctx, item_types, geom, filter, limit, name, sort, pretty):
     """Execute a structured item search.
 
     This function outputs a series of GeoJSON descriptions, one for each of the
     returned items, optionally pretty-printed.
 
     ITEM_TYPES is a comma-separated list of item-types to search.
 
@@ -307,52 +308,61 @@
 
     Quick searches are stored for approximately 30 days and the --name
     parameter will be applied to the stored quick search.
     """
     async with data_client(ctx) as cl:
 
         async for item in cl.search(item_types,
+                                    geometry=geom,
                                     search_filter=filter,
                                     name=name,
                                     sort=sort,
                                     limit=limit):
             echo_json(item, pretty)
 
 
 @data.command(epilog=valid_item_string)  # type: ignore
 @click.pass_context
 @translate_exceptions
 @coro
 @click.argument("item_types",
                 type=types.CommaSeparatedString(),
                 callback=check_item_types)
+@click.option("--geom", type=types.Geometry(), callback=check_geom)
 @click.option(
     '--filter',
     type=types.JSON(),
     required=True,
     help="""Filter to apply to search. Can be a json string, filename,
          or '-' for stdin.""")
 @click.option('--name',
               type=str,
               required=True,
               help='Name of the saved search.')
 @click.option('--daily-email',
               is_flag=True,
               help='Send a daily email when new results are added.')
 @pretty
-async def search_create(ctx, item_types, filter, name, daily_email, pretty):
+async def search_create(ctx,
+                        item_types,
+                        geom,
+                        filter,
+                        name,
+                        daily_email,
+                        pretty):
     """Create a new saved structured item search.
 
     This function outputs a full JSON description of the created search,
     optionally pretty-printed.
 
     ITEM_TYPES is a comma-separated list of item-types to search.
     """
     async with data_client(ctx) as cl:
         items = await cl.create_search(item_types=item_types,
+                                       geometry=geom,
                                        search_filter=filter,
                                        name=name,
                                        enable_email=daily_email)
         echo_json(items, pretty)
 
 
 @data.command()  # type: ignore
@@ -481,36 +491,42 @@
     required=True,
     help="""Filter to apply to search. Can be a json string, filename,
          or '-' for stdin.""")
 @click.option('--name',
               type=str,
               required=True,
               help='Name of the saved search.')
+@click.option("--geom",
+              type=types.Geometry(),
+              callback=check_geom,
+              default=None)
 @click.option('--daily-email',
               is_flag=True,
               help='Send a daily email when new results are added.')
 @pretty
 async def search_update(ctx,
                         search_id,
                         item_types,
                         filter,
+                        geom,
                         name,
                         daily_email,
                         pretty):
     """Update a saved search with the given search request.
 
     This function outputs a full JSON description of the updated search,
     optionally pretty-printed.
     """
     async with data_client(ctx) as cl:
         items = await cl.update_search(search_id,
                                        item_types,
-                                       filter,
-                                       name,
-                                       daily_email)
+                                       search_filter=filter,
+                                       name=name,
+                                       geometry=geom,
+                                       enable_email=daily_email)
         echo_json(items, pretty)
 
 
 @data.command(epilog=valid_item_string)  # type: ignore
 @click.pass_context
 @translate_exceptions
 @coro
```

### Comparing `planet-2.6.dev0/planet/cli/io.py` & `planet-2.7/planet/cli/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/options.py` & `planet-2.7/planet/cli/options.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/orders.py` & `planet-2.7/planet/cli/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/cli/subscriptions.py` & `planet-2.7/planet/cli/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .io import echo_json
 from .options import limit, pretty
 from .session import CliSession
 from planet.clients.subscriptions import SubscriptionsClient
 from .. import subscription_request
 from ..subscription_request import sentinel_hub
 from ..specs import get_item_types, validate_item_type, SpecificationException
+from .validators import check_geom
 
 ALL_ITEM_TYPES = get_item_types()
 valid_item_string = "Valid entries for ITEM_TYPES: " + "|".join(ALL_ITEM_TYPES)
 
 
 def check_item_types(ctx, param, item_types) -> Optional[List[dict]]:
     """Validates each item types provided by comparing them to all supported
@@ -342,15 +343,16 @@
 @click.option('--asset-types',
               required=True,
               type=types.CommaSeparatedString(),
               help='One or more comma-separated asset types.')
 @click.option(
     '--geometry',
     required=True,
-    type=types.JSON(),
+    type=types.Geometry(),
+    callback=check_geom,
     help="""Geometry of the area of interest of the subscription that will be
     used to determine matches. Can be a string, filename, or - for stdin.""")
 @click.option('--start-time',
               required=True,
               type=types.DateTime(),
               help='Date and time to begin subscription.')
 @click.option('--end-time',
@@ -402,27 +404,29 @@
 @subscriptions.command()  # type: ignore
 @translate_exceptions
 @click.option(
     '--var-type',
     required=True,
     help='Planetary variable type.',
     type=click.Choice([
+        "analysis_ready_ps",
         "biomass_proxy",
         "land_surface_temperature",
         "soil_water_content",
         "vegetation_optical_depth",
         "forest_carbon_diligence_30m",
         "field_boundaries_sentinel_2_p1m"
     ]),
 )
 @click.option('--var-id', required=True, help='Planetary variable id.')
 @click.option(
     '--geometry',
     required=True,
-    type=types.JSON(),
+    type=types.Geometry(),
+    callback=check_geom,
     help="""Geometry of the area of interest of the subscription that will be
     used to determine matches. Can be a string, filename, or - for stdin.""")
 @click.option('--start-time',
               required=True,
               type=types.DateTime(),
               help='Date and time to begin subscription.')
 @click.option('--end-time',
```

### Comparing `planet-2.6.dev0/planet/cli/types.py` & `planet-2.7/planet/cli/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -89,14 +89,28 @@
 
         if convdict == {}:
             self.fail('JSON cannot be empty.')
 
         return convdict
 
 
+class Geometry(click.ParamType):
+    name = 'geom'
+
+    def __init__(self):
+        self.types = [JSON(), CommaSeparatedString()]
+
+    def convert(self, value, param, ctx):
+        for type in self.types:
+            try:
+                return type.convert(value, param, ctx)
+            except click.BadParameter:
+                continue
+
+
 class Field(click.ParamType):
     """Clarify that this entry is for a field"""
     name = 'field'
 
 
 class Comparison(click.ParamType):
     name = 'comp'
```

### Comparing `planet-2.6.dev0/planet/clients/__init__.py` & `planet-2.7/planet/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/clients/data.py` & `planet-2.7/planet/clients/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from ..data_filter import empty_filter
 from .. import exceptions
 from ..constants import PLANET_BASE_URL
 from ..http import Session
 from ..models import Paged, StreamingBody
 from ..specs import validate_data_item_type
+from ..geojson import as_geom_or_ref
 
 BASE_URL = f'{PLANET_BASE_URL}/data/v1/'
 SEARCHES_PATH = '/searches'
 STATS_PATH = '/stats'
 
 # TODO: get these values from the spec directly gh-619
 # NOTE: these values are mached against a lower-case value so must also be
@@ -108,14 +109,15 @@
         return f'{self._base_url}{SEARCHES_PATH}'
 
     def _item_url(self, item_type, item_id):
         return f'{self._base_url}/item-types/{item_type}/items/{item_id}'
 
     async def search(self,
                      item_types: List[str],
+                     geometry: Optional[dict] = None,
                      search_filter: Optional[dict] = None,
                      name: Optional[str] = None,
                      sort: Optional[str] = None,
                      limit: int = 100) -> AsyncIterator[dict]:
         """Iterate over results from a quick search.
 
         Quick searches are saved for a short period of time (~month). The
@@ -130,14 +132,16 @@
         Parameters:
             item_types: The item types to include in the search.
             search_filter: Structured search criteria to apply. If None,
                 no search criteria is applied.
             sort: Field and direction to order results by. Valid options are
             given in SEARCH_SORT.
             name: The name of the saved search.
+            geometry: GeoJSON, a feature reference or a list of feature
+                references
             limit: Maximum number of results to return. When set to 0, no
                 maximum is applied.
 
         Yields:
             Description of an item.
 
         Raises:
@@ -145,36 +149,39 @@
         """
         url = f'{self._base_url}/quick-search'
 
         search_filter = search_filter or empty_filter()
 
         item_types = [validate_data_item_type(item) for item in item_types]
         request_json = {'filter': search_filter, 'item_types': item_types}
+
+        if geometry:
+            request_json['geometry'] = as_geom_or_ref(geometry)
         if name:
             request_json['name'] = name
 
         params = {}
         if sort and sort != SEARCH_SORT_DEFAULT:
             sort = sort.lower()
             if sort not in SEARCH_SORT:
                 raise exceptions.ClientError(
                     f'{sort} must be one of {SEARCH_SORT}')
             params['_sort'] = sort
-
         response = await self._session.request(method='POST',
                                                url=url,
                                                json=request_json,
                                                params=params)
         async for i in Items(response, self._session.request, limit=limit):
             yield i
 
     async def create_search(self,
                             item_types: List[str],
                             search_filter: dict,
                             name: str,
+                            geometry: Optional[dict] = None,
                             enable_email: bool = False) -> dict:
         """Create a new saved structured item search.
 
         To filter to items you have access to download which are of standard
         (aka not test) quality, use the following:
 
         ```python
@@ -188,66 +195,75 @@
 
         To avoid filtering out any imagery, supply a blank AndFilter, which can
         be created with `data_filter.and_filter([])`.
 
 
         Parameters:
             item_types: The item types to include in the search.
+            geometry: A feature reference or a GeoJSON
             search_filter: Structured search criteria.
             name: The name of the saved search.
             enable_email: Send a daily email when new results are added.
 
         Returns:
             Description of the saved search.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         url = self._searches_url()
 
         item_types = [validate_data_item_type(item) for item in item_types]
+
         request = {
             'name': name,
             'filter': search_filter,
             'item_types': item_types,
             '__daily_email_enabled': enable_email
         }
+        if geometry:
+            request['geometry'] = as_geom_or_ref(geometry)
 
         response = await self._session.request(method='POST',
                                                url=url,
                                                json=request)
         return response.json()
 
     async def update_search(self,
                             search_id: str,
                             item_types: List[str],
                             search_filter: dict,
                             name: str,
+                            geometry: Optional[dict] = None,
                             enable_email: bool = False) -> dict:
         """Update an existing saved search.
 
         Parameters:
             search_id: Saved search identifier.
             item_types: The item types to include in the search.
+            geometry: A feature reference or a GeoJSON
             search_filter: Structured search criteria.
             name: The name of the saved search.
             enable_email: Send a daily email when new results are added.
 
         Returns:
             Description of the saved search.
         """
         url = f'{self._searches_url()}/{search_id}'
 
         item_types = [validate_data_item_type(item) for item in item_types]
+
         request = {
             'name': name,
             'filter': search_filter,
             'item_types': item_types,
             '__daily_email_enabled': enable_email
         }
+        if geometry:
+            request['geometry'] = geometry
 
         response = await self._session.request(method='PUT',
                                                url=url,
                                                json=request)
         return response.json()
 
     async def list_searches(self,
```

### Comparing `planet-2.6.dev0/planet/clients/orders.py` & `planet-2.7/planet/clients/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/clients/subscriptions.py` & `planet-2.7/planet/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/constants.py` & `planet-2.7/planet/constants.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/data/Feature.json` & `planet-2.7/planet/data/Feature.json`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/data/README.md` & `planet-2.7/planet/data/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/data/orders_product_bundle_2023-02-24.json` & `planet-2.7/planet/data/orders_product_bundle_2023-02-24.json`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/data_filter.py` & `planet-2.7/planet/data_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,17 +234,18 @@
     API will automatically attempt to correct the geometry and return matching
     search results.
 
     Parameters:
         geom: GeoJSON describing the filter geometry, feature, or feature
             collection.
     """
-    return _field_filter('GeometryFilter',
-                         field_name='geometry',
-                         config=geojson.as_geom(geom))
+    geom_filter = _field_filter('GeometryFilter',
+                                field_name='geometry',
+                                config=geojson.validate_geom_as_geojson(geom))
+    return geom_filter
 
 
 def number_in_filter(field_name: str, values: List[float]) -> dict:
     """Create a NumberInFilter
 
     The NumberInFilter can be used to search for items with numerical
     poperties. It is useful for matching fields such as gsd.
```

### Comparing `planet-2.6.dev0/planet/exceptions.py` & `planet-2.7/planet/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,7 +86,11 @@
 class PagingError(ClientError):
     """For errors that occur during paging."""
     pass
 
 
 class GeoJSONError(ClientError):
     """Errors that occur due to invalid GeoJSON"""
+
+
+class FeatureError(ClientError):
+    """Errors that occur due to incorrectly formatted feature reference"""
```

### Comparing `planet-2.6.dev0/planet/http.py` & `planet-2.7/planet/http.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/io.py` & `planet-2.7/planet/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/models.py` & `planet-2.7/planet/models.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/order_request.py` & `planet-2.7/planet/order_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,17 +352,17 @@
     Parameters:
         aoi: clip GeoJSON, either Polygon or Multipolygon.
 
     Raises:
         planet.exceptions.ClientError: If GeoJSON is not a valid polygon or
             multipolygon.
     """
-    valid_types = ['Polygon', 'MultiPolygon']
+    valid_types = ['Polygon', 'MultiPolygon', 'ref']
 
-    geom = geojson.as_geom(aoi)
+    geom = geojson.as_geom_or_ref(aoi)
     if geom['type'].lower() not in [v.lower() for v in valid_types]:
         raise ClientError(
             f'Invalid geometry type: {geom["type"]} is not in {valid_types}.')
     return _tool('clip', {'aoi': geom})
 
 
 def composite_tool() -> dict:
```

### Comparing `planet-2.6.dev0/planet/reporting.py` & `planet-2.7/planet/reporting.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/specs.py` & `planet-2.7/planet/specs.py`

 * *Files identical despite different names*

### Comparing `planet-2.6.dev0/planet/subscription_request.py` & `planet-2.7/planet/subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
     return details
 
 
 def catalog_source(
     item_types: List[str],
     asset_types: List[str],
-    geometry: Mapping,
+    geometry: dict,
     start_time: datetime,
     filter: Optional[Mapping] = None,
     end_time: Optional[datetime] = None,
     rrule: Optional[str] = None,
     publishing_stages: Optional[Sequence[Literal["preview",
                                                  "standard",
                                                  "finalized"]]] = None,
@@ -246,15 +246,15 @@
         ]
     except specs.SpecificationException as exception:
         raise ClientError(exception)
 
     parameters = {
         "item_types": item_types,
         "asset_types": asset_types,
-        "geometry": geojson.as_geom(dict(geometry)),
+        "geometry": geojson.as_geom_or_ref(geometry),
     }
 
     try:
         parameters['start_time'] = _datetime_to_rfc3339(start_time)
     except AttributeError:
         raise ClientError('Could not convert start_time to an iso string')
 
@@ -276,22 +276,23 @@
     if time_range_type:
         parameters['time_range_type'] = time_range_type
 
     return {"type": "catalog", "parameters": parameters}
 
 
 def planetary_variable_source(
-    var_type: Literal["biomass_proxy",
+    var_type: Literal["analysis_ready_ps",
+                      "biomass_proxy",
                       "land_surface_temperature",
                       "soil_water_content",
                       "vegetation_optical_depth",
                       "forest_carbon_diligence_30m",
                       "field_boundaries_sentinel_2_p1m"],
     var_id: str,
-    geometry: Mapping,
+    geometry: dict,
     start_time: datetime,
     end_time: Optional[datetime] = None,
 ) -> dict:
     """Construct a Planetary Variable subscription source.
 
     Planetary Variables come in 4 types and are further subdivided
     within these types. See [Subscribing to Planetary
@@ -300,17 +301,18 @@
 
     The return value can be passed to
     [planet.subscription_request.build_request][].
 
     Note: this function does not validate variable types and ids.
 
     Parameters:
-        var_type: one of "biomass_proxy", "land_surface_temperature",
-            "soil_water_content", "vegetation_optical_depth",
-            "forest_carbon_diligence_30m, or field_boundaries_sentinel_2_p1m".
+        var_type: one of "analysis_ready_ps", "biomass_proxy",
+            "land_surface_temperature", "soil_water_content",
+            "vegetation_optical_depth", "forest_carbon_diligence_30m,
+            or field_boundaries_sentinel_2_p1m".
         var_id: a value such as "SWC-AMSR2-C_V1.0_100" for soil water
             content derived from AMSR2 C band.
         geometry: The area of interest of the subscription that will be
             used to determine matches.
         start_time: The start time of the subscription. This time can be
             in the past or future.
         end_time: The end time of the subscription. This time can be in
@@ -351,15 +353,15 @@
         )
         ```
     """
     # TODO: validation of variable types and ids.
 
     parameters = {
         "id": var_id,
-        "geometry": geojson.as_geom(dict(geometry)),
+        "geometry": geojson.as_geom_or_ref(geometry),
     }
 
     try:
         parameters['start_time'] = _datetime_to_rfc3339(start_time)
     except AttributeError:
         raise ClientError('Could not convert start_time to an iso string')
 
@@ -592,17 +594,17 @@
             500 vertices. The minimum geographic area of any polygon or
             internal ring is one square meter.
 
     Raises:
         planet.exceptions.ClientError: If aoi is not a valid polygon or
             multipolygon.
     """
-    valid_types = ['Polygon', 'MultiPolygon']
+    valid_types = ['Polygon', 'MultiPolygon', 'ref']
 
-    geom = geojson.as_geom(dict(aoi))
+    geom = geojson.as_geom_or_ref(dict(aoi))
     if geom['type'].lower() not in [v.lower() for v in valid_types]:
         raise ClientError(
             f'Invalid geometry type: {geom["type"]} is not in {valid_types}.')
 
     return _tool('clip', {'aoi': geom})
```

### Comparing `planet-2.6.dev0/planet.egg-info/PKG-INFO` & `planet-2.7/planet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.6.dev0
+Version: 2.7
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.6.dev0/planet.egg-info/SOURCES.txt` & `planet-2.7/planet.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 planet/cli/data.py
 planet/cli/io.py
 planet/cli/options.py
 planet/cli/orders.py
 planet/cli/session.py
 planet/cli/subscriptions.py
 planet/cli/types.py
+planet/cli/validators.py
 planet/clients/__init__.py
 planet/clients/data.py
 planet/clients/orders.py
 planet/clients/subscriptions.py
 planet/data/Feature.json
 planet/data/README.md
 planet/data/orders_product_bundle_2023-02-24.json
```

### Comparing `planet-2.6.dev0/setup.py` & `planet-2.7/setup.py`

 * *Files identical despite different names*

