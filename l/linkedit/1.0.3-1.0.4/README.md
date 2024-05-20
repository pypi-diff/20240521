# Comparing `tmp/linkedit-1.0.3.tar.gz` & `tmp/linkedit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedit-1.0.3.tar", last modified: Sun May 19 22:48:10 2024, max compression
+gzip compressed data, was "linkedit-1.0.4.tar", last modified: Mon May 20 22:03:21 2024, max compression
```

## Comparing `linkedit-1.0.3.tar` & `linkedit-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:48:10.583886 linkedit-1.0.3/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    74010 2024-05-19 22:48:10.583886 linkedit-1.0.3/PKG-INFO
--rw-rw-r--   0 khiat     (1000) khiat     (1000)    73556 2024-05-19 22:43:18.000000 linkedit-1.0.3/README.md
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:48:10.583886 linkedit-1.0.3/linkedit/
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.3/linkedit/__init__.py
--rw-r--r--   0 khiat     (1000) khiat     (1000)   100702 2024-05-19 22:10:00.000000 linkedit-1.0.3/linkedit/linkedit.py
-drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-19 22:48:10.583886 linkedit-1.0.3/linkedit.egg-info/
--rw-r--r--   0 khiat     (1000) khiat     (1000)    74010 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/PKG-INFO
--rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/SOURCES.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/dependency_links.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/requires.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-19 22:48:10.000000 linkedit-1.0.3/linkedit.egg-info/top_level.txt
--rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-19 22:48:10.583886 linkedit-1.0.3/setup.cfg
--rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-19 22:47:33.000000 linkedit-1.0.3/setup.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-20 22:03:21.227932 linkedit-1.0.4/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-20 22:03:21.227932 linkedit-1.0.4/PKG-INFO
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)    71021 2024-05-20 21:58:55.000000 linkedit-1.0.4/README.md
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-20 22:03:21.227932 linkedit-1.0.4/linkedit/
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      280 2024-05-19 17:39:14.000000 linkedit-1.0.4/linkedit/__init__.py
+-rw-r--r--   0 khiat     (1000) khiat     (1000)   100341 2024-05-20 22:01:42.000000 linkedit-1.0.4/linkedit/linkedit.py
+drwxr-xr-x   0 khiat     (1000) khiat     (1000)        0 2024-05-20 22:03:21.227932 linkedit-1.0.4/linkedit.egg-info/
+-rw-r--r--   0 khiat     (1000) khiat     (1000)    71475 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/PKG-INFO
+-rw-r--r--   0 khiat     (1000) khiat     (1000)      219 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/SOURCES.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        1 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/dependency_links.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       16 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/requires.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)        9 2024-05-20 22:03:21.000000 linkedit-1.0.4/linkedit.egg-info/top_level.txt
+-rw-r--r--   0 khiat     (1000) khiat     (1000)       38 2024-05-20 22:03:21.227932 linkedit-1.0.4/setup.cfg
+-rw-rw-r--   0 khiat     (1000) khiat     (1000)      721 2024-05-20 21:54:11.000000 linkedit-1.0.4/setup.py
```

### Comparing `linkedit-1.0.3/PKG-INFO` & `linkedit-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
@@ -319,37 +319,14 @@
 
 ```bash
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
 None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
 ```
 
 
-#### You Can Create A List From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-[6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### You Can Create A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -650,37 +627,14 @@
 
 ```bash
 > [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
 => [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7], circular=True)
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-> [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -725,37 +679,14 @@
 
 
 ```bash
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None
 ```
 
 
-##### You Can Create A List Of Nodes Objects From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
-
-
-nodes_object_list = x.to_list(node=True)
-print(nodes_object_list)
-```
-
-
-### Output
-
-
-```bash
-[<linkedit.singlyLinkedListNode object at 0x7f7bc6ea33d0>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c10>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c90>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c50>, <linkedit.singlyLinkedListNode object at 0x7f7bc6ee0450>, <linkedit.singlyLinkedListNode object at 0x7f7bc6cdfd90>, <linkedit.singlyLinkedListNode object at 0x7f7bc6cdfbd0>]
-```
-
-
 ##### You Can Create A Dict Of Nodes Objects From The Linked List
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -1063,37 +994,14 @@
 
 ```bash
 None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7])
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import doublyLinkedList
 
 
@@ -1394,37 +1302,14 @@
 
 ```bash
 => [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
 > [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7], circular=True)
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-=> [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import doublyLinkedList
 
 
@@ -1481,37 +1366,14 @@
 Forward : 
 None <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None
 Backward : 
 None <- [7] <=> [5] <=> [9] <=> [1] <=> [8] <=> [3] <=> [6] -> None
 ```
 
 
-##### You Can Create A List Of Nodes Objects From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7])
-
-
-nodes_object_list = x.to_list(node=True)
-print(nodes_object_list)
-```
-
-
-### Output
-
-
-```bash
-[<linkedit.doublyLinkedListNode object at 0x7fcf159b3a90>, <linkedit.doublyLinkedListNode object at 0x7fcf159b3b10>, <linkedit.doublyLinkedListNode object at 0x7fcf159b3ad0>, <linkedit.doublyLinkedListNode object at 0x7fcf159dc350>, <linkedit.doublyLinkedListNode object at 0x7fcf157db550>, <linkedit.doublyLinkedListNode object at 0x7fcf157dbcd0>, <linkedit.doublyLinkedListNode object at 0x7fcf157dbb10>]
-```
-
-
 ##### You Can Create A Dict Of Nodes Objects From The Linked List
 
 
 ```python
 from linkedit import doublyLinkedList
```

### Comparing `linkedit-1.0.3/README.md` & `linkedit-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -304,37 +304,14 @@
 
 ```bash
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
 None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
 ```
 
 
-#### You Can Create A List From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-[6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### You Can Create A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -635,37 +612,14 @@
 
 ```bash
 > [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
 => [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7], circular=True)
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-> [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -710,37 +664,14 @@
 
 
 ```bash
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None
 ```
 
 
-##### You Can Create A List Of Nodes Objects From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
-
-
-nodes_object_list = x.to_list(node=True)
-print(nodes_object_list)
-```
-
-
-### Output
-
-
-```bash
-[<linkedit.singlyLinkedListNode object at 0x7f7bc6ea33d0>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c10>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c90>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c50>, <linkedit.singlyLinkedListNode object at 0x7f7bc6ee0450>, <linkedit.singlyLinkedListNode object at 0x7f7bc6cdfd90>, <linkedit.singlyLinkedListNode object at 0x7f7bc6cdfbd0>]
-```
-
-
 ##### You Can Create A Dict Of Nodes Objects From The Linked List
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -1048,37 +979,14 @@
 
 ```bash
 None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7])
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import doublyLinkedList
 
 
@@ -1379,37 +1287,14 @@
 
 ```bash
 => [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
 > [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7], circular=True)
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-=> [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import doublyLinkedList
 
 
@@ -1466,37 +1351,14 @@
 Forward : 
 None <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None
 Backward : 
 None <- [7] <=> [5] <=> [9] <=> [1] <=> [8] <=> [3] <=> [6] -> None
 ```
 
 
-##### You Can Create A List Of Nodes Objects From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7])
-
-
-nodes_object_list = x.to_list(node=True)
-print(nodes_object_list)
-```
-
-
-### Output
-
-
-```bash
-[<linkedit.doublyLinkedListNode object at 0x7fcf159b3a90>, <linkedit.doublyLinkedListNode object at 0x7fcf159b3b10>, <linkedit.doublyLinkedListNode object at 0x7fcf159b3ad0>, <linkedit.doublyLinkedListNode object at 0x7fcf159dc350>, <linkedit.doublyLinkedListNode object at 0x7fcf157db550>, <linkedit.doublyLinkedListNode object at 0x7fcf157dbcd0>, <linkedit.doublyLinkedListNode object at 0x7fcf157dbb10>]
-```
-
-
 ##### You Can Create A Dict Of Nodes Objects From The Linked List
 
 
 ```python
 from linkedit import doublyLinkedList
```

### Comparing `linkedit-1.0.3/linkedit/linkedit.py` & `linkedit-1.0.4/linkedit/linkedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,25 +254,14 @@
     @tail.deleter
     def tail(self: "linkedList") -> None:
         self._tail = None
 
     def isEmpty(self: "linkedList") -> bool:
         return not self._head
 
-    def to_list(self: "linkedList", node: bool = False) -> list:
-        head: object | None = self._head
-        new_list: list = []
-        for _ in range(self.len):
-            if not node:
-                new_list.append(head.data)
-            else:
-                new_list.append(head)
-            head: object | None = head.next
-        return new_list
-
     def index(
         self: "linkedList",
         value: int | float | complex | str | list | tuple | set | dict | None,
     ) -> int:
         """Return first index of value.
 
         Raises ValueError if the value is not present."""
```

### Comparing `linkedit-1.0.3/linkedit.egg-info/PKG-INFO` & `linkedit-1.0.4/linkedit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedit
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sophisticate Linked List
 Home-page: https://pypi.org/project/linkedit/
 Author: khiat Mohammed Abderrezzak
 Author-email: khiat.abderrezzak@gmail.com
 License: MIT
 Keywords: linked list
 Classifier: Programming Language :: Python :: 3
@@ -319,37 +319,14 @@
 
 ```bash
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
 None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
 ```
 
 
-#### You Can Create A List From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-[6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### You Can Create A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -650,37 +627,14 @@
 
 ```bash
 > [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
 => [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7], circular=True)
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-> [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -725,37 +679,14 @@
 
 
 ```bash
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None
 ```
 
 
-##### You Can Create A List Of Nodes Objects From The Linked List
-
-
-```python
-from linkedit import singlyLinkedList
-
-
-x = singlyLinkedList([6, 3, 8, 1, 9, 5, 7])
-
-
-nodes_object_list = x.to_list(node=True)
-print(nodes_object_list)
-```
-
-
-### Output
-
-
-```bash
-[<linkedit.singlyLinkedListNode object at 0x7f7bc6ea33d0>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c10>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c90>, <linkedit.singlyLinkedListNode object at 0x7f7bc6eb7c50>, <linkedit.singlyLinkedListNode object at 0x7f7bc6ee0450>, <linkedit.singlyLinkedListNode object at 0x7f7bc6cdfd90>, <linkedit.singlyLinkedListNode object at 0x7f7bc6cdfbd0>]
-```
-
-
 ##### You Can Create A Dict Of Nodes Objects From The Linked List
 
 
 ```python
 from linkedit import singlyLinkedList
 
 
@@ -1063,37 +994,14 @@
 
 ```bash
 None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
 [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -> None (NULL)
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7])
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-None (NULL) <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None (NULL)
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import doublyLinkedList
 
 
@@ -1394,37 +1302,14 @@
 
 ```bash
 => [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
 > [6] -> [3] -> [8] -> [1] -> [9] -> [5] -> [7] -
 ```
 
 
-#### Creating A List From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7], circular=True)
-y = x.to_list()
-print(x)
-print(y)
-```
-
-
-### Output
-
-
-```bash
-=> [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] <=
-[6, 3, 8, 1, 9, 5, 7]
-```
-
-
 #### Creating A Dictionary From The Linked List 
 
 
 ```python
 from linkedit import doublyLinkedList
 
 
@@ -1481,37 +1366,14 @@
 Forward : 
 None <- [6] <=> [3] <=> [8] <=> [1] <=> [9] <=> [5] <=> [7] -> None
 Backward : 
 None <- [7] <=> [5] <=> [9] <=> [1] <=> [8] <=> [3] <=> [6] -> None
 ```
 
 
-##### You Can Create A List Of Nodes Objects From The Linked List
-
-
-```python
-from linkedit import doublyLinkedList
-
-
-x = doublyLinkedList([6, 3, 8, 1, 9, 5, 7])
-
-
-nodes_object_list = x.to_list(node=True)
-print(nodes_object_list)
-```
-
-
-### Output
-
-
-```bash
-[<linkedit.doublyLinkedListNode object at 0x7fcf159b3a90>, <linkedit.doublyLinkedListNode object at 0x7fcf159b3b10>, <linkedit.doublyLinkedListNode object at 0x7fcf159b3ad0>, <linkedit.doublyLinkedListNode object at 0x7fcf159dc350>, <linkedit.doublyLinkedListNode object at 0x7fcf157db550>, <linkedit.doublyLinkedListNode object at 0x7fcf157dbcd0>, <linkedit.doublyLinkedListNode object at 0x7fcf157dbb10>]
-```
-
-
 ##### You Can Create A Dict Of Nodes Objects From The Linked List
 
 
 ```python
 from linkedit import doublyLinkedList
```

### Comparing `linkedit-1.0.3/setup.py` & `linkedit-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="linkedit",
-    version="1.0.3",
+    version="1.0.4",
     author="khiat Mohammed Abderrezzak",
     author_email="khiat.abderrezzak@gmail.com",
     license="MIT",
     description="Sophisticate Linked List",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/linkedit/",
```

