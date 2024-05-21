# Comparing `tmp/rucio_clients-34.3.0.tar.gz` & `tmp/rucio_clients-34.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio_clients-34.3.0.tar", last modified: Mon May  6 12:44:10 2024, max compression
+gzip compressed data, was "rucio_clients-34.4.0.tar", last modified: Tue May 21 14:54:26 2024, max compression
```

## Comparing `rucio_clients-34.3.0.tar` & `rucio_clients-34.4.0.tar`

### file list

```diff
@@ -1,204 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.743766 rucio_clients-34.3.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-06 12:44:07.000000 rucio_clients-34.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-06 12:44:10.743766 rucio_clients-34.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.709766 rucio_clients-34.3.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/bin/rucio-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.710766 rucio_clients-34.3.0/etc/
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.3.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/etc/rucio.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.707766 rucio_clients-34.3.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.711766 rucio_clients-34.3.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.715766 rucio_clients-34.3.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16352 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    48007 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86094 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27121 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12734 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46627 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.718766 rucio_clients-34.3.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24636 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     5507 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/didtype.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45296 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6071 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.720766 rucio_clients-34.3.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5384 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18523 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15885 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5427 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79121 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.720766 rucio_clients-34.3.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.723766 rucio_clients-34.3.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7199 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29100 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9730 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3411 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10400 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22703 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15260 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5501 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14655 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17473 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8127 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22168 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12571 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/rse/rsemanager.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-05-06 11:04:02.000000 rucio_clients-34.3.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.741766 rucio_clients-34.3.0/lib/rucio_clients.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5205 2024-05-06 12:44:10.000000 rucio_clients-34.3.0/lib/rucio_clients.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     4349 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5235 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-06 12:44:10.745766 rucio_clients-34.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-06 12:44:07.000000 rucio_clients-34.3.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.741766 rucio_clients-34.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15923 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    14964 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23265 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96724 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23870 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7728 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28183 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10869 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5821 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57290 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20429 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54332 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108359 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7662 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62453 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38868 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22796 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17257 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13033 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75080 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8940 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91949 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48389 2024-05-06 11:03:53.000000 rucio_clients-34.3.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8924 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15575 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:10.741766 rucio_clients-34.3.0/tools/
--rw-r--r--   0 root         (0) root         (0)     6163 2024-05-06 09:19:47.000000 rucio_clients-34.3.0/tools/merge_rucio_configs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.463628 rucio_clients-34.4.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-21 14:54:22.000000 rucio_clients-34.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-21 14:54:26.463628 rucio_clients-34.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.425627 rucio_clients-34.4.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/bin/rucio-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.426627 rucio_clients-34.4.0/etc/
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio_clients-34.4.0/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio_clients-34.4.0/etc/rucio.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.422627 rucio_clients-34.4.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.426627 rucio_clients-34.4.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.431627 rucio_clients-34.4.0/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16352 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    48035 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    87520 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19518 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27121 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12734 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46627 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.435627 rucio_clients-34.4.0/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24636 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/didtype.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45338 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.437627 rucio_clients-34.4.0/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79163 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.437627 rucio_clients-34.4.0/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.441627 rucio_clients-34.4.0/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29100 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10414 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    21937 2024-05-21 07:56:16.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14689 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17473 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22448 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37238 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/rse/rsemanager.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-21 12:45:12.000000 rucio_clients-34.4.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.461628 rucio_clients-34.4.0/lib/rucio_clients.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5117 2024-05-21 14:54:26.000000 rucio_clients-34.4.0/lib/rucio_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio_clients-34.4.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     5763 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-21 14:54:26.464628 rucio_clients-34.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-21 14:54:22.000000 rucio_clients-34.4.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.461628 rucio_clients-34.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62467 2024-05-21 07:56:54.000000 rucio_clients-34.4.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    42098 2024-05-21 07:16:09.000000 rucio_clients-34.4.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-21 09:35:26.000000 rucio_clients-34.4.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15575 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:26.461628 rucio_clients-34.4.0/tools/
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-05-16 07:28:57.000000 rucio_clients-34.4.0/tools/merge_rucio_configs.py
```

### Comparing `rucio_clients-34.3.0/AUTHORS.rst` & `rucio_clients-34.4.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/LICENSE` & `rucio_clients-34.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/MANIFEST.in` & `rucio_clients-34.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/PKG-INFO` & `rucio_clients-34.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio-clients
-Version: 34.3.0
+Version: 34.4.0
 Summary: Rucio Client Lite Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio_clients-34.3.0/README.rst` & `rucio_clients-34.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/bin/rucio` & `rucio_clients-34.4.0/bin/rucio`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/bin/rucio-admin` & `rucio_clients-34.4.0/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/etc/rse-accounts.cfg.template` & `rucio_clients-34.4.0/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/etc/rucio.cfg.atlas.client.template` & `rucio_clients-34.4.0/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/etc/rucio.cfg.template` & `rucio_clients-34.4.0/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/__init__.py` & `rucio_clients-34.4.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/alembicrevision.py` & `rucio_clients-34.4.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/__init__.py` & `rucio_clients-34.4.0/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/accountclient.py` & `rucio_clients-34.4.0/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/accountlimitclient.py` & `rucio_clients-34.4.0/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/baseclient.py` & `rucio_clients-34.4.0/lib/rucio/client/baseclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
 class BaseClient:
 
     """Main client class for accessing Rucio resources. Handles the authentication."""
 
     AUTH_RETRIES, REQUEST_RETRIES = 2, 3
     TOKEN_PATH_PREFIX = get_tmp_dir() + '/.rucio_'
-    TOKEN_PREFIX = 'auth_token_'
-    TOKEN_EXP_PREFIX = 'auth_token_exp_'
+    TOKEN_PREFIX = 'auth_token_'  # noqa: S105
+    TOKEN_EXP_PREFIX = 'auth_token_exp_'  # noqa: S105
 
     def __init__(self,
                  rucio_host: Optional[str] = None,
                  auth_host: Optional[str] = None,
                  account: Optional[str] = None,
                  ca_cert: Optional[str] = None,
                  auth_type: Optional[str] = None,
```

### Comparing `rucio_clients-34.3.0/lib/rucio/client/client.py` & `rucio_clients-34.4.0/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/configclient.py` & `rucio_clients-34.4.0/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/credentialclient.py` & `rucio_clients-34.4.0/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/didclient.py` & `rucio_clients-34.4.0/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/diracclient.py` & `rucio_clients-34.4.0/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/downloadclient.py` & `rucio_clients-34.4.0/lib/rucio/client/downloadclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import secrets
 import shutil
 import signal
 import subprocess
 import time
 from queue import Empty, Queue, deque
 from threading import Thread
+from typing import Any, Optional
 
 from rucio import version
 from rucio.client.client import Client
 from rucio.common.config import config_get
 from rucio.common.didtype import DID
 from rucio.common.exception import InputValidationError, NoFilesDownloaded, NotAllFilesDownloaded, RucioException
 from rucio.common.pcache import Pcache
@@ -170,15 +171,22 @@
         self.extraction_tools.append(BaseExtractionTool('unzip', '-v', extract_args, logger=self.logger))
 
         # tar -C <dest_dir_path> -xf <archive_file_path>  <did_name>
         extract_args = '-C %(dest_dir_path)s -xf %(archive_file_path)s %(file_to_extract)s'
         self.extraction_tools.append(BaseExtractionTool('tar', '--version', extract_args, logger=self.logger))
         self.extract_scope_convention = config_get('common', 'extract_scope', False, None)
 
-    def download_pfns(self, items, num_threads=2, trace_custom_fields={}, traces_copy_out=None, deactivate_file_download_exceptions=False):
+    def download_pfns(
+        self,
+        items: list[dict[str, Any]],
+        num_threads: int = 2,
+        trace_custom_fields: Optional[dict[str, Any]] = None,
+        traces_copy_out: Optional[list[dict[str, Any]]] = None,
+        deactivate_file_download_exceptions: bool = False
+    ) -> list[dict[str, Any]]:
         """
         Download items with a given PFN. This function can only download files, no datasets.
 
         :param items: List of dictionaries. Each dictionary describing a file to download. Keys:
             pfn                            - PFN string of this file
             did                            - DID string of this file (e.g. 'scope:file.name'). Wildcards are not allowed
             rse                            - rse name (e.g. 'CERN-PROD_DATADISK'). RSE Expressions are not allowed
@@ -198,14 +206,15 @@
                   clientState can be one of the following: ALREADY_DONE, DONE, FILE_NOT_FOUND, FAIL_VALIDATE, FAILED
 
         :raises InputValidationError: if one of the input items is in the wrong format
         :raises NoFilesDownloaded: if no files could be downloaded
         :raises NotAllFilesDownloaded: if not all files could be downloaded
         :raises RucioException: if something unexpected went wrong during the download
         """
+        trace_custom_fields = trace_custom_fields or {}
         logger = self.logger
         trace_custom_fields['uuid'] = generate_uuid()
 
         logger(logging.INFO, 'Processing %d item(s) for input' % len(items))
         input_items = []
         for item in items:
             did_str = item.get('did')
@@ -246,16 +255,23 @@
         num_files_out = len(output_items)
 
         if not deactivate_file_download_exceptions and num_files_in != num_files_out:
             raise RucioException('%d items were in the input queue but only %d are in the output queue' % (num_files_in, num_files_out))
 
         return self._check_output(output_items, deactivate_file_download_exceptions=deactivate_file_download_exceptions)
 
-    def download_dids(self, items, num_threads=2, trace_custom_fields={}, traces_copy_out=None,
-                      deactivate_file_download_exceptions=False, sort=None):
+    def download_dids(
+        self,
+        items: list[dict[str, Any]],
+        num_threads: int = 2,
+        trace_custom_fields: Optional[dict[str, Any]] = None,
+        traces_copy_out: Optional[list[dict[str, Any]]] = None,
+        deactivate_file_download_exceptions: bool = False,
+        sort: Optional[str] = None
+    ) -> list[dict[str, Any]]:
         """
         Download items with given DIDs. This function can also download datasets and wildcarded DIDs.
 
         :param items: List of dictionaries. Each dictionary describing an item to download. Keys:
             did                            - DID string of this file (e.g. 'scope:file.name')
             filters                        - Filter to select DIDs for download. Optional if DID is given
             rse                            - Optional: rse name (e.g. 'CERN-PROD_DATADISK') or rse expression from where to download
@@ -282,14 +298,15 @@
         :returns: a list of dictionaries with an entry for each file, containing the input options, the did, and the clientState
 
         :raises InputValidationError: if one of the input items is in the wrong format
         :raises NoFilesDownloaded: if no files could be downloaded
         :raises NotAllFilesDownloaded: if not all files could be downloaded
         :raises RucioException: if something unexpected went wrong during the download
         """
+        trace_custom_fields = trace_custom_fields or {}
         logger = self.logger
         trace_custom_fields['uuid'] = generate_uuid()
 
         logger(logging.INFO, 'Processing %d item(s) for input' % len(items))
         did_to_input_items, file_items_with_sources = self._resolve_and_merge_input_items(copy.deepcopy(items), sort=sort)
         self.logger(logging.DEBUG, 'num_unmerged_items=%d; num_dids=%d; num_file_items=%d' % (len(items), len(did_to_input_items), len(file_items_with_sources)))
 
@@ -300,15 +317,23 @@
         num_files_out = len(output_items)
 
         if not deactivate_file_download_exceptions and num_files_in != num_files_out:
             raise RucioException('%d items were in the input queue but only %d are in the output queue' % (num_files_in, num_files_out))
 
         return self._check_output(output_items, deactivate_file_download_exceptions=deactivate_file_download_exceptions)
 
-    def download_from_metalink_file(self, item, metalink_file_path, num_threads=2, trace_custom_fields={}, traces_copy_out=None, deactivate_file_download_exceptions=False):
+    def download_from_metalink_file(
+        self,
+        item: dict[str, Any],
+        metalink_file_path: str,
+        num_threads: int = 2,
+        trace_custom_fields: Optional[dict[str, Any]] = None,
+        traces_copy_out: Optional[list[dict[str, Any]]] = None,
+        deactivate_file_download_exceptions: bool = False
+    ) -> list[dict[str, Any]]:
         """
         Download items using a given metalink file.
 
         :param item: dictionary describing an item to download. Keys:
             base_dir                       - Optional: base directory where the downloaded files will be stored. (Default: '.')
             no_subdir                      - Optional: If true, files are written directly into base_dir. (Default: False)
             ignore_checksum                - Optional: If true, skips the checksum validation between the downloaded file and the rucio catalouge. (Default: False)
@@ -323,14 +348,15 @@
         :returns: a list of dictionaries with an entry for each file, containing the input options, the did, and the clientState
 
         :raises InputValidationError: if one of the input items is in the wrong format
         :raises NoFilesDownloaded: if no files could be downloaded
         :raises NotAllFilesDownloaded: if not all files could be downloaded
         :raises RucioException: if something unexpected went wrong during the download
         """
+        trace_custom_fields = trace_custom_fields or {}
         logger = self.logger
 
         logger(logging.INFO, 'Getting sources from metalink file')
         metalinks = parse_replicas_from_file(metalink_file_path)
 
         trace_custom_fields['uuid'] = generate_uuid()
 
@@ -347,26 +373,33 @@
         num_files_out = len(output_items)
 
         if not deactivate_file_download_exceptions and num_files_in != num_files_out:
             raise RucioException('%d items were in the input queue but only %d are in the output queue' % (num_files_in, num_files_out))
 
         return self._check_output(output_items, deactivate_file_download_exceptions=deactivate_file_download_exceptions)
 
-    def _download_multithreaded(self, input_items, num_threads, trace_custom_fields={}, traces_copy_out=None):
+    def _download_multithreaded(
+        self,
+        input_items: list[dict[str, Any]],
+        num_threads: int,
+        trace_custom_fields: Optional[dict[str, Any]] = None,
+        traces_copy_out: Optional[list[dict[str, Any]]] = None
+    ) -> list[dict[str, Any]]:
         """
         Starts an appropriate number of threads to download items from the input list.
         (This function is meant to be used as class internal only)
 
         :param input_items: list containing the input items to download
         :param num_threads: suggestion of how many threads should be started
         :param trace_custom_fields: Custom key value pairs to send with the traces
         :param traces_copy_out: reference to an external list, where the traces should be uploaded
 
         :returns: list with output items as dictionaries
         """
+        trace_custom_fields = trace_custom_fields or {}
         logger = self.logger
 
         num_files = len(input_items)
         nlimit = 5
         num_threads = max(1, num_threads)
         num_threads = min(num_files, num_threads, nlimit)
 
@@ -726,15 +759,22 @@
 
             if not item.get('shall_keep_archive'):
                 logger(logging.DEBUG, '%sDeleting archive %s' % (log_prefix, did_name))
                 os.remove(archive_file_path)
 
         return item
 
-    def download_aria2c(self, items, trace_custom_fields={}, filters={}, deactivate_file_download_exceptions=False, sort=None):
+    def download_aria2c(
+        self,
+        items: list[dict[str, Any]],
+        trace_custom_fields: Optional[dict[str, Any]] = None,
+        filters: Optional[dict[str, Any]] = None,
+        deactivate_file_download_exceptions: bool = False,
+        sort: Optional[str] = None
+    ) -> list[dict[str, Any]]:
         """
         Uses aria2c to download the items with given DIDs. This function can also download datasets and wildcarded DIDs.
         It only can download files that are available via https/davs.
         Aria2c needs to be installed and X509_USER_PROXY needs to be set!
 
         :param items: List of dictionaries. Each dictionary describing an item to download. Keys:
             did                            - DID string of this file (e.g. 'scope:file.name'). Wildcards are not allowed
@@ -756,14 +796,16 @@
         :returns: a list of dictionaries with an entry for each file, containing the input options, the did, and the clientState
 
         :raises InputValidationError: if one of the input items is in the wrong format
         :raises NoFilesDownloaded: if no files could be downloaded
         :raises NotAllFilesDownloaded: if not all files could be downloaded
         :raises RucioException: if something went wrong during the download (e.g. aria2c could not be started)
         """
+        trace_custom_fields = trace_custom_fields or {}
+        filters = filters or {}
         logger = self.logger
         trace_custom_fields['uuid'] = generate_uuid()
 
         rpc_secret = '%x' % (secrets.randbits(64))
         rpc_auth = 'token:%s' % rpc_secret
         rpcproc, aria_rpc = self._start_aria2c_rpc(rpc_secret)
 
@@ -856,27 +898,34 @@
         try:
             aria_rpc = RPCServerProxy('http://localhost:%d/rpc' % port)
         except Exception as error:
             rpcproc.kill()
             raise RucioException('Failed to initialise rpc proxy!', error)
         return (rpcproc, aria_rpc)
 
-    def _download_items_aria2c(self, items, aria_rpc, rpc_auth, trace_custom_fields={}):
+    def _download_items_aria2c(
+        self,
+        items: list[dict[str, Any]],
+        aria_rpc: Any,
+        rpc_auth: str,
+        trace_custom_fields: Optional[dict[str, Any]] = None
+    ) -> list[dict[str, Any]]:
         """
         Uses aria2c to download the given items. Aria2c needs to be started
         as RPC background process first and a RPC proxy is needed.
         (This function is meant to be used as class internal only)
 
         :param items: list of dictionaries containing one dict for each file to download
         :param aria_rcp: RPCProxy to the aria2c process
         :param rpc_auth: the rpc authentication token
         :param trace_custom_fields: Custom key value pairs to send with the traces
 
         :returns: a list of dictionaries with an entry for each file, containing the input options, the did, and the clientState
         """
+        trace_custom_fields = trace_custom_fields or {}
         logger = self.logger
 
         gid_to_item = {}  # maps an aria2c download id (gid) to the download item
         pfn_to_rse = {}
         items_to_queue = [item for item in items]
 
         # items get removed from gid_to_item when they are complete or failed
```

### Comparing `rucio_clients-34.3.0/lib/rucio/client/exportclient.py` & `rucio_clients-34.4.0/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/fileclient.py` & `rucio_clients-34.4.0/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/importclient.py` & `rucio_clients-34.4.0/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/lifetimeclient.py` & `rucio_clients-34.4.0/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/lockclient.py` & `rucio_clients-34.4.0/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/metaconventionsclient.py` & `rucio_clients-34.4.0/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/pingclient.py` & `rucio_clients-34.4.0/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/replicaclient.py` & `rucio_clients-34.4.0/lib/rucio/client/replicaclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from datetime import datetime
 from json import dumps, loads
+from typing import Any, Optional
 from urllib.parse import quote_plus
 
 from requests.status_codes import codes
 
 from rucio.client.baseclient import BaseClient, choice
 from rucio.common.utils import build_url, chunks, render_json
 
@@ -229,15 +230,25 @@
                         path='/'.join([self.REPLICAS_BASEURL, 'suspicious']))
         r = self._send_request(url, type_='GET', params=params)
         if r.status_code == codes.ok:
             return self._load_json_data(r)
         exc_cls, exc_msg = self._get_exception(headers=r.headers, status_code=r.status_code, data=r.content)
         raise exc_cls(exc_msg)
 
-    def add_replica(self, rse, scope, name, bytes_, adler32, pfn=None, md5=None, meta={}):
+    def add_replica(
+        self,
+        rse: str,
+        scope: str,
+        name: str,
+        bytes_: int,
+        adler32: str,
+        pfn: Optional[str] = None,
+        md5: Optional[str] = None,
+        meta: Optional[dict[str, Any]] = None
+    ) -> bool:
         """
         Add file replicas to a RSE.
 
         :param rse: the RSE name.
         :param scope: The scope of the file.
         :param name: The name of the file.
         :param bytes_: The size in bytes.
@@ -245,14 +256,15 @@
         :param pfn: PFN of the file for non deterministic RSE.
         :param md5: md5 checksum.
         :param meta: Metadata attributes.
 
         :return: True if files were created successfully.
 
         """
+        meta = meta or {}
         dict_ = {'scope': scope, 'name': name, 'bytes': bytes_, 'meta': meta, 'adler32': adler32}
         if md5:
             dict_['md5'] = md5
         if pfn:
             dict_['pfn'] = pfn
         return self.add_replicas(rse=rse, files=[dict_])
```

### Comparing `rucio_clients-34.3.0/lib/rucio/client/requestclient.py` & `rucio_clients-34.4.0/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/rseclient.py` & `rucio_clients-34.4.0/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/ruleclient.py` & `rucio_clients-34.4.0/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/scopeclient.py` & `rucio_clients-34.4.0/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/subscriptionclient.py` & `rucio_clients-34.4.0/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/touchclient.py` & `rucio_clients-34.4.0/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/client/uploadclient.py` & `rucio_clients-34.4.0/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/__init__.py` & `rucio_clients-34.4.0/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/cache.py` & `rucio_clients-34.4.0/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/config.py` & `rucio_clients-34.4.0/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/constants.py` & `rucio_clients-34.4.0/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/constraints.py` & `rucio_clients-34.4.0/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/didtype.py` & `rucio_clients-34.4.0/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/exception.py` & `rucio_clients-34.4.0/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/extra.py` & `rucio_clients-34.4.0/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/logging.py` & `rucio_clients-34.4.0/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/pcache.py` & `rucio_clients-34.4.0/lib/rucio/common/pcache.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,15 +525,15 @@
             # Leave one '/' on dst
             while ((len(self.dst) > 1) and (self.dst[1] == '/')):
                 self.dst_prefix += '/'
                 self.dst = self.dst[1:]
 
         # Execute original command, no further action
         if (not (self.dst.startswith(self.scratch_dir) and self.accept(self.src) and (not self.reject(self.src)))):
-            os.execvp(self.copy_util, self.args)
+            os.execvp(self.copy_util, self.args)  # noqa: S606
             os._exit(1)
 
         # XXXX todo:  fast-path - try to acquire lock
         # first, if that succeeds, don't call
         # create_pcache_dst_dir
 
         # load file into pcache
@@ -678,15 +678,15 @@
         self.pcache_dst_dir = d
         status = self.mkdir_p(d)
         if (status):
             self.log(ERROR, "mkdir %s %s", d, status)
             self.fail(103)
 
     def get_disk_usage(self):
-        p = os.popen("df -P %s | tail -1" % self.pcache_dir, 'r')
+        p = os.popen("df -P %s | tail -1" % self.pcache_dir, 'r')  # noqa: S605
         data = p.read()
         status = p.close()
         if status:
             self.log(ERROR, "get_disk_usage: df command failed, status=%s", status)
             sys.exit(1)
         tok = data.split()
         percent = tok[-2]
@@ -768,15 +768,15 @@
             self.panda_flush_cache()
         self.reset_stats()
         ts = '.' + str(time.time())
         for d in "CACHE", "MRU":
             d = self.pcache_dir + d
             try:
                 os.rename(d, d + ts)
-                os.system("rm -rf %s &" % (d + ts))
+                os.system("rm -rf %s &" % (d + ts))  # noqa: S605
             except OSError as e:
                 if e.errno != errno.ENOENT:
                     self.log(ERROR, "%s: %s", d, e)
 
     def do_transfer(self):
 
         # Cache file and transfer file locations
```

### Comparing `rucio_clients-34.3.0/lib/rucio/common/plugins.py` & `rucio_clients-34.4.0/lib/rucio/common/plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/policy.py` & `rucio_clients-34.4.0/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/__init__.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/atlas.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/belleii.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/cms.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/generic.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,49 +31,40 @@
 
 ACCOUNT_TYPE = {"description": "Account type",
                 "type": "string",
                 "enum": ["USER", "GROUP", "SERVICE"]}
 
 ACTIVITY = {"description": "Activity name",
             "type": "string",
-            "enum": ["Data Brokering", "Data Consolidation", "Data rebalancing",
+            "enum": ["Data Brokering", "Data Consolidation", "Data Rebalancing",
                      "Debug", "Express", "Functional Test", "Group Subscriptions",
                      "Production Input", "Production Output",
                      "Analysis Input", "Analysis Output", "Staging",
                      "T0 Export", "T0 Tape", "Upload/Download (Job)",
                      "Upload/Download (User)", "User Subscriptions", "Data Challenge"]}
 
 SCOPE_LENGTH = 25
 
 SCOPE = {"description": "Scope name",
          "type": "string",
-         "pattern": r"^(cms)|(logs)|(user\.[a-z0-9-_]{1,%s})$" % (SCOPE_LENGTH - len('user.'))}
+         "pattern": "^[a-zA-Z_\\-.0-9]{1,%s}$" % SCOPE_LENGTH}
 
 R_SCOPE = {"description": "Scope name",
            "type": "string",
            "pattern": "\\w"}
 
-CMS_LFN_LENGTH = 500
-CMS_DATASET_CORE = r'/[a-zA-Z0-9\-_]{1,99}/[a-zA-Z0-9\.\-_]{1,199}/[A-Z\-]{1,50}'
-CMS_BLOCK_PART = r'[a-zA-Z0-9\.\-_]{1,100}'
-
-CMS_DATASET = r'^%s$' % CMS_DATASET_CORE
-CMS_BLOCK = r'^%s#%s$' % (CMS_DATASET_CORE, CMS_BLOCK_PART)  # Valid dataset name and block separated by #
-CMS_LFN = r'^\/store\/[A-Za-z0-9][A-Za-z0-9\.\-\_\/]{1,%s}$' % (CMS_LFN_LENGTH - len('/store/'))
-
-CMS_BLOCK_LENGTH = 100 + 200 + 51 + 101
+NAME_LENGTH = 250
 
 NAME = {"description": "Data Identifier name",
         "type": "string",
-        "pattern": r"%s|%s|%s" % (CMS_DATASET, CMS_BLOCK, CMS_LFN)}
-
-NAME_LENGTH = max(CMS_LFN_LENGTH, CMS_BLOCK_LENGTH)
+        "pattern": "^[A-Za-z0-9][A-Za-z0-9\\.\\-\\_]{1,%s}$" % NAME_LENGTH}
 
-# read name
-R_NAME = NAME
+R_NAME = {"description": "Data Identifier name",
+          "type": "string",
+          "pattern": "\\w"}
 
 LOCKED = {"description": "Rule locked status",
           "type": ["boolean", "null"]}
 
 ASK_APPROVAL = {"description": "Rule approval request",
                 "type": ["boolean", "null"]}
 
@@ -87,23 +78,23 @@
                   "type": "boolean"}
 
 IGNORE_AVAILABILITY = {"description": "Rule ignore availability status",
                        "type": "boolean"}
 
 RSE = {"description": "RSE name",
        "type": "string",
-       "pattern": "^T[0-3]_[A-Z]{2}((_[A-Za-z0-9]+)+)$"}
+       "pattern": "^([A-Z0-9]+([_-][A-Z0-9]+)*)$"}
 
 RSE_ATTRIBUTE = {"description": "RSE attribute",
                  "type": "string",
                  "pattern": r'([A-Za-z0-9\._-]+[=<>][A-Za-z0-9_-]+)'}
 
 DEFAULT_RSE_ATTRIBUTE = {"description": "Default RSE attribute",
                          "type": "string",
-                         "pattern": r'([A-Z0-9]+([_-][A-Za-z0-9]+)*)'}
+                         "pattern": r'([A-Z0-9]+([_-][A-Z0-9]+)*)'}
 
 REPLICA_STATE = {"description": "Replica state",
                  "type": "string",
                  "enum": ["AVAILABLE", "UNAVAILABLE", "COPYING", "BEING_DELETED", "BAD", "SOURCE", "A", "U", "C", "B", "D", "S"]}
 
 DATE = {"description": "Date",
         "type": "string",
@@ -168,14 +159,41 @@
 
 PRIORITY = {"description": "Priority of the transfers",
             "type": "integer"}
 
 SPLIT_CONTAINER = {"description": "Rule split container mode",
                    "type": ["boolean", "null"]}
 
+TIME_ENTRY = {
+    "description": "Datetime, ISO 8601",
+    "type": "string",
+    "pattern": r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}.\d*$'
+}
+
+IP = {
+    "description": "Internet Protocol address v4, RFC 791",
+    "type": "string",
+    "pattern": r'^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(\.|$)){4}$'
+}
+
+IPv4orIPv6 = {
+    "description": "IPv4 or IPv6 address",
+    "type": "string",
+    "format": "ipv4_or_ipv6"
+}
+
+CLIENT_STATE = {
+    "description": "Client state",
+    "type": "string",
+    "enum": ['DONE', 'FAILED', 'PROCESSING', 'ALREADY_DONE', 'FILE_NOT_FOUND', 'FOUND_IN_PCACHE', 'DOWNLOAD_ATTEMPT',
+             'FAIL_VALIDATE', 'FOUND_ROOT', 'ServiceUnavailable', 'SERVICE_ERROR', 'CP_TIMEOUT', 'COPY_ERROR',
+             'STAGEIN_ATTEMPT_FAILED', 'SourceNotFound', 'MISSINGOUTPUTFILE', 'MD_MISMATCH', 'CHECKSUMCALCULATIONFAILURE',
+             'MISSINGINPUT', 'MISSING_INPUT']
+}
+
 RULE = {"description": "Replication rule",
         "type": "object",
         "properties": {"dids": {"type": "array"},
                        "account": ACCOUNT,
                        "copies": COPIES,
                        "rse_expression": RSE_EXPRESSION,
                        "grouping": GROUPING,
@@ -220,47 +238,27 @@
 
 COLLECTIONS = {"description": "Array of datasets or containers",
                "type": "array",
                "items": COLLECTION,
                "minItems": 1,
                "maxItems": 1000}
 
-# No else if in JSON Schema
-# if type == container
-#      must match CMS dataset/container guidelines
-# else if type == dataset
-#      must match CMS block guidelines
-# else if type == file
-#      must match CMS LFN guidelines
-#      CMS scope must not be in /store/user
-#      user.jdoe scope must be in /store/user/rucio
-#         (making sure it's in /store/user/rucio/jdoe seems to be impossible in JSON Schema, handled outside)
 DID = {"description": "Data Identifier(DID)",
        "type": "object",
        "properties": {"scope": SCOPE,
                       "name": NAME,
                       "type": DID_TYPE,
                       "meta": META,
                       "rules": RULES,
                       "bytes": BYTES,
                       "adler32": ADLER32,
                       "md5": MD5,
                       "state": REPLICA_STATE,
                       "pfn": PFN},
-       "allOf": [
-           {"if": {"properties": {"type": {"const": "CONTAINER"}}},
-            "then": {"properties": {"name": {"pattern": CMS_DATASET}}}},
-           {"if": {"properties": {"type": {"const": "DATASET"}}},
-            "then": {"properties": {"name": {"pattern": CMS_BLOCK}}}},
-           {"if": {"properties": {"type": {"const": "FILE"}}},
-            "then": {"properties": {"name": {"pattern": CMS_LFN}}}},
-           {"if": {"properties": {"type": {"const": "F"}}},
-            "then": {"properties": {"name": {"pattern": CMS_LFN}}}},
-       ],
-       "required": ["scope", "name", "type"],
+       "required": ["scope", "name"],
        "additionalProperties": False}
 
 DID_FILTERS = {"description": "Array to filter DIDs by metadata",
                "type": "array",
                "additionalProperties": True}
 
 R_DID = {"description": "Data Identifier(DID)",
@@ -278,38 +276,38 @@
          "required": ["scope", "name"],
          "additionalProperties": False}
 
 DIDS = {"description": "Array of Data Identifiers(DIDs)",
         "type": "array",
         "items": DID,
         "minItems": 1,
-        "maxItems": 3000}  # Was 1000
+        "maxItems": 1000}
 
 R_DIDS = {"description": "Array of Data Identifiers(DIDs)",
           "type": "array",
           "items": R_DID,
           "minItems": 1,
-          "maxItems": 30000}
+          "maxItems": 1000}
 
 ATTACHMENT = {"description": "Attachement",
               "type": "object",
               "properties": {"scope": SCOPE,
                              "name": NAME,
                              "rse": {"description": "RSE name",
                                      "type": ["string", "null"],
-                                     "pattern": "^T[0-3]_[A-Z]{2}((_[A-Za-z0-9]+)+)$"},
-                             "dids": R_DIDS},  # Loosen up, we're not creating these DIDs
+                                     "pattern": "^([A-Z0-9]+([_-][A-Z0-9]+)*)$"},
+                             "dids": DIDS},
               "required": ["dids"],
               "additionalProperties": False}
 
 ATTACHMENTS = {"description": "Array of attachments",
                "type": "array",
                "items": ATTACHMENT,
                "minItems": 1,
-               "maxItems": 3000}  # Was 1000
+               "maxItems": 1000}
 
 SUBSCRIPTION_FILTER = {"type": "object",
                        "properties": {"datatype": {"type": "array"},
                                       "prod_step": {"type": "array"},
                                       "stream_name": {"type": "array"},
                                       "project": {"type": "array"},
                                       "scope": {"type": "array"},
@@ -365,15 +363,15 @@
 MESSAGE_OPERATION = {"type": "object",
                      "properties": {'operation': {"enum": ["add_replicas", "delete_replicas"]}}}
 
 ACCOUNT_ATTRIBUTE = {"description": "Account attribute",
                      "type": "string",
                      "pattern": r'^[a-zA-Z0-9-_\\/\\.]{1,30}$'}
 
-SCOPE_NAME_REGEXP = '/([^/]*)(?=/)(.*)'
+SCOPE_NAME_REGEXP = '/(.*)/(.*)'
 
 DISTANCE = {"description": "RSE distance",
             "type": "object",
             "properties": {
                 "src_rse_id": {"type": "string"},
                 "dest_rse_id": {"type": "string"},
                 "ranking": {"type": "integer"}
@@ -426,52 +424,7 @@
     :param obj: The object to validate.
     """
     try:
         if obj:
             validate(obj, SCHEMAS.get(name, {}))
     except ValidationError as error:  # NOQA, pylint: disable=W0612
         raise InvalidObject(f'Problem validating {name}: {error}')
-
-    # Apply some extra constraints to CMS DIDs
-    if name.lower() in ['did']:
-        validate_cms_did(obj)
-    elif name.lower() in ['dids']:
-        for did in obj:
-            validate_cms_did(did)
-
-
-def validate_cms_did(obj):
-    """
-    Special checking for DIDs
-    Most of the checking is done with JSON schema, but this check
-    makes sure user LFNs are in the correct /store/user/rucio/USERNAME namespace
-    makes sure group LFNs are in the correct /store/group/rucio/GROUPNAME namespace
-    """
-    if not obj:
-        return
-
-    did_type = obj['type']
-    lfn = obj['name']
-    scope = obj['scope']
-
-    if did_type != "FILE":
-        return
-
-    verify_scope_lfn_match(lfn, scope, "user")
-    verify_scope_lfn_match(lfn, scope, "group")
-
-    if scope == 'logs':
-        if not lfn.startswith('/store/logs/'):
-            raise InvalidObject(f'Problem with LFN {lfn}: Logs must start with /store/logs')
-
-
-def verify_scope_lfn_match(lfn, scope, scope_type):
-    if lfn.startswith(f'/store/{scope_type}') and not lfn.startswith(f'/store/{scope_type}/rucio/'):
-        raise InvalidObject(f"Problem with LFN {lfn} : Legacy {scope_type} files are not managed with Rucio")
-
-    if lfn.startswith(f'/store/{scope_type}/rucio') and not scope.startswith(f'{scope_type}.'):
-        raise InvalidObject(f"Problem with LFN {lfn}: Only {scope_type} scopes allowed in /store/{scope_type}/rucio")
-
-    if scope.startswith(f'{scope_type}.'):
-        _, account = scope.split('.', 1)
-        if not lfn.startswith(f'/store/{scope_type}/rucio/{account}/'):
-            raise InvalidObject(f"Problem with LFN {lfn} : Not allowed for {scope_type} {account}")
```

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/domatpc.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/escape.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/generic.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/icecube.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,40 +31,40 @@
 
 ACCOUNT_TYPE = {"description": "Account type",
                 "type": "string",
                 "enum": ["USER", "GROUP", "SERVICE"]}
 
 ACTIVITY = {"description": "Activity name",
             "type": "string",
-            "enum": ["Data Brokering", "Data Consolidation", "Data Rebalancing",
+            "enum": ["Data Brokering", "Data Consolidation", "Data rebalancing",
                      "Debug", "Express", "Functional Test", "Group Subscriptions",
                      "Production Input", "Production Output",
                      "Analysis Input", "Analysis Output", "Staging",
                      "T0 Export", "T0 Tape", "Upload/Download (Job)",
-                     "Upload/Download (User)", "User Subscriptions", "Data Challenge"]}
+                     "Upload/Download (User)", "User Subscriptions"]}
 
 SCOPE_LENGTH = 25
 
 SCOPE = {"description": "Scope name",
          "type": "string",
          "pattern": "^[a-zA-Z_\\-.0-9]{1,%s}$" % SCOPE_LENGTH}
 
 R_SCOPE = {"description": "Scope name",
            "type": "string",
            "pattern": "\\w"}
 
-NAME_LENGTH = 250
 
-NAME = {"description": "Data Identifier name",
+NAME_LENGTH = 500
+
+NAME = {"description": "IceCube Data Identifier name",
         "type": "string",
-        "pattern": "^[A-Za-z0-9][A-Za-z0-9\\.\\-\\_]{1,%s}$" % NAME_LENGTH}
+        "pattern": r"^\/[A-Za-z0-9][A-Za-z0-9\\.\\-\\_\/\#]{1,%s}$" % NAME_LENGTH}
 
-R_NAME = {"description": "Data Identifier name",
-          "type": "string",
-          "pattern": "\\w"}
+# read name
+R_NAME = NAME
 
 LOCKED = {"description": "Rule locked status",
           "type": ["boolean", "null"]}
 
 ASK_APPROVAL = {"description": "Rule approval request",
                 "type": ["boolean", "null"]}
 
@@ -159,41 +159,14 @@
 
 PRIORITY = {"description": "Priority of the transfers",
             "type": "integer"}
 
 SPLIT_CONTAINER = {"description": "Rule split container mode",
                    "type": ["boolean", "null"]}
 
-TIME_ENTRY = {
-    "description": "Datetime, ISO 8601",
-    "type": "string",
-    "pattern": r'^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}.\d*$'
-}
-
-IP = {
-    "description": "Internet Protocol address v4, RFC 791",
-    "type": "string",
-    "pattern": r'^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(\.|$)){4}$'
-}
-
-IPv4orIPv6 = {
-    "description": "IPv4 or IPv6 address",
-    "type": "string",
-    "format": "ipv4_or_ipv6"
-}
-
-CLIENT_STATE = {
-    "description": "Client state",
-    "type": "string",
-    "enum": ['DONE', 'FAILED', 'PROCESSING', 'ALREADY_DONE', 'FILE_NOT_FOUND', 'FOUND_IN_PCACHE', 'DOWNLOAD_ATTEMPT',
-             'FAIL_VALIDATE', 'FOUND_ROOT', 'ServiceUnavailable', 'SERVICE_ERROR', 'CP_TIMEOUT', 'COPY_ERROR',
-             'STAGEIN_ATTEMPT_FAILED', 'SourceNotFound', 'MISSINGOUTPUTFILE', 'MD_MISMATCH', 'CHECKSUMCALCULATIONFAILURE',
-             'MISSINGINPUT', 'MISSING_INPUT']
-}
-
 RULE = {"description": "Replication rule",
         "type": "object",
         "properties": {"dids": {"type": "array"},
                        "account": ACCOUNT,
                        "copies": COPIES,
                        "rse_expression": RSE_EXPRESSION,
                        "grouping": GROUPING,
@@ -363,15 +336,15 @@
 MESSAGE_OPERATION = {"type": "object",
                      "properties": {'operation': {"enum": ["add_replicas", "delete_replicas"]}}}
 
 ACCOUNT_ATTRIBUTE = {"description": "Account attribute",
                      "type": "string",
                      "pattern": r'^[a-zA-Z0-9-_\\/\\.]{1,30}$'}
 
-SCOPE_NAME_REGEXP = '/(.*)/(.*)'
+SCOPE_NAME_REGEXP = '/([^/]*)(?=/)(.*)'
 
 DISTANCE = {"description": "RSE distance",
             "type": "object",
             "properties": {
                 "src_rse_id": {"type": "string"},
                 "dest_rse_id": {"type": "string"},
                 "ranking": {"type": "integer"}
```

### Comparing `rucio_clients-34.3.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio_clients-34.4.0/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/stomp_utils.py` & `rucio_clients-34.4.0/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/stopwatch.py` & `rucio_clients-34.4.0/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/test_rucio_server.py` & `rucio_clients-34.4.0/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/common/types.py` & `rucio_clients-34.4.0/lib/rucio/common/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Callable
+from datetime import datetime
 from typing import TYPE_CHECKING, Any, Literal, Optional, TypedDict, Union
 
 if TYPE_CHECKING:
     from rucio.common.constants import SUPPORTED_PROTOCOLS_LITERAL
 
 
 class InternalType:
@@ -187,7 +188,20 @@
 class HopDict(TypedDict):
     source_rse_id: str
     source_scheme: "SUPPORTED_PROTOCOLS_LITERAL"
     source_scheme_priority: int
     dest_rse_id: str
     dest_scheme: "SUPPORTED_PROTOCOLS_LITERAL"
     dest_scheme_priority: int
+
+
+class TokenDict(TypedDict):
+    token: str
+    expires_at: datetime
+
+
+class TokenValidationDict(TypedDict):
+    account: Optional[InternalAccount]
+    identity: Optional[str]
+    lifetime: datetime
+    audience: Optional[str]
+    authz_scope: Optional[str]
```

### Comparing `rucio_clients-34.3.0/lib/rucio/common/utils.py` & `rucio_clients-34.4.0/lib/rucio/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1241,15 +1241,15 @@
             s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             s.connect(("8.8.8.8", 80))
             ip = s.getsockname()[0]
         except Exception:
             pass
 
     if not ip:
-        ip = '0.0.0.0'
+        ip = '0.0.0.0'  # noqa: S104
 
     site = os.environ.get('SITE_NAME',
                           os.environ.get('ATLAS_SITE_NAME',
                                          os.environ.get('OSG_SITE_NAME',
                                                         'ROAMING')))
 
     latitude = os.environ.get('RUCIO_LATITUDE')
@@ -1555,15 +1555,15 @@
 
     :param path: the path to the input file
 
     :returns: a list with a dictionary for each file
     """
     with open(path) as fp:
         try:
-            root = ElementTree.parse(fp).getroot()
+            root = ElementTree.parse(fp).getroot()  # noqa: S314
             return parse_replicas_metalink(root)
         except ElementTree.ParseError as xml_err:
             try:
                 return json.load(fp)
             except ValueError as json_err:
                 raise MetalinkJsonParsingError(path, xml_err, json_err)
 
@@ -1575,15 +1575,15 @@
     it tries to parse json.
 
     :param string: the string to parse
 
     :returns: a list with a dictionary for each file
     """
     try:
-        root = ElementTree.fromstring(string)
+        root = ElementTree.fromstring(string)  # noqa: S314
         return parse_replicas_metalink(root)
     except ElementTree.ParseError as xml_err:
         try:
             return json.loads(string)
         except ValueError as json_err:
             raise MetalinkJsonParsingError(string, xml_err, json_err)
```

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/__init__.py` & `rucio_clients-34.4.0/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/__init__.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/cache.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/dummy.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/gfal.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/globus.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/http_cache.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/mock.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/ngarc.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/posix.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/posix.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
          """
         try:
             shutil.copy(self.pfn2path(pfn), dest)
         except OSError as e:
             try:  # To check if the error happened local or remote
                 with open(dest, 'wb'):
                     pass
-                call(['rm', '-rf', dest])
+                call(['rm', '-rf', dest])  # noqa: S607
             except OSError as e:
                 if e.errno == 2:
                     raise exception.DestinationNotAccessible(e)
                 else:
                     raise exception.ServiceUnavailable(e)
             if e.errno == 2:
                 raise exception.SourceNotFound(e)
```

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/protocol.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,46 +195,24 @@
         """
         del rse
         del rse_attrs
         del protocol_attrs
 
         return '%s/%s/%s/%s' % (scope[0:7], scope[4:len(scope)], name.split('-')[0] + "-" + name.split('-')[1], name)
 
-    @staticmethod
-    def __lsst(scope, name, rse, rse_attrs, protocol_attrs):
-        """
-        LFN2PFN algorithm for Rubin-LSST in the ESCAPE project
-
-        Replace convention delimiter '__' by '/'
-        The Escape instance does use the 'generic' Rucio schema.
-
-        :param scope: Scope of the LFN (ignored)
-        :param name: File name of the LFN.
-        :param rse: RSE for PFN (ignored)
-        :param rse_attrs: RSE attributes for PFN (ignored)
-        :param protocol_attrs: RSE protocol attributes for PFN (ignored)
-        :returns: Path for use in the PFN generation.
-        """
-        del scope
-        del rse
-        del rse_attrs
-        del protocol_attrs
-        return name.replace('__', '/')
-
     @classmethod
     def _module_init_(cls):
         """
         Initialize the class object on first module load.
         """
         cls.register(cls.__hash, "hash")
         cls.register(cls.__identity, "identity")
         cls.register(cls.__ligo, "ligo")
         cls.register(cls.__belleii, "belleii")
         cls.register(cls.__xenon, "xenon")
-        cls.register(cls.__lsst, "lsst")
         policy_module = None
         try:
             policy_module = config.config_get('policy', 'lfn2pfn_module')
         except (NoOptionError, NoSectionError):
             pass
         if policy_module:
             # TODO: The import of importlib is done like this due to a dependency issue with python 2.6 and incompatibility of the module with py3.x
```

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/rclone.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/rfio.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/srm.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/srm.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,19 +169,19 @@
         Establishes the actual connection to the referred RSE.
         As a quick and dirty implementation we just use this method to check if the lcg tools are available.
         If we decide to use gfal, init should be done here.
 
         :raises RSEAccessDenied: Cannot connect.
         """
 
-        status, lcglscommand = getstatusoutput('which lcg-ls')
+        status, lcglscommand = getstatusoutput('which lcg-ls')  # noqa: S605, S607
         if status:
             raise exception.RSEAccessDenied('Cannot find lcg tools')
         endpoint_basepath = self.path2pfn(self.attributes['prefix'])
-        status, result = getstatusoutput('%s -vv $LCGVO -b --srm-timeout 60 -D srmv2 -l %s' % (lcglscommand, endpoint_basepath))
+        status, result = getstatusoutput('%s -vv $LCGVO -b --srm-timeout 60 -D srmv2 -l %s' % (lcglscommand, endpoint_basepath))  # noqa: S605
         if status:
             if result == '':
                 raise exception.RSEAccessDenied('Endpoint not reachable. lcg-ls failed with status code %s but no further details.' % (str(status)))
             else:
                 raise exception.RSEAccessDenied('Endpoint not reachable : %s' % str(result))
 
     def get(self, path, dest, transfer_timeout=None):
```

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/ssh.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/storm.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/storm.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 rcode, etag_meta = requests_etag(pfn, 300)
             except:
                 pass
             # fallback to davix
             if rcode != 207:
                 rcode, etag_meta = davix_etag(pfn, 300)
 
-            p_output = minidom.parseString(etag_meta)
+            p_output = minidom.parseString(etag_meta)  # noqa: S318
             # we need to strip off the quotation marks and the <timestamp> from the etag
             # but since we can have multiple underscores, we have to rely on the uniqueness
             # of the full LFN to make the split
             target = p_output.getElementsByTagName('d:getetag')[0].childNodes[0].nodeValue.replace('"', '')
             target_ending = '_' + target.split('_')[-1]
             target = target.split(target_ending)[0]
```

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/webdav.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/webdav.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import sys
 import xml.etree.ElementTree as ET
 from dataclasses import dataclass
-from typing import Optional
+from typing import Any, Optional
 from urllib.parse import urlparse
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.poolmanager import PoolManager
 
 from rucio.common import exception
@@ -129,15 +129,15 @@
 
         :param document: XML document to parse.
         :raises ValueError: if the XML document couldn't be parsed.
         :returns: The parsed response.
         """
 
         try:
-            xml = ET.fromstring(document)
+            xml = ET.fromstring(document)  # noqa: S314
         except ET.ParseError as ex:
             raise ValueError("Couldn't parse XML document") from ex
 
         if xml.tag != '{DAV:}multistatus':
             raise ValueError('Root element is not "{DAV:}multistatus".')
 
         files = []
@@ -147,23 +147,24 @@
         return cls(files=tuple(files))  # type: ignore
 
 
 class Default(protocol.RSEProtocol):
 
     """ Implementing access to RSEs using the webDAV protocol."""
 
-    def connect(self, credentials={}):
+    def connect(self, credentials: Optional[dict[str, Any]] = None) -> None:
         """ Establishes the actual connection to the referred RSE.
 
             :param credentials: Provides information to establish a connection
                 to the referred storage system. For WebDAV connections these are
                 ca_cert, cert, auth_type, timeout
 
             :raises RSEAccessDenied
         """
+        credentials = credentials or {}
         try:
             parse_url = urlparse(self.path2pfn(''))
             self.server = f'{parse_url.scheme}://{parse_url.netloc}'
         except KeyError:
             raise exception.RSEAccessDenied('No specified Server')
 
         try:
@@ -180,20 +181,23 @@
             self.cert = credentials['cert']
         except KeyError:
             x509 = os.getenv('X509_USER_PROXY')
             if not x509:
                 # Trying to get the proxy from the default location
                 proxy_path = '/tmp/x509up_u%s' % os.geteuid()
                 if os.path.isfile(proxy_path):
-                    x509 = proxy_path
+                    self.cert = (proxy_path, proxy_path)
                 elif self.auth_token:
+                    # If no proxy is found, we set the cert to None and use the auth_token
+                    self.cert = None
                     pass
                 else:
                     raise exception.RSEAccessDenied('X509_USER_PROXY is not set')
-            self.cert = (x509, x509)
+            else:
+                self.cert = (x509, x509)
 
         try:
             self.timeout = credentials['timeout']
         except KeyError:
             self.timeout = 300
         self.session = requests.Session()
         self.session.mount('https://', TLSHTTPAdapter())
@@ -529,15 +533,15 @@
 
         :raises ServiceUnavailable: if some generic error occurred in the library.
         """
         endpoint_basepath = self.path2pfn('')
         headers = {'Depth': '0'}
 
         try:
-            root = ET.fromstring(self.session.request('PROPFIND', endpoint_basepath, verify=False, headers=headers, cert=self.session.cert).text)
+            root = ET.fromstring(self.session.request('PROPFIND', endpoint_basepath, verify=False, headers=headers, cert=self.session.cert).text)  # noqa: S314
             usedsize = root[0][1][0].find('{DAV:}quota-used-bytes').text
             try:
                 unusedsize = root[0][1][0].find('{DAV:}quota-available-bytes').text
             except Exception:
                 print('No free space given, return -999')
                 unusedsize = -999
             totalsize = int(usedsize) + int(unusedsize)
```

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/protocols/xrootd.py` & `rucio_clients-34.4.0/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/rse/rsemanager.py` & `rucio_clients-34.4.0/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio/version.py` & `rucio_clients-34.4.0/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/lib/rucio_clients.egg-info/SOURCES.txt` & `rucio_clients-34.4.0/lib/rucio_clients.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,21 +59,19 @@
 lib/rucio/common/stopwatch.py
 lib/rucio/common/test_rucio_server.py
 lib/rucio/common/types.py
 lib/rucio/common/utils.py
 lib/rucio/common/schema/__init__.py
 lib/rucio/common/schema/atlas.py
 lib/rucio/common/schema/belleii.py
-lib/rucio/common/schema/cms.py
 lib/rucio/common/schema/domatpc.py
 lib/rucio/common/schema/escape.py
 lib/rucio/common/schema/generic.py
 lib/rucio/common/schema/generic_multi_vo.py
 lib/rucio/common/schema/icecube.py
-lib/rucio/common/schema/lsst.py
 lib/rucio/rse/__init__.py
 lib/rucio/rse/rsemanager.py
 lib/rucio/rse/protocols/__init__.py
 lib/rucio/rse/protocols/bittorrent.py
 lib/rucio/rse/protocols/cache.py
 lib/rucio/rse/protocols/dummy.py
 lib/rucio/rse/protocols/gfal.py
@@ -171,15 +169,14 @@
 tests/test_rse_protocol_srm.py
 tests/test_rse_protocol_ssh.py
 tests/test_rse_protocol_webdav.py
 tests/test_rse_protocol_xrootd.py
 tests/test_rse_selector.py
 tests/test_rucio_server.py
 tests/test_rule.py
-tests/test_schema_cms.py
 tests/test_scope.py
 tests/test_subscription.py
 tests/test_throttler.py
 tests/test_tpc.py
 tests/test_trace.py
 tests/test_transfer.py
 tests/test_transfer_plugins.py
```

### Comparing `rucio_clients-34.3.0/pylintrc` & `rucio_clients-34.4.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/requirements.txt` & `rucio_clients-34.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/setup.py` & `rucio_clients-34.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/setuputil.py` & `rucio_clients-34.4.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_abacus_account.py` & `rucio_clients-34.4.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_abacus_collection_replica.py` & `rucio_clients-34.4.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_abacus_rse.py` & `rucio_clients-34.4.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_account.py` & `rucio_clients-34.4.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_account_limits.py` & `rucio_clients-34.4.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_api_external_representation.py` & `rucio_clients-34.4.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_archive.py` & `rucio_clients-34.4.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_auditor.py` & `rucio_clients-34.4.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_auditor_hdfs.py` & `rucio_clients-34.4.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_auditor_srmdumps.py` & `rucio_clients-34.4.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_authentication.py` & `rucio_clients-34.4.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_automatix.py` & `rucio_clients-34.4.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_bad_replica.py` & `rucio_clients-34.4.0/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_bb8.py` & `rucio_clients-34.4.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_belleii.py` & `rucio_clients-34.4.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_bin_rucio.py` & `rucio_clients-34.4.0/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_boolean.py` & `rucio_clients-34.4.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_clients.py` & `rucio_clients-34.4.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_common_types.py` & `rucio_clients-34.4.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_config.py` & `rucio_clients-34.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_conveyor.py` & `rucio_clients-34.4.0/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_conveyor_submitter.py` & `rucio_clients-34.4.0/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_counter.py` & `rucio_clients-34.4.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_credential.py` & `rucio_clients-34.4.0/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_curl.py` & `rucio_clients-34.4.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_daemons.py` & `rucio_clients-34.4.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_dataset_replicas.py` & `rucio_clients-34.4.0/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_db.py` & `rucio_clients-34.4.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_did.py` & `rucio_clients-34.4.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_did_meta_plugins.py` & `rucio_clients-34.4.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_didtype.py` & `rucio_clients-34.4.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_download.py` & `rucio_clients-34.4.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_dumper.py` & `rucio_clients-34.4.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_dumper_consistency.py` & `rucio_clients-34.4.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_dumper_data_model.py` & `rucio_clients-34.4.0/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_dumper_path_parsing.py` & `rucio_clients-34.4.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_filter_engine.py` & `rucio_clients-34.4.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_heartbeat.py` & `rucio_clients-34.4.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_hermes.py` & `rucio_clients-34.4.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_identity.py` & `rucio_clients-34.4.0/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_impl_upload_download.py` & `rucio_clients-34.4.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_import_export.py` & `rucio_clients-34.4.0/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_judge_cleaner.py` & `rucio_clients-34.4.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_judge_evaluator.py` & `rucio_clients-34.4.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_judge_injector.py` & `rucio_clients-34.4.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_judge_repairer.py` & `rucio_clients-34.4.0/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_lifetime.py` & `rucio_clients-34.4.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_message.py` & `rucio_clients-34.4.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_meta_conventions.py` & `rucio_clients-34.4.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_meta_did.py` & `rucio_clients-34.4.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_module_import.py` & `rucio_clients-34.4.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_monitor.py` & `rucio_clients-34.4.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_multi_vo.py` & `rucio_clients-34.4.0/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_naming_convention.py` & `rucio_clients-34.4.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_oauthmanager.py` & `rucio_clients-34.4.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_oidc.py` & `rucio_clients-34.4.0/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_permission.py` & `rucio_clients-34.4.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_pfns.py` & `rucio_clients-34.4.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_ping.py` & `rucio_clients-34.4.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_preparer.py` & `rucio_clients-34.4.0/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_qos.py` & `rucio_clients-34.4.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_quarantined_replica.py` & `rucio_clients-34.4.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_reaper.py` & `rucio_clients-34.4.0/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_redirect.py` & `rucio_clients-34.4.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_replica.py` & `rucio_clients-34.4.0/tests/test_replica.py`

 * *Files 0% similar despite different names*

```diff
@@ -1205,15 +1205,15 @@
         # for metalink, this builds the incomplete XML that should be returned by the API on error
         metalink = ''
         for line in list_replicas_on_api():
             metalink += line
         assert metalink
         print(metalink)
         with pytest.raises(ElementTree.ParseError):
-            ElementTree.fromstring(metalink)
+            ElementTree.fromstring(metalink)  # noqa: S314
 
     elif content_type == Mime.JSON_STREAM:
         # for the json stream mimetype the API method just returns all mocked replicas on error
         replicas = []
         for json_doc in list_replicas_on_api():
             if json_doc:
                 replicas.append(parse_response(json_doc))
```

### Comparing `rucio_clients-34.3.0/tests/test_replica_recoverer.py` & `rucio_clients-34.4.0/tests/test_replica_recoverer.py`

 * *Files 4% similar despite different names*

```diff
@@ -516,7 +516,80 @@
         assert (self.tmp_file7.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
         assert (self.tmp_file8.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
         assert (self.tmp_file9.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
         assert (self.tmp_file10.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
         assert (self.tmp_file11.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
         assert (self.tmp_file12.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
         assert (self.tmp_file13.name, self.rse4recovery_id, BadFilesStatus.BAD) not in bad_checklist
+
+
+@pytest.mark.parametrize(
+    "file_config_mock", [{"overrides": [
+        ("replicarecoverer", "rule_rse_expression", "type=SCRATCHDISK"),
+        ('replicarecoverer', 'use_file_metadata', 'False'),
+        ('replicarecoverer', 'did_name_expression', '^.*')]}],
+    indirect=True)
+def test_vo_agnostic_rules(file_config_mock, replica_client, rse_factory, scope_factory, file_factory, vo):
+    """
+    Runs only a single time, make sure it makes a new rule with this config.
+
+    Examining files without a datatype, but because the "use_file_metadata" is turned off,
+    files without a datatype can be acted on.
+    """
+    rse4suspicious, rse4suspicious_id = rse_factory.make_posix_rse(deterministic=True, vo=vo)
+    rse4recovery, rse4recovery_id = rse_factory.make_posix_rse(deterministic=True, vo=vo)
+
+    add_rse_attribute(rse4suspicious_id, "enable_suspicious_file_recovery", True)
+    add_rse_attribute(rse4recovery_id, "enable_suspicious_file_recovery", True)
+
+    # Create new scopes
+    _, [scope_declarebad] = scope_factory(vos=[vo])
+
+    tmp_file_delare_bad = file_factory.file_generator()
+
+    replicas_without_types = [{'scope': scope_declarebad, 'name': tmp_file_delare_bad.name, 'type': DIDType.FILE}]
+    for rse in [rse4suspicious, rse4recovery]:
+        cmd = f'rucio -v upload --rse {rse} --scope {scope_declarebad} {tmp_file_delare_bad}'
+        exitcode, _, _ = execute(cmd)
+        assert exitcode == 0
+
+    remove(tmp_file_delare_bad)
+    rse_expression_parser.REGION.invalidate()
+
+    update_replica_state(rse4recovery_id, scope_declarebad, tmp_file_delare_bad.name, ReplicaState.UNAVAILABLE)
+    replical_declare_bad = list(list_replicas(dids=replicas_without_types))
+
+    for replica in replical_declare_bad:
+        suspicious_pfns = replica['rses'][rse4suspicious_id]
+        for _ in range(3):
+            # The reason must contain the word "checksum", so that the replica can be declared bad.
+            replica_client.declare_suspicious_file_replicas([suspicious_pfns[0], ], 'checksum')
+            sleep(1)
+
+    recovery_policy = [{"action": "declare bad", "datatype": [str(tmp_file_delare_bad.name)], "scope": [str(scope_declarebad)]}]
+    recovery_policy_json = "/opt/rucio/etc/test_replica_recoverer_vo_agonistism.json"
+    json.dump(recovery_policy, open(recovery_policy_json, mode="w"))
+
+    try:
+        run(
+            once=True,
+            younger_than=1,
+            nattempts=2,
+            limit_suspicious_files_on_rse=2,
+            json_file_name=recovery_policy_json,
+            sleep_time=0,
+            active_mode=True
+        )
+    except KeyboardInterrupt:
+        stop()
+
+    # dids without types now have a different behavior
+
+    for replica in replicas_without_types:
+        # Files that are now acted on now the datatype can be found.
+        if replica['name'] == tmp_file_delare_bad.name:
+            # tmp_file11 should no longer be ignored.
+            assert not replica.get('states')
+
+    bad_replicas_list = list_bad_replicas_status(rse_id=rse4suspicious_id, vo=vo)
+    bad_checklist = [(badf['name'], badf['rse_id'], badf['state']) for badf in bad_replicas_list]
+    assert (tmp_file_delare_bad.name, rse4suspicious_id, BadFilesStatus.BAD) in bad_checklist
```

### Comparing `rucio_clients-34.3.0/tests/test_replica_sorting.py` & `rucio_clients-34.4.0/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_request.py` & `rucio_clients-34.4.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_root_proxy.py` & `rucio_clients-34.4.0/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse.py` & `rucio_clients-34.4.0/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_expression_parser.py` & `rucio_clients-34.4.0/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_lfn2path.py` & `rucio_clients-34.4.0/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_gfal2.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_posix.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_rclone.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_rsync.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_srm.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_ssh.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_webdav.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_protocol_xrootd.py` & `rucio_clients-34.4.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rse_selector.py` & `rucio_clients-34.4.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rucio_server.py` & `rucio_clients-34.4.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_rule.py` & `rucio_clients-34.4.0/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_scope.py` & `rucio_clients-34.4.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_subscription.py` & `rucio_clients-34.4.0/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_throttler.py` & `rucio_clients-34.4.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_tpc.py` & `rucio_clients-34.4.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_trace.py` & `rucio_clients-34.4.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_transfer.py` & `rucio_clients-34.4.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_transfer_plugins.py` & `rucio_clients-34.4.0/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_undertaker.py` & `rucio_clients-34.4.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_upload.py` & `rucio_clients-34.4.0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tests/test_utils.py` & `rucio_clients-34.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio_clients-34.3.0/tools/merge_rucio_configs.py` & `rucio_clients-34.4.0/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

