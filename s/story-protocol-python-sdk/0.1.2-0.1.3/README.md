# Comparing `tmp/story_protocol_python_sdk-0.1.2.tar.gz` & `tmp/story_protocol_python_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.2.tar", last modified: Tue May 21 20:59:56 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.1.3.tar", last modified: Tue May 21 21:28:17 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.2.tar` & `story_protocol_python_sdk-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.292609 story_protocol_python_sdk-0.1.2/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      955 2024-05-21 20:59:56.288610 story_protocol_python_sdk-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:59:56.292609 story_protocol_python_sdk-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      927 2024-05-21 20:59:22.000000 story_protocol_python_sdk-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.092983 story_protocol_python_sdk-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.121479 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.161480 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.169478 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 18:18:17.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 18:18:17.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.173477 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.181478 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 18:18:21.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 18:18:21.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.189476 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 18:18:23.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 18:18:23.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.198543 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 18:18:20.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 18:18:20.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.220610 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 18:18:18.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 18:18:18.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.224607 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 18:18:25.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 18:18:25.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.232611 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 18:18:24.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 18:18:24.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.272610 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/
--rw-rw-rw-   0        0        0     6729 2024-05-21 20:58:11.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    16042 2024-05-21 20:58:07.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/License.py
--rw-rw-rw-   0        0        0    12301 2024-05-21 20:58:00.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.284613 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7343 2024-05-21 18:16:50.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5270 2024-05-21 18:18:06.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1557 2024-05-21 20:57:32.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.288610 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/license_terms.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.157477 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      955 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2710 2024-05-21 20:59:56.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.868385 story_protocol_python_sdk-0.1.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      932 2024-05-21 21:28:17.866385 story_protocol_python_sdk-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.3/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 21:28:17.868385 story_protocol_python_sdk-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-21 21:22:06.000000 story_protocol_python_sdk-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.687206 story_protocol_python_sdk-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.698766 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.714960 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.722963 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-21 21:26:30.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.726958 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.736960 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-21 21:25:30.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.746149 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-21 21:25:32.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.755374 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-21 21:25:29.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.764384 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-21 21:26:32.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.773385 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-21 21:25:34.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.783384 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-21 21:25:33.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.801386 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     6739 2024-05-21 21:20:33.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    16122 2024-05-21 21:21:25.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0    12345 2024-05-21 21:21:50.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.856384 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7361 2024-05-21 21:24:57.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5288 2024-05-21 21:26:03.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1557 2024-05-21 20:57:32.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.863385 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:28:17.713959 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      932 2024-05-21 21:28:17.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2024-05-21 21:28:17.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:28:17.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-21 21:28:17.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-21 21:28:17.000000 story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.2/LICENSE` & `story_protocol_python_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/PKG-INFO` & `story_protocol_python_sdk-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python SDK for interacting with the Story Protocol.
-Home-page: https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install
+Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: web3>=5.0.0
 Requires-Dist: pytest
 Requires-Dist: python-dotenv
 
 # Story Protocol SDK
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from web3 import Web3
 from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
 from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
 from story_protocol_python_sdk.abi.LicenseToken.LicenseToken_client import LicenseTokenClient
 from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
 
 # Configure logging
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger(__name__)
+# logging.basicConfig(level=logging.INFO)
+# logger = logging.getLogger(__name__)
 
 class IPAsset:
     def __init__(self, web3: Web3, account, chain_id):
         self.web3 = web3
         self.account = account
         self.chain_id = chain_id
 
@@ -60,15 +60,15 @@
             
             return {
                 'txHash': tx_hash.hex(),
                 'ipId': ip_id
             }
 
         except Exception as e:
-            logger.error(f"Error interacting with contract: {e}")
+            # logger.error(f"Error interacting with contract: {e}")
             raise e
 
     def registerDerivative(self, child_ip_id, parent_ip_ids, license_terms_ids, license_template):
         try:
             # Check if the child IP is registered
             if not self._is_registered(child_ip_id):
                 raise ValueError(f"The child IP with id {child_ip_id} is not registered.")
@@ -106,15 +106,15 @@
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             
             return {
                 'txHash': tx_hash.hex()
             }
 
         except Exception as e:
-            logger.error(f"Failed to register derivative: {e}")
+            # logger.error(f"Failed to register derivative: {e}")
             raise e
         
     def registerDerivativeWithLicenseTokens(self, child_ip_id, license_token_ids):
         try:
             # Check if the child IP is registered
             if not self._is_registered(child_ip_id):
                 raise ValueError(f"The child IP with id {child_ip_id} is not registered.")
@@ -142,9 +142,9 @@
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
             
             return {
                 'txHash': tx_hash.hex()
             }
 
         except Exception as e:
-            logger.error(f"Failed to register derivative with license tokens: {e}")
+            # logger.error(f"Failed to register derivative with license tokens: {e}")
             raise e
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/License.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,204 +5,204 @@
 from story_protocol_python_sdk.abi.PILicenseTemplate.PILicenseTemplate_client import PILicenseTemplateClient
 from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
 from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
 from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
 from story_protocol_python_sdk.utils.license_terms import get_license_term_by_type, PIL_TYPE
 
 # Configure logging
-logging.basicConfig(level=logging.DEBUG)  # Set to DEBUG to capture all log messages
-logger = logging.getLogger(__name__)
+# logging.basicConfig(level=logging.DEBUG)  # Set to DEBUG to capture all log messages
+# logger = logging.getLogger(__name__)
 
 class License:
     def __init__(self, web3: Web3, account, chain_id):
         self.web3 = web3
         self.account = account
         self.chain_id = chain_id
 
         self.license_template_client = PILicenseTemplateClient(web3)
         self.license_registry_client = LicenseRegistryClient(web3)
         self.licensing_module_client  = LicensingModuleClient(web3)
         self.ip_asset_registry_client = IPAssetRegistryClient(web3)
 
     def _get_license_terms_id(self, license_terms):
-        logger.info(f"Getting license terms ID for: {license_terms}")
+        # logger.info(f"Getting license terms ID for: {license_terms}")
         return self.license_template_client.getLicenseTermsId(license_terms)
 
     def registerNonComSocialRemixingPIL(self):
         try:
             # Get the license terms for non-commercial social remixing PIL
             license_terms = get_license_term_by_type(PIL_TYPE['NON_COMMERCIAL_REMIX'])
-            logger.info(f"License terms: {license_terms}")
+            # logger.info(f"License terms: {license_terms}")
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(license_terms)
-            logger.info(f"License terms ID: {license_terms_id}")
+            # logger.info(f"License terms ID: {license_terms_id}")
             if (license_terms_id is not None) and (license_terms_id != 0):
                 return {'licenseTermsId': license_terms_id}
 
             # Build the transaction
             transaction = self.license_template_client.build_registerLicenseTerms_transaction(
                 license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': self.web3.to_wei('100', 'gwei')  # Adjusted gas price for faster processing
                 }
             )
-            logger.info(f"Transaction: {transaction}")
+            # logger.info(f"Transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
 
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
             }
 
         except Exception as e:
-            logger.error(f"Error interacting with contract: {e}")
+            # logger.error(f"Error interacting with contract: {e}")
             raise e
         
     def registerCommercialUsePIL(self, minting_fee, currency, royalty_policy, tx_options=None):
         try:
-            logger.info(f"Starting registerCommercialUsePIL with minting_fee: {minting_fee}, currency: {currency}, royalty_policy: {royalty_policy}")
+            # logger.info(f"Starting registerCommercialUsePIL with minting_fee: {minting_fee}, currency: {currency}, royalty_policy: {royalty_policy}")
 
             # Construct complete license terms
             complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_USE'], {
                 'mintingFee': minting_fee,
                 'currency': currency,
                 'royaltyPolicy': royalty_policy,
             })
-            logger.info(f"Complete license terms: {complete_license_terms}")
+            # logger.info(f"Complete license terms: {complete_license_terms}")
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(complete_license_terms)
-            logger.info(f"License terms ID: {license_terms_id}")
+            # logger.info(f"License terms ID: {license_terms_id}")
             if (license_terms_id is not None) and (license_terms_id != 0):
                 return {'licenseTermsId': license_terms_id}
 
             # Build the transaction
             transaction = self.license_template_client.build_registerLicenseTerms_transaction(
                 complete_license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': self.web3.to_wei('100', 'gwei')  # Adjusted gas price for faster processing
                 }
             )
-            logger.info(f"Built transaction: {transaction}")
+            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             if not tx_receipt.logs:
-                logger.error(f"No logs found in transaction receipt: {tx_receipt}")
+                # logger.error(f"No logs found in transaction receipt: {tx_receipt}")
                 return None
 
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
             }
 
         except Exception as e:
-            logger.error(f"Error interacting with contract: {e}")
+            # logger.error(f"Error interacting with contract: {e}")
             raise e
 
     def registerCommercialRemixPIL(self, minting_fee, currency, commercial_rev_share, royalty_policy, tx_options=None):
         try:
-            logger.info(f"Starting registerCommercialRemixPIL with minting_fee: {minting_fee}, currency: {currency}, commercial_rev_share: {commercial_rev_share}, royalty_policy: {royalty_policy}")
+            # logger.info(f"Starting registerCommercialRemixPIL with minting_fee: {minting_fee}, currency: {currency}, commercial_rev_share: {commercial_rev_share}, royalty_policy: {royalty_policy}")
 
             # Construct complete license terms
             complete_license_terms = get_license_term_by_type(PIL_TYPE['COMMERCIAL_REMIX'], {
                 'mintingFee': minting_fee,
                 'currency': currency,
                 'commercialRevShare': commercial_rev_share,
                 'royaltyPolicy': royalty_policy,
             })
-            logger.info(f"Complete license terms: {complete_license_terms}")
+            # logger.info(f"Complete license terms: {complete_license_terms}")
 
             # Check if the license terms are already registered
             license_terms_id = self._get_license_terms_id(complete_license_terms)
-            logger.info(f"License terms ID: {license_terms_id}")
+            # logger.info(f"License terms ID: {license_terms_id}")
             if license_terms_id and license_terms_id != 0:
                 return {'licenseTermsId': license_terms_id}
 
             # Build the transaction
             transaction = self.license_template_client.build_registerLicenseTerms_transaction(
                 complete_license_terms, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': self.web3.to_wei('100', 'gwei')
                 }
             )
-            logger.info(f"Built transaction: {transaction}")
+            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTermsRegistered
             if not tx_receipt.logs:
-                logger.error(f"No logs found in transaction receipt: {tx_receipt}")
+                # logger.error(f"No logs found in transaction receipt: {tx_receipt}")
                 return None
 
             target_logs = self._parse_tx_license_terms_registered_event(tx_receipt)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTermsId': target_logs
             }
 
         except Exception as e:
-            logger.error(f"Error interacting with contract: {e}")
+            # logger.error(f"Error interacting with contract: {e}")
             raise e
 
     def _parse_tx_license_terms_registered_event(self, tx_receipt):
         event_signature = self.web3.keccak(text="LicenseTermsRegistered(uint256,address,bytes)").hex()
 
         for log in tx_receipt['logs']:
             if log['topics'][0].hex() == event_signature:
                 return int(log['topics'][1].hex(), 16)
 
         return None
     
     def attachLicenseTerms(self, ip_id, license_template, license_terms_id):
         try:
-            logger.info(f"Starting attachLicenseTerms with ip_id: {ip_id}, license_template: {license_template}, license_terms_id: {license_terms_id}")
+            # logger.info(f"Starting attachLicenseTerms with ip_id: {ip_id}, license_template: {license_template}, license_terms_id: {license_terms_id}")
 
             # Validate the license template address
             if not Web3.is_address(license_template):
                 raise ValueError(f'Address "{license_template}" is invalid.')
 
             # Check if the IP is registered
             is_registered = self.ip_asset_registry_client.isRegistered(ip_id)
@@ -224,37 +224,37 @@
                 ip_id, license_template, license_terms_id, {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': self.web3.to_wei('100', 'gwei')
                 }
             )
-            logger.info(f"Built transaction: {transaction}")
+            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for the transaction receipt
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             return {'txHash': tx_hash.hex()}
         
         except Exception as e:
-            logger.error(f"Failed to attach license terms: {e}")
+            # logger.error(f"Failed to attach license terms: {e}")
             raise e
         
     def mintLicenseTokens(self, licensor_ip_id, license_template, license_terms_id, amount, receiver):
         try:
-            logger.info(f"Starting mintLicenseTokens with licensor_ip_id: {licensor_ip_id}, license_template: {license_template}, license_terms_id: {license_terms_id}, amount: {amount}, receiver: {receiver}")
+            # logger.info(f"Starting mintLicenseTokens with licensor_ip_id: {licensor_ip_id}, license_template: {license_template}, license_terms_id: {license_terms_id}, amount: {amount}, receiver: {receiver}")
 
             # Validate the license template address
             if not Web3.is_address(license_template):
                 raise ValueError(f'Address "{license_template}" is invalid.')
             
             # Validate the license template address
             if not Web3.is_address(receiver):
@@ -280,38 +280,38 @@
                 licensor_ip_id, license_template, license_terms_id, amount, receiver, '0x0000000000000000000000000000000000000000', {
                     'from': self.account.address,
                     'nonce': self.web3.eth.get_transaction_count(self.account.address),
                     'gas': 2000000,
                     'gasPrice': self.web3.to_wei('100', 'gwei')
                 }
             )
-            logger.info(f"Built transaction: {transaction}")
+            # logger.info(f"Built transaction: {transaction}")
 
             # Sign the transaction
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for the transaction receipt
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             # Parse the event logs for LicenseTokensMinted
             target_logs = self._parse_tx_license_tokens_minted_event(tx_receipt)
             # print("the license token id is " , target_logs)
             return {
                 'txHash': tx_hash.hex(),
                 'licenseTokenIds': target_logs
             }
 
         except Exception as e:
-            logger.error(f"Failed to mint license tokens: {e}")
+            # logger.error(f"Failed to mint license tokens: {e}")
             raise e
 
     def _parse_tx_license_tokens_minted_event(self, tx_receipt):
         event_signature = self.web3.keccak(text="LicenseTokenMinted(address,address,uint256)").hex()
         token_ids = []
 
         for log in tx_receipt['logs']:
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from web3 import Web3
 from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
 from story_protocol_python_sdk.abi.IpRoyaltyVaultImpl.IpRoyaltyVaultImpl_client import IpRoyaltyVaultImplClient
 from story_protocol_python_sdk.abi.RoyaltyPolicyLAP.RoyaltyPolicyLAP_client import RoyaltyPolicyLAPClient
 from story_protocol_python_sdk.abi.RoyaltyModule.RoyaltyModule_client import RoyaltyModuleClient
 
 # Configure logging
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger(__name__)
+# logging.basicConfig(level=logging.INFO)
+# logger = logging.getLogger(__name__)
 
 class Royalty:
     def __init__(self, web3: Web3, account, chain_id):
         self.web3 = web3
         self.account = account
         self.chain_id = chain_id
 
@@ -42,34 +42,34 @@
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
                 'gasPrice': self.web3.to_wei('300', 'gwei')
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
     
             royaltyTokensCollected = self._parseTxRoyaltyTokensCollectedEvent(tx_receipt)
             # print("Number of royalty tokens collected: ", royaltyTokensCollected)
 
             return {
                 'txHash': tx_hash.hex(),
                 'royaltyTokensCollected': royaltyTokensCollected
             }
         
         except Exception as e:
-            logger.error(f"Failed to collect royalty tokens: {e}")
+            # logger.error(f"Failed to collect royalty tokens: {e}")
             raise e
 
     def _getRoyaltyVaultAddress(self, royalty_vault_ip_id):
         # Check if the royalty vault IP is registered
         is_registered = self.ip_asset_registry_client.isRegistered(royalty_vault_ip_id)
         if not is_registered:
             raise ValueError(f"The royalty vault IP with id {royalty_vault_ip_id} is not registered.")
@@ -95,15 +95,15 @@
 
         return None
     
     def snapshot(self, child_ip_id, tx_options=None):
         try:
             # Get the royalty vault address
             proxy_address = self._getRoyaltyVaultAddress(child_ip_id)
-            logger.info(f"The proxy address: {proxy_address}")
+            # logger.info(f"The proxy address: {proxy_address}")
             #print("Thne proxy addres: ", proxy_address)
 
             # Initialize the IP Royalty Vault client with the proxy address
             ip_royalty_vault_client = IpRoyaltyVaultImplClient(self.web3, contract_address=proxy_address)
 
             # Build the transaction
             transaction = ip_royalty_vault_client.build_snapshot_transaction({
@@ -111,33 +111,33 @@
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
                 'gasPrice': self.web3.to_wei('300', 'gwei')
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             snapshotId =  self._parseTxSnapshotCompletedEvent(tx_receipt)
 
             return {
                 'txHash': tx_hash.hex(),
                 'snapshotId': snapshotId
             }
         except Exception as e:
-            logger.error(f"Failed to snapshot: {e}")
+            # logger.error(f"Failed to snapshot: {e}")
             raise e
 
     def _parseTxSnapshotCompletedEvent(self, tx_receipt):
         event_signature = self.web3.keccak(text="SnapshotCompleted(uint256,uint256,uint32)").hex()
         
         for log in tx_receipt['logs']:
             if log['topics'][0].hex() == event_signature:
@@ -150,15 +150,15 @@
 
         return None
 
     def claimableRevenue(self, child_ip_id, account_address, snapshot_id, token, tx_options=None):
         try:
             # Get the royalty vault address
             proxy_address = self._getRoyaltyVaultAddress(child_ip_id)
-            logger.info(f"The proxy address: {proxy_address}")
+            # logger.info(f"The proxy address: {proxy_address}")
             # print("Thne proxy addres: ", proxy_address)
 
             # Initialize the IP Royalty Vault client with the proxy address
             ip_royalty_vault_client = IpRoyaltyVaultImplClient(self.web3, contract_address=proxy_address)
 
             # Get the claimable revenue
             claimable_revenue = ip_royalty_vault_client.claimableRevenue(
@@ -166,15 +166,15 @@
                 snapshotId=snapshot_id,
                 token=token
             )
 
             return claimable_revenue
 
         except Exception as e:
-            logger.error(f"Failed to calculate claimable revenue: {e}")
+            # logger.error(f"Failed to calculate claimable revenue: {e}")
             raise e
         
     def payRoyaltyOnBehalf(self, receiver_ip_id, payer_ip_id, token, amount, tx_options=None):
         try:
             # Check if the receiver IP is registered
             is_receiver_registered = self.ip_asset_registry_client.isRegistered(receiver_ip_id)
             if not is_receiver_registered:
@@ -191,38 +191,38 @@
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
                 'gasPrice': self.web3.to_wei('300', 'gwei')
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             if tx_options and tx_options.get('wait_for_transaction'):
                 self.web3.eth.wait_for_transaction_receipt(tx_hash)
 
             return {'txHash': tx_hash.hex()}
 
         except Exception as e:
-            logger.error(f"Failed to pay royalty on behalf: {e}")
+            # logger.error(f"Failed to pay royalty on behalf: {e}")
             raise e
     
     def claimRevenue(self, snapshotIds, child_ip_id, token):
         try:
             # Get the royalty vault address
             proxy_address = self._getRoyaltyVaultAddress(child_ip_id)
-            logger.info(f"The proxy address: {proxy_address}")
+            # logger.info(f"The proxy address: {proxy_address}")
             # print("The proxy addres: ", proxy_address)
 
             # Initialize the IP Royalty Vault client with the proxy address
             ip_royalty_vault_client = IpRoyaltyVaultImplClient(self.web3, contract_address=proxy_address)
 
             # Build the transaction
             transaction = ip_royalty_vault_client.build_claimRevenueBySnapshotBatch_transaction(snapshotIds, token, {
@@ -230,33 +230,33 @@
                 'nonce': self.web3.eth.get_transaction_count(self.account.address),
                 'gas': 2000000,
                 'gasPrice': self.web3.to_wei('300', 'gwei')
             })
 
             # Sign the transaction using the account object
             signed_txn = self.account.sign_transaction(transaction)
-            logger.info(f"Signed transaction: {signed_txn}")
+            # logger.info(f"Signed transaction: {signed_txn}")
 
             # Send the transaction
             tx_hash = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
-            logger.info(f"Transaction hash: {tx_hash.hex()}")
+            # logger.info(f"Transaction hash: {tx_hash.hex()}")
 
             # Wait for transaction receipt with a longer timeout
             tx_receipt = self.web3.eth.wait_for_transaction_receipt(tx_hash, timeout=600)  # 10 minutes timeout
-            logger.info(f"Transaction receipt: {tx_receipt}")
+            # logger.info(f"Transaction receipt: {tx_receipt}")
 
             revenue_tokens_claimed =  self._parseTxRevenueTokenClaimedEvent(tx_receipt)
             # print("Amount: ", revenue_tokens_claimed)
 
             return {
                 'txHash': tx_hash.hex(),
                 'claimableToken': revenue_tokens_claimed
             }
         except Exception as e:
-            logger.error(f"Failed to claim revenue: {e}")
+            # logger.error(f"Failed to claim revenue: {e}")
             raise e
         
     def _parseTxRevenueTokenClaimedEvent(self, tx_receipt):
         event_signature = self.web3.keccak(text="RevenueTokenClaimed(address,address,uint256)").hex()
         
         for log in tx_receipt['logs']:
             if log['topics'][0].hex() == event_signature:
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import os
 from jinja2 import Template
 from dotenv import load_dotenv
 import time
 
 # Load environment variables from .env file
-load_dotenv(os.path.join(os.path.dirname(__file__), '.env'))
+load_dotenv(os.path.join(os.path.dirname(__file__), '..', '..', '..', '.env'))
 
 # Get the API key from environment variables
 api_key = os.getenv('ETHERSCAN_API_KEY')
 if not api_key:
     raise ValueError("Please set ETHERSCAN_API_KEY in the .env file")
 
 def fetch_abi(contract_address, api_key):
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os
 from jinja2 import Template
 from dotenv import load_dotenv
 import time
 
 # Load environment variables from .env file
-load_dotenv(os.path.join(os.path.dirname(__file__), '.env'))
+load_dotenv(os.path.join(os.path.dirname(__file__), '..', '..', '..', '.env'))
 
 # Get the API key from environment variables
 api_key = os.getenv('ETHERSCAN_API_KEY')
 if not api_key:
     raise ValueError("Please set ETHERSCAN_API_KEY in the .env file")
 
 def fetch_abi(contract_address, api_key):
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: story-protocol-python-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python SDK for interacting with the Story Protocol.
-Home-page: https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install
+Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: web3>=5.0.0
 Requires-Dist: pytest
 Requires-Dist: python-dotenv
 
 # Story Protocol SDK
```

### Comparing `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.1.3/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

