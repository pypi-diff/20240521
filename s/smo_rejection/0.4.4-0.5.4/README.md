# Comparing `tmp/smo_rejection-0.4.4.tar.gz` & `tmp/smo_rejection-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.4.4.tar", max compression
+gzip compressed data, was "smo_rejection-0.5.4.tar", max compression
```

## Comparing `smo_rejection-0.4.4.tar` & `smo_rejection-0.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      283 2024-05-21 11:14:25.971590 smo_rejection-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    16387 2024-05-21 11:13:02.127103 smo_rejection-0.4.4/README.md
--rw-r--r--   0        0        0      496 2024-05-21 11:13:02.130096 smo_rejection-0.4.4/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-21 11:13:02.136049 smo_rejection-0.4.4/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-21 11:13:02.136049 smo_rejection-0.4.4/smo_rejection/models.py
--rw-r--r--   0        0        0     4236 2024-05-21 11:13:02.137051 smo_rejection-0.4.4/smo_rejection/pdf_export.py
--rw-r--r--   0        0        0     4403 2024-05-21 11:13:28.975815 smo_rejection-0.4.4/smo_rejection/processing.py
--rw-r--r--   0        0        0     4306 2024-05-21 11:13:02.137051 smo_rejection-0.4.4/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-21 11:13:02.138052 smo_rejection-0.4.4/smo_rejection/utils.py
--rw-r--r--   0        0        0     4797 2024-05-21 11:13:02.138052 smo_rejection-0.4.4/smo_rejection/xml_export.py
--rw-r--r--   0        0        0    16485 1970-01-01 00:00:00.000000 smo_rejection-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      305 2024-05-21 21:18:54.154757 smo_rejection-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    16387 2024-05-21 11:13:02.127103 smo_rejection-0.5.4/README.md
+-rw-r--r--   0        0        0      496 2024-05-21 11:13:02.130096 smo_rejection-0.5.4/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-21 11:13:02.136049 smo_rejection-0.5.4/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-21 11:13:02.136049 smo_rejection-0.5.4/smo_rejection/models.py
+-rw-r--r--   0        0        0     4409 2024-05-21 21:18:28.009912 smo_rejection-0.5.4/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4403 2024-05-21 11:13:28.975815 smo_rejection-0.5.4/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4306 2024-05-21 11:13:02.137051 smo_rejection-0.5.4/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-21 11:13:02.138052 smo_rejection-0.5.4/smo_rejection/utils.py
+-rw-r--r--   0        0        0     4797 2024-05-21 11:13:02.138052 smo_rejection-0.5.4/smo_rejection/xml_export.py
+-rw-r--r--   0        0        0    16527 1970-01-01 00:00:00.000000 smo_rejection-0.5.4/PKG-INFO
```

### Comparing `smo_rejection-0.4.4/README.md` & `smo_rejection-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/smo_rejection/exception.py` & `smo_rejection-0.5.4/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/smo_rejection/models.py` & `smo_rejection-0.5.4/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/smo_rejection/pdf_export.py` & `smo_rejection-0.5.4/smo_rejection/pdf_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from reportlab.lib.pagesizes import letter
 from reportlab.platypus import SimpleDocTemplate, Table, TableStyle, Paragraph, Spacer
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import inch
 from reportlab.lib import colors
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.pdfbase import pdfmetrics
-from .utils import calculate_mean_served_requests
+import io
 
-def export_to_pdf(results, filename):
+def export_to_pdf(results):
     """
     Экспортирует результаты симуляции в PDF-файл.
 
     ### Параметры:
     * `results (list)` - Список результатов симуляции.
-    * `filename (str)` - Имя файла для сохранения результатов.
 
-    ### Примечание:
-    Функция создает новый PDF-документ и записывает в него результаты симуляции.
+    ### Возвращает:
+    * `pdf_content (bytes)` - Содержимое PDF-файла в виде байтового объекта.
     """
     # Регистрация шрифта Arial для поддержки кириллицы
     pdfmetrics.registerFont(TTFont('Arial', 'arial.ttf'))
 
     # Получение стандартных стилей и добавление стилей для кириллицы
     styles = getSampleStyleSheet()
     styles.add(ParagraphStyle(name='Cyrillic', fontName='Arial', fontSize=10))
     styles.add(ParagraphStyle(name='CyrillicHeading3', fontName='Arial', fontSize=12, spaceAfter=6))
 
+    # Создание байтового объекта для записи PDF
+    pdf_bytes = io.BytesIO()
+
     # Создание документа PDF с указанным размером страницы и кодировкой
-    doc = SimpleDocTemplate(filename, pagesize=letter, encoding='UTF-8')
+    doc = SimpleDocTemplate(pdf_bytes, pagesize=letter, encoding='UTF-8')
     elements = []
 
     for i, result in enumerate(results, start=1):
         # Добавление заголовка для каждой симуляции
         header = Paragraph(f"----------------------------------------- Симуляция номер: {i} -----------------------------------------", styles["CyrillicHeading3"])
         elements.append(header)
 
@@ -64,7 +66,13 @@
 
     # Добавление среднего количества обслуженных заявок в конце документа
     mean_served = Paragraph(f"В качестве оценки искомого математического ожидания a – числа обслуженных заявок примем выборочную среднюю: a = {calculate_mean_served_requests(results)}", styles["Cyrillic"])
     elements.append(mean_served)
 
     # Построение и сохранение PDF документа
     doc.build(elements)
+
+    # Получение содержимого PDF в виде байтов
+    pdf_bytes.seek(0)  # Перематываем объект BytesIO в начало
+    pdf_content = pdf_bytes.getvalue()
+
+    return pdf_content
```

### Comparing `smo_rejection-0.4.4/smo_rejection/processing.py` & `smo_rejection-0.5.4/smo_rejection/processing.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/smo_rejection/simulation.py` & `smo_rejection-0.5.4/smo_rejection/simulation.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/smo_rejection/utils.py` & `smo_rejection-0.5.4/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/smo_rejection/xml_export.py` & `smo_rejection-0.5.4/smo_rejection/xml_export.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.4/PKG-INFO` & `smo_rejection-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.4.4
+Version: 0.5.4
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: reportlab (>=4.2.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # smo_rejection
 smo_rejection - это Python-библиотека для симуляции системы массового обслуживания (СМО) с отказами. Библиотека позволяет задавать различные параметры, такие как количество каналов обслуживания, время обслуживания заявок, интенсивность поступления заявок и общее время симуляции. После запуска симуляции библиотека предоставляет результаты, включая количество обслуженных и отклоненных заявок, а также подробную информацию о каждой заявке.
 
 
 ## Установка
```

