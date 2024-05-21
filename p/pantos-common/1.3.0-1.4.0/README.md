# Comparing `tmp/pantos_common-1.3.0.tar.gz` & `tmp/pantos_common-1.4.0.tar.gz`

## Comparing `pantos_common-1.3.0.tar` & `pantos_common-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:14.000000 ./
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:14.000000 ./pantos_common-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos-logo-full.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-20 13:24:08.000000 ./pantos_common-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-05-20 13:24:14.000000 ./pantos_common-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:14.000000 ./pantos_common-1.3.0/pantos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:14.000000 ./pantos_common-1.3.0/pantos/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:14.000000 ./pantos_common-1.3.0/pantos/common/blockchains/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/cronos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/solana.py
--rw-r--r--   0 runner    (1001) docker     (127)    19287 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/ethereum.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/avalanche.py
--rw-r--r--   0 runner    (1001) docker     (127)    41291 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/bnbchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/fantom.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/celo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:14.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_pantos_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_standard_token.abi
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_pantos_hub.abi
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi
--rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/servicenodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/restapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-20 13:24:07.000000 ./pantos_common-1.3.0/pantos/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:27.000000 ./
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:27.000000 ./pantos_common-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-21 15:11:27.000000 ./pantos_common-1.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:27.000000 ./pantos_common-1.4.0/pantos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:27.000000 ./pantos_common-1.4.0/pantos/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:27.000000 ./pantos_common-1.4.0/pantos/common/blockchains/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/cronos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/solana.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19287 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/ethereum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/avalanche.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41291 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/bnbchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/fantom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/celo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:27.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_pantos_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_standard_token.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_pantos_hub.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/servicenodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/restapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-21 15:11:18.000000 ./pantos_common-1.4.0/pantos/common/exceptions.py
```

### Comparing `./pantos_common-1.3.0/README.md` & `./pantos_common-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="pantos-logo-full.svg" alt="Pantos logo" align="right" width="120" />
+<img src="https://raw.githubusercontent.com/pantos-io/common/img/pantos-logo-full.svg" alt="Pantos logo" align="right" width="120" />
 
 [![CI](https://github.com/pantos-io/common/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/pantos-io/common/actions/workflows/ci.yaml) 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=pantos-io_common&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=pantos-io_common)
 
 # Common code for Pantos off-chain components
 
 ## 1. Introduction
```

### Comparing `./pantos_common-1.3.0/LICENSE.md` & `./pantos_common-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pyproject.toml` & `./pantos_common-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [tool.poetry]
 name = "pantos-common"
-version = "1.3.0"
+version = "1.4.0"
 description = "Common code for Pantos off-chain components."
 authors = ["Pantos GmbH <contact@pantos.io>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://pantos.io"
 repository = "https://github.com/pantos-io/common"
 packages = [
-    { include = "pantos" },
-    { include = "pantos-logo-full.svg" }
+    { include = "pantos" }
 ]
 
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["pantos"]
+namespaces = true
+
 [tool.poetry.group.test.dependencies]
 pytest = "7.4.0"
 pytest-cov = "4.1.0"
 web3 = {extras = ["tester"], version = "^6.5.0"}
 
 [tool.poetry.group.lint.dependencies]
 bandit = "1.7.5"
@@ -32,15 +36,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 celery = "5.3.1"
 Cerberus = "1.3.4"
 Flask-RESTful = "0.3.10"
 JSON-log-formatter = "0.5.2"
 PyYAML = "6.0.1"
-requests = "2.31.0"
+requests = "2.32.0"
 web3 = "6.5.0"
 pyaml-env = "1.2.1"
 python-dotenv = "1.0.1"
 pycryptodome = "3.20.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `./pantos_common-1.3.0/PKG-INFO` & `./pantos_common-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantos-common
-Version: 1.3.0
+Version: 1.4.0
 Summary: Common code for Pantos off-chain components.
 Home-page: https://pantos.io
 License: GPL-3.0-only
 Author: Pantos GmbH
 Author-email: contact@pantos.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: celery (==5.3.1) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: cerberus (==1.3.4) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: flask-restful (==0.3.10) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: json-log-formatter (==0.5.2) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: pyyaml (==6.0.1) ; python_version >= "3.10" and python_version < "4.0"
-Requires-Dist: requests (==2.31.0) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: requests (==2.32.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: web3 (==6.5.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: pyaml-env (==1.2.1) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: python-dotenv (==1.0.1) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: pycryptodome (==3.20.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: billiard (==4.2.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: click (==8.1.7) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: click-didyoumean (==0.3.1) ; python_version >= "3.10" and python_version < "4.0"
@@ -80,15 +80,15 @@
 Requires-Dist: rpds-py (==0.18.0) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: wcwidth (==0.2.13) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: markupsafe (==2.1.5) ; python_version >= "3.10" and python_version < "4.0"
 Requires-Dist: regex (==2024.4.28) ; python_version >= "3.10" and python_version < "4"
 Project-URL: Repository, https://github.com/pantos-io/common
 Description-Content-Type: text/markdown
 
-<img src="pantos-logo-full.svg" alt="Pantos logo" align="right" width="120" />
+<img src="https://raw.githubusercontent.com/pantos-io/common/img/pantos-logo-full.svg" alt="Pantos logo" align="right" width="120" />
 
 [![CI](https://github.com/pantos-io/common/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/pantos-io/common/actions/workflows/ci.yaml) 
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=pantos-io_common&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=pantos-io_common)
 
 # Common code for Pantos off-chain components
 
 ## 1. Introduction
```

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/tasks.py` & `./pantos_common-1.4.0/pantos/common/blockchains/tasks.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/polygon.py` & `./pantos_common-1.4.0/pantos/common/blockchains/polygon.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/cronos.py` & `./pantos_common-1.4.0/pantos/common/blockchains/cronos.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/solana.py` & `./pantos_common-1.4.0/pantos/common/blockchains/solana.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/ethereum.py` & `./pantos_common-1.4.0/pantos/common/blockchains/ethereum.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/avalanche.py` & `./pantos_common-1.4.0/pantos/common/blockchains/avalanche.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/base.py` & `./pantos_common-1.4.0/pantos/common/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/factory.py` & `./pantos_common-1.4.0/pantos/common/blockchains/factory.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/bnbchain.py` & `./pantos_common-1.4.0/pantos/common/blockchains/bnbchain.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/enums.py` & `./pantos_common-1.4.0/pantos/common/blockchains/enums.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/fantom.py` & `./pantos_common-1.4.0/pantos/common/blockchains/fantom.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/celo.py` & `./pantos_common-1.4.0/pantos/common/blockchains/celo.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/polygon_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/polygon_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/celo_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/celo_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/bnb_chain_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/bnb_chain_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/fantom_pantos_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/fantom_pantos_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/ethereum_standard_token.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/ethereum_standard_token.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/cronos_pantos_hub.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/cronos_pantos_hub.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi` & `./pantos_common-1.4.0/pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/servicenodes.py` & `./pantos_common-1.4.0/pantos/common/servicenodes.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/restapi.py` & `./pantos_common-1.4.0/pantos/common/restapi.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/entities.py` & `./pantos_common-1.4.0/pantos/common/entities.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/logging.py` & `./pantos_common-1.4.0/pantos/common/logging.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/configuration.py` & `./pantos_common-1.4.0/pantos/common/configuration.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/signer.py` & `./pantos_common-1.4.0/pantos/common/signer.py`

 * *Files identical despite different names*

### Comparing `./pantos_common-1.3.0/pantos/common/exceptions.py` & `./pantos_common-1.4.0/pantos/common/exceptions.py`

 * *Files identical despite different names*

