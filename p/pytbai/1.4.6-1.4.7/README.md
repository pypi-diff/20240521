# Comparing `tmp/pytbai-1.4.6.tar.gz` & `tmp/pytbai-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.4.6.tar", last modified: Thu Oct  5 14:07:43 2023, max compression
+gzip compressed data, was "pytbai-1.4.7.tar", last modified: Tue May 21 07:20:36 2024, max compression
```

## Comparing `pytbai-1.4.6.tar` & `pytbai-1.4.7.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3092 2023-10-05 14:07:42.000000 pytbai-1.4.6/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2023-10-05 14:07:42.000000 pytbai-1.4.6/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2023-10-05 14:07:42.000000 pytbai-1.4.6/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2023-10-05 14:07:42.000000 pytbai-1.4.6/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-10-05 14:07:42.000000 pytbai-1.4.6/Makefile
--rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2023-10-05 14:07:43.687402 pytbai-1.4.6/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2023-10-05 14:07:42.000000 pytbai-1.4.6/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11347 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2091 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/utils/pdf.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5251 2023-10-05 14:07:42.000000 pytbai-1.4.6/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/pytbai.egg-info/
--rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2023-10-05 14:07:43.000000 pytbai-1.4.6/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      839 2023-10-05 14:07:43.000000 pytbai-1.4.6/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2023-10-05 14:07:43.000000 pytbai-1.4.6/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2023-10-05 14:07:43.000000 pytbai-1.4.6/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2023-10-05 14:07:42.000000 pytbai-1.4.6/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2023-10-05 14:07:43.687402 pytbai-1.4.6/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1131 2023-10-05 14:07:42.000000 pytbai-1.4.6/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2023-10-05 14:07:43.687402 pytbai-1.4.6/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2023-10-05 14:07:42.000000 pytbai-1.4.6/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3273 2024-05-21 07:20:33.000000 pytbai-1.4.7/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2024-05-21 07:20:33.000000 pytbai-1.4.7/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2024-05-21 07:20:33.000000 pytbai-1.4.7/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2024-05-21 07:20:33.000000 pytbai-1.4.7/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 07:20:33.000000 pytbai-1.4.7/Makefile
+-rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 07:20:36.669219 pytbai-1.4.7/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2024-05-21 07:20:33.000000 pytbai-1.4.7/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11391 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5251 2024-05-21 07:20:33.000000 pytbai-1.4.7/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/pytbai.egg-info/
+-rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 07:20:36.000000 pytbai-1.4.7/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      819 2024-05-21 07:20:36.000000 pytbai-1.4.7/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2024-05-21 07:20:36.000000 pytbai-1.4.7/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2024-05-21 07:20:36.000000 pytbai-1.4.7/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 07:20:33.000000 pytbai-1.4.7/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2024-05-21 07:20:36.669219 pytbai-1.4.7/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1131 2024-05-21 07:20:33.000000 pytbai-1.4.7/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 07:20:36.669219 pytbai-1.4.7/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2024-05-21 07:20:33.000000 pytbai-1.4.7/tests/test_basic.py
```

### Comparing `pytbai-1.4.6/CHANGELOG.txt` & `pytbai-1.4.7/CHANGELOG.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+1.4.7 (2024-05-21)
+------------------
+
+- Update core.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+- Delete pytbai/utils/pdf.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.4.6 (2023-10-05)
 ------------------
 
 - signedxml string [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.4.6/LICENSE` & `pytbai-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/PKG-INFO` & `pytbai-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.6
+Version: 1.4.7
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.6/README.md` & `pytbai-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai/core.py` & `pytbai-1.4.7/pytbai/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,23 @@
 
 
 class Subject:
     def __init__(
         self,
         entity_id,
         name,
+        logo=None,
         territory=GIPUZKOA,
         multi_recipient=N,
         external_invoice=N,
         env="DEV",
     ):
         self.entity_id = entity_id
         self.name = name
+        self.logo = logo
         if not territory:
             self.authority_api = GIPUZKOA[env]["invoice"]
             self.qr_api = GIPUZKOA[env]["qr"]
         elif territory in AUTHORITY_APIS:
             self.authority_api = AUTHORITY_APIS[territory][env]["invoice"]
             self.qr_api = AUTHORITY_APIS[territory][env]["qr"]
         else:
```

### Comparing `pytbai-1.4.6/pytbai/definitions.py` & `pytbai-1.4.7/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.4.7/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.4.7/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.4.7/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.4.7/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai/utils/xml.py` & `pytbai-1.4.7/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/pytbai.egg-info/PKG-INFO` & `pytbai-1.4.7/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.6
+Version: 1.4.7
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.6/pytbai.egg-info/SOURCES.txt` & `pytbai-1.4.7/pytbai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 pytbai/templates/XML/__init__.py
 pytbai/templates/XML/tbai_structure.xml
 pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
 pytbai/templates/XSD/__init__.py
 pytbai/templates/XSD/ticketBaiV1-2-1.xsd
 pytbai/utils/__init__.py
 pytbai/utils/crypto.py
-pytbai/utils/pdf.py
 pytbai/utils/xml.py
 tests/__init__.py
 tests/context.py
 tests/test_basic.py
 tests/certs/cert.pem
 tests/certs/cert_for_tests.p12
 tests/certs/key.pem
```

### Comparing `pytbai-1.4.6/setup.py` & `pytbai-1.4.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.4.6",
+    version="1.4.7",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.4.6/tests/certs/cert.pem` & `pytbai-1.4.7/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/tests/certs/cert_for_tests.p12` & `pytbai-1.4.7/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/tests/certs/key.pem` & `pytbai-1.4.7/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/tests/data/tbai_json.py` & `pytbai-1.4.7/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.6/tests/test_basic.py` & `pytbai-1.4.7/tests/test_basic.py`

 * *Files identical despite different names*

