# Comparing `tmp/jageocoder-2.1.6.post1.tar.gz` & `tmp/jageocoder-2.1.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.1.6.post1.tar", max compression
+gzip compressed data, was "jageocoder-2.1.7.dev2.tar", max compression
```

## Comparing `jageocoder-2.1.6.post1.tar` & `jageocoder-2.1.7.dev2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.6.post1/LICENSE
--rw-r--r--   0        0        0    10310 2024-05-08 05:06:37.213667 jageocoder-2.1.6.post1/README.md
--rw-r--r--   0        0        0     1370 2024-05-08 05:44:38.488032 jageocoder-2.1.6.post1/jageocoder/__init__.py
--rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-08-03 02:25:59.209435 jageocoder-2.1.6.post1/jageocoder/address.py
--rw-r--r--   0        0        0     1421 2023-08-03 02:25:59.209435 jageocoder-2.1.6.post1/jageocoder/aliases.json
--rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.6.post1/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.6.post1/jageocoder/dataset.py
--rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/exceptions.py
--rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.6.post1/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.6.post1/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    13645 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/module.py
--rw-r--r--   0        0        0    54152 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/node.py
--rw-r--r--   0        0        0     9824 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/remote.py
--rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/result.py
--rw-r--r--   0        0        0    15687 2024-04-16 08:33:55.201079 jageocoder-2.1.6.post1/jageocoder/rtree.py
--rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.6.post1/jageocoder/strlib.py
--rw-r--r--   0        0        0    53605 2024-05-08 03:51:15.514717 jageocoder-2.1.6.post1/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.6.post1/jageocoder/trie.py
--rw-r--r--   0        0        0     1309 2024-05-08 05:44:22.963766 jageocoder-2.1.6.post1/pyproject.toml
--rw-r--r--   0        0        0    11853 1970-01-01 00:00:00.000000 jageocoder-2.1.6.post1/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.7.dev2/LICENSE
+-rw-r--r--   0        0        0    10479 2024-05-21 05:03:13.340045 jageocoder-2.1.7.dev2/README.md
+-rw-r--r--   0        0        0     1571 2024-05-21 05:06:11.091329 jageocoder-2.1.7.dev2/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev2/jageocoder/__main__.py
+-rw-r--r--   0        0        0     3489 2024-05-14 07:28:53.462543 jageocoder-2.1.7.dev2/jageocoder/address.py
+-rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev2/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.7.dev2/jageocoder/dataset.py
+-rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev2/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev2/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.7.dev2/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    16470 2024-05-13 05:54:01.596831 jageocoder-2.1.7.dev2/jageocoder/module.py
+-rw-r--r--   0        0        0    55284 2024-05-15 04:29:24.686867 jageocoder-2.1.7.dev2/jageocoder/node.py
+-rw-r--r--   0        0        0    11679 2024-05-20 07:49:12.679443 jageocoder-2.1.7.dev2/jageocoder/remote.py
+-rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev2/jageocoder/result.py
+-rw-r--r--   0        0        0    16645 2024-05-20 04:30:05.890848 jageocoder-2.1.7.dev2/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.7.dev2/jageocoder/strlib.py
+-rw-r--r--   0        0        0    43706 2024-05-16 02:30:24.211931 jageocoder-2.1.7.dev2/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.7.dev2/jageocoder/trie.py
+-rw-r--r--   0        0        0     1308 2024-05-21 05:06:18.411466 jageocoder-2.1.7.dev2/pyproject.toml
+-rw-r--r--   0        0        0    12021 1970-01-01 00:00:00.000000 jageocoder-2.1.7.dev2/PKG-INFO
```

### Comparing `jageocoder-2.1.6.post1/README.md` & `jageocoder-2.1.7.dev2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 日本語版は README_ja.md をお読みください。
 
 This is a Python port of the Japanese-address geocoder `DAMS` used in CSIS at the University of Tokyo's ["Address Matching Service"](https://newspat.csis.u-tokyo.ac.jp/geocode/modules/addmatch/index.php?content_id=1) and [GSI Maps](https://maps.gsi.go.jp/).
 
 # Getting Started
 
-This package provides address-geocoding functionality for Python programs. The basic usage is to specify a dictionary with `init()` then call `search()` to get geocoding results.
+This package provides address-geocoding and reverse-geocoding functionality for Python programs. The basic usage is to specify a dictionary with `init()` then call `search()` to get geocoding results.
 
 ```python
 >>> import jageocoder
 >>> jageocoder.init(url='https://jageocoder.info-proto.com/jsonrpc')
 >>> jageocoder.search('新宿区西新宿2-8-1')
 {'matched': '新宿区西新宿2-8-', 'candidates': [{'id': 5961406, 'name': '8番', 'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}]}
 ```
@@ -27,19 +27,19 @@
 
 - Install the package with `pip install jageocoder`
 
 To use Jageocoder, you need to install the "Dictionary Database" on the same machine or connect to the RPC service provided by [jageocoder-server](https://t-sagara.github.io/jageocoder/server/) .
 
 ### Install Dictionary Database
 
-Large amounts of data can be processed at high speed when a dictionary database is installed. A database covering addresses in Japan requires 30 GB or more of storage.
+When a dictionary database is installed, large amounts of data can be processed at high speed. A database covering addresses in Japan requires 25 GB or more of storage.
 
 - Download an address database file compatible with that version from [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 
-      wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip 
+      jageocoder download-dictionary https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip 
 
 - Install the dictionary with `install-dictionary` command
 
       jageocoder install-dictionary jukyo_all_v21.zip
 
 If you need to know the location of the dictionary directory,
 perform `get-db-dir` command as follows. (Or call
@@ -257,14 +257,20 @@
 ```python
 >>> parent.children
 <sqlalchemy.orm.dynamic.AppenderQuery object at 0x7fbc08404b38>
 >>> [child.name for child in parent.children]
 ['10番', '11番', '1番', '2番', '3番', '4番', '5番', '6番', '7番', '8番', '9番']
 ```
 
+# For developers
+
+## Documentation
+
+Tutorials and references are [here](https://jageocoder.readthedocs.io/ja/latest/).
+
 ## Create your own dictionary
 
 Consider using [jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
 
 ## Contributing
 
 Address notation varies. So suggestions for logic improvements are welcome.
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/__init__.py` & `jageocoder-2.1.7.dev2/jageocoder/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.1.6.post1'  # The package version
+__version__ = '2.1.7.dev2'  # The package version
 __dictionary_version__ = '20230927'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
@@ -33,20 +33,26 @@
     'get_module_tree',
     'download_dictionary',
     'install_dictionary',
     'uninstall_dictionary',
     'create_trie_index',
     'search',
     'searchNode',
+    'search_by_machiaza_id',
+    'search_by_postcode',
+    'search_by_citycode',
+    'search_by_prefcode',
     'reverse',
     'version',
     'dictionary_version',
     'installed_dictionary_version',
     'installed_dictionary_readme',
 ]
 
 from jageocoder.module import init, free, is_initialized, \
     get_db_dir, set_search_config, get_search_config, \
     get_module_tree, download_dictionary, install_dictionary, \
     uninstall_dictionary, create_trie_index, \
-    search, searchNode, reverse, version, dictionary_version, \
+    search, searchNode, search_by_machiaza_id, search_by_postcode, \
+    search_by_citycode, search_by_prefcode, reverse, \
+    version, dictionary_version, \
     installed_dictionary_version, installed_dictionary_readme  # noqa: F401
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/__main__.py` & `jageocoder-2.1.7.dev2/jageocoder/__main__.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/aza_master.py` & `jageocoder-2.1.7.dev2/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/dataset.py` & `jageocoder-2.1.7.dev2/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/exceptions.py` & `jageocoder-2.1.7.dev2/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/itaiji.py` & `jageocoder-2.1.7.dev2/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/itaiji_dic.json` & `jageocoder-2.1.7.dev2/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/module.py` & `jageocoder-2.1.7.dev2/jageocoder/module.py`

 * *Files 12% similar despite different names*

```diff
@@ -478,14 +478,128 @@
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
 
     global _tree
     return _tree.reverse(x, y, level, as_dict)
 
 
+def search_by_machiaza_id(
+        id: str
+) -> list:
+    """
+    Finds the corresponding address nodes from the "machiaza-id" of
+    the address base registry.
+
+    Parameters
+    ----------
+    id: str
+        Machiaza-id.
+
+    Returns
+    -------
+    List[AddressNode]
+
+    Notes
+    -----
+    - If "id" is 12 characters, the first 5 characters are considered the JISX0402 code.
+    - If "id" is 13 characters, the first 6 characters are considered the lg-code.
+    - In either of the above cases, search for the address node whose machiaza-id
+        matches the rest 7 characters in the corresponding municipality.
+    - Otherwise, it searches for address nodes whose machiaza-id matches "id"
+        from all municipalities. In this case, aza_id must be 7 characters.
+    """
+    if not is_initialized():
+        raise JageocoderError("Not initialized. Call 'init()' first.")
+
+    global _tree
+    return _tree.search_by_machiaza_id(id)
+
+
+def search_by_postcode(
+        code: str
+) -> list:
+    """
+    Finds the corresponding address node from a postcode.
+
+    Parameters
+    ----------
+    code: str
+        The postal code as defined by the Japan Post.
+
+    Returns
+    -------
+    List[AddressNode]
+
+    Notes
+    -----
+    - The "code" must be 7 characters.
+    """
+    if not is_initialized():
+        raise JageocoderError("Not initialized. Call 'init()' first.")
+
+    global _tree
+    return _tree.search_by_postcode(code)
+
+
+def search_by_prefcode(
+        code: str
+) -> list:
+    """
+    Finds the corresponding address nodes from the JISX0401 code
+    or the prefacture's local-government code.
+
+    Parameters
+    ----------
+    code: str
+        Prefacture code as defined in JISX0401, of local government code defined by MIC.
+
+    Returns
+    -------
+    List[AddressNode]
+
+    Notes
+    -----
+    - If "code" is 2 characters, the code is considered the JISX0401 code.
+    - If "code" is 6 characters, the code is considered the local-govenment code.
+    """
+    if not is_initialized():
+        raise JageocoderError("Not initialized. Call 'init()' first.")
+
+    global _tree
+    return _tree.search_by_prefcode(code)
+
+
+def search_by_citycode(
+        code: str
+) -> list:
+    """
+    Finds the corresponding address nodes from the JISX0402 code
+    or the local-government code.
+
+    Parameters
+    ----------
+    code: str
+        City code as defined in JISX0402, of local government code defined by MIC.
+
+    Returns
+    -------
+    List[AddressNode]
+
+    Notes
+    -----
+    - If "code" is 5 characters, the code is considered the JISX0402 code.
+    - If "code" is 6 characters, the code is considered the local-govenment code.
+    """
+    if not is_initialized():
+        raise JageocoderError("Not initialized. Call 'init()' first.")
+
+    global _tree
+    return _tree.search_by_citycode(code)
+
+
 def create_trie_index() -> None:
     """
     Create the TRIE index from the database file.
 
     This function is a shortcut for AddressTree.create_trie_index().
     """
     if not is_initialized():
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/node.py` & `jageocoder-2.1.7.dev2/jageocoder/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,18 +208,24 @@
 
         return self.name
 
     @property
     def dataset(self):
         """
         Get dataset record.
-
         """
         return self.table.datasets.get(id=self.priority)
 
+    @property
+    def levelname(self) -> str:
+        """
+        Get level by name.
+        """
+        return AddressLevel.levelname(self.level)
+
     @classmethod
     def from_record(cls, record) -> AddressNode:
         """
         Convert from a record of AddressNodeTable to an AddressNode object.
 
         Parameters
         ----------
@@ -1248,14 +1254,36 @@
                 "level": self.level,
                 "priority": self.priority,
                 "note": self.note,
                 "fullname": self.get_fullname(),
             }
         }
 
+    def to_json(self):
+        """
+        Convert node to JSONable dict for data transfer.
+
+        Notes
+        -----
+        - Different from the 'as_dict' method, this method includes
+            all attributes in the database, such as 'parent_id'.
+        """
+        return {
+            "id": self.id,
+            "name": self.name,
+            "name_index": self.name_index,
+            "x": self.x,
+            "y": self.y,
+            "level": self.level,
+            "priority": self.priority,
+            "note": self.note,
+            "parent_id": self.parent_id,
+            "sibling_id": self.sibling_id,
+        }
+
     def get_fullname(
         self,
         delimiter: Optional[str] = None,
         alt: Optional[str] = '',
     ) -> Union[str, List[str]]:
         """
         Returns a complete address notation starting with the name of
@@ -1296,15 +1324,15 @@
         cur_node = self
         while cur_node is not None:
             nodes.insert(0, cur_node)
             cur_node = cur_node.get_parent()
 
         return nodes
 
-    def get_nodes_by_level(self):
+    def get_nodes_by_level(self) -> List[AddressNode | None]:
         """
         The method returns an array of this node and its upper nodes.
         The Nth node of the array contains the node corresponding
         to address level N.
         If there is no element corresponding to level N, None is stored.
 
         Example
@@ -1504,34 +1532,42 @@
 
         aza_record = tree.aza_masters.search_by_code(code)
         return aza_record
 
     def get_aza_names(
         self,
         tree: Optional[AddressTree] = None,
+        levelname: Optional[bool] = False,
     ) -> list:
         """
         Returns representation of Aza node containing this node.
 
         Parameters
         ----------
         tree: AddressTree, optional
             The tree containing this node.
+        levelname: bool, optional
+            If true, Returns the address level by name, not by number.
 
         Returns
         -------
         list
             A list containing notations from the prefecture level
             to the Aza level in the following format:
 
             [AddressLevel, Kanji, Kana, English, code]
         """
         aza_record = self.get_aza_record(tree)
         if aza_record:
-            return json.loads(aza_record.names)
+            results = json.loads(aza_record.names)
+            if levelname:
+                for i in range(len(results)):
+                    results[i][0] = AddressLevel.levelname(results[i][0])
+
+            return results
 
         return []
 
     def get_postcode(self) -> str:
         """
         Returns the 7digit postcode of the oaza that
         contains this node.
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/remote.py` & `jageocoder-2.1.7.dev2/jageocoder/remote.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from functools import lru_cache
 import json
+from logging import getLogger
 import os
 import requests
-from typing import Any, List, Optional, Union
+from typing import Any, List, NoReturn, Optional, Union
 import uuid
 
 from jageocoder.address import AddressLevel
 from jageocoder.exceptions import RemoteTreeException
 from jageocoder.node import AddressNode
 from jageocoder.result import Result
-from jageocoder.tree import LRU
+from jageocoder.tree import AddressTree, LRU
 
 
+logger = getLogger(__name__)
 _session = None
 
 
 def _json_request(
         url: str,
         method: str,
         params: object,
@@ -24,25 +26,35 @@
     payload = {
         "jsonrpc": "2.0",
         "method": method,
         "params": params,
         "id": str(uuid.uuid4()),
     }
     if _session is None:
+        logger.debug("Start a new HTTP session with the remote tree.")
         _session = requests.Session()
 
+    logger.debug(
+        "Send JSON-RPC request ---\n" +
+        json.dumps(payload, indent=2, ensure_ascii=False)
+    )
     response = _session.post(
         url=url,
         data=json.dumps(payload),
         headers={"Content-Type": "application/json"}
     ).json()
 
     if "error" in response:
         raise RemoteTreeException(response["error"])
 
+    logger.debug(
+        "Receive JSON-RPC response ---\n" +
+        json.dumps(response["result"], indent=2, ensure_ascii=False)
+    )
+
     return response["result"]
 
 
 class RemoteDataset(object):
 
     def __init__(self, url: str) -> None:
         self.url = url
@@ -68,14 +80,15 @@
 class RemoteNodeTable(object):
 
     def __init__(self, url: str) -> None:
         self.url = url
         self.datasets = RemoteDataset(url=url)
         self.cache = LRU()
         self.server_signature = None
+        self.mode = 'r'   # Always read only
 
     def update_server_signature(self) -> str:
         """
         Update the remote server's signature.
 
         Note
         ----
@@ -93,15 +106,15 @@
             self.cache.clear()
             self.server_signature = server_signature
 
         return self.server_signature
 
     def get_record(self, pos: int) -> AddressNode:
         """
-        Get the record at the specified position
+        Get the record at the specified position from the remote server
         and convert it to AddressNode object.
 
         Parameters
         ----------
         pos: int
             The position.
 
@@ -119,16 +132,64 @@
             params={"pos": pos, "server": self.server_signature},
         )
         node = AddressNode(**rpc_result)
         node.table = self
         self.cache[pos] = node
         return node
 
+    def search_records_on(
+            self,
+            attr: str,
+            value: str,
+            funcname: str = "get") -> list:
+        """
+        Search value from the table on the specified attribute on the remote server.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+        value: str
+            The target value.
+        funcname: str
+            The name of search method.
+            - "get" searches for records that exactly match the value.
+            - "prefixes" searches for records that contained in the value.
+            - "keys" searches for records that containing the value.
 
-class RemoteTree(object):
+        Returns
+        -------
+        List[Record]
+            List of records.
+
+        Notes
+        -----
+        - TRIE index must be created on the column before searching.
+        - The TRIE index file will be automatically opened if it exists.
+        """
+        rpc_result = _json_request(
+            url=self.url,
+            method="node.search_records_on",
+            params={
+                "attr": attr,
+                "value": value,
+                "funcname": funcname,
+                "server": self.server_signature
+            },
+        )
+        nodes = []
+        for record in rpc_result:
+            node = AddressNode(**record)
+            node.table = self
+            nodes.append(node)
+
+        return nodes
+
+
+class RemoteTree(AddressTree):
     """
     The proxy class for remote server's address-tree structure.
 
     Attributes
     ----------
     url: str
         Endpoint URL of the currently connected server.
@@ -202,74 +263,41 @@
 
         - auto_redirect: bool (default = True)
             When this option is set and the retrieved node has a
             new address recorded in the "ref" attribute,
             the new address is retrieved automatically.
         """
         for k, v in kwargs.items():
+            self.validate_config(key=k, value=v)
             self.config[k] = v
 
-    def get_config(
-            self,
-            keys: Union[str, List[str], None] = None
-    ) -> dict:
-        """
-        Get configurable parameter(s).
-
-        Parameters
-        ----------
-        keys: str, List[str], optional
-            If a name of parameter is specified, return its value.
-            Otherwise, a dict of specified key and its value pairs
-            will be returned.
-
-        Returns
-        -------
-        Any, or dict.
-        """
-        if keys is None:
-            return self.config
-
-        if isinstance(keys, str):
-            return self.config.get(keys)
-
-        results = {}
-        for key in keys:
-            if key in self.config:
-                results[key] = self.config[key]
-
-        return results
-
     def _close(self) -> None:
         if _session:
             del _session
             _session = None
 
-    def get_node_by_id(self, node_id: int) -> AddressNode:
-        """
-        Get the full node information by its id.
-
-        Parameters
-        ----------
-        node_id: int
-            The target node id.
-
-        Return
-        ------
-        AddressNode
-        """
-        return self.address_nodes.get_record(node_id)
+    def get_trie_nodes(self) -> NoReturn:
+        raise RemoteTreeException(
+            "This method is not available for RemoteTree."
+        )
 
     def installed_dictionary_version(self) -> str:
         return _json_request(
             url=self.url,
             method="jageocoder.installed_dictionary_version",
             params={},
         )
 
+    def search_by_trie(
+            self, *args, **kwargs
+    ) -> NoReturn:
+        raise RemoteTreeException(
+            "This method is not available for RemoteTree."
+        )
+
     def searchNode(self, query: str) -> List[Result]:
         """
         Searches for address nodes corresponding to an address notation
         and returns the matching substring and a list of nodes.
 
         Parameters
         ----------
@@ -348,7 +376,23 @@
         for r in rpc_result:
             if not as_dict:
                 r["candidate"] = self.get_node_by_id(r["candidate"]["id"])
 
             results.append(r)
 
         return results
+
+    def search_by_machiaza_id(self, id: str) -> List[AddressNode]:
+        self.address_nodes.update_server_signature()
+        return super().search_by_machiaza_id(id)
+
+    def search_by_postcode(self, code: str) -> List[AddressNode]:
+        self.address_nodes.update_server_signature()
+        return super().search_by_postcode(code)
+
+    def search_by_prefcode(self, code: str) -> List[AddressNode]:
+        self.address_nodes.update_server_signature()
+        return super().search_by_prefcode(code)
+
+    def search_by_citycode(self, code: str) -> List[AddressNode]:
+        self.address_nodes.update_server_signature()
+        return super().search_by_citycode(code)
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/result.py` & `jageocoder-2.1.7.dev2/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/rtree.py` & `jageocoder-2.1.7.dev2/jageocoder/rtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,16 +320,18 @@
                 if node.level > AddressLevel.AZA:
                     id = node.sibling_id
                     continue
                 elif node.level < AddressLevel.OAZA:
                     id += 1
                     continue
                 elif not node.has_valid_coordinate_values():
-                    id += 1
-                    continue
+                    node = node.add_dummy_coordinates()
+                    if not node.has_valid_coordinate_values():
+                        id += 1
+                        continue
 
                 file_idx.insert(
                     id=id,
                     coordinates=(node.x, node.y, node.x, node.y)
                 )
                 id += 1
 
@@ -438,14 +440,17 @@
         nodes = []
         ancestors = set()
         max_level = 0
         for node in self._sort_by_dist(x, y, self.idx.nearest((x, y, x, y), 10)):
             if node.id in ancestors:
                 continue
 
+            if not node.has_valid_coordinate_values():
+                node = node.add_dummy_coordinates()
+
             nodes.append(node)
             max_level = max(max_level, node.level)
             # Ancestor nodes of registering node are excluded.
             cur = node.parent
             while cur is not None:
                 nodes = [node for node in nodes if node.id != cur.id]
                 ancestors.add(cur.id)
@@ -458,41 +463,56 @@
                 child_id = node.id
                 while child_id < node.sibling_id:
                     child_node = self._tree.get_address_node(id=child_id)
                     if child_node.level > level:
                         child_id = child_node.parent.sibling_id
                         continue
                     elif not child_node.has_valid_coordinate_values():
-                        child_id += 1
-                        continue
+                        child_node = child_node.add_dummy_coordinates()
+                        if not child_node.has_valid_coordinate_values():
+                            child_id += 1
+                            continue
 
                     local_idx.insert(
                         id=child_id,
                         coordinates=(
                             child_node.x, child_node.y,
                             child_node.x, child_node.y))
                     child_id += 1
 
             nodes = []
             ancestors = set()
             for node in self._sort_by_dist(x, y, local_idx.nearest((x, y, x, y), 20)):
                 if node.id in ancestors:
                     continue
 
+                if not node.has_valid_coordinate_values():
+                    node = node.add_dummy_coordinates()
+
                 nodes.append(node)
                 # Ancestor nodes of registering node are excluded.
                 cur = node.parent
                 while cur is not None:
                     nodes = [node for node in nodes if node.id != cur.id]
                     ancestors.add(cur.id)
                     cur = cur.parent
 
         # Select the 3 nodes that make the smallest triangle
         # surrounding the target point
-        nodes = DelaunayTriangle.select(x, y, nodes)
+        if len(nodes) == 0:
+            return []
+
+        if self.distance(x, y, nodes[0].x, nodes[0].y) < 1.0e-02:
+            # If the distance between the nearest point and the search point is
+            # less than 1 cm, it returns three points in order of distance.
+            # This is because the nearest point may not be included in
+            # the search results due to a calculation error.
+            nodes = nodes[0:3]
+        else:
+            nodes = DelaunayTriangle.select(x, y, nodes)
 
         # Convert nodes to the dict format.
         results = []
         registered = set()
         for node in nodes:
             while node.level > level:
                 node = node.parent
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/strlib.py` & `jageocoder-2.1.7.dev2/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/jageocoder/tree.py` & `jageocoder-2.1.7.dev2/jageocoder/tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -233,33 +233,14 @@
                 'JAGEOCODER_OPT_AUTO_REDIRECT',
                 self.config["auto_redirect"]),
         })
 
         # Itaiji converter
         self.converter = Converter()
 
-    def close(self) -> NoReturn:
-        raise RuntimeError("Unnecessary function close was called.")
-
-    def is_version_compatible(self) -> bool:
-        """
-        Check if the dictionary version is compatible with the package.
-
-        Returns
-        -------
-        bool
-            True if compatible, otherwize False.
-        """
-        current_dict_ver = self.get_version()
-        required_dict_ver = jageocoder.dictionary_version()
-        if current_dict_ver != required_dict_ver:
-            return False
-
-        return True
-
     def __not_in_readonly_mode(self) -> None:
         """
         Check if the dictionary is not opened in the read-only mode.
 
         If the mode is read-only, AddressTreeException will be raised.
         """
         if self.mode == 'r':
@@ -272,20 +253,17 @@
         If not set yet, create and get the node from the database.
 
         Returns
         -------
         AddressNode:
             The root node object.
         """
-        if self.root is None:
-            self.root = AddressNode.get(
-                tree=self,
-                pos=AddressNode.ROOT_NODE_ID)
-
-        return self.root
+        return self.get_node_by_id(
+            node_id=AddressNode.ROOT_NODE_ID
+        )
 
     def get_version(self) -> str:
         """
         Get the version of the tree file.
 
         Return
         ------
@@ -322,43 +300,32 @@
 
         Parameters
         ----------
         category: str
             Category name such as 'jisx0402' or 'postcode'.
         value: str
             Target value.
-        levels: List[int], optional
-            The address levels of target nodes.
 
         Returns
         -------
         List[AddressNode]
         """
         nodes = []
         pattern = '{}:{}'.format(category, value)
         nodes = self.address_nodes.search_records_on(
             attr="note", value=pattern)  # exact match
 
         return nodes
 
+    @deprecated("Use 'node.get_fullname()' instead of this method.")
     def get_node_fullname(self, node: Union[AddressNode, int]) -> List[str]:
-        if isinstance(node, AddressNode):
-            node_id = node.id
-        else:
-            node_id = node
-
-        names = []
-        while node_id >= 0:
-            node = self.session.execute(
-                'SELECT parent_id, name FROM node WHERE id={}'.format(
-                    node_id)).one()
-            names.insert(0, node.name)
-            node_id = node.parent_id
+        if isinstance(node, int):
+            node = self.get_node_by_id(node)
 
-        return names
+        return node.get_fullname()
 
     def set_config(self, **kwargs):
         """
         Set configuration parameters.
 
         Note
         ----
@@ -562,293 +529,25 @@
     def _get_config(self, key: str):
         if key not in self.config:
             raise RuntimeError(
                 "The config key '{}' does not exist.".format(key))
 
         return self.config[key]
 
-    def check_line_format(self, args: List[str]) -> int:
-        """
-        Receives split args from a line of comma-separated text
-        representing a single address element, and returns
-        the format ID.
-
-        Parameters
-        ----------
-        args: list[str]
-
-        Return
-        ------
-        int
-            The id of the identified format.
-            1. Address names without level, lon, lat
-            2. Address names without level, lon, lat, note
-            3. Address names without level, lon, lat, level without note
-            4. Address names without level, lon, lat, level, note
-
-        Examples
-        --------
-        >>> from jageocoder_converter import BaseConverter
-        >>> base = BaseConverter()
-        >>> base.check_line_format(['1;北海道','3;札幌市','4;中央区','141.34103','43.05513'])
-        1
-        >>> base.check_line_format(['1;北海道','3;札幌市','4;中央区','5;大通','6;西二十丁目','141.326249','43.057218','01101/ODN-20/'])
-        2
-        >>> base.check_line_format(['北海道','札幌市','中央区','大通','西二十丁目','141.326249','43.057218',6])
-        3
-        >>> base.check_line_format(['北海道','札幌市','中央区','大通','西二十丁目','141.326249','43.057218',6,'01101/ODN-20/'])
-        4
-        """  # noqa: E501
-
-        # Find the first consecutive position of a real number or None.
-        pos0 = None
-        pos1 = None
-        for pos, arg in enumerate(args):
-            if arg == '' or self.re_float.match(arg):
-                if pos0:
-                    pos1 = pos
-                    break
-                else:
-                    pos0 = pos
-            else:
-                pos0 = None
-
-        if pos1 is None:
-            raise AddressTreeException(
-                'Unexpected line format.\n{}'.format(','.join(args)))
-
-        names = args[0:pos0]
-
-        if self.re_address.match(names[0]):
-            if len(args) == pos1 + 1:
-                logger.debug("line format id: 1")
-                return 1
-
-            if len(args) == pos1 + 2:
-                logger.debug("line format id: 2")
-                return 2
-
-        else:
-            if len(args) == pos1 + 2 and self.re_int.match(args[pos1 + 1]):
-                logger.debug("line format id: 3")
-                return 3
-
-            if len(args) == pos1 + 3 and self.re_int.match(args[pos1 + 1]):
-                logger.debug("line format id: 4")
-                return 4
-
-        raise AddressTreeException(
-            'Unexpected line format.\n{}'.format(','.join(args)))
-
-    def parse_line_args(self, args: List[str], format_id: int) -> list:
-        """
-        Receives split args from a line of comma-separated text
-        representing a single address element, and returns
-        a list of parsed attributes.
-
-        Parameters
-        ----------
-        args: list[str]
-            List of split args in a line
-        format_id: int
-            The id of the line format identfied by `check_line_format`
-
-        Return
-        ------
-        list
-            A list containing the following attributes.
-            - Address names: list[str]
-            - Longitude: float
-            - Latitude: float
-            - Level: int or None
-            - note: str or None
-
-        Examples
-        --------
-        >>> from jageocoder_converter import BaseConverter
-        >>> base = BaseConverter()
-        >>> base.parse_line_args(['1;北海道','3;札幌市','4;中央区','141.34103','43.05513'], 1)
-        [['1;北海道','3;札幌市','4;中央区'], 141.34103, 43.05513, None, None]
-        >>> base.parse_line_args(['1;北海道','3;札幌市','4;中央区','5;大通','6;西二十丁目','141.326249','43.057218','01101/ODN-20/'], 2)
-        [['1;北海道','3;札幌市','4;中央区','5;大通','6;西二十丁目'],141.326249,43.057218,None,'01101/ODN-20/']
-        >>> base.parse_line_args(['北海道','札幌市','中央区','大通','西二十丁目','141.326249','43.057218',6,'01101/ODN-20/'], 4)
-        [['北海道','札幌市','中央区','大通','西二十丁目'],141.326249,43.057218,6,'01101/ODN-20/']
-        """  # noqa: E501
-
-        def fv(val: str) -> Union[float, None]:
-            """
-            Convert str to float value.
-            If the str is empty, return None.
-            """
-            if val == '':
-                return None
-            return float(val)
-
-        nargs = len(args)
-        if format_id == 1:
-            return [
-                args[0:nargs-2], fv(args[nargs-2]), fv(args[nargs-1]),
-                None, None]
-
-        if format_id == 2:
-            return [
-                args[0:nargs-3], fv(args[nargs-3]), fv(args[nargs-2]),
-                None, args[nargs-1]]
-
-        if format_id == 3:
-            return [
-                args[0:nargs-3], fv(args[nargs-3]), fv(args[nargs-2]),
-                int(args[nargs-1]), None]
-
-        if format_id == 4:
-            return [
-                args[0:nargs-4], fv(args[nargs-4]), fv(args[nargs-3]),
-                int(args[nargs-2]), args[nargs-1]]
-
-        raise AddressTreeException(
-            'Unexpected line format id: {}'.format(format_id))
-
-    def add_address(self,
-                    address_names: List[str],
-                    do_update: bool = False,
-                    cache: Optional[LRU] = None,
-                    **kwargs) -> AddressNode:
-        """
-        Create a new AddressNode and add to the tree.
-
-        Parameters
-        ----------
-        address_names : list of str
-            A list of the address element names.
-            For example, ["東京都","新宿区","西新宿", "２丁目"]
-        do_update : bool
-            When an address with the same name already exists,
-            update it with the value of kwargs if 'do_update' is true,
-            otherwise do nothing.
-        cache : LRU, optional
-            A dict object to use as a cache for improving performance,
-            whose keys are the address notation from the prefecture level
-            and whose values are the corresponding nodes.
-            If not specified or None is given, do not use the cache.
-        **kwargs : properties of the new address node.
-            x : float. X coordinate or longitude in decimal degree
-            y : float. Y coordinate or latitude in decimal degree
-            level: int. Level of the node
-            note : str. Note
-
-        Return
-        ------
-        AddressNode:
-            The added node.
-        """
-        self.__not_in_readonly_mode()
-        cur_node = self.get_root()
-        for i, elem in enumerate(address_names):
-            path = ''.join(address_names[0:i + 1])
-            is_leaf = (i == len(address_names) - 1)
-
-            if cache is not None:
-                if path in cache:
-                    cur_node = cache[path]
-                    continue
-                elif i < len(address_names):
-                    logger.debug("Cache miss: '{}'".format(path))
-
-            m = self.re_address.match(elem)
-            if m:
-                level = m.group(1)
-                name = m.group(2)
-            else:
-                level = AddressLevel.UNDEFINED
-                name = elem
-                if is_leaf:
-                    level = kwargs.get('level', AddressLevel.UNDEFINED)
-
-            name_index = self.converter.standardize(name)
-            node = cur_node.get_child(name_index)
-            if not node:
-                kwargs.update({
-                    'name': name,
-                    'parent': cur_node,
-                    'level': level})
-                new_node = AddressNode(**kwargs)
-                cur_node.add_child(new_node)
-                cur_node = new_node
-            else:
-                cur_node = node
-                if is_leaf:
-                    if do_update:
-                        cur_node.set_attributes(**kwargs)
-                    else:
-                        cur_node = None
-
-            if cache is not None and \
-                    cur_node is not None and \
-                    not is_leaf:
-                cache[path] = cur_node
-
-        return cur_node
-
-    def update_name_index(self) -> int:
-        """
-        Update `name_index` field using the standardizing logic
-        of the current version.
-
-        Note
-        ----
-        This method also updates the version information of
-        the dictionary.
-
-        Return
-        ------
-        int:
-            Number of records updated.
-        """
-        self.__not_in_readonly_mode()
-        counts = self.session.query(AddressNode).count()
-        pct = 0
-        pagesize = int(counts / 100) + 1
-        diffs = 0
-        for offset in range(0, counts, pagesize):
-            nodes = self.session.query(
-                AddressNode).offset(offset).limit(pagesize)
-            for node in nodes:
-                new_name_index = self.converter.standardize(node.name)
-                if node.name_index != new_name_index:
-                    logger.info((
-                        'The index of "{}" was updated from "{}" to "{}"'
-                    ).format(node.name, node.name_index, new_name_index))
-                    node.name_index = new_name_index
-                    self.session.add(node)
-                    diffs += 1
-
-            self.session.commit()
-            pct += 1
-            logger.info("Updated {pct}% ({offset}/{total})".format(
-                pct=pct, offset=offset + pagesize, total=counts))
-
-        logger.info("Update completed.")
-        # Update version
-        root_node = self.get_root()
-        root_node.note = jageocoder.dictionary_version()
-        self.session.add(root_node)
-        self.session.commit()
-
-        return diffs
-
     def get_trie_nodes(self) -> TrieNode:
         """
         Get the TRIE node table.
 
         Notes
         -----
         - Todo: If the trie index is not created, create.
         """
         return TrieNode(db_dir=self.db_dir)
 
+    '''
     def create_trie_index(self) -> None:
         """
         Create the TRIE index from the tree.
         """
         self.__not_in_readonly_mode()
         self.index_table = {}
         logger.debug("Collecting labels for the trie index...")
@@ -872,14 +571,16 @@
         The collected notations will be stored in `tree.index_table`.
 
         Generates notations that describe everything from the name of
         the prefecture to the name of the oaza without abbreviation,
         notations that omit the name of the prefecture, or notations
         that omit the name of the prefecture and the city.
         """
+        self.__not_in_readonly_mode()
+
         # Build temporary lookup table
         logger.debug("Building temporary lookup table..")
         tmp_id_name_table = {}
         pos = AddressNode.ROOT_NODE_ID + 1
         while pos < self.address_nodes.count_records():
             node = self.address_nodes.get_record(pos=pos)
             if node.level <= AddressLevel.OAZA:
@@ -940,14 +641,16 @@
                 else:
                     self.index_table[candidate] = [v.id]
 
     def _extend_index_table(self) -> None:
         """
         Expand the index, including support for omission of county names.
         """
+        self.__not_in_readonly_mode()
+
         # Build temporary lookup table
         logger.debug("Building temporary town and village table..")
         tmp_id_name_table = {}
         pos = AddressNode.ROOT_NODE_ID + 1
         while pos < self.address_nodes.count_records():
             node = self.address_nodes.get_record(pos=pos)
             if node.level <= AddressLevel.CITY:
@@ -1004,137 +707,35 @@
 
         Collect notations recursively the names of all address elements
         which was registered in the TRIE index, retrieve
         the id of each notations in the TRIE index,
         then add the TrieNode to the database that maps
         the TRIE id to the node id.
         """
+        self.__not_in_readonly_mode()
+
         logger.debug("Creating mapping table from trie_id:node_id")
         trie_nodes = []
         for k, node_id_list in self.index_table.items():
             trie_id = self.trie.get_id(k)
             if len(trie_nodes) <= trie_id:
                 trie_nodes += [None for _ in range(
                     trie_id - len(trie_nodes) + 1)]
 
             trie_nodes[trie_id] = {
                 "id": trie_id,
                 "nodes": node_id_list,
             }
 
         return trie_nodes
-
-    def read_file(self, path: os.PathLike,
-                  do_update: bool = False) -> None:
-        """
-        Add AddressNodes from a text file.
-        See 'data/test.txt' for the format of the text file.
-
-        Parameters
-        ----------
-        path : os.PathLike
-            Text file path.
-        do_update : bool (default=False)
-            When an address with the same name already exists,
-            update it with the value of the new data
-            if 'do_update' is true, otherwise do nothing.
-        """
-        raise AddressTreeException(
-            'This method is not available in read-only mode.')
-        logger.debug("Starting read_file...")
-        with open(path, 'r', encoding='utf-8',
-                  errors='backslashreplace') as f:
-            self.read_stream(f, do_update=do_update)
-
-    def read_stream(self, fp: TextIO,
-                    do_update: bool = False) -> None:
-        """
-        Add AddressNodes to the tree from a stream.
-
-        Parameters
-        ----------
-        fp : io.TextIO
-            Input text stream.
-        do_update : bool (default=False)
-            When an address with the same name already exists,
-            update it with the value of the new data
-            if 'do_update' is true, otherwise do nothing.
-        """
-        self.__not_in_readonly_mode()
-        nread = 0
-        stocked = []
-        prev_names = None
-        cache = LRU(maxsize=512)
-
-        reader = csv.reader(fp)
-        format_id = None
-
-        while True:
-            try:
-                args = reader.__next__()
-            except UnicodeDecodeError:
-                logger.error("Decode error at the next line of {}".format(
-                    prev_names))
-                exit(1)
-            except StopIteration:
-                break
-
-            if args is None:
-                break
-
-            if format_id is None:
-                format_id = self.check_line_format(args)
-
-            names, lon, lat, level, note = self.parse_line_args(
-                args, format_id)
-
-            if names[-1].startswith('!'):
-                names = names[0:-1]
-
-            if prev_names == names:
-                logger.debug("Skipping '{}".format(prev_names))
-                continue
-
-            prev_names = names
-
-            node = self.add_address(
-                names, do_update, cache=cache,
-                x=lon, y=lat, level=level, note=note)
-            nread += 1
-            if nread % 1000 == 0:
-                logger.info("- read {} lines.".format(nread))
-
-            if node is None:
-                # The node exists and not updated.
-                continue
-
-            stocked.append(node)
-            if len(stocked) > 10000:
-                logger.debug("Inserting into the database... ({} - {})".format(
-                    stocked[0].get_fullname(), stocked[-1].get_fullname()))
-                for node in stocked:
-                    self.session.add(node)
-
-                self.session.commit()
-                stocked.clear()
-
-        logger.debug("Finished reading the stream.")
-        if len(stocked) > 0:
-            logger.debug("Inserting into the database... ({} - {})".format(
-                stocked[0].get_fullname(), stocked[-1].get_fullname()))
-            for node in stocked:
-                self.session.add(node)
-
-            self.session.commit()
-
-        logger.debug("Done.")
+    '''
 
     def search_by_tree(self, address_names: List[str]) -> AddressNode:
         """
-        Get the corresponding node id from the list of address element names,
+        Get the corresponding node from the list of address element names,
         recursively search for child nodes using the tree.
 
         For example, ['東京都','新宿区','西新宿','二丁目'] will search
         the '東京都' node under the root node, search the '新宿区' node
         from the children of the '東京都' node. Repeat this process and
         return the '二丁目' node which is a child of '西新宿' node.
 
@@ -1222,20 +823,17 @@
             trie_node = self.trie_nodes.get_record(pos=trie_id)
             offset = self.converter.match_len(index, k)
             key = index[0:offset]
             rest_index = index[offset:]
             for node_id in trie_node.nodes:
                 node = self.get_address_node(id=node_id)
 
-                if node.y > 90.0 and self.get_config('require_coordinates'):
+                if not node.has_valid_coordinate_values() \
+                        and self.get_config('require_coordinates'):
                     node = node.add_dummy_coordinates()
-                    # if node.y > 90.0:
-                    #     logger.debug("Node {}({}) has no coordinates.".format(
-                    #         node.name, node.id))
-                    #     continue
 
                 if min_key == '' and node.level <= AddressLevel.WARD:
                     # To make the process quicker, once a node higher
                     # than the city level is found, addresses shorter
                     # than the node are not searched after this.
                     logger.debug((
                         "A node with ward or higher levels found. "
@@ -1320,15 +918,16 @@
 
                         if inside != 1:
                             msg = "Node {}({}) is not in the target area."
                             logger.debug(msg.format(
                                 cand.node.name, cand.node.id))
                             continue
 
-                    if self.get_config("require_coordinates") and cand.node.y > 90.0:
+                    if self.get_config("require_coordinates") \
+                            and not cand.node.has_valid_coordinate_values():
                         logger.debug("Node {}({}) has no coordinates.".format(
                             cand.node.name, cand.node.id
                         ))
                         continue
 
                     _len = offset + cand.nchars
                     _part = offset + len(cand.matched)
@@ -1500,22 +1099,17 @@
         return recovered
 
     def create_note_index_table(self) -> None:
         """
         Collect notes from all address elements and create
         search table with index.
         """
+        self.__not_in_readonly_mode()
         self.address_nodes.create_indexes()
 
-    def get_cache_info(self) -> dict:
-        cache_info = {
-            "get_record": AddressNodeTable.get_record.cache_info(),
-        }
-        return cache_info
-
     def reverse(
         self,
         x: float,
         y: float,
         level: Optional[int] = None,
         as_dict: Optional[bool] = True
     ) -> list:
@@ -1544,7 +1138,153 @@
             {"candidate":AddressNode, "dist":float} 
         """
         if self.reverse_index is None:
             from jageocoder.rtree import Index
             self.reverse_index = Index(tree=self)
 
         return self.reverse_index.nearest(x=x, y=y, level=level, as_dict=as_dict)
+
+    def search_by_machiaza_id(
+            self,
+            id: str
+    ) -> List[AddressNode]:
+        """
+        Finds the corresponding address nodes from the "machiaza-id" of
+        the address base registry.
+
+        Parameters
+        ----------
+        id: str
+            Machiaza-id.
+
+        Returns
+        -------
+        List[AddressNode]
+
+        Notes
+        -----
+        - If "id" is 12 characters, the first 5 characters are considered the JISX0402 code.
+        - If "id" is 13 characters, the first 6 characters are considered the lg-code.
+        - In either of the above cases, search for the address node whose machiaza-id
+            matches the rest 7 characters in the corresponding municipality.
+        - Otherwise, it searches for address nodes whose machiaza-id matches "id"
+            from all municipalities. In this case, aza_id must be 7 characters.
+        """
+        if len(id) == 12:
+            # jisx0402(5digits) + aza_id(7digits)
+            candidates = self.search_nodes_by_codes(
+                category="aza_id",
+                value=id[-7:])
+            nodes = [x for x in candidates if x.get_city_jiscode() == id[0:5]]
+        elif len(id) == 13:
+            # lasdec(6digits) + aza_id(7digits)
+            candidates = self.search_nodes_by_codes(
+                category="aza_id",
+                value=id[-7:])
+            nodes = [x for x in candidates
+                     if x.get_city_local_authority_code() == id[0:6]]
+        else:
+            nodes = self.search_nodes_by_codes(
+                category="aza_id",
+                value=id)
+
+        return nodes
+
+    def search_by_postcode(
+            self,
+            code: str
+    ) -> List[AddressNode]:
+        """
+        Finds the corresponding address node from a postcode.
+
+        Parameters
+        ----------
+        code: str
+            The postal code as defined by the Japan Post.
+
+        Returns
+        -------
+        List[AddressNode]
+
+        Notes
+        -----
+        - The "code" must be 7 characters.
+        """
+        if len(code) == 7:
+            # Postcode(7digits)
+            return self.search_nodes_by_codes(
+                category="postcode",
+                value=code)
+
+        return []
+
+    def search_by_prefcode(
+            self,
+            code: str
+    ) -> List[AddressNode]:
+        """
+        Finds the corresponding address nodes from the JISX0401 code
+        or the prefacture's local-government code.
+
+        Parameters
+        ----------
+        code: str
+            Prefacture code as defined in JISX0401, of local government code defined by MIC.
+
+        Returns
+        -------
+        List[AddressNode]
+
+        Notes
+        -----
+        - If "code" is 2 characters, the code is considered the JISX0401 code.
+        - If "code" is 6 characters, the code is considered the local-govenment code.
+        """
+        if len(code) == 2:
+            # jisx0401(2digits)
+            return self.search_nodes_by_codes(
+                category="jisx0401",
+                value=code)
+
+        elif len(code) == 6:
+            # lg-code(6digits)
+            return self.search_nodes_by_codes(
+                category="jisx0401",
+                value=code[0:2])
+
+        return []
+
+    def search_by_citycode(
+            self,
+            code: str
+    ) -> List[AddressNode]:
+        """
+        Finds the corresponding address nodes from the JISX0402 code
+        or the local-government code.
+
+        Parameters
+        ----------
+        code: str
+            City code as defined in JISX0402, of local government code defined by MIC.
+
+        Returns
+        -------
+        List[AddressNode]
+
+        Notes
+        -----
+        - If "code" is 5 characters, the code is considered the JISX0402 code.
+        - If "code" is 6 characters, the code is considered the local-govenment code.
+        """
+        if len(code) == 5:
+            # jisx0402(5digits)
+            return self.search_nodes_by_codes(
+                category="jisx0402",
+                value=code)
+
+        elif len(code) == 6:
+            # lg-code(6digits)
+            return self.search_nodes_by_codes(
+                category="jisx0402",
+                value=code[0:5])
+
+        return []
```

### Comparing `jageocoder-2.1.6.post1/jageocoder/trie.py` & `jageocoder-2.1.7.dev2/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.6.post1/pyproject.toml` & `jageocoder-2.1.7.dev2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.1.6.post1"
+version = "2.1.7.dev2"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-2.1.6.post1/PKG-INFO` & `jageocoder-2.1.7.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.1.6.post1
+Version: 2.1.7.dev2
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,15 @@
 
 日本語版は README_ja.md をお読みください。
 
 This is a Python port of the Japanese-address geocoder `DAMS` used in CSIS at the University of Tokyo's ["Address Matching Service"](https://newspat.csis.u-tokyo.ac.jp/geocode/modules/addmatch/index.php?content_id=1) and [GSI Maps](https://maps.gsi.go.jp/).
 
 # Getting Started
 
-This package provides address-geocoding functionality for Python programs. The basic usage is to specify a dictionary with `init()` then call `search()` to get geocoding results.
+This package provides address-geocoding and reverse-geocoding functionality for Python programs. The basic usage is to specify a dictionary with `init()` then call `search()` to get geocoding results.
 
 ```python
 >>> import jageocoder
 >>> jageocoder.init(url='https://jageocoder.info-proto.com/jsonrpc')
 >>> jageocoder.search('新宿区西新宿2-8-1')
 {'matched': '新宿区西新宿2-8-', 'candidates': [{'id': 5961406, 'name': '8番', 'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}]}
 ```
@@ -66,19 +66,19 @@
 
 - Install the package with `pip install jageocoder`
 
 To use Jageocoder, you need to install the "Dictionary Database" on the same machine or connect to the RPC service provided by [jageocoder-server](https://t-sagara.github.io/jageocoder/server/) .
 
 ### Install Dictionary Database
 
-Large amounts of data can be processed at high speed when a dictionary database is installed. A database covering addresses in Japan requires 30 GB or more of storage.
+When a dictionary database is installed, large amounts of data can be processed at high speed. A database covering addresses in Japan requires 25 GB or more of storage.
 
 - Download an address database file compatible with that version from [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 
-      wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip 
+      jageocoder download-dictionary https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip 
 
 - Install the dictionary with `install-dictionary` command
 
       jageocoder install-dictionary jukyo_all_v21.zip
 
 If you need to know the location of the dictionary directory,
 perform `get-db-dir` command as follows. (Or call
@@ -296,14 +296,20 @@
 ```python
 >>> parent.children
 <sqlalchemy.orm.dynamic.AppenderQuery object at 0x7fbc08404b38>
 >>> [child.name for child in parent.children]
 ['10番', '11番', '1番', '2番', '3番', '4番', '5番', '6番', '7番', '8番', '9番']
 ```
 
+# For developers
+
+## Documentation
+
+Tutorials and references are [here](https://jageocoder.readthedocs.io/ja/latest/).
+
 ## Create your own dictionary
 
 Consider using [jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
 
 ## Contributing
 
 Address notation varies. So suggestions for logic improvements are welcome.
```

