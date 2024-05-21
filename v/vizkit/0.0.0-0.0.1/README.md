# Comparing `tmp/vizkit-0.0.0.tar.gz` & `tmp/vizkit-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizkit-0.0.0.tar", max compression
+gzip compressed data, was "vizkit-0.0.1.tar", max compression
```

## Comparing `vizkit-0.0.0.tar` & `vizkit-0.0.1.tar`

### file list

```diff
@@ -1,5 +1,23 @@
--rw-r--r--   0        0        0     1068 2024-04-15 01:29:13.345313 vizkit-0.0.0/LICENSE
--rw-r--r--   0        0        0        8 2024-03-06 23:32:14.523348 vizkit-0.0.0/README.md
--rw-r--r--   0        0        0      292 2024-05-10 14:32:26.737052 vizkit-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 01:29:13.345869 vizkit-0.0.0/src/vizkit/__init__.py
--rw-r--r--   0        0        0      462 1970-01-01 00:00:00.000000 vizkit-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      688 2024-05-21 11:57:34.946055 vizkit-0.0.1/README.md
+-rw-r--r--   0        0        0      651 2024-05-21 12:03:18.997721 vizkit-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1919 2024-05-19 11:48:26.557546 vizkit-0.0.1/vizkit/__init__.py
+-rw-r--r--   0        0        0       72 2024-05-17 01:21:28.031844 vizkit-0.0.1/vizkit/api/__init__.py
+-rw-r--r--   0        0        0     6370 2024-05-19 06:05:37.373533 vizkit-0.0.1/vizkit/api/api.py
+-rw-r--r--   0        0        0     4836 2024-05-20 11:37:58.429796 vizkit-0.0.1/vizkit/api/v1/__init__.py
+-rw-r--r--   0        0        0     1047 2024-05-19 06:38:20.564008 vizkit-0.0.1/vizkit/cookies.py
+-rw-r--r--   0        0        0      706 2024-05-19 11:45:31.827682 vizkit-0.0.1/vizkit/main.py
+-rw-r--r--   0        0        0     3933 2024-05-21 11:31:47.724103 vizkit-0.0.1/vizkit/pipeline/__init__.py
+-rw-r--r--   0        0        0    18834 2024-05-21 12:44:50.733001 vizkit-0.0.1/vizkit/pipeline/blocks.py
+-rw-r--r--   0        0        0     3175 2024-05-19 11:34:32.797192 vizkit-0.0.1/vizkit/pipeline/data_source/__init__.py
+-rw-r--r--   0        0        0     5976 2024-05-21 01:31:48.828056 vizkit-0.0.1/vizkit/pipeline/data_source/firebase/__init__.py
+-rw-r--r--   0        0        0     4836 2024-05-21 01:25:35.019001 vizkit-0.0.1/vizkit/pipeline/data_source/firebase/auth.py
+-rw-r--r--   0        0        0     6980 2024-05-21 01:01:35.272840 vizkit-0.0.1/vizkit/pipeline/data_source/firebase/fb_utils.py
+-rw-r--r--   0        0        0     4702 2024-05-21 11:27:19.346383 vizkit-0.0.1/vizkit/pipeline/data_source/local.py
+-rw-r--r--   0        0        0     2274 2024-05-19 04:37:16.597671 vizkit-0.0.1/vizkit/pipeline/serialize.py
+-rw-r--r--   0        0        0     1783 2024-05-21 06:44:18.404351 vizkit-0.0.1/vizkit/pipeline/utils.py
+-rw-r--r--   0        0        0      725 2024-05-21 01:18:41.980028 vizkit-0.0.1/vizkit/web/components/block_controls.py
+-rw-r--r--   0        0        0     5120 2024-05-21 02:22:17.496473 vizkit-0.0.1/vizkit/web/components/filters.py
+-rw-r--r--   0        0        0     2368 2024-05-21 12:43:56.146630 vizkit-0.0.1/vizkit/web/components/flex.py
+-rw-r--r--   0        0        0     3172 2024-05-21 13:03:26.468745 vizkit-0.0.1/vizkit/web/components/footer.py
+-rw-r--r--   0        0        0     2146 2024-05-21 12:39:19.611443 vizkit-0.0.1/vizkit/web/plot.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 vizkit-0.0.1/PKG-INFO
```

