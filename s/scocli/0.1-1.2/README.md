# Comparing `tmp/scocli-0.1.tar.gz` & `tmp/scocli-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scocli-0.1.tar", last modified: Mon May 13 18:22:42 2024, max compression
+gzip compressed data, was "scocli-1.2.tar", last modified: Tue May 21 00:15:36 2024, max compression
```

## Comparing `scocli-0.1.tar` & `scocli-1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-13 18:22:42.040774 scocli-0.1/
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      187 2024-05-13 18:22:42.040774 scocli-0.1/PKG-INFO
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      468 2024-04-10 14:37:41.000000 scocli-0.1/README.md
-drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-13 18:22:42.040774 scocli-0.1/sco/
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        0 2024-04-10 14:37:41.000000 scocli-0.1/sco/__init__.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     5072 2024-04-19 13:11:57.000000 scocli-0.1/sco/addResource.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4705 2024-04-19 12:03:08.000000 scocli-0.1/sco/build.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4064 2024-05-13 17:30:19.000000 scocli-0.1/sco/checkManifest.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2247 2024-05-13 18:08:11.000000 scocli-0.1/sco/organizeManifest.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2261 2024-04-10 14:37:41.000000 scocli-0.1/sco/removeResource.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1024 2024-04-18 17:59:39.000000 scocli-0.1/sco/seeManifest.py
-drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-13 18:22:42.040774 scocli-0.1/scocli.egg-info/
--rw-r--r--   0 vasapg    (1000) vasapg    (1000)      187 2024-05-13 18:22:42.000000 scocli-0.1/scocli.egg-info/PKG-INFO
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      272 2024-05-13 18:22:42.000000 scocli-0.1/scocli.egg-info/SOURCES.txt
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        1 2024-05-13 18:22:42.000000 scocli-0.1/scocli.egg-info/dependency_links.txt
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        4 2024-05-13 18:22:42.000000 scocli-0.1/scocli.egg-info/top_level.txt
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)       38 2024-05-13 18:22:42.040774 scocli-0.1/setup.cfg
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      442 2024-05-13 18:09:19.000000 scocli-0.1/setup.py
+drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-21 00:15:36.142665 scocli-1.2/
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      187 2024-05-21 00:15:36.142665 scocli-1.2/PKG-INFO
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      468 2024-04-10 14:37:41.000000 scocli-1.2/README.md
+drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-21 00:15:36.142665 scocli-1.2/sco/
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        0 2024-04-10 14:37:41.000000 scocli-1.2/sco/__init__.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     5095 2024-05-21 00:07:37.000000 scocli-1.2/sco/addResource.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4334 2024-05-21 00:07:37.000000 scocli-1.2/sco/build.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1131 2024-05-21 00:07:37.000000 scocli-1.2/sco/bundle.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4537 2024-05-21 00:07:37.000000 scocli-1.2/sco/checkManifest.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2270 2024-05-21 00:07:37.000000 scocli-1.2/sco/organizeManifest.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2284 2024-05-21 00:07:37.000000 scocli-1.2/sco/removeResource.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1047 2024-05-21 00:07:37.000000 scocli-1.2/sco/seeManifest.py
+drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-21 00:15:36.142665 scocli-1.2/scocli.egg-info/
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      187 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/PKG-INFO
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      286 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        1 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        4 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/top_level.txt
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)       38 2024-05-21 00:15:36.142665 scocli-1.2/setup.cfg
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      467 2024-05-21 00:07:37.000000 scocli-1.2/setup.py
```

### Comparing `scocli-0.1/sco/addResource.py` & `scocli-1.2/sco/addResource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 import os
 import sys
 import xml.etree.ElementTree as ET
 import xml.dom.minidom
 
 def prettify_xml(elem):
     """Retorna una versión con formato legible del elemento XML"""
@@ -28,15 +29,15 @@
         if not os.path.exists(file_path):
             print("El archivo " + file_path + " no existe")
             sys.exit(1)
         file_name = os.path.basename(file_path)
         existing_file = resource.find(f"./{{http://www.imsglobal.org/xsd/imscp_v1p1}}file[@href='{file_name}']")
         if existing_file is None:
             file_element = ET.SubElement(resource, "{http://www.imsglobal.org/xsd/imscp_v1p1}file")
-            file_element.set("href", file_name)
+            file_element.set("href", file_path)
             file_element.tail = '\n'  # Agregar salto de línea después de la etiqueta <file>
 
 def add_resource_to_imsmanifest(files):
     # Buscar el archivo imsmanifest.xml en el directorio actual
     current_directory = os.getcwd()
     xml_file = os.path.join(current_directory, "imsmanifest.xml")
```

### Comparing `scocli-0.1/sco/build.py` & `scocli-1.2/sco/build.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,14 @@
+#!/usr/bin/env python3
 #coding=utf-8
 import xml.etree.ElementTree as ET
 import os
 import xml.dom.minidom
 import subprocess
 
-
-def create_javascript_file(project_name):
-    javascript_code = """
-    const scoAPI = require('scoapi')
-    window.onload = scoAPI().Init();"""
-
-    # Escribir el código JavaScript en el archivo javascript.js
-    with open(project_name + "/javascript/APIinit.js", "w") as f:
-        f.write(javascript_code)
-
-    print("Archivo javascript.js creado con éxito.")
-
-
 def create_imsmanifest(project_name):
     # Crear el elemento raíz <manifest>
     identifier = project_name.replace(" ", "_")
     root = ET.Element("manifest")
     root.set("xmlns", "http://www.imsglobal.org/xsd/imscp_v1p1")
     root.set("xmlns:xsi", "http://www.w3.org/2001/XMLSchema-instance")
     root.set("xmlns:adlcp", "http://www.adlnet.org/xsd/adlcp_v1p3")
@@ -53,17 +41,17 @@
 
     # Agregar la sección <resources>
     resources = ET.SubElement(root, "resources")
     resource = ET.SubElement(resources, "resource")
     resource.set("identifier", "resource_1")
     resource.set("type", "webcontent")
     resource.set("{http://www.adlnet.org/xsd/adlcp_v1p3}scormType", "sco")
-    resource.set("href", "index.html")
+    resource.set("href", "html/index.html")
     file = ET.SubElement(resource, "file")
-    file.set("href", "index.html")
+    file.set("href", "html/index.html")
 
     # Crear el árbol XML
     tree = ET.ElementTree(root)
 
     # Convertir el árbol XML a una cadena de texto con formato
     xml_string = ET.tostring(root, encoding="utf-8")
     reparsed = xml.dom.minidom.parseString(xml_string)
@@ -86,21 +74,20 @@
     # Create subfolders
     for folder in folders:
         folder_path = os.path.join(project_name, folder)
         os.mkdir(folder_path)
         print(f"Created '{folder}' folder.")
 
     # Create index.html file
-    index_html = os.path.join(project_name, 'index.html')
+    index_html = os.path.join(project_name, 'html/index.html')
     with open(index_html, 'w') as f:
         f.write('<!DOCTYPE html>\n<html>\n<head>\n<title>SCORM Project</title>\n</head>\n<body>\n'
                 + '<script src = "node_modules/scoapi/scoAPI.js"> </script><h1>This is the index of the project, where the activity begins.</h1>\n</body>\n</html>')
     print("Created 'index.html' file.")
     create_imsmanifest(project_name)
-    create_javascript_file(project_name)
 
     print("SCORM project structure created successfully.")
 
 def install_npm_package(package_name, project_path):
     try:
         subprocess.check_call(['npm', 'i', package_name], cwd=project_path)
         print(f"Successfully installed {package_name}")
```

### Comparing `scocli-0.1/sco/checkManifest.py` & `scocli-1.2/sco/checkManifest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+#!/usr/bin/env python3
 import os
 from xml.etree import ElementTree as ET
 
 def recopilar_archivos(ruta, recursos):
     archivos = []
     archivos_no_utilizados = []
+    # Files to ignore
+    ignore_files = ["package-lock.json", "package.json", "imsmanifest.xml", "node_modules/.package-lock.json", "node_modules/scoapi/scoAPI.js", "node_modules/scoapi/package.json"]
+    # Extensions to ignore
+    ignore_extensions = [".zip", ".babelrc"]
+
     for root, dirs, files in os.walk(ruta):
         for file in files:
             archivo = os.path.relpath(os.path.join(root, file), ruta)
             archivos.append(archivo)
+            # Check if the file is in the ignore list
+            if archivo in ignore_files or file.endswith(tuple(ignore_extensions)):
+                continue
             # Comprobar si el archivo no está en los recursos definidos
             if archivo not in recursos:
                 archivos_no_utilizados.append(archivo)
     return archivos, archivos_no_utilizados
 
+
 def validar_archivos_necesarios(raiz_proyecto):
     # Lista de archivos necesarios en un proyecto SCORM
     archivos_necesarios = [
         "imsmanifest.xml",
     ]
 
     for elemento in archivos_necesarios:
@@ -35,63 +45,64 @@
 
         # Definir el espacio de nombres
         ns = {
             'ims': 'http://www.imsglobal.org/xsd/imscp_v1p1',
             'ns2': 'http://www.adlnet.org/xsd/adlcp_v1p3'
         }
 
-        # Obtener todos los identifiers de los recursos definidos en imsmanifest.xml
-        recursos = {resource.attrib['identifier'] for resource in root.findall(".//ims:resource", namespaces=ns)}
+        # Obtener todos los archivos asociados a los recursos definidos en imsmanifest.xml
+        recursos = set()
+        files = set()
+        for resource in root.findall(".//{http://www.imsglobal.org/xsd/imscp_v1p1}resource", namespaces=ns):
+            identifier = resource.attrib['identifier']
+            for file_elem in resource.findall(".//{http://www.imsglobal.org/xsd/imscp_v1p1}file", namespaces=ns):
+                href = file_elem.attrib['href']
+                recursos.add(href)
+                files.add((identifier, href))
 
         # Obtener los identifierref de los items dentro de organization
         organization_items = root.findall(".//ims:organizations/ims:organization/ims:item", namespaces=ns)
         for item in organization_items:
             identifierref = item.attrib['identifierref']
-            if identifierref not in recursos:
-                print(f"Error: El identifierref '{identifierref}' no coincide con ningún identifier de recurso en imsmanifest.xml")
-                return False
+            for identifier, href in files:
+                if identifierref == identifier:
+                    recursos.add(href)
 
         #print("recursos:", recursos)
         #print("organization_items:", organization_items)
         print("La validación de imsmanifest.xml se ha completado correctamente.")
-        return True
+        return recursos
 
     except Exception as e:
         print(f"Error al analizar el archivo imsmanifest.xml: {e}")
-        return False
-
+        return set()
 
 if __name__ == "__main__":
     # Buscar imsmanifest.xml en el directorio actual
     ruta_actual = os.getcwd()
     ruta_imsmanifest = os.path.join(ruta_actual, "imsmanifest.xml")
 
     if not os.path.exists(ruta_imsmanifest):
         print("Error: No se encontró el archivo imsmanifest.xml en el directorio actual.")
     else:
         # Validar archivos necesarios
         if not validar_archivos_necesarios(ruta_actual):
             print("El proyecto SCORM no está completo o tiene errores.")
         else:
             # Validar imsmanifest.xml
-            if not validar_imsmanifest(ruta_imsmanifest):
+            recursos = validar_imsmanifest(ruta_imsmanifest)
+            if not recursos:
                 print("El proyecto SCORM no está completo o tiene errores.")
             else:
                 # Recopilar todos los archivos en el proyecto
-                recursos = set()
-                tree = ET.parse(ruta_imsmanifest)
-                root = tree.getroot()
-                for resource in root.findall(".//{http://www.imsglobal.org/xsd/imsmd_rootv1p2p1}resource"):
-                    recursos.add(resource.attrib['identifier'])
-
                 archivos, archivos_no_utilizados = recopilar_archivos(ruta_actual, recursos)
                 
                 print("Archivos encontrados en el proyecto:")
-                for archivo in archivos:
-                    print(archivo)
+                #for archivo in archivos:
+                    #print(archivo)
 
                 if archivos_no_utilizados:
                     print("\nWarnings:")
                     for archivo_no_utilizado in archivos_no_utilizados:
                         print(f"Warning: El archivo '{archivo_no_utilizado}' no está siendo declarado en el paquete SCORM.")
                         
-                print("\nEl proyecto SCORM está listo para ser subido al LMS.")
+                print("\nEl proyecto SCORM está listo para ser subido al LMS.")
```

### Comparing `scocli-0.1/sco/organizeManifest.py` & `scocli-1.2/sco/organizeManifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 import sys
 import os
 from xml.etree import ElementTree as ET
 
 def reorganize_organization(manifest_xml, item_identifier, new_position):
     # Define namespaces
     namespaces = {
```

### Comparing `scocli-0.1/sco/removeResource.py` & `scocli-1.2/sco/removeResource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 import os
 import sys
 import xml.etree.ElementTree as ET
 import xml.dom.minidom
 
 def prettify_xml(elem):
     """Retorna una versión con formato legible del elemento XML"""
```

### Comparing `scocli-0.1/sco/seeManifest.py` & `scocli-1.2/sco/seeManifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 import xml.etree.ElementTree as ET
 
 def print_manifest_tree(manifest_path, indent=0):
     tree = ET.parse(manifest_path)
     root = tree.getroot()
     print_element(root, indent)
```

