# Comparing `tmp/django_iris-0.2.5b1.tar.gz` & `tmp/django_iris-0.2.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_iris-0.2.5b1.tar", last modified: Mon May 20 12:52:39 2024, max compression
+gzip compressed data, was "django_iris-0.2.5b2.tar", last modified: Mon May 20 23:15:42 2024, max compression
```

## Comparing `django_iris-0.2.5b1.tar` & `django_iris-0.2.5b2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.876733 django_iris-0.2.5b1/django_iris/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13484 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/django_iris/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/django_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/django_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.884733 django_iris-0.2.5b1/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (127)      299 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1337 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1896 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      578 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1483 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    20104 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2311 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      618 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (127)       96 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2735 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    49548 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    21467 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2614 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    12049 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      797 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6906 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    10247 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6756 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      213 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    14456 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4905 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6643 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4130 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      354 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2966 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5515 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     3797 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1662 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1327 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1963 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    41638 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4330 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1773 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      218 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.888733 django_iris-0.2.5b1/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (127)     2535 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (127)   102320 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1391 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2115 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     4076 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5293 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5541 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    12910 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      557 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.888733 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (127)    78828 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    16163 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2304 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     6770 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.888733 django_iris-0.2.5b1/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (127)     4370 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5241 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    10774 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     5441 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (127)    10509 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1203 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      172 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      585 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      171 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      522 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     2296 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      320 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1628 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (127)     1379 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (127)      665 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (127)      341 2024-05-20 12:52:39.000000 django_iris-0.2.5b1/irisnative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-20 12:52:39.892733 django_iris-0.2.5b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 12:52:28.000000 django_iris-0.2.5b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.206027 django_iris-0.2.5b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 23:15:42.206027 django_iris-0.2.5b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.194027 django_iris-0.2.5b2/django_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13484 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/django_iris/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.206027 django_iris-0.2.5b2/django_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-20 23:15:42.000000 django_iris-0.2.5b2/django_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-20 23:15:42.000000 django_iris-0.2.5b2/django_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 23:15:42.000000 django_iris-0.2.5b2/django_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 23:15:42.000000 django_iris-0.2.5b2/django_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.198027 django_iris-0.2.5b2/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      299 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1337 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1896 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      578 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1483 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    20104 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2311 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      618 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)       96 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2735 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    49548 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    21467 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2614 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    12049 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      797 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6906 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    10247 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6756 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      213 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    14456 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4905 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6643 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4130 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      354 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2966 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5515 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     3797 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1662 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1327 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1963 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    41638 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4330 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1773 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      218 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.202027 django_iris-0.2.5b2/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2535 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)   102320 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1391 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2115 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4076 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5293 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5541 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    12910 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      557 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.202027 django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (127)    78828 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    16163 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2304 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6770 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.206027 django_iris-0.2.5b2/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4370 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5241 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    10774 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5441 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)    10509 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1203 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      172 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      585 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      171 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      522 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2296 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      320 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1628 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1379 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:15:42.206027 django_iris-0.2.5b2/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      665 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (127)      341 2024-05-20 23:15:41.000000 django_iris-0.2.5b2/irisnative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-20 23:15:42.206027 django_iris-0.2.5b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-20 23:15:30.000000 django_iris-0.2.5b2/setup.py
```

### Comparing `django_iris-0.2.5b1/LICENSE` & `django_iris-0.2.5b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/PKG-INFO` & `django_iris-0.2.5b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iris
-Version: 0.2.5b1
+Version: 0.2.5b2
 Summary: Django backend for InterSystems IRIS
 Home-page: https://github.com/caretdev/django-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/django-iris
 Project-URL: Tracker, https://github.com/caretdev/django-iris/issues
```

### Comparing `django_iris-0.2.5b1/README.md` & `django_iris-0.2.5b2/README.md`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/__init__.py` & `django_iris-0.2.5b2/django_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/base.py` & `django_iris-0.2.5b2/django_iris/base.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/compiler.py` & `django_iris-0.2.5b2/django_iris/compiler.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/creation.py` & `django_iris-0.2.5b2/django_iris/creation.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/cursor.py` & `django_iris-0.2.5b2/django_iris/cursor.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/features.py` & `django_iris-0.2.5b2/django_iris/features.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/introspection.py` & `django_iris-0.2.5b2/django_iris/introspection.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/operations.py` & `django_iris-0.2.5b2/django_iris/operations.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/schema.py` & `django_iris-0.2.5b2/django_iris/schema.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris/utils.py` & `django_iris-0.2.5b2/django_iris/utils.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/django_iris.egg-info/PKG-INFO` & `django_iris-0.2.5b2/django_iris.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iris
-Version: 0.2.5b1
+Version: 0.2.5b2
 Summary: Django backend for InterSystems IRIS
 Home-page: https://github.com/caretdev/django-iris
 Maintainer: CaretDev
 Maintainer-email: dmitry@caretdev.com
 License: MIT
 Project-URL: Source, https://github.com/caretdev/django-iris
 Project-URL: Tracker, https://github.com/caretdev/django-iris/issues
```

### Comparing `django_iris-0.2.5b1/django_iris.egg-info/SOURCES.txt` & `django_iris-0.2.5b2/django_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_BufferWriter.py` & `django_iris-0.2.5b2/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_ConnectionInformation.py` & `django_iris-0.2.5b2/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_ConnectionParameters.py` & `django_iris-0.2.5b2/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_Constant.py` & `django_iris-0.2.5b2/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_DBList.py` & `django_iris-0.2.5b2/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_Device.py` & `django_iris-0.2.5b2/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_GatewayContext.py` & `django_iris-0.2.5b2/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_GatewayUtility.py` & `django_iris-0.2.5b2/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRIS.py` & `django_iris-0.2.5b2/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISConnection.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISEmbedded.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNode.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISGlobalNodeView.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISIterator.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISList.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISNative.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISObject.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_IRISReference.py` & `django_iris-0.2.5b2/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_InStream.py` & `django_iris-0.2.5b2/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_LegacyIterator.py` & `django_iris-0.2.5b2/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_ListReader.py` & `django_iris-0.2.5b2/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_ListWriter.py` & `django_iris-0.2.5b2/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_LogFileStream.py` & `django_iris-0.2.5b2/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_MessageHeader.py` & `django_iris-0.2.5b2/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_OutStream.py` & `django_iris-0.2.5b2/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_PrintStream.py` & `django_iris-0.2.5b2/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_PythonGateway.py` & `django_iris-0.2.5b2/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/_SharedMemorySocket.py` & `django_iris-0.2.5b2/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/__init__.py` & `django_iris-0.2.5b2/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_Column.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_DBAPI.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_DBAPI.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_Descriptor.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_IRISStream.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_Message.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_Parameter.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_ParameterCollection.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_ResultSetRow.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/_SQLType.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_PreParser.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Scanner.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_Token.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/dbapi/preparser/_TokenList.py` & `django_iris-0.2.5b2/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessHost.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessOperation.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessProcess.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_BusinessService.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_Common.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_Director.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_IRISBusinessService.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_IRISOutboundAdapter.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_InboundAdapter.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/_OutboundAdapter.py` & `django_iris-0.2.5b2/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/intersystems_iris/pex/__init__.py` & `django_iris-0.2.5b2/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/irisnative/_IRISNative.py` & `django_iris-0.2.5b2/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `django_iris-0.2.5b1/setup.cfg` & `django_iris-0.2.5b2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-iris
-version = 0.2.5b1
+version = 0.2.5b2
 url = https://github.com/caretdev/django-iris
 maintainer = CaretDev
 maintainer_email = dmitry@caretdev.com
 license = MIT
 description = Django backend for InterSystems IRIS
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `django_iris-0.2.5b1/setup.py` & `django_iris-0.2.5b2/setup.py`

 * *Files identical despite different names*

