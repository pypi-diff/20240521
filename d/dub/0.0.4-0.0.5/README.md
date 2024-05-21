# Comparing `tmp/dub-0.0.4.tar.gz` & `tmp/dub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dub-0.0.4.tar", last modified: Thu May 16 10:30:14 2024, max compression
+gzip compressed data, was "dub-0.0.5.tar", last modified: Tue May 21 19:07:05 2024, max compression
```

## Comparing `dub-0.0.4.tar` & `dub-0.0.5.tar`

### file list

```diff
@@ -1,101 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.501723 dub-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-16 10:30:14.501723 dub-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-05-16 10:30:04.000000 dub-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:30:14.501723 dub-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 10:30:04.000000 dub-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.485723 dub-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    76999 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    91910 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    68151 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/metatags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/domainschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    50145 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/linkschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/tagschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/components/workspaceschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.493723 dub-0.0.4/src/dub/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/badrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/forbidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/internalservererror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/inviteexpired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/notfound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/ratelimitexceeded.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/unauthorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/errors/unprocessableentity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.493723 dub-0.0.4/src/dub/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.501723 dub-0.0.4/src/dub/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/adddomain.py
--rw-r--r--   0 runner    (1001) docker     (127)    49255 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/bulkcreatelinks.py
--rw-r--r--   0 runner    (1001) docker     (127)    49337 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/createlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/createtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/createworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/deletedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/deletelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getbrowsersbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getbrowsersbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcitiesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcitiesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getclickscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getclickscountdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    13007 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcountriesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getcountriesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getdevicesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getdevicesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getlinkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getlinkscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getmetatags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getosbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getosbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getqrcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getreferersbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getreferersbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettimeseriesbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettimeseriesbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettoplinksbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettoplinksbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettopurlsbyclicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/gettopurlsbyclicksdeprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/getworkspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/listdomains.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/setprimarydomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/transferdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/updatedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)    49829 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/updatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    49358 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/models/operations/upsertlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/qr_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.501723 dub-0.0.4/src/dub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-05-16 10:30:04.000000 dub-0.0.4/src/dub/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:30:14.489723 dub-0.0.4/src/dub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17397 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 10:30:14.000000 dub-0.0.4/src/dub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.686021 dub-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    17862 2024-05-21 19:07:05.686021 dub-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-21 19:06:57.000000 dub-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:07:05.686021 dub-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-21 19:06:57.000000 dub-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.666021 dub-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.670021 dub-0.0.5/src/dub/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76952 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91883 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68151 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/metatags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/clicksbycities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/clicksbycountry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/countrycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/domainschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/linkgeotargeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50145 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/linkschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/tagschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/components/workspaceschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.678021 dub-0.0.5/src/dub/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/badrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/internalservererror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/inviteexpired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/notfound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/ratelimitexceeded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/errors/unprocessableentity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.678021 dub-0.0.5/src/dub/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.682021 dub-0.0.5/src/dub/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/adddomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/bulkcreatelinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/createlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/createtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/createworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/deletedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/deletelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getbrowsersbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getbrowsersbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcitiesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcitiesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getclickscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getclickscountdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcountriesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getcountriesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getdevicesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getdevicesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getlinkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getlinkscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getmetatags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getosbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getosbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getqrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getreferersbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getreferersbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettimeseriesbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettimeseriesbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettoplinksbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettoplinksbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettopurlsbyclicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/gettopurlsbyclicksdeprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/getworkspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/listdomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/setprimarydomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/trackcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/tracklead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/tracksale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/transferdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/updatedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/updatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/models/operations/upsertlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/qr_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24875 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.686021 dub-0.0.5/src/dub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24355 2024-05-21 19:06:57.000000 dub-0.0.5/src/dub/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:07:05.674021 dub-0.0.5/src/dub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17862 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 19:07:05.000000 dub-0.0.5/src/dub.egg-info/top_level.txt
```

### Comparing `dub-0.0.4/PKG-INFO` & `dub-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # dub
         
         <div align="left">
@@ -145,14 +145,20 @@
         * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#list) - Retrieve a list of domains
         * [add](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add a domain
         * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#delete) - Delete a domain
         * [update](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a domain
         * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#set_primary) - Set a domain as primary
         * [transfer](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#transfer) - Transfer a domain
         
+        ### [track](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md)
+        
+        * [lead](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md#lead) - Track a lead
+        * [sale](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md#sale) - Track a sale
+        * [customer](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md#customer) - Track a customer
+        
         ### [metatags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md)
         
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md#get) - Retrieve the metatags for a URL
         <!-- End Available Resources and Operations [operations] -->
         
         <!-- Start Error Handling [errors] -->
         ## Error Handling
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.4 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.5 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy License: UNKNOWN Description: # dub
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
 based on your OpenAPI spec. However, it is not yet ready for production use.
@@ -100,30 +100,35 @@
 github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add
 a domain * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
 domains/README.md#delete) - Delete a domain * [update](https://github.com/
 dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a
 domain * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/
 sdks/domains/README.md#set_primary) - Set a domain as primary * [transfer]
 (https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
-README.md#transfer) - Transfer a domain ### [metatags](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/metatags/README.md) * [get](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md#get) -
-Retrieve the metatags for a URL ## Error Handling Handling errors in this SDK
-should largely match your expectations. All operations return a response object
-or raise an error. If Error objects are specified in your OpenAPI Spec, the SDK
-will raise the appropriate Error type. | Error Object | Status Code | Content
-Type | | -------------------------- | -------------------------- | ------------
--------------- | | errors.BadRequest | 400 | application/json | |
-errors.Unauthorized | 401 | application/json | | errors.Forbidden | 403 |
-application/json | | errors.NotFound | 404 | application/json | |
-errors.Conflict | 409 | application/json | | errors.InviteExpired | 410 |
-application/json | | errors.UnprocessableEntity | 422 | application/json | |
-errors.RateLimitExceeded | 429 | application/json | |
-errors.InternalServerError | 500 | application/json | | errors.SDKError | 4xx-
-5xx | */* | ### Example ```python import dub from dub.models import errors,
+README.md#transfer) - Transfer a domain ### [track](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/track/README.md) * [lead](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/track/README.md#lead) - Track a lead *
+[sale](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/
+README.md#sale) - Track a sale * [customer](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/track/README.md#customer) - Track a customer ###
+[metatags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/
+README.md) * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+metatags/README.md#get) - Retrieve the metatags for a URL ## Error Handling
+Handling errors in this SDK should largely match your expectations. All
+operations return a response object or raise an error. If Error objects are
+specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
+| Error Object | Status Code | Content Type | | -------------------------- | --
+------------------------ | -------------------------- | | errors.BadRequest |
+400 | application/json | | errors.Unauthorized | 401 | application/json | |
+errors.Forbidden | 403 | application/json | | errors.NotFound | 404 |
+application/json | | errors.Conflict | 409 | application/json | |
+errors.InviteExpired | 410 | application/json | | errors.UnprocessableEntity |
+422 | application/json | | errors.RateLimitExceeded | 429 | application/json |
+| errors.InternalServerError | 500 | application/json | | errors.SDKError |
+4xx-5xx | */* | ### Example ```python import dub from dub.models import errors,
 operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res = None try:
 res = s.links.list(request=operations.GetLinksRequest()) except
 errors.BadRequest as e: # handle exception raise(e) except errors.Unauthorized
 as e: # handle exception raise(e) except errors.Forbidden as e: # handle
 exception raise(e) except errors.NotFound as e: # handle exception raise(e)
 except errors.Conflict as e: # handle exception raise(e) except
 errors.InviteExpired as e: # handle exception raise(e) except
```

### Comparing `dub-0.0.4/README.md` & `dub-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,20 @@
 * [list](docs/sdks/domains/README.md#list) - Retrieve a list of domains
 * [add](docs/sdks/domains/README.md#add) - Add a domain
 * [delete](docs/sdks/domains/README.md#delete) - Delete a domain
 * [update](docs/sdks/domains/README.md#update) - Update a domain
 * [set_primary](docs/sdks/domains/README.md#set_primary) - Set a domain as primary
 * [transfer](docs/sdks/domains/README.md#transfer) - Transfer a domain
 
+### [track](docs/sdks/track/README.md)
+
+* [lead](docs/sdks/track/README.md#lead) - Track a lead
+* [sale](docs/sdks/track/README.md#sale) - Track a sale
+* [customer](docs/sdks/track/README.md#customer) - Track a customer
+
 ### [metatags](docs/sdks/metatags/README.md)
 
 * [get](docs/sdks/metatags/README.md#get) - Retrieve the metatags for a URL
 <!-- End Available Resources and Operations [operations] -->
 
 <!-- Start Error Handling [errors] -->
 ## Error Handling
```

#### html2text {}

```diff
@@ -68,15 +68,18 @@
 Retrieve a list of tags * [create](docs/sdks/tags/README.md#create) - Create a
 new tag ### [domains](docs/sdks/domains/README.md) * [list](docs/sdks/domains/
 README.md#list) - Retrieve a list of domains * [add](docs/sdks/domains/
 README.md#add) - Add a domain * [delete](docs/sdks/domains/README.md#delete) -
 Delete a domain * [update](docs/sdks/domains/README.md#update) - Update a
 domain * [set_primary](docs/sdks/domains/README.md#set_primary) - Set a domain
 as primary * [transfer](docs/sdks/domains/README.md#transfer) - Transfer a
-domain ### [metatags](docs/sdks/metatags/README.md) * [get](docs/sdks/metatags/
+domain ### [track](docs/sdks/track/README.md) * [lead](docs/sdks/track/
+README.md#lead) - Track a lead * [sale](docs/sdks/track/README.md#sale) - Track
+a sale * [customer](docs/sdks/track/README.md#customer) - Track a customer ###
+[metatags](docs/sdks/metatags/README.md) * [get](docs/sdks/metatags/
 README.md#get) - Retrieve the metatags for a URL ## Error Handling Handling
 errors in this SDK should largely match your expectations. All operations
 return a response object or raise an error. If Error objects are specified in
 your OpenAPI Spec, the SDK will raise the appropriate Error type. | Error
 Object | Status Code | Content Type | | -------------------------- | ----------
 ---------------- | -------------------------- | | errors.BadRequest | 400 |
 application/json | | errors.Unauthorized | 401 | application/json | |
```

### Comparing `dub-0.0.4/setup.py` & `dub-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='dub',
-    version='0.0.4',
+    version='0.0.5',
     author='Speakeasy',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/dubinc/dub-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `dub-0.0.4/src/dub/_hooks/registration.py` & `dub-0.0.5/src/dub/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/_hooks/sdkhooks.py` & `dub-0.0.5/src/dub/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/_hooks/types.py` & `dub-0.0.5/src/dub/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/analytics.py` & `dub-0.0.5/src/dub/analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,16 +207,16 @@
         
         
         res = operations.GetCountriesByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCountriesByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCountry]])
+                res.clicks_by_countries = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequest)
@@ -345,16 +345,16 @@
         
         
         res = operations.GetCitiesByClicksDeprecatedResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCitiesByClicksDeprecatedResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCities]])
+                res.clicks_by_cities = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequest)
```

### Comparing `dub-0.0.4/src/dub/clicks.py` & `dub-0.0.5/src/dub/clicks.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,16 +333,16 @@
         
         
         res = operations.GetCountriesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCountriesByClicksResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCountry]])
+                res.clicks_by_countries = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequest)
@@ -469,16 +469,16 @@
         
         
         res = operations.GetCitiesByClicksResponse(http_meta=components.HTTPMetadata(request=req, response=http_res))
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[operations.GetCitiesByClicksResponseBody]])
-                res.response_bodies = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[components.ClicksByCities]])
+                res.clicks_by_cities = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequest)
```

### Comparing `dub-0.0.4/src/dub/domains.py` & `dub-0.0.5/src/dub/domains.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/links.py` & `dub-0.0.5/src/dub/links.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/metatags.py` & `dub-0.0.5/src/dub/metatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/components/domainschema.py` & `dub-0.0.5/src/dub/models/components/domainschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,13 +29,15 @@
     r"""The type of redirect to use for this domain."""
     verified: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('verified'), 'exclude': lambda f: f is None }})
     r"""Whether the domain is verified."""
     primary: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('primary'), 'exclude': lambda f: f is None }})
     r"""Whether the domain is the primary domain for the workspace."""
     archived: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('archived'), 'exclude': lambda f: f is None }})
     r"""Whether the domain is archived."""
+    noindex: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noindex'), 'exclude': lambda f: f is None }})
+    r"""Prevent search engines from indexing the domain."""
     placeholder: Optional[str] = dataclasses.field(default='https://dub.co/help/article/what-is-dub', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('placeholder'), 'exclude': lambda f: f is None }})
     r"""Provide context to your teammates in the link creation modal by showing them an example of a link to be shortened."""
     clicks: Optional[float] = dataclasses.field(default=0, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clicks'), 'exclude': lambda f: f is None }})
     r"""The number of clicks on the domain."""
```

### Comparing `dub-0.0.4/src/dub/models/components/httpmetadata.py` & `dub-0.0.5/src/dub/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/components/linkschema.py` & `dub-0.0.5/src/dub/models/components/linkschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/components/tagschema.py` & `dub-0.0.5/src/dub/models/components/tagschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/components/workspaceschema.py` & `dub-0.0.5/src/dub/models/components/workspaceschema.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,19 +71,23 @@
     r"""The users limit of the workspace."""
     plan: Plan = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan') }})
     r"""The plan of the workspace."""
     stripe_id: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stripeId') }})
     r"""The Stripe ID of the workspace."""
     billing_cycle_start: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billingCycleStart') }})
     r"""The date and time when the billing cycle starts for the workspace."""
+    stripe_connect_id: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stripeConnectId') }})
+    r"""[BETA]: The Stripe Connect ID of the workspace."""
     created_at: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt') }})
     r"""The date and time when the workspace was created."""
     users: List[Users] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users') }})
     r"""The role of the authenticated user in the workspace."""
     domains: List[Domains] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domains') }})
     r"""The domains of the workspace."""
     invite_code: Optional[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inviteCode') }})
     r"""The invite code of the workspace."""
     logo: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logo'), 'exclude': lambda f: f is WorkspaceSchema.UNSET }})
     r"""The logo of the workspace."""
+    beta_tester: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('betaTester'), 'exclude': lambda f: f is None }})
+    r"""Whether the workspace is enrolled in the beta testing program."""
```

### Comparing `dub-0.0.4/src/dub/models/errors/__init__.py` & `dub-0.0.5/src/dub/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/badrequest.py` & `dub-0.0.5/src/dub/models/errors/badrequest.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/conflict.py` & `dub-0.0.5/src/dub/models/errors/conflict.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/forbidden.py` & `dub-0.0.5/src/dub/models/errors/forbidden.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/internalservererror.py` & `dub-0.0.5/src/dub/models/errors/internalservererror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/inviteexpired.py` & `dub-0.0.5/src/dub/models/errors/inviteexpired.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/notfound.py` & `dub-0.0.5/src/dub/models/errors/notfound.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/ratelimitexceeded.py` & `dub-0.0.5/src/dub/models/errors/ratelimitexceeded.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/sdkerror.py` & `dub-0.0.5/src/dub/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/unauthorized.py` & `dub-0.0.5/src/dub/models/errors/unauthorized.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/errors/unprocessableentity.py` & `dub-0.0.5/src/dub/models/errors/unprocessableentity.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/internal/globals.py` & `dub-0.0.5/src/dub/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/__init__.py` & `dub-0.0.5/src/dub/models/operations/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,13 +33,16 @@
 from .gettoplinksbyclicksdeprecated import *
 from .gettopurlsbyclicks import *
 from .gettopurlsbyclicksdeprecated import *
 from .getworkspace import *
 from .getworkspaces import *
 from .listdomains import *
 from .setprimarydomain import *
+from .trackcustomer import *
+from .tracklead import *
+from .tracksale import *
 from .transferdomain import *
 from .updatedomain import *
 from .updatelink import *
 from .upsertlink import *
 
-__all__ = ["AddDomainGlobals","AddDomainRequestBody","AddDomainResponse","BulkCreateLinksGeo","BulkCreateLinksGlobals","BulkCreateLinksResponse","Color","Country","CreateLinkGlobals","CreateLinkRequestBody","CreateLinkResponse","CreateTagGlobals","CreateTagRequestBody","CreateTagResponse","CreateWorkspaceRequestBody","CreateWorkspaceResponse","DeleteDomainGlobals","DeleteDomainRequest","DeleteDomainResponse","DeleteDomainResponseBody","DeleteLinkGlobals","DeleteLinkRequest","DeleteLinkResponse","DeleteLinkResponseBody","Geo","GetBrowsersByClicksDeprecatedGlobals","GetBrowsersByClicksDeprecatedQueryParamCountry","GetBrowsersByClicksDeprecatedQueryParamInterval","GetBrowsersByClicksDeprecatedRequest","GetBrowsersByClicksDeprecatedResponse","GetBrowsersByClicksDeprecatedResponseBody","GetBrowsersByClicksGlobals","GetBrowsersByClicksQueryParamCountry","GetBrowsersByClicksQueryParamInterval","GetBrowsersByClicksRequest","GetBrowsersByClicksResponse","GetBrowsersByClicksResponseBody","GetCitiesByClicksCountry","GetCitiesByClicksDeprecatedCountry","GetCitiesByClicksDeprecatedGlobals","GetCitiesByClicksDeprecatedQueryParamCountry","GetCitiesByClicksDeprecatedQueryParamInterval","GetCitiesByClicksDeprecatedRequest","GetCitiesByClicksDeprecatedResponse","GetCitiesByClicksDeprecatedResponseBody","GetCitiesByClicksGlobals","GetCitiesByClicksQueryParamCountry","GetCitiesByClicksQueryParamInterval","GetCitiesByClicksRequest","GetCitiesByClicksResponse","GetCitiesByClicksResponseBody","GetClicksCountDeprecatedGlobals","GetClicksCountDeprecatedQueryParamCountry","GetClicksCountDeprecatedQueryParamInterval","GetClicksCountDeprecatedRequest","GetClicksCountDeprecatedResponse","GetClicksCountGlobals","GetClicksCountRequest","GetClicksCountResponse","GetCountriesByClicksCountry","GetCountriesByClicksDeprecatedCountry","GetCountriesByClicksDeprecatedGlobals","GetCountriesByClicksDeprecatedQueryParamCountry","GetCountriesByClicksDeprecatedQueryParamInterval","GetCountriesByClicksDeprecatedRequest","GetCountriesByClicksDeprecatedResponse","GetCountriesByClicksDeprecatedResponseBody","GetCountriesByClicksGlobals","GetCountriesByClicksQueryParamCountry","GetCountriesByClicksQueryParamInterval","GetCountriesByClicksRequest","GetCountriesByClicksResponse","GetCountriesByClicksResponseBody","GetDevicesByClicksDeprecatedGlobals","GetDevicesByClicksDeprecatedQueryParamCountry","GetDevicesByClicksDeprecatedQueryParamInterval","GetDevicesByClicksDeprecatedRequest","GetDevicesByClicksDeprecatedResponse","GetDevicesByClicksDeprecatedResponseBody","GetDevicesByClicksGlobals","GetDevicesByClicksQueryParamCountry","GetDevicesByClicksQueryParamInterval","GetDevicesByClicksRequest","GetDevicesByClicksResponse","GetDevicesByClicksResponseBody","GetLinkInfoGlobals","GetLinkInfoRequest","GetLinkInfoResponse","GetLinksCountGlobals","GetLinksCountRequest","GetLinksCountResponse","GetLinksGlobals","GetLinksRequest","GetLinksResponse","GetMetatagsRequest","GetMetatagsResponse","GetMetatagsResponseBody","GetOSByClicksDeprecatedGlobals","GetOSByClicksDeprecatedQueryParamCountry","GetOSByClicksDeprecatedQueryParamInterval","GetOSByClicksDeprecatedRequest","GetOSByClicksDeprecatedResponse","GetOSByClicksDeprecatedResponseBody","GetOSByClicksGlobals","GetOSByClicksQueryParamCountry","GetOSByClicksQueryParamInterval","GetOSByClicksRequest","GetOSByClicksResponse","GetOSByClicksResponseBody","GetQRCodeRequest","GetQRCodeResponse","GetReferersByClicksDeprecatedGlobals","GetReferersByClicksDeprecatedQueryParamCountry","GetReferersByClicksDeprecatedQueryParamInterval","GetReferersByClicksDeprecatedRequest","GetReferersByClicksDeprecatedResponse","GetReferersByClicksDeprecatedResponseBody","GetReferersByClicksGlobals","GetReferersByClicksQueryParamCountry","GetReferersByClicksQueryParamInterval","GetReferersByClicksRequest","GetReferersByClicksResponse","GetReferersByClicksResponseBody","GetTagsGlobals","GetTagsRequest","GetTagsResponse","GetTimeseriesByClicksDeprecatedGlobals","GetTimeseriesByClicksDeprecatedQueryParamCountry","GetTimeseriesByClicksDeprecatedQueryParamInterval","GetTimeseriesByClicksDeprecatedRequest","GetTimeseriesByClicksDeprecatedResponse","GetTimeseriesByClicksDeprecatedResponseBody","GetTimeseriesByClicksGlobals","GetTimeseriesByClicksRequest","GetTimeseriesByClicksResponse","GetTopLinksByClicksDeprecatedGlobals","GetTopLinksByClicksDeprecatedQueryParamCountry","GetTopLinksByClicksDeprecatedQueryParamInterval","GetTopLinksByClicksDeprecatedRequest","GetTopLinksByClicksDeprecatedResponse","GetTopLinksByClicksDeprecatedResponseBody","GetTopLinksByClicksGlobals","GetTopLinksByClicksQueryParamCountry","GetTopLinksByClicksQueryParamInterval","GetTopLinksByClicksRequest","GetTopLinksByClicksResponse","GetTopLinksByClicksResponseBody","GetTopURLsByClicksDeprecatedGlobals","GetTopURLsByClicksDeprecatedQueryParamCountry","GetTopURLsByClicksDeprecatedQueryParamInterval","GetTopURLsByClicksDeprecatedRequest","GetTopURLsByClicksDeprecatedResponse","GetTopURLsByClicksDeprecatedResponseBody","GetTopURLsByClicksGlobals","GetTopURLsByClicksQueryParamCountry","GetTopURLsByClicksQueryParamInterval","GetTopURLsByClicksRequest","GetTopURLsByClicksResponse","GetTopURLsByClicksResponseBody","GetWorkspaceRequest","GetWorkspaceResponse","GetWorkspacesResponse","Interval","Level","ListDomainsGlobals","ListDomainsRequest","ListDomainsResponse","One","QueryParamCountry","QueryParamInterval","RequestBody","ResponseBody","SetPrimaryDomainGlobals","SetPrimaryDomainRequest","SetPrimaryDomainResponse","Sort","TransferDomainGlobals","TransferDomainRequest","TransferDomainRequestBody","TransferDomainResponse","Two","Type","UpdateDomainGlobals","UpdateDomainRequest","UpdateDomainRequestBody","UpdateDomainResponse","UpdateDomainType","UpdateLinkGeo","UpdateLinkGlobals","UpdateLinkRequest","UpdateLinkRequestBody","UpdateLinkResponse","UpsertLinkGeo","UpsertLinkGlobals","UpsertLinkRequestBody","UpsertLinkResponse"]
+__all__ = ["AddDomainGlobals","AddDomainRequestBody","AddDomainResponse","BulkCreateLinksGlobals","BulkCreateLinksResponse","BulkCreateLinksTagIds","BulkCreateLinksTagNames","Color","CreateLinkGlobals","CreateLinkRequestBody","CreateLinkResponse","CreateTagGlobals","CreateTagRequestBody","CreateTagResponse","CreateWorkspaceRequestBody","CreateWorkspaceResponse","DeleteDomainGlobals","DeleteDomainRequest","DeleteDomainResponse","DeleteDomainResponseBody","DeleteLinkGlobals","DeleteLinkRequest","DeleteLinkResponse","DeleteLinkResponseBody","GetBrowsersByClicksDeprecatedGlobals","GetBrowsersByClicksDeprecatedQueryParamInterval","GetBrowsersByClicksDeprecatedRequest","GetBrowsersByClicksDeprecatedResponse","GetBrowsersByClicksDeprecatedResponseBody","GetBrowsersByClicksGlobals","GetBrowsersByClicksQueryParamInterval","GetBrowsersByClicksRequest","GetBrowsersByClicksResponse","GetBrowsersByClicksResponseBody","GetCitiesByClicksDeprecatedGlobals","GetCitiesByClicksDeprecatedQueryParamInterval","GetCitiesByClicksDeprecatedRequest","GetCitiesByClicksDeprecatedResponse","GetCitiesByClicksGlobals","GetCitiesByClicksQueryParamInterval","GetCitiesByClicksRequest","GetCitiesByClicksResponse","GetClicksCountDeprecatedGlobals","GetClicksCountDeprecatedQueryParamInterval","GetClicksCountDeprecatedRequest","GetClicksCountDeprecatedResponse","GetClicksCountGlobals","GetClicksCountRequest","GetClicksCountResponse","GetCountriesByClicksDeprecatedGlobals","GetCountriesByClicksDeprecatedQueryParamInterval","GetCountriesByClicksDeprecatedRequest","GetCountriesByClicksDeprecatedResponse","GetCountriesByClicksGlobals","GetCountriesByClicksQueryParamInterval","GetCountriesByClicksRequest","GetCountriesByClicksResponse","GetDevicesByClicksDeprecatedGlobals","GetDevicesByClicksDeprecatedQueryParamInterval","GetDevicesByClicksDeprecatedRequest","GetDevicesByClicksDeprecatedResponse","GetDevicesByClicksDeprecatedResponseBody","GetDevicesByClicksGlobals","GetDevicesByClicksQueryParamInterval","GetDevicesByClicksRequest","GetDevicesByClicksResponse","GetDevicesByClicksResponseBody","GetLinkInfoGlobals","GetLinkInfoRequest","GetLinkInfoResponse","GetLinksCountGlobals","GetLinksCountQueryParamTagIds","GetLinksCountQueryParamTagNames","GetLinksCountRequest","GetLinksCountResponse","GetLinksGlobals","GetLinksRequest","GetLinksResponse","GetMetatagsRequest","GetMetatagsResponse","GetMetatagsResponseBody","GetOSByClicksDeprecatedGlobals","GetOSByClicksDeprecatedQueryParamInterval","GetOSByClicksDeprecatedRequest","GetOSByClicksDeprecatedResponse","GetOSByClicksDeprecatedResponseBody","GetOSByClicksGlobals","GetOSByClicksQueryParamInterval","GetOSByClicksRequest","GetOSByClicksResponse","GetOSByClicksResponseBody","GetQRCodeRequest","GetQRCodeResponse","GetReferersByClicksDeprecatedGlobals","GetReferersByClicksDeprecatedQueryParamInterval","GetReferersByClicksDeprecatedRequest","GetReferersByClicksDeprecatedResponse","GetReferersByClicksDeprecatedResponseBody","GetReferersByClicksGlobals","GetReferersByClicksQueryParamInterval","GetReferersByClicksRequest","GetReferersByClicksResponse","GetReferersByClicksResponseBody","GetTagsGlobals","GetTagsRequest","GetTagsResponse","GetTimeseriesByClicksDeprecatedGlobals","GetTimeseriesByClicksDeprecatedQueryParamInterval","GetTimeseriesByClicksDeprecatedRequest","GetTimeseriesByClicksDeprecatedResponse","GetTimeseriesByClicksDeprecatedResponseBody","GetTimeseriesByClicksGlobals","GetTimeseriesByClicksRequest","GetTimeseriesByClicksResponse","GetTopLinksByClicksDeprecatedGlobals","GetTopLinksByClicksDeprecatedQueryParamInterval","GetTopLinksByClicksDeprecatedRequest","GetTopLinksByClicksDeprecatedResponse","GetTopLinksByClicksDeprecatedResponseBody","GetTopLinksByClicksGlobals","GetTopLinksByClicksQueryParamInterval","GetTopLinksByClicksRequest","GetTopLinksByClicksResponse","GetTopLinksByClicksResponseBody","GetTopURLsByClicksDeprecatedGlobals","GetTopURLsByClicksDeprecatedQueryParamInterval","GetTopURLsByClicksDeprecatedRequest","GetTopURLsByClicksDeprecatedResponse","GetTopURLsByClicksDeprecatedResponseBody","GetTopURLsByClicksGlobals","GetTopURLsByClicksQueryParamInterval","GetTopURLsByClicksRequest","GetTopURLsByClicksResponse","GetTopURLsByClicksResponseBody","GetWorkspaceRequest","GetWorkspaceResponse","GetWorkspacesResponse","GroupBy","Interval","Level","ListDomainsGlobals","ListDomainsRequest","ListDomainsResponse","One","PaymentProcessor","QueryParamInterval","QueryParamTagIds","QueryParamTagNames","RequestBody","ResponseBody","SetPrimaryDomainGlobals","SetPrimaryDomainRequest","SetPrimaryDomainResponse","Sort","TagIds","TagNames","TrackCustomerRequestBody","TrackCustomerResponse","TrackCustomerResponseBody","TrackLeadRequestBody","TrackLeadResponse","TrackLeadResponseBody","TrackSaleRequestBody","TrackSaleResponse","TrackSaleResponseBody","TransferDomainGlobals","TransferDomainRequest","TransferDomainRequestBody","TransferDomainResponse","Two","Type","UpdateDomainGlobals","UpdateDomainRequest","UpdateDomainRequestBody","UpdateDomainResponse","UpdateDomainType","UpdateLinkGlobals","UpdateLinkRequest","UpdateLinkRequestBody","UpdateLinkResponse","UpdateLinkTagIds","UpdateLinkTagNames","UpsertLinkGlobals","UpsertLinkRequestBody","UpsertLinkResponse","UpsertLinkTagIds","UpsertLinkTagNames"]
```

### Comparing `dub-0.0.4/src/dub/models/operations/adddomain.py` & `dub-0.0.5/src/dub/models/operations/adddomain.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     r"""The type of redirect to use for this domain."""
     target: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target'), 'exclude': lambda f: f is AddDomainRequestBody.UNSET }})
     r"""The page your users will get redirected to when they visit your domain."""
     expired_url: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiredUrl'), 'exclude': lambda f: f is AddDomainRequestBody.UNSET }})
     r"""Redirect users to a specific URL when any link under this domain has expired."""
     archived: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('archived'), 'exclude': lambda f: f is None }})
     r"""Whether to archive this domain. `false` will unarchive a previously archived domain."""
+    noindex: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noindex'), 'exclude': lambda f: f is None }})
+    r"""Prevent search engines from indexing the domain. Defaults to `false`."""
     placeholder: Optional[str] = dataclasses.field(default='https://dub.co/help/article/what-is-dub', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('placeholder'), 'exclude': lambda f: f is AddDomainRequestBody.UNSET }})
     r"""Provide context to your teammates in the link creation modal by showing them an example of a link to be shortened."""
     
 
 
 
 @dataclasses.dataclass
```

### Comparing `dub-0.0.4/src/dub/models/operations/bulkcreatelinks.py` & `dub-0.0.5/src/dub/models/components/linkgeotargeting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import httpmetadata as components_httpmetadata
-from ...models.components import linkschema as components_linkschema
 from dataclasses_json import Undefined, dataclass_json
 from dub import utils
-from typing import List, Optional, Union
-
-
-@dataclasses.dataclass
-class BulkCreateLinksGlobals:
-    workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
-    project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
-    r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
-    
-
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BulkCreateLinksGeo:
+class LinkGeoTargeting:
     r"""Geo targeting information for the short link in JSON format `{[COUNTRY]: https://example.com }`."""
     af: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AF'), 'exclude': lambda f: f is None }})
     al: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AL'), 'exclude': lambda f: f is None }})
     dz: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DZ'), 'exclude': lambda f: f is None }})
     as_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AS'), 'exclude': lambda f: f is None }})
     ad: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AD'), 'exclude': lambda f: f is None }})
     ao: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AO'), 'exclude': lambda f: f is None }})
@@ -270,71 +259,7 @@
     mf: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('MF'), 'exclude': lambda f: f is None }})
     rs: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('RS'), 'exclude': lambda f: f is None }})
     sx: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('SX'), 'exclude': lambda f: f is None }})
     ss: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('SS'), 'exclude': lambda f: f is None }})
     xk: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('XK'), 'exclude': lambda f: f is None }})
     
 
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class RequestBody:
-    UNSET='__SPEAKEASY_UNSET__'
-    url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-    r"""The destination URL of the short link."""
-    domain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain'), 'exclude': lambda f: f is None }})
-    r"""The domain of the short link. If not provided, the primary domain for the workspace will be used (or `dub.sh` if the workspace has no domains)."""
-    key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    r"""The short link slug. If not provided, a random 7-character slug will be generated."""
-    external_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('externalId'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""This is the ID of the link in your database. If set, it can be used to identify the link in the future. Must be prefixed with `ext_` when passed as a query parameter."""
-    prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
-    r"""The prefix of the short link slug for randomly-generated keys (e.g. if prefix is `/c/`, generated keys will be in the `/c/:key` format). Will be ignored if `key` is provided."""
-    archived: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('archived'), 'exclude': lambda f: f is None }})
-    r"""Whether the short link is archived."""
-    public_stats: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('publicStats'), 'exclude': lambda f: f is None }})
-    r"""Whether the short link's stats are publicly accessible."""
-    tag_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagId'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The unique ID of the tag assigned to the short link. This field is deprecated – use `tagIds` instead.
-
-    Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible.
-    """
-    tag_ids: Optional[Union[str, List[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagIds'), 'exclude': lambda f: f is None }})
-    r"""The unique IDs of the tags assigned to the short link."""
-    tag_names: Optional[Union[str, List[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tagNames'), 'exclude': lambda f: f is None }})
-    r"""The unique name of the tags assigned to the short link (case insensitive)."""
-    comments: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('comments'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The comments for the short link."""
-    expires_at: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiresAt'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The date and time when the short link will expire at."""
-    expired_url: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiredUrl'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The URL to redirect to when the short link has expired."""
-    password: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The password required to access the destination URL of the short link."""
-    proxy: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('proxy'), 'exclude': lambda f: f is None }})
-    r"""Whether the short link uses Custom Social Media Cards feature."""
-    title: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The title of the short link generated via `api.dub.co/metatags`. Will be used for Custom Social Media Cards if `proxy` is true."""
-    description: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The description of the short link generated via `api.dub.co/metatags`. Will be used for Custom Social Media Cards if `proxy` is true."""
-    image: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('image'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The image of the short link generated via `api.dub.co/metatags`. Will be used for Custom Social Media Cards if `proxy` is true."""
-    rewrite: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rewrite'), 'exclude': lambda f: f is None }})
-    r"""Whether the short link uses link cloaking."""
-    ios: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ios'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The iOS destination URL for the short link for iOS device targeting."""
-    android: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('android'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""The Android destination URL for the short link for Android device targeting."""
-    geo: Optional[BulkCreateLinksGeo] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('geo'), 'exclude': lambda f: f is RequestBody.UNSET }})
-    r"""Geo targeting information for the short link in JSON format `{[COUNTRY]: https://example.com }`."""
-    
-
-
-
-@dataclasses.dataclass
-class BulkCreateLinksResponse:
-    http_meta: components_httpmetadata.HTTPMetadata = dataclasses.field()
-    link_schemas: Optional[List[components_linkschema.LinkSchema]] = dataclasses.field(default=None)
-    r"""The created links"""
-    
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dub-0.0.4/src/dub/models/operations/createtag.py` & `dub-0.0.5/src/dub/models/operations/createtag.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/createworkspace.py` & `dub-0.0.5/src/dub/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/deletedomain.py` & `dub-0.0.5/src/dub/models/operations/deletedomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/deletelink.py` & `dub-0.0.5/src/dub/models/operations/deletelink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/getlinkinfo.py` & `dub-0.0.5/src/dub/models/operations/getlinkinfo.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/getlinks.py` & `dub-0.0.5/src/dub/models/operations/getlinks.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,35 @@
 class GetLinksGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+QueryParamTagIds = Union[str, List[str]]
+
+QueryParamTagNames = Union[str, List[str]]
+
 
 class Sort(str, Enum):
     r"""The field to sort the links by. The default is `createdAt`, and sort order is always descending."""
     CREATED_AT = 'createdAt'
     CLICKS = 'clicks'
     LAST_CLICKED = 'lastClicked'
 
 
 @dataclasses.dataclass
 class GetLinksRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
     r"""The domain to filter the links by. E.g. `ac.me`. If not provided, all links for the workspace will be returned."""
     tag_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagId', 'style': 'form', 'explode': True }})
     r"""The tag ID to filter the links by. This field is deprecated – use `tagIds` instead."""
-    tag_ids: Optional[Union[str, List[str]]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagIds', 'style': 'form', 'explode': True }})
+    tag_ids: Optional[QueryParamTagIds] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagIds', 'style': 'form', 'explode': True }})
     r"""The tag IDs to filter the links by."""
-    tag_names: Optional[Union[str, List[str]]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagNames', 'style': 'form', 'explode': True }})
+    tag_names: Optional[QueryParamTagNames] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagNames', 'style': 'form', 'explode': True }})
     r"""The unique name of the tags assigned to the short link (case insensitive)."""
     search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
     r"""The search term to filter the links by. The search term will be matched against the short link slug and the destination url."""
     user_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'userId', 'style': 'form', 'explode': True }})
     r"""The user ID to filter the links by."""
     show_archived: Optional[bool] = dataclasses.field(default=True, metadata={'query_param': { 'field_name': 'showArchived', 'style': 'form', 'explode': True }})
     r"""Whether to include archived links in the response. Defaults to `false` if not provided."""
```

### Comparing `dub-0.0.4/src/dub/models/operations/getlinkscount.py` & `dub-0.0.5/src/dub/models/operations/getlinkscount.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,48 @@
 class GetLinksCountGlobals:
     workspace_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'workspaceId', 'style': 'form', 'explode': True }})
     project_slug: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'projectSlug', 'style': 'form', 'explode': True }})
     r"""Deprecated field: This will be removed in a future release, please migrate away from it as soon as possible."""
     
 
 
+GetLinksCountQueryParamTagIds = Union[str, List[str]]
+
+GetLinksCountQueryParamTagNames = Union[str, List[str]]
+
 
 class Two(str, Enum):
     TAG_ID = 'tagId'
 
 
 class One(str, Enum):
     DOMAIN = 'domain'
 
+GroupBy = Union['One', 'Two']
+
 
 @dataclasses.dataclass
 class GetLinksCountRequest:
     domain: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'domain', 'style': 'form', 'explode': True }})
     r"""The domain to filter the links by. E.g. `ac.me`. If not provided, all links for the workspace will be returned."""
     tag_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagId', 'style': 'form', 'explode': True }})
     r"""The tag ID to filter the links by. This field is deprecated – use `tagIds` instead."""
-    tag_ids: Optional[Union[str, List[str]]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagIds', 'style': 'form', 'explode': True }})
+    tag_ids: Optional[GetLinksCountQueryParamTagIds] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagIds', 'style': 'form', 'explode': True }})
     r"""The tag IDs to filter the links by."""
-    tag_names: Optional[Union[str, List[str]]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagNames', 'style': 'form', 'explode': True }})
+    tag_names: Optional[GetLinksCountQueryParamTagNames] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tagNames', 'style': 'form', 'explode': True }})
     r"""The unique name of the tags assigned to the short link (case insensitive)."""
     search: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'search', 'style': 'form', 'explode': True }})
     r"""The search term to filter the links by. The search term will be matched against the short link slug and the destination url."""
     user_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'userId', 'style': 'form', 'explode': True }})
     r"""The user ID to filter the links by."""
     show_archived: Optional[bool] = dataclasses.field(default=True, metadata={'query_param': { 'field_name': 'showArchived', 'style': 'form', 'explode': True }})
     r"""Whether to include archived links in the response. Defaults to `false` if not provided."""
     with_tags: Optional[bool] = dataclasses.field(default=True, metadata={'query_param': { 'field_name': 'withTags', 'style': 'form', 'explode': True }})
     r"""Whether to include tags in the response. Defaults to `false` if not provided."""
-    group_by: Optional[Union[One, Two]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'groupBy', 'style': 'form', 'explode': True }})
+    group_by: Optional[GroupBy] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'groupBy', 'style': 'form', 'explode': True }})
     r"""The field to group the links by."""
     
 
 
 
 @dataclasses.dataclass
 class GetLinksCountResponse:
```

### Comparing `dub-0.0.4/src/dub/models/operations/getmetatags.py` & `dub-0.0.5/src/dub/models/operations/getmetatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/getqrcode.py` & `dub-0.0.5/src/dub/models/operations/getqrcode.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/gettags.py` & `dub-0.0.5/src/dub/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/getworkspace.py` & `dub-0.0.5/src/dub/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/getworkspaces.py` & `dub-0.0.5/src/dub/models/operations/getworkspaces.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/listdomains.py` & `dub-0.0.5/src/dub/models/operations/listdomains.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/setprimarydomain.py` & `dub-0.0.5/src/dub/models/operations/setprimarydomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/transferdomain.py` & `dub-0.0.5/src/dub/models/operations/transferdomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/models/operations/updatedomain.py` & `dub-0.0.5/src/dub/models/operations/updatedomain.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     r"""The type of redirect to use for this domain."""
     target: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target'), 'exclude': lambda f: f is UpdateDomainRequestBody.UNSET }})
     r"""The page your users will get redirected to when they visit your domain."""
     expired_url: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiredUrl'), 'exclude': lambda f: f is UpdateDomainRequestBody.UNSET }})
     r"""Redirect users to a specific URL when any link under this domain has expired."""
     archived: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('archived'), 'exclude': lambda f: f is None }})
     r"""Whether to archive this domain. `false` will unarchive a previously archived domain."""
+    noindex: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noindex'), 'exclude': lambda f: f is None }})
+    r"""Prevent search engines from indexing the domain. Defaults to `false`."""
     placeholder: Optional[str] = dataclasses.field(default='https://dub.co/help/article/what-is-dub', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('placeholder'), 'exclude': lambda f: f is UpdateDomainRequestBody.UNSET }})
     r"""Provide context to your teammates in the link creation modal by showing them an example of a link to be shortened."""
     
 
 
 
 @dataclasses.dataclass
```

### Comparing `dub-0.0.4/src/dub/qr_codes.py` & `dub-0.0.5/src/dub/qr_codes.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/sdk.py` & `dub-0.0.5/src/dub/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .analytics import Analytics
 from .domains import Domains
 from .links import Links
 from .metatags import Metatags
 from .qr_codes import QRCodes
 from .sdkconfiguration import SDKConfiguration
 from .tags import Tags
+from .track import Track
 from .utils.retries import RetryConfig
 from .workspaces import Workspaces
 from dub import utils
 from dub._hooks import SDKHooks
 from dub.models import components, internal
 from typing import Callable, Dict, Optional, Union
 
@@ -19,14 +20,15 @@
     r"""Dub.co API: Dub is link management infrastructure for companies to create marketing campaigns, link sharing features, and referral programs."""
     links: Links
     qr_codes: QRCodes
     analytics: Analytics
     workspaces: Workspaces
     tags: Tags
     domains: Domains
+    track: Track
     metatags: Metatags
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
                  token: Union[Optional[str], Callable[[], Optional[str]]] = None,
                  workspace_id: str = None,
@@ -99,8 +101,9 @@
     def _init_sdks(self):
         self.links = Links(self.sdk_configuration)
         self.qr_codes = QRCodes(self.sdk_configuration)
         self.analytics = Analytics(self.sdk_configuration)
         self.workspaces = Workspaces(self.sdk_configuration)
         self.tags = Tags(self.sdk_configuration)
         self.domains = Domains(self.sdk_configuration)
+        self.track = Track(self.sdk_configuration)
         self.metatags = Metatags(self.sdk_configuration)
```

### Comparing `dub-0.0.4/src/dub/sdkconfiguration.py` & `dub-0.0.5/src/dub/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '0.0.1'
-    sdk_version: str = '0.0.4'
-    gen_version: str = '2.332.4'
-    user_agent: str = 'speakeasy-sdk/python 0.0.4 2.332.4 0.0.1 dub'
+    sdk_version: str = '0.0.5'
+    gen_version: str = '2.333.3'
+    user_agent: str = 'speakeasy-sdk/python 0.0.5 2.333.3 0.0.1 dub'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `dub-0.0.4/src/dub/tags.py` & `dub-0.0.5/src/dub/tags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/utils/retries.py` & `dub-0.0.5/src/dub/utils/retries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/utils/utils.py` & `dub-0.0.5/src/dub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub/workspaces.py` & `dub-0.0.5/src/dub/workspaces.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.4/src/dub.egg-info/PKG-INFO` & `dub-0.0.5/src/dub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # dub
         
         <div align="left">
@@ -145,14 +145,20 @@
         * [list](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#list) - Retrieve a list of domains
         * [add](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add a domain
         * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#delete) - Delete a domain
         * [update](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a domain
         * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#set_primary) - Set a domain as primary
         * [transfer](https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#transfer) - Transfer a domain
         
+        ### [track](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md)
+        
+        * [lead](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md#lead) - Track a lead
+        * [sale](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md#sale) - Track a sale
+        * [customer](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/README.md#customer) - Track a customer
+        
         ### [metatags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md)
         
         * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md#get) - Retrieve the metatags for a URL
         <!-- End Available Resources and Operations [operations] -->
         
         <!-- Start Error Handling [errors] -->
         ## Error Handling
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.4 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.5 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy License: UNKNOWN Description: # dub
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
 based on your OpenAPI spec. However, it is not yet ready for production use.
@@ -100,30 +100,35 @@
 github.com/dubinc/dub-python/blob/master/docs/sdks/domains/README.md#add) - Add
 a domain * [delete](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
 domains/README.md#delete) - Delete a domain * [update](https://github.com/
 dubinc/dub-python/blob/master/docs/sdks/domains/README.md#update) - Update a
 domain * [set_primary](https://github.com/dubinc/dub-python/blob/master/docs/
 sdks/domains/README.md#set_primary) - Set a domain as primary * [transfer]
 (https://github.com/dubinc/dub-python/blob/master/docs/sdks/domains/
-README.md#transfer) - Transfer a domain ### [metatags](https://github.com/
-dubinc/dub-python/blob/master/docs/sdks/metatags/README.md) * [get](https://
-github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/README.md#get) -
-Retrieve the metatags for a URL ## Error Handling Handling errors in this SDK
-should largely match your expectations. All operations return a response object
-or raise an error. If Error objects are specified in your OpenAPI Spec, the SDK
-will raise the appropriate Error type. | Error Object | Status Code | Content
-Type | | -------------------------- | -------------------------- | ------------
--------------- | | errors.BadRequest | 400 | application/json | |
-errors.Unauthorized | 401 | application/json | | errors.Forbidden | 403 |
-application/json | | errors.NotFound | 404 | application/json | |
-errors.Conflict | 409 | application/json | | errors.InviteExpired | 410 |
-application/json | | errors.UnprocessableEntity | 422 | application/json | |
-errors.RateLimitExceeded | 429 | application/json | |
-errors.InternalServerError | 500 | application/json | | errors.SDKError | 4xx-
-5xx | */* | ### Example ```python import dub from dub.models import errors,
+README.md#transfer) - Transfer a domain ### [track](https://github.com/dubinc/
+dub-python/blob/master/docs/sdks/track/README.md) * [lead](https://github.com/
+dubinc/dub-python/blob/master/docs/sdks/track/README.md#lead) - Track a lead *
+[sale](https://github.com/dubinc/dub-python/blob/master/docs/sdks/track/
+README.md#sale) - Track a sale * [customer](https://github.com/dubinc/dub-
+python/blob/master/docs/sdks/track/README.md#customer) - Track a customer ###
+[metatags](https://github.com/dubinc/dub-python/blob/master/docs/sdks/metatags/
+README.md) * [get](https://github.com/dubinc/dub-python/blob/master/docs/sdks/
+metatags/README.md#get) - Retrieve the metatags for a URL ## Error Handling
+Handling errors in this SDK should largely match your expectations. All
+operations return a response object or raise an error. If Error objects are
+specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
+| Error Object | Status Code | Content Type | | -------------------------- | --
+------------------------ | -------------------------- | | errors.BadRequest |
+400 | application/json | | errors.Unauthorized | 401 | application/json | |
+errors.Forbidden | 403 | application/json | | errors.NotFound | 404 |
+application/json | | errors.Conflict | 409 | application/json | |
+errors.InviteExpired | 410 | application/json | | errors.UnprocessableEntity |
+422 | application/json | | errors.RateLimitExceeded | 429 | application/json |
+| errors.InternalServerError | 500 | application/json | | errors.SDKError |
+4xx-5xx | */* | ### Example ```python import dub from dub.models import errors,
 operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res = None try:
 res = s.links.list(request=operations.GetLinksRequest()) except
 errors.BadRequest as e: # handle exception raise(e) except errors.Unauthorized
 as e: # handle exception raise(e) except errors.Forbidden as e: # handle
 exception raise(e) except errors.NotFound as e: # handle exception raise(e)
 except errors.Conflict as e: # handle exception raise(e) except
 errors.InviteExpired as e: # handle exception raise(e) except
```

### Comparing `dub-0.0.4/src/dub.egg-info/SOURCES.txt` & `dub-0.0.5/src/dub.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,33 @@
 src/dub/domains.py
 src/dub/links.py
 src/dub/metatags.py
 src/dub/qr_codes.py
 src/dub/sdk.py
 src/dub/sdkconfiguration.py
 src/dub/tags.py
+src/dub/track.py
 src/dub/workspaces.py
 src/dub.egg-info/PKG-INFO
 src/dub.egg-info/SOURCES.txt
 src/dub.egg-info/dependency_links.txt
 src/dub.egg-info/requires.txt
 src/dub.egg-info/top_level.txt
 src/dub/_hooks/__init__.py
 src/dub/_hooks/registration.py
 src/dub/_hooks/sdkhooks.py
 src/dub/_hooks/types.py
 src/dub/models/__init__.py
 src/dub/models/components/__init__.py
+src/dub/models/components/clicksbycities.py
+src/dub/models/components/clicksbycountry.py
+src/dub/models/components/countrycode.py
 src/dub/models/components/domainschema.py
 src/dub/models/components/httpmetadata.py
+src/dub/models/components/linkgeotargeting.py
 src/dub/models/components/linkschema.py
 src/dub/models/components/security.py
 src/dub/models/components/tagschema.py
 src/dub/models/components/workspaceschema.py
 src/dub/models/errors/__init__.py
 src/dub/models/errors/badrequest.py
 src/dub/models/errors/conflict.py
@@ -75,14 +80,17 @@
 src/dub/models/operations/gettoplinksbyclicksdeprecated.py
 src/dub/models/operations/gettopurlsbyclicks.py
 src/dub/models/operations/gettopurlsbyclicksdeprecated.py
 src/dub/models/operations/getworkspace.py
 src/dub/models/operations/getworkspaces.py
 src/dub/models/operations/listdomains.py
 src/dub/models/operations/setprimarydomain.py
+src/dub/models/operations/trackcustomer.py
+src/dub/models/operations/tracklead.py
+src/dub/models/operations/tracksale.py
 src/dub/models/operations/transferdomain.py
 src/dub/models/operations/updatedomain.py
 src/dub/models/operations/updatelink.py
 src/dub/models/operations/upsertlink.py
 src/dub/utils/__init__.py
 src/dub/utils/retries.py
 src/dub/utils/utils.py
```

