# Comparing `tmp/rucio-34.3.0.tar.gz` & `tmp/rucio-34.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-34.3.0.tar", last modified: Mon May  6 12:44:06 2024, max compression
+gzip compressed data, was "rucio-34.4.0.tar", last modified: Tue May 21 14:54:21 2024, max compression
```

## Comparing `rucio-34.3.0.tar` & `rucio-34.4.0.tar`

### file list

```diff
@@ -1,650 +1,646 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.093713 rucio-34.3.0/
--rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-06 09:19:47.000000 rucio-34.3.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.3.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      934 2024-05-06 12:44:02.000000 rucio-34.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2799 2024-05-06 12:44:06.093713 rucio-34.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1982 2024-05-06 11:03:53.000000 rucio-34.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.993712 rucio-34.3.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio
--rwxr-xr-x   0 root         (0) root         (0)     2820 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-abacus-account
--rwxr-xr-x   0 root         (0) root         (0)     1823 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-abacus-collection-replica
--rwxr-xr-x   0 root         (0) root         (0)     2567 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-abacus-rse
--rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-admin
--rwxr-xr-x   0 root         (0) root         (0)     3185 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-atropos
--rwxr-xr-x   0 root         (0) root         (0)     5850 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-auditor
--rwxr-xr-x   0 root         (0) root         (0)     2010 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-automatix
--rwxr-xr-x   0 root         (0) root         (0)     3103 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-bb8
--rwxr-xr-x   0 root         (0) root         (0)     6100 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-c3po
--rwxr-xr-x   0 root         (0) root         (0)     5060 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-cache-client
--rwxr-xr-x   0 root         (0) root         (0)     1362 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-cache-consumer
--rwxr-xr-x   0 root         (0) root         (0)     2347 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-finisher
--rwxr-xr-x   0 root         (0) root         (0)     2839 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-poller
--rwxr-xr-x   0 root         (0) root         (0)     1759 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-preparer
--rwxr-xr-x   0 root         (0) root         (0)     1682 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-receiver
--rwxr-xr-x   0 root         (0) root         (0)     3385 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-stager
--rwxr-xr-x   0 root         (0) root         (0)     6752 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-submitter
--rwxr-xr-x   0 root         (0) root         (0)     3859 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-conveyor-throttler
--rwxr-xr-x   0 root         (0) root         (0)     2546 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-dark-reaper
--rwxr-xr-x   0 root         (0) root         (0)     6463 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-dumper
--rwxr-xr-x   0 root         (0) root         (0)     1414 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-follower
--rwxr-xr-x   0 root         (0) root         (0)     1987 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-hermes
--rwxr-xr-x   0 root         (0) root         (0)     4649 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-cleaner
--rwxr-xr-x   0 root         (0) root         (0)     7472 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-evaluator
--rwxr-xr-x   0 root         (0) root         (0)     1671 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-injector
--rwxr-xr-x   0 root         (0) root         (0)     1675 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-judge-repairer
--rwxr-xr-x   0 root         (0) root         (0)     1782 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-kronos
--rwxr-xr-x   0 root         (0) root         (0)     2260 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-minos
--rwxr-xr-x   0 root         (0) root         (0)     1997 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-minos-temporary-expiration
--rwxr-xr-x   0 root         (0) root         (0)     5626 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-necromancer
--rwxr-xr-x   0 root         (0) root         (0)     2790 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-oauth-manager
--rwxr-xr-x   0 root         (0) root         (0)     4070 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-reaper
--rwxr-xr-x   0 root         (0) root         (0)    18988 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-replica-recoverer
--rwxr-xr-x   0 root         (0) root         (0)     2351 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-rse-decommissioner
--rwxr-xr-x   0 root         (0) root         (0)     3920 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-storage-consistency-actions
--rwxr-xr-x   0 root         (0) root         (0)     3364 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-transmogrifier
--rwxr-xr-x   0 root         (0) root         (0)     2720 2024-05-06 09:19:47.000000 rucio-34.3.0/bin/rucio-undertaker
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.994711 rucio-34.3.0/etc/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/alembic.ini.template
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/alembic_offline.ini.template
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/globus-config.yml.template
--rw-r--r--   0 root         (0) root         (0)      806 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/ldap.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.995712 rucio-34.3.0/etc/mail_templates/
--rw-r--r--   0 root         (0) root         (0)     1210 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/mail_templates/rule_approval_request.tmpl
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_approved_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_approved_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_denied_admin.tmpl
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_denied_user.tmpl
--rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/mail_templates/rule_ok_notification.tmpl
--rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/rse-accounts.cfg.template
--rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.3.0/etc/rucio.cfg.atlas.client.template
--rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/rucio.cfg.template
--rw-r--r--   0 root         (0) root         (0)     7477 2024-05-06 09:19:47.000000 rucio-34.3.0/etc/rucio_multi_vo.cfg.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.980711 rucio-34.3.0/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.996712 rucio-34.3.0/lib/rucio/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/alembicrevision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:05.999712 rucio-34.3.0/lib/rucio/api/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9292 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/account.py
--rw-r--r--   0 root         (0) root         (0)    11394 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    12890 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/authentication.py
--rw-r--r--   0 root         (0) root         (0)     9085 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/config.py
--rw-r--r--   0 root         (0) root         (0)     2908 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/credential.py
--rw-r--r--   0 root         (0) root         (0)    28964 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/did.py
--rw-r--r--   0 root         (0) root         (0)     3206 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2105 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/exporter.py
--rw-r--r--   0 root         (0) root         (0)     2651 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)     6830 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/importer.py
--rw-r--r--   0 root         (0) root         (0)     3685 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/lock.py
--rw-r--r--   0 root         (0) root         (0)     3573 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/permission.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    22398 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/replica.py
--rw-r--r--   0 root         (0) root         (0)    10550 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/request.py
--rw-r--r--   0 root         (0) root         (0)    23582 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/rse.py
--rw-r--r--   0 root         (0) root         (0)    15938 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/rule.py
--rw-r--r--   0 root         (0) root         (0)     3003 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/scope.py
--rw-r--r--   0 root         (0) root         (0)    10537 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/subscription.py
--rw-r--r--   0 root         (0) root         (0)     4817 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/api/vo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.004712 rucio-34.3.0/lib/rucio/client/
--rw-r--r--   0 root         (0) root         (0)      660 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16352 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/accountclient.py
--rw-r--r--   0 root         (0) root         (0)     5961 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 root         (0) root         (0)    48007 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/baseclient.py
--rw-r--r--   0 root         (0) root         (0)     3079 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4401 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/configclient.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/credentialclient.py
--rw-r--r--   0 root         (0) root         (0)    28378 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/didclient.py
--rw-r--r--   0 root         (0) root         (0)     2114 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/diracclient.py
--rw-r--r--   0 root         (0) root         (0)    86094 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/downloadclient.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/exportclient.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/fileclient.py
--rw-r--r--   0 root         (0) root         (0)     1469 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/importclient.py
--rw-r--r--   0 root         (0) root         (0)     2822 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/lifetimeclient.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/lockclient.py
--rw-r--r--   0 root         (0) root         (0)     5195 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/metaconventionsclient.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/pingclient.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/replicaclient.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/requestclient.py
--rw-r--r--   0 root         (0) root         (0)    27121 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/rseclient.py
--rw-r--r--   0 root         (0) root         (0)    12734 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/ruleclient.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/scopeclient.py
--rw-r--r--   0 root         (0) root         (0)     7971 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 root         (0) root         (0)     2642 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/touchclient.py
--rw-r--r--   0 root         (0) root         (0)    46627 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.007712 rucio-34.3.0/lib/rucio/common/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2301 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/cache.py
--rw-r--r--   0 root         (0) root         (0)    24636 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/config.py
--rw-r--r--   0 root         (0) root         (0)     5507 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/constants.py
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/constraints.py
--rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/didtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.008712 rucio-34.3.0/lib/rucio/common/dumper/
--rw-r--r--   0 root         (0) root         (0)    10796 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/consistency.py
--rw-r--r--   0 root         (0) root         (0)     9693 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/data_models.py
--rw-r--r--   0 root         (0) root         (0)     1923 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/dumper/path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    32345 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/exception.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/extra.py
--rw-r--r--   0 root         (0) root         (0)    15046 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/logging.py
--rw-r--r--   0 root         (0) root         (0)    45296 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/pcache.py
--rw-r--r--   0 root         (0) root         (0)     6071 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/plugins.py
--rw-r--r--   0 root         (0) root         (0)     3085 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/policy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.010712 rucio-34.3.0/lib/rucio/common/schema/
--rw-r--r--   0 root         (0) root         (0)     5384 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15589 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/atlas.py
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/belleii.py
--rw-r--r--   0 root         (0) root         (0)    18523 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/cms.py
--rw-r--r--   0 root         (0) root         (0)    14987 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/domatpc.py
--rw-r--r--   0 root         (0) root         (0)    15926 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/escape.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/generic.py
--rw-r--r--   0 root         (0) root         (0)    15468 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)    15277 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/icecube.py
--rw-r--r--   0 root         (0) root         (0)    15885 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/schema/lsst.py
--rw-r--r--   0 root         (0) root         (0)     5414 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/stomp_utils.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)     5427 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/common/types.py
--rw-r--r--   0 root         (0) root         (0)    79121 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.018712 rucio-34.3.0/lib/rucio/core/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14952 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/account.py
--rw-r--r--   0 root         (0) root         (0)     6289 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/account_counter.py
--rw-r--r--   0 root         (0) root         (0)    14274 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/account_limit.py
--rw-r--r--   0 root         (0) root         (0)    20045 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/authentication.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/config.py
--rw-r--r--   0 root         (0) root         (0)     8211 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/credential.py
--rw-r--r--   0 root         (0) root         (0)   125584 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.019712 rucio-34.3.0/lib/rucio/core/did_meta_plugins/
--rw-r--r--   0 root         (0) root         (0)    11733 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17445 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
--rw-r--r--   0 root         (0) root         (0)     4932 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
--rw-r--r--   0 root         (0) root         (0)    29313 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     9215 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/json_meta.py
--rw-r--r--   0 root         (0) root         (0)     7431 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
--rw-r--r--   0 root         (0) root         (0)    13727 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/dirac.py
--rw-r--r--   0 root         (0) root         (0)     5695 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/distance.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/exporter.py
--rw-r--r--   0 root         (0) root         (0)    10986 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    12099 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/identity.py
--rw-r--r--   0 root         (0) root         (0)    14169 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/importer.py
--rw-r--r--   0 root         (0) root         (0)    15254 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/lifetime_exception.py
--rw-r--r--   0 root         (0) root         (0)    22857 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/lock.py
--rw-r--r--   0 root         (0) root         (0)     9693 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/message.py
--rw-r--r--   0 root         (0) root         (0)     8691 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)    15984 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/monitor.py
--rw-r--r--   0 root         (0) root         (0)     6054 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/naming_convention.py
--rw-r--r--   0 root         (0) root         (0)     4890 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/nongrid_trace.py
--rw-r--r--   0 root         (0) root         (0)    69763 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/oidc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.020712 rucio-34.3.0/lib/rucio/core/permission/
--rw-r--r--   0 root         (0) root         (0)     4070 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55734 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/atlas.py
--rw-r--r--   0 root         (0) root         (0)    46969 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/belleii.py
--rw-r--r--   0 root         (0) root         (0)    46848 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/cms.py
--rw-r--r--   0 root         (0) root         (0)    43171 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/escape.py
--rw-r--r--   0 root         (0) root         (0)    48439 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/generic.py
--rw-r--r--   0 root         (0) root         (0)    45926 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/permission/generic_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)   177379 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/replica.py
--rw-r--r--   0 root         (0) root         (0)    15420 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/replica_sorter.py
--rw-r--r--   0 root         (0) root         (0)   116306 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/request.py
--rw-r--r--   0 root         (0) root         (0)    68025 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse.py
--rw-r--r--   0 root         (0) root         (0)     5506 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse_counter.py
--rw-r--r--   0 root         (0) root         (0)    15368 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)    13941 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rse_selector.py
--rw-r--r--   0 root         (0) root         (0)   208510 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rule.py
--rw-r--r--   0 root         (0) root         (0)    92320 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/rule_grouping.py
--rw-r--r--   0 root         (0) root         (0)     5364 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/scope.py
--rw-r--r--   0 root         (0) root         (0)    15235 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/subscription.py
--rw-r--r--   0 root         (0) root         (0)    18930 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/topology.py
--rw-r--r--   0 root         (0) root         (0)    13107 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/trace.py
--rw-r--r--   0 root         (0) root         (0)    64200 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/transfer.py
--rw-r--r--   0 root         (0) root         (0)     5585 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/vo.py
--rw-r--r--   0 root         (0) root         (0)     5066 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/core/volatile_replica.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.021712 rucio-34.3.0/lib/rucio/daemons/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.022712 rucio-34.3.0/lib/rucio/daemons/abacus/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3736 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/account.py
--rw-r--r--   0 root         (0) root         (0)     3856 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/abacus/rse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.022712 rucio-34.3.0/lib/rucio/daemons/atropos/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/atropos/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10574 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/atropos/atropos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.022712 rucio-34.3.0/lib/rucio/daemons/auditor/
--rw-r--r--   0 root         (0) root         (0)    10003 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/auditor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2865 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/auditor/hdfs.py
--rw-r--r--   0 root         (0) root         (0)    10314 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/auditor/srmdumps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.023712 rucio-34.3.0/lib/rucio/daemons/automatix/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/automatix/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9974 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/automatix/automatix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.023712 rucio-34.3.0/lib/rucio/daemons/badreplicas/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15769 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/minos.py
--rw-r--r--   0 root         (0) root         (0)     8626 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
--rw-r--r--   0 root         (0) root         (0)     9892 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/badreplicas/necromancer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.024712 rucio-34.3.0/lib/rucio/daemons/bb8/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13071 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/bb8.py
--rw-r--r--   0 root         (0) root         (0)    26598 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/common.py
--rw-r--r--   0 root         (0) root         (0)     6693 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
--rw-r--r--   0 root         (0) root         (0)     6571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.025712 rucio-34.3.0/lib/rucio/daemons/c3po/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.025712 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/simple.py
--rw-r--r--   0 root         (0) root         (0)     4651 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
--rw-r--r--   0 root         (0) root         (0)    12212 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
--rw-r--r--   0 root         (0) root         (0)    15009 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/c3po.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.027712 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3261 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/agis.py
--rw-r--r--   0 root         (0) root         (0)     2094 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/free_space.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
--rw-r--r--   0 root         (0) root         (0)     1339 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/mock_did.py
--rw-r--r--   0 root         (0) root         (0)     2068 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3818 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/collectors/workload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.027712 rucio-34.3.0/lib/rucio/daemons/c3po/utils/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1386 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1523 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_list.py
--rw-r--r--   0 root         (0) root         (0)     2440 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/popularity.py
--rw-r--r--   0 root         (0) root         (0)     2087 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/c3po/utils/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.028712 rucio-34.3.0/lib/rucio/daemons/cache/
--rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.3.0/lib/rucio/daemons/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6744 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/cache/consumer.py
--rw-r--r--   0 root         (0) root         (0)    14947 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.029712 rucio-34.3.0/lib/rucio/daemons/conveyor/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25817 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/common.py
--rw-r--r--   0 root         (0) root         (0)    23645 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/finisher.py
--rw-r--r--   0 root         (0) root         (0)    16241 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/poller.py
--rw-r--r--   0 root         (0) root         (0)     7462 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/preparer.py
--rw-r--r--   0 root         (0) root         (0)     8289 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/receiver.py
--rw-r--r--   0 root         (0) root         (0)     3827 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/stager.py
--rw-r--r--   0 root         (0) root         (0)    16333 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/submitter.py
--rw-r--r--   0 root         (0) root         (0)    20351 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/conveyor/throttler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.030712 rucio-34.3.0/lib/rucio/daemons/follower/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/follower/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3355 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/follower/follower.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.030712 rucio-34.3.0/lib/rucio/daemons/hermes/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/hermes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26475 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/hermes/hermes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.031712 rucio-34.3.0/lib/rucio/daemons/judge/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5772 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/cleaner.py
--rw-r--r--   0 root         (0) root         (0)     7170 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     6394 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/injector.py
--rw-r--r--   0 root         (0) root         (0)     5310 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/judge/repairer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.031712 rucio-34.3.0/lib/rucio/daemons/oauthmanager/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/oauthmanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8817 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.032712 rucio-34.3.0/lib/rucio/daemons/reaper/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/reaper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11222 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/reaper/dark_reaper.py
--rw-r--r--   0 root         (0) root         (0)    35602 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/reaper/reaper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.032712 rucio-34.3.0/lib/rucio/daemons/replicarecoverer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/replicarecoverer/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    33152 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.033712 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.033712 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/
--rw-r--r--   0 root         (0) root         (0)      863 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
--rw-r--r--   0 root         (0) root         (0)    16280 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
--rw-r--r--   0 root         (0) root         (0)     2927 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
--rw-r--r--   0 root         (0) root         (0)    10413 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.033712 rucio-34.3.0/lib/rucio/daemons/storage/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.034712 rucio-34.3.0/lib/rucio/daemons/storage/consistency/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/storage/consistency/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29562 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/storage/consistency/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.034712 rucio-34.3.0/lib/rucio/daemons/tracer/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/tracer/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23764 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/tracer/kronos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.035712 rucio-34.3.0/lib/rucio/daemons/transmogrifier/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/transmogrifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30581 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.035712 rucio-34.3.0/lib/rucio/daemons/undertaker/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/undertaker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5230 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/daemons/undertaker/undertaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.035712 rucio-34.3.0/lib/rucio/db/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.036712 rucio-34.3.0/lib/rucio/db/sqla/
--rw-r--r--   0 root         (0) root         (0)     2506 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4151 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.037712 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3545 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.058712 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/
--rw-r--r--   0 root         (0) root         (0)     3340 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
--rw-r--r--   0 root         (0) root         (0)     2640 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
--rw-r--r--   0 root         (0) root         (0)     1533 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     5272 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
--rw-r--r--   0 root         (0) root         (0)     1548 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
--rw-r--r--   0 root         (0) root         (0)     2816 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1260 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
--rw-r--r--   0 root         (0) root         (0)     1678 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
--rw-r--r--   0 root         (0) root         (0)     2675 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
--rw-r--r--   0 root         (0) root         (0)     8494 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
--rw-r--r--   0 root         (0) root         (0)     3277 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3782 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
--rw-r--r--   0 root         (0) root         (0)     4360 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
--rw-r--r--   0 root         (0) root         (0)     3014 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     1497 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
--rw-r--r--   0 root         (0) root         (0)     2781 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
--rw-r--r--   0 root         (0) root         (0)     2297 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     2274 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1723 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
--rw-r--r--   0 root         (0) root         (0)     2206 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
--rw-r--r--   0 root         (0) root         (0)     2837 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
--rw-r--r--   0 root         (0) root         (0)     1554 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
--rw-r--r--   0 root         (0) root         (0)     1308 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
--rw-r--r--   0 root         (0) root         (0)     3882 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     3997 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2817 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     7527 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2396 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     3592 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
--rw-r--r--   0 root         (0) root         (0)     2777 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     1644 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
--rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
--rw-r--r--   0 root         (0) root         (0)     2424 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
--rw-r--r--   0 root         (0) root         (0)     1598 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
--rw-r--r--   0 root         (0) root         (0)     2476 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
--rw-r--r--   0 root         (0) root         (0)     1526 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
--rw-r--r--   0 root         (0) root         (0)     2363 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
--rw-r--r--   0 root         (0) root         (0)     6101 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
--rw-r--r--   0 root         (0) root         (0)     2266 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
--rw-r--r--   0 root         (0) root         (0)     1666 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
--rw-r--r--   0 root         (0) root         (0)     1969 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
--rw-r--r--   0 root         (0) root         (0)     5023 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
--rw-r--r--   0 root         (0) root         (0)     3568 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
--rw-r--r--   0 root         (0) root         (0)     1889 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
--rw-r--r--   0 root         (0) root         (0)     1661 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
--rw-r--r--   0 root         (0) root         (0)     1715 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
--rw-r--r--   0 root         (0) root         (0)     3118 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1749 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
--rw-r--r--   0 root         (0) root         (0)     5038 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
--rw-r--r--   0 root         (0) root         (0)     3689 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
--rw-r--r--   0 root         (0) root         (0)     2614 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
--rw-r--r--   0 root         (0) root         (0)     3117 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
--rw-r--r--   0 root         (0) root         (0)     5836 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
--rw-r--r--   0 root         (0) root         (0)     2195 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
--rw-r--r--   0 root         (0) root         (0)     1585 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
--rw-r--r--   0 root         (0) root         (0)     7344 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
--rw-r--r--   0 root         (0) root         (0)     3704 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
--rw-r--r--   0 root         (0) root         (0)     2091 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
--rw-r--r--   0 root         (0) root         (0)     2934 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
--rw-r--r--   0 root         (0) root         (0)     2784 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     9561 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
--rw-r--r--   0 root         (0) root         (0)     1736 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
--rw-r--r--   0 root         (0) root         (0)     1594 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
--rw-r--r--   0 root         (0) root         (0)     5263 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
--rw-r--r--   0 root         (0) root         (0)     2429 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
--rw-r--r--   0 root         (0) root         (0)     4865 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
--rw-r--r--   0 root         (0) root         (0)     2947 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
--rw-r--r--   0 root         (0) root         (0)     1949 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
--rw-r--r--   0 root         (0) root         (0)     1110 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
--rw-r--r--   0 root         (0) root         (0)     1599 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
--rw-r--r--   0 root         (0) root         (0)   112134 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/db/sqla/models.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/sautils.py
--rw-r--r--   0 root         (0) root         (0)    17773 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/session.py
--rw-r--r--   0 root         (0) root         (0)     6088 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/types.py
--rw-r--r--   0 root         (0) root         (0)    21426 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/db/sqla/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.058712 rucio-34.3.0/lib/rucio/rse/
--rw-r--r--   0 root         (0) root         (0)     3303 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.062712 rucio-34.3.0/lib/rucio/rse/protocols/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7199 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     4603 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 root         (0) root         (0)     4225 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 root         (0) root         (0)    29100 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 root         (0) root         (0)     9730 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/globus.py
--rw-r--r--   0 root         (0) root         (0)     3411 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 root         (0) root         (0)     2975 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 root         (0) root         (0)     4495 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 root         (0) root         (0)     7224 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 root         (0) root         (0)    10400 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 root         (0) root         (0)    22703 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 root         (0) root         (0)    15260 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/rclone.py
--rw-r--r--   0 root         (0) root         (0)     5501 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 root         (0) root         (0)    14655 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 root         (0) root         (0)    17473 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/ssh.py
--rw-r--r--   0 root         (0) root         (0)     8127 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/storm.py
--rw-r--r--   0 root         (0) root         (0)    22168 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 root         (0) root         (0)    12571 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 root         (0) root         (0)    37238 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.062712 rucio-34.3.0/lib/rucio/tests/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8907 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/tests/common_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.064712 rucio-34.3.0/lib/rucio/transfertool/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8342 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/bittorrent.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver.py
--rw-r--r--   0 root         (0) root         (0)     4966 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
--rw-r--r--   0 root         (0) root         (0)    72157 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/fts3.py
--rw-r--r--   0 root         (0) root         (0)     6156 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/fts3_plugins.py
--rw-r--r--   0 root         (0) root         (0)     7716 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/globus.py
--rw-r--r--   0 root         (0) root         (0)     8411 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/globus_library.py
--rw-r--r--   0 root         (0) root         (0)     2859 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/mock.py
--rw-r--r--   0 root         (0) root         (0)     7752 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/transfertool/transfertool.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-05-06 11:04:02.000000 rucio-34.3.0/lib/rucio/vcsversion.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.064712 rucio-34.3.0/lib/rucio/web/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.065712 rucio-34.3.0/lib/rucio/web/rest/
--rwxr-xr-x   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.065712 rucio-34.3.0/lib/rucio/web/rest/flaskapi/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.071713 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7791 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
--rw-r--r--   0 root         (0) root         (0)    36983 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
--rw-r--r--   0 root         (0) root         (0)     3344 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/archives.py
--rw-r--r--   0 root         (0) root         (0)    61047 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/auth.py
--rw-r--r--   0 root         (0) root         (0)    16148 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/common.py
--rw-r--r--   0 root         (0) root         (0)    10143 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/config.py
--rw-r--r--   0 root         (0) root         (0)     7714 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
--rw-r--r--   0 root         (0) root         (0)    80867 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dids.py
--rw-r--r--   0 root         (0) root         (0)     4706 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
--rw-r--r--   0 root         (0) root         (0)     2656 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/export.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
--rw-r--r--   0 root         (0) root         (0)     7894 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/identities.py
--rw-r--r--   0 root         (0) root         (0)     5259 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/import.py
--rw-r--r--   0 root         (0) root         (0)    12009 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12990 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/locks.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/main.py
--rw-r--r--   0 root         (0) root         (0)     7785 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
--rw-r--r--   0 root         (0) root         (0)     3131 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
--rw-r--r--   0 root         (0) root         (0)     3096 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/ping.py
--rw-r--r--   0 root         (0) root         (0)    13331 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
--rw-r--r--   0 root         (0) root         (0)    72711 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
--rw-r--r--   0 root         (0) root         (0)    41622 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/requests.py
--rw-r--r--   0 root         (0) root         (0)    81948 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rses.py
--rw-r--r--   0 root         (0) root         (0)    32189 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rules.py
--rw-r--r--   0 root         (0) root         (0)     5068 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
--rw-r--r--   0 root         (0) root         (0)    24151 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.071713 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
--rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
--rw-r--r--   0 root         (0) root         (0)     3213 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/traces.py
--rw-r--r--   0 root         (0) root         (0)     9154 2024-05-06 11:03:53.000000 rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/vos.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/main.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1010 2024-05-06 09:19:47.000000 rucio-34.3.0/lib/rucio/web/rest/ping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.089713 rucio-34.3.0/lib/rucio.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25997 2024-05-06 12:44:05.000000 rucio-34.3.0/lib/rucio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio-34.3.0/pylintrc
--rw-r--r--   0 root         (0) root         (0)     4349 2024-05-06 09:19:47.000000 rucio-34.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5235 2024-05-06 11:03:53.000000 rucio-34.3.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-06 12:44:06.095713 rucio-34.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-05-06 12:44:02.000000 rucio-34.3.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-05-06 09:19:47.000000 rucio-34.3.0/setuputil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.088713 rucio-34.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3682 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_abacus_account.py
--rw-r--r--   0 root         (0) root         (0)    10677 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_abacus_collection_replica.py
--rw-r--r--   0 root         (0) root         (0)     3229 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_abacus_rse.py
--rw-r--r--   0 root         (0) root         (0)    15923 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_account.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_account_limits.py
--rw-r--r--   0 root         (0) root         (0)    20523 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_api_external_representation.py
--rw-r--r--   0 root         (0) root         (0)    13352 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_archive.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_auditor.py
--rw-r--r--   0 root         (0) root         (0)     2181 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_auditor_hdfs.py
--rw-r--r--   0 root         (0) root         (0)     4201 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_auditor_srmdumps.py
--rw-r--r--   0 root         (0) root         (0)    14964 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     3464 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_automatix.py
--rw-r--r--   0 root         (0) root         (0)    23265 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_bad_replica.py
--rw-r--r--   0 root         (0) root         (0)    12425 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_bb8.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_belleii.py
--rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_bin_rucio.py
--rw-r--r--   0 root         (0) root         (0)     2065 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_boolean.py
--rw-r--r--   0 root         (0) root         (0)     8398 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_clients.py
--rw-r--r--   0 root         (0) root         (0)     1865 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_common_types.py
--rw-r--r--   0 root         (0) root         (0)     6942 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)    96724 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_conveyor.py
--rw-r--r--   0 root         (0) root         (0)    23870 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_conveyor_submitter.py
--rw-r--r--   0 root         (0) root         (0)     6947 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     7728 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_credential.py
--rw-r--r--   0 root         (0) root         (0)     7337 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_curl.py
--rw-r--r--   0 root         (0) root         (0)     2618 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_daemons.py
--rw-r--r--   0 root         (0) root         (0)    28183 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dataset_replicas.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_db.py
--rw-r--r--   0 root         (0) root         (0)    58823 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_did.py
--rw-r--r--   0 root         (0) root         (0)    29517 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_did_meta_plugins.py
--rw-r--r--   0 root         (0) root         (0)     4185 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_didtype.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_download.py
--rw-r--r--   0 root         (0) root         (0)     7118 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper.py
--rw-r--r--   0 root         (0) root         (0)    16419 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper_consistency.py
--rw-r--r--   0 root         (0) root         (0)    10869 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper_data_model.py
--rw-r--r--   0 root         (0) root         (0)     3082 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_dumper_path_parsing.py
--rw-r--r--   0 root         (0) root         (0)    38301 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_filter_engine.py
--rw-r--r--   0 root         (0) root         (0)     7953 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_heartbeat.py
--rw-r--r--   0 root         (0) root         (0)    10106 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_hermes.py
--rw-r--r--   0 root         (0) root         (0)     5821 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_identity.py
--rw-r--r--   0 root         (0) root         (0)    18584 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_impl_upload_download.py
--rw-r--r--   0 root         (0) root         (0)    57290 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     5258 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    22277 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_evaluator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_injector.py
--rw-r--r--   0 root         (0) root         (0)    20429 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_judge_repairer.py
--rw-r--r--   0 root         (0) root         (0)    12180 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_lifetime.py
--rw-r--r--   0 root         (0) root         (0)     5855 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_message.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_meta_conventions.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_meta_did.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_module_import.py
--rw-r--r--   0 root         (0) root         (0)     2034 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_monitor.py
--rw-r--r--   0 root         (0) root         (0)    54332 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_multi_vo.py
--rw-r--r--   0 root         (0) root         (0)     2759 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_naming_convention.py
--rw-r--r--   0 root         (0) root         (0)    11582 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_oauthmanager.py
--rw-r--r--   0 root         (0) root         (0)   108359 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_oidc.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     4123 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_pfns.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_ping.py
--rw-r--r--   0 root         (0) root         (0)     7662 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_preparer.py
--rw-r--r--   0 root         (0) root         (0)     2741 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_qos.py
--rw-r--r--   0 root         (0) root         (0)     2023 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_quarantined_replica.py
--rw-r--r--   0 root         (0) root         (0)    27487 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_reaper.py
--rw-r--r--   0 root         (0) root         (0)     6440 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_redirect.py
--rw-r--r--   0 root         (0) root         (0)    62453 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_replica.py
--rw-r--r--   0 root         (0) root         (0)    38868 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_replica_recoverer.py
--rw-r--r--   0 root         (0) root         (0)    22796 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_replica_sorting.py
--rw-r--r--   0 root         (0) root         (0)    17257 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_request.py
--rw-r--r--   0 root         (0) root         (0)    13033 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_root_proxy.py
--rw-r--r--   0 root         (0) root         (0)    75080 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse.py
--rw-r--r--   0 root         (0) root         (0)    13184 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_expression_parser.py
--rw-r--r--   0 root         (0) root         (0)     8940 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_lfn2path.py
--rw-r--r--   0 root         (0) root         (0)     4277 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_gfal2_impl.py
--rw-r--r--   0 root         (0) root         (0)     3267 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_posix.py
--rw-r--r--   0 root         (0) root         (0)     3690 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_rclone.py
--rw-r--r--   0 root         (0) root         (0)     4799 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_rsync.py
--rw-r--r--   0 root         (0) root         (0)     3979 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_srm.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_ssh.py
--rw-r--r--   0 root         (0) root         (0)     3015 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 root         (0) root         (0)     7746 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rse_selector.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_rucio_server.py
--rw-r--r--   0 root         (0) root         (0)    91949 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_rule.py
--rw-r--r--   0 root         (0) root         (0)    13848 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_schema_cms.py
--rw-r--r--   0 root         (0) root         (0)     7486 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_scope.py
--rw-r--r--   0 root         (0) root         (0)    48389 2024-05-06 11:03:53.000000 rucio-34.3.0/tests/test_subscription.py
--rw-r--r--   0 root         (0) root         (0)    55587 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_throttler.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_tpc.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_trace.py
--rw-r--r--   0 root         (0) root         (0)    25254 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_transfer.py
--rw-r--r--   0 root         (0) root         (0)     8924 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_transfer_plugins.py
--rw-r--r--   0 root         (0) root         (0)     8412 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_undertaker.py
--rw-r--r--   0 root         (0) root         (0)    15575 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_upload.py
--rw-r--r--   0 root         (0) root         (0)     7427 2024-05-06 09:19:47.000000 rucio-34.3.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 12:44:06.089713 rucio-34.3.0/tools/
--rwxr-xr-x   0 root         (0) root         (0)     1259 2024-05-06 09:19:47.000000 rucio-34.3.0/tools/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     6163 2024-05-06 09:19:47.000000 rucio-34.3.0/tools/merge_rucio_configs.py
--rwxr-xr-x   0 root         (0) root         (0)     1351 2024-05-06 09:19:47.000000 rucio-34.3.0/tools/reset_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.782573 rucio-34.4.0/
+-rwxr-xr-x   0 root         (0) root         (0)     4487 2024-05-16 07:28:57.000000 rucio-34.4.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-27 12:40:37.000000 rucio-34.4.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-27 12:40:37.000000 rucio-34.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      934 2024-05-21 14:54:17.000000 rucio-34.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2799 2024-05-21 14:54:21.781573 rucio-34.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-05-21 09:35:26.000000 rucio-34.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.675572 rucio-34.4.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)   127119 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio
+-rwxr-xr-x   0 root         (0) root         (0)     2820 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-abacus-account
+-rwxr-xr-x   0 root         (0) root         (0)     1823 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-abacus-collection-replica
+-rwxr-xr-x   0 root         (0) root         (0)     2567 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-abacus-rse
+-rwxr-xr-x   0 root         (0) root         (0)   133582 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-admin
+-rwxr-xr-x   0 root         (0) root         (0)     3185 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-atropos
+-rwxr-xr-x   0 root         (0) root         (0)     5850 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-auditor
+-rwxr-xr-x   0 root         (0) root         (0)     2010 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-automatix
+-rwxr-xr-x   0 root         (0) root         (0)     3103 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-bb8
+-rwxr-xr-x   0 root         (0) root         (0)     6100 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-c3po
+-rwxr-xr-x   0 root         (0) root         (0)     5060 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-cache-client
+-rwxr-xr-x   0 root         (0) root         (0)     1362 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-cache-consumer
+-rwxr-xr-x   0 root         (0) root         (0)     2347 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-finisher
+-rwxr-xr-x   0 root         (0) root         (0)     2839 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-poller
+-rwxr-xr-x   0 root         (0) root         (0)     1759 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-preparer
+-rwxr-xr-x   0 root         (0) root         (0)     1682 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-receiver
+-rwxr-xr-x   0 root         (0) root         (0)     3385 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-stager
+-rwxr-xr-x   0 root         (0) root         (0)     6752 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-submitter
+-rwxr-xr-x   0 root         (0) root         (0)     3859 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-conveyor-throttler
+-rwxr-xr-x   0 root         (0) root         (0)     2546 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-dark-reaper
+-rwxr-xr-x   0 root         (0) root         (0)     6463 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-dumper
+-rwxr-xr-x   0 root         (0) root         (0)     1414 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-follower
+-rwxr-xr-x   0 root         (0) root         (0)     1987 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-hermes
+-rwxr-xr-x   0 root         (0) root         (0)     4649 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-cleaner
+-rwxr-xr-x   0 root         (0) root         (0)     7472 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-evaluator
+-rwxr-xr-x   0 root         (0) root         (0)     1671 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-injector
+-rwxr-xr-x   0 root         (0) root         (0)     1675 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-judge-repairer
+-rwxr-xr-x   0 root         (0) root         (0)     1782 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-kronos
+-rwxr-xr-x   0 root         (0) root         (0)     2260 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-minos
+-rwxr-xr-x   0 root         (0) root         (0)     1997 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-minos-temporary-expiration
+-rwxr-xr-x   0 root         (0) root         (0)     5626 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-necromancer
+-rwxr-xr-x   0 root         (0) root         (0)     2790 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-oauth-manager
+-rwxr-xr-x   0 root         (0) root         (0)     4070 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-reaper
+-rwxr-xr-x   0 root         (0) root         (0)    18988 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-replica-recoverer
+-rwxr-xr-x   0 root         (0) root         (0)     2351 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-rse-decommissioner
+-rwxr-xr-x   0 root         (0) root         (0)     3920 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-storage-consistency-actions
+-rwxr-xr-x   0 root         (0) root         (0)     3364 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-transmogrifier
+-rwxr-xr-x   0 root         (0) root         (0)     2720 2024-05-16 07:28:57.000000 rucio-34.4.0/bin/rucio-undertaker
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.677572 rucio-34.4.0/etc/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/alembic.ini.template
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/alembic_offline.ini.template
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/globus-config.yml.template
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-16 07:28:57.000000 rucio-34.4.0/etc/ldap.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.678572 rucio-34.4.0/etc/mail_templates/
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-05-06 09:19:47.000000 rucio-34.4.0/etc/mail_templates/rule_approval_request.tmpl
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_approved_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_approved_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_denied_admin.tmpl
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_denied_user.tmpl
+-rw-r--r--   0 root         (0) root         (0)      546 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/mail_templates/rule_ok_notification.tmpl
+-rwxr-xr-x   0 root         (0) root         (0)      543 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/rse-accounts.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-07-27 12:40:37.000000 rucio-34.4.0/etc/rucio.cfg.atlas.client.template
+-rw-r--r--   0 root         (0) root         (0)     8534 2024-05-06 09:19:47.000000 rucio-34.4.0/etc/rucio.cfg.template
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-05-06 09:19:47.000000 rucio-34.4.0/etc/rucio_multi_vo.cfg.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.662572 rucio-34.4.0/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.678572 rucio-34.4.0/lib/rucio/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/alembicrevision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.683572 rucio-34.4.0/lib/rucio/api/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9396 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/account.py
+-rw-r--r--   0 root         (0) root         (0)    11394 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/config.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/credential.py
+-rw-r--r--   0 root         (0) root         (0)    29418 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/did.py
+-rw-r--r--   0 root         (0) root         (0)     3206 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/exporter.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/importer.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/lock.py
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/permission.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    22565 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/replica.py
+-rw-r--r--   0 root         (0) root         (0)    10550 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/request.py
+-rw-r--r--   0 root         (0) root         (0)    23637 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/rse.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/rule.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/scope.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/api/vo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.688572 rucio-34.4.0/lib/rucio/client/
+-rw-r--r--   0 root         (0) root         (0)      660 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16352 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/accountclient.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 root         (0) root         (0)    48035 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/client/baseclient.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/configclient.py
+-rw-r--r--   0 root         (0) root         (0)     1989 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/credentialclient.py
+-rw-r--r--   0 root         (0) root         (0)    28378 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/didclient.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/diracclient.py
+-rw-r--r--   0 root         (0) root         (0)    87520 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/downloadclient.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/exportclient.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/fileclient.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/importclient.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/lifetimeclient.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/lockclient.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/metaconventionsclient.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/pingclient.py
+-rw-r--r--   0 root         (0) root         (0)    19518 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/requestclient.py
+-rw-r--r--   0 root         (0) root         (0)    27121 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/rseclient.py
+-rw-r--r--   0 root         (0) root         (0)    12734 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/touchclient.py
+-rw-r--r--   0 root         (0) root         (0)    46627 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.691572 rucio-34.4.0/lib/rucio/common/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/cache.py
+-rw-r--r--   0 root         (0) root         (0)    24636 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/constants.py
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/constraints.py
+-rwxr-xr-x   0 root         (0) root         (0)     6545 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/didtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.692572 rucio-34.4.0/lib/rucio/common/dumper/
+-rw-r--r--   0 root         (0) root         (0)    10796 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/consistency.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/data_models.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/dumper/path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    32345 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/exception.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/extra.py
+-rw-r--r--   0 root         (0) root         (0)    15046 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/logging.py
+-rw-r--r--   0 root         (0) root         (0)    45338 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/common/pcache.py
+-rw-r--r--   0 root         (0) root         (0)     6071 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/policy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.694572 rucio-34.4.0/lib/rucio/common/schema/
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15589 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    14987 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/domatpc.py
+-rw-r--r--   0 root         (0) root         (0)    15926 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/escape.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/generic.py
+-rw-r--r--   0 root         (0) root         (0)    15468 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)    15277 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/schema/icecube.py
+-rw-r--r--   0 root         (0) root         (0)     5414 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/stomp_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)     5716 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/common/types.py
+-rw-r--r--   0 root         (0) root         (0)    79163 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.702572 rucio-34.4.0/lib/rucio/core/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14952 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/account.py
+-rw-r--r--   0 root         (0) root         (0)     6289 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/account_counter.py
+-rw-r--r--   0 root         (0) root         (0)    14274 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/account_limit.py
+-rw-r--r--   0 root         (0) root         (0)    21045 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/config.py
+-rw-r--r--   0 root         (0) root         (0)     8211 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/credential.py
+-rw-r--r--   0 root         (0) root         (0)   129547 2024-05-21 09:34:41.000000 rucio-34.4.0/lib/rucio/core/did.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.704573 rucio-34.4.0/lib/rucio/core/did_meta_plugins/
+-rw-r--r--   0 root         (0) root         (0)    11733 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17445 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_column_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4932 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py
+-rw-r--r--   0 root         (0) root         (0)    30038 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     9215 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/json_meta.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/mongo_meta.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/did_meta_plugins/postgres_meta.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     5735 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/distance.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/exporter.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/identity.py
+-rw-r--r--   0 root         (0) root         (0)    14169 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/importer.py
+-rw-r--r--   0 root         (0) root         (0)    15254 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/lifetime_exception.py
+-rw-r--r--   0 root         (0) root         (0)    22857 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/lock.py
+-rw-r--r--   0 root         (0) root         (0)     9693 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/message.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)    15984 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/nongrid_trace.py
+-rw-r--r--   0 root         (0) root         (0)    69833 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/core/oidc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.705572 rucio-34.4.0/lib/rucio/core/permission/
+-rw-r--r--   0 root         (0) root         (0)     4070 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55734 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    46969 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/belleii.py
+-rw-r--r--   0 root         (0) root         (0)    43171 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/escape.py
+-rw-r--r--   0 root         (0) root         (0)    48439 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/generic.py
+-rw-r--r--   0 root         (0) root         (0)    45926 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/permission/generic_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)   178001 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/replica.py
+-rw-r--r--   0 root         (0) root         (0)    15434 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/core/replica_sorter.py
+-rw-r--r--   0 root         (0) root         (0)   116306 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/request.py
+-rw-r--r--   0 root         (0) root         (0)    68107 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse_counter.py
+-rw-r--r--   0 root         (0) root         (0)    15368 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)    14577 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)   208876 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rule.py
+-rw-r--r--   0 root         (0) root         (0)    94279 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/rule_grouping.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/scope.py
+-rw-r--r--   0 root         (0) root         (0)    15235 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    18930 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/topology.py
+-rw-r--r--   0 root         (0) root         (0)    13107 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/trace.py
+-rw-r--r--   0 root         (0) root         (0)    64200 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/transfer.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/core/vo.py
+-rw-r--r--   0 root         (0) root         (0)     5066 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/core/volatile_replica.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.705572 rucio-34.4.0/lib/rucio/daemons/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.706573 rucio-34.4.0/lib/rucio/daemons/abacus/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/account.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/abacus/rse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.706573 rucio-34.4.0/lib/rucio/daemons/atropos/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/atropos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10574 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/atropos/atropos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.707573 rucio-34.4.0/lib/rucio/daemons/auditor/
+-rw-r--r--   0 root         (0) root         (0)    10003 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/auditor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/auditor/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)    10409 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/auditor/srmdumps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.707573 rucio-34.4.0/lib/rucio/daemons/automatix/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/automatix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9974 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/automatix/automatix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.708572 rucio-34.4.0/lib/rucio/daemons/badreplicas/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15769 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/minos.py
+-rw-r--r--   0 root         (0) root         (0)     8626 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py
+-rw-r--r--   0 root         (0) root         (0)     9892 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/badreplicas/necromancer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.709573 rucio-34.4.0/lib/rucio/daemons/bb8/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13071 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/bb8.py
+-rw-r--r--   0 root         (0) root         (0)    26778 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/common.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/bb8/t2_background_rebalance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.709573 rucio-34.4.0/lib/rucio/daemons/c3po/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.710573 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/simple.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
+-rw-r--r--   0 root         (0) root         (0)    12212 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
+-rw-r--r--   0 root         (0) root         (0)    15009 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/c3po.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.711573 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/agis.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/free_space.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/jedi_did.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/mock_did.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/network_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/collectors/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.712573 rucio-34.4.0/lib/rucio/daemons/c3po/utils/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_list.py
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/popularity.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/c3po/utils/timeseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.713573 rucio-34.4.0/lib/rucio/daemons/cache/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-07-27 12:40:37.000000 rucio-34.4.0/lib/rucio/daemons/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6744 2024-05-06 09:19:47.000000 rucio-34.4.0/lib/rucio/daemons/cache/consumer.py
+-rw-r--r--   0 root         (0) root         (0)    14947 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.714573 rucio-34.4.0/lib/rucio/daemons/conveyor/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25817 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/common.py
+-rw-r--r--   0 root         (0) root         (0)    23645 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/finisher.py
+-rw-r--r--   0 root         (0) root         (0)    16241 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/poller.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/preparer.py
+-rw-r--r--   0 root         (0) root         (0)     8289 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/receiver.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/stager.py
+-rw-r--r--   0 root         (0) root         (0)    16333 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/submitter.py
+-rw-r--r--   0 root         (0) root         (0)    20351 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/conveyor/throttler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.715573 rucio-34.4.0/lib/rucio/daemons/follower/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/follower/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/follower/follower.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.715573 rucio-34.4.0/lib/rucio/daemons/hermes/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/hermes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26475 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/hermes/hermes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.716573 rucio-34.4.0/lib/rucio/daemons/judge/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5772 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/cleaner.py
+-rw-r--r--   0 root         (0) root         (0)     7170 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     6394 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/injector.py
+-rw-r--r--   0 root         (0) root         (0)     5310 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/judge/repairer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.716573 rucio-34.4.0/lib/rucio/daemons/oauthmanager/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/oauthmanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8817 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/oauthmanager/oauthmanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.717573 rucio-34.4.0/lib/rucio/daemons/reaper/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/reaper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11431 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/reaper/dark_reaper.py
+-rw-r--r--   0 root         (0) root         (0)    35602 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/reaper/reaper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.717573 rucio-34.4.0/lib/rucio/daemons/replicarecoverer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/replicarecoverer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    35895 2024-05-21 07:16:09.000000 rucio-34.4.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.718573 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.719573 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/
+-rw-r--r--   0 root         (0) root         (0)      863 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py
+-rw-r--r--   0 root         (0) root         (0)    10413 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.719573 rucio-34.4.0/lib/rucio/daemons/storage/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.719573 rucio-34.4.0/lib/rucio/daemons/storage/consistency/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/storage/consistency/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29562 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/storage/consistency/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.720573 rucio-34.4.0/lib/rucio/daemons/tracer/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/tracer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23764 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/tracer/kronos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.720573 rucio-34.4.0/lib/rucio/daemons/transmogrifier/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/transmogrifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30581 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/transmogrifier/transmogrifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.720573 rucio-34.4.0/lib/rucio/daemons/undertaker/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/undertaker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/daemons/undertaker/undertaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.721573 rucio-34.4.0/lib/rucio/db/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.722573 rucio-34.4.0/lib/rucio/db/sqla/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.722573 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.745573 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/
+-rw-r--r--   0 root         (0) root         (0)     3340 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
+-rw-r--r--   0 root         (0) root         (0)     8494 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py
+-rw-r--r--   0 root         (0) root         (0)     3882 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
+-rw-r--r--   0 root         (0) root         (0)     6101 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py
+-rw-r--r--   0 root         (0) root         (0)     5023 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py
+-rw-r--r--   0 root         (0) root         (0)     5038 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py
+-rw-r--r--   0 root         (0) root         (0)     3689 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py
+-rw-r--r--   0 root         (0) root         (0)     3117 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py
+-rw-r--r--   0 root         (0) root         (0)     5836 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
+-rw-r--r--   0 root         (0) root         (0)     2784 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     9561 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py
+-rw-r--r--   0 root         (0) root         (0)     4865 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
+-rw-r--r--   0 root         (0) root         (0)   112134 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/db/sqla/models.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/sautils.py
+-rw-r--r--   0 root         (0) root         (0)    17773 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/session.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/db/sqla/types.py
+-rw-r--r--   0 root         (0) root         (0)    22230 2024-05-21 09:34:41.000000 rucio-34.4.0/lib/rucio/db/sqla/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.746573 rucio-34.4.0/lib/rucio/rse/
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.749573 rucio-34.4.0/lib/rucio/rse/protocols/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7199 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 root         (0) root         (0)    29100 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/globus.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 root         (0) root         (0)    10414 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 root         (0) root         (0)    21937 2024-05-21 07:56:16.000000 rucio-34.4.0/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/rclone.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 root         (0) root         (0)    14689 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 root         (0) root         (0)    17473 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     8141 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/storm.py
+-rw-r--r--   0 root         (0) root         (0)    22448 2024-05-21 07:56:54.000000 rucio-34.4.0/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 root         (0) root         (0)    12571 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 root         (0) root         (0)    37238 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.749573 rucio-34.4.0/lib/rucio/tests/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/tests/common_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.751573 rucio-34.4.0/lib/rucio/transfertool/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/bittorrent.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py
+-rw-r--r--   0 root         (0) root         (0)    72157 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/fts3.py
+-rw-r--r--   0 root         (0) root         (0)     6156 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/fts3_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/globus.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/globus_library.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/mock.py
+-rw-r--r--   0 root         (0) root         (0)     7752 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/transfertool/transfertool.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-05-21 12:45:12.000000 rucio-34.4.0/lib/rucio/vcsversion.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.751573 rucio-34.4.0/lib/rucio/web/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.752573 rucio-34.4.0/lib/rucio/web/rest/
+-rwxr-xr-x   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.752573 rucio-34.4.0/lib/rucio/web/rest/flaskapi/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.758573 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7791 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py
+-rw-r--r--   0 root         (0) root         (0)    36983 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accounts.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/archives.py
+-rw-r--r--   0 root         (0) root         (0)    61047 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/auth.py
+-rw-r--r--   0 root         (0) root         (0)    16148 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/common.py
+-rw-r--r--   0 root         (0) root         (0)    10143 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/config.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/credentials.py
+-rw-r--r--   0 root         (0) root         (0)    80867 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dids.py
+-rw-r--r--   0 root         (0) root         (0)     4706 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dirac.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/export.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py
+-rw-r--r--   0 root         (0) root         (0)     7894 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/identities.py
+-rw-r--r--   0 root         (0) root         (0)     5259 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/import.py
+-rw-r--r--   0 root         (0) root         (0)    12009 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12990 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/locks.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/main.py
+-rw-r--r--   0 root         (0) root         (0)     7785 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/ping.py
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/redirect.py
+-rw-r--r--   0 root         (0) root         (0)    72711 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/replicas.py
+-rw-r--r--   0 root         (0) root         (0)    41622 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/requests.py
+-rw-r--r--   0 root         (0) root         (0)    81948 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rses.py
+-rw-r--r--   0 root         (0) root         (0)    32189 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rules.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/scopes.py
+-rw-r--r--   0 root         (0) root         (0)    24151 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.758573 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-07-27 12:40:37.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-07-27 12:40:37.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/traces.py
+-rw-r--r--   0 root         (0) root         (0)     9154 2024-05-21 09:35:26.000000 rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/vos.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/main.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2024-05-16 07:28:57.000000 rucio-34.4.0/lib/rucio/web/rest/ping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.777573 rucio-34.4.0/lib/rucio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25876 2024-05-21 14:54:21.000000 rucio-34.4.0/lib/rucio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    16384 2024-05-06 09:19:47.000000 rucio-34.4.0/pylintrc
+-rw-r--r--   0 root         (0) root         (0)     5763 2024-05-21 07:56:54.000000 rucio-34.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     5235 2024-05-21 09:35:26.000000 rucio-34.4.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-21 14:54:21.783573 rucio-34.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-05-21 14:54:17.000000 rucio-34.4.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-05-16 07:28:57.000000 rucio-34.4.0/setuputil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.776573 rucio-34.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     3682 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_abacus_account.py
+-rw-r--r--   0 root         (0) root         (0)    10677 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_abacus_collection_replica.py
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_abacus_rse.py
+-rw-r--r--   0 root         (0) root         (0)    15923 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_account.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_account_limits.py
+-rw-r--r--   0 root         (0) root         (0)    20523 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_api_external_representation.py
+-rw-r--r--   0 root         (0) root         (0)    13352 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_archive.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_auditor.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_auditor_hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 root         (0) root         (0)    14964 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_automatix.py
+-rw-r--r--   0 root         (0) root         (0)    23265 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_bad_replica.py
+-rw-r--r--   0 root         (0) root         (0)    12425 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_bb8.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_belleii.py
+-rwxr-xr-x   0 root         (0) root         (0)   107450 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_bin_rucio.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_boolean.py
+-rw-r--r--   0 root         (0) root         (0)     8398 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_common_types.py
+-rw-r--r--   0 root         (0) root         (0)     6942 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)    96724 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_conveyor.py
+-rw-r--r--   0 root         (0) root         (0)    23870 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_conveyor_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     6947 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     7728 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7337 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_curl.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_daemons.py
+-rw-r--r--   0 root         (0) root         (0)    28183 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dataset_replicas.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_db.py
+-rw-r--r--   0 root         (0) root         (0)    58823 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_did.py
+-rw-r--r--   0 root         (0) root         (0)    29517 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_did_meta_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_didtype.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_download.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper_consistency.py
+-rw-r--r--   0 root         (0) root         (0)    10869 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper_data_model.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    38301 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_filter_engine.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_heartbeat.py
+-rw-r--r--   0 root         (0) root         (0)    10106 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_hermes.py
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_identity.py
+-rw-r--r--   0 root         (0) root         (0)    18584 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_impl_upload_download.py
+-rw-r--r--   0 root         (0) root         (0)    57290 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     5258 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_cleaner.py
+-rw-r--r--   0 root         (0) root         (0)    22277 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_evaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_injector.py
+-rw-r--r--   0 root         (0) root         (0)    20429 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_judge_repairer.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_lifetime.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     6299 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_meta_conventions.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_meta_did.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_module_import.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_monitor.py
+-rw-r--r--   0 root         (0) root         (0)    54332 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_multi_vo.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_naming_convention.py
+-rw-r--r--   0 root         (0) root         (0)    11582 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_oauthmanager.py
+-rw-r--r--   0 root         (0) root         (0)   108359 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_oidc.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_pfns.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_ping.py
+-rw-r--r--   0 root         (0) root         (0)     7662 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_preparer.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_qos.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_quarantined_replica.py
+-rw-r--r--   0 root         (0) root         (0)    27487 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_reaper.py
+-rw-r--r--   0 root         (0) root         (0)     6440 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_redirect.py
+-rw-r--r--   0 root         (0) root         (0)    62467 2024-05-21 07:56:54.000000 rucio-34.4.0/tests/test_replica.py
+-rw-r--r--   0 root         (0) root         (0)    42098 2024-05-21 07:16:09.000000 rucio-34.4.0/tests/test_replica_recoverer.py
+-rw-r--r--   0 root         (0) root         (0)    22796 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_replica_sorting.py
+-rw-r--r--   0 root         (0) root         (0)    17257 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_request.py
+-rw-r--r--   0 root         (0) root         (0)    13033 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_root_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    75080 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse.py
+-rw-r--r--   0 root         (0) root         (0)    13184 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_expression_parser.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_lfn2path.py
+-rw-r--r--   0 root         (0) root         (0)     4277 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_gfal2_impl.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_rclone.py
+-rw-r--r--   0 root         (0) root         (0)     4799 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_rsync.py
+-rw-r--r--   0 root         (0) root         (0)     3979 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_ssh.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 root         (0) root         (0)     7746 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rse_selector.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_rucio_server.py
+-rw-r--r--   0 root         (0) root         (0)    91949 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7486 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_scope.py
+-rw-r--r--   0 root         (0) root         (0)    48389 2024-05-21 09:35:26.000000 rucio-34.4.0/tests/test_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    55587 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_throttler.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_tpc.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_trace.py
+-rw-r--r--   0 root         (0) root         (0)    25254 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_transfer.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_transfer_plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_undertaker.py
+-rw-r--r--   0 root         (0) root         (0)    15575 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_upload.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2024-05-16 07:28:57.000000 rucio-34.4.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:21.777573 rucio-34.4.0/tools/
+-rwxr-xr-x   0 root         (0) root         (0)     1259 2024-05-16 07:28:57.000000 rucio-34.4.0/tools/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2024-05-16 07:28:57.000000 rucio-34.4.0/tools/merge_rucio_configs.py
+-rwxr-xr-x   0 root         (0) root         (0)     1351 2024-05-16 07:28:57.000000 rucio-34.4.0/tools/reset_database.py
```

### Comparing `rucio-34.3.0/AUTHORS.rst` & `rucio-34.4.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/LICENSE` & `rucio-34.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/MANIFEST.in` & `rucio-34.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/PKG-INFO` & `rucio-34.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rucio
-Version: 34.3.0
+Version: 34.4.0
 Summary: Rucio Package
 Home-page: https://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `rucio-34.3.0/README.rst` & `rucio-34.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio` & `rucio-34.4.0/bin/rucio`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-abacus-account` & `rucio-34.4.0/bin/rucio-abacus-account`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-abacus-collection-replica` & `rucio-34.4.0/bin/rucio-abacus-collection-replica`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-abacus-rse` & `rucio-34.4.0/bin/rucio-abacus-rse`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-admin` & `rucio-34.4.0/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-atropos` & `rucio-34.4.0/bin/rucio-atropos`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-auditor` & `rucio-34.4.0/bin/rucio-auditor`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-automatix` & `rucio-34.4.0/bin/rucio-automatix`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-bb8` & `rucio-34.4.0/bin/rucio-bb8`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-c3po` & `rucio-34.4.0/bin/rucio-c3po`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-cache-client` & `rucio-34.4.0/bin/rucio-cache-client`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-cache-consumer` & `rucio-34.4.0/bin/rucio-cache-consumer`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-finisher` & `rucio-34.4.0/bin/rucio-conveyor-finisher`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-poller` & `rucio-34.4.0/bin/rucio-conveyor-poller`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-preparer` & `rucio-34.4.0/bin/rucio-conveyor-preparer`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-receiver` & `rucio-34.4.0/bin/rucio-conveyor-receiver`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-stager` & `rucio-34.4.0/bin/rucio-conveyor-stager`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-submitter` & `rucio-34.4.0/bin/rucio-conveyor-submitter`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-conveyor-throttler` & `rucio-34.4.0/bin/rucio-conveyor-throttler`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-dark-reaper` & `rucio-34.4.0/bin/rucio-dark-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-dumper` & `rucio-34.4.0/bin/rucio-dumper`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-follower` & `rucio-34.4.0/bin/rucio-follower`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-hermes` & `rucio-34.4.0/bin/rucio-hermes`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-judge-cleaner` & `rucio-34.4.0/bin/rucio-judge-cleaner`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-judge-evaluator` & `rucio-34.4.0/bin/rucio-judge-evaluator`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-judge-injector` & `rucio-34.4.0/bin/rucio-judge-injector`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-judge-repairer` & `rucio-34.4.0/bin/rucio-judge-repairer`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-kronos` & `rucio-34.4.0/bin/rucio-kronos`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-minos` & `rucio-34.4.0/bin/rucio-minos`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-minos-temporary-expiration` & `rucio-34.4.0/bin/rucio-minos-temporary-expiration`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-necromancer` & `rucio-34.4.0/bin/rucio-necromancer`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-oauth-manager` & `rucio-34.4.0/bin/rucio-oauth-manager`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-reaper` & `rucio-34.4.0/bin/rucio-reaper`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-replica-recoverer` & `rucio-34.4.0/bin/rucio-replica-recoverer`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-rse-decommissioner` & `rucio-34.4.0/bin/rucio-rse-decommissioner`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-storage-consistency-actions` & `rucio-34.4.0/bin/rucio-storage-consistency-actions`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-transmogrifier` & `rucio-34.4.0/bin/rucio-transmogrifier`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/bin/rucio-undertaker` & `rucio-34.4.0/bin/rucio-undertaker`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/alembic.ini.template` & `rucio-34.4.0/etc/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/alembic_offline.ini.template` & `rucio-34.4.0/etc/alembic_offline.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/ldap.cfg.template` & `rucio-34.4.0/etc/ldap.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/mail_templates/rule_approval_request.tmpl` & `rucio-34.4.0/etc/mail_templates/rule_approval_request.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/mail_templates/rule_ok_notification.tmpl` & `rucio-34.4.0/etc/mail_templates/rule_ok_notification.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/rse-accounts.cfg.template` & `rucio-34.4.0/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/rucio.cfg.atlas.client.template` & `rucio-34.4.0/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/rucio.cfg.template` & `rucio-34.4.0/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/etc/rucio_multi_vo.cfg.template` & `rucio-34.4.0/etc/rucio_multi_vo.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/__init__.py` & `rucio-34.4.0/lib/rucio/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/alembicrevision.py` & `rucio-34.4.0/lib/rucio/alembicrevision.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/__init__.py` & `rucio-34.4.0/lib/rucio/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/account.py` & `rucio-34.4.0/lib/rucio/api/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from collections.abc import Iterator
+from typing import TYPE_CHECKING, Any, Optional
 
 import rucio.api.permission
 import rucio.common.exception
 import rucio.core.identity
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount
 from rucio.common.utils import api_update_return_dict
@@ -111,29 +112,28 @@
 
     account = InternalAccount(account, vo=vo)
 
     return account_core.update_account(account, key, value, session=session)
 
 
 @stream_session
-def list_accounts(filter_={}, vo='def', *, session: "Session"):
+def list_accounts(filter_: Optional[dict[str, Any]] = None, vo: str = 'def', *, session: "Session") -> Iterator[dict[str, Any]]:
     """
     Lists all the Rucio account names.
 
     REST API: http://<host>:<port>/rucio/accounts
 
     :param filter_: Dictionary of attributes by which the input data should be filtered
     :param vo: The VO to act on.
     :param session: The database session in use.
 
     :returns: List of all accounts.
     """
     # If filter is empty, create a new dict to avoid overwriting the function's default
-    if not filter_:
-        filter_ = {}
+    filter_ = filter_ or {}
 
     if 'account' in filter_:
         filter_['account'] = InternalAccount(filter_['account'], vo=vo)
     else:
         filter_['account'] = InternalAccount(account='*', vo=vo)
     for result in account_core.list_accounts(filter_=filter_, session=session):
         yield api_update_return_dict(result, session=session)
```

### Comparing `rucio-34.3.0/lib/rucio/api/account_limit.py` & `rucio-34.4.0/lib/rucio/api/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/authentication.py` & `rucio-34.4.0/lib/rucio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/config.py` & `rucio-34.4.0/lib/rucio/api/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/credential.py` & `rucio-34.4.0/lib/rucio/api/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/did.py` & `rucio-34.4.0/lib/rucio/api/did.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from collections.abc import Iterator
+from collections.abc import Iterator, Sequence
 from copy import deepcopy
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import rucio.api.permission
 from rucio.common.constants import RESERVED_KEYS
 from rucio.common.exception import RucioException
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import api_update_return_dict
 from rucio.core import did, naming_convention
 from rucio.core import meta_conventions as meta_convention_core
 from rucio.core.rse import get_rse_id
 from rucio.db.sqla.constants import DIDType
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
 
 if TYPE_CHECKING:
-    from typing import Any, Optional
+    from typing import Optional
 
     from sqlalchemy.orm import Session
 
 
 @stream_session
 def list_dids(scope, filters, did_type='collection', ignore_case=False, limit=None, offset=None, long=False, recursive=False, vo='def', *, session: "Session"):
     """
@@ -63,15 +63,30 @@
                            limit=limit, offset=offset, long=long, recursive=recursive, session=session)
 
     for d in result:
         yield api_update_return_dict(d, session=session)
 
 
 @transactional_session
-def add_did(scope, name, did_type, issuer, account=None, statuses={}, meta={}, rules=[], lifetime=None, dids=[], rse=None, vo='def', *, session: "Session"):
+def add_did(
+    scope: str,
+    name: str,
+    did_type: str,
+    issuer: str,
+    account: "Optional[str]" = None,
+    statuses: "Optional[dict[str, str]]" = None,
+    meta: "Optional[dict[str, str]]" = None,
+    rules: "Optional[Sequence[dict[str, Any]]]" = None,
+    lifetime: "Optional[str]" = None,
+    dids: "Optional[Sequence[dict[str, Any]]]" = None,
+    rse: "Optional[str]" = None,
+    vo: str = 'def',
+    *,
+    session: "Session"
+) -> None:
     """
     Add data did.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param did_type: The data identifier type.
     :param issuer: The issuer account.
@@ -81,51 +96,54 @@
     :rules: Replication rules associated with the data did. A list of dictionaries, e.g., [{'copies': 2, 'rse_expression': 'TIERS1'}, ].
     :param lifetime: DID's lifetime (in seconds).
     :param dids: The content.
     :param rse: The RSE name when registering replicas.
     :param vo: The VO to act on.
     :param session: The database session in use.
     """
+    statuses = statuses or {}
+    meta = meta or {}
+    rules = rules or []
+    dids = dids or []
     v_did = {'name': name, 'type': did_type.upper(), 'scope': scope}
     validate_schema(name='did', obj=v_did, vo=vo)
     validate_schema(name='dids', obj=dids, vo=vo)
     validate_schema(name='rse', obj=rse, vo=vo)
     kwargs = {'scope': scope, 'name': name, 'type': did_type, 'issuer': issuer, 'account': account, 'statuses': statuses, 'meta': meta, 'rules': rules, 'lifetime': lifetime}
     if not rucio.api.permission.has_permission(issuer=issuer, vo=vo, action='add_did', kwargs=kwargs, session=session):
         raise rucio.common.exception.AccessDenied('Account %s can not add data identifier to scope %s' % (issuer, scope))
 
-    if account is not None:
-        account = InternalAccount(account, vo=vo)
-    issuer = InternalAccount(issuer, vo=vo)
-    scope = InternalScope(scope, vo=vo)
+    owner_account = None if account is None else InternalAccount(account, vo=vo)
+    issuer_account = InternalAccount(issuer, vo=vo)
+    internal_scope = InternalScope(scope, vo=vo)
     for d in dids:
         d['scope'] = InternalScope(d['scope'], vo=vo)
     for r in rules:
         r['account'] = InternalAccount(r['account'], vo=vo)
 
     rse_id = None
     if rse is not None:
         rse_id = get_rse_id(rse=rse, vo=vo, session=session)
 
     if did_type == 'DATASET':
         # naming_convention validation
-        extra_meta = naming_convention.validate_name(scope=scope, name=name, did_type='D', session=session)
+        extra_meta = naming_convention.validate_name(scope=internal_scope, name=name, did_type='D', session=session)
 
         # merge extra_meta with meta
         for k in extra_meta or {}:
             if k not in meta:
                 meta[k] = extra_meta[k]
             elif meta[k] != extra_meta[k]:
                 print("Provided metadata %s doesn't match the naming convention: %s != %s" % (k, meta[k], extra_meta[k]))
                 raise rucio.common.exception.InvalidObject("Provided metadata %s doesn't match the naming convention: %s != %s" % (k, meta[k], extra_meta[k]))
 
         # Validate metadata
         meta_convention_core.validate_meta(meta=meta, did_type=DIDType[did_type.upper()], session=session)
 
-    return did.add_did(scope=scope, name=name, did_type=DIDType[did_type.upper()], account=account or issuer,
+    return did.add_did(scope=internal_scope, name=name, did_type=DIDType[did_type.upper()], account=owner_account or issuer_account,
                        statuses=statuses, meta=meta, rules=rules, lifetime=lifetime,
                        dids=dids, rse_id=rse_id, session=session)
 
 
 @transactional_session
 def add_dids(dids, issuer, vo='def', *, session: "Session"):
     """
@@ -326,15 +344,15 @@
     dids = did.list_content_history(scope=scope, name=name, session=session)
 
     for d in dids:
         yield api_update_return_dict(d, session=session)
 
 
 @stream_session
-def bulk_list_files(dids: "list[dict[str, Any]]", long: bool = False, vo: str = 'def', *, session: "Session") -> "Iterator[dict[str, Any]]":
+def bulk_list_files(dids: list[dict[str, Any]], long: bool = False, vo: str = 'def', *, session: "Session") -> Iterator[dict[str, Any]]:
     """
     List file contents of a list of data identifiers.
 
     :param dids:       A list of DIDs.
     :param long:       A boolean to choose if more metadata are returned or not.
     :param vo:         The VO to act on.
     :param session:    The database session in use.
```

### Comparing `rucio-34.3.0/lib/rucio/api/dirac.py` & `rucio-34.4.0/lib/rucio/api/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/exporter.py` & `rucio-34.4.0/lib/rucio/api/exporter.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from rucio.api import permission
 from rucio.common import exception
 from rucio.core import exporter
 from rucio.core.rse import get_rse_name
 from rucio.db.sqla.session import read_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @read_session
-def export_data(issuer, distance=True, vo='def', *, session: "Session"):
+def export_data(issuer: str, distance: bool = True, vo: str = 'def', *, session: "Session") -> dict[str, Any]:
     """
     Export data from Rucio.
 
     :param issuer: the issuer.
     :param distance: To enable the reporting of distance.
     :param vo: the VO of the issuer.
     :param session: The database session in use.
```

### Comparing `rucio-34.3.0/lib/rucio/api/heartbeat.py` & `rucio-34.4.0/lib/rucio/api/heartbeat.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from rucio.api import permission
 from rucio.common import exception
 from rucio.core import heartbeat
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
+    from threading import Thread
+
     from sqlalchemy.orm import Session
 
 
 @read_session
-def list_heartbeats(issuer=None, vo='def', *, session: "Session"):
+def list_heartbeats(issuer: Optional[str] = None, vo: str = 'def', *, session: "Session") -> list["heartbeat.HeartbeatDict"]:
     """
     Return a list of tuples of all heartbeats.
 
     :param issuer: The issuer account.
     :param vo: the VO for the issuer.
     :param session: The database session in use.
     :returns: List of tuples [('Executable', 'Hostname', ...), ...]
@@ -37,15 +39,26 @@
     kwargs = {'issuer': issuer}
     if not permission.has_permission(issuer=issuer, vo=vo, action='list_heartbeats', kwargs=kwargs, session=session):
         raise exception.AccessDenied('%s cannot list heartbeats' % issuer)
     return heartbeat.list_heartbeats(session=session)
 
 
 @transactional_session
-def create_heartbeat(executable, hostname, pid, older_than, payload, thread=None, issuer=None, vo='def', *, session: "Session"):
+def create_heartbeat(
+    executable: str,
+    hostname: str,
+    pid: int,
+    older_than: int,
+    payload: Optional[str],
+    thread: Optional["Thread"] = None,
+    issuer: Optional[str] = None,
+    vo: str = 'def',
+    *,
+    session: "Session"
+) -> None:
     """
     Creates a heartbeat.
     :param issuer: The issuer account.
     :param vo: the VO for the issuer.
     :param executable: Executable name as a string, e.g., conveyor-submitter.
     :param hostname: Hostname as a string, e.g., rucio-daemon-prod-01.cern.ch.
     :param pid: UNIX Process ID as a number, e.g., 1234.
```

### Comparing `rucio-34.3.0/lib/rucio/api/identity.py` & `rucio-34.4.0/lib/rucio/api/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/importer.py` & `rucio-34.4.0/lib/rucio/api/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from rucio.api import permission
 from rucio.common import exception
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount
 from rucio.core import importer
 from rucio.db.sqla.session import transactional_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @transactional_session
-def import_data(data, issuer, vo='def', *, session: "Session"):
+def import_data(data: dict[str, Any], issuer: str, vo: str = 'def', *, session: "Session") -> None:
     """
     Import data to add/update/delete records in Rucio.
 
     :param data: data to be imported.
     :param issuer: the issuer.
     :param vo: the VO of the issuer.
     :param session: The database session in use.
```

### Comparing `rucio-34.3.0/lib/rucio/api/lifetime_exception.py` & `rucio-34.4.0/lib/rucio/api/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/lock.py` & `rucio-34.4.0/lib/rucio/api/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/meta_conventions.py` & `rucio-34.4.0/lib/rucio/api/meta_conventions.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,41 +23,41 @@
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from rucio.common.types import InternalAccount
 
 
 @read_session
-def list_keys(*, session: "Session"):
+def list_keys(*, session: "Session") -> list[str]:
     """
     Lists all keys for DID Metadata Conventions.
 
     :param session: The database session in use.
 
     :returns: A list containing all keys.
     """
     return meta_conventions.list_keys(session=session)
 
 
 @read_session
-def list_values(key: str, *, session: "Session"):
+def list_values(key: str, *, session: "Session") -> list[str]:
     """
     Lists all allowed values for a DID key (all values for a key in DID Metadata Conventions).
 
     :param key: the name for the key.
     :param session: The database session in use.
 
 
     :returns: A list containing all values.
     """
     return meta_conventions.list_values(key=key, session=session)
 
 
 @transactional_session
-def add_key(key: str, key_type: Union[KeyType, str], issuer: "InternalAccount", value_type: Optional[str] = None, value_regexp: Optional[str] = None, vo: str = 'def', *, session: "Session"):
+def add_key(key: str, key_type: Union[KeyType, str], issuer: "InternalAccount", value_type: Optional[str] = None, value_regexp: Optional[str] = None, vo: str = 'def', *, session: "Session") -> None:
     """
     Add an allowed key for DID metadata (update the DID Metadata Conventions table with a new key).
 
     :param key: the name for the new key.
     :param key_type: the type of the key: all(container, dataset, file), collection(dataset or container), file, derived(compute from file for collection).
     :param issuer: The issuer account.
     :param value_type: the type of the value, if defined.
@@ -68,15 +68,15 @@
     kwargs = {'key': key, 'key_type': key_type, 'value_type': value_type, 'value_regexp': value_regexp}
     if not has_permission(issuer=issuer, vo=vo, action='add_key', kwargs=kwargs, session=session):
         raise AccessDenied('Account %s can not add key' % (issuer))
     return meta_conventions.add_key(key=key, key_type=key_type, value_type=value_type, value_regexp=value_regexp, session=session)
 
 
 @transactional_session
-def add_value(key: str, value: str, issuer: "InternalAccount", vo: str = 'def', *, session: "Session"):
+def add_value(key: str, value: str, issuer: "InternalAccount", vo: str = 'def', *, session: "Session") -> None:
     """
     Add an allowed value for DID metadata (update a key in DID Metadata Conventions table).
 
     :param key: the name for the key.
     :param value: the value.
     :param vo: the vo to act on.
     :param session: The database session in use.
```

### Comparing `rucio-34.3.0/lib/rucio/api/permission.py` & `rucio-34.4.0/lib/rucio/api/permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from copy import deepcopy
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from rucio.common.exception import RSENotFound
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.core import permission
 from rucio.core.rse import get_rse_id
 from rucio.db.sqla.session import read_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @read_session
-def has_permission(issuer, action, kwargs, vo='def', *, session: "Session"):
+def has_permission(issuer: str, action: str, kwargs: dict[str, Any], vo: str = 'def', *, session: "Session") -> bool:
     """
     Checks if an account has the specified permission to
     execute an action with parameters.
 
     :param issuer:  The Account issuer.
     :param vo:      The VO to check against.
     :param action:  The action (API call) called by the account.
@@ -62,10 +62,10 @@
             r['account'] = InternalAccount(r['account'], vo=vo)
     if 'dids' in kwargs:
         for d in kwargs['dids']:
             if 'rules' in d:
                 for r in d['rules']:
                     r['account'] = InternalAccount(r['account'], vo=vo)
 
-    issuer = InternalAccount(issuer, vo=vo)
+    issuer_account = InternalAccount(issuer, vo=vo)
 
-    return permission.has_permission(issuer=issuer, action=action, kwargs=kwargs, session=session)
+    return permission.has_permission(issuer=issuer_account, action=action, kwargs=kwargs, session=session)
```

### Comparing `rucio-34.3.0/lib/rucio/api/quarantined_replica.py` & `rucio-34.4.0/lib/rucio/api/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/replica.py` & `rucio-34.4.0/lib/rucio/api/replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
-from typing import TYPE_CHECKING
+from collections.abc import Iterator
+from typing import TYPE_CHECKING, Any, Optional
 
 from rucio.api import permission
 from rucio.common import exception
 from rucio.common.constants import SuspiciousAvailability
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import api_update_return_dict, invert_dict
@@ -414,26 +415,27 @@
 
     scope = InternalScope(scope, vo=vo)
     for r in replica.list_dataset_replicas_vp(scope=scope, name=name, deep=deep, session=session):
         yield api_update_return_dict(r, session=session)
 
 
 @stream_session
-def list_datasets_per_rse(rse, filters={}, limit=None, vo='def', *, session: "Session"):
+def list_datasets_per_rse(rse: str, filters: Optional[dict[str, Any]] = None, limit: Optional[int] = None, vo: str = 'def', *, session: "Session") -> Iterator[dict[str, Any]]:
     """
     :param scope: The scope of the dataset.
     :param name: The name of the dataset.
     :param filters: dictionary of attributes by which the results should be filtered.
     :param limit: limit number.
     :param vo: The VO to act on.
     :param session: The database session in use.
 
     :returns: A list of dict dataset replicas
     """
 
+    filters = filters or {}
     rse_id = get_rse_id(rse=rse, vo=vo, session=session)
     if 'scope' in filters:
         filters['scope'] = InternalScope(filters['scope'], vo=vo)
     for r in replica.list_datasets_per_rse(rse_id, filters=filters, limit=limit, session=session):
         yield api_update_return_dict(r, session=session)
```

### Comparing `rucio-34.3.0/lib/rucio/api/request.py` & `rucio-34.4.0/lib/rucio/api/request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/rse.py` & `rucio-34.4.0/lib/rucio/api/rse.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from rucio.api import permission
 from rucio.common import exception
 from rucio.common.schema import validate_schema
 from rucio.common.utils import api_update_return_dict
 from rucio.core import distance as distance_module
 from rucio.core import rse as rse_module
@@ -105,26 +105,25 @@
     if not permission.has_permission(issuer=issuer, vo=vo, action='del_rse', kwargs=kwargs, session=session):
         raise exception.AccessDenied('Account %s can not delete RSE' % (issuer))
 
     return rse_module.del_rse(rse_id, session=session)
 
 
 @read_session
-def list_rses(filters={}, vo='def', *, session: "Session"):
+def list_rses(filters: "Optional[dict[str, Any]]" = None, vo: str = 'def', *, session: "Session") -> list[dict[str, Any]]:
     """
     Lists all RSEs.
 
     :param filters: dictionary of attributes by which the results should be filtered.
     :param vo: The VO to act on.
     :param session: The database session in use.
 
     :returns: List of all RSEs.
     """
-    if not filters:
-        filters = {}
+    filters = filters or {}
 
     filters['vo'] = vo
 
     return rse_module.list_rses(filters=filters, session=session)
 
 
 @transactional_session
```

### Comparing `rucio-34.3.0/lib/rucio/api/rule.py` & `rucio-34.4.0/lib/rucio/api/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, Any
+from collections.abc import Iterator
+from typing import TYPE_CHECKING, Any, Optional
 
 from rucio.api.permission import has_permission
 from rucio.common.config import config_get_bool
 from rucio.common.exception import AccessDenied
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.common.utils import api_update_return_dict
@@ -130,25 +131,24 @@
     if is_multi_vo(session=session) and not has_permission(issuer=issuer, vo=vo, action='access_rule_vo', kwargs=kwargs, session=session):
         raise AccessDenied('Account %s can not access rules at other VOs.' % (issuer))
     result = rule.get_rule(rule_id, session=session)
     return api_update_return_dict(result, session=session)
 
 
 @stream_session
-def list_replication_rules(filters={}, vo='def', *, session: "Session"):
+def list_replication_rules(filters: Optional[dict[str, Any]] = None, vo: str = 'def', *, session: "Session") -> Iterator[dict[str, Any]]:
     """
     Lists replication rules based on a filter.
 
     :param filters: dictionary of attributes by which the results should be filtered.
     :param vo: The VO to act on.
     :param session: The database session in use.
     """
     # If filters is empty, create a new dict to avoid overwriting the function's default
-    if not filters:
-        filters = {}
+    filters = filters or {}
 
     if 'scope' in filters:
         scope = filters['scope']
     else:
         scope = '*'
     filters['scope'] = InternalScope(scope=scope, vo=vo)
```

### Comparing `rucio-34.3.0/lib/rucio/api/scope.py` & `rucio-34.4.0/lib/rucio/api/scope.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,41 +8,40 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
 
 import rucio.api.permission
 import rucio.common.exception
 from rucio.common.schema import validate_schema
 from rucio.common.types import InternalAccount, InternalScope
 from rucio.core import scope as core_scope
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @read_session
-def list_scopes(filter_={}, vo='def', *, session: "Session"):
+def list_scopes(filter_: Optional[dict[str, Any]] = None, vo: str = 'def', *, session: "Session") -> list[str]:
     """
     Lists all scopes.
 
     :param filter_: Dictionary of attributes by which the input data should be filtered
     :param vo: The VO to act on.
     :param session: The database session in use.
 
     :returns: A list containing all scopes.
     """
     # If filter is empty, create a new dict to avoid overwriting the function's default
-    if not filter_:
-        filter_ = {}
+    filter_ = filter_ or {}
 
     if 'scope' in filter_:
         filter_['scope'] = InternalScope(scope=filter_['scope'], vo=vo)
     else:
         filter_['scope'] = InternalScope(scope='*', vo=vo)
     return [scope.external for scope in core_scope.list_scopes(filter_=filter_, session=session)]
```

### Comparing `rucio-34.3.0/lib/rucio/api/subscription.py` & `rucio-34.4.0/lib/rucio/api/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/api/vo.py` & `rucio-34.4.0/lib/rucio/api/vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/__init__.py` & `rucio-34.4.0/lib/rucio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/accountclient.py` & `rucio-34.4.0/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/accountlimitclient.py` & `rucio-34.4.0/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/baseclient.py` & `rucio-34.4.0/lib/rucio/client/baseclient.py`

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

### Comparing `rucio-34.3.0/lib/rucio/client/client.py` & `rucio-34.4.0/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/configclient.py` & `rucio-34.4.0/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/credentialclient.py` & `rucio-34.4.0/lib/rucio/client/credentialclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/didclient.py` & `rucio-34.4.0/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/diracclient.py` & `rucio-34.4.0/lib/rucio/client/diracclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/downloadclient.py` & `rucio-34.4.0/lib/rucio/client/downloadclient.py`

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

### Comparing `rucio-34.3.0/lib/rucio/client/exportclient.py` & `rucio-34.4.0/lib/rucio/client/exportclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/fileclient.py` & `rucio-34.4.0/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/importclient.py` & `rucio-34.4.0/lib/rucio/client/importclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/lifetimeclient.py` & `rucio-34.4.0/lib/rucio/client/lifetimeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/lockclient.py` & `rucio-34.4.0/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/metaconventionsclient.py` & `rucio-34.4.0/lib/rucio/client/metaconventionsclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/pingclient.py` & `rucio-34.4.0/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/replicaclient.py` & `rucio-34.4.0/lib/rucio/client/replicaclient.py`

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

### Comparing `rucio-34.3.0/lib/rucio/client/requestclient.py` & `rucio-34.4.0/lib/rucio/client/requestclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/rseclient.py` & `rucio-34.4.0/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/ruleclient.py` & `rucio-34.4.0/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/scopeclient.py` & `rucio-34.4.0/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/subscriptionclient.py` & `rucio-34.4.0/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/touchclient.py` & `rucio-34.4.0/lib/rucio/client/touchclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/client/uploadclient.py` & `rucio-34.4.0/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/__init__.py` & `rucio-34.4.0/lib/rucio/common/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/cache.py` & `rucio-34.4.0/lib/rucio/common/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/config.py` & `rucio-34.4.0/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/constants.py` & `rucio-34.4.0/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/constraints.py` & `rucio-34.4.0/lib/rucio/common/constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/didtype.py` & `rucio-34.4.0/lib/rucio/common/didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/dumper/__init__.py` & `rucio-34.4.0/lib/rucio/common/dumper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/dumper/consistency.py` & `rucio-34.4.0/lib/rucio/common/dumper/consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/dumper/data_models.py` & `rucio-34.4.0/lib/rucio/common/dumper/data_models.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/dumper/path_parsing.py` & `rucio-34.4.0/lib/rucio/common/dumper/path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/exception.py` & `rucio-34.4.0/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/extra.py` & `rucio-34.4.0/lib/rucio/common/extra.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/logging.py` & `rucio-34.4.0/lib/rucio/common/logging.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/pcache.py` & `rucio-34.4.0/lib/rucio/common/pcache.py`

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

### Comparing `rucio-34.3.0/lib/rucio/common/plugins.py` & `rucio-34.4.0/lib/rucio/common/plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/policy.py` & `rucio-34.4.0/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/schema/__init__.py` & `rucio-34.4.0/lib/rucio/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/schema/atlas.py` & `rucio-34.4.0/lib/rucio/common/schema/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/schema/belleii.py` & `rucio-34.4.0/lib/rucio/common/schema/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/schema/cms.py` & `rucio-34.4.0/lib/rucio/common/schema/generic.py`

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

### Comparing `rucio-34.3.0/lib/rucio/common/schema/domatpc.py` & `rucio-34.4.0/lib/rucio/common/schema/domatpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/schema/escape.py` & `rucio-34.4.0/lib/rucio/common/schema/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/schema/generic.py` & `rucio-34.4.0/lib/rucio/common/schema/icecube.py`

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

### Comparing `rucio-34.3.0/lib/rucio/common/schema/generic_multi_vo.py` & `rucio-34.4.0/lib/rucio/common/schema/generic_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/stomp_utils.py` & `rucio-34.4.0/lib/rucio/common/stomp_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/stopwatch.py` & `rucio-34.4.0/lib/rucio/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/test_rucio_server.py` & `rucio-34.4.0/lib/rucio/common/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/common/types.py` & `rucio-34.4.0/lib/rucio/common/types.py`

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

### Comparing `rucio-34.3.0/lib/rucio/common/utils.py` & `rucio-34.4.0/lib/rucio/common/utils.py`

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

### Comparing `rucio-34.3.0/lib/rucio/core/__init__.py` & `rucio-34.4.0/lib/rucio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/account.py` & `rucio-34.4.0/lib/rucio/core/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/account_counter.py` & `rucio-34.4.0/lib/rucio/core/account_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/account_limit.py` & `rucio-34.4.0/lib/rucio/core/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/authentication.py` & `rucio-34.4.0/lib/rucio/core/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 import datetime
 import hashlib
 import random
 import re
 import sys
 import traceback
 from base64 import b64decode
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, Union, cast
 
 import paramiko
 from dogpile.cache import make_region
-from dogpile.cache.api import NO_VALUE
+from dogpile.cache.api import NO_VALUE, NoValue
 from sqlalchemy import delete, null, or_, select
 
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get_bool
 from rucio.common.exception import CannotAuthenticate, RucioException
 from rucio.common.utils import chunks, date_to_str, generate_uuid
 from rucio.core.account import account_exists
 from rucio.core.oidc import validate_jwt
 from rucio.db.sqla import filter_thread_work, models
 from rucio.db.sqla.constants import IdentityType
 from rucio.db.sqla.session import read_session, transactional_session
 
 if TYPE_CHECKING:
-    from typing import Any, Union
-
     from sqlalchemy.orm import Session
 
+    from rucio.common.types import InternalAccount, TokenDict, TokenValidationDict
+
 
 def strip_x509_proxy_attributes(dn: str) -> str:
     """Strip X509 proxy attributes from a DN.
 
     When an X509 VOMS proxy certificate is produced, an additional Common Name
     attribute is added to the subject of the original certificate.  Its value
     can take different forms.  For proxy versions 3 and later (the default), the
@@ -85,15 +85,23 @@
 if config_get_bool('cache', 'use_external_cache_for_auth_tokens', default=False):
     TOKENREGION = make_region_memcached(expiration_time=900, function_key_generator=token_key_generator)
 else:
     TOKENREGION = make_region(function_key_generator=token_key_generator).configure('dogpile.cache.memory', expiration_time=900)
 
 
 @transactional_session
-def get_auth_token_user_pass(account, username, password, appid, ip=None, *, session: "Session"):
+def get_auth_token_user_pass(
+    account: "InternalAccount",
+    username: str,
+    password: str,
+    appid: str,
+    ip: Optional[str] = None,
+    *,
+    session: "Session"
+) -> Optional["TokenDict"]:
     """
     Authenticate a Rucio account temporarily via username and password.
 
     The token lifetime is 1 hour.
 
     :param account: Account identifier as a string.
     :param username: Username as a string.
@@ -145,15 +153,22 @@
     new_token = models.Token(account=db_account, identity=username, token=token, ip=ip)
     new_token.save(session=session)
 
     return token_dictionary(new_token)
 
 
 @transactional_session
-def get_auth_token_x509(account, dn, appid, ip=None, *, session: "Session"):
+def get_auth_token_x509(
+    account: "InternalAccount",
+    dn: str,
+    appid: str,
+    ip: Optional[str] = None,
+    *,
+    session: "Session"
+) -> Optional["TokenDict"]:
     """
     Authenticate a Rucio account temporarily via an x509 certificate.
 
     The token lifetime is 1 hour.
 
     :param account: Account identifier as a string.
     :param dn: Client certificate distinguished name string, as extracted by Apache/mod_ssl.
@@ -177,15 +192,22 @@
     new_token = models.Token(account=account, identity=dn, token=token, ip=ip)
     new_token.save(session=session)
 
     return token_dictionary(new_token)
 
 
 @transactional_session
-def get_auth_token_gss(account, gsstoken, appid, ip=None, *, session: "Session"):
+def get_auth_token_gss(
+    account: "InternalAccount",
+    gsstoken: str,
+    appid: str,
+    ip: Optional[str] = None,
+    *,
+    session: "Session"
+) -> Optional["TokenDict"]:
     """
     Authenticate a Rucio account temporarily via a GSS token.
 
     The token lifetime is 1 hour.
 
     :param account: Account identifier as a string.
     :param gsscred: GSS principal@REALM as a string.
@@ -209,15 +231,22 @@
     new_token = models.Token(account=account, token=token, ip=ip)
     new_token.save(session=session)
 
     return token_dictionary(new_token)
 
 
 @transactional_session
-def get_auth_token_ssh(account, signature, appid, ip=None, *, session: "Session"):
+def get_auth_token_ssh(
+    account: "InternalAccount",
+    signature: str,
+    appid: str,
+    ip: Optional[str] = None,
+    *,
+    session: "Session"
+) -> Optional["TokenDict"]:
     """
     Authenticate a Rucio account temporarily via SSH key exchange.
 
     The token lifetime is 1 hour.
 
     :param account: Account identifier as a string.
     :param signature: Response to server challenge signed with SSH private key as a base64 encoded string.
@@ -227,15 +256,15 @@
 
     :returns: A dict with token and expires_at entries.
     """
 
     # decode the signature which must come in base64 encoded
     try:
         signature += '=' * ((4 - len(signature) % 4) % 4)  # adding required padding
-        signature = b64decode(signature)
+        decoded_signature = b64decode(signature)
     except TypeError:
         raise CannotAuthenticate(f'Cannot authenticate to account {account} with malformed signature')
 
     # Make sure the account exists
     if not account_exists(account, session=session):
         return None
 
@@ -266,15 +295,15 @@
     match = False
     for identity in identities:
         data = identity['identity'].split()[1]
         data += '=' * ((4 - len(data) % 4) % 4)  # adding required padding
         pub_k = paramiko.RSAKey(data=b64decode(data))
         for challenge_token in active_challenge_tokens:
             if pub_k.verify_ssh_sig(str(challenge_token['token']).encode(),
-                                    paramiko.Message(signature)):
+                                    paramiko.Message(decoded_signature)):
                 match = True
                 break
         if match:
             break
 
     if not match:
         return None
@@ -288,15 +317,21 @@
     new_token = models.Token(account=account, token=token, ip=ip)
     new_token.save(session=session)
 
     return token_dictionary(new_token)
 
 
 @transactional_session
-def get_ssh_challenge_token(account, appid, ip=None, *, session: "Session"):
+def get_ssh_challenge_token(
+    account: "InternalAccount",
+    appid: str,
+    ip: Optional[str] = None,
+    *,
+    session: "Session"
+) -> Optional["TokenDict"]:
     """
     Prepare a challenge token for subsequent SSH public key authentication.
 
     The challenge lifetime is fixed to 10 seconds.
 
     :param account: Account identifier as a string.
     :param appid: The application identifier as a string.
@@ -324,15 +359,22 @@
                                        expired_at=expiration)
     new_challenge_token.save(session=session)
 
     return token_dictionary(new_challenge_token)
 
 
 @transactional_session
-def get_auth_token_saml(account, saml_nameid, appid, ip=None, *, session: "Session"):
+def get_auth_token_saml(
+    account: "InternalAccount",
+    saml_nameid: str,
+    appid: str,
+    ip: Optional[str] = None,
+    *,
+    session: "Session"
+) -> Optional["TokenDict"]:
     """
     Authenticate a Rucio account temporarily via SAML.
 
     The token lifetime is 1 hour.
 
     :param account: Account identifier as a string.
     :param saml_nameid: SAML NameID of the client.
@@ -355,15 +397,20 @@
     new_token = models.Token(account=account, identity=saml_nameid, token=token, ip=ip)
     new_token.save(session=session)
 
     return token_dictionary(new_token)
 
 
 @transactional_session
-def redirect_auth_oidc(auth_code, fetchtoken=False, *, session: "Session"):
+def redirect_auth_oidc(
+    auth_code: str,
+    fetchtoken: bool = False,
+    *,
+    session: "Session"
+) -> Optional[str]:
     """
     Finds the Authentication URL in the Rucio DB oauth_requests table
     and redirects user's browser to this URL.
 
     :param auth_code: Rucio assigned code to redirect
                       authorization securely to IdP via Rucio Auth server through a browser.
     :param fetchtoken: If True, valid token temporarily saved in the oauth_requests table
@@ -396,15 +443,21 @@
             # return redirection URL
             return redirect_result
     except:
         raise CannotAuthenticate(traceback.format_exc())
 
 
 @transactional_session
-def delete_expired_tokens(total_workers, worker_number, limit=1000, *, session: "Session"):
+def delete_expired_tokens(
+    total_workers: int,
+    worker_number: int,
+    limit: int = 1000,
+    *,
+    session: "Session"
+) -> int:
     """
     Delete expired tokens.
 
     :param total_workers:      Number of total workers.
     :param worker_number:      id of the executing worker.
     :param limit:              Maximum number of tokens to delete.
     :param session:            Database session in use.
@@ -456,15 +509,15 @@
     except Exception as error:
         raise RucioException(error.args)
 
     return deleted_tokens
 
 
 @read_session
-def query_token(token, *, session: "Session"):
+def query_token(token: str, *, session: "Session") -> Optional["TokenValidationDict"]:
     """
     Validate an authentication token using the database. This method will only be called
     if no entry could be found in the according cache.
 
     :param token: Authentication token as a variable-length string.
     :param session: The database session in use.
 
@@ -484,20 +537,20 @@
         models.Token.oidc_scope.label('authz_scope')
     ).where(
         models.Token.token == token,
         models.Token.expired_at > datetime.datetime.utcnow()
     )
     result = session.execute(query).first()
     if result:
-        return result._asdict()
+        return cast("TokenValidationDict", result._asdict())
     return None
 
 
 @transactional_session
-def validate_auth_token(token: str, *, session: "Session") -> "dict[str, Any]":
+def validate_auth_token(token: str, *, session: "Session") -> "TokenValidationDict":
     """
     Validate an authentication token.
 
     :param token: Authentication token as a variable-length string.
 
     :returns: dictionary { account: <account name>,
                            identity: <identity>,
@@ -510,40 +563,40 @@
     if not token:
         raise CannotAuthenticate("No token was passed!")
 
     # Be gentle with bash variables, there can be whitespace
     token = token.strip()
     cache_key = token.replace(' ', '')
 
-    # Check if token ca be found in cache region
-    value: "Union[NO_VALUE, dict[str, Any]]" = TOKENREGION.get(cache_key)
+    # Check if token can be found in cache region
+    value: Union[NoValue, "TokenValidationDict"] = TOKENREGION.get(cache_key)
     if value is NO_VALUE:  # no cached entry found
         value = query_token(token, session=session)
         if not value:
             # identify JWT access token and validate
             # & save it in Rucio if scope and audience are correct
             if len(token.split(".")) == 3:
                 value = validate_jwt(token, session=session)
             else:
                 raise CannotAuthenticate(traceback.format_exc())
         # save token in the cache
         TOKENREGION.set(cache_key, value)
-    lifetime = value.get('lifetime', datetime.datetime(1970, 1, 1))
+    lifetime = value.get('lifetime', datetime.datetime(1970, 1, 1))  # type: ignore (value is narrowed to dict, but type-checker doesn't see it)
     if lifetime < datetime.datetime.utcnow():  # check if expired
         TOKENREGION.delete(cache_key)
         raise CannotAuthenticate(f"Token found but expired since {date_to_str(lifetime)}.")
-    return value
+    return cast("TokenValidationDict", value)
 
 
-def token_dictionary(token: models.Token):
+def token_dictionary(token: models.Token) -> "TokenDict":
     return {'token': token.token, 'expires_at': token.expired_at}
 
 
 @transactional_session
-def __delete_expired_tokens_account(account, *, session: "Session"):
+def __delete_expired_tokens_account(account: "InternalAccount", *, session: "Session") -> None:
     """"
     Deletes expired tokens from the database.
 
     :param account: Account to delete expired tokens.
     :param session: The database session in use.
     """
     select_query = select(
```

### Comparing `rucio-34.3.0/lib/rucio/core/config.py` & `rucio-34.4.0/lib/rucio/core/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/credential.py` & `rucio-34.4.0/lib/rucio/core/credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/did.py` & `rucio-34.4.0/lib/rucio/core/did.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import logging
 import random
 from datetime import datetime, timedelta
 from enum import Enum
 from hashlib import md5
 from re import match
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 
 from sqlalchemy import and_, delete, exists, insert, or_, update
 from sqlalchemy.exc import DatabaseError, IntegrityError, NoResultFound
 from sqlalchemy.sql import func, not_
 from sqlalchemy.sql.expression import bindparam, case, false, null, select, true
 
 import rucio.core.replica  # import add_replicas
@@ -36,34 +36,34 @@
 from rucio.core.naming_convention import validate_name
 from rucio.db.sqla import filter_thread_work, models
 from rucio.db.sqla.constants import BadFilesStatus, DIDAvailability, DIDReEvaluation, DIDType, RuleState
 from rucio.db.sqla.session import read_session, stream_session, transactional_session
 from rucio.db.sqla.util import temp_table_mngr
 
 if TYPE_CHECKING:
-    from collections.abc import Iterator, Sequence
-    from typing import Any, Optional, Union
+    from collections.abc import Iterable, Iterator, Mapping, Sequence
 
     from sqlalchemy.orm import Session
-    from sqlalchemy.schema import Table
+    from sqlalchemy.sql._typing import ColumnExpressionArgument
+    from sqlalchemy.sql.selectable import Select
 
     from rucio.common.types import InternalAccount, InternalScope, LoggerFunction
 
 
 METRICS = MetricManager(module=__name__)
 
 
 @read_session
 def list_expired_dids(
-        worker_number: int = None,
-        total_workers: int = None,
-        limit: int = None,
+        worker_number: Optional[int] = None,
+        total_workers: Optional[int] = None,
+        limit: Optional[int] = None,
         *,
         session: "Session"
-):
+) -> list[dict[str, Any]]:
     """
     List expired data identifiers.
 
     :param limit: limit number.
     :param session: The database session in use.
     """
 
@@ -115,25 +115,25 @@
              'purge_replicas': purge_replicas} for scope, name, did_type, created_at, purge_replicas in session.execute(list_stmt)]
 
 
 @transactional_session
 def add_did(
         scope: "InternalScope",
         name: str,
-        did_type: "Union[str, DIDType]",
+        did_type: Union[str, DIDType],
         account: "InternalAccount",
-        statuses: "Optional[dict[str, Any]]" = None,
-        meta: "Optional[dict[str, Any]]" = None,
-        rules: "Optional[Sequence[str]]" = None,
-        lifetime: "Optional[int]" = None,
-        dids: "Optional[Sequence[dict[str, Any]]]" = None,
-        rse_id: "Optional[str]" = None,
+        statuses: Optional["Mapping[str, Any]"] = None,
+        meta: Optional["Mapping[str, Any]"] = None,
+        rules: Optional["Sequence[str]"] = None,
+        lifetime: Optional[int] = None,
+        dids: Optional["Sequence[Mapping[str, Any]]"] = None,
+        rse_id: Optional[str] = None,
         *,
         session: "Session",
-):
+) -> None:
     """
     Add data identifier.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param did_type: The data identifier type.
     :param account: The account owner.
@@ -154,15 +154,15 @@
 
 @transactional_session
 def add_dids(
         dids: "Sequence[dict[str, Any]]",
         account: "InternalAccount",
         *,
         session: "Session",
-):
+) -> None:
     """
     Bulk add data identifiers.
 
     :param dids: A list of dids.
     :param account: The account owner.
     :param session: The database session in use.
     """
@@ -246,20 +246,20 @@
         raise exception.RucioException(error.args)
 
 
 @transactional_session
 def attach_dids(
         scope: "InternalScope",
         name: str,
-        dids: "Sequence[dict[str, Any]]",
+        dids: "Sequence[Mapping[str, Any]]",
         account: "InternalAccount",
-        rse_id: "Optional[str]" = None,
+        rse_id: Optional[str] = None,
         *,
         session: "Session",
-):
+) -> None:
     """
     Append data identifier.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param dids: The content.
     :param account: The account owner.
@@ -267,20 +267,20 @@
     :param session: The database session in use.
     """
     return attach_dids_to_dids(attachments=[{'scope': scope, 'name': name, 'dids': dids, 'rse_id': rse_id}], account=account, session=session)
 
 
 @transactional_session
 def attach_dids_to_dids(
-        attachments: "dict[str, Any]",
+        attachments: "Sequence[Mapping[str, Any]]",
         account: "InternalAccount",
         ignore_duplicate: bool = False,
         *,
         session: "Session",
-):
+) -> None:
     children_temp_table = temp_table_mngr(session).create_scope_name_table()
     parent_dids = list()
     first_iteration = True
     for attachment in attachments:
         try:
             children = {(a['scope'], a['name']): a for a in attachment['dids']}
             cont = []
@@ -345,15 +345,23 @@
     # (convert the list of dictionaries into a list of tuple, then to a set of tuple
     # to remove duplicates, then back to a list of unique dictionaries)
     parent_dids = [dict(tup) for tup in set(tuple(dictionary.items()) for dictionary in parent_dids)]
     if parent_dids:
         session.execute(insert(models.UpdatedDID), parent_dids)
 
 
-def __add_files_to_archive(parent_did, files_temp_table, files, account, ignore_duplicate=False, *, session: "Session"):
+def __add_files_to_archive(
+        parent_did: models.DataIdentifier,
+        files_temp_table: Any,
+        files: "Mapping[tuple[InternalScope, str], Mapping[str, Any]]",
+        account: "InternalAccount",
+        ignore_duplicate: bool = False,
+        *,
+        session: "Session"
+) -> None:
     """
     Add files to archive.
 
     :param parent_did: the DataIdentifier object of the parent did
     :param files: archive content.
     :param account: The account owner.
     :param ignore_duplicate: If True, ignore duplicate entries.
@@ -500,15 +508,24 @@
         ).values(
             is_archive=True
         )
         session.execute(stmt)
 
 
 @transactional_session
-def __add_files_to_dataset(parent_did, files_temp_table, files, account, rse_id, ignore_duplicate=False, *, session: "Session"):
+def __add_files_to_dataset(
+    parent_did: models.DataIdentifier,
+    files_temp_table: Any,
+    files: "Mapping[tuple[InternalScope, str], Mapping[str, Any]]",
+    account: "InternalAccount",
+    rse_id: str,
+    ignore_duplicate: bool = False,
+    *,
+    session: "Session"
+) -> dict[tuple["InternalScope", str], dict[str, Any]]:
     """
     Add files to dataset.
 
     :param parent_did:         the DataIdentifier object of the parent did
     :param files_temp_table:   Temporary table containing the scope and name of files to add.
     :param account:            The account owner.
     :param rse_id:             The RSE id for the replicas.
@@ -625,15 +642,22 @@
                 or match('.*IntegrityError.*columns? .*not unique.*', error.args[0]):
             raise exception.FileAlreadyExists(error.args)
         else:
             raise exception.RucioException(error.args)
 
 
 @transactional_session
-def __add_collections_to_container(parent_did, collections_temp_table, collections, account, *, session: "Session"):
+def __add_collections_to_container(
+    parent_did: models.DataIdentifier,
+    collections_temp_table: Any,
+    collections: "Mapping[tuple[InternalScope, str], Mapping[str, Any]]",
+    account: "InternalAccount",
+    *,
+    session: "Session"
+) -> None:
     """
     Add collections (datasets or containers) to container.
 
     :param parent_did: the DataIdentifier object of the parent did
     :param collections: .
     :param account: The account owner.
     :param session: The database session in use.
@@ -725,15 +749,23 @@
                 or match('.*IntegrityError.*duplicate key value violates unique constraint.*', error.args[0]) \
                 or match('.*UniqueViolation.*duplicate key value violates unique constraint.*', error.args[0]) \
                 or match('.*IntegrityError.* UNIQUE constraint failed: contents.scope, contents.name, contents.child_scope, contents.child_name.*', error.args[0]):
             raise exception.DuplicateContent(error.args)
         raise exception.RucioException(error.args)
 
 
-def __add_files_to_archive_without_temp_tables(scope, name, files, account, ignore_duplicate=False, *, session: "Session"):
+def __add_files_to_archive_without_temp_tables(
+        scope: "InternalScope",
+        name: str,
+        files: "Sequence[dict[str, Any]]",
+        account: "InternalAccount",
+        ignore_duplicate: bool = False,
+        *,
+        session: "Session"
+) -> None:
     """
     Add files to archive.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param files: archive content.
     :param account: The account owner.
@@ -882,15 +914,24 @@
         ).values(
             is_archive=True
         )
         session.execute(stmt)
 
 
 @transactional_session
-def __add_files_to_dataset_without_temp_tables(scope, name, files, account, rse_id, ignore_duplicate=False, *, session: "Session"):
+def __add_files_to_dataset_without_temp_tables(
+    scope: "InternalScope",
+    name: str,
+    files: "Sequence[Mapping[str, str]]",
+    account: "InternalAccount",
+    rse_id: str,
+    ignore_duplicate: bool = False,
+    *,
+    session: "Session"
+) -> list[dict[str, Any]]:
     """
     Add files to dataset.
 
     :param scope:              The scope name.
     :param name:               The data identifier name.
     :param files:              The list of files.
     :param account:            The account owner.
@@ -988,15 +1029,22 @@
                 or match('.*IntegrityError.*columns? .*not unique.*', error.args[0]):
             raise exception.FileAlreadyExists(error.args)
         else:
             raise exception.RucioException(error.args)
 
 
 @transactional_session
-def __add_collections_to_container_without_temp_tables(scope, name, collections, account, *, session: "Session"):
+def __add_collections_to_container_without_temp_tables(
+    scope: "InternalScope",
+    name: str,
+    collections: "Sequence[Mapping[str, Any]]",
+    account: "InternalAccount",
+    *,
+    session: "Session"
+) -> None:
     """
     Add collections (datasets or containers) to container.
 
     :param scope: The scope name.
     :param name: The container name.
     :param collections: .
     :param account: The account owner.
@@ -1091,21 +1139,21 @@
                 or match('.*IntegrityError.* UNIQUE constraint failed: contents.scope, contents.name, contents.child_scope, contents.child_name.*', error.args[0]):
             raise exception.DuplicateContent(error.args)
         raise exception.RucioException(error.args)
 
 
 @transactional_session
 def delete_dids(
-        dids: "Sequence[dict[str, Any]]",
+        dids: "Sequence[Mapping[str, Any]]",
         account: "InternalAccount",
         expire_rules: bool = False,
         *,
         session: "Session",
         logger: "LoggerFunction" = logging.log,
-):
+) -> None:
     """
     Delete data identifiers
 
     :param dids:          The list of dids to delete.
     :param account:       The account.
     :param expire_rules:  Expire large rules instead of deleting them right away. This should only be used in Undertaker mode, as it can be that
                           the method returns normally, but a did was not deleted; This trusts in the fact that the undertaker will retry an
@@ -1436,15 +1484,21 @@
         ).values(
             expired_at=None
         )
         session.execute(stmt)
 
 
 @transactional_session
-def detach_dids(scope, name, dids, *, session: "Session"):
+def detach_dids(
+    scope: "InternalScope",
+    name: str,
+    dids: "Sequence[Mapping[str, Any]]",
+    *,
+    session: "Session"
+) -> None:
     """
     Detach data identifier
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param dids: The content.
     :param session: The database session in use.
@@ -1556,15 +1610,22 @@
         if scope.vo != 'def':
             message['vo'] = scope.vo
 
         add_message('DETACH', message, session=session)
 
 
 @stream_session
-def list_new_dids(did_type, thread=None, total_threads=None, chunk_size=1000, *, session: "Session"):
+def list_new_dids(
+    did_type: Union[str, "DIDType"],
+    thread: Optional[int] = None,
+    total_threads: Optional[int] = None,
+    chunk_size: int = 1000,
+    *,
+    session: "Session",
+) -> "Iterator[dict[str, Any]]":
     """
     List recent identifiers.
 
     :param did_type : The DID type.
     :param thread: The assigned thread for this necromancer.
     :param total_threads: The total number of threads of all necromancers.
     :param chunk_size: Number of requests to return per yield.
@@ -1605,15 +1666,20 @@
         if row_count <= chunk_size:
             yield {'scope': chunk.scope, 'name': chunk.name, 'did_type': chunk.did_type}  # TODO Change this to the proper filebytes [RUCIO-199]
         else:
             break
 
 
 @transactional_session
-def set_new_dids(dids, new_flag, *, session: "Session"):
+def set_new_dids(
+    dids: "Sequence[Mapping[str, Any]]",
+    new_flag: Optional[bool],
+    *,
+    session: "Session"
+) -> bool:
     """
     Set/reset the flag new
 
     :param dids: A list of dids
     :param new_flag: A boolean to flag new DIDs.
     :param session: The database session in use.
     """
@@ -1642,15 +1708,20 @@
         raise exception.RucioException(error.args[0])
     except DatabaseError as error:
         raise exception.RucioException(error.args[0])
     return True
 
 
 @stream_session
-def list_content(scope, name, *, session: "Session"):
+def list_content(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List data identifier contents.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param session: The database session in use.
     """
@@ -1669,15 +1740,20 @@
                'bytes': tmp_did.bytes, 'adler32': tmp_did.adler32, 'md5': tmp_did.md5}
     if not children_found:
         # Raise exception if the did doesn't exist
         __get_did(scope=scope, name=name, session=session)
 
 
 @stream_session
-def list_content_history(scope, name, *, session: "Session"):
+def list_content_history(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List data identifier contents history.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param session: The database session in use.
     """
@@ -1695,15 +1771,20 @@
                    'deleted_at': tmp_did.deleted_at, 'created_at': tmp_did.created_at,
                    'updated_at': tmp_did.updated_at}
     except NoResultFound:
         raise exception.DataIdentifierNotFound(f"Data identifier '{scope}:{name}' not found")
 
 
 @stream_session
-def list_parent_dids(scope, name, *, session: "Session"):
+def list_parent_dids(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List parent datasets and containers of a did.
 
     :param scope:     The scope.
     :param name:      The name.
     :param session:   The database session.
     :returns:         List of dids.
@@ -1719,15 +1800,20 @@
         child_name=name
     )
     for did in session.execute(stmt).yield_per(5):
         yield {'scope': did.scope, 'name': did.name, 'type': did.did_type}
 
 
 @stream_session
-def list_all_parent_dids(scope, name, *, session: "Session"):
+def list_all_parent_dids(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List all parent datasets and containers of a did, no matter on what level.
 
     :param scope:     The scope.
     :param name:      The name.
     :param session:   The database session.
     :returns:         List of dids.
@@ -1746,17 +1832,17 @@
         yield {'scope': did.scope, 'name': did.name, 'type': did.did_type}
         # Note that only Python3 supports recursive yield, that's the reason to do the nested for.
         for pdid in list_all_parent_dids(scope=did.scope, name=did.name, session=session):
             yield {'scope': pdid['scope'], 'name': pdid['name'], 'type': pdid['type']}
 
 
 def list_child_dids_stmt(
-        input_dids_table: "Table",
+        input_dids_table: Any,
         did_type: DIDType,
-):
+) -> "Select[tuple[InternalScope, str]]":
     """
     Build and returns a query which recursively lists children dids of type `did_type`
     for the dids given as input in a scope/name (temporary) table.
 
     did_type defines the desired type of DIDs in the result. If set to DIDType.Dataset,
     will only resolve containers and return datasets. If set to DIDType.File, will
     also resolve the datasets and return files.
@@ -1807,15 +1893,15 @@
     return stmt
 
 
 def list_one_did_childs_stmt(
         scope: "InternalScope",
         name: str,
         did_type: DIDType,
-):
+) -> "Select[tuple[InternalScope, str]]":
     """
     Returns the sqlalchemy query for recursively fetching the child dids of type
     'did_type' for the input did.
 
     did_type defines the desired type of DIDs in the result. If set to DIDType.Dataset,
     will only resolve containers and return datasets. If set to DIDType.File, will
     also resolve the datasets and return files.
@@ -1864,15 +1950,15 @@
 
 @transactional_session
 def list_child_datasets(
         scope: "InternalScope",
         name: str,
         *,
         session: "Session"
-):
+) -> list[dict[str, Union["InternalScope", str]]]:
     """
     List all child datasets of a container.
 
     :param scope:     The scope.
     :param name:      The name.
     :param session:   The database session
     :returns:         List of dids
@@ -1883,15 +1969,20 @@
     for row in session.execute(stmt):
         result.append({'scope': row.scope, 'name': row.name})
 
     return result
 
 
 @stream_session
-def bulk_list_files(dids: "list[dict[str, Any]]", long: bool = False, *, session: "Session") -> "Optional[Iterator[dict[str, Any]]]":
+def bulk_list_files(
+    dids: "Iterable[Mapping[str, Any]]",
+    long: bool = False,
+    *,
+    session: "Session"
+) -> "Optional[Iterator[dict[str, Any]]]":
     """
     List file contents of a list of data identifier.
 
     :param dids:       A list of DIDs.
     :param long:       A boolean to choose if more metadata are returned or not.
     :param session:    The database session in use.
     """
@@ -2008,15 +2099,21 @@
                         dids.append((child_scope, child_name, child_type))
 
     except NoResultFound:
         raise exception.DataIdentifierNotFound(f"Data identifier '{scope}:{name}' not found")
 
 
 @stream_session
-def scope_list(scope, name=None, recursive=False, *, session: "Session"):
+def scope_list(
+    scope: "InternalScope",
+    name: Optional[str] = None,
+    recursive: bool = False,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List data identifiers in a scope.
 
     :param scope: The scope name.
     :param session: The database session in use.
     :param name: The data identifier name.
     :param recursive: boolean, True or False.
@@ -2046,15 +2143,15 @@
         )
         for row in session.execute(stmt).yield_per(5):
             if row.did_type == DIDType.FILE:
                 yield {'scope': scope, 'name': row.name, 'type': row.did_type, 'parent': None, 'level': 0, 'bytes': row.bytes}
             else:
                 yield {'scope': scope, 'name': row.name, 'type': row.did_type, 'parent': None, 'level': 0, 'bytes': None}
 
-    def __diddriller(pdid):
+    def __diddriller(pdid: "Mapping[str, Any]") -> "Iterator[dict[str, Any]]":
         stmt = select(
             models.DataIdentifierAssociation
         ).filter_by(
             scope=pdid['scope'],
             name=pdid['name']
         ).order_by(
             models.DataIdentifierAssociation.child_name
@@ -2092,15 +2189,20 @@
     else:
         for topdid in topdids:
             for did in __diddriller(topdid):
                 yield did
 
 
 @read_session
-def __get_did(scope, name, *, session: "Session"):
+def __get_did(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> "models.DataIdentifier":
     try:
         stmt = select(
             models.DataIdentifier
         ).with_hint(
             models.DataIdentifier, "INDEX(DIDS DIDS_PK)", 'oracle'
         ).where(
             models.DataIdentifier.scope == scope,
@@ -2137,15 +2239,15 @@
         return {'scope': did.scope, 'name': did.name, 'type': did.did_type,
                 'account': did.account, 'open': did.is_open,
                 'monotonic': did.monotonic, 'expired_at': did.expired_at,
                 'length': length, 'bytes': bytes_}
 
 
 @read_session
-def get_files(files, *, session: "Session"):
+def get_files(files: "Sequence[Mapping[str, Any]]", *, session: "Session") -> list[dict[str, Any]]:
     """
     Retrieve a list of files.
 
     :param files: A list of files (dictionaries).
     :param session: The database session in use.
     """
     file_condition = []
@@ -2192,16 +2294,25 @@
                     break
             if not found:
                 raise exception.DataIdentifierNotFound("Data identifier '%(scope)s:%(name)s' not found" % file)
     return rows
 
 
 @transactional_session
-def set_metadata(scope, name, key, value, did_type=None, did=None,
-                 recursive=False, *, session: "Session"):
+def set_metadata(
+    scope: "InternalScope",
+    name: str,
+    key: str,
+    value: Any,
+    did_type: Optional[DIDType] = None,
+    did: Optional["Mapping[str, Any]"] = None,
+    recursive: bool = False,
+    *,
+    session: "Session"
+) -> None:
     """
     Add single metadata to a data identifier.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param key: the key.
     :param value: the value.
@@ -2209,57 +2320,79 @@
     :param recursive: Option to propagate the metadata change to content.
     :param session: The database session in use.
     """
     did_meta_plugins.set_metadata(scope=scope, name=name, key=key, value=value, recursive=recursive, session=session)
 
 
 @transactional_session
-def set_metadata_bulk(scope, name, meta, recursive=False, *, session: "Session"):
+def set_metadata_bulk(
+    scope: "InternalScope",
+    name: str,
+    meta: "Mapping[str, Any]",
+    recursive: bool = False,
+    *,
+    session: "Session"
+) -> None:
     """
     Add metadata to a data identifier.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param meta: the key-values.
     :param recursive: Option to propagate the metadata change to content.
     :param session: The database session in use.
     """
     did_meta_plugins.set_metadata_bulk(scope=scope, name=name, meta=meta, recursive=recursive, session=session)
 
 
 @transactional_session
-def set_dids_metadata_bulk(dids, recursive=False, *, session: "Session"):
+def set_dids_metadata_bulk(
+    dids: "Iterable[Mapping[str, Any]]",
+    recursive: bool = False,
+    *,
+    session: "Session"
+) -> None:
     """
     Add metadata to a list of data identifiers.
 
     :param dids: A list of dids including metadata.
     :param recursive: Option to propagate the metadata change to content.
     :param session: The database session in use.
     """
 
     for did in dids:
         did_meta_plugins.set_metadata_bulk(scope=did['scope'], name=did['name'], meta=did['meta'], recursive=recursive, session=session)
 
 
 @read_session
-def get_metadata(scope, name, plugin='DID_COLUMN', *, session: "Session"):
+def get_metadata(
+    scope: "InternalScope",
+    name: str,
+    plugin: str = 'DID_COLUMN',
+    *,
+    session: "Session"
+) -> dict[str, Any]:
     """
     Get data identifier metadata
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param session: The database session in use.
 
     :returns: List of HARDCODED metadata for did.
     """
     return did_meta_plugins.get_metadata(scope, name, plugin=plugin, session=session)
 
 
 @stream_session
-def list_parent_dids_bulk(dids, *, session: "Session"):
+def list_parent_dids_bulk(
+    dids: "Iterable[Mapping[str, Any]]",
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List parent datasets and containers of a did.
 
     :param dids:               A list of dids.
     :param session:            The database session in use.
     :returns:                  List of dids.
     :rtype:                    Generator.
@@ -2283,15 +2416,20 @@
             for did_chunk in session.execute(stmt).yield_per(5):
                 yield {'scope': did_chunk.scope, 'name': did_chunk.name, 'child_scope': did_chunk.child_scope, 'child_name': did_chunk.child_name, 'type': did_chunk.did_type}
     except NoResultFound:
         raise exception.DataIdentifierNotFound('No Data Identifiers found')
 
 
 @stream_session
-def get_metadata_bulk(dids, inherit=False, *, session: "Session"):
+def get_metadata_bulk(
+    dids: list["Mapping[Any, Any]"],
+    inherit: bool = False,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     Get metadata for a list of dids
     :param dids:               A list of dids.
     :param inherit:            A boolean. If set to true, the metadata of the parent are concatenated.
     :param session:            The database session in use.
     """
     if inherit:
@@ -2351,27 +2489,39 @@
                 for row in session.execute(stmt).scalars():
                     yield row.to_dict()
         except NoResultFound:
             raise exception.DataIdentifierNotFound('No Data Identifiers found')
 
 
 @transactional_session
-def delete_metadata(scope, name, key, *, session: "Session"):
+def delete_metadata(
+    scope: "InternalScope",
+    name: str,
+    key: str,
+    *,
+    session: "Session"
+) -> None:
     """
     Delete a key from the metadata column
 
     :param scope: the scope of did
     :param name: the name of the did
     :param key: the key to be deleted
     """
     did_meta_plugins.delete_metadata(scope, name, key, session=session)
 
 
 @transactional_session
-def set_status(scope, name, *, session: "Session", **kwargs):
+def set_status(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session",
+    **kwargs
+) -> None:
     """
     Set data identifier status
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param session: The database session in use.
     :param kwargs:  Keyword arguments of the form status_name=value.
@@ -2472,16 +2622,27 @@
                 name=name
             )
             for rule in session.execute(stmt).scalars():
                 rucio.core.rule.generate_rule_notifications(rule=rule, session=session)
 
 
 @read_session
-def list_dids(scope, filters, did_type='collection', ignore_case=False, limit=None,
-              offset=None, long=False, recursive=False, ignore_dids=None, *, session: "Session"):
+def list_dids(
+    scope: "InternalScope",
+    filters: "Mapping[Any, Any]",
+    did_type: Literal['all', 'collection', 'dataset', 'container', 'file'] = 'collection',
+    ignore_case: bool = False,
+    limit: Optional[int] = None,
+    offset: Optional[int] = None,
+    long: bool = False,
+    recursive: bool = False,
+    ignore_dids: Optional["Sequence[str]"] = None,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     Search data identifiers.
 
     :param scope: the scope name.
     :param filters: dictionary of attributes by which the results should be filtered.
     :param did_type: the type of the did: all(container, dataset, file), collection(dataset or container), dataset, container, file.
     :param ignore_case: ignore case distinctions.
@@ -2492,15 +2653,20 @@
     :param ignore_dids: List of DIDs to refrain from yielding.
     :param session: The database session in use.
     """
     return did_meta_plugins.list_dids(scope, filters, did_type, ignore_case, limit, offset, long, recursive, ignore_dids, session=session)
 
 
 @read_session
-def get_did_atime(scope, name, *, session: "Session"):
+def get_did_atime(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> datetime:
     """
     Get the accessed_at timestamp for a did. Just for testing.
     :param scope: the scope name.
     :param name: The data identifier name.
     :param session: Database session to use.
 
     :returns: A datetime timestamp with the last access time.
@@ -2511,15 +2677,20 @@
         scope=scope,
         name=name
     )
     return session.execute(stmt).one()[0]
 
 
 @read_session
-def get_did_access_cnt(scope, name, *, session: "Session"):
+def get_did_access_cnt(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> int:
     """
     Get the access_cnt for a did. Just for testing.
     :param scope: the scope name.
     :param name: The data identifier name.
     :param session: Database session to use.
 
     :returns: A datetime timestamp with the last access time.
@@ -2530,15 +2701,19 @@
         scope=scope,
         name=name
     )
     return session.execute(stmt).one()[0]
 
 
 @stream_session
-def get_dataset_by_guid(guid, *, session: "Session"):
+def get_dataset_by_guid(
+    guid: str,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Union[InternalScope, str]]]":
     """
     Get the parent datasets for a given GUID.
     :param guid: The GUID.
     :param session: Database session to use.
 
     :returns: A did.
     """
@@ -2565,15 +2740,19 @@
     except NoResultFound:
         raise exception.DataIdentifierNotFound("No file associated to GUID : %s" % guid)
     for tmp_did in session.execute(datasets_stmt).yield_per(5):
         yield {'scope': tmp_did.scope, 'name': tmp_did.name}
 
 
 @transactional_session
-def touch_dids(dids, *, session: "Session"):
+def touch_dids(
+    dids: "Iterable[Mapping[str, Any]]",
+    *,
+    session: "Session"
+) -> bool:
     """
     Update the accessed_at timestamp and the access_cnt of the given dids.
 
     :param replicas: the list of dids.
     :param session: The database session in use.
 
     :returns: True, if successful, False otherwise.
@@ -2600,15 +2779,24 @@
     except DatabaseError:
         return False
 
     return True
 
 
 @transactional_session
-def create_did_sample(input_scope, input_name, output_scope, output_name, account, nbfiles, *, session: "Session"):
+def create_did_sample(
+    input_scope: "InternalScope",
+    input_name: str,
+    output_scope: "InternalScope",
+    output_name: str,
+    account: "InternalAccount",
+    nbfiles: str,
+    *,
+    session: "Session"
+) -> None:
     """
     Create a sample from an input collection.
 
     :param input_scope: The scope of the input DID.
     :param input_name: The name of the input DID.
     :param output_scope: The scope of the output dataset.
     :param output_name: The name of the output dataset.
@@ -2686,15 +2874,15 @@
         bytes_, length, events = did.bytes or 0, 1, did.events or 0
     else:
         bytes_, length, events = did.bytes or 0, did.length or 0, did.events or 0
     return bytes_, length, events
 
 
 @transactional_session
-def resurrect(dids, *, session: "Session"):
+def resurrect(dids: "Iterable[Mapping[str, Any]]", *, session: "Session") -> None:
     """
     Resurrect data identifiers.
 
     :param dids: The list of dids to resurrect.
     :param session: The database session in use.
     """
     for did in dids:
@@ -2745,15 +2933,20 @@
         session.execute(stmt)
 
         models.DataIdentifier(**kargs).\
             save(session=session, flush=False)
 
 
 @stream_session
-def list_archive_content(scope, name, *, session: "Session"):
+def list_archive_content(
+    scope: "InternalScope",
+    name,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, Any]]":
     """
     List archive contents.
 
     :param scope: The archive scope name.
     :param name: The archive data identifier name.
     :param session: The database session in use.
     """
@@ -2771,29 +2964,40 @@
             yield {'scope': tmp_did.child_scope, 'name': tmp_did.child_name,
                    'bytes': tmp_did.bytes, 'adler32': tmp_did.adler32, 'md5': tmp_did.md5}
     except NoResultFound:
         raise exception.DataIdentifierNotFound(f"Data identifier '{scope}:{name}' not found")
 
 
 @transactional_session
-def add_did_to_followed(scope, name, account, *, session: "Session"):
+def add_did_to_followed(
+    scope: "InternalScope",
+    name: str,
+    account: "InternalAccount",
+    *,
+    session: "Session"
+) -> None:
     """
     Mark a did as followed by the given account
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param account: The account owner.
     :param session: The database session in use.
     """
     return add_dids_to_followed(dids=[{'scope': scope, 'name': name}],
                                 account=account, session=session)
 
 
 @transactional_session
-def add_dids_to_followed(dids, account, *, session: "Session"):
+def add_dids_to_followed(
+    dids: "Iterable[Mapping[str, Any]]",
+    account: "InternalAccount",
+    *,
+    session: "Session"
+) -> None:
     """
     Bulk mark datasets as followed
 
     :param dids: A list of dids.
     :param account: The account owner.
     :param session: The database session in use.
     """
@@ -2815,15 +3019,20 @@
 
         session.flush()
     except IntegrityError as error:
         raise exception.RucioException(error.args)
 
 
 @stream_session
-def get_users_following_did(scope, name, *, session: "Session"):
+def get_users_following_did(
+    scope: "InternalScope",
+    name: str,
+    *,
+    session: "Session"
+) -> "Iterator[dict[str, InternalAccount]]":
     """
     Return list of users following a did
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param session: The database session in use.
     """
@@ -2839,29 +3048,40 @@
             yield {'user': user.account}
 
     except NoResultFound:
         raise exception.DataIdentifierNotFound("Data identifier '%s:%s' not found" % (scope, name))
 
 
 @transactional_session
-def remove_did_from_followed(scope, name, account, *, session: "Session"):
+def remove_did_from_followed(
+    scope: "InternalScope",
+    name: str,
+    account: "InternalAccount",
+    *,
+    session: "Session"
+) -> None:
     """
     Mark a did as not followed
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param account: The account owner.
     :param session: The database session in use.
     """
     return remove_dids_from_followed(dids=[{'scope': scope, 'name': name}],
                                      account=account, session=session)
 
 
 @transactional_session
-def remove_dids_from_followed(dids, account, *, session: "Session"):
+def remove_dids_from_followed(
+    dids: "Iterable[Mapping[str, Any]]",
+    account: "InternalAccount",
+    *,
+    session: "Session"
+) -> None:
     """
     Bulk mark datasets as not followed
 
     :param dids: A list of dids.
     :param account: The account owner.
     :param session: The database session in use.
     """
@@ -2878,15 +3098,22 @@
             )
             session.execute(stmt)
     except NoResultFound:
         raise exception.DataIdentifierNotFound("Data identifier '%s:%s' not found" % (did['scope'], did['name']))
 
 
 @transactional_session
-def trigger_event(scope, name, event_type, payload, *, session: "Session"):
+def trigger_event(
+    scope: "InternalScope",
+    name: str,
+    event_type: str,
+    payload: str,
+    *,
+    session: "Session"
+) -> None:
     """
     Records changes occurring in the did to the FollowEvents table
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param event_type: The type of event affecting the did.
     :param payload: Any message to be stored along with the event.
@@ -2907,15 +3134,20 @@
 
         session.flush()
     except IntegrityError as error:
         raise exception.RucioException(error.args)
 
 
 @read_session
-def create_reports(total_workers, worker_number, *, session: "Session"):
+def create_reports(
+    total_workers: int,
+    worker_number: int,
+    *,
+    session: "Session"
+) -> None:
     """
     Create a summary report of the events affecting a dataset, for its followers.
 
     :param session: The database session in use.
     """
     # Query the FollowEvents table
     stmt = select(
@@ -2969,15 +3201,20 @@
                                   'body': body})
 
     except NoResultFound:
         raise exception.AccountNotFound("No email found for given account.")
 
 
 @transactional_session
-def insert_content_history(filter_, did_created_at, *, session: "Session"):
+def insert_content_history(
+    filter_: "ColumnExpressionArgument[bool]",
+    did_created_at: datetime,
+    *,
+    session: "Session"
+) -> None:
     """
     Insert into content history a list of did
 
     :param filter_: Content clause of the files to archive
     :param did_created_at: Creation date of the did
     :param session: The database session in use.
     """
@@ -3020,15 +3257,15 @@
             created_at=cont.created_at,
             did_created_at=new_did_created_at,
             deleted_at=datetime.utcnow()
         ).save(session=session, flush=False)
 
 
 @transactional_session
-def insert_deleted_dids(filter_, *, session: "Session"):
+def insert_deleted_dids(filter_: "ColumnExpressionArgument[bool]", *, session: "Session") -> None:
     """
     Insert into deleted_dids a list of did
 
     :param filter_: The database filter to retrieve dids for archival
     :param session: The database session in use.
     """
     stmt = select(
```

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/__init__.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_column_meta.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_column_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/did_meta_plugin_interface.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/filter_engine.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/filter_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import ast
 import fnmatch
 import operator
+from collections.abc import Callable, Iterable
 from datetime import date, datetime, timedelta
 from importlib import import_module
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
 
 import sqlalchemy
 from sqlalchemy import and_, cast, or_
+from sqlalchemy.orm import InstrumentedAttribute, Query
 from sqlalchemy.sql.expression import text
 
 from rucio.common import exception
 from rucio.common.utils import parse_did_filter_from_string_fe
 from rucio.db.sqla.constants import DIDType
 from rucio.db.sqla.session import read_session
 
@@ -267,21 +269,25 @@
             operators = ('+', '-', '*', '/')
             if not any(operator in value for operator in operators):    # fix for lax ast literal_eval in earlier python versions
                 value = ast.literal_eval(value)                         # will catch float, int and bool
         except (ValueError, SyntaxError):
             pass
         return value
 
-    def create_mongo_query(self, additional_filters={}):
+    def create_mongo_query(
+        self,
+        additional_filters: Optional[Iterable[tuple[str, Callable, str]]] = None
+    ) -> dict[str, Any]:
         """
         Returns a single mongo query describing the filters expression.
 
         :param additional_filters: additional filters to be applied to all clauses.
         :returns: a mongo query string describing the filters expression.
         """
+        additional_filters = additional_filters or []
         # Add additional filters, applied as AND clauses to each OR group.
         for or_group in self._filters:
             for filter in additional_filters:
                 or_group.append(list(filter))
 
         or_expressions = []
         for or_group in self._filters:
@@ -322,23 +328,28 @@
         if len(or_expressions) > 1:
             query_str = {'$or': or_expressions}                     # $or key must have array as value...
         else:
             query_str = or_expressions[0]                           # ...otherwise just use the first, and only, entry.
 
         return query_str
 
-    def create_postgres_query(self, additional_filters={}, fixed_table_columns=('scope', 'name', 'vo'),
-                              jsonb_column='data'):
+    def create_postgres_query(
+        self,
+        additional_filters: Optional[Iterable[tuple[str, Callable, str]]] = None,
+        fixed_table_columns: Iterable[str] = ('scope', 'name', 'vo'),
+        jsonb_column: str = 'data'
+    ) -> str:
         """
         Returns a single postgres query describing the filters expression.
 
         :param additional_filters: additional filters to be applied to all clauses.
         :param fixed_table_columns: the table columns
         :returns: a postgres query string describing the filters expression.
         """
+        additional_filters = additional_filters or []
         # Add additional filters, applied as AND clauses to each OR group.
         for or_group in self._filters:
             for _filter in additional_filters:
                 or_group.append(list(_filter))
 
         or_expressions = []
         for or_group in self._filters:
@@ -396,28 +407,37 @@
                     except Exception as e:
                         raise exception.FilterEngineGenericError(e)
                 and_expressions.append(expression)
             or_expressions.append(' AND '.join(and_expressions))
         return ' OR '.join(or_expressions)
 
     @read_session
-    def create_sqla_query(self, *, session: "Session", additional_model_attributes=[], additional_filters={}, json_column=None):
+    def create_sqla_query(
+        self,
+        *,
+        session: "Session",
+        additional_model_attributes: Optional[list[InstrumentedAttribute]] = None,
+        additional_filters: Optional[Iterable[tuple[str, Callable, str]]] = None,
+        json_column: Optional[InstrumentedAttribute] = None
+    ) -> Query:
         """
         Returns a database query that fully describes the filters.
 
         The logic for construction of syntax describing a filter for key is dependent on whether the key has been previously coerced to a model attribute (i.e. key
         is a table column).
 
         :param session: The database session.
         :param additional_model_attributes: Additional model attributes to retrieve.
         :param additional_filters: Additional filters to be applied to all clauses.
         :param json_column: Column to be checked if filter key has not been coerced to a model attribute. Only valid if engine instantiated with strict_coerce=False.
         :returns: A database query.
         :raises: FilterEngineGenericError
         """
+        additional_model_attributes = additional_model_attributes or []
+        additional_filters = additional_filters or []
         all_model_attributes = set(self.mandatory_model_attributes + additional_model_attributes)
 
         # Add additional filters, applied as AND clauses to each OR group.
         for or_group in self._filters:
             for _filter in additional_filters:
                 or_group.append(list(_filter))
```

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/json_meta.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/json_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/mongo_meta.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/mongo_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/did_meta_plugins/postgres_meta.py` & `rucio-34.4.0/lib/rucio/core/did_meta_plugins/postgres_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/dirac.py` & `rucio-34.4.0/lib/rucio/core/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/distance.py` & `rucio-34.4.0/lib/rucio/core/distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,21 +117,22 @@
             query = query.filter(Distance.dest_rse_id == dest_rse_id)
         query.update({Distance.distance: distance})
     except IntegrityError as error:
         raise exception.RucioException(error.args)
 
 
 @read_session
-def list_distances(filter_: dict[str, Any] = {}, *, session: "Session") -> list[dict[str, Any]]:
+def list_distances(filter_: Optional[dict[str, Any]] = None, *, session: "Session") -> list[dict[str, Any]]:
     """
     Get distances between all the RSEs.
 
     :param filter_: dictionary to filter distances.
     :param session: The database session in use.
     """
+    filter_ = filter_ or {}
     return [distance.to_dict() for distance in session.query(Distance).all()]
 
 
 @read_session
 def export_distances(vo: str = 'def', *, session: "Session") -> dict[str, Any]:
     """
     Export distances between all the RSEs using RSE ids.
```

### Comparing `rucio-34.3.0/lib/rucio/core/exporter.py` & `rucio-34.4.0/lib/rucio/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/heartbeat.py` & `rucio-34.4.0/lib/rucio/core/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/identity.py` & `rucio-34.4.0/lib/rucio/core/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/importer.py` & `rucio-34.4.0/lib/rucio/core/importer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/lifetime_exception.py` & `rucio-34.4.0/lib/rucio/core/lifetime_exception.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/lock.py` & `rucio-34.4.0/lib/rucio/core/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/message.py` & `rucio-34.4.0/lib/rucio/core/message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/meta_conventions.py` & `rucio-34.4.0/lib/rucio/core/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/monitor.py` & `rucio-34.4.0/lib/rucio/core/monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/naming_convention.py` & `rucio-34.4.0/lib/rucio/core/naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/nongrid_trace.py` & `rucio-34.4.0/lib/rucio/core/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/oidc.py` & `rucio-34.4.0/lib/rucio/core/oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,19 +290,19 @@
         if token_object:
             issuer = token_object.identity.split(", ")[1].split("=")[1]
             oidc_client = OIDC_CLIENTS[issuer]
             auth_args["client_id"] = oidc_client.client_id
             token = ''
             if not token_type:
                 token_type = kwargs.get('token_type', None)
-            if token_type == 'subject_token':
+            if token_type == 'subject_token':  # noqa: S105
                 token = token_object.token
                 # do not remove - even though None, oic expects this key to exist
                 auth_args["redirect_uri"] = None
-            if token_type == 'refresh_token':
+            if token_type == 'refresh_token':  # noqa: S105
                 token = token_object.refresh_token
                 # do not remove - even though None, oic expects this key to exist
                 auth_args["redirect_uri"] = None
             if token_type and token:
                 oidc_client.grant[auth_args['state']] = Grant()
                 oidc_client.grant[auth_args['state']].grant_expiration_time = time_util.utc_time_sans_frac() + 300
                 resp = AccessTokenResponse()
@@ -914,15 +914,15 @@
     # (happens when user presents subject token acquired from other sources then Rucio CLI mechanism),
     # add offline_access scope to the token exchange request !
     if 'offline_access' in str(subject_token_object.oidc_scope) and not subject_token_object.refresh_token:
         jwt_row_dict['authz_scope'] += ' offline_access'
     if not grant_type:
         grant_type = EXCHANGE_GRANT_TYPE
     try:
-        oidc_dict = __get_init_oidc_client(token_object=subject_token_object, token_type="subject_token")
+        oidc_dict = __get_init_oidc_client(token_object=subject_token_object, token_type="subject_token")  # noqa: S106
         oidc_client = oidc_dict['client']
         args = {"subject_token": subject_token_object.token,
                 "scope": jwt_row_dict['authz_scope'],
                 "audience": jwt_row_dict['audience'],
                 "grant_type": grant_type}
         # exchange , access token for a new one
         oidc_token_response = oidc_dict['client'].do_any(Message,
@@ -1158,15 +1158,15 @@
         if token_object.refresh_lifetime:
             extra_dict['refresh_lifetime'] = token_object.refresh_lifetime
         # if the token has been refreshed for time exceeding
         # the refresh_lifetime, the attempt will be aborted and refresh stopped
         if datetime.utcnow() - extra_dict['refresh_start'] > timedelta(hours=extra_dict['refresh_lifetime']):
             __change_refresh_state(token_object.token, refresh=False, session=session)
             return None
-        oidc_dict = __get_init_oidc_client(token_object=token_object, token_type="refresh_token")
+        oidc_dict = __get_init_oidc_client(token_object=token_object, token_type="refresh_token")  # noqa: S106
         oidc_client = oidc_dict['client']
         # getting a new refreshed set of tokens
         state = oidc_dict['state']
         oidc_tokens = oidc_client.do_access_token_refresh(state=state, skew=LEEWAY_SECS)
         if 'error' in oidc_tokens:
             raise CannotAuthorize(oidc_tokens['error'])
         METRICS.counter(name='IdP_authorization.refresh_token.refreshed').inc()
@@ -1394,15 +1394,15 @@
         oidc_client = OIDC_CLIENTS[issuer]
         issuer_keys = oidc_client.keyjar.get_issuer_keys(issuer)
         JWS().verify_compact(json_web_token, issuer_keys)
         # if there is no audience and scope information,
         # try to get it from IdP introspection endpoint
         # TO-BE-REMOVED - once all IdPs support scope and audience in token claims !!!
         if not token_dict['authz_scope'] or not token_dict['audience']:
-            clprocess = subprocess.Popen(['curl', '-s', '-L', '-u', '%s:%s'
+            clprocess = subprocess.Popen(['curl', '-s', '-L', '-u', '%s:%s'  # noqa: S607
                                           % (oidc_client.client_id, oidc_client.client_secret),
                                           '-d', 'token=%s' % (json_web_token),
                                           oidc_client.introspection_endpoint],
                                          shell=False, stdout=subprocess.PIPE)
             inspect_claims = json.loads(clprocess.communicate()[0])
             try:
                 token_dict['audience'] = inspect_claims['aud']
```

### Comparing `rucio-34.3.0/lib/rucio/core/permission/__init__.py` & `rucio-34.4.0/lib/rucio/core/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/permission/atlas.py` & `rucio-34.4.0/lib/rucio/core/permission/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/permission/belleii.py` & `rucio-34.4.0/lib/rucio/core/permission/belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/permission/cms.py` & `rucio-34.4.0/lib/rucio/core/permission/generic_multi_vo.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING
 
 import rucio.core.scope
 from rucio.common.constants import RseAttr
-from rucio.core.account import has_account_attribute
+from rucio.core.account import has_account_attribute, list_account_attributes
 from rucio.core.identity import exist_identity_account
-from rucio.core.permission.generic import perm_get_global_account_usage
+from rucio.core.lifetime_exception import list_exceptions
 from rucio.core.rse import list_rse_attributes
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.core.rule import get_rule
 from rucio.db.sqla.constants import IdentityType
 
 if TYPE_CHECKING:
     from typing import Optional
@@ -50,16 +50,14 @@
             'add_subscription': perm_add_subscription,
             'add_scope': perm_add_scope,
             'add_rse': perm_add_rse,
             'update_rse': perm_update_rse,
             'add_protocol': perm_add_protocol,
             'del_protocol': perm_del_protocol,
             'update_protocol': perm_update_protocol,
-            'add_qos_policy': perm_add_qos_policy,
-            'delete_qos_policy': perm_delete_qos_policy,
             'declare_bad_file_replicas': perm_declare_bad_file_replicas,
             'declare_suspicious_file_replicas': perm_declare_suspicious_file_replicas,
             'add_replicas': perm_add_replicas,
             'delete_replicas': perm_delete_replicas,
             'skip_availability_check': perm_skip_availability_check,
             'update_replicas_states': perm_update_replicas_states,
             'add_rse_attribute': perm_add_rse_attribute,
@@ -83,15 +81,18 @@
             'attach_dids_to_dids': perm_attach_dids_to_dids,
             'create_did_sample': perm_create_did_sample,
             'set_metadata': perm_set_metadata,
             'set_status': perm_set_status,
             'queue_requests': perm_queue_requests,
             'set_rse_usage': perm_set_rse_usage,
             'set_rse_limits': perm_set_rse_limits,
+            'list_requests': perm_list_requests,
+            'list_requests_history': perm_list_requests_history,
             'get_request_by_did': perm_get_request_by_did,
+            'get_request_history_by_did': perm_get_request_history_by_did,
             'cancel_request': perm_cancel_request,
             'get_next': perm_get_next,
             'set_local_account_limit': perm_set_local_account_limit,
             'set_global_account_limit': perm_set_global_account_limit,
             'delete_local_account_limit': perm_delete_local_account_limit,
             'delete_global_account_limit': perm_delete_global_account_limit,
             'config_sections': perm_config,
@@ -172,35 +173,14 @@
     Checks if an account can add a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-
-    rses = parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)
-
-    # Keep while sync is running so it can make rules on all RSEs
-    if _is_root(issuer) and repr(kwargs['account']).startswith('sync_'):
-        return True
-
-    if isinstance(repr(issuer), str) and repr(issuer).startswith('sync_'):  # noqa
-        return True
-
-    # Anyone can use _Temp RSEs if a lifetime is set and under a month
-    all_temp = True
-    for rse in rses:
-        rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        rse_type = rse_attr.get(RseAttr.CMS_TYPE, None)
-        if rse_type not in ['temp']:
-            all_temp = False
-
-    if all_temp and kwargs['lifetime'] is not None and kwargs['lifetime'] < 31 * 24 * 60 * 60:
-        return True
-
     if kwargs['account'] == issuer and not kwargs['locked']:
         return True
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
     return False
 
 
@@ -412,26 +392,18 @@
     """
     # Check the accounts of the issued rules
     if not _is_root(issuer) and not has_account_attribute(account=issuer, key='admin', session=session):
         for rule in kwargs.get('rules', []):
             if rule['account'] != issuer:
                 return False
 
-    if kwargs['scope'].external != 'cms':
-        if kwargs['type'] == 'DATASET':
-            if '/USER#' not in kwargs['name']:
-                return False
-        elif kwargs['type'] == 'CONTAINER':
-            if not kwargs['name'].endswith('/USER'):
-                return False
-
-    return (_is_root(issuer)
-            or has_account_attribute(account=issuer, key='admin', session=session)  # NOQA: W503
-            or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)  # NOQA: W503
-            or kwargs['scope'].external == 'mock')  # NOQA: W503
+    return _is_root(issuer)\
+        or has_account_attribute(account=issuer, key='admin', session=session)\
+        or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)\
+        or kwargs['scope'].external == 'mock'
 
 
 def perm_add_dids(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can bulk add data identifiers.
 
     :param issuer: Account identifier which issues the command.
@@ -454,18 +426,18 @@
     Checks if an account can append an data identifier to the other data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return (_is_root(issuer)
-            or has_account_attribute(account=issuer, key='admin', session=session)  # NOQA: W503
-            or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)  # NOQA: W503
-            or kwargs['scope'].external == 'mock')  # NOQA: W503
+    return _is_root(issuer)\
+        or has_account_attribute(account=issuer, key='admin', session=session)\
+        or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)\
+        or kwargs['scope'].external == 'mock'
 
 
 def perm_attach_dids_to_dids(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can append an data identifier to the other data identifier.
 
     :param issuer: Account identifier which issues the command.
@@ -490,34 +462,31 @@
     Checks if an account can create a sample of a data identifier collection.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return issuer == ('root'
-                      or has_account_attribute(account=issuer, key='admin', session=session)  # NOQA: W503
-                      or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)  # NOQA: W503
-                      or kwargs['scope'].external == 'mock')  # NOQA: W503
+    return _is_root(issuer)\
+        or has_account_attribute(account=issuer, key='admin', session=session)\
+        or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)\
+        or kwargs['scope'].external == 'mock'
 
 
 def perm_del_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an issuer can delete a replication rule.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    if get_rule(kwargs['rule_id'])['account'] == issuer:
-        return True
-
     return False
 
 
 def perm_update_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an issuer can update a replication rule.
 
@@ -538,25 +507,14 @@
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-
-    rule = get_rule(rule_id=kwargs['rule_id'])
-    rses = parse_expression(rule['rse_expression'], filter_={'vo': issuer.vo}, session=session)
-
-    # Those in rule_approvers can approve the rule
-    for rse in rses:
-        rse_attr = list_rse_attributes(rse_id=rse['id'], session=session)
-        rule_approvers = rse_attr.get(RseAttr.RULE_APPROVERS, None)
-        if rule_approvers and issuer.external in rule_approvers.split(','):
-            return True
-
     return False
 
 
 def perm_reduce_rule(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an issuer can reduce a replication rule.
 
@@ -616,16 +574,15 @@
     Checks if an account can set a metadata on a data identifier.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return (_is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
-            or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session))  # NOQA: W503
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)
 
 
 def perm_set_status(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can set status on an data identifier.
 
     :param issuer: Account identifier which issues the command.
@@ -633,16 +590,15 @@
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if kwargs.get('open', False):
         if not _is_root(issuer) and not has_account_attribute(account=issuer, key='admin', session=session):
             return False
 
-    return (_is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
-            or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session))  # NOQA: W503
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or rucio.core.scope.is_scope_owner(scope=kwargs['scope'], account=issuer, session=session)
 
 
 def perm_add_protocol(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can add a protocol to an RSE.
 
     :param issuer: Account identifier which issues the command.
@@ -673,142 +629,151 @@
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_qos_policy(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_declare_bad_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can add QoS policies to an RSE.
+    Checks if an account can declare bad file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+    return _is_root(issuer)
 
 
-def perm_delete_qos_policy(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_declare_suspicious_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can delete QoS policies from an RSE.
+    Checks if an account can declare suspicious file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+    return True
 
 
-def perm_declare_bad_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_add_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can declare bad file replicas.
+    Checks if an account can add replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+    return str(kwargs.get('rse', '')).endswith('SCRATCHDISK')\
+        or str(kwargs.get('rse', '')).endswith('USERDISK')\
+        or str(kwargs.get('rse', '')).endswith('MOCK')\
+        or str(kwargs.get('rse', '')).endswith('LOCALGROUPDISK')\
+        or _is_root(issuer)\
+        or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_declare_suspicious_file_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_skip_availability_check(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can declare suspicious file replicas.
+    Checks if an account can skip the availabity check to add/delete file replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return True
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_add_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_delete_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can add replicas.
+    Checks if an account can delete replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-
-    is_root = _is_root(issuer)
-    is_temp = str(kwargs.get('rse', '')).endswith('_Temp')
-    is_admin = has_account_attribute(account=issuer, key='admin', session=session)
-
-    return is_root or is_temp or is_admin
+    return False
 
 
-def perm_skip_availability_check(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_update_replicas_states(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can skip the availabity check to add/delete file replicas.
+    Checks if an account can delete replicas.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_delete_replicas(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_queue_requests(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can delete replicas.
+    Checks if an account can submit transfer or deletion requests on destination RSEs for data identifiers.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-
-    # FIXME: Remove after the transition is over?
-
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+    return _is_root(issuer)
 
 
-def perm_update_replicas_states(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_list_requests(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can delete replicas.
+    Checks if an account can list requests.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
-def perm_queue_requests(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_list_requests_history(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can submit transfer or deletion requests on destination RSEs for data identifiers.
+    Checks if an account can list historical requests.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return _is_root(issuer)
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
 def perm_get_request_by_did(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can get a request by DID.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return True
 
 
+def perm_get_request_history_by_did(issuer, kwargs, *, session: "Optional[Session]" = None):
+    """
+    Checks if an account can get a historical request by DID.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+
+
 def perm_cancel_request(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can cancel a request.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
@@ -853,110 +818,96 @@
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
 def perm_set_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can set an account limit.
 
-    :param issuer: Account identifier which issues the command.
+    :param account: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    # # Check if user is a country admin
-    # admin_in_country = []
-    # from rucio.core.account import has_account_attribute, list_account_attributes
-    # for kv in list_account_attributes(account=issuer, session=session):
-    #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
-    #         admin_in_country.append(kv['key'].partition('-')[2])
-    # if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
-    #     return True
-
-    # Those listed as quota approvers can add to quotas
-    rse_attr = list_rse_attributes(rse_id=kwargs['rse_id'], session=session)
-    quota_approvers = rse_attr.get(RseAttr.QUOTA_APPROVERS, None)
-    if quota_approvers and issuer.external in quota_approvers.split(','):
+    # Check if user is a country admin
+    admin_in_country = []
+    for kv in list_account_attributes(account=issuer, session=session):
+        if kv['key'].startswith('country-') and kv['value'] == 'admin':
+            admin_in_country.append(kv['key'].partition('-')[2])
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
         return True
-
     return False
 
 
 def perm_set_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can set a global account limit.
 
     :param account: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    # # Check if user is a country admin
-    # admin_in_country = set()
-    # for kv in list_account_attributes(account=issuer, session=session):
-    #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
-    #         admin_in_country.add(kv['key'].partition('-')[2])
-    # resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
-    #                           for rse in parse_expression(kwargs['rse_expression'], filter={'vo': issuer.vo}, session=session)}
-    # if resolved_rse_countries.issubset(admin_in_country):
-    #     return True
+    # Check if user is a country admin
+    admin_in_country = set()
+    for kv in list_account_attributes(account=issuer, session=session):
+        if kv['key'].startswith('country-') and kv['value'] == 'admin':
+            admin_in_country.add(kv['key'].partition('-')[2])
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
+                              for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
+    if resolved_rse_countries.issubset(admin_in_country):
+        return True
     return False
 
 
-def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can delete a global account limit.
+    Checks if an account can delete an account limit.
 
-    :param issuer: Account identifier which issues the command.
+    :param account: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    # # Check if user is a country admin
-    # admin_in_country = set()
-    # for kv in list_account_attributes(account=issuer, session=session):
-    #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
-    #         admin_in_country.add(kv['key'].partition('-')[2])
-    # if admin_in_country:
-    #     resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
-    #                               for rse in parse_expression(kwargs['rse_expression'], filter={'vo': issuer.vo}, session=session)}
-    #     if resolved_rse_countries.issubset(admin_in_country):
-    #         return True
+    # Check if user is a country admin
+    admin_in_country = []
+    for kv in list_account_attributes(account=issuer, session=session):
+        if kv['key'].startswith('country-') and kv['value'] == 'admin':
+            admin_in_country.append(kv['key'].partition('-')[2])
+    if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
+        return True
     return False
 
 
-def perm_delete_local_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
+def perm_delete_global_account_limit(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
-    Checks if an account can delete an account limit.
+    Checks if an account can delete a global account limit.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session):
         return True
-    # # Check if user is a country admin
-    # admin_in_country = []
-    # for kv in list_account_attributes(account=issuer, session=session):
-    #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
-    #         admin_in_country.append(kv['key'].partition('-')[2])
-    # if admin_in_country and list_rse_attributes(rse_id=kwargs['rse_id'], session=session).get(RseAttr.COUNTRY) in admin_in_country:
-    #     return True
-
-    rse_attr = list_rse_attributes(rse_id=kwargs['rse_id'], session=session)
-    quota_approvers = rse_attr.get(RseAttr.QUOTA_APPROVERS, None)
-    if quota_approvers and issuer.external in quota_approvers.split(','):
-        return True
-
+    # Check if user is a country admin
+    admin_in_country = set()
+    for kv in list_account_attributes(account=issuer, session=session):
+        if kv['key'].startswith('country-') and kv['value'] == 'admin':
+            admin_in_country.add(kv['key'].partition('-')[2])
+    if admin_in_country:
+        resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
+                                  for rse in parse_expression(kwargs['rse_expression'], filter_={'vo': issuer.vo}, session=session)}
+        if resolved_rse_countries.issubset(admin_in_country):
+            return True
     return False
 
 
 def perm_config(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can read/write the configuration.
 
@@ -975,18 +926,43 @@
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or kwargs.get('account') == issuer:
         return True
-    # # Check if user is a country admin
-    # for kv in list_account_attributes(account=issuer, session=session):
-    #     if kv['key'].startswith('country-') and kv['value'] == 'admin':
-    #         return True
+    # Check if user is a country admin
+    for kv in list_account_attributes(account=issuer, session=session):
+        if kv['key'].startswith('country-') and kv['value'] == 'admin':
+            return True
+    return False
+
+
+def perm_get_global_account_usage(issuer, kwargs, *, session: "Optional[Session]" = None):
+    """
+    Checks if an account can get the account usage of an account.
+
+    :param issuer: Account identifier which issues the command.
+    :param kwargs: List of arguments for the action.
+    :param session: The DB session to use
+    :returns: True if account is allowed, otherwise False
+    """
+    if _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session) or kwargs.get('account') == issuer:
+        return True
+
+    # Check if user is a country admin for all involved countries
+    admin_in_country = set()
+    for kv in list_account_attributes(account=issuer, session=session):
+        if kv['key'].startswith('country-') and kv['value'] == 'admin':
+            admin_in_country.add(kv['key'].partition('-')[2])
+    resolved_rse_countries = {list_rse_attributes(rse_id=rse['rse_id'], session=session).get(RseAttr.COUNTRY)
+                              for rse in parse_expression(kwargs['rse_exp'], filter_={'vo': issuer.vo}, session=session)}
+
+    if resolved_rse_countries.issubset(admin_in_country):
+        return True
     return False
 
 
 def perm_add_account_attribute(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can add attributes to accounts.
 
@@ -1035,27 +1011,29 @@
 
 
 def perm_update_lifetime_exceptions(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can approve/reject Lifetime Model exceptions.
 
     :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
+    if kwargs['vo'] is not None:
+        exceptions = next(list_exceptions(exception_id=kwargs['exception_id'], states=False, session=session))
+        if exceptions['scope'].vo != kwargs['vo']:
+            return False
     return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
 
 
 def perm_get_auth_token_ssh(issuer: "InternalAccount", kwargs: dict, *, session: "Optional[Session]" = None) -> bool:
     """
     Checks if an account can request an ssh token.
 
     :param issuer: Account identifier which issues the command.
-    :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed to call the API call, otherwise False
     """
     return True
 
 
 def perm_get_signed_url(issuer, kwargs, *, session: "Optional[Session]" = None):
@@ -1074,30 +1052,30 @@
     Checks if an account can declare bad PFNs.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return _is_root(issuer) or has_account_attribute(account=issuer, key='admin', session=session)
+    return _is_root(issuer)
 
 
 def perm_remove_did_from_followed(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can remove did from followed table.
 
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
-    return (_is_root(issuer)
-            or has_account_attribute(account=issuer, key='admin', session=session)  # NOQA: W503
-            or kwargs['account'] == issuer  # NOQA: W503
-            or kwargs['scope'].external == 'mock')  # NOQA: W503
+    return _is_root(issuer)\
+        or has_account_attribute(account=issuer, key='admin', session=session)\
+        or kwargs['account'] == issuer\
+        or kwargs['scope'].external == 'mock'
 
 
 def perm_remove_dids_from_followed(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can bulk remove dids from followed table.
 
     :param issuer: Account identifier which issues the command.
@@ -1111,58 +1089,62 @@
         return False
     return True
 
 
 def perm_add_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can add a VO.
+
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return (issuer.internal == 'super_root')
 
 
 def perm_list_vos(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can list a VO.
+
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
-    :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return (issuer.internal == 'super_root')
 
 
 def perm_recover_vo_root_identity(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can recover identities for VOs.
+
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return (issuer.internal == 'super_root')
 
 
 def perm_update_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if an account can update a VO.
+
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return (issuer.internal == 'super_root')
 
 
 def perm_access_rule_vo(issuer, kwargs, *, session: "Optional[Session]" = None):
     """
     Checks if we're at the same VO as the rule_id's
+
     :param issuer: Account identifier which issues the command.
     :param kwargs: List of arguments for the action.
     :param session: The DB session to use
     :returns: True if account is allowed, otherwise False
     """
     return get_rule(kwargs['rule_id'])['scope'].vo == issuer.vo
```

### Comparing `rucio-34.3.0/lib/rucio/core/permission/escape.py` & `rucio-34.4.0/lib/rucio/core/permission/escape.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/permission/generic.py` & `rucio-34.4.0/lib/rucio/core/permission/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/quarantined_replica.py` & `rucio-34.4.0/lib/rucio/core/quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/replica.py` & `rucio-34.4.0/lib/rucio/core/replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,19 +54,20 @@
 from rucio.db.sqla import filter_thread_work, models
 from rucio.db.sqla.constants import OBSOLETE, BadFilesStatus, BadPFNStatus, DIDAvailability, DIDType, ReplicaState, RuleState
 from rucio.db.sqla.session import BASE, DEFAULT_SCHEMA_NAME, read_session, stream_session, transactional_session
 from rucio.db.sqla.util import temp_table_mngr
 from rucio.rse import rsemanager as rsemgr
 
 if TYPE_CHECKING:
-    from collections.abc import Iterator, Sequence
+    from collections.abc import Iterable, Iterator, Sequence
     from typing import Any, Optional
 
     from sqlalchemy.orm import Session
 
+    from rucio.common.types import LoggerFunction
     from rucio.rse.protocols.protocol import RSEProtocol
 
 REGION = make_region_memcached(expiration_time=60)
 METRICS = MetricManager(module=__name__)
 
 
 ScopeName = namedtuple('ScopeName', ['scope', 'name'])
@@ -1422,15 +1423,15 @@
 def __bulk_add_file_dids(files, account, dataset_meta=None, *, session: "Session"):
     """
     Bulk add new dids.
 
     :param dids: the list of files.
     :param account: The account owner.
     :param session: The database session in use.
-    :returns: True is successful.
+    :returns: list of replicas.
     """
     condition = []
     for f in files:
         condition.append(and_(models.DataIdentifier.scope == f['scope'], models.DataIdentifier.name == f['name'], models.DataIdentifier.did_type == DIDType.FILE))
 
     q = session.query(models.DataIdentifier.scope,
                       models.DataIdentifier.name,
@@ -1534,15 +1535,15 @@
 
     :param rse_id:  The RSE id.
     :param files:   The list of files.
     :param account: The account owner.
     :param ignore_availability: Ignore the RSE blocklisting.
     :param session: The database session in use.
 
-    :returns: True is successful.
+    :returns: list of replicas.
     """
 
     def _expected_pfns(lfns, rse_settings, scheme, operation='write', domain='wan', protocol_attr=None):
         p = rsemgr.create_protocol(rse_settings=rse_settings, operation='write', scheme=scheme, domain=domain, protocol_attr=protocol_attr)
         expected_pfns = p.lfns2pfns(lfns)
         return clean_surls(expected_pfns.values())
 
@@ -1597,15 +1598,30 @@
 
     nbfiles, bytes_ = __bulk_add_replicas(rse_id=rse_id, files=files, account=account, session=session)
     increase(rse_id=rse_id, files=nbfiles, bytes_=bytes_, session=session)
     return replicas
 
 
 @transactional_session
-def add_replica(rse_id, scope, name, bytes_, account, adler32=None, md5=None, dsn=None, pfn=None, meta=None, rules=[], tombstone=None, *, session: "Session"):
+def add_replica(
+    rse_id: str,
+    scope: InternalScope,
+    name: str,
+    bytes_: int,
+    account: models.InternalAccount,
+    adler32: "Optional[str]" = None,
+    md5: "Optional[str]" = None,
+    dsn: "Optional[str]" = None,
+    pfn: "Optional[str]" = None,
+    meta: "Optional[dict[str, Any]]" = None,
+    rules: "Optional[list[dict[str, Any]]]" = None,
+    tombstone: "Optional[datetime]" = None,
+    *,
+    session: "Session"
+) -> "list[dict[str, Any]]":
     """
     Add File replica.
 
     :param rse_id: the rse id.
     :param scope: the scope name.
     :param name: The data identifier name.
     :param bytes_: the size of the file.
@@ -1614,18 +1630,18 @@
     :param adler32: The adler32 checksum.
     :param pfn: Physical file name (for nondeterministic rse).
     :param meta: Meta-data associated with the file. Represented as key/value pairs in a dictionary.
     :param rules: Replication rules associated with the file. A list of dictionaries, e.g., [{'copies': 2, 'rse_expression': 'TIERS1'}, ].
     :param tombstone: If True, create replica with a tombstone.
     :param session: The database session in use.
 
-    :returns: True is successful.
+    :returns: list of replicas.
     """
-    if meta is None:
-        meta = {}
+    meta = meta or {}
+    rules = rules or []
 
     file = {'scope': scope, 'name': name, 'bytes': bytes_, 'adler32': adler32, 'md5': md5, 'meta': meta, 'rules': rules, 'tombstone': tombstone}
     if pfn:
         file['pfn'] = pfn
     return add_replicas(rse_id=rse_id, files=[file, ], account=account, session=session)
 
 
@@ -3423,15 +3439,27 @@
         if state not in states:
             states[state] = []
         states[state].append(rse_id)
     return states
 
 
 @read_session
-def get_suspicious_files(rse_expression, available_elsewhere, filter_=None, logger=logging.log, younger_than=5, nattempts=0, nattempts_exact=False, *, session: "Session", exclude_states=['B', 'R', 'D'], is_suspicious=False):
+def get_suspicious_files(
+    rse_expression: str,
+    available_elsewhere: int,
+    filter_: "Optional[dict[str, Any]]" = None,
+    logger: "LoggerFunction" = logging.log,
+    younger_than: "Optional[datetime]" = None,
+    nattempts: int = 0,
+    nattempts_exact: bool = False,
+    *,
+    session: "Session",
+    exclude_states: "Optional[Iterable[str]]" = None,
+    is_suspicious: bool = False
+) -> "list[dict[str, Any]]":
     """
     Gets a list of replicas from bad_replicas table which are: declared more than <nattempts> times since <younger_than> date,
     present on the RSE specified by the <rse_expression> and do not have a state in <exclude_states> list.
     Selected replicas can also be required to be <available_elsewhere> on another RSE than the one declared in bad_replicas table and/or
     be declared as <is_suspicious> in the bad_replicas table.
     Keyword Arguments:
     :param younger_than: Datetime object to select the replicas which were declared since younger_than date. Default value = 10 days ago.
@@ -3449,14 +3477,15 @@
     :param is_suspicious: If True, only replicas declared as SUSPICIOUS in bad replicas table will be taken into account. Default value = False.
     :param session: The database session in use. Default value = None.
 
     :returns: a list of replicas:
     [{'scope': scope, 'name': name, 'rse': rse, 'rse_id': rse_id, cnt': cnt, 'created_at': created_at}, ...]
     """
 
+    exclude_states = exclude_states or ['B', 'R', 'D']
     if available_elsewhere not in [SuspiciousAvailability["ALL"].value, SuspiciousAvailability["EXIST_COPIES"].value, SuspiciousAvailability["LAST_COPY"].value]:
         logger(logging.WARNING, """ERROR, available_elsewhere must be set to one of the following:
         SuspiciousAvailability["ALL"].value: (default) all suspicious replicas are returned
         SuspiciousAvailability["EXIST_COPIES"].value: only replicas that additionally have copies declared as AVAILABLE on at least one other RSE are returned
         SuspiciousAvailability["LAST_COPY"].value: only replicas that do not have another copy declared as AVAILABLE on another RSE are returned""")
         raise exception.RucioException("""ERROR, available_elsewhere must be set to one of the following:
         SuspiciousAvailability["ALL"].value: (default) all suspicious replicas are returned
```

### Comparing `rucio-34.3.0/lib/rucio/core/replica_sorter.py` & `rucio-34.4.0/lib/rucio/core/replica_sorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Extract one file from the archive and put it at the destination
 
     archive_fileobj is supposed to be at position 0
     """
     with TemporaryDirectory(prefix=file_name) as tmp_dir:
         tmp_dir = Path(tmp_dir)
         with tarfile.open(fileobj=archive_file_obj, mode='r:gz') as tfile:
-            tfile.extractall(path=tmp_dir)
+            tfile.extractall(path=tmp_dir)  # noqa: S202
             for entry in tfile:
                 if entry.name.find(file_name) > -1:
                     print('Will move %s to %s' % (tmp_dir / entry.name, destination))
                     shutil.move(tmp_dir / entry.name, destination)
 
 
 def __download_geoip_db(destination):
```

### Comparing `rucio-34.3.0/lib/rucio/core/request.py` & `rucio-34.4.0/lib/rucio/core/request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/rse.py` & `rucio-34.4.0/lib/rucio/core/rse.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,24 +696,25 @@
         cache_prefix='rse-vo',
         include_deleted=include_deleted,
         session=session
     )
 
 
 @read_session
-def list_rses(filters={}, *, session: "Session"):
+def list_rses(filters: Optional[dict[str, Any]] = None, *, session: "Session") -> list[dict[str, Any]]:
     """
     Returns a list of all RSEs.
 
     :param filters: dictionary of attributes by which the results should be filtered.
     :param session: The database session in use.
 
     :returns: a list of dictionaries.
     """
 
+    filters = filters or {}
     rse_list = []
     filters = filters.copy()  # Make a copy, so we can pop() without affecting the object `filters` outside this function
 
     stmt = select(
         models.RSE
     ).where(
         models.RSE.deleted == false()
```

### Comparing `rucio-34.3.0/lib/rucio/core/rse_counter.py` & `rucio-34.4.0/lib/rucio/core/rse_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/rse_expression_parser.py` & `rucio-34.4.0/lib/rucio/core/rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/rse_selector.py` & `rucio-34.4.0/lib/rucio/core/rse_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from collections.abc import Iterable, Sequence
 from random import shuffle, uniform
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from rucio.common.exception import InsufficientAccountLimit, InsufficientTargetRSEs, InvalidRuleWeight, RSEOverQuota
+from rucio.common.types import InternalAccount
 from rucio.core.account import get_all_rse_usages_per_account, get_usage, has_account_attribute
 from rucio.core.account_limit import get_global_account_limits, get_local_account_limit
 from rucio.core.rse import get_rse_limits, has_rse_attribute, list_rse_attributes
 from rucio.core.rse_counter import get_counter as get_rse_counter
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.db.sqla.session import read_session
 
@@ -129,28 +131,37 @@
         self.rses = rses_with_enough_quota
         if len(self.rses) < self.copies:
             raise InsufficientAccountLimit('There is insufficient quota on any of the target RSE\'s to fulfill the operation.')
 
         # don't consider removing rses based on the total space here - because files already on the RSE are taken into account
         # it is possible to have no space but still be able to fulfil the rule
 
-    def select_rse(self, size, preferred_rse_ids, copies=0, blocklist=[], prioritize_order_over_weight=False, existing_rse_size=None):
+    def select_rse(
+        self,
+        size: int,
+        preferred_rse_ids: Iterable[str],
+        copies: int = 0,
+        blocklist: Optional[Sequence[str]] = None,
+        prioritize_order_over_weight: bool = False,
+        existing_rse_size: Optional[dict[str, int]] = None
+    ) -> list[tuple[str, bool, bool]]:
         """
         Select n RSEs to replicate data to.
 
         :param size:                         Size of the block being replicated.
         :param preferred_rse_ids:            Ordered list of preferred rses. (If possible replicate to them)
         :param copies:                       Select this amount of copies, if 0 use the pre-defined rule value.
         :param blocklist:                    List of blocked rses. (Do not put replicas on these sites)
         :param prioritze_order_over_weight:  Prioritize the order of the preferred_rse_ids list over the picking done by weight.
         :existing_rse_size:                  Dictionary of size of files already present at each rse
         :returns:                            List of (RSE_id, staging_area, availability_write) tuples.
         :raises:                             InsufficientAccountLimit, InsufficientTargetRSEs
         """
 
+        blocklist = blocklist or []
         result = []
         rses = self.rses
         count = self.copies if copies == 0 else copies
 
         # Remove blocklisted rses
         if blocklist:
             rses = [rse for rse in self.rses if rse['rse_id'] not in blocklist]
@@ -241,20 +252,35 @@
         for rse in rses:
             weight += rse['weight']
             if pick <= weight:
                 return (rse['rse_id'], rse['staging_area'], rse['availability_write'])
 
 
 @read_session
-def resolve_rse_expression(rse_expression, account, weight=None, copies=1, ignore_account_limit=False, size=0, preferred_rses=[], blocklist=[], prioritize_order_over_weight=False, existing_rse_size=None, *, session: "Session"):
+def resolve_rse_expression(
+    rse_expression: str,
+    account: InternalAccount,
+    weight: Optional[int] = None,
+    copies: int = 1,
+    ignore_account_limit: bool = False,
+    size: int = 0,
+    preferred_rses: Optional[Iterable[str]] = None,
+    blocklist: Optional[Sequence[str]] = None,
+    prioritize_order_over_weight: bool = False,
+    existing_rse_size: Optional[dict[str, int]] = None,
+    *,
+    session: "Session"
+) -> tuple[list[str], list[str]]:
     """
     Resolve a potentially complex RSE expression into `copies` single-RSE expressions. Uses `parse_expression()`
     to decompose the expression, then `RSESelector.select_rse()` to pick the target RSEs.
     """
 
+    preferred_rses = preferred_rses or []
+    blocklist = blocklist or []
     rses = parse_expression(rse_expression, filter_={'vo': account.vo}, session=session)
 
     rse_to_id = dict((rse_dict['rse'], rse_dict['id']) for rse_dict in rses)
     id_to_rse = dict((rse_dict['id'], rse_dict['rse']) for rse_dict in rses)
 
     selector = RSESelector(account=account,
                            rses=rses,
```

### Comparing `rucio-34.3.0/lib/rucio/core/rule.py` & `rucio-34.4.0/lib/rucio/core/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -2106,27 +2106,28 @@
 
 
 @read_session
 def get_updated_dids(
     total_workers: int,
     worker_number: int,
     limit: int = 100,
-    blocked_dids: Sequence[tuple[str, str]] = [],
+    blocked_dids: Optional[Sequence[tuple[str, str]]] = None,
     *,
     session: "Session"
 ) -> list[tuple[str, InternalScope, str, DIDReEvaluation]]:
     """
     Get updated dids.
 
     :param total_workers:      Number of total workers.
     :param worker_number:      id of the executing worker.
     :param limit:              Maximum number of dids to return.
     :param blocked_dids:       Blocked dids to filter.
     :param session:            Database session in use.
     """
+    blocked_dids = blocked_dids or []
     stmt = select(
         models.UpdatedDID.id,
         models.UpdatedDID.scope,
         models.UpdatedDID.name,
         models.UpdatedDID.rule_evaluation_action
     )
     stmt = filter_thread_work(session=session, query=stmt, total_threads=total_workers, thread_id=worker_number, hash_variable='name')
@@ -2191,28 +2192,29 @@
 
 
 @read_session
 def get_expired_rules(
     total_workers: int,
     worker_number: int,
     limit: int = 100,
-    blocked_rules: Sequence[str] = [],
+    blocked_rules: Optional[Sequence[str]] = None,
     *,
     session: "Session"
 ) -> list[tuple[str, str]]:
     """
     Get expired rules.
 
     :param total_workers:      Number of total workers.
     :param worker_number:      id of the executing worker.
     :param limit:              Maximum number of rules to return.
     :param blocked_rules:      List of blocked rules.
     :param session:            Database session in use.
     """
 
+    blocked_rules = blocked_rules or []
     stmt = select(
         models.ReplicationRule.id,
         models.ReplicationRule.rse_expression
     ).with_hint(
         models.ReplicationRule, 'INDEX(RULES RULES_EXPIRES_AT_IDX)', 'oracle'
     ).where(
         and_(models.ReplicationRule.expires_at < datetime.utcnow(),
@@ -2240,28 +2242,29 @@
 
 
 @read_session
 def get_injected_rules(
     total_workers: int,
     worker_number: int,
     limit: int = 100,
-    blocked_rules: Sequence[str] = [],
+    blocked_rules: Optional[Sequence[str]] = None,
     *,
     session: "Session"
 ) -> list[str]:
     """
     Get rules to be injected.
 
     :param total_workers:      Number of total workers.
     :param worker_number:      id of the executing worker.
     :param limit:              Maximum number of rules to return.
     :param blocked_rules:      Blocked rules not to include.
     :param session:            Database session in use.
     """
 
+    blocked_rules = blocked_rules or []
     stmt = select(
         models.ReplicationRule.id
     ).with_hint(
         models.ReplicationRule, 'INDEX(RULES RULES_STATE_IDX)', 'oracle'
     ).where(
         and_(models.ReplicationRule.state == RuleState.INJECT,
              models.ReplicationRule.created_at <= datetime.utcnow())
@@ -2288,28 +2291,29 @@
 
 @read_session
 def get_stuck_rules(
     total_workers: int,
     worker_number: int,
     delta: int = 600,
     limit: int = 10,
-    blocked_rules: Sequence[str] = [],
+    blocked_rules: Optional[Sequence[str]] = None,
     *,
     session: "Session"
 ) -> list[str]:
     """
     Get stuck rules.
 
     :param total_workers:      Number of total workers.
     :param worker_number:      id of the executing worker.
     :param delta:              Delta in seconds to select rules in.
     :param limit:              Maximum number of rules to select.
     :param blocked_rules:      Blocked rules to filter out.
     :param session:            Database session in use.
     """
+    blocked_rules = blocked_rules or []
     stmt = select(
         models.ReplicationRule.id
     ).with_hint(
         models.ReplicationRule, 'INDEX(RULES RULES_STATE_IDX)', 'oracle'
     ).where(
         and_(models.ReplicationRule.state == RuleState.STUCK,
              models.ReplicationRule.updated_at < datetime.utcnow() - timedelta(seconds=delta),
@@ -3902,15 +3906,15 @@
     return datasetfiles, locks, replicas, source_replicas
 
 
 @transactional_session
 def __resolve_dids_to_locks_and_replicas(
     dids: Sequence[models.DataIdentifierAssociation],
     nowait: bool = False,
-    restrict_rses: Sequence[str] = [],
+    restrict_rses: Optional[Sequence[str]] = None,
     source_rses: Optional[Sequence[str]] = None,
     *,
     session: "Session"
 ) -> tuple[list[dict[str, Any]],
            dict[tuple[str, str], models.ReplicaLock],
            dict[tuple[str, str], models.RSEFileAssociation],
            dict[tuple[str, str], str]]:
@@ -3926,14 +3930,15 @@
     """
 
     datasetfiles = []     # List of Datasets and their files in the Tree [{'scope':, 'name':, 'files': []}]
     # Files are in the format [{'scope':, 'name':, 'bytes':, 'md5':, 'adler32':}]
     locks = {}            # {(scope,name): [SQLAlchemy]}
     replicas = {}         # {(scope, name): [SQLAlchemy]}
     source_replicas = {}  # {(scope, name): [rse_id]
+    restrict_rses = restrict_rses or []
 
     if dids[0].child_type == DIDType.FILE:
         # All the dids will be files!
         # Prepare the datasetfiles
         files = []
         for did in dids:
             files.append({'scope': did.child_scope,
@@ -4075,16 +4080,16 @@
 def __create_locks_replicas_transfers(
     datasetfiles: Sequence[dict[str, Any]],
     locks: dict[tuple[InternalScope, str], Sequence[models.ReplicaLock]],
     replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
     source_replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
     rseselector: RSESelector,
     rule: models.ReplicationRule,
-    preferred_rse_ids: Sequence[str] = [],
-    source_rses: Sequence[str] = [],
+    preferred_rse_ids: Optional[Sequence[str]] = None,
+    source_rses: Optional[Sequence[str]] = None,
     *,
     session: "Session",
     logger: LoggerFunction = logging.log
 ) -> None:
     """
     Apply a created replication rule to a set of files
 
@@ -4098,14 +4103,16 @@
     :param source_rses:        RSE ids of eligible source replicas.
     :param session:            Session of the db.
     :param logger:             Optional decorated logger that can be passed from the calling daemons or servers.
     :raises:                   InsufficientAccountLimit, IntegrityError, InsufficientTargetRSEs, RSEOverQuota
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
+    preferred_rse_ids = preferred_rse_ids or []
+    source_rses = source_rses or []
     logger(logging.DEBUG, "Creating locks and replicas for rule %s [%d/%d/%d]", str(rule.id), rule.locks_ok_cnt, rule.locks_replicating_cnt, rule.locks_stuck_cnt)
 
     replicas_to_create, locks_to_create, transfers_to_create = apply_rule_grouping(datasetfiles=datasetfiles,
                                                                                    locks=locks,
                                                                                    replicas=replicas,
                                                                                    source_replicas=source_replicas,
                                                                                    rseselector=rseselector,
```

### Comparing `rucio-34.3.0/lib/rucio/core/rule_grouping.py` & `rucio-34.4.0/lib/rucio/core/rule_grouping.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from collections.abc import Sequence
 from datetime import datetime
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Optional
 
 from sqlalchemy import func
 from sqlalchemy.exc import NoResultFound
 
 import rucio.core.did
 import rucio.core.lock
 import rucio.core.replica
@@ -38,20 +38,21 @@
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
 
 @transactional_session
 def apply_rule_grouping(
     datasetfiles: Sequence[dict[str, Any]],
-    locks: dict[tuple[InternalScope, str], models.ReplicaLock],
+    locks: dict[tuple[InternalScope, str], Sequence[models.ReplicaLock]],
     replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
     source_replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
-    rseselector: RSESelector, rule: models.ReplicationRule,
-    preferred_rse_ids: Sequence[str] = [],
-    source_rses: Sequence[str] = [],
+    rseselector: RSESelector,
+    rule: models.ReplicationRule,
+    preferred_rse_ids: Optional[Sequence[str]] = None,
+    source_rses: Optional[Sequence[str]] = None,
     *,
     session: "Session"
 ) -> tuple[dict[str, list[dict[str, models.RSEFileAssociation]]],
            dict[str, list[dict[str, models.ReplicaLock]]],
            list[dict[str, Any]]]:
     """
     Apply rule grouping to files.
@@ -70,14 +71,16 @@
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     # locks_to_create =     {'rse_id': [locks]}
     # replicas_to_create =  {'rse_id': [replicas]}
     # transfers_to_create = [{'dest_rse_id':, 'scope':, 'name':, 'request_type':, 'metadata':}]
 
+    preferred_rse_ids = preferred_rse_ids or []
+    source_rses = source_rses or []
     if rule.grouping == RuleGrouping.NONE:
         replicas_to_create, locks_to_create, \
             transfers_to_create = __apply_rule_to_files_none_grouping(datasetfiles=datasetfiles,
                                                                       locks=locks,
                                                                       replicas=replicas,
                                                                       source_replicas=source_replicas,
                                                                       rseselector=rseselector,
@@ -220,15 +223,28 @@
             'request_type': request_type,
             'retry_count': retry_count,
             'account': rule.account,
             'requested_at': lock.created_at if lock else rule.created_at}
 
 
 @transactional_session
-def __apply_rule_to_files_none_grouping(datasetfiles, locks, replicas, source_replicas, rseselector, rule, preferred_rse_ids=[], source_rses=[], *, session: "Session"):
+def __apply_rule_to_files_none_grouping(
+    datasetfiles: Sequence[dict[str, Any]],
+    locks: dict[tuple[InternalScope, str], Sequence[models.ReplicaLock]],
+    replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
+    source_replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
+    rseselector: RSESelector,
+    rule: models.ReplicationRule,
+    preferred_rse_ids: Optional[Sequence[str]] = None,
+    source_rses: Optional[Sequence[str]] = None,
+    *,
+    session: "Session"
+) -> tuple[dict[str, list[dict[str, models.RSEFileAssociation]]],
+           dict[str, list[dict[str, models.ReplicaLock]]],
+           list[dict[str, Any]]]:
     """
     Apply a rule to files with NONE grouping.
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
@@ -240,31 +256,33 @@
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create
     :raises:                   InsufficientAccountLimit, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
     locks_to_create = {}            # {'rse_id': [locks]}
     replicas_to_create = {}         # {'rse_id': [replicas]}
     transfers_to_create = []        # [{'dest_rse_id':, 'scope':, 'name':, 'request_type':, 'metadata':}]
+    preferred_rse_ids = preferred_rse_ids or []
+    source_rses = source_rses or []
 
     for dataset in datasetfiles:
         selected_rse_ids = []
         for file in dataset['files']:
             if len([lock for lock in locks[(file['scope'], file['name'])] if lock.rule_id == rule.id]) == rule.copies:
                 # Nothing to do as the file already has the requested amount of locks
                 continue
-            rse_coverage = {replica.rse_id: file['bytes'] for replica in replicas[(file['scope'], file['name'])] if replica.state in (ReplicaState.AVAILABLE, ReplicaState.COPYING, ReplicaState.TEMPORARY_UNAVAILABLE)}
+            rse_coverage = {str(replica.rse_id): file['bytes'] for replica in replicas[(file['scope'], file['name'])] if replica.state in (ReplicaState.AVAILABLE, ReplicaState.COPYING, ReplicaState.TEMPORARY_UNAVAILABLE)}
             if len(preferred_rse_ids) == 0:
                 rse_tuples = rseselector.select_rse(size=file['bytes'],
                                                     preferred_rse_ids=rse_coverage.keys(),
-                                                    blocklist=[replica.rse_id for replica in replicas[(file['scope'], file['name'])] if replica.state == ReplicaState.BEING_DELETED],
+                                                    blocklist=[str(replica.rse_id) for replica in replicas[(file['scope'], file['name'])] if replica.state == ReplicaState.BEING_DELETED],
                                                     existing_rse_size=rse_coverage)
             else:
                 rse_tuples = rseselector.select_rse(size=file['bytes'],
                                                     preferred_rse_ids=preferred_rse_ids,
-                                                    blocklist=[replica.rse_id for replica in replicas[(file['scope'], file['name'])] if replica.state == ReplicaState.BEING_DELETED],
+                                                    blocklist=[str(replica.rse_id) for replica in replicas[(file['scope'], file['name'])] if replica.state == ReplicaState.BEING_DELETED],
                                                     existing_rse_size=rse_coverage)
             for rse_tuple in rse_tuples:
                 if len([lock for lock in locks[(file['scope'], file['name'])] if lock.rule_id == rule.id and lock.rse_id == rse_tuple[0]]) == 1:
                     # Due to a bug a lock could have been already submitted for this, in that case, skip it
                     continue
                 __create_lock_and_replica(file=file,
                                           dataset=dataset,
@@ -301,15 +319,28 @@
                                                     name=dataset['name'],
                                                     did_type=DIDType.DATASET).save(flush=False, session=session)
 
     return replicas_to_create, locks_to_create, transfers_to_create
 
 
 @transactional_session
-def __apply_rule_to_files_all_grouping(datasetfiles, locks, replicas, source_replicas, rseselector, rule, preferred_rse_ids=[], source_rses=[], *, session: "Session"):
+def __apply_rule_to_files_all_grouping(
+    datasetfiles: Sequence[dict[str, Any]],
+    locks: dict[tuple[InternalScope, str], Sequence[models.ReplicaLock]],
+    replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
+    source_replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
+    rseselector: RSESelector,
+    rule: models.ReplicationRule,
+    preferred_rse_ids: Optional[Sequence[str]] = None,
+    source_rses: Optional[Sequence[str]] = None,
+    *,
+    session: "Session"
+) -> tuple[dict[str, list[dict[str, models.RSEFileAssociation]]],
+           dict[str, list[dict[str, models.ReplicaLock]]],
+           list[dict[str, Any]]]:
     """
     Apply a rule to files with ALL grouping.
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source_replicas.
@@ -322,14 +353,16 @@
     :raises:                   InsufficientQuota, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
 
     locks_to_create = {}            # {'rse_id': [locks]}
     replicas_to_create = {}         # {'rse_id': [replicas]}
     transfers_to_create = []        # [{'dest_rse_id':, 'scope':, 'name':, 'request_type':, 'metadata':}]
+    preferred_rse_ids = preferred_rse_ids or []
+    source_rses = source_rses or []
 
     bytes_ = 0
     rse_coverage = {}  # {'rse_id': coverage }
     blocklist = set()
     for dataset in datasetfiles:
         for file in dataset['files']:
             bytes_ += file['bytes']
@@ -421,15 +454,28 @@
                                                     name=dataset['name'],
                                                     did_type=DIDType.DATASET).save(flush=False, session=session)
 
     return replicas_to_create, locks_to_create, transfers_to_create
 
 
 @transactional_session
-def __apply_rule_to_files_dataset_grouping(datasetfiles, locks, replicas, source_replicas, rseselector, rule, preferred_rse_ids=[], source_rses=[], *, session: "Session"):
+def __apply_rule_to_files_dataset_grouping(
+    datasetfiles: Sequence[dict[str, Any]],
+    locks: dict[tuple[InternalScope, str], Sequence[models.ReplicaLock]],
+    replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
+    source_replicas: dict[tuple[InternalScope, str], Sequence[models.CollectionReplica]],
+    rseselector: RSESelector,
+    rule: models.ReplicationRule,
+    preferred_rse_ids: Optional[Sequence[str]] = None,
+    source_rses: Optional[Sequence[str]] = None,
+    *,
+    session: "Session"
+) -> tuple[dict[str, list[dict[str, models.RSEFileAssociation]]],
+           dict[str, list[dict[str, models.ReplicaLock]]],
+           list[dict[str, Any]]]:
     """
     Apply a rule to files with ALL grouping.
 
     :param datasetfiles:       Dict holding all datasets and files.
     :param locks:              Dict holding all locks.
     :param replicas:           Dict holding all replicas.
     :param source_replicas:    Dict holding all source replicas.
@@ -441,14 +487,16 @@
     :returns:                  replicas_to_create, locks_to_create, transfers_to_create
     :raises:                   InsufficientQuota, InsufficientTargetRSEs
     :attention:                This method modifies the contents of the locks and replicas input parameters.
     """
     locks_to_create = {}            # {'rse_id': [locks]}
     replicas_to_create = {}         # {'rse_id': [replicas]}
     transfers_to_create = []        # [{'dest_rse_id':, 'scope':, 'name':, 'request_type':, 'metadata':}]
+    preferred_rse_ids = preferred_rse_ids or []
+    source_rses = source_rses or []
 
     for dataset in datasetfiles:
         bytes_ = sum([file['bytes'] for file in dataset['files']])
         rse_coverage = {}  # {'rse_id': coverage }
         blocklist = set()
         for file in dataset['files']:
             for replica in replicas[(file['scope'], file['name'])]:
```

### Comparing `rucio-34.3.0/lib/rucio/core/scope.py` & `rucio-34.4.0/lib/rucio/core/scope.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from re import match
 from traceback import format_exc
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional
 
 from sqlalchemy.exc import IntegrityError
 
 from rucio.common.exception import AccountNotFound, Duplicate, RucioException, VONotFound
 from rucio.core.vo import vo_exists
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import AccountStatus, ScopeStatus
@@ -75,22 +75,23 @@
             add_scope(scope, account, session=session)
         except Duplicate:
             if not skipExisting:
                 raise
 
 
 @read_session
-def list_scopes(filter_={}, *, session: "Session"):
+def list_scopes(filter_: Optional[dict[str, Any]] = None, *, session: "Session") -> list[str]:
     """
     Lists all scopes.
     :param filter_: Dictionary of attributes by which the input data should be filtered
     :param session: The database session in use.
 
     :returns: A list containing all scopes.
     """
+    filter_ = filter_ or {}
     scope_list = []
     query = session.query(models.Scope).filter(models.Scope.status != ScopeStatus.DELETED)
     for filter_type in filter_:
         if filter_type == 'scope':
             if '*' in filter_['scope'].internal:
                 scope_str = filter_['scope'].internal.replace('*', '%')
                 query = query.filter(models.Scope.scope.like(scope_str))
```

### Comparing `rucio-34.3.0/lib/rucio/core/subscription.py` & `rucio-34.4.0/lib/rucio/core/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/topology.py` & `rucio-34.4.0/lib/rucio/core/topology.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/trace.py` & `rucio-34.4.0/lib/rucio/core/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/transfer.py` & `rucio-34.4.0/lib/rucio/core/transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/core/vo.py` & `rucio-34.4.0/lib/rucio/core/vo.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     new_root = InternalAccount('root', vo=vo)
     add_account(account=new_root, type_=AccountType['SERVICE'], email=email, session=session)
     add_account_identity(identity='root@{}'.format(vo),
                          type_=IdentityType['USERPASS'],
                          account=new_root,
                          email=email,
                          default=False,
-                         password='password',
+                         password='password',  # noqa: S106
                          session=session)
 
     for ident in list_identities(account=InternalAccount('super_root', vo='def'), session=session):
         add_account_identity(identity=ident['identity'], type_=ident['type'], account=new_root, email='', session=session)
 
 
 @read_session
```

### Comparing `rucio-34.3.0/lib/rucio/core/volatile_replica.py` & `rucio-34.4.0/lib/rucio/core/volatile_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/abacus/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/abacus/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/abacus/account.py` & `rucio-34.4.0/lib/rucio/daemons/abacus/account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/abacus/collection_replica.py` & `rucio-34.4.0/lib/rucio/daemons/abacus/collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/abacus/rse.py` & `rucio-34.4.0/lib/rucio/daemons/abacus/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/atropos/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/atropos/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/atropos/atropos.py` & `rucio-34.4.0/lib/rucio/daemons/atropos/atropos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/auditor/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/auditor/hdfs.py` & `rucio-34.4.0/lib/rucio/daemons/auditor/hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/auditor/srmdumps.py` & `rucio-34.4.0/lib/rucio/daemons/auditor/srmdumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import glob
 import hashlib
 import html.parser as HTMLParser
 import logging
 import operator
 import os
 import re
+from typing import Optional
 
 import gfal2
 import requests
 
 from rucio.common.config import get_config_dirs
 from rucio.common.constants import RseAttr
 from rucio.common.dumper import DUMPS_CACHE_DIR, HTTPDownloadFailed, ddmendpoint_url, gfal_download_to_file, http_download_to_file, temp_file
@@ -193,19 +194,20 @@
 def download(url, filename):
     '''
     Given the URL `url` downloads its contents on `filename`.
     '''
     return protocol_funcs[protocol(url)]['download'](url, filename)
 
 
-def parse_configuration(conf_dirs=__DUMPERCONFIGDIRS):
+def parse_configuration(conf_dirs: Optional[list[str]] = None) -> Parser:
     '''
     Parses the configuration for the endpoints contained in `conf_dir`.
     Returns a ConfParser.RawConfParser subclass instance.
     '''
+    conf_dirs = conf_dirs or __DUMPERCONFIGDIRS
     logger = logging.getLogger('auditor.srmdumps')
     if len(conf_dirs) == 0:
         logger.error('No configuration directory given to load SRM dumps paths')
         raise Exception('No configuration directory given to load SRM dumps paths')
 
     configuration = Parser({
         'disabled': False,
```

### Comparing `rucio-34.3.0/lib/rucio/daemons/automatix/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/automatix/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/automatix/automatix.py` & `rucio-34.4.0/lib/rucio/daemons/automatix/automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/badreplicas/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/badreplicas/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/badreplicas/minos.py` & `rucio-34.4.0/lib/rucio/daemons/badreplicas/minos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py` & `rucio-34.4.0/lib/rucio/daemons/badreplicas/minos_temporary_expiration.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/badreplicas/necromancer.py` & `rucio-34.4.0/lib/rucio/daemons/badreplicas/necromancer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/bb8/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/bb8/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/bb8/bb8.py` & `rucio-34.4.0/lib/rucio/daemons/bb8/bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/bb8/common.py` & `rucio-34.4.0/lib/rucio/daemons/bb8/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from datetime import date, datetime, timedelta
 from string import Template
+from typing import Any, Optional
 
 from requests import get
 from sqlalchemy import BigInteger, and_, cast, func, or_
 from sqlalchemy.orm import aliased
 from sqlalchemy.sql.expression import case, select
 
 from rucio.common.config import config_get, config_get_bool, config_get_int
@@ -474,39 +475,40 @@
         models.DatasetLock.accessed_at,
     ).all()
     return summary
 
 
 @read_session
 def select_target_rse(
-    parent_rule,
-    current_rse_id,
-    rse_expression,
-    subscription_id,
-    rse_attributes,
-    other_rses=[],
-    exclude_expression=None,
-    force_expression=None,
+    parent_rule: dict[str, Any],
+    current_rse_id: str,
+    rse_expression: str,
+    subscription_id: str,
+    rse_attributes: dict[str, Any],
+    other_rses: Optional[list[str]] = None,
+    exclude_expression: Optional[str] = None,
+    force_expression: Optional[str] = None,
     *,
     session=None,
-):
+) -> str:
     """
     Select a new target RSE for a rebalanced rule.
     :param parent_rule           rule that is rebalanced.
     :param current_rse_id:       RSE of the source.
     :param rse_expression:       RSE Expression of the source rule.
     :param subscription_id:      Subscription ID of the source rule.
     :param rse_attributes:       The attributes of the source rse.
     :param other_rses:           Other RSEs with existing dataset replicas.
     :param exclude_expression:   Exclude this rse_expression from being target_rses.
     :param force_expression:     Force a specific rse_expression as target.
     :param session:              The DB Session.
     :returns:                    New RSE expression.
     """
 
+    other_rses = other_rses or []
     current_rse = get_rse_name(rse_id=current_rse_id)
     current_rse_expr = current_rse
     # if parent rule has a vo, enforce it
     vo = parent_rule["scope"].vo
     if exclude_expression:
         target_rse = "((%s)|(%s))" % (exclude_expression, current_rse_expr)
     else:
```

### Comparing `rucio-34.3.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py` & `rucio-34.4.0/lib/rucio/daemons/bb8/nuclei_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/bb8/t2_background_rebalance.py` & `rucio-34.4.0/lib/rucio/daemons/bb8/t2_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/simple.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/c3po.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/c3po.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/agis.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/agis.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/free_space.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/jedi_did.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/jedi_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/mock_did.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/mock_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/network_metrics.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/network_metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/collectors/workload.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/collectors/workload.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/utils/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/utils/dataset_cache.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/utils/dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/utils/expiring_list.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/utils/expiring_list.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/utils/popularity.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/utils/popularity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/c3po/utils/timeseries.py` & `rucio-34.4.0/lib/rucio/daemons/c3po/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/cache/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/cache/consumer.py` & `rucio-34.4.0/lib/rucio/daemons/cache/consumer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/common.py` & `rucio-34.4.0/lib/rucio/daemons/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/common.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/finisher.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/finisher.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/poller.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/poller.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/preparer.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/receiver.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/receiver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/stager.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/stager.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,30 +75,31 @@
     Graceful exit.
     """
 
     GRACEFUL_STOP.set()
 
 
 def run(
-        once=False,
-        total_threads=1,
-        group_bulk=1,
-        group_policy='rule',
-        rses=None,
-        include_rses=None,
-        exclude_rses=None,
-        vos=None,
-        bulk=100,
-        source_strategy=None,
-        activities=[],
-        sleep_time=600
-):
+    once: bool = False,
+    total_threads: int = 1,
+    group_bulk: int = 1,
+    group_policy: str = 'rule',
+    rses: Optional[list[str]] = None,
+    include_rses: Optional[str] = None,
+    exclude_rses: Optional[str] = None,
+    vos: Optional[list[str]] = None,
+    bulk: int = 100,
+    source_strategy: Optional[str] = None,
+    activities: Optional[list[str]] = None,
+    sleep_time: int = 600
+) -> None:
     """
     Starts up the conveyor threads.
     """
+    activities = activities or []
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise exception.DatabaseException('Database was not updated, daemon won\'t start')
 
     multi_vo = config_get_bool('common', 'multi_vo', raise_exception=False, default=False)
     working_rses = None
```

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/submitter.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/conveyor/throttler.py` & `rucio-34.4.0/lib/rucio/daemons/conveyor/throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/follower/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/follower/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/follower/follower.py` & `rucio-34.4.0/lib/rucio/daemons/follower/follower.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/hermes/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/hermes/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/hermes/hermes.py` & `rucio-34.4.0/lib/rucio/daemons/hermes/hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/judge/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/judge/cleaner.py` & `rucio-34.4.0/lib/rucio/daemons/judge/cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/judge/evaluator.py` & `rucio-34.4.0/lib/rucio/daemons/judge/evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/judge/injector.py` & `rucio-34.4.0/lib/rucio/daemons/judge/injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/judge/repairer.py` & `rucio-34.4.0/lib/rucio/daemons/judge/repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/oauthmanager/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/oauthmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/oauthmanager/oauthmanager.py` & `rucio-34.4.0/lib/rucio/daemons/oauthmanager/oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/reaper/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/reaper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/reaper/dark_reaper.py` & `rucio-34.4.0/lib/rucio/daemons/reaper/dark_reaper.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,29 +184,40 @@
 def stop(signum: "Optional[int]" = None, frame: "Optional[FrameType]" = None) -> None:
     """
     Graceful exit.
     """
     GRACEFUL_STOP.set()
 
 
-def run(total_workers=1, chunk_size=100, once=False, rses=[], scheme=None,
-        exclude_rses=None, include_rses=None, vos=None, delay_seconds=0, sleep_time=300):
+def run(
+    total_workers: int = 1,
+    chunk_size: int = 100,
+    once: bool = False,
+    rses: "Optional[list[str]]" = None,
+    scheme: "Optional[str]" = None,
+    exclude_rses: "Optional[str]" = None,
+    include_rses: "Optional[str]" = None,
+    vos: "Optional[list[str]]" = None,
+    delay_seconds: int = 0,
+    sleep_time: int = 300
+) -> None:
     """
     Starts up the reaper threads.
 
     :param total_workers: The total number of workers.
     :param chunk_size: the size of chunk for deletion.
     :param once: If True, only runs one iteration of the main loop.
     :param rses: List of RSEs the reaper should work against. If empty, it considers all RSEs (Single-VO only).
     :param scheme: Force the reaper to use a particular protocol/scheme, e.g., mock.
     :param exclude_rses: RSE expression to exclude RSEs from the Reaper.
     :param include_rses: RSE expression to include RSEs.
     :param vos: VOs on which to look for RSEs. Only used in multi-VO mode.
                 If None, we either use all VOs if run from "def", or the current VO otherwise.
     """
+    rses = rses or []
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise exception.DatabaseException('Database was not updated, daemon won\'t start')
 
     logging.info('main: starting processes')
```

### Comparing `rucio-34.3.0/lib/rucio/daemons/reaper/reaper.py` & `rucio-34.4.0/lib/rucio/daemons/reaper/reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/replicarecoverer/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/replicarecoverer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py` & `rucio-34.4.0/lib/rucio/daemons/replicarecoverer/suspicious_replica_recoverer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 
 import functools
 import json
 import logging
 import re
 import threading
 import time
+from configparser import NoOptionError, NoSectionError
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, Optional
 
 import rucio.db.sqla.util
-from rucio.common.config import config_get_bool
+from rucio.common.config import config_get, config_get_bool
 from rucio.common.constants import SuspiciousAvailability
 from rucio.common.exception import DatabaseException, DuplicateRule, VONotFound
 from rucio.common.logging import setup_logging
-from rucio.common.types import InternalAccount
+from rucio.common.types import InternalAccount, LoggerFunction
 from rucio.core.did import get_metadata
 from rucio.core.replica import (
     add_bad_pfns,
     declare_bad_file_replicas,
     get_suspicious_files,
     get_suspicious_reason,
     list_replicas,
@@ -45,14 +46,15 @@
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.core.rule import add_rule
 from rucio.core.vo import list_vos
 from rucio.daemons.common import run_daemon
 from rucio.db.sqla.util import get_db_time
 
 if TYPE_CHECKING:
+    from collections.abc import Sequence
     from types import FrameType
 
 GRACEFUL_STOP = threading.Event()
 DAEMON_NAME = 'suspicious-replica-recoverer'
 
 
 def check_suspicious_policy(policy: dict[str, str], file_metadata_datatype: str, file_metadata_scope: str) -> str:
@@ -76,15 +78,62 @@
 
     if match_scope and match_datatype:
         action = policy["action"]
 
     return action
 
 
-def declare_suspicious_replicas_bad(once: bool = False, younger_than: int = 5, nattempts: int = 5, vos: Optional[list[str]] = None, limit_suspicious_files_on_rse: int = 5, json_file_name: str = "/opt/rucio/etc/suspicious_replica_recoverer.json", sleep_time: int = 3600, active_mode: bool = False) -> None:
+def parse_replica_datatype(
+        did_name_expression: Optional[str],
+        file_name: str,
+        rse_key: str,
+        logger: LoggerFunction) -> Optional[str]:
+
+    file_metadata_datatype = None
+    if did_name_expression is not None:
+        logger(logging.WARNING, f'Using {did_name_expression} as regex to determine file datatype for file: {file_name} on rse: {rse_key}')
+        try:
+            file_metadata_datatype_reg = re.compile(did_name_expression).search(file_name)
+            if file_metadata_datatype_reg is not None:
+                file_metadata_datatype = file_metadata_datatype_reg[0]
+        except (re.error, TypeError) as e:
+            logger(logging.WARNING, f'Could not determine datatype using regex {did_name_expression} on file: {file_name}, ignoring: {e}')
+
+    return file_metadata_datatype
+
+
+def _read_from_config(logger: LoggerFunction) -> tuple[str, bool, Optional[str]]:
+    rule_suspicious_rse_expression = config_get("replicarecoverer", "rule_rse_expression", raise_exception=False, default='type=SCRATCHDISK')
+    logger(logging.INFO, f"Recovering with the rse expression: {rule_suspicious_rse_expression}")
+
+    use_file_metadata = config_get_bool("replicarecoverer", "use_file_metadata", raise_exception=False, default=True)
+    did_name_expression = None
+
+    if not use_file_metadata:
+        try:
+            did_name_expression = config_get('replicarecoverer', 'did_name_expression', raise_exception=True)
+            logger(logging.INFO, f"Setting replica datatype from did name with regex expression: {did_name_expression}")
+
+        except (NoOptionError, NoSectionError) as e:
+            logger(logging.WARNING, f"Cannot use option 'use_file_metadata' without setting a replacement expression with 'did_name_expression'- {e}")
+            use_file_metadata = True
+
+    logger(logging.INFO, f"Recovering with the rse expression: {rule_suspicious_rse_expression}")
+    return rule_suspicious_rse_expression, use_file_metadata, did_name_expression
+
+
+def declare_suspicious_replicas_bad(
+        once: bool = False,
+        younger_than: int = 5,
+        nattempts: int = 5,
+        vos: "Optional[Sequence[str]]" = None,
+        limit_suspicious_files_on_rse: int = 5,
+        json_file_name: str = "/opt/rucio/etc/suspicious_replica_recoverer.json",
+        sleep_time: int = 3600,
+        active_mode: bool = False) -> None:
     """
     Main loop to check for available replicas which are labeled as suspicious.
 
     Gets a list of suspicious replicas that are listed as AVAILABLE in 'replicas' table
     and available on other RSE. Finds surls of these replicas and declares them as bad.
     Replicas that are the last remaining copy of a file have additional checks (checksum
     comparison, etc.) before being declared bad.
@@ -119,18 +168,18 @@
             limit_suspicious_files_on_rse=limit_suspicious_files_on_rse,
             json_file_name=json_file_name,
             active_mode=active_mode
         ),
     )
 
 
-def run_once(heartbeat_handler: Any, younger_than: int, nattempts: int, vos: Optional[list[str]], limit_suspicious_files_on_rse: int, json_file_name: str, active_mode: int, **_kwargs) -> bool:
-
-    worker_number, total_workers, logger = heartbeat_handler.live()
+def run_once(heartbeat_handler: Any, younger_than: int, nattempts: int, vos: "Optional[Sequence[str]]", limit_suspicious_files_on_rse: int, json_file_name: str, active_mode: int, **_kwargs) -> bool:
 
+    _, _, logger = heartbeat_handler.live()
+    rule_suspicious_rse_expression, use_file_metadata, did_name_expression = _read_from_config(logger=logger)
     vos = vos or []
 
     multi_vo = config_get_bool('common', 'multi_vo', raise_exception=False, default=False)
     if not multi_vo:
         if vos:
             logger(logging.WARNING, 'Ignoring argument vos, this is only applicable in a multi-VO setup.')
         vos = ['def']
@@ -298,15 +347,15 @@
                 logger(logging.DEBUG, 'List of replicas on %s with nattempts=1 for which the pfns have been found:', rse_expr)
                 for i in replicas_nattempts_1[vo][rse_expr]:
                     logger(logging.DEBUG, '%s', i)
 
         logger(logging.INFO, 'All RSEs have been checked for suspicious replicas. Total time: %s seconds.', time.time() - start)
 
         # Checking that everything is still working properly
-        worker_number, total_workers, logger = heartbeat_handler.live()
+        _, _, logger = heartbeat_handler.live()
 
         logger(logging.INFO, 'Create rules for replicas with nattempts=1.')
 
         # Create as many rules as necessary for the replicas to be picked up by the daemon on the next run
         # Create rules only for replicas that can be declared bad.
         # Replicas from the auditor should be declared bad regardless of suspicious declarations, so no rules necessary.
         for rse_key in list(replicas_nattempts_1[vo].keys()):
@@ -336,19 +385,21 @@
                 if not from_auditor:
                     if (file_name.startswith("log.")) or (file_name.startswith("user")):
                         # Don't keep log files or user files
                         files_to_be_declared_bad_nattempts_1.append(replicas_nattempts_1[vo][rse_key][replica_key])
                         action = ""
                     else:
                         # Deal with replicas based on their metadata.
-                        if file_metadata["datatype"] is None:  # "None" type has no function "split()"
+                        if (file_metadata["datatype"] is None) and (use_file_metadata):  # "None" type has no function "split()"
                             logger(logging.WARNING, "RSE: %s, replica name %s, surl %s: Replica does not have a data type associated with it. No action will be taken.",
                                    rse_key, replica_key, replicas_nattempts_1[vo][rse_key][replica_key]['surl'])
                             continue
                         file_metadata_datatype = str(file_metadata["datatype"])
+                        if not use_file_metadata:
+                            file_metadata_datatype = parse_replica_datatype(did_name_expression, file_name, rse_key, logger)
                         file_metadata_scope = str(file_metadata["scope"])
                         action = ""
                         if file_metadata_datatype:
                             # Some files don't have a datatype. They should be ignored.
                             for policy in json_data:
                                 action = check_suspicious_policy(policy=policy, file_metadata_datatype=file_metadata_datatype, file_metadata_scope=file_metadata_scope)
                                 if action:
@@ -357,15 +408,15 @@
                     if action:
                         # Rules will be created for these replicas.
                         dids = {'scope': file_scope, 'name': file_name, 'rse': rse_key}
                         dids_nattempts_1.append(dids)
             if active_mode:
                 if len(dids_nattempts_1) > 0:
                     try:
-                        add_rule(dids=dids_nattempts_1, account=InternalAccount('root', vo=vo), copies=nattempts, rse_expression='type=SCRATCHDISK', grouping=None, weight=None, lifetime=5 * 24 * 3600, locked=False, subscription_id=None)
+                        add_rule(dids=dids_nattempts_1, account=InternalAccount('root', vo=vo), copies=nattempts, rse_expression=rule_suspicious_rse_expression, grouping=None, weight=None, lifetime=5 * 24 * 3600, locked=False, subscription_id=None)
                         logger(logging.INFO, 'Rules have been created for %i replicas on %s.', len(dids_nattempts_1), rse_key)
                     except DuplicateRule:
                         logger(logging.INFO, 'Tried to create rules on %s, but it already exists.', rse_key)
                 else:
                     logger(logging.INFO, 'No replicas on %s have nattmepts=1, so no rules have been created.', rse_key)
                 if len(files_to_be_declared_bad_nattempts_1) > 0:
                     logger(logging.INFO, 'Ready to declare %s bad replica(s) with nattempts=1 on %s (RSE id: %s).', len(files_to_be_declared_bad_nattempts_1), rse_key, str(rse_id))
@@ -399,15 +450,15 @@
                 del recoverable_replicas[vo][rse_key]
 
         logger(logging.INFO, "Following RSEs were deemed problematic (total: %s)", len(list_problematic_rses))
         for rse in list_problematic_rses:
             logger(logging.INFO, "%s", rse)
 
         # Checking that everything is still working properly
-        worker_number, total_workers, logger = heartbeat_handler.live()
+        _, _, logger = heartbeat_handler.live()
 
         auditor = 0
         checksum = 0
 
         # Label suspicious replicas as bad if they have other copies on other RSEs (that aren't also marked as suspicious).
         # If they are the last remaining copies, deal with them differently.
         for rse_key in list(recoverable_replicas[vo].keys()):
@@ -447,21 +498,23 @@
                     elif recoverable_replicas[vo][rse_key][replica_key]['available_elsewhere'] is False:
                         if (file_name.startswith("log.")) or (file_name.startswith("user")):
                             # Don't keep log files or user files
                             files_to_be_declared_bad.append(recoverable_replicas[vo][rse_key][replica_key])
                             del recoverable_replicas[vo][rse_key][replica_key]
                         else:
                             # Deal with replicas based on their metadata.
-                            if file_metadata["datatype"] is None:  # "None" type has no function "split()"
+                            if (file_metadata["datatype"] is None) and use_file_metadata:  # "None" type has no function "split()"
                                 files_to_be_ignored.append(recoverable_replicas[vo][rse_key][replica_key])
                                 logger(logging.WARNING, "RSE: %s, replica name %s, surl %s: Replica does not have a data type associated with it. No action will be taken.",
                                        rse_key, replica_key, recoverable_replicas[vo][rse_key][replica_key]['surl'])
                                 continue
 
                             file_metadata_datatype = str(file_metadata["datatype"])
+                            if not use_file_metadata:
+                                file_metadata_datatype = parse_replica_datatype(did_name_expression, file_name, rse_key, logger)
                             file_metadata_scope = str(file_metadata["scope"])
                             action = ""
                             if file_metadata_datatype:
                                 # Some files don't have a datatype. They should be ignored.
                                 for policy in json_data:
                                     action = check_suspicious_policy(policy=policy, file_metadata_datatype=file_metadata_datatype, file_metadata_scope=file_metadata_scope)
                                     if action:
@@ -520,15 +573,23 @@
 
     time_passed = time.time() - start
     logger(logging.INFO, 'Total time: %s seconds', time_passed)
     must_sleep = True
     return must_sleep
 
 
-def run(once: bool = False, younger_than: int = 5, nattempts: int = 5, vos: list[str] = None, limit_suspicious_files_on_rse: int = 5, json_file_name: str = "/opt/rucio/etc/suspicious_replica_recoverer.json", sleep_time: int = 3600, active_mode: bool = False) -> None:
+def run(
+        once: bool = False,
+        younger_than: int = 5,
+        nattempts: int = 5,
+        vos: "Optional[Sequence[str]]" = None,
+        limit_suspicious_files_on_rse: int = 5,
+        json_file_name: str = "/opt/rucio/etc/suspicious_replica_recoverer.json",
+        sleep_time: int = 3600,
+        active_mode: bool = False) -> None:
     """
     Starts up the Suspicious-Replica-Recoverer threads.
     """
     setup_logging(process_name=DAEMON_NAME)
 
     if rucio.db.sqla.util.is_old_db():
         raise DatabaseException('Database was not updated, daemon won\'t start')
```

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/config.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/profiles/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py` & `rucio-34.4.0/lib/rucio/daemons/rsedecommissioner/rse_decommissioner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/storage/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/storage/consistency/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/storage/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/storage/consistency/actions.py` & `rucio-34.4.0/lib/rucio/daemons/storage/consistency/actions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/tracer/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/tracer/kronos.py` & `rucio-34.4.0/lib/rucio/daemons/tracer/kronos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/transmogrifier/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/transmogrifier/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/transmogrifier/transmogrifier.py` & `rucio-34.4.0/lib/rucio/daemons/transmogrifier/transmogrifier.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/undertaker/__init__.py` & `rucio-34.4.0/lib/rucio/daemons/undertaker/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/daemons/undertaker/undertaker.py` & `rucio-34.4.0/lib/rucio/daemons/undertaker/undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/__init__.py` & `rucio-34.4.0/lib/rucio/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/__init__.py` & `rucio-34.4.0/lib/rucio/db/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/constants.py` & `rucio-34.4.0/lib/rucio/db/sqla/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/__init__.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/env.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/env.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/01eaf73ab656_add_new_rule_notification_state_progress.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/0f1adb7a599a_create_transfer_hops_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/13d4f70c66a9_introduce_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/140fef722e91_cleanup_distances_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1677d4d803c8_split_rse_availability_into_multiple.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1c45d9730ca6_increase_identity_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1f46c5f240ac_add_bytes_column_to_bad_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2190e703eb6e_move_rse_settings_to_rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/27e3a68927fb_remove_replicas_tombstone_and_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/295289b5a800_processed_by_and__at_in_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2962ece31cf4_add_nbaccesses_column_in_the_did_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b69addda658_add_columns_for_third_party_copy_read_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2cbee484dcf9_added_column_volume_to_rse_transfer_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/30fa38b6434e_add_index_on_service_column_in_the_message_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3345511706b8_replicas_table_pk_definition_is_in_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ac1660a1a72_extend_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/4df2c5ddabc0_remove_temporary_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/50280c53117c_add_qos_class_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52153819589c_add_rse_id_to_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/53b479c3cb0f_fix_did_meta_table_missing_updated_at_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5673b4b6e843_add_wfms_metadata_to_rule_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/688ef1840840_adding_did_meta_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/739064d31565_remove_history_table_pks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7541902bf173_add_didsfollowed_and_followevents_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/7ec22226cdbf_new_replica_state_for_temporary_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/810a41685bc1_added_columns_rse_transfer_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/83f991c63a93_correct_rse_expression_length.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8523998e2e76_increase_size_of_extended_attributes_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/8ea9122275b1_adding_missing_function_based_indices.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/90f47792bb76_add_clob_payload_to_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/94a5961ddbf2_add_estimator_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a1b149a2044_add_saml_identity_type.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9a45bc4ea66d_add_vp_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/9eb936a81eb1_true_is_true.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a08fa8de1545_transfer_stats_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a118956323f8_added_vo_table_and_vo_col_to_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a193a275255c_add_status_column_in_messages.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a6eb23955c28_state_idx_non_functional.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a74275a1ad30_added_global_quota_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b4293a99f344_added_column_identity_to_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b7d287de34fd_removal_of_replicastate_source.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b818052fa670_add_index_to_quarantined_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b8caac94d7f0_add_comments_column_for_subscriptions_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/b96a1c7e1cc4_new_bad_pfns_table_and_bad_replicas_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bc68e9946deb_add_staging_timestamps_to_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/bf3baa1c1474_correct_pk_and_idx_for_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c0937668555f_add_qos_policy_map_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/ccdbcd48206e_add_did_type_column_index_on_did_meta_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/cebad904c4dd_new_payload_column_for_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d1189a09c6e0_oauth2_0_and_jwt_feature_support_adding_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d23453595260_extend_request_state_for_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d6e2c3b2cf26_remove_third_party_copy_column_from_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e138c364ebd0_extending_columns_for_filter_and_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/e59300c8b179_support_for_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f1b14a8c2ac1_postgres_use_check_constraints.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f41ffe206f37_oracle_global_temporary_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/f85a2962b021_adding_transfertool_column_to_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fa7a7d78b602_increase_refresh_token_size.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fb28a95fe288_add_replicas_rse_id_tombstone_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe1a65b176c9_set_third_party_copy_read_and_write_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py` & `rucio-34.4.0/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/models.py` & `rucio-34.4.0/lib/rucio/db/sqla/models.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/sautils.py` & `rucio-34.4.0/lib/rucio/db/sqla/sautils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/session.py` & `rucio-34.4.0/lib/rucio/db/sqla/session.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/types.py` & `rucio-34.4.0/lib/rucio/db/sqla/types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/db/sqla/util.py` & `rucio-34.4.0/lib/rucio/db/sqla/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from datetime import datetime
 from hashlib import sha256
 from os import urandom
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
 
 import sqlalchemy
 from alembic import command, op
 from alembic.config import Config
 from dogpile.cache.api import NoValue
 from sqlalchemy import Column, PrimaryKeyConstraint, func, inspect
 from sqlalchemy.dialects.postgresql.base import PGInspector
@@ -30,31 +30,34 @@
 from sqlalchemy.sql.ddl import DropSchema
 from sqlalchemy.sql.expression import select, text
 
 from rucio import alembicrevision
 from rucio.common.cache import make_region_memcached
 from rucio.common.config import config_get, config_get_list
 from rucio.common.schema import get_schema_value
-from rucio.common.types import InternalAccount
+from rucio.common.types import InternalAccount, LoggerFunction
 from rucio.common.utils import generate_uuid
 from rucio.db.sqla import models
 from rucio.db.sqla.constants import AccountStatus, AccountType, IdentityType
 from rucio.db.sqla.session import get_dump_engine, get_engine, get_session
 from rucio.db.sqla.types import InternalScopeString, String
 
 if TYPE_CHECKING:
-    from typing import Optional, Union  # noqa: F401
+    from collections.abc import Sequence
 
-    from sqlalchemy.engine import Inspector  # noqa: F401
-    from sqlalchemy.orm import Session  # noqa: F401
+    from sqlalchemy.engine import Inspector
+    from sqlalchemy.orm import Query, Session
+
+    # TypeVar representing the DeclarativeObj class defined inside _create_temp_table
+    DeclarativeObj = TypeVar('DeclarativeObj')
 
 REGION = make_region_memcached(expiration_time=600, memcached_expire_time=3660)
 
 
-def build_database():
+def build_database() -> None:
     """ Applies the schema to the database. Run this command once to build the database. """
     engine = get_engine()
 
     schema = config_get('database', 'schema', raise_exception=False, check_config_table=False)
     if schema:
         print('Schema set in config, trying to create schema:', schema)
         try:
@@ -67,45 +70,45 @@
     models.register_models(engine)
 
     # Put the database under version control
     alembic_cfg = Config(config_get('alembic', 'cfg'))
     command.stamp(alembic_cfg, "head")
 
 
-def dump_schema():
+def dump_schema() -> None:
     """ Creates a schema dump to a specific database. """
     engine = get_dump_engine()
     models.register_models(engine)
 
 
-def destroy_database():
+def destroy_database() -> None:
     """ Removes the schema from the database. Only useful for test cases or malicious intents. """
     engine = get_engine()
 
     try:
         models.unregister_models(engine)
     except Exception as e:
         print('Cannot destroy schema -- assuming already gone, continuing:', e)
 
 
-def drop_everything():
+def drop_everything() -> None:
     """
     Pre-gather all named constraints and table names, and drop everything.
     This is better than using metadata.reflect(); metadata.drop_all()
     as it handles cyclical constraints between tables.
     Ref. https://github.com/sqlalchemy/sqlalchemy/wiki/DropEverything
     """
     engine = get_engine()
 
     # the transaction only applies if the DB supports
     # transactional DDL, i.e. Postgresql, MS SQL Server
 
     with engine.connect() as conn:
 
-        inspector = inspect(conn)  # type: Union[Inspector, PGInspector]
+        inspector: Union["Inspector", PGInspector] = inspect(conn)
 
         for tname, fkcs in reversed(
                 inspector.get_sorted_table_and_fkc_names(schema='*')):
             if tname:
                 drop_table_stmt = DropTable(Table(tname, MetaData(), schema='*'))
                 conn.execute(drop_table_stmt)
             elif fkcs:
@@ -123,26 +126,26 @@
 
         if engine.dialect.name == 'postgresql':
             assert isinstance(inspector, PGInspector), 'expected a PGInspector'
             for enum in inspector.get_enums(schema='*'):
                 sqlalchemy.Enum(**enum).drop(bind=conn)
 
 
-def create_base_vo():
+def create_base_vo() -> None:
     """ Creates the base VO """
 
     session_scoped = get_session()
 
     vo = models.VO(vo='def', description='Default base VO', email='N/A')
     with session_scoped() as s:
         with s.begin():
             s.add_all([vo])
 
 
-def create_root_account():
+def create_root_account() -> None:
     """
     Inserts the default root account to an existing database. Make sure to change the default password later.
     """
 
     multi_vo = bool(config_get('common', 'multi_vo', False, False))
 
     up_id = 'ddmlab'
@@ -212,15 +215,15 @@
                 s.rollback()
         s.add(account)
         s.flush()
         s.add_all([iaa1, iaa2, iaa3, iaa4])
         s.commit()
 
 
-def get_db_time():
+def get_db_time() -> Optional[datetime]:
     """ Gives the utc time on the db. """
     session_scoped = get_session()
     try:
         storage_date_format = None
         if session_scoped.bind.dialect.name == 'oracle':
             query = select(text("sys_extract_utc(systimestamp)"))
         elif session_scoped.bind.dialect.name == 'mysql':
@@ -237,27 +240,27 @@
             if storage_date_format:
                 return datetime.strptime(now, storage_date_format)
             return now
     finally:
         session_scoped.remove()
 
 
-def get_count(q):
+def get_count(q: "Query") -> int:
     """
     Fast way to get count in SQLAlchemy
     Source: https://gist.github.com/hest/8798884
     Some limits, see a more thorough version above
     """
 
     count_q = q.statement.with_only_columns([func.count()]).order_by(None)
     count = q.session.execute(count_q).scalar()
     return count
 
 
-def is_old_db():
+def is_old_db() -> bool:
     """
     Returns true, if alembic is used and the database is not on the
     same revision as the code base.
     """
     schema = config_get('database', 'schema', raise_exception=False)
 
     # checks if alembic is being used by looking up the AlembicVersion table
@@ -270,15 +273,15 @@
         with s.begin():
             # query = s.query(models.AlembicVersion.version_num)
             query = s.execute(select(models.AlembicVersion)).scalars().all()
             # return query.count() != 0 and str(query.first()[0]) != alembicrevision.ALEMBIC_REVISION
             return (len(query) != 0 and str(query[0].version_num) != alembicrevision.ALEMBIC_REVISION)
 
 
-def json_implemented(*, session=None):
+def json_implemented(*, session: Optional["Session"] = None) -> bool:
     """
     Checks if the database on the current server installation can support json fields.
 
     :param session: The active session of the database.
     :type session: Optional[Session]
     :returns: True, if json is supported, False otherwise.
     """
@@ -291,29 +294,29 @@
             return False
     elif session.bind.dialect.name == 'sqlite':
         return False
 
     return True
 
 
-def try_drop_constraint(constraint_name, table_name):
+def try_drop_constraint(constraint_name: str, table_name: str) -> None:
     """
     Tries to drop the given constrained and returns successfully if the
     constraint already existed on Oracle databases.
 
     :param constraint_name: the constraint's name
     :param table_name: the table name where the constraint resides
     """
     try:
         op.drop_constraint(constraint_name, table_name)
     except DatabaseError as e:
         assert 'nonexistent constraint' in str(e)
 
 
-def list_oracle_global_temp_tables(session):
+def list_oracle_global_temp_tables(session: "Session") -> list[str]:
     """
     Retrieve the list of global temporary tables in oracle
     """
     global_temp_tables = config_get_list('core', 'oracle_global_temp_tables', raise_exception=False, check_config_table=False, default='')
     if global_temp_tables:
         return [t.upper() for t in global_temp_tables]
 
@@ -334,15 +337,22 @@
                 dict(owner=models.BASE.metadata.schema.upper())
             )
         ]
         REGION.set(cache_key, global_temp_tables)
     return global_temp_tables
 
 
-def _create_temp_table(name, *columns, primary_key=None, oracle_global_name=None, session=None, logger=logging.log):
+def _create_temp_table(
+        name: str,
+        *columns: "Sequence[Column]",
+        primary_key: Optional["Sequence[Any]"] = None,
+        oracle_global_name: Optional[str] = None,
+        session: Optional["Session"] = None,
+        logger: LoggerFunction = logging.log
+) -> type["DeclarativeObj"]:
     """
     Create a temporary table with the given columns, register it into a declarative base, and return it.
 
     Attention! calling this function while a table with the same `name` is being used will lead to
     bad consequences. Don't use it in recursive calls without taking special care.
 
     Declarative definition _requires_ a primary key. It should be a subset of '*columns' argument
@@ -448,26 +458,32 @@
     The recursive call may be indirect and hard to catch. For example:
     functionA -> functionB -> functionC -> functionA
 
     The lifecycle of this object is bound to a particular session. In rucio, we naver use
     sessions in multiple threads at a time, so no need to protect indexes with a mutex.
     """
 
-    def __init__(self, session):
+    def __init__(self, session: "Session"):
         self.session = session
 
         self.next_idx_to_use = {}
 
-    def create_temp_table(self, name, *columns, primary_key=None, logger=logging.log):
+    def create_temp_table(
+            self,
+            name: str,
+            *columns: "Sequence[Column]",
+            primary_key: Optional["Sequence[Any]"] = None,
+            logger: LoggerFunction = logging.log
+    ) -> type["DeclarativeObj"]:
         idx = self.next_idx_to_use.setdefault(name, 0)
         table = _create_temp_table(f'{name}_{idx}', *columns, primary_key=primary_key, session=self.session, logger=logger)
         self.next_idx_to_use[name] = idx + 1
         return table
 
-    def create_scope_name_table(self, logger=logging.log):
+    def create_scope_name_table(self, logger: LoggerFunction = logging.log) -> type["DeclarativeObj"]:
         """
         Create a temporary table with columns 'scope' and 'name'
         """
 
         columns = [
             Column("scope", InternalScopeString(get_schema_value('SCOPE_LENGTH'))),
             Column("name", String(get_schema_value('NAME_LENGTH'))),
@@ -475,15 +491,15 @@
         return self.create_temp_table(
             'TEMPORARY_SCOPE_NAME',
             *columns,
             primary_key=columns,
             logger=logger,
         )
 
-    def create_association_table(self, logger=logging.log):
+    def create_association_table(self, logger: LoggerFunction = logging.log) -> type["DeclarativeObj"]:
         """
         Create a temporary table with columns 'scope', 'name', 'child_scope'and 'child_name'
         """
 
         columns = [
             Column("scope", InternalScopeString(get_schema_value('SCOPE_LENGTH'))),
             Column("name", String(get_schema_value('NAME_LENGTH'))),
@@ -493,15 +509,15 @@
         return self.create_temp_table(
             'TEMPORARY_ASSOCIATION',
             *columns,
             primary_key=columns,
             logger=logger,
         )
 
-    def create_id_table(self, logger=logging.log):
+    def create_id_table(self, logger: LoggerFunction = logging.log) -> type["DeclarativeObj"]:
         """
         Create a temp table with a single id column of uuid type
         """
 
         return self.create_temp_table(
             'TEMPORARY_ID',
             Column("id", models.GUID()),
```

### Comparing `rucio-34.3.0/lib/rucio/rse/__init__.py` & `rucio-34.4.0/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/__init__.py` & `rucio-34.4.0/lib/rucio/rse/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/bittorrent.py` & `rucio-34.4.0/lib/rucio/rse/protocols/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/cache.py` & `rucio-34.4.0/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/dummy.py` & `rucio-34.4.0/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/gfal.py` & `rucio-34.4.0/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/globus.py` & `rucio-34.4.0/lib/rucio/rse/protocols/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/gsiftp.py` & `rucio-34.4.0/lib/rucio/rse/protocols/gsiftp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/http_cache.py` & `rucio-34.4.0/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/mock.py` & `rucio-34.4.0/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/ngarc.py` & `rucio-34.4.0/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/posix.py` & `rucio-34.4.0/lib/rucio/rse/protocols/posix.py`

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

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/protocol.py` & `rucio-34.4.0/lib/rucio/rse/protocols/protocol.py`

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

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/rclone.py` & `rucio-34.4.0/lib/rucio/rse/protocols/rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/rfio.py` & `rucio-34.4.0/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/srm.py` & `rucio-34.4.0/lib/rucio/rse/protocols/srm.py`

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

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/ssh.py` & `rucio-34.4.0/lib/rucio/rse/protocols/ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/storm.py` & `rucio-34.4.0/lib/rucio/rse/protocols/storm.py`

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

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/webdav.py` & `rucio-34.4.0/lib/rucio/rse/protocols/webdav.py`

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

### Comparing `rucio-34.3.0/lib/rucio/rse/protocols/xrootd.py` & `rucio-34.4.0/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/rse/rsemanager.py` & `rucio-34.4.0/lib/rucio/rse/rsemanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/tests/__init__.py` & `rucio-34.4.0/lib/rucio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/tests/common.py` & `rucio-34.4.0/lib/rucio/tests/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/tests/common_server.py` & `rucio-34.4.0/lib/rucio/tests/common_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/__init__.py` & `rucio-34.4.0/lib/rucio/transfertool/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/bittorrent.py` & `rucio-34.4.0/lib/rucio/transfertool/bittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver.py` & `rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py` & `rucio-34.4.0/lib/rucio/transfertool/bittorrent_driver_qbittorrent.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/fts3.py` & `rucio-34.4.0/lib/rucio/transfertool/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/fts3_plugins.py` & `rucio-34.4.0/lib/rucio/transfertool/fts3_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/globus.py` & `rucio-34.4.0/lib/rucio/transfertool/globus.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/globus_library.py` & `rucio-34.4.0/lib/rucio/transfertool/globus_library.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/mock.py` & `rucio-34.4.0/lib/rucio/transfertool/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/transfertool/transfertool.py` & `rucio-34.4.0/lib/rucio/transfertool/transfertool.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/version.py` & `rucio-34.4.0/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/__init__.py` & `rucio-34.4.0/lib/rucio/web/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/__init__.py` & `rucio-34.4.0/lib/rucio/web/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/__init__.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/authenticated_bp.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/__init__.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accountlimits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/accounts.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/accounts.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/archives.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/archives.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/auth.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/auth.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/common.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/common.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/config.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/credentials.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/credentials.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dids.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dids.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/dirac.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/dirac.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/export.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/identities.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/identities.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/import.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/lifetime_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/locks.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/locks.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/main.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/metrics.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/nongrid_traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/ping.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/redirect.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/replicas.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/requests.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/requests.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rses.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rses.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/rules.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/rules.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/scopes.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/scopes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_crash.html`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/templates/auth_granted.html`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/traces.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/traces.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/flaskapi/v1/vos.py` & `rucio-34.4.0/lib/rucio/web/rest/flaskapi/v1/vos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/main.py` & `rucio-34.4.0/lib/rucio/web/rest/main.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/metrics.py` & `rucio-34.4.0/lib/rucio/web/rest/metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio/web/rest/ping.py` & `rucio-34.4.0/lib/rucio/web/rest/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/lib/rucio.egg-info/SOURCES.txt` & `rucio-34.4.0/lib/rucio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,21 +134,19 @@
 lib/rucio/common/dumper/__init__.py
 lib/rucio/common/dumper/consistency.py
 lib/rucio/common/dumper/data_models.py
 lib/rucio/common/dumper/path_parsing.py
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
 lib/rucio/core/__init__.py
 lib/rucio/core/account.py
 lib/rucio/core/account_counter.py
 lib/rucio/core/account_limit.py
 lib/rucio/core/authentication.py
 lib/rucio/core/config.py
 lib/rucio/core/credential.py
@@ -190,15 +188,14 @@
 lib/rucio/core/did_meta_plugins/filter_engine.py
 lib/rucio/core/did_meta_plugins/json_meta.py
 lib/rucio/core/did_meta_plugins/mongo_meta.py
 lib/rucio/core/did_meta_plugins/postgres_meta.py
 lib/rucio/core/permission/__init__.py
 lib/rucio/core/permission/atlas.py
 lib/rucio/core/permission/belleii.py
-lib/rucio/core/permission/cms.py
 lib/rucio/core/permission/escape.py
 lib/rucio/core/permission/generic.py
 lib/rucio/core/permission/generic_multi_vo.py
 lib/rucio/daemons/__init__.py
 lib/rucio/daemons/common.py
 lib/rucio/daemons/abacus/__init__.py
 lib/rucio/daemons/abacus/account.py
@@ -572,15 +569,14 @@
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

### Comparing `rucio-34.3.0/pylintrc` & `rucio-34.4.0/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/requirements.txt` & `rucio-34.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/setup.py` & `rucio-34.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/setuputil.py` & `rucio-34.4.0/setuputil.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_abacus_account.py` & `rucio-34.4.0/tests/test_abacus_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_abacus_collection_replica.py` & `rucio-34.4.0/tests/test_abacus_collection_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_abacus_rse.py` & `rucio-34.4.0/tests/test_abacus_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_account.py` & `rucio-34.4.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_account_limits.py` & `rucio-34.4.0/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_api_external_representation.py` & `rucio-34.4.0/tests/test_api_external_representation.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_archive.py` & `rucio-34.4.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_auditor.py` & `rucio-34.4.0/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_auditor_hdfs.py` & `rucio-34.4.0/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_auditor_srmdumps.py` & `rucio-34.4.0/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_authentication.py` & `rucio-34.4.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_automatix.py` & `rucio-34.4.0/tests/test_automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_bad_replica.py` & `rucio-34.4.0/tests/test_bad_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_bb8.py` & `rucio-34.4.0/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_belleii.py` & `rucio-34.4.0/tests/test_belleii.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_bin_rucio.py` & `rucio-34.4.0/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_boolean.py` & `rucio-34.4.0/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_clients.py` & `rucio-34.4.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_common_types.py` & `rucio-34.4.0/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_config.py` & `rucio-34.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_conveyor.py` & `rucio-34.4.0/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_conveyor_submitter.py` & `rucio-34.4.0/tests/test_conveyor_submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_counter.py` & `rucio-34.4.0/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_credential.py` & `rucio-34.4.0/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_curl.py` & `rucio-34.4.0/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_daemons.py` & `rucio-34.4.0/tests/test_daemons.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_dataset_replicas.py` & `rucio-34.4.0/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_db.py` & `rucio-34.4.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_did.py` & `rucio-34.4.0/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_did_meta_plugins.py` & `rucio-34.4.0/tests/test_did_meta_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_didtype.py` & `rucio-34.4.0/tests/test_didtype.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_download.py` & `rucio-34.4.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_dumper.py` & `rucio-34.4.0/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_dumper_consistency.py` & `rucio-34.4.0/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_dumper_data_model.py` & `rucio-34.4.0/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_dumper_path_parsing.py` & `rucio-34.4.0/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_filter_engine.py` & `rucio-34.4.0/tests/test_filter_engine.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_heartbeat.py` & `rucio-34.4.0/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_hermes.py` & `rucio-34.4.0/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_identity.py` & `rucio-34.4.0/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_impl_upload_download.py` & `rucio-34.4.0/tests/test_impl_upload_download.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_import_export.py` & `rucio-34.4.0/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_judge_cleaner.py` & `rucio-34.4.0/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_judge_evaluator.py` & `rucio-34.4.0/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_judge_injector.py` & `rucio-34.4.0/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_judge_repairer.py` & `rucio-34.4.0/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_lifetime.py` & `rucio-34.4.0/tests/test_lifetime.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_message.py` & `rucio-34.4.0/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_meta_conventions.py` & `rucio-34.4.0/tests/test_meta_conventions.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_meta_did.py` & `rucio-34.4.0/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_module_import.py` & `rucio-34.4.0/tests/test_module_import.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_monitor.py` & `rucio-34.4.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_multi_vo.py` & `rucio-34.4.0/tests/test_multi_vo.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_naming_convention.py` & `rucio-34.4.0/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_oauthmanager.py` & `rucio-34.4.0/tests/test_oauthmanager.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_oidc.py` & `rucio-34.4.0/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_permission.py` & `rucio-34.4.0/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_pfns.py` & `rucio-34.4.0/tests/test_pfns.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_ping.py` & `rucio-34.4.0/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_preparer.py` & `rucio-34.4.0/tests/test_preparer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_qos.py` & `rucio-34.4.0/tests/test_qos.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_quarantined_replica.py` & `rucio-34.4.0/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_reaper.py` & `rucio-34.4.0/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_redirect.py` & `rucio-34.4.0/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_replica.py` & `rucio-34.4.0/tests/test_replica.py`

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

### Comparing `rucio-34.3.0/tests/test_replica_recoverer.py` & `rucio-34.4.0/tests/test_replica_recoverer.py`

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

### Comparing `rucio-34.3.0/tests/test_replica_sorting.py` & `rucio-34.4.0/tests/test_replica_sorting.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_request.py` & `rucio-34.4.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_root_proxy.py` & `rucio-34.4.0/tests/test_root_proxy.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse.py` & `rucio-34.4.0/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_expression_parser.py` & `rucio-34.4.0/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_lfn2path.py` & `rucio-34.4.0/tests/test_rse_lfn2path.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_gfal2.py` & `rucio-34.4.0/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_gfal2_impl.py` & `rucio-34.4.0/tests/test_rse_protocol_gfal2_impl.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_posix.py` & `rucio-34.4.0/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_rclone.py` & `rucio-34.4.0/tests/test_rse_protocol_rclone.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_rsync.py` & `rucio-34.4.0/tests/test_rse_protocol_rsync.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_srm.py` & `rucio-34.4.0/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_ssh.py` & `rucio-34.4.0/tests/test_rse_protocol_ssh.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_webdav.py` & `rucio-34.4.0/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_protocol_xrootd.py` & `rucio-34.4.0/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rse_selector.py` & `rucio-34.4.0/tests/test_rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rucio_server.py` & `rucio-34.4.0/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_rule.py` & `rucio-34.4.0/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_scope.py` & `rucio-34.4.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_subscription.py` & `rucio-34.4.0/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_throttler.py` & `rucio-34.4.0/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_tpc.py` & `rucio-34.4.0/tests/test_tpc.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_trace.py` & `rucio-34.4.0/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_transfer.py` & `rucio-34.4.0/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_transfer_plugins.py` & `rucio-34.4.0/tests/test_transfer_plugins.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_undertaker.py` & `rucio-34.4.0/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_upload.py` & `rucio-34.4.0/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tests/test_utils.py` & `rucio-34.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tools/bootstrap.py` & `rucio-34.4.0/tools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tools/merge_rucio_configs.py` & `rucio-34.4.0/tools/merge_rucio_configs.py`

 * *Files identical despite different names*

### Comparing `rucio-34.3.0/tools/reset_database.py` & `rucio-34.4.0/tools/reset_database.py`

 * *Files identical despite different names*

