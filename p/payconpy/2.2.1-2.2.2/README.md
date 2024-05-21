# Comparing `tmp/payconpy-2.2.1.tar.gz` & `tmp/payconpy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payconpy-2.2.1.tar", last modified: Tue May 21 14:36:22 2024, max compression
+gzip compressed data, was "payconpy-2.2.2.tar", last modified: Tue May 21 15:15:18 2024, max compression
```

## Comparing `payconpy-2.2.1.tar` & `payconpy-2.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.516488 payconpy-2.2.1/
--rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.1/LICENSE
--rw-rw-rw-   0        0        0      920 2024-05-21 14:36:22.509534 payconpy-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.224937 payconpy-2.2.1/payconpy/
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.294963 payconpy-2.2.1/payconpy/femails/
--rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.1/payconpy/femails/__init__.py
--rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.1/payconpy/femails/femails.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.309196 payconpy-2.2.1/payconpy/fexceptions/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.316289 payconpy-2.2.1/payconpy/fpdf/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.332482 payconpy-2.2.1/payconpy/fpdf/focr/
--rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.1/payconpy/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.1/payconpy/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.361816 payconpy-2.2.1/payconpy/fpdf/pdfutils/
--rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpdf/pdfutils/__init__.py
--rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.1/payconpy/fpdf/pdfutils/pdfutils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.376094 payconpy-2.2.1/payconpy/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.1/payconpy/fpysimplegui/fpysimplegui.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.389529 payconpy-2.2.1/payconpy/fpython/
--rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fpython/__init__.py
--rw-rw-rw-   0        0        0    57479 2024-04-21 19:22:58.000000 payconpy-2.2.1/payconpy/fpython/fpython.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.407232 payconpy-2.2.1/payconpy/fregex/
--rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fregex/__init__.py
--rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.1/payconpy/fregex/fregex.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.420760 payconpy-2.2.1/payconpy/fselenium/
--rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.1/payconpy/fselenium/__init__.py
--rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.1/payconpy/fselenium/fselenium.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.433200 payconpy-2.2.1/payconpy/odoo/
--rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.1/payconpy/odoo/__init__.py
--rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.1/payconpy/odoo/odoo_xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.450056 payconpy-2.2.1/payconpy/openai/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.1/payconpy/openai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.461006 payconpy-2.2.1/payconpy/openai/apis/
--rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.1/payconpy/openai/apis/__init__.py
--rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.1/payconpy/openai/apis/apis.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.479353 payconpy-2.2.1/payconpy/openai/assistants/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.1/payconpy/openai/assistants/__init__.py
--rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.1/payconpy/openai/assistants/assistants.py
--rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.1/payconpy/openai/get_cost.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.496783 payconpy-2.2.1/payconpy/utils/
--rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.1/payconpy/utils/__init__.py
--rw-rw-rw-   0        0        0   195592 2024-05-21 14:36:04.000000 payconpy-2.2.1/payconpy/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:36:22.282790 payconpy-2.2.1/payconpy.egg-info/
--rw-rw-rw-   0        0        0      920 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-05-21 14:36:22.000000 payconpy-2.2.1/payconpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      261 2024-05-21 14:36:21.000000 payconpy-2.2.1/payconpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 14:36:22.517513 payconpy-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2093 2024-05-21 14:36:12.000000 payconpy-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.417829 payconpy-2.2.2/
+-rw-rw-rw-   0        0        0     1073 2024-03-28 18:34:30.000000 payconpy-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0      920 2024-05-21 15:15:18.411279 payconpy-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2024-04-21 22:27:53.000000 payconpy-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:17.890278 payconpy-2.2.2/payconpy/
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.024371 payconpy-2.2.2/payconpy/femails/
+-rw-rw-rw-   0        0        0       40 2024-03-28 18:29:40.000000 payconpy-2.2.2/payconpy/femails/__init__.py
+-rw-rw-rw-   0        0        0     7021 2024-03-28 18:29:45.000000 payconpy-2.2.2/payconpy/femails/femails.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.044769 payconpy-2.2.2/payconpy/fexceptions/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.056142 payconpy-2.2.2/payconpy/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.072878 payconpy-2.2.2/payconpy/fpdf/focr/
+-rw-rw-rw-   0        0        0      104 2024-03-28 18:29:53.000000 payconpy-2.2.2/payconpy/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0    10766 2024-05-21 14:26:58.000000 payconpy-2.2.2/payconpy/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.089242 payconpy-2.2.2/payconpy/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     5758 2024-04-21 19:13:23.000000 payconpy-2.2.2/payconpy/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.109237 payconpy-2.2.2/payconpy/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4676 2024-03-28 17:58:49.000000 payconpy-2.2.2/payconpy/fpysimplegui/fpysimplegui.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.129547 payconpy-2.2.2/payconpy/fpython/
+-rw-rw-rw-   0        0        0       25 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fpython/__init__.py
+-rw-rw-rw-   0        0        0    56910 2024-05-21 15:14:57.000000 payconpy-2.2.2/payconpy/fpython/fpython.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.187835 payconpy-2.2.2/payconpy/fregex/
+-rw-rw-rw-   0        0        0       24 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10366 2024-03-28 17:52:21.000000 payconpy-2.2.2/payconpy/fregex/fregex.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.241729 payconpy-2.2.2/payconpy/fselenium/
+-rw-rw-rw-   0        0        0       27 2023-09-12 12:27:01.000000 payconpy-2.2.2/payconpy/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    40190 2024-03-28 20:51:18.000000 payconpy-2.2.2/payconpy/fselenium/fselenium.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.278336 payconpy-2.2.2/payconpy/odoo/
+-rw-rw-rw-   0        0        0        0 2024-04-21 19:01:38.000000 payconpy-2.2.2/payconpy/odoo/__init__.py
+-rw-rw-rw-   0        0        0    11717 2024-05-13 20:36:27.000000 payconpy-2.2.2/payconpy/odoo/odoo_xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.311315 payconpy-2.2.2/payconpy/openai/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.2/payconpy/openai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.328970 payconpy-2.2.2/payconpy/openai/apis/
+-rw-rw-rw-   0        0        0        0 2024-04-21 21:37:31.000000 payconpy-2.2.2/payconpy/openai/apis/__init__.py
+-rw-rw-rw-   0        0        0     3192 2024-04-21 21:37:47.000000 payconpy-2.2.2/payconpy/openai/apis/apis.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.360531 payconpy-2.2.2/payconpy/openai/assistants/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.2/payconpy/openai/assistants/__init__.py
+-rw-rw-rw-   0        0        0     4085 2023-11-27 13:03:14.000000 payconpy-2.2.2/payconpy/openai/assistants/assistants.py
+-rw-rw-rw-   0        0        0     4427 2023-11-27 14:53:41.000000 payconpy-2.2.2/payconpy/openai/get_cost.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.396149 payconpy-2.2.2/payconpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-27 12:53:25.000000 payconpy-2.2.2/payconpy/utils/__init__.py
+-rw-rw-rw-   0        0        0   195592 2024-05-21 14:36:04.000000 payconpy-2.2.2/payconpy/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:15:18.007547 payconpy-2.2.2/payconpy.egg-info/
+-rw-rw-rw-   0        0        0      920 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      261 2024-05-21 15:15:17.000000 payconpy-2.2.2/payconpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:15:18.421159 payconpy-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2093 2024-05-21 15:15:11.000000 payconpy-2.2.2/setup.py
```

### Comparing `payconpy-2.2.1/LICENSE` & `payconpy-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/PKG-INFO` & `payconpy-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.2.1
+Version: 2.2.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.2.1/payconpy/femails/femails.py` & `payconpy-2.2.2/payconpy/femails/femails.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/fexceptions/exceptions.py` & `payconpy-2.2.2/payconpy/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/fpdf/focr/orc.py` & `payconpy-2.2.2/payconpy/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/fpdf/pdfutils/pdfutils.py` & `payconpy-2.2.2/payconpy/fpdf/pdfutils/pdfutils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/fpysimplegui/fpysimplegui.py` & `payconpy-2.2.2/payconpy/fpysimplegui/fpysimplegui.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/fpython/fpython.py` & `payconpy-2.2.2/payconpy/fpython/fpython.py`

 * *Files 4% similar despite different names*

```diff
@@ -434,29 +434,45 @@
 
 def limpa_terminal_e_cmd() -> None:
     """Essa função limpa o Terminal / CMD no Linux e no Windows"""
     
     os.system('cls' if os.name == 'nt' else 'clear')
 
 
-def limpa_diretorio(dir:str):
+def limpa_diretorio(dir: str, timeout_for_clear=5):
     """Limpa diretório(s)
     
     Args:
         dir (str): Caminho do diretório para limpar.
+        timeout_for_clear (int): Tempo em segundos para esperar antes de tentar novamente em caso de PermissionError.
     """
     DIR = os.path.abspath(dir)
-    if os.path.exists(DIR):
-        shutil.rmtree(DIR)
+    
+    def tentar_criar_dir(diretorio):
         try:
-            os.makedirs(DIR)
+            os.makedirs(diretorio)
         except FileExistsError:
             pass
+    
+    if os.path.exists(DIR):
+        tentativas = 0
+        sucesso = False
+        while not sucesso and tentativas * timeout_for_clear < timeout_for_clear * 3:  # Tenta por até 3 vezes o timeout_for_clear
+            try:
+                shutil.rmtree(DIR)
+                sucesso = True
+            except PermissionError:
+                tentativas += 1
+                time.sleep(timeout_for_clear)
+        if not sucesso:
+            raise PermissionError(f"Não foi possível limpar o diretório {DIR} após {tentativas} tentativas.")
+        
+        tentar_criar_dir(DIR)
     else:
-        os.makedirs(DIR)
+        tentar_criar_dir(DIR)
 
 
 def print_bonito(string : str, efeito='=', quebra_ultima_linha : bool=True) -> str:
     """Faz um print com separadores
     
 
     Args:
@@ -980,156 +996,130 @@
     base_path = getattr(
         sys,
         '_MEIPASS',
         os.path.dirname(os.path.abspath(__file__)))
     return os.path.join(base_path, relative_path)    
 
 
-def faz_log(msg: str, level: str = 'i', color: None|str=None, format: None|str=None) -> None:
-    """Faz log na pasta padrão (./logs/botLog.log)
+# FAZ LOGS
+console = Console()
 
+# Configura o logger globalmente
+path_logs_dir = os.path.abspath('logs')
+path_logs_file = os.path.join(path_logs_dir, 'logs.log')
+
+if not os.path.exists(path_logs_dir):
+    os.mkdir(path_logs_dir)
+
+logging.basicConfig(filename=path_logs_file,
+                    encoding='utf-8',
+                    filemode='a',  # append mode
+                    format='%(asctime)s - %(levelname)s - %(message)s',
+                    level=logging.INFO)
 
+logger = logging.getLogger()
+
+def faz_log(msg: str, level: str = 'i', color: None|str=None, format: None|str=None) -> None:
+    """Faz log na pasta padrão (./logs/botLog.log)
 
     Args:
         msg (str): "Mensagem de Log"
         level (str): "Niveis de Log"
         color (None|str): Cores Rich; defaut is None
         format (None|str) Formatação Rich; defaut is None
 
     Levels:
         'i' or not passed = info and print
-
         'i*' = info log only
-
         'w' = warning
-        
         'c*' = critical / Exception Error exc_info=True
-        
         'c' = critical
-        
         'e' = error
 
     Use:
     >>> faz_log('@@@@@@@@@@@@@@@@@@@', color='red')
     >>> faz_log('@@@@@@@@@@@@@@@@@@@', color='red', format='b')
     >>> faz_log('@ O SISTEMA CAIU! @', color='red on yellow b i s blink')
     >>> faz_log('@@@@@@@@@@@@@@@@@@@', color='green')
     >>> faz_log('@@@@@@@@@@@@@@@@@@@', color='green b i')
 
     Formatação Rich:
-            Colors: https://rich.readthedocs.io/en/latest/appendix/colors.html
+        Colors: https://rich.readthedocs.io/en/latest/appendix/colors.html
     """
-    path_logs_dir = os.path.abspath('logs')
-    path_logs_file = os.path.join(path_logs_dir, 'logs.log')
-
-    if not os.path.exists(path_logs_dir):
-        os.mkdir(path_logs_dir)
-    else:
-        pass
-
+    
     if isinstance(msg, str):
         pass
     
     if isinstance(msg, (object)):
         msg = str(msg)    
     
-
     if isinstance(level, (str)):
         pass
     else:
         print('COLOQUE UMA STING NO PARAMETRO LEVEL!')
 
     if isinstance(msg, (str)) and isinstance(level, (str)):
         if level == 'i' or level == '' or level is None:
-            logging.basicConfig(filename=path_logs_file,
-                                encoding='utf-8',
-                                filemode='w',
-                                format='%(asctime)s - %(levelname)s - %(message)s',
-                                level=logging.INFO
-                                )
+            logger.setLevel(logging.INFO)
             if isinstance(color, str) and isinstance(format, str):
-                print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
+                console.print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
             elif isinstance(color, str):
-                print(f'[{color}]{msg}[/{color}]')
+                console.print(f'[{color}]{msg}[/{color}]')
             else:
-                print(msg)
+                console.print(msg)
             if r'\n' in msg:
                 msg = msg.replace(r"\n", "")
-            logging.info(msg)
+            logger.info(msg)
 
-        if level == 'i*':
-            logging.basicConfig(filename=path_logs_file,
-                                encoding='utf-8',
-                                filemode='w',
-                                format='%(asctime)s - %(levelname)s - %(message)s',
-                                level=logging.INFO
-                                )
+        elif level == 'i*':
+            logger.setLevel(logging.INFO)
             if r'\n' in msg:
                 msg = msg.replace(r"\n", "")
-            logging.info(msg)
+            logger.info(msg)
 
         elif level == 'w':
-            logging.basicConfig(filename=path_logs_file,
-                                encoding='utf-8',
-                                filemode='w',
-                                format='%(asctime)s - %(levelname)s - %(message)s',
-                                level=logging.WARNING
-                                )
-            logging.warning(msg)
+            logger.setLevel(logging.WARNING)
+            logger.warning(msg)
             if isinstance(color, str) and isinstance(format, str):
-                print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
+                console.print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
             elif isinstance(color, str):
-                print(f'[{color}]{msg}[/{color}]')
+                console.print(f'[{color}]{msg}[/{color}]')
             else:
-                print(msg)
+                console.print(msg)
 
         elif level == 'e':
-            logging.basicConfig(filename=path_logs_file,
-                                encoding='utf-8',
-                                filemode='w',
-                                format='%(asctime)s - %(levelname)s - %(message)s',
-                                level=logging.ERROR
-                                )
-            logging.error(msg)
+            logger.setLevel(logging.ERROR)
+            logger.error(msg)
             if isinstance(color, str) and isinstance(format, str):
-                print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
+                console.print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
             elif isinstance(color, str):
-                print(f'[{color}]{msg}[/{color}]')
+                console.print(f'[{color}]{msg}[/{color}]')
             else:
-                print(msg)
+                console.print(msg)
 
         elif level == 'c':
-            logging.basicConfig(filename=path_logs_file,
-                                encoding='utf-8',
-                                filemode='w',
-                                format='%(asctime)s - %(levelname)s - %(message)s',
-                                level=logging.CRITICAL
-                                )
-            logging.critical(msg)
+            logger.setLevel(logging.CRITICAL)
+            logger.critical(msg)
             if isinstance(color, str) and isinstance(format, str):
-                print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
+                console.print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
             elif isinstance(color, str):
-                print(f'[{color}]{msg}[/{color}]')
+                console.print(f'[{color}]{msg}[/{color}]')
             else:
-                print(msg)
+                console.print(msg)
 
         elif level == 'c*':
-            logging.basicConfig(filename=path_logs_file,
-                                encoding='utf-8',
-                                filemode='w',
-                                format='%(asctime)s - %(levelname)s - %(message)s',
-                                level=logging.CRITICAL
-                                )
-            logging.critical(msg, exc_info=True)
+            logger.setLevel(logging.CRITICAL)
+            logger.critical(msg, exc_info=True)
             if isinstance(color, str) and isinstance(format, str):
-                print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
+                console.print(f'[{format}][{color}]{msg}[/{color}][/{format}]')
             elif isinstance(color, str):
-                print(f'[{color}]{msg}[/{color}]')
+                console.print(f'[{color}]{msg}[/{color}]')
             else:
-                print(msg)
+                console.print(msg)
+# FAZ LOGS
     
 
 def retorna_data_e_hora_a_frente(dias_a_frente: int, sep: str='/') -> str:
     """Retorna a data e hora com dias a frente da data atual
     ex: 15/06/2002 18:31 -> dias_a_frente=3 -> 18/06/2002 18:31
     """
     hj = date.today()
```

### Comparing `payconpy-2.2.1/payconpy/fregex/fregex.py` & `payconpy-2.2.2/payconpy/fregex/fregex.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/fselenium/fselenium.py` & `payconpy-2.2.2/payconpy/fselenium/fselenium.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/odoo/odoo_xmlrpc.py` & `payconpy-2.2.2/payconpy/odoo/odoo_xmlrpc.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/openai/apis/apis.py` & `payconpy-2.2.2/payconpy/openai/apis/apis.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/openai/assistants/assistants.py` & `payconpy-2.2.2/payconpy/openai/assistants/assistants.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/openai/get_cost.py` & `payconpy-2.2.2/payconpy/openai/get_cost.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy/utils/utils.py` & `payconpy-2.2.2/payconpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/payconpy.egg-info/PKG-INFO` & `payconpy-2.2.2/payconpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payconpy
-Version: 2.2.1
+Version: 2.2.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/payconpy
 Author: Paycon Automações
 Author-email: fernanda.yamamoto@paycon.com.br
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `payconpy-2.2.1/payconpy.egg-info/SOURCES.txt` & `payconpy-2.2.2/payconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payconpy-2.2.1/setup.py` & `payconpy-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '2.2.1'
+version = '2.2.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='payconpy',
         version=version,
         url='https://github.com/githubpaycon/payconpy',
```

