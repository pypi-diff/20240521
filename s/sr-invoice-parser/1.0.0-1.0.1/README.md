# Comparing `tmp/sr_invoice_parser-1.0.0.tar.gz` & `tmp/sr_invoice_parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sr_invoice_parser-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sr_invoice_parser-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sr_invoice_parser-1.0.0.tar` & `sr_invoice_parser-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,7 @@
--rw-r--r--   0        0        0      682 2024-04-08 23:31:24.766554 sr_invoice_parser-1.0.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0     3109 2024-04-08 23:22:50.000724 sr_invoice_parser-1.0.0/.gitignore
--rw-r--r--   0        0        0     1065 2024-04-08 17:07:56.026458 sr_invoice_parser-1.0.0/LICENSE
--rw-r--r--   0        0        0     3442 2024-04-09 00:03:12.560238 sr_invoice_parser-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-08 17:07:57.186790 sr_invoice_parser-1.0.0/conftest.py
--rw-r--r--   0        0        0      801 2024-04-08 23:30:00.171318 sr_invoice_parser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-04-08 23:31:16.989745 sr_invoice_parser-1.0.0/requirements.txt
--rw-r--r--   0        0        0      528 2024-04-09 00:06:32.762411 sr_invoice_parser-1.0.0/sr_invoice_parser/__init__.py
--rw-r--r--   0        0        0      478 2024-04-08 17:07:57.187362 sr_invoice_parser-1.0.0/sr_invoice_parser/decorators.py
--rw-r--r--   0        0        0      100 2024-04-08 17:07:57.187451 sr_invoice_parser-1.0.0/sr_invoice_parser/exceptions.py
--rw-r--r--   0        0        0     7080 2024-04-08 22:47:00.020130 sr_invoice_parser-1.0.0/sr_invoice_parser/parser.py
--rw-r--r--   0        0        0    23152 2024-04-08 23:54:28.033672 sr_invoice_parser-1.0.0/tests/example_response.html
--rw-r--r--   0        0        0    19322 2024-04-08 23:54:21.627350 sr_invoice_parser-1.0.0/tests/test_parser.py
--rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 sr_invoice_parser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3639 2024-05-21 19:09:46.997163 sr_invoice_parser-1.0.1/README.md
+-rw-r--r--   0        0        0      801 2024-04-08 23:30:00.171318 sr_invoice_parser-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      528 2024-05-21 19:09:58.668824 sr_invoice_parser-1.0.1/sr_invoice_parser/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-08 17:07:57.187362 sr_invoice_parser-1.0.1/sr_invoice_parser/decorators.py
+-rw-r--r--   0        0        0      100 2024-04-08 17:07:57.187451 sr_invoice_parser-1.0.1/sr_invoice_parser/exceptions.py
+-rw-r--r--   0        0        0     7497 2024-05-21 19:09:45.105301 sr_invoice_parser-1.0.1/sr_invoice_parser/parser.py
+-rw-r--r--   0        0        0     4496 1970-01-01 00:00:00.000000 sr_invoice_parser-1.0.1/PKG-INFO
```

### Comparing `sr_invoice_parser-1.0.0/README.md` & `sr_invoice_parser-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SR Invoice Parser
 
 [![build-status-image]][build-status]
 
 SR Invoice Parser is a small library that is parsing invoices and extracting relevant information.
-It is designed to work with invoices from the Tax Administration of the Republic of Serbia (Poreska uprava Republike Srbije).
+It is designed to work with invoices from the TaxCore Tax Administration of the Republic of Serbia (Poreska uprava Republike Srbije).
 
-- https://purs.gov.rs/
-- https://suf.purs.gov.rs/
+It works on domain [suf.purs.gov.rs](https://suf.purs.gov.rs/) where they use TaxCore website to show invoices.
 
 QR code gives a URL to the invoice web page, and this parser extracts the relevant information from the web page, like a crawler.
 
 ## Installation
 
 To install SR Invoice Parser, follow these steps:
 
@@ -21,14 +20,15 @@
 The `InvoiceParser` class is the entry point for using the parser.
 
 ### Methods
 
 - `get_data()` - Extracts all the data from the invoice and returns it as a dictionary
 - `get_company_name()` - Extracts the company name.
 - `get_company_tin()` - Extracts the company's tax identification number/PFR.
+- `get_buyer_tin()` - Extracts the buyer's tax identification number/PFR.
 - `get_total_amount()` - Extracts the total amount of the invoice.
 - `get_dt()` - Extracts the date and time of the invoice and converts it to UTC as a datetime object.
 - `get_invoice_number()` - Extracts the invoice number.
 - `get_invoice_text()` - Extracts the full text of the invoice with QR code base64.
 - `get_items()` - Extracts items details from the invoice. This is array of dictionaries with keys: `name`, `quantity`, `price`, `total_price`.
 
 Here's a basic example of how to use it:
@@ -40,28 +40,30 @@
 # or
 parser = InvoiceParser(html_text="<HTML source code of invoice web page>")
 
 parser.data()
 
 parser.get_company_name()
 parser.get_company_tin()
+parser.get_buyer_tin()
 parser.get_total_amount()
 parser.get_dt()
 parser.get_invoice_number()
 parser.get_invoice_text()
 parser.get_items()
 
 ```
 
 ## Example response data
 
 ```python
 {
     "company_name": "Company Name",
     "company_tin": "123456789",
+    "buyer_tin": "987654321",
     "invoice_number": "QWERTYU1-QWERTYU1-12345",
     "invoice_datetime": datetime.datetime(2021, 1, 1, 0, 0, tzinfo=datetime.timezone.utc),
     "invoice_total_amount": 123.45,
     "invoice_text": "============ ФИСКАЛНИ РАЧУН ============.....",
     "invoice_items": [
         {
             "name": "Item 1",
```

### Comparing `sr_invoice_parser-1.0.0/pyproject.toml` & `sr_invoice_parser-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sr_invoice_parser-1.0.0/sr_invoice_parser/__init__.py` & `sr_invoice_parser-1.0.1/sr_invoice_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """SR Invoice Parser is a small library(crawler) that is parsing invoices and extracting relevant information from URL. For Serbian market."""
 
 __title__ = "sr_invoice_parser"
 __author__ = "Innovigo"
 __website__ = "https://wwwinnovigo.co/"
 __email__ = "hello@innovigo.co"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 VERSION = __version__
 
 from .exceptions import ParserParseException, ParserRequestException  # noqa: E402
 from .parser import InvoiceParser  # noqa: E402
 
 __all__ = ["InvoiceParser", "ParserRequestException", "ParserParseException"]
```

### Comparing `sr_invoice_parser-1.0.0/sr_invoice_parser/parser.py` & `sr_invoice_parser-1.0.1/sr_invoice_parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,25 @@
     @handle_exception()
     def get_company_tin(self) -> str:
         """Get the company tin/tax identification number"""
 
         value = self.html_selector.css("span#tinLabel::text").get().strip()
         return value
 
+    @handle_exception()
+    def get_buyer_tin(self) -> str:
+        """Get the buyer tin/tax identification number"""
+
+        value = self.html_selector.css("span#buyerIdLabel::text").get().strip()
+        if value:
+            value = value.split(":")
+            if len(value) == 2:
+                return value[1]
+        return value
+
     def string_to_float(self, string: str) -> float:
         return float(string.replace(".", "").replace(",", "."))
 
     @handle_exception()
     def get_total_amount(self) -> float:
         """Get the total amount of the invoice"""
 
@@ -192,21 +203,23 @@
         return items
 
     def data(self) -> dict:
         """Parse and return the data from the invoice"""
 
         company_name = self.get_company_name()
         company_tin = self.get_company_tin()
+        buyer_tin = self.get_buyer_tin()
         total_amount = self.get_total_amount()
         invoice_number = self.get_invoice_number()
         invoice_text = self.get_invoice_text()
         invoice_items = self.get_items(invoice_text)
         dt = self.get_dt()
         return {
             "company_name": company_name,
             "company_tin": company_tin,
+            "buyer_tin": buyer_tin,
             "invoice_number": invoice_number,
             "invoice_datetime": dt,
             "invoice_total_amount": total_amount,
             "invoice_items": invoice_items,
             "invoice_text": invoice_text,
         }
```

### Comparing `sr_invoice_parser-1.0.0/PKG-INFO` & `sr_invoice_parser-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sr-invoice-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: SR Invoice Parser is a small library(crawler) that is parsing invoices and extracting relevant information from URL. For Serbian market.
 Author-email: Innovigo <hello@innovigo.co>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,17 @@
 Project-URL: Source, https://github.com/Innovigo/sr-invoice-parser
 
 # SR Invoice Parser
 
 [![build-status-image]][build-status]
 
 SR Invoice Parser is a small library that is parsing invoices and extracting relevant information.
-It is designed to work with invoices from the Tax Administration of the Republic of Serbia (Poreska uprava Republike Srbije).
+It is designed to work with invoices from the TaxCore Tax Administration of the Republic of Serbia (Poreska uprava Republike Srbije).
 
-- https://purs.gov.rs/
-- https://suf.purs.gov.rs/
+It works on domain [suf.purs.gov.rs](https://suf.purs.gov.rs/) where they use TaxCore website to show invoices.
 
 QR code gives a URL to the invoice web page, and this parser extracts the relevant information from the web page, like a crawler.
 
 ## Installation
 
 To install SR Invoice Parser, follow these steps:
 
@@ -40,14 +39,15 @@
 The `InvoiceParser` class is the entry point for using the parser.
 
 ### Methods
 
 - `get_data()` - Extracts all the data from the invoice and returns it as a dictionary
 - `get_company_name()` - Extracts the company name.
 - `get_company_tin()` - Extracts the company's tax identification number/PFR.
+- `get_buyer_tin()` - Extracts the buyer's tax identification number/PFR.
 - `get_total_amount()` - Extracts the total amount of the invoice.
 - `get_dt()` - Extracts the date and time of the invoice and converts it to UTC as a datetime object.
 - `get_invoice_number()` - Extracts the invoice number.
 - `get_invoice_text()` - Extracts the full text of the invoice with QR code base64.
 - `get_items()` - Extracts items details from the invoice. This is array of dictionaries with keys: `name`, `quantity`, `price`, `total_price`.
 
 Here's a basic example of how to use it:
@@ -59,28 +59,30 @@
 # or
 parser = InvoiceParser(html_text="<HTML source code of invoice web page>")
 
 parser.data()
 
 parser.get_company_name()
 parser.get_company_tin()
+parser.get_buyer_tin()
 parser.get_total_amount()
 parser.get_dt()
 parser.get_invoice_number()
 parser.get_invoice_text()
 parser.get_items()
 
 ```
 
 ## Example response data
 
 ```python
 {
     "company_name": "Company Name",
     "company_tin": "123456789",
+    "buyer_tin": "987654321",
     "invoice_number": "QWERTYU1-QWERTYU1-12345",
     "invoice_datetime": datetime.datetime(2021, 1, 1, 0, 0, tzinfo=datetime.timezone.utc),
     "invoice_total_amount": 123.45,
     "invoice_text": "============ ФИСКАЛНИ РАЧУН ============.....",
     "invoice_items": [
         {
             "name": "Item 1",
```

