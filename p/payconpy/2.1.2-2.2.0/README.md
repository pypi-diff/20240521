# Comparing `tmp/payconpy-2.1.2.tar.gz` & `tmp/payconpy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-2.1.2.tar", last modified: Mon May 13 20:37:10 2024, max compression
+gzip compressed data, was "payconpy-2.2.0.tar", last modified: Tue May 21 14:28:39 2024, max compression
```

## Comparing `payconpy-2.1.2.tar` & `payconpy-2.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.126229 payconpy-2.1.2/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.1.2/LICENSE
--rw-rw-rw-   0        0        0      899 2024-05-13 20:37:10.121486 payconpy-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.794518 payconpy-2.1.2/payconpy/
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.887333 payconpy-2.1.2/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.1.2/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.1.2/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.910264 payconpy-2.1.2/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.918010 payconpy-2.1.2/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.934283 payconpy-2.1.2/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.1.2/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    11597 2024-05-09 12:27:06.000000 payconpy-2.1.2/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.952263 payconpy-2.1.2/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.1.2/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.970352 payconpy-2.1.2/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.1.2/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.984990 payconpy-2.1.2/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.1.2/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.002048 payconpy-2.1.2/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.1.2/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.015445 payconpy-2.1.2/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.1.2/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.1.2/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.031048 payconpy-2.1.2/payconpy/odoo/
--rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.1.2/payconpy/odoo/__init__.py
--rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.1.2/payconpy/odoo/odoo_xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.054770 payconpy-2.1.2/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.2/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.067902 payconpy-2.1.2/payconpy/openai/apis/
--rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.1.2/payconpy/openai/apis/__init__.py
--rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.1.2/payconpy/openai/apis/apis.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.087158 payconpy-2.1.2/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.2/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.1.2/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.1.2/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:10.109961 payconpy-2.1.2/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.1.2/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   147726 2024-04-22 17:45:30.000000 payconpy-2.1.2/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 20:37:09.866217 payconpy-2.1.2/payconpy.egg-info/
--rw-rw-rw-   0        0        0      899 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      202 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      261 2024-05-13 20:37:08.000000 payconpy-2.1.2/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 20:37:10.126229 payconpy-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2049 2024-05-13 20:36:54.000000 payconpy-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:39.001614 payconpy-2.2.0/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0      920 2024-05-21 14:28:38.997311 payconpy-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.566334 payconpy-2.2.0/payconpy/
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.697411 payconpy-2.2.0/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.0/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.0/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.733703 payconpy-2.2.0/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.745331 payconpy-2.2.0/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.758402 payconpy-2.2.0/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.0/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.0/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.773180 payconpy-2.2.0/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.0/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.803471 payconpy-2.2.0/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.0/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.835330 payconpy-2.2.0/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.2.0/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.857219 payconpy-2.2.0/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.0/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.883751 payconpy-2.2.0/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.0/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.0/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.900819 payconpy-2.2.0/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.0/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.0/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.928147 payconpy-2.2.0/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.0/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.942894 payconpy-2.2.0/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.0/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.0/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.966015 payconpy-2.2.0/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.0/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.0/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.0/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.986075 payconpy-2.2.0/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.0/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   147726 2024-04-22 17:45:30.000000 payconpy-2.2.0/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:28:38.680312 payconpy-2.2.0/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      920 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-05-21 14:28:37.000000 payconpy-2.2.0/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:28:39.001614 payconpy-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2093 2024-05-21 14:28:20.000000 payconpy-2.2.0/setup.py
```

### Comparing `payconpy-2.1.2/LICENSE` & `payconpy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/PKG-INFO` & `payconpy-2.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.1.2
+Version: 2.2.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
 Provides-Extra: openai
+Provides-Extra: gui
 License-File: LICENSE
 
 # payconpy - Funcoes para automatizar criação de sistemas Python
 
 ## pip install payconpy | NECESSARIO PYTHON 3.10
 
 Aqui voce achara funcoes produzidas para ter maior agilidade nos desenvolvimentos nas tecnologias abaixo:
```

### Comparing `payconpy-2.1.2/payconpy/femails/femails.py` & `payconpy-2.2.0/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/fexceptions/exceptions.py` & `payconpy-2.2.0/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/fpdf/focr/orc.py` & `payconpy-2.2.0/payconpy/fpdf/focr/orc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from payconpy.fpython.fpython import *
-from payconpy.fpdf.pdfutils.pdfutils import split_pdf
-from payconpy.utils.utils import download_file_from_github
 from tqdm import tqdm
 from PIL import Image
 import numpy as np
-import fitz, uuid, os, gdown, pytesseract, cv2, base64
+import fitz, uuid, os, pytesseract, base64
 
 def faz_ocr_em_pdf_offline(path_pdf: str, export_from_file_txt: str = False) -> str:
     """
     Converte pdf(s) em texto com fitz (PyMuPDF)
         
     Atenção, só funciona corretamente em PDF's que o texto é selecionável!
     
@@ -169,30 +167,19 @@
         Exception: Pode lançar uma exceção se ocorrer um erro durante o download dos binários, o processamento OCR ou se a integridade do arquivo baixado for questionável.
     """
     path_exit = arquivo_com_caminho_absoluto('temp_tess', 'Tesseract-OCR.zip')
     path_tesseract_extract = arquivo_com_caminho_absoluto('bin', 'Tesseract-OCR')
     path_tesseract = arquivo_com_caminho_absoluto(('bin', 'Tesseract-OCR'), 'tesseract.exe')
 
     if not os.path.exists(path_tesseract):
-        faz_log('Baixando binários do Tesseract, aguarde...')
-        cria_dir_no_dir_de_trabalho_atual('temp_tess')
-        cria_dir_no_dir_de_trabalho_atual('bin')
-        download_file_from_github('https://github.com/Paycon-Automacoes/payconpy/raw/main/tesseract_bin_pt.zip', path_exit)
-        sleep(1)
-        with zipfile.ZipFile(path_exit, 'r') as zip_ref:
-            # Obtém o nome da pasta interna dentro do arquivo ZIP
-            zip_info = zip_ref.infolist()[0]
-            folder_name = zip_info.filename.split("/")[0]
-
-            # Extrai o conteúdo da pasta interna para a pasta de destino
-            for file_info in zip_ref.infolist():
-                if file_info.filename.startswith(f"{folder_name}/"):
-                    file_info.filename = file_info.filename.replace(f"{folder_name}/", "", 1)
-                    zip_ref.extract(file_info, path_tesseract_extract)
-        deleta_diretorio('temp_tess')
+        while not os.path.exists(path_tesseract):
+            faz_log('*** COLOQUE OS BINÁRIOS DO TESSERACT NA PASTA BIN (O NOME DA PASTA DOS BINÁRIOS DEVE SER "Tesseract-OCR") ***')
+            sleep(10)
+        else:
+            pass
     pytesseract.pytesseract.tesseract_cmd = path_tesseract
 
     with fitz.open(pdf) as pdf_fitz:
         cria_dir_no_dir_de_trabalho_atual('pages')
         limpa_diretorio('pages')
         faz_log(f'Convertendo PDF para páginas...')
         number_of_pages = len(pdf_fitz) if limit_pages is None else min(limit_pages, len(pdf_fitz))
```

### Comparing `payconpy-2.1.2/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-2.2.0/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.2.0/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/fpython/fpython.py` & `payconpy-2.2.0/payconpy/fpython/fpython.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/fregex/fregex.py` & `payconpy-2.2.0/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/fselenium/fselenium.py` & `payconpy-2.2.0/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/odoo/odoo_xmlrpc.py` & `payconpy-2.2.0/payconpy/odoo/odoo_xmlrpc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/openai/apis/apis.py` & `payconpy-2.2.0/payconpy/openai/apis/apis.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/openai/assistants/assistants.py` & `payconpy-2.2.0/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/openai/get_cost.py` & `payconpy-2.2.0/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy/utils/utils.py` & `payconpy-2.2.0/payconpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/payconpy.egg-info/PKG-INFO` & `payconpy-2.2.0/payconpy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.1.2
+Version: 2.2.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
 Provides-Extra: openai
+Provides-Extra: gui
 License-File: LICENSE
 
 # payconpy - Funcoes para automatizar criação de sistemas Python
 
 ## pip install payconpy | NECESSARIO PYTHON 3.10
 
 Aqui voce achara funcoes produzidas para ter maior agilidade nos desenvolvimentos nas tecnologias abaixo:
```

### Comparing `payconpy-2.1.2/payconpy.egg-info/SOURCES.txt` & `payconpy-2.2.0/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-2.1.2/setup.py` & `payconpy-2.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '2.1.2'
+version = '2.2.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
@@ -37,24 +37,27 @@
         install_requires= [
             'selenium',
             'bs4',
             'requests',
             'html5lib',
             'webdriver-manager',
             'pretty-html-table',
-            'PySimpleGUI==4.60.0',
             'xlsxwriter',
             'pandas',
             'sqlalchemy',
             'rich',
-            'pyinstaller==5.12.0',
+            'pyinstaller',
             # for ocr
-            'opencv-python==4.8.1.78',
             'pytesseract',
+            'tqdm',
+            'pillow',
             'PyMuPDF',
         ],
         extras_require={
             'openai': [ # for chatpdf
                 'openai',
             ],
+            'gui': [ # for chatpdf
+                'PySimpleGUI',
+            ],
     },
 )
```

