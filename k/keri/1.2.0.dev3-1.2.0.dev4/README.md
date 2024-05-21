# Comparing `tmp/keri-1.2.0.dev3.tar.gz` & `tmp/keri-1.2.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keri-1.2.0.dev3.tar", last modified: Sat May 18 21:02:18 2024, max compression
+gzip compressed data, was "keri-1.2.0.dev4.tar", last modified: Tue May 21 19:25:07 2024, max compression
```

## Comparing `keri-1.2.0.dev3.tar` & `keri-1.2.0.dev4.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.691207 keri-1.2.0.dev3/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-18 21:02:18.690889 keri-1.2.0.dev3/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-05-18 21:02:18.691253 keri-1.2.0.dev3/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-05-18 21:00:07.000000 keri-1.2.0.dev3/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.654579 keri-1.2.0.dev3/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.657395 keri-1.2.0.dev3/src/keri/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-05-18 21:00:08.000000 keri-1.2.0.dev3/src/keri/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.664834 keri-1.2.0.dev3/src/keri/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/apping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/challenging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.666496 keri-1.2.0.dev3/src/keri/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.671115 keri-1.2.0.dev3/src/keri/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.671864 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/respond.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/clean.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.672145 keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/decrypt.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.672577 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9099 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/confirm.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/request.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.672801 keri-1.2.0.dev3/src/keri/app/cli/commands/did/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/did/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/did/generate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.673325 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/add.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ends/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/escrow.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7158 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/init.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/interact.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.674814 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/admit.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      531 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/agree.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      472 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/apply.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/grant.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10073 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/offer.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/spurn.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/kevers.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.675074 keri-1.2.0.dev3/src/keri/app/cli/commands/local/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/local/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/local/watch.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.675492 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/debug.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/update.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.675984 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/run.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/show.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/migrate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.677576 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/continue.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/interact.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    31512 2024-05-18 15:25:02.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/notice.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10166 2024-05-18 15:25:02.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/shell.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      442 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/nonce.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.678186 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/clean.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/resolve.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.678847 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/remove.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/set.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/query.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/rename.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/rollback.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/saidify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/salt.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/sign.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.679058 keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/time.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.679783 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/create.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.680321 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/vc/revoke.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/version.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.680587 keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4507 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/add.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.681283 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4187 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/authenticate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/commands/witness/submit.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.682549 keri-1.2.0.dev3/src/keri/app/cli/common/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/config.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/common/displaying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/cli/common/existing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/cli/common/incepting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/rotating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/cli/common/terming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-04-22 16:39:31.000000 keri-1.2.0.dev3/src/keri/app/cli/kli.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/configing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/connecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10593 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/directing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/forwarding.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26489 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   124689 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/habbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    41828 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26860 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/app/oobiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/querying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/signaling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev3/src/keri/app/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/app/storing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.684687 keri-1.2.0.dev3/src/keri/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      468 2024-05-08 02:11:51.000000 keri-1.2.0.dev3/src/keri/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   201749 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/coring.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    38577 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/counting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   304791 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/core/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34501 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/indexing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    58336 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/core/parsing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/routing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/core/scheming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/serdering.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    33908 2024-05-08 02:11:51.000000 keri-1.2.0.dev3/src/keri/core/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    15364 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/streaming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    25641 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/core/structing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.685954 keri-1.2.0.dev3/src/keri/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   127640 2024-05-18 20:59:33.000000 keri-1.2.0.dev3/src/keri/db/basing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/dbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9246 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/escrowing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/db/koming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.686219 keri-1.2.0.dev3/src/keri/db/migrations/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/migrations/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/migrations/rekey_habs.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/db/subing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.687187 keri-1.2.0.dev3/src/keri/demo/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/demo/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/demo/demo_bob.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/demo/demo_eve.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/demo/demo_kev.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/demo/demo_sam.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/demo/demoing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.687785 keri-1.2.0.dev3/src/keri/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    25038 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/end/ending.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/end/priming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.688029 keri-1.2.0.dev3/src/keri/help/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/help/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12484 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/help/helping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    27254 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/kering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.688340 keri-1.2.0.dev3/src/keri/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-05-18 15:25:13.000000 keri-1.2.0.dev3/src/keri/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.689229 keri-1.2.0.dev3/src/keri/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev3/src/keri/vc/protocoling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vc/proving.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev3/src/keri/vc/walleting.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.690143 keri-1.2.0.dev3/src/keri/vdr/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev3/src/keri/vdr/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    84698 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/verifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/src/keri/vdr/viring.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.690509 keri-1.2.0.dev3/src/keri.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6046 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev3/src/keri.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-05-18 21:02:18.000000 keri-1.2.0.dev3/src/keri.egg-info/top_level.txt
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-18 21:02:18.690319 keri-1.2.0.dev3/tests/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-05-06 20:55:04.000000 keri-1.2.0.dev3/tests/test_kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.538574 keri-1.2.0.dev4/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-21 19:25:07.538247 keri-1.2.0.dev4/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2457 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-05-21 19:25:07.538633 keri-1.2.0.dev4/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4061 2024-05-21 19:24:42.000000 keri-1.2.0.dev4/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.503527 keri-1.2.0.dev4/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.506836 keri-1.2.0.dev4/src/keri/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       83 2024-05-21 19:24:42.000000 keri-1.2.0.dev4/src/keri/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.512403 keri-1.2.0.dev4/src/keri/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    37921 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/apping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/challenging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.512807 keri-1.2.0.dev4/src/keri/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.517084 keri-1.2.0.dev4/src/keri/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.517824 keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/respond.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1847 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/clean.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.518132 keri-1.2.0.dev4/src/keri/app/cli/commands/contacts/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/contacts/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2662 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/contacts/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2074 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/decrypt.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.518500 keri-1.2.0.dev4/src/keri/app/cli/commands/delegate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/delegate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8975 2024-05-21 19:23:55.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/delegate/confirm.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4076 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/delegate/request.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.518752 keri-1.2.0.dev4/src/keri/app/cli/commands/did/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/did/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/did/generate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.519250 keri-1.2.0.dev4/src/keri/app/cli/commands/ends/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ends/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ends/add.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ends/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ends/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/escrow.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3744 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7158 2024-05-18 20:59:33.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5479 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/init.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4897 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/interact.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.520805 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/admit.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      531 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/agree.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      472 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/apply.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/grant.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10073 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      566 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/offer.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/spurn.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/kevers.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.521068 keri-1.2.0.dev4/src/keri/app/cli/commands/local/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/local/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/local/watch.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.521505 keri-1.2.0.dev4/src/keri/app/cli/commands/mailbox/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/mailbox/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/mailbox/debug.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/mailbox/update.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.522051 keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1938 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1785 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/run.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1806 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/show.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6153 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/migrate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.524173 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3045 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/continue.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6698 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/interact.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    31512 2024-05-18 15:25:02.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/notice.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10166 2024-05-18 15:25:02.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/shell.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4891 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      442 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/nonce.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.524949 keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/clean.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-05-18 15:25:13.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/resolve.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.525654 keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/remove.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2549 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/set.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/query.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2161 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/rename.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/rollback.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8964 2024-05-18 20:59:33.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/saidify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      519 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/salt.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/sign.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.526006 keri-1.2.0.dev4/src/keri/app/cli/commands/ssh/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ssh/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/ssh/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-04-05 21:44:00.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/time.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.526970 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10874 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/create.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.527584 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/vc/revoke.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2940 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1251 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/version.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.527870 keri-1.2.0.dev4/src/keri/app/cli/commands/watcher/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/watcher/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4507 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/watcher/add.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.528673 keri-1.2.0.dev4/src/keri/app/cli/commands/witness/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/witness/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4187 2024-05-18 15:25:13.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/witness/authenticate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3047 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/witness/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4836 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/witness/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4655 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/commands/witness/submit.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.529826 keri-1.2.0.dev4/src/keri/app/cli/common/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/common/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/common/config.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3887 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/common/displaying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3357 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/cli/common/existing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/cli/common/incepting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/common/rotating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/cli/common/terming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-04-22 16:39:31.000000 keri-1.2.0.dev4/src/keri/app/cli/kli.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8151 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/configing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/connecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10593 2024-05-18 20:59:33.000000 keri-1.2.0.dev4/src/keri/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24676 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/directing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18769 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/forwarding.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26489 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   124689 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/habbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8702 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    41828 2024-05-18 15:25:13.000000 keri-1.2.0.dev4/src/keri/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    73656 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26860 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/app/oobiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/querying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/signaling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-04-05 21:44:00.000000 keri-1.2.0.dev4/src/keri/app/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/app/storing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.532538 keri-1.2.0.dev4/src/keri/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      468 2024-05-08 02:11:51.000000 keri-1.2.0.dev4/src/keri/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   201749 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/coring.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    38577 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/counting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   310736 2024-05-21 19:23:55.000000 keri-1.2.0.dev4/src/keri/core/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34501 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/indexing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    58336 2024-05-18 20:59:33.000000 keri-1.2.0.dev4/src/keri/core/parsing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26820 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/routing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/core/scheming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    82877 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/serdering.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    33908 2024-05-08 02:11:51.000000 keri-1.2.0.dev4/src/keri/core/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    15364 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/streaming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25641 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/core/structing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.533478 keri-1.2.0.dev4/src/keri/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   127640 2024-05-18 20:59:33.000000 keri-1.2.0.dev4/src/keri/db/basing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    77257 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/db/dbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9246 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/db/escrowing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/db/koming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.533697 keri-1.2.0.dev4/src/keri/db/migrations/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/db/migrations/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2861 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/db/migrations/rekey_habs.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    59458 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/db/subing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.534807 keri-1.2.0.dev4/src/keri/demo/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/demo/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2790 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/demo/demo_bob.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2806 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/demo/demo_eve.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/demo/demo_kev.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2831 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/demo/demo_sam.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/demo/demoing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.535329 keri-1.2.0.dev4/src/keri/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    25038 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/end/ending.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/end/priming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.535580 keri-1.2.0.dev4/src/keri/help/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      619 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/help/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12484 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/help/helping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    27254 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.535798 keri-1.2.0.dev4/src/keri/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    19698 2024-05-18 15:25:13.000000 keri-1.2.0.dev4/src/keri/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.536414 keri-1.2.0.dev4/src/keri/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-04-05 21:44:00.000000 keri-1.2.0.dev4/src/keri/vc/protocoling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2528 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/vc/proving.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.2.0.dev4/src/keri/vc/walleting.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.537212 keri-1.2.0.dev4/src/keri/vdr/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.2.0.dev4/src/keri/vdr/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34327 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/vdr/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    84698 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/vdr/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14424 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/vdr/verifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35856 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/src/keri/vdr/viring.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.537802 keri-1.2.0.dev4/src/keri.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1594 2024-05-21 19:25:07.000000 keri-1.2.0.dev4/src/keri.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6046 2024-05-21 19:25:07.000000 keri-1.2.0.dev4/src/keri.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-05-21 19:25:07.000000 keri-1.2.0.dev4/src/keri.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-05-21 19:25:07.000000 keri-1.2.0.dev4/src/keri.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.2.0.dev4/src/keri.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      314 2024-05-21 19:25:07.000000 keri-1.2.0.dev4/src/keri.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-05-21 19:25:07.000000 keri-1.2.0.dev4/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-05-21 19:25:07.537350 keri-1.2.0.dev4/tests/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    28418 2024-05-06 20:55:04.000000 keri-1.2.0.dev4/tests/test_kering.py
```

### Comparing `keri-1.2.0.dev3/LICENSE` & `keri-1.2.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/PKG-INFO` & `keri-1.2.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev3
+Version: 1.2.0.dev4
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.2.0.dev3/README.md` & `keri-1.2.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/setup.py` & `keri-1.2.0.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from glob import glob
 from os.path import basename
 from os.path import splitext
 
 from setuptools import find_packages, setup
 setup(
     name='keri',
-    version='1.2.0-dev3',  # also change in src/keri/__init__.py
+    version='1.2.0-dev4',  # also change in src/keri/__init__.py
     license='Apache Software License 2.0',
     description='Key Event Receipt Infrastructure',
     long_description="KERI Decentralized Key Management Infrastructure",
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
     url='https://github.com/WebOfTrust/keripy',
     packages=find_packages('src'),
```

### Comparing `keri-1.2.0.dev3/src/keri/app/agenting.py` & `keri-1.2.0.dev4/src/keri/app/agenting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/apping.py` & `keri-1.2.0.dev4/src/keri/app/apping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/challenging.py` & `keri-1.2.0.dev4/src/keri/app/challenging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/generate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/respond.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/respond.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/challenge/verify.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/challenge/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/clean.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/contacts/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/contacts/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/decrypt.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/decrypt.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/confirm.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/delegate/confirm.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                         approve = yn in ('', 'y', 'Y')
 
                     if not approve:
                         continue
 
                     if isinstance(hab, GroupHab):
                         aids = hab.smids
-                        #seqner = coring.Seqner(sn=eserder.sn)
+
                         anchor = dict(i=eserder.ked["i"], s=eserder.snh, d=eserder.said)
                         if self.interact:
                             msg = hab.interact(data=[anchor])
                         else:
                             print("Confirm does not support rotation for delegation approval with group multisig")
                             continue
 
@@ -162,15 +162,15 @@
                         print(f"Delegate {eserder.pre} {typ} event committed.")
 
                         self.remove(self.toRemove)
                         return True
 
                     else:
                         cur = hab.kever.sner.num
-                        #seqner = coring.Seqner(sn=eserder.sn)
+
                         anchor = dict(i=eserder.ked["i"], s=eserder.snh, d=eserder.said)
                         if self.interact:
                             hab.interact(data=[anchor])
                         else:
                             hab.rotate(data=[anchor])
 
                         witDoer = agenting.WitnessReceiptor(hby=self.hby)
```

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/delegate/request.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/delegate/request.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/did/generate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/did/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ends/add.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ends/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ends/export.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ends/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ends/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ends/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/escrow.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/escrow.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/export.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/incept.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/init.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/interact.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/admit.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/admit.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/agree.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/agree.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/grant.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/grant.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/join.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/offer.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/offer.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ipex/spurn.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ipex/spurn.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/kevers.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/kevers.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/local/watch.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/local/watch.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/debug.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/mailbox/debug.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/mailbox/update.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/mailbox/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/run.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/run.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate/show.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/migrate/show.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/migrate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/continue.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/continue.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/demo.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/incept.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/interact.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/join.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/notice.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/notice.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/rotate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/rotate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/shell.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/shell.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/multisig/update.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/multisig/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/clean.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/generate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/oobi/resolve.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/oobi/resolve.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/generate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/remove.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/remove.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/passcode/set.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/passcode/set.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/query.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/rename.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/rename.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/rollback.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/rollback.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/rotate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/rotate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/saidify.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/saidify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/salt.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/salt.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/sign.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/sign.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/ssh/export.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/ssh/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/status.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/create.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/create.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/export.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/incept.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/list.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/registry/status.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/registry/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/vc/revoke.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/vc/revoke.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/verify.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/version.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/watcher/add.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/watcher/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/authenticate.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/witness/authenticate.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/demo.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/witness/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/start.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/witness/start.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/commands/witness/submit.py` & `keri-1.2.0.dev4/src/keri/app/cli/commands/witness/submit.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/common/config.py` & `keri-1.2.0.dev4/src/keri/app/cli/common/config.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/common/displaying.py` & `keri-1.2.0.dev4/src/keri/app/cli/common/displaying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/common/existing.py` & `keri-1.2.0.dev4/src/keri/app/cli/common/existing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/common/incepting.py` & `keri-1.2.0.dev4/src/keri/app/cli/common/incepting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/common/rotating.py` & `keri-1.2.0.dev4/src/keri/app/cli/common/rotating.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/cli/kli.py` & `keri-1.2.0.dev4/src/keri/app/cli/kli.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/configing.py` & `keri-1.2.0.dev4/src/keri/app/configing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/connecting.py` & `keri-1.2.0.dev4/src/keri/app/connecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/delegating.py` & `keri-1.2.0.dev4/src/keri/app/delegating.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/directing.py` & `keri-1.2.0.dev4/src/keri/app/directing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/forwarding.py` & `keri-1.2.0.dev4/src/keri/app/forwarding.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/grouping.py` & `keri-1.2.0.dev4/src/keri/app/grouping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/habbing.py` & `keri-1.2.0.dev4/src/keri/app/habbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/httping.py` & `keri-1.2.0.dev4/src/keri/app/httping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/indirecting.py` & `keri-1.2.0.dev4/src/keri/app/indirecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/keeping.py` & `keri-1.2.0.dev4/src/keri/app/keeping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/notifying.py` & `keri-1.2.0.dev4/src/keri/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/oobiing.py` & `keri-1.2.0.dev4/src/keri/app/oobiing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/querying.py` & `keri-1.2.0.dev4/src/keri/app/querying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/signaling.py` & `keri-1.2.0.dev4/src/keri/app/signaling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/signing.py` & `keri-1.2.0.dev4/src/keri/app/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/specing.py` & `keri-1.2.0.dev4/src/keri/app/specing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/app/storing.py` & `keri-1.2.0.dev4/src/keri/app/storing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/coring.py` & `keri-1.2.0.dev4/src/keri/core/coring.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/counting.py` & `keri-1.2.0.dev4/src/keri/core/counting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/eventing.py` & `keri-1.2.0.dev4/src/keri/core/eventing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5710,14 +5710,132 @@
                     logger.info("Kevery unescrow succeeded for event pre=%s "
                                 "sn=%s", pre, sn)
 
             if ekey == key:  # still same so no escrows found on last while iteration
                 break
             key = ekey  # setup next while iteration, with key after ekey
 
+    def processEscrowDelegables(self):
+        """
+        Process events escrowed by Kever that require delegation.
+
+        Escrowed items are indexed in database table keyed by prefix and
+        sn with duplicates given by different dig inserted in insertion order.
+        This allows FIFO processing of events with same prefix and sn but different
+        digest.
+
+        Uses  .db.delegables.add(key, val) which is IOVal with dups.
+
+        Value is dgkey for event stored in .Evt where .Evt has serder.raw of event.
+
+        Steps:
+            Each pass  (walk index table)
+                For each prefix,sn
+                    For each escrow item dup at prefix,sn:
+                        Get Event
+                        Get and Attach Signatures
+                        Process event as if it came in over the wire
+                        If successful then remove from escrow table
+        """
+
+        for (pre, sn), dig in self.db.delegables.getItemIter():
+            try:
+                edig = dig.encode("utf-8")
+                dgkey = dgKey(pre.encode("utf-8"), edig)
+                if not (esr := self.db.esrs.get(keys=dgkey)):  # get event source, otherwise error
+                    # no local sourde so raise ValidationError which unescrows below
+                    raise ValidationError("Missing escrowed event source "
+                                          "at dig = {}.".format(bytes(edig)))
+
+                # check date if expired then remove escrow.
+                dtb = self.db.getDts(dgkey)
+                if dtb is None:  # othewise is a datetime as bytes
+                    # no date time so raise ValidationError which unescrows below
+                    logger.info("Kevery unescrow error: Missing event datetime"
+                                " at dig = %s", bytes(edig))
+
+                    raise ValidationError("Missing escrowed event datetime "
+                                          "at dig = {}.".format(bytes(edig)))
+
+                # do date math here and discard if stale nowIso8601() bytes
+                dtnow = helping.nowUTC()
+                dte = helping.fromIso8601(bytes(dtb))
+                if (dtnow - dte) > datetime.timedelta(seconds=self.TimeoutOOE):
+                    # escrow stale so raise ValidationError which unescrows below
+                    logger.info("Kevery unescrow error: Stale event escrow "
+                                " at dig = %s", bytes(edig))
+
+                    raise ValidationError("Stale event escrow "
+                                          "at dig = {}.".format(bytes(edig)))
+
+                # get the escrowed event using edig
+                eraw = self.db.getEvt(dgKey(pre, bytes(edig)))
+                if eraw is None:
+                    # no event so raise ValidationError which unescrows below
+                    logger.info("Kevery unescrow error: Missing event at."
+                                "dig = %s", bytes(edig))
+
+                    raise ValidationError("Missing escrowed evt at dig = {}."
+                                          "".format(bytes(edig)))
+
+                eserder = serdering.SerderKERI(raw=bytes(eraw))  # escrowed event
+
+                #  get sigs and attach
+                sigs = self.db.getSigs(dgKey(pre, bytes(edig)))
+                if not sigs:  # otherwise its a list of sigs
+                    # no sigs so raise ValidationError which unescrows below
+                    logger.info("Kevery unescrow error: Missing event sigs at."
+                                "dig = %s", bytes(edig))
+
+                    raise ValidationError("Missing escrowed evt sigs at "
+                                          "dig = {}.".format(bytes(edig)))
+
+                sigers = [Siger(qb64b=bytes(sig)) for sig in sigs]
+
+                #  get wigs
+                wigs = self.db.getWigs(dgKey(pre, bytes(edig)))  # list of wigs
+                wigers = [Siger(qb64b=bytes(wig)) for wig in wigs]
+
+                # get delgate seal
+                couple = self.db.getAes(dgkey)
+                if couple is not None:  # Only try to parse the event if we have the del seal
+                    raw = bytearray(couple)
+                    seqner = coring.Seqner(qb64b=raw, strip=True)
+                    saider = coring.Saider(qb64b=raw)
+
+                    # process event
+                    self.processEvent(serder=eserder, sigers=sigers, wigers=wigers, delseqner=seqner,
+                                      delsaider=saider, local=esr.local)
+                else:
+                    raise MissingDelegableApprovalError()
+
+            except MissingDelegableApprovalError as ex:
+                # still waiting on missing delegation approval
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Kevery unescrow failed: %s", ex.args[0])
+                else:
+                    logger.error("Kevery unescrow failed: %s", ex.args[0])
+
+            except Exception as ex:  # log diagnostics errors etc
+                # error other than out of order so remove from OO escrow
+                self.db.delegables.rem(keys=(pre, sn,), val=edig)  # removes one escrow at key val
+                if logger.isEnabledFor(logging.DEBUG):
+                    logger.exception("Kevery unescrowed: %s", ex.args[0])
+                else:
+                    logger.error("Kevery unescrowed: %s", ex.args[0])
+
+            else:  # unescrow succeeded, remove from escrow
+                # We don't remove all escrows at pre,sn because some might be
+                # duplicitous so we process remaining escrows in spite of found
+                # valid event escrow.
+                self.db.delegables.rem(keys=(pre, sn,), val=edig)  # removes one escrow at key val
+                logger.info("Kevery unescrow succeeded in valid event: "
+                            "event=%s", eserder.said)
+                logger.debug(f"event=\n{eserder.pretty()}\n")
+
     def processQueryNotFound(self):
         """
         Process qry events escrowed by Kevery for KELs that have not yet met the criteria of the query.
         A missing KEL or criteria for an event in a KEL at a particular sequence number or an event containing a
         specific anchor can result in query not found escrowed events.
 
         Escrowed items are indexed in database table keyed by prefix and
```

### Comparing `keri-1.2.0.dev3/src/keri/core/indexing.py` & `keri-1.2.0.dev4/src/keri/core/indexing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/parsing.py` & `keri-1.2.0.dev4/src/keri/core/parsing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/routing.py` & `keri-1.2.0.dev4/src/keri/core/routing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/scheming.py` & `keri-1.2.0.dev4/src/keri/core/scheming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/serdering.py` & `keri-1.2.0.dev4/src/keri/core/serdering.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/signing.py` & `keri-1.2.0.dev4/src/keri/core/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/streaming.py` & `keri-1.2.0.dev4/src/keri/core/streaming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/core/structing.py` & `keri-1.2.0.dev4/src/keri/core/structing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/db/basing.py` & `keri-1.2.0.dev4/src/keri/db/basing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/db/dbing.py` & `keri-1.2.0.dev4/src/keri/db/dbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/db/escrowing.py` & `keri-1.2.0.dev4/src/keri/db/escrowing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/db/koming.py` & `keri-1.2.0.dev4/src/keri/db/koming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/db/migrations/rekey_habs.py` & `keri-1.2.0.dev4/src/keri/db/migrations/rekey_habs.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/db/subing.py` & `keri-1.2.0.dev4/src/keri/db/subing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/demo/demo_bob.py` & `keri-1.2.0.dev4/src/keri/demo/demo_bob.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/demo/demo_eve.py` & `keri-1.2.0.dev4/src/keri/demo/demo_eve.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/demo/demo_kev.py` & `keri-1.2.0.dev4/src/keri/demo/demo_kev.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/demo/demo_sam.py` & `keri-1.2.0.dev4/src/keri/demo/demo_sam.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/demo/demoing.py` & `keri-1.2.0.dev4/src/keri/demo/demoing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/end/ending.py` & `keri-1.2.0.dev4/src/keri/end/ending.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/end/priming.py` & `keri-1.2.0.dev4/src/keri/end/priming.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/help/__init__.py` & `keri-1.2.0.dev4/src/keri/help/__init__.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/help/helping.py` & `keri-1.2.0.dev4/src/keri/help/helping.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/kering.py` & `keri-1.2.0.dev4/src/keri/kering.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/peer/exchanging.py` & `keri-1.2.0.dev4/src/keri/peer/exchanging.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vc/protocoling.py` & `keri-1.2.0.dev4/src/keri/vc/protocoling.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vc/proving.py` & `keri-1.2.0.dev4/src/keri/vc/proving.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vc/walleting.py` & `keri-1.2.0.dev4/src/keri/vc/walleting.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vdr/credentialing.py` & `keri-1.2.0.dev4/src/keri/vdr/credentialing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vdr/eventing.py` & `keri-1.2.0.dev4/src/keri/vdr/eventing.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vdr/verifying.py` & `keri-1.2.0.dev4/src/keri/vdr/verifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri/vdr/viring.py` & `keri-1.2.0.dev4/src/keri/vdr/viring.py`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/src/keri.egg-info/PKG-INFO` & `keri-1.2.0.dev4/src/keri.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.2.0.dev3
+Version: 1.2.0.dev4
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.2.0.dev3/src/keri.egg-info/SOURCES.txt` & `keri-1.2.0.dev4/src/keri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keri-1.2.0.dev3/tests/test_kering.py` & `keri-1.2.0.dev4/tests/test_kering.py`

 * *Files identical despite different names*

