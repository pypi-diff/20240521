# Comparing `tmp/BarteSDK-0.1.4.tar.gz` & `tmp/BarteSDK-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-0.1.4.tar", last modified: Mon May 20 18:14:04 2024, max compression
+gzip compressed data, was "BarteSDK-0.1.5.tar", last modified: Mon May 20 21:33:29 2024, max compression
```

## Comparing `BarteSDK-0.1.4.tar` & `BarteSDK-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.005409 BarteSDK-0.1.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.001409 BarteSDK-0.1.4/BarteChargesAPI/
--rw-rw-r--   0 root         (0) root         (0)       34 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteChargesAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      405 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteChargesAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.001409 BarteSDK-0.1.4/BarteReportAPI/
--rw-rw-r--   0 root         (0) root         (0)       33 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteReportAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      718 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/BarteReportAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 18:14:04.001409 BarteSDK-0.1.4/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4072 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 18:14:03.000000 BarteSDK-0.1.4/BarteSDK.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4072 2024-05-20 18:14:04.005409 BarteSDK-0.1.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3796 2024-05-20 18:13:34.000000 BarteSDK-0.1.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 18:14:04.005409 BarteSDK-0.1.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      562 2024-05-20 18:13:42.000000 BarteSDK-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.252346 BarteSDK-0.1.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/BarteChargesAPI/
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/BarteChargesAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/BarteChargesAPI/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-20 21:33:29.000000 BarteSDK-0.1.5/BarteSDK.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:33:29.248345 BarteSDK-0.1.5/reportsellers/
+-rw-rw-r--   0 root         (0) root         (0)       32 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/reportsellers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      719 2024-05-20 21:33:08.000000 BarteSDK-0.1.5/reportsellers/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 21:33:29.252346 BarteSDK-0.1.5/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-20 21:33:11.000000 BarteSDK-0.1.5/setup.py
```

### Comparing `BarteSDK-0.1.4/BarteReportAPI/main.py` & `BarteSDK-0.1.5/reportsellers/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 
-class BarteReportAPI:
+class reportsellers:
     def __init__(self, api_key):
         self.api_key = api_key
         self.base_url = 'https://api2.barte.com/function/report-sellers'
 
-    def send_report(self, query_file, recipient_email, id_seller, report_name, days_ago):
+    def reportsellers(self, query_file, recipient_email, id_seller, report_name, days_ago):
         headers = {
             'x-api-key': self.api_key,
             'Content-Type': 'application/json'
         }
         payload = {
             'query_file': query_file,
             'recipient_email': recipient_email,
```

### Comparing `BarteSDK-0.1.4/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-0.1.5/BarteSDK.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1.4
+Version: 0.1.5
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,26 +61,26 @@
 from BarteReportAPI import BarteReportAPI
 
 # Crie uma instância da classe com os parâmetros necessários
 api_key = "inserir-token"
 api_client = BarteReportAPI(api_key)
 
 # Faça chamadas aos métodos definidos
-response = api_client.send_report(
+response = api_client.reportsellers(
     query_file='cobrancas-completo.sql',
     recipient_email='e-mail@barte.com',
     id_seller='1111',
     report_name='Vendas',
     days_ago='7'
 )
 
 # Imprima a resposta ou faça outras operações com ela
 print(response)
 ```
 
-### Parâmetros do Método `send_report`
+### Parâmetros do Método `reportsellers`
 
 - `query_file`: Nome do arquivo SQL que contém a query para gerar o relatório.
 - `recipient_email`: Endereço de e-mail do Seller que receberá o relatório.
 - `id_seller`: Identificação do Seller para quem o relatório é destinado.
 - `report_name`: Título amigável do relatório, que será usado no título do e-mail.
 - `days_ago`: Número de dias retroativos para geração do relatório.
```

### Comparing `BarteSDK-0.1.4/PKG-INFO` & `BarteSDK-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1.4
+Version: 0.1.5
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -61,26 +61,26 @@
 from BarteReportAPI import BarteReportAPI
 
 # Crie uma instância da classe com os parâmetros necessários
 api_key = "inserir-token"
 api_client = BarteReportAPI(api_key)
 
 # Faça chamadas aos métodos definidos
-response = api_client.send_report(
+response = api_client.reportsellers(
     query_file='cobrancas-completo.sql',
     recipient_email='e-mail@barte.com',
     id_seller='1111',
     report_name='Vendas',
     days_ago='7'
 )
 
 # Imprima a resposta ou faça outras operações com ela
 print(response)
 ```
 
-### Parâmetros do Método `send_report`
+### Parâmetros do Método `reportsellers`
 
 - `query_file`: Nome do arquivo SQL que contém a query para gerar o relatório.
 - `recipient_email`: Endereço de e-mail do Seller que receberá o relatório.
 - `id_seller`: Identificação do Seller para quem o relatório é destinado.
 - `report_name`: Título amigável do relatório, que será usado no título do e-mail.
 - `days_ago`: Número de dias retroativos para geração do relatório.
```

### Comparing `BarteSDK-0.1.4/README.md` & `BarteSDK-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,26 +50,26 @@
 from BarteReportAPI import BarteReportAPI
 
 # Crie uma instância da classe com os parâmetros necessários
 api_key = "inserir-token"
 api_client = BarteReportAPI(api_key)
 
 # Faça chamadas aos métodos definidos
-response = api_client.send_report(
+response = api_client.reportsellers(
     query_file='cobrancas-completo.sql',
     recipient_email='e-mail@barte.com',
     id_seller='1111',
     report_name='Vendas',
     days_ago='7'
 )
 
 # Imprima a resposta ou faça outras operações com ela
 print(response)
 ```
 
-### Parâmetros do Método `send_report`
+### Parâmetros do Método `reportsellers`
 
 - `query_file`: Nome do arquivo SQL que contém a query para gerar o relatório.
 - `recipient_email`: Endereço de e-mail do Seller que receberá o relatório.
 - `id_seller`: Identificação do Seller para quem o relatório é destinado.
 - `report_name`: Título amigável do relatório, que será usado no título do e-mail.
 - `days_ago`: Número de dias retroativos para geração do relatório.
```

### Comparing `BarteSDK-0.1.4/setup.py` & `BarteSDK-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

