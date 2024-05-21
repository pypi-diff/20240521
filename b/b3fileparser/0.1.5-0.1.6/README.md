# Comparing `tmp/b3fileparser-0.1.5.tar.gz` & `tmp/b3fileparser-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b3fileparser-0.1.5.tar", last modified: Thu Mar  7 14:26:27 2024, max compression
+gzip compressed data, was "b3fileparser-0.1.6.tar", max compression
```

## Comparing `b3fileparser-0.1.5.tar` & `b3fileparser-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,7 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-07 14:26:27.609584 b3fileparser-0.1.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1069 2024-03-07 14:13:26.000000 b3fileparser-0.1.5/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      280 2024-03-07 14:26:27.609584 b3fileparser-0.1.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12480 2024-03-07 14:13:26.000000 b3fileparser-0.1.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-07 14:26:27.601584 b3fileparser-0.1.5/b3fileparser/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-03-07 14:14:14.000000 b3fileparser-0.1.5/b3fileparser/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3330 2024-03-07 14:13:26.000000 b3fileparser-0.1.5/b3fileparser/b3_meta_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2062 2024-03-07 14:16:36.000000 b3fileparser-0.1.5/b3fileparser/b3parser.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-07 14:26:27.609584 b3fileparser-0.1.5/b3fileparser.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      280 2024-03-07 14:26:27.000000 b3fileparser-0.1.5/b3fileparser.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      358 2024-03-07 14:26:27.000000 b3fileparser-0.1.5/b3fileparser.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-07 14:26:27.000000 b3fileparser-0.1.5/b3fileparser.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-07 14:22:38.000000 b3fileparser-0.1.5/b3fileparser.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2024-03-07 14:26:27.000000 b3fileparser-0.1.5/b3fileparser.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2024-03-07 14:26:27.000000 b3fileparser-0.1.5/b3fileparser.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-07 14:26:27.609584 b3fileparser-0.1.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      391 2024-03-07 14:24:05.000000 b3fileparser-0.1.5/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-07 14:26:27.609584 b3fileparser-0.1.5/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-03-07 14:14:14.000000 b3fileparser-0.1.5/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      417 2024-03-07 14:16:05.000000 b3fileparser-0.1.5/tests/test_b3file.py
+-rw-r--r--   0        0        0     1069 2024-05-20 13:09:26.899061 b3fileparser-0.1.6/LICENSE
+-rw-r--r--   0        0        0    12480 2024-05-20 13:09:26.899061 b3fileparser-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-20 13:09:26.899061 b3fileparser-0.1.6/b3fileparser/__init__.py
+-rw-r--r--   0        0        0     3984 2024-05-20 23:38:12.075313 b3fileparser-0.1.6/b3fileparser/b3_meta_data.py
+-rw-r--r--   0        0        0     3101 2024-05-21 00:43:49.374664 b3fileparser-0.1.6/b3fileparser/b3parser.py
+-rw-r--r--   0        0        0      422 2024-05-21 11:56:57.815597 b3fileparser-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    13035 1970-01-01 00:00:00.000000 b3fileparser-0.1.6/PKG-INFO
```

### Comparing `b3fileparser-0.1.5/LICENSE` & `b3fileparser-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `b3fileparser-0.1.5/README.md` & `b3fileparser-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `b3fileparser-0.1.5/b3fileparser/b3_meta_data.py` & `b3fileparser-0.1.6/b3fileparser/b3_meta_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,102 @@
 META_DATA = {    
-    "TIPREG":{'name':"TIPO_DE_REGISTRO", 'size':2 },
-    "DATAPR":{'name':"DATA_DO_PREGAO", 'size':8},
-    "CODBDI":{'name':"CODIGO_BDI", 'size':2},
-    "CODNEG":{'name':"CODIGO_DE_NEGOCIACAO",'size':12},
-    "TPMERC":{'name':"TIPO_DE_MERCADO",'size':3},
-    "NOMRES":{'name':"NOME_DA_EMPRESA",'size':12},
-    "ESPECI":{'name':"ESPECIFICACAO_DO_PAPEL",'size':10},
-    "PRAZOT":{'name':"PRAZO_EM_DIAS_DO_MERCADO_A_TERMO",'size':3},
-    "MODREF":{'name':"MOEDA_DE_REFERENCIA",'size':4},
-    "PREABE":{'name':"PRECO_DE_ABERTURA",'size':13},
-    "PREMAX":{'name':"PRECO_MAXIMO",'size':13},
-    "PREMIN":{'name':"PRECO_MINIMO",'size':13},
-    "PREMED":{'name':"PRECO_MEDIO",'size':13},
-    "PREULT":{'name':"PRECO_ULTIMO_NEGOCIO",'size':13},
-    "PREOFC":{'name':"PRECO_MELHOR_OFERTA_DE_COMPRA",'size':13},
-    "PREOFV":{'name':"PRECO_MELHOR_OFERTA_DE_VENDAS",'size':13},
-    "TOTNEG":{'name':"NUMERO_DE_NEGOCIOS",'size':5},
-    "QUATOT":{'name':"QUANTIDADE_NEGOCIADA",'size':18},
-    "VOLTOT":{'name':"VOLUME_TOTAL_NEGOCIADO",'size':18},
-    "PREEXE":{'name':"PRECO_DE_EXERCICIO",'size':13},
-    "INDOPC":{'name':"INDICADOR_DE_CORRECAO_DE_PRECOS",'size':1},
-    "DATVEN":{'name':"DATA_DE_VENCIMENTO",'size':8},
-    "FATCOT":{'name':"FATOR_DE_COTACAO",'size':7},
-    "PTOEXE":{'name':"PRECO_DE_EXERCICIO_EM_PONTOS",'size':13},
-    "CODISI":{'name':"CODIGO_ISIN",'size':12},
-    "DISMES":{'name':"NUMERO_DE_DISTRIBUICAO",'size':3}
+    "TIPREG":{'name':"TIPO_DE_REGISTRO", 'size':2, 'dtype':'category'},
+    "DATAPR":{'name':"DATA_DO_PREGAO", 'size':8, 'dtype': 'object'},
+    "CODBDI":{'name':"CODIGO_BDI", 'size':2, 'dtype':'category'},
+    "CODNEG":{'name':"CODIGO_DE_NEGOCIACAO",'size':12,'dtype':'category'},
+    "TPMERC":{'name':"TIPO_DE_MERCADO",'size':3, 'dtype':'category'},
+    "NOMRES":{'name':"NOME_DA_EMPRESA",'size':12, 'dtype':'category'},
+    "ESPECI":{'name':"ESPECIFICACAO_DO_PAPEL",'size':10, 'dtype':'category'},
+    "PRAZOT":{'name':"PRAZO_EM_DIAS_DO_MERCADO_A_TERMO",'size':3, 'dtype':'object'},
+    "MODREF":{'name':"MOEDA_DE_REFERENCIA",'size':4, 'dtype':'category'},
+    "PREABE":{'name':"PRECO_DE_ABERTURA",'size':13, 'dtype': 'float32'},
+    "PREMAX":{'name':"PRECO_MAXIMO",'size':13, 'dtype': 'float32'},
+    "PREMIN":{'name':"PRECO_MINIMO",'size':13, 'dtype': 'float32'},
+    "PREMED":{'name':"PRECO_MEDIO",'size':13, 'dtype': 'float32'},
+    "PREULT":{'name':"PRECO_ULTIMO_NEGOCIO",'size':13, 'dtype': 'float32'},
+    "PREOFC":{'name':"PRECO_MELHOR_OFERTA_DE_COMPRA",'size':13, 'dtype': 'float32'},
+    "PREOFV":{'name':"PRECO_MELHOR_OFERTA_DE_VENDAS",'size':13, 'dtype': 'float32'},
+    "TOTNEG":{'name':"NUMERO_DE_NEGOCIOS",'size':5, 'dtype':'object'},
+    "QUATOT":{'name':"QUANTIDADE_NEGOCIADA",'size':18, 'dtype':'object'},
+    "VOLTOT":{'name':"VOLUME_TOTAL_NEGOCIADO",'size':18, 'dtype': 'float64'},
+    "PREEXE":{'name':"PRECO_DE_EXERCICIO",'size':13, 'dtype': 'float32'},
+    "INDOPC":{'name':"INDICADOR_DE_CORRECAO_DE_PRECOS",'size':1, 'dtype':'category'},
+    "DATVEN":{'name':"DATA_DE_VENCIMENTO",'size':8, 'dtype':'object'},
+    "FATCOT":{'name':"FATOR_DE_COTACAO",'size':7, 'dtype':'category'},
+    "PTOEXE":{'name':"PRECO_DE_EXERCICIO_EM_PONTOS",'size':13, 'dtype': 'float32'},
+    "CODISI":{'name':"CODIGO_ISIN",'size':12, 'dtype':'category'},
+    "DISMES":{'name':"NUMERO_DE_DISTRIBUICAO",'size':3, 'dtype':'category'}
 }
 
 
 MARKETS = {
-    10:'VISTA',
-    12:'EXERCICIO_DE_OPCOES_DE_COMPRA',
-    13:'EXERCÍCIO_DE_OPCOES_DE_VENDA',
-    17:'LEILAO',
-    20:'FRACIONARIO',
-    30:'TERMO',
-    50:'FUTURO_COM_RETENCAO_DE_GANHO',
-    60:'FUTURO_COM_MOVIMENTACAO_CONTINUA',
-    70:'OPCOES_DE_COMPRA',
-    80:'OPCOES_DE_VENDA'
+    '010':'VISTA',
+    '012':'EXERCICIO_DE_OPCOES_DE_COMPRA',
+    '013':'EXERCÍCIO_DE_OPCOES_DE_VENDA',
+    '017':'LEILAO',
+    '020':'FRACIONARIO',
+    '030':'TERMO',
+    '050':'FUTURO_COM_RETENCAO_DE_GANHO',
+    '060':'FUTURO_COM_MOVIMENTACAO_CONTINUA',
+    '070':'OPCOES_DE_COMPRA',
+    '080':'OPCOES_DE_VENDA'
 }
 
 INDOPC = {
-    0:'0',
-    1:'US$',
-    2:"TJLP",
-    8:"IGPM",
-    9:"URV"
+    '0':'0',
+    '1':'US$',
+    '2':"TJLP",
+    '8':"IGPM",
+    '9':"URV"
 }
 
 CODBDI = {
-    0:'0',
-    2:"LOTE_PADRAO",
-    5:"SANCIONADAS PELOS REGULAMENTOS BMFBOVESPA",
-    6:"CONCORDATARIAS",
-    7:"RECUPERACAO_EXTRAJUDICIAL",
-    8:"RECUPERAÇÃO_JUDICIAL",
-    9:"REGIME_DE_ADMINISTRACAO_ESPECIAL_TEMPORARIA",
-    10:"DIREITOS_E_RECIBOS",
-    11:"INTERVENCAO",
-    12:"FUNDOS_IMOBILIARIOS",
-    13:'13',
-    14:"CERT.INVEST/TIT.DIV.PUBLICA",
-    18:"OBRIGACÕES",
-    22:"BÔNUS(PRIVADOS)",
-    26:"APOLICES/BÔNUS/TITULOS PUBLICOS",
-    32:"EXERCICIO_DE_OPCOES_DE_COMPRA_DE_INDICES",
-    33:"EXERCICIO_DE_OPCOES_DE_VENDA_DE_INDICES",
-    34:'34',
-    35:'35',
-    36:'36',
-    37:'37',
-    38:"EXERCICIO_DE_OPCOES_DE_COMPRA",
-    42:"EXERCICIO_DE_OPCOES_DE_VENDA",
-    46:"LEILAO_DE_NAO_COTADOS",
-    48:"LEILAO_DE_PRIVATIZACAO",
-    49:"LEILAO_DO_FUNDO_RECUPERACAO_ECONOMICA_ESPIRITO_SANTO",
-    50:"LEILAO",
-    51:"LEILAO_FINOR",
-    52:"LEILAO_FINAM",
-    53:"LEILAO_FISET",
-    54:"LEILAO_DE_ACÕES_EM_MORA",
-    56:"VENDAS_POR_ALVARA_JUDICIAL",
-    58:"OUTROS",
-    60:"PERMUTA_POR_ACÕES",
-    61:"META",
-    62:"MERCADO_A_TERMO",
-    66:"DEBENTURES_COM_DATA_DE_VENCIMENTO_ATE_3_ANOS",
-    68:"DEBENTURES_COM_DATA_DE_VENCIMENTO_MAIOR_QUE_3_ANOS",
-    70:"FUTURO_COM_RETENCAO_DE_GANHOS",
-    71:"MERCADO_DE_FUTURO",
-    74:"OPCOES_DE_COMPRA_DE_INDICES",
-    75:"OPCOES_DE_VENDA_DE_INDICES",
-    78:"OPCOES_DE_COMPRA",
-    82:"OPCOES_DE_VENDA",
-    83:"BOVESPAFIX",
-    84:"SOMA_FIX",
-    90:"TERMO_VISTA_REGISTRADO",
-    96:"MERCADO_FRACIONARIO",
-    99:"TOTAL_GERAL"
+    '00':'0',
+    '02':"LOTE_PADRAO",
+    '05':"SANCIONADAS PELOS REGULAMENTOS BMFBOVESPA",
+    '06':"CONCORDATARIAS",
+    '07':"RECUPERACAO_EXTRAJUDICIAL",
+    '08':"RECUPERAÇÃO_JUDICIAL",
+    '09':"REGIME_DE_ADMINISTRACAO_ESPECIAL_TEMPORARIA",
+    '10':"DIREITOS_E_RECIBOS",
+    '11':"INTERVENCAO",
+    '12':"FUNDOS_IMOBILIARIOS",
+    '13':'13',
+    '14':"CERT.INVEST/TIT.DIV.PUBLICA",
+    '18':"OBRIGACÕES",
+    '22':"BÔNUS(PRIVADOS)",
+    '26':"APOLICES/BÔNUS/TITULOS PUBLICOS",
+    '32':"EXERCICIO_DE_OPCOES_DE_COMPRA_DE_INDICES",
+    '33':"EXERCICIO_DE_OPCOES_DE_VENDA_DE_INDICES",
+    '34':'34',
+    '35':'35',
+    '36':'36',
+    '37':'37',
+    '38':"EXERCICIO_DE_OPCOES_DE_COMPRA",
+    '42':"EXERCICIO_DE_OPCOES_DE_VENDA",
+    '46':"LEILAO_DE_NAO_COTADOS",
+    '48':"LEILAO_DE_PRIVATIZACAO",
+    '49':"LEILAO_DO_FUNDO_RECUPERACAO_ECONOMICA_ESPIRITO_SANTO",
+    '50':"LEILAO",
+    '51':"LEILAO_FINOR",
+    '52':"LEILAO_FINAM",
+    '53':"LEILAO_FISET",
+    '54':"LEILAO_DE_ACÕES_EM_MORA",
+    '56':"VENDAS_POR_ALVARA_JUDICIAL",
+    '58':"OUTROS",
+    '60':"PERMUTA_POR_ACÕES",
+    '61':"META",
+    '62':"MERCADO_A_TERMO",
+    '66':"DEBENTURES_COM_DATA_DE_VENCIMENTO_ATE_3_ANOS",
+    '68':"DEBENTURES_COM_DATA_DE_VENCIMENTO_MAIOR_QUE_3_ANOS",
+    '70':"FUTURO_COM_RETENCAO_DE_GANHOS",
+    '71':"MERCADO_DE_FUTURO",
+    '74':"OPCOES_DE_COMPRA_DE_INDICES",
+    '75':"OPCOES_DE_VENDA_DE_INDICES",
+    '78':"OPCOES_DE_COMPRA",
+    '82':"OPCOES_DE_VENDA",
+    '83':"BOVESPAFIX",
+    '84':"SOMA_FIX",
+    '90':"TERMO_VISTA_REGISTRADO",
+    '96':"MERCADO_FRACIONARIO",
+    '99':"TOTAL_GERAL"
 }
```

