# Comparing `tmp/tester_story_sdk-0.1.0.tar.gz` & `tmp/tester_story_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tester_story_sdk-0.1.0.tar", last modified: Tue May 21 20:23:32 2024, max compression
+gzip compressed data, was "tester_story_sdk-0.1.1.tar", last modified: Tue May 21 20:31:47 2024, max compression
```

## Comparing `tester_story_sdk-0.1.0.tar` & `tester_story_sdk-0.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.222775 tester_story_sdk-0.1.0/
--rw-rw-rw-   0        0        0     1092 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      160 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      946 2024-05-21 20:23:32.219776 tester_story_sdk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/README.md
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:23:32.222775 tester_story_sdk-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-05-21 20:23:08.000000 tester_story_sdk-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:31.979320 tester_story_sdk-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:31.999321 tester_story_sdk-0.1.0/src/tester_story_sdk/
--rw-rw-rw-   0        0        0      221 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.028320 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.040320 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IPAssetRegistry/
--rw-rw-rw-   0        0        0    13409 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-rw-rw-   0        0        0     4546 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IPAssetRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.052320 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/
--rw-rw-rw-   0        0        0    16117 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-rw-rw-   0        0        0     1761 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.063319 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseRegistry/
--rw-rw-rw-   0        0        0    26905 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-rw-rw-   0        0        0     4230 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseRegistry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.074331 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseToken/
--rw-rw-rw-   0        0        0    23007 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseToken/LicenseToken.json
--rw-rw-rw-   0        0        0     1159 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseToken/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.085331 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicensingModule/
--rw-rw-rw-   0        0        0    19697 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicensingModule/LicensingModule.json
--rw-rw-rw-   0        0        0     5246 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicensingModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.095418 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/PILicenseTemplate/
--rw-rw-rw-   0        0        0    26246 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-rw-rw-   0        0        0     4625 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/PILicenseTemplate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.114775 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyModule/
--rw-rw-rw-   0        0        0    16029 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-rw-rw-   0        0        0     1489 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyModule/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.151774 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyPolicyLAP/
--rw-rw-rw-   0        0        0    14037 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-rw-rw-   0        0        0     1183 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/abi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.172774 tester_story_sdk-0.1.0/src/tester_story_sdk/resources/
--rw-rw-rw-   0        0        0     6641 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/resources/IPAsset.py
--rw-rw-rw-   0        0        0    15932 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/resources/License.py
--rw-rw-rw-   0        0        0    12213 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/resources/Royalty.py
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.214774 tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0     3539 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/config.json
--rw-rw-rw-   0        0        0      426 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/config_impl.json
--rw-rw-rw-   0        0        0     7343 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/generate_client.py
--rw-rw-rw-   0        0        0     5270 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/generate_client_impl.py
--rw-rw-rw-   0        0        0     1491 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/story_client.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.217774 tester_story_sdk-0.1.0/src/tester_story_sdk/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0     2444 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.0/src/tester_story_sdk/utils/license_terms.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:23:32.027321 tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/
--rw-rw-rw-   0        0        0      946 2024-05-21 20:23:31.000000 tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2323 2024-05-21 20:23:31.000000 tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:23:31.000000 tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-21 20:23:31.000000 tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-21 20:23:31.000000 tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.644238 tester_story_sdk-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      160 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      946 2024-05-21 20:31:47.644238 tester_story_sdk-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/README.md
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 20:31:47.644238 tester_story_sdk-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-05-21 20:31:45.000000 tester_story_sdk-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.500240 tester_story_sdk-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.520242 tester_story_sdk-0.1.1/src/tester_story_sdk/
+-rw-rw-rw-   0        0        0      221 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.548236 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.556240 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IPAssetRegistry/
+-rw-rw-rw-   0        0        0    13409 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-rw-rw-   0        0        0     4546 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IPAssetRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.560239 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/
+-rw-rw-rw-   0        0        0    16117 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-rw-rw-   0        0        0     1761 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.568243 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseRegistry/
+-rw-rw-rw-   0        0        0    26905 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-rw-rw-   0        0        0     4230 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseRegistry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.576242 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseToken/
+-rw-rw-rw-   0        0        0    23007 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseToken/LicenseToken.json
+-rw-rw-rw-   0        0        0     1159 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseToken/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.580239 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicensingModule/
+-rw-rw-rw-   0        0        0    19697 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicensingModule/LicensingModule.json
+-rw-rw-rw-   0        0        0     5246 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicensingModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.588238 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/PILicenseTemplate/
+-rw-rw-rw-   0        0        0    26246 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-rw-rw-   0        0        0     4625 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/PILicenseTemplate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.596239 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyModule/
+-rw-rw-rw-   0        0        0    16029 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-rw-rw-   0        0        0     1489 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyModule/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.600237 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyPolicyLAP/
+-rw-rw-rw-   0        0        0    14037 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-rw-rw-   0        0        0     1183 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/abi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.628245 tester_story_sdk-0.1.1/src/tester_story_sdk/resources/
+-rw-rw-rw-   0        0        0     6709 2024-05-21 20:31:36.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/resources/IPAsset.py
+-rw-rw-rw-   0        0        0    15932 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/resources/License.py
+-rw-rw-rw-   0        0        0    12213 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/resources/Royalty.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.636239 tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0     3539 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/config.json
+-rw-rw-rw-   0        0        0      426 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/config_impl.json
+-rw-rw-rw-   0        0        0     7343 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/generate_client.py
+-rw-rw-rw-   0        0        0     5270 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/generate_client_impl.py
+-rw-rw-rw-   0        0        0     1491 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/story_client.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.640236 tester_story_sdk-0.1.1/src/tester_story_sdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     2444 2024-05-21 20:20:23.000000 tester_story_sdk-0.1.1/src/tester_story_sdk/utils/license_terms.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:31:47.548236 tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/
+-rw-rw-rw-   0        0        0      946 2024-05-21 20:31:47.000000 tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2323 2024-05-21 20:31:47.000000 tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 20:31:47.000000 tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-21 20:31:47.000000 tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-21 20:31:47.000000 tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/top_level.txt
```

### Comparing `tester_story_sdk-0.1.0/LICENSE` & `tester_story_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/PKG-INFO` & `tester_story_sdk-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tester_story_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tester_story_sdk-0.1.0/setup.py` & `tester_story_sdk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tester_story_sdk',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
```

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseToken/LicenseToken.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicenseToken/LicenseToken_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicensingModule/LicensingModule.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/LicensingModule/LicensingModule_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/resources/IPAsset.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/resources/IPAsset.py`

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
+from src.tester_story_sdk.abi.IPAssetRegistry.IPAssetRegistry_client import IPAssetRegistryClient
+from src.tester_story_sdk.abi.LicensingModule.LicensingModule_client import LicensingModuleClient
+from src.tester_story_sdk.abi.LicenseToken.LicenseToken_client import LicenseTokenClient
+from src.tester_story_sdk.abi.LicenseRegistry.LicenseRegistry_client import LicenseRegistryClient
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 class IPAsset:
     def __init__(self, web3: Web3, account, chain_id):
```

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/resources/License.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/resources/License.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/resources/Royalty.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/resources/Royalty.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/config.json` & `tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/generate_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/scripts/generate_client_impl.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/story_client.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk/utils/license_terms.py` & `tester_story_sdk-0.1.1/src/tester_story_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/PKG-INFO` & `tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tester-story-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/aandrewchung/python-sdk/tree/andrew/pip-install
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tester_story_sdk-0.1.0/src/tester_story_sdk.egg-info/SOURCES.txt` & `tester_story_sdk-0.1.1/src/tester_story_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

