# Comparing `tmp/story_protocol_python_sdk-0.1.1.tar.gz` & `tmp/story_protocol_python_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.1.1.tar", last modified: Tue May 21 18:54:50 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.1.2.tar", last modified: Tue May 21 20:59:56 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.1.1.tar` & `story_protocol_python_sdk-0.1.2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.800325 story_protocol_python_sdk-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      160 2024-05-21 17:54:58.000000 story_protocol_python_sdk-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      955 2024-05-21 18:54:50.798076 story_protocol_python_sdk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/README.md
--rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 18:54:50.800325 story_protocol_python_sdk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      860 2024-05-21 18:54:25.000000 story_protocol_python_sdk-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.699554 story_protocol_python_sdk-0.1.1/src/
--rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.699554 story_protocol_python_sdk-0.1.1/src/abi/
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.709165 story_protocol_python_sdk-0.1.1/src/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 18:18:17.000000 story_protocol_python_sdk-0.1.1/src/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 18:18:17.000000 story_protocol_python_sdk-0.1.1/src/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.715038 story_protocol_python_sdk-0.1.1/src/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.1/src/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.1/src/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.721159 story_protocol_python_sdk-0.1.1/src/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 18:18:21.000000 story_protocol_python_sdk-0.1.1/src/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 18:18:21.000000 story_protocol_python_sdk-0.1.1/src/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.727101 story_protocol_python_sdk-0.1.1/src/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 18:18:23.000000 story_protocol_python_sdk-0.1.1/src/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 18:18:23.000000 story_protocol_python_sdk-0.1.1/src/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.733176 story_protocol_python_sdk-0.1.1/src/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 18:18:20.000000 story_protocol_python_sdk-0.1.1/src/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 18:18:20.000000 story_protocol_python_sdk-0.1.1/src/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.739282 story_protocol_python_sdk-0.1.1/src/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 18:18:18.000000 story_protocol_python_sdk-0.1.1/src/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 18:18:18.000000 story_protocol_python_sdk-0.1.1/src/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.746186 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 18:18:25.000000 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 18:18:25.000000 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.752474 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 18:18:24.000000 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 18:18:24.000000 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.760111 story_protocol_python_sdk-0.1.1/src/resources/
--rw-rw-rw-   0        0        0     6641 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/resources/IPAsset.py
--rw-rw-rw-   0        0        0    15932 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/resources/License.py
--rw-rw-rw-   0        0        0    12213 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.770683 story_protocol_python_sdk-0.1.1/src/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7343 2024-05-21 18:16:50.000000 story_protocol_python_sdk-0.1.1/src/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5270 2024-05-21 18:18:06.000000 story_protocol_python_sdk-0.1.1/src/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1491 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.789295 story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      955 2024-05-21 18:54:50.000000 story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2024-05-21 18:54:50.000000 story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 18:54:50.000000 story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-21 18:54:50.000000 story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-05-21 18:54:50.000000 story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 18:54:50.795909 story_protocol_python_sdk-0.1.1/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.1/src/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.1/src/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.292609 story_protocol_python_sdk-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-14 01:32:03.000000 story_protocol_python_sdk-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      219 2024-05-21 20:55:29.000000 story_protocol_python_sdk-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      955 2024-05-21 20:59:56.288610 story_protocol_python_sdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:58:37.000000 story_protocol_python_sdk-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 20:59:56.292609 story_protocol_python_sdk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      927 2024-05-21 20:59:22.000000 story_protocol_python_sdk-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.092983 story_protocol_python_sdk-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.121479 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-21 18:30:08.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.161480 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.169478 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-21 18:18:17.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-21 18:18:17.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.173477 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-21 18:18:31.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.181478 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-21 18:18:21.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-21 18:18:21.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.189476 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-21 18:18:23.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-21 18:18:23.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.198543 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-21 18:18:20.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-21 18:18:20.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.220610 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-21 18:18:18.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-21 18:18:18.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.224607 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-21 18:18:25.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-21 18:18:25.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.232611 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-21 18:18:24.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-21 18:18:24.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.272610 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/
+-rw-rw-rw-   0        0        0     6729 2024-05-21 20:58:11.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    16042 2024-05-21 20:58:07.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/License.py
+-rw-rw-rw-   0        0        0    12301 2024-05-21 20:58:00.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.284613 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7343 2024-05-21 18:16:50.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5270 2024-05-21 18:18:06.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1557 2024-05-21 20:57:32.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.288610 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 18:29:02.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-21 17:37:13.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:59:56.157477 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      955 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2710 2024-05-21 20:59:56.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-21 20:59:55.000000 story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.1.1/LICENSE` & `story_protocol_python_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/PKG-INFO` & `story_protocol_python_sdk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.1/setup.py` & `story_protocol_python_sdk-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
+    include_package_data=True,  # Ensure package data is included
     url='https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install',
     license='MIT',
     author='Andrew Chung',
     author_email='andrew@storyprotocol.xyz',
     description='A Python SDK for interacting with the Story Protocol.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/resources/IPAsset.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #src/resources/IPAsset.py
 
 import logging
 from web3 import Web3
-from src.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
-from src.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
-from src.abi.LicenseToken.LicenseToken_client import LicenseTokenClient
-from src.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
+from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
+from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
+from story_protocol_python_sdk.abi.LicenseToken.LicenseToken_client import LicenseTokenClient
+from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 class IPAsset:
     def __init__(self, web3: Web3, account, chain_id):
```

### Comparing `story_protocol_python_sdk-0.1.1/src/resources/License.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/License.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from web3 import Web3
 from web3.exceptions import LogTopicError
 
-from src.abi.PILicenseTemplate.PILicenseTemplate_client import PILicenseTemplateClient
-from src.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
-from src.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
-from src.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
-from src.utils.license_terms import get_license_term_by_type, PIL_TYPE
+from story_protocol_python_sdk.abi.PILicenseTemplate.PILicenseTemplate_client import PILicenseTemplateClient
+from story_protocol_python_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
+from story_protocol_python_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
+from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
+from story_protocol_python_sdk.utils.license_terms import get_license_term_by_type, PIL_TYPE
 
 # Configure logging
 logging.basicConfig(level=logging.DEBUG)  # Set to DEBUG to capture all log messages
 logger = logging.getLogger(__name__)
 
 class License:
     def __init__(self, web3: Web3, account, chain_id):
```

### Comparing `story_protocol_python_sdk-0.1.1/src/resources/Royalty.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #src/resources/Royalty.py
 
 import logging
 from web3 import Web3
-from src.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
-from src.abi.IpRoyaltyVaultImpl.IpRoyaltyVaultImpl_client import IpRoyaltyVaultImplClient
-from src.abi.RoyaltyPolicyLAP.RoyaltyPolicyLAP_client import RoyaltyPolicyLAPClient
-from src.abi.RoyaltyModule.RoyaltyModule_client import RoyaltyModuleClient
+from story_protocol_python_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
+from story_protocol_python_sdk.abi.IpRoyaltyVaultImpl.IpRoyaltyVaultImpl_client import IpRoyaltyVaultImplClient
+from story_protocol_python_sdk.abi.RoyaltyPolicyLAP.RoyaltyPolicyLAP_client import RoyaltyPolicyLAPClient
+from story_protocol_python_sdk.abi.RoyaltyModule.RoyaltyModule_client import RoyaltyModuleClient
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 class Royalty:
     def __init__(self, web3: Web3, account, chain_id):
```

### Comparing `story_protocol_python_sdk-0.1.1/src/scripts/config.json` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/scripts/generate_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.1.1/src/story_client.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/story_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # Ensure the src directory is in the Python path
 current_dir = os.path.dirname(__file__)
 src_path = os.path.abspath(os.path.join(current_dir, '..'))
 if src_path not in sys.path:
     sys.path.append(src_path)
 
-from src.resources.IPAsset import IPAsset
-from src.resources.License import License
-from src.resources.Royalty import Royalty
+from story_protocol_python_sdk.resources.IPAsset import IPAsset
+from story_protocol_python_sdk.resources.License import License
+from story_protocol_python_sdk.resources.Royalty import Royalty
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 class StoryClient:
     def __init__(self, web3, account, chain_id):
```

### Comparing `story_protocol_python_sdk-0.1.1/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story-protocol-python-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.1.1/src/utils/license_terms.py` & `story_protocol_python_sdk-0.1.2/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

