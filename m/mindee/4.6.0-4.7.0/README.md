# Comparing `tmp/mindee-4.6.0.tar.gz` & `tmp/mindee-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-4.6.0.tar", last modified: Tue Apr 30 16:18:17 2024, max compression
+gzip compressed data, was "mindee-4.7.0.tar", last modified: Tue May 21 08:46:19 2024, max compression
```

## Comparing `mindee-4.6.0.tar` & `mindee-4.7.0.tar`

### file list

```diff
@@ -1,336 +1,340 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-30 16:17:59.000000 mindee-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-30 16:18:17.244418 mindee-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-30 16:17:59.000000 mindee-4.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/error/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/geometry_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/mimetype_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/mindee_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/error/mindee_http_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/polygon_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/geometry/quadrilateral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.204418 mindee-4.6.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/mindee_http/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/base_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/mindee_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/mindee_http/response_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/parsing/common/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/async_predict_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.208418 mindee-4.6.0/mindee/parsing/common/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/extras/cropper_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/extras/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/feedback_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/common/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/mvision_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/ocr/ocr_word.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/predict_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/product.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/string_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/common/summary_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/line_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/custom/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/generated/generated_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/generated/generated_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/parsing/standard/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/position.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/parsing/standard/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.212418 mindee-4.6.0/mindee/product/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/barcode_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/barcode_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/cropper/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/cropper_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/cropper/cropper_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/custom/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/custom_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/custom/custom_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/eu/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/eu/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/financial_document/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/financial_document_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/financial_document/financial_document_v1_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.216418 mindee-4.6.0/mindee/product/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.220418 mindee-4.6.0/mindee/product/fr/petrol_receipt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/generated/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/generated/generated_v1_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/international_id/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/international_id/international_id_v2_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/invoice_v4_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice/invoice_v4_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/material_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/material_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/multi_receipts_detector/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/multi_receipts_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.224418 mindee-4.6.0/mindee/product/passport/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/passport/passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/passport/passport_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1_document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/receipt/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v4_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v5_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/receipt/receipt_v5_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/resume/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_education.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_professional_experience.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/resume/resume_v1_social_networks_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/us/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.228418 mindee-4.6.0/mindee/product/us/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/mindee/product/us/w9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/w9_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/w9_v1_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/product/us/w9/w9_v1_page.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-30 16:17:59.000000 mindee-4.6.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:18:03.000000 mindee-4.6.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 16:18:17.000000 mindee-4.6.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-30 16:17:59.000000 mindee-4.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-30 16:18:17.248418 mindee-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-30 16:17:59.000000 mindee-4.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_ocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/fields/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/product/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.232418 mindee-4.6.0/tests/product/barcode_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/barcode_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/cropper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/cropper/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/cropper/test_cropper_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/eu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/eu/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/driver_license/test_driver_license_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.236418 mindee-4.6.0/tests/product/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/international_id/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/international_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/international_id/test_international_id_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/international_id/test_international_id_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/invoice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/invoice/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/invoice/test_invoice_v4_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/material_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/material_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/material_certificate/test_material_certificate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/multi_receipts_detector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/multi_receipts_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/passport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/passport/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/passport/test_passport_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/proof_of_address/test_proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/receipt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v4_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/receipt/test_receipt_v5_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/resume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/resume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/resume/test_resume_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/us/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.240418 mindee-4.6.0/tests/product/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/tests/product/us/driver_license/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/driver_license/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:18:17.244418 mindee-4.6.0/tests/product/us/w9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/w9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/w9/test_w9_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/product/us/w9/test_w9_v1_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-30 16:17:59.000000 mindee-4.6.0/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 08:45:58.000000 mindee-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-21 08:46:19.922949 mindee-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-21 08:45:58.000000 mindee-4.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.874949 mindee-4.7.0/mindee/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18091 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/geometry_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/mimetype_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/mindee_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/error/mindee_http_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/polygon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/geometry/quadrilateral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/mindee_http/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/base_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/mindee_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/mindee_http/response_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.878949 mindee-4.7.0/mindee/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.882949 mindee-4.7.0/mindee/parsing/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/async_predict_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.882949 mindee-4.7.0/mindee/parsing/common/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/extras/cropper_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/extras/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/feedback_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.882949 mindee-4.7.0/mindee/parsing/common/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/mvision_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/ocr/ocr_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/predict_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/string_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/common/summary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/parsing/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/line_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/custom/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/parsing/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/generated/generated_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/generated/generated_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/parsing/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/parsing/standard/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.886949 mindee-4.7.0/mindee/product/barcode_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/barcode_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/cropper/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/cropper_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/cropper/cropper_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/custom_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/custom/custom_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/eu/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/financial_document_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/financial_document/financial_document_v1_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.890949 mindee-4.7.0/mindee/product/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.894949 mindee-4.7.0/mindee/product/fr/petrol_receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/generated/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/generated/generated_v1_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/international_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/international_id/international_id_v2_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/invoice_v4_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice/invoice_v4_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/material_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/material_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.898949 mindee-4.7.0/mindee/product/multi_receipts_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/multi_receipts_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/passport/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/passport/passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/passport/passport_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1_document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v4_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v5_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/receipt/receipt_v5_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/resume/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_education.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_professional_experience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/resume/resume_v1_social_networks_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.902949 mindee-4.7.0/mindee/product/us/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/mindee/product/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/mindee/product/us/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/mindee/product/us/w9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/w9_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/w9_v1_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/product/us/w9/w9_v1_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-21 08:45:58.000000 mindee-4.7.0/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:46:04.000000 mindee-4.7.0/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 08:46:19.000000 mindee-4.7.0/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-21 08:45:58.000000 mindee-4.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-21 08:46:19.926950 mindee-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 08:45:58.000000 mindee-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.906949 mindee-4.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/fields/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/barcode_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/barcode_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/cropper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/cropper/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/cropper/test_cropper_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/eu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/eu/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/driver_license/test_driver_license_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.910949 mindee-4.7.0/tests/product/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/financial_document/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/financial_document/test_financial_document_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.914949 mindee-4.7.0/tests/product/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/international_id/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/international_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/international_id/test_international_id_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/international_id/test_international_id_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/invoice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/invoice/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/invoice/test_invoice_v4_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/material_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/material_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/material_certificate/test_material_certificate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/multi_receipts_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/multi_receipts_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/passport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/passport/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/passport/test_passport_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/proof_of_address/test_proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/receipt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v4_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/receipt/test_receipt_v5_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/resume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/resume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/resume/test_resume_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.918949 mindee-4.7.0/tests/product/us/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/tests/product/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/tests/product/us/driver_license/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/driver_license/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:46:19.922949 mindee-4.7.0/tests/product/us/w9/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/w9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/w9/test_w9_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/product/us/w9/test_w9_v1_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 08:45:58.000000 mindee-4.7.0/tests/test_pkg_versions.py
```

### Comparing `mindee-4.6.0/LICENSE` & `mindee-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/PKG-INFO` & `mindee-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 4.6.0
+Version: 4.7.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: opensource@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-4.6.0/README.md` & `mindee-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/cli.py` & `mindee-4.7.0/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/client.py` & `mindee-4.7.0/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/error/mindee_error.py` & `mindee-4.7.0/mindee/error/mindee_error.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/error/mindee_http_error.py` & `mindee-4.7.0/mindee/error/mindee_http_error.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/geometry/__init__.py` & `mindee-4.7.0/mindee/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/geometry/bbox.py` & `mindee-4.7.0/mindee/geometry/bbox.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/geometry/minmax.py` & `mindee-4.7.0/mindee/geometry/minmax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/geometry/polygon.py` & `mindee-4.7.0/mindee/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/geometry/polygon_utils.py` & `mindee-4.7.0/mindee/geometry/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/geometry/quadrilateral.py` & `mindee-4.7.0/mindee/geometry/quadrilateral.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/input/page_options.py` & `mindee-4.7.0/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/input/sources.py` & `mindee-4.7.0/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/mindee_http/endpoint.py` & `mindee-4.7.0/mindee/mindee_http/endpoint.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/mindee_http/mindee_api.py` & `mindee-4.7.0/mindee/mindee_http/mindee_api.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/mindee_http/response_validation.py` & `mindee-4.7.0/mindee/mindee_http/response_validation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/__init__.py` & `mindee-4.7.0/mindee/parsing/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/api_request.py` & `mindee-4.7.0/mindee/parsing/common/api_request.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/api_response.py` & `mindee-4.7.0/mindee/parsing/common/api_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/async_predict_response.py` & `mindee-4.7.0/mindee/parsing/common/async_predict_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/document.py` & `mindee-4.7.0/mindee/parsing/common/document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/extras/cropper_extra.py` & `mindee-4.7.0/mindee/parsing/common/extras/cropper_extra.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/extras/extras.py` & `mindee-4.7.0/mindee/parsing/common/extras/extras.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/inference.py` & `mindee-4.7.0/mindee/parsing/common/inference.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/job.py` & `mindee-4.7.0/mindee/parsing/common/job.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/ocr/ocr_page.py` & `mindee-4.7.0/mindee/parsing/common/ocr/ocr_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/ocr/ocr_word.py` & `mindee-4.7.0/mindee/parsing/common/ocr/ocr_word.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/orientation.py` & `mindee-4.7.0/mindee/parsing/common/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/page.py` & `mindee-4.7.0/mindee/parsing/common/page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/predict_response.py` & `mindee-4.7.0/mindee/parsing/common/predict_response.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/prediction.py` & `mindee-4.7.0/mindee/parsing/common/prediction.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/common/summary_helper.py` & `mindee-4.7.0/mindee/parsing/common/summary_helper.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/custom/line_items.py` & `mindee-4.7.0/mindee/parsing/custom/line_items.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/custom/list.py` & `mindee-4.7.0/mindee/parsing/custom/list.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/generated/generated_list.py` & `mindee-4.7.0/mindee/parsing/generated/generated_list.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/generated/generated_object.py` & `mindee-4.7.0/mindee/parsing/generated/generated_object.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/__init__.py` & `mindee-4.7.0/mindee/parsing/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/amount.py` & `mindee-4.7.0/mindee/parsing/standard/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/base.py` & `mindee-4.7.0/mindee/parsing/standard/base.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/classification.py` & `mindee-4.7.0/mindee/parsing/standard/classification.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/company_registration.py` & `mindee-4.7.0/mindee/parsing/standard/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/date.py` & `mindee-4.7.0/mindee/parsing/standard/date.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/locale.py` & `mindee-4.7.0/mindee/parsing/standard/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/payment_details.py` & `mindee-4.7.0/mindee/parsing/standard/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/position.py` & `mindee-4.7.0/mindee/parsing/standard/position.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/tax.py` & `mindee-4.7.0/mindee/parsing/standard/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/parsing/standard/text.py` & `mindee-4.7.0/mindee/parsing/standard/text.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/__init__.py` & `mindee-4.7.0/mindee/product/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1.py` & `mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/barcode_reader/barcode_reader_v1_document.py` & `mindee-4.7.0/mindee/product/barcode_reader/barcode_reader_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/cropper/cropper_v1.py` & `mindee-4.7.0/mindee/product/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/cropper/cropper_v1_page.py` & `mindee-4.7.0/mindee/product/cropper/cropper_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/custom/custom_v1.py` & `mindee-4.7.0/mindee/product/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/custom/custom_v1_document.py` & `mindee-4.7.0/mindee/product/custom/custom_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/custom/custom_v1_page.py` & `mindee-4.7.0/mindee/product/custom/custom_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1.py` & `mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_document.py` & `mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/eu/driver_license/driver_license_v1_page.py` & `mindee-4.7.0/mindee/product/eu/driver_license/driver_license_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1.py` & `mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/eu/license_plate/license_plate_v1_document.py` & `mindee-4.7.0/mindee/product/eu/license_plate/license_plate_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/financial_document/financial_document_v1.py` & `mindee-4.7.0/mindee/product/financial_document/financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/financial_document/financial_document_v1_document.py` & `mindee-4.7.0/mindee/product/financial_document/financial_document_v1_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from mindee.product.financial_document.financial_document_v1_line_item import (
     FinancialDocumentV1LineItem,
 )
 
 
 class FinancialDocumentV1Document(Prediction):
-    """Financial Document API version 1.6 document data."""
+    """Financial Document API version 1.7 document data."""
 
     billing_address: StringField
     """The customer's address used for billing."""
     category: ClassificationField
     """The purchase category among predefined classes."""
     customer_address: StringField
     """The address of the customer."""
@@ -29,24 +29,28 @@
     """List of company registrations associated to the customer."""
     customer_id: StringField
     """The customer account number or identifier from the supplier."""
     customer_name: StringField
     """The name of the customer."""
     date: DateField
     """The date the purchase was made."""
+    document_number: StringField
+    """The document number or identifier."""
     document_type: ClassificationField
     """One of: 'INVOICE', 'CREDIT NOTE', 'CREDIT CARD RECEIPT', 'EXPENSE RECEIPT'."""
     due_date: DateField
     """The date on which the payment is due."""
     invoice_number: StringField
-    """The invoice number or identifier."""
+    """The invoice number or identifier only if document is an invoice."""
     line_items: List[FinancialDocumentV1LineItem]
     """List of line item details."""
     locale: LocaleField
     """The locale detected on the document."""
+    receipt_number: StringField
+    """The receipt number or identifier only if document is a receipt."""
     reference_numbers: List[StringField]
     """List of Reference numbers, including PO number."""
     shipping_address: StringField
     """The customer's address used for shipping."""
     subcategory: ClassificationField
     """The purchase subcategory among predefined classes for transport and food."""
     supplier_address: StringField
@@ -112,14 +116,18 @@
             raw_prediction["customer_name"],
             page_id=page_id,
         )
         self.date = DateField(
             raw_prediction["date"],
             page_id=page_id,
         )
+        self.document_number = StringField(
+            raw_prediction["document_number"],
+            page_id=page_id,
+        )
         self.document_type = ClassificationField(
             raw_prediction["document_type"],
             page_id=page_id,
         )
         self.due_date = DateField(
             raw_prediction["due_date"],
             page_id=page_id,
@@ -132,14 +140,18 @@
             FinancialDocumentV1LineItem(prediction, page_id=page_id)
             for prediction in raw_prediction["line_items"]
         ]
         self.locale = LocaleField(
             raw_prediction["locale"],
             page_id=page_id,
         )
+        self.receipt_number = StringField(
+            raw_prediction["receipt_number"],
+            page_id=page_id,
+        )
         self.reference_numbers = [
             StringField(prediction, page_id=page_id)
             for prediction in raw_prediction["reference_numbers"]
         ]
         self.shipping_address = StringField(
             raw_prediction["shipping_address"],
             page_id=page_id,
@@ -242,14 +254,16 @@
             [str(item) for item in self.supplier_company_registrations],
         )
         supplier_payment_details = f"\n { ' ' * 26 }".join(
             [str(item) for item in self.supplier_payment_details],
         )
         out_str: str = f":Locale: {self.locale}\n"
         out_str += f":Invoice Number: {self.invoice_number}\n"
+        out_str += f":Receipt Number: {self.receipt_number}\n"
+        out_str += f":Document Number: {self.document_number}\n"
         out_str += f":Reference Numbers: {reference_numbers}\n"
         out_str += f":Purchase Date: {self.date}\n"
         out_str += f":Due Date: {self.due_date}\n"
         out_str += f":Total Net: {self.total_net}\n"
         out_str += f":Total Amount: {self.total_amount}\n"
         out_str += f":Taxes: {self.taxes}\n"
         out_str += f":Supplier Payment Details: {supplier_payment_details}\n"
```

### Comparing `mindee-4.6.0/mindee/product/financial_document/financial_document_v1_line_item.py` & `mindee-4.7.0/mindee/product/financial_document/financial_document_v1_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/__init__.py` & `mindee-4.7.0/mindee/product/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py` & `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py` & `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py` & `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py` & `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_bban.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py` & `mindee-4.7.0/mindee/product/fr/bank_account_details/bank_account_details_v2_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1.py` & `mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py` & `mindee-4.7.0/mindee/product/fr/carte_grise/carte_grise_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py` & `mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py` & `mindee-4.7.0/mindee/product/fr/carte_vitale/carte_vitale_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/id_card/id_card_v1.py` & `mindee-4.7.0/mindee/product/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_document.py` & `mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/id_card/id_card_v1_page.py` & `mindee-4.7.0/mindee/product/fr/id_card/id_card_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/id_card/id_card_v2.py` & `mindee-4.7.0/mindee/product/fr/id_card/id_card_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_document.py` & `mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/id_card/id_card_v2_page.py` & `mindee-4.7.0/mindee/product/fr/id_card/id_card_v2_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py` & `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py` & `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py` & `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_fuel.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py` & `mindee-4.7.0/mindee/product/fr/petrol_receipt/petrol_receipt_v1_total.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/generated/generated_v1.py` & `mindee-4.7.0/mindee/product/generated/generated_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/generated/generated_v1_document.py` & `mindee-4.7.0/mindee/product/generated/generated_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/generated/generated_v1_page.py` & `mindee-4.7.0/mindee/product/generated/generated_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/generated/generated_v1_prediction.py` & `mindee-4.7.0/mindee/product/generated/generated_v1_prediction.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/international_id/international_id_v1.py` & `mindee-4.7.0/mindee/product/international_id/international_id_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/international_id/international_id_v1_document.py` & `mindee-4.7.0/mindee/product/international_id/international_id_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/international_id/international_id_v2.py` & `mindee-4.7.0/mindee/product/international_id/international_id_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/international_id/international_id_v2_document.py` & `mindee-4.7.0/mindee/product/international_id/international_id_v2_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/invoice/invoice_v4.py` & `mindee-4.7.0/mindee/product/invoice/invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/invoice/invoice_v4_document.py` & `mindee-4.7.0/mindee/product/invoice/invoice_v4_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/invoice/invoice_v4_line_item.py` & `mindee-4.7.0/mindee/product/invoice/invoice_v4_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1.py` & `mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py` & `mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py` & `mindee-4.7.0/mindee/product/invoice_splitter/invoice_splitter_v1_page_group.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1.py` & `mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/material_certificate/material_certificate_v1_document.py` & `mindee-4.7.0/mindee/product/material_certificate/material_certificate_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py` & `mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py` & `mindee-4.7.0/mindee/product/multi_receipts_detector/multi_receipts_detector_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/passport/passport_v1.py` & `mindee-4.7.0/mindee/product/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/passport/passport_v1_document.py` & `mindee-4.7.0/mindee/product/passport/passport_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1.py` & `mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/proof_of_address/proof_of_address_v1_document.py` & `mindee-4.7.0/mindee/product/proof_of_address/proof_of_address_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/receipt/receipt_v4.py` & `mindee-4.7.0/mindee/product/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/receipt/receipt_v4_document.py` & `mindee-4.7.0/mindee/product/receipt/receipt_v4_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/receipt/receipt_v5.py` & `mindee-4.7.0/mindee/product/receipt/receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/receipt/receipt_v5_document.py` & `mindee-4.7.0/mindee/product/receipt/receipt_v5_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,28 @@
     StringField,
     Taxes,
 )
 from mindee.product.receipt.receipt_v5_line_item import ReceiptV5LineItem
 
 
 class ReceiptV5Document(Prediction):
-    """Receipt API version 5.1 document data."""
+    """Receipt API version 5.2 document data."""
 
     category: ClassificationField
     """The purchase category among predefined classes."""
     date: DateField
     """The date the purchase was made."""
     document_type: ClassificationField
     """One of: 'CREDIT CARD RECEIPT', 'EXPENSE RECEIPT'."""
     line_items: List[ReceiptV5LineItem]
     """List of line item details."""
     locale: LocaleField
     """The locale detected on the document."""
+    receipt_number: StringField
+    """The receipt number or identifier."""
     subcategory: ClassificationField
     """The purchase subcategory among predefined classes for transport and food."""
     supplier_address: StringField
     """The address of the supplier or merchant."""
     supplier_company_registrations: List[CompanyRegistrationField]
     """List of company registrations associated to the supplier."""
     supplier_name: StringField
@@ -77,14 +79,18 @@
             ReceiptV5LineItem(prediction, page_id=page_id)
             for prediction in raw_prediction["line_items"]
         ]
         self.locale = LocaleField(
             raw_prediction["locale"],
             page_id=page_id,
         )
+        self.receipt_number = StringField(
+            raw_prediction["receipt_number"],
+            page_id=page_id,
+        )
         self.subcategory = ClassificationField(
             raw_prediction["subcategory"],
             page_id=page_id,
         )
         self.supplier_address = StringField(
             raw_prediction["supplier_address"],
             page_id=page_id,
@@ -167,9 +173,10 @@
         out_str += f":Taxes: {self.taxes}\n"
         out_str += f":Supplier Name: {self.supplier_name}\n"
         out_str += (
             f":Supplier Company Registrations: {supplier_company_registrations}\n"
         )
         out_str += f":Supplier Address: {self.supplier_address}\n"
         out_str += f":Supplier Phone Number: {self.supplier_phone_number}\n"
+        out_str += f":Receipt Number: {self.receipt_number}\n"
         out_str += f":Line Items: {self._line_items_to_str()}\n"
         return clean_out_string(out_str)
```

### Comparing `mindee-4.6.0/mindee/product/receipt/receipt_v5_line_item.py` & `mindee-4.7.0/mindee/product/receipt/receipt_v5_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/__init__.py` & `mindee-4.7.0/mindee/product/resume/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1.py` & `mindee-4.7.0/mindee/product/resume/resume_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1_certificate.py` & `mindee-4.7.0/mindee/product/resume/resume_v1_certificate.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1_document.py` & `mindee-4.7.0/mindee/product/resume/resume_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1_education.py` & `mindee-4.7.0/mindee/product/resume/resume_v1_education.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1_language.py` & `mindee-4.7.0/mindee/product/resume/resume_v1_language.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1_professional_experience.py` & `mindee-4.7.0/mindee/product/resume/resume_v1_professional_experience.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/resume/resume_v1_social_networks_url.py` & `mindee-4.7.0/mindee/product/resume/resume_v1_social_networks_url.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/__init__.py` & `mindee-4.7.0/mindee/product/us/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1.py` & `mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_document.py` & `mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/bank_check/bank_check_v1_page.py` & `mindee-4.7.0/mindee/product/us/bank_check/bank_check_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1.py` & `mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_document.py` & `mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_document.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/driver_license/driver_license_v1_page.py` & `mindee-4.7.0/mindee/product/us/driver_license/driver_license_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/w9/w9_v1.py` & `mindee-4.7.0/mindee/product/us/w9/w9_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/product/us/w9/w9_v1_page.py` & `mindee-4.7.0/mindee/product/us/w9/w9_v1_page.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee/versions.py` & `mindee-4.7.0/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/mindee.egg-info/PKG-INFO` & `mindee-4.7.0/mindee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 4.6.0
+Version: 4.7.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: opensource@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-4.6.0/mindee.egg-info/SOURCES.txt` & `mindee-4.7.0/mindee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,17 @@
 tests/product/cropper/test_cropper_v1_regression.py
 tests/product/eu/__init__.py
 tests/product/eu/driver_license/__init__.py
 tests/product/eu/driver_license/test_driver_license_v1.py
 tests/product/eu/license_plate/__init__.py
 tests/product/eu/license_plate/test_license_plate_v1.py
 tests/product/eu/license_plate/test_license_plate_v1_regression.py
+tests/product/financial_document/__init__.py
+tests/product/financial_document/test_financial_document_v1.py
+tests/product/financial_document/test_financial_document_v1_regression.py
 tests/product/fr/__init__.py
 tests/product/fr/bank_account_details/__init__.py
 tests/product/fr/bank_account_details/test_bank_account_details_v1.py
 tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py
 tests/product/fr/bank_account_details/test_bank_account_details_v2.py
 tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py
 tests/product/fr/carte_grise/__init__.py
```

### Comparing `mindee-4.6.0/pyproject.toml` & `mindee-4.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/setup.cfg` & `mindee-4.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_amount.py` & `mindee-4.7.0/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_date.py` & `mindee-4.7.0/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_field.py` & `mindee-4.7.0/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_locale.py` & `mindee-4.7.0/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_orientation.py` & `mindee-4.7.0/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_payment_details.py` & `mindee-4.7.0/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_position.py` & `mindee-4.7.0/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_tax.py` & `mindee-4.7.0/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/fields/test_text.py` & `mindee-4.7.0/tests/fields/test_text.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/__init__.py` & `mindee-4.7.0/tests/product/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1.py` & `mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py` & `mindee-4.7.0/tests/product/barcode_reader/test_barcode_reader_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/cropper/test_cropper_v1.py` & `mindee-4.7.0/tests/product/cropper/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/cropper/test_cropper_v1_regression.py` & `mindee-4.7.0/tests/product/cropper/test_cropper_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/eu/driver_license/test_driver_license_v1.py` & `mindee-4.7.0/tests/product/eu/driver_license/test_driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1.py` & `mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py` & `mindee-4.7.0/tests/product/eu/license_plate/test_license_plate_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py` & `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py` & `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py` & `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py` & `mindee-4.7.0/tests/product/fr/bank_account_details/test_bank_account_details_v2_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1.py` & `mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py` & `mindee-4.7.0/tests/product/fr/carte_grise/test_carte_grise_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py` & `mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py` & `mindee-4.7.0/tests/product/fr/carte_vitale/test_carte_vitale_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1.py` & `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v1_regression.py` & `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2.py` & `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/fr/id_card/test_id_card_v2_regression.py` & `mindee-4.7.0/tests/product/fr/id_card/test_id_card_v2_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/international_id/test_international_id_v1.py` & `mindee-4.7.0/tests/product/international_id/test_international_id_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/international_id/test_international_id_v2.py` & `mindee-4.7.0/tests/product/international_id/test_international_id_v2.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/invoice/test_invoice_v4.py` & `mindee-4.7.0/tests/product/invoice/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/invoice/test_invoice_v4_regression.py` & `mindee-4.7.0/tests/product/invoice/test_invoice_v4_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/material_certificate/test_material_certificate_v1.py` & `mindee-4.7.0/tests/product/material_certificate/test_material_certificate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py` & `mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py` & `mindee-4.7.0/tests/product/multi_receipts_detector/test_multi_receipts_detector_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/passport/test_passport_v1.py` & `mindee-4.7.0/tests/product/passport/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/passport/test_passport_v1_regression.py` & `mindee-4.7.0/tests/product/passport/test_passport_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/proof_of_address/test_proof_of_address_v1.py` & `mindee-4.7.0/tests/product/proof_of_address/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/receipt/test_receipt_v4.py` & `mindee-4.7.0/tests/product/receipt/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/receipt/test_receipt_v4_regression.py` & `mindee-4.7.0/tests/product/receipt/test_receipt_v4_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/receipt/test_receipt_v5.py` & `mindee-4.7.0/tests/product/receipt/test_receipt_v5.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,8 +51,9 @@
     assert prediction.total_tax.value is None
     assert prediction.tip.value is None
     assert len(prediction.taxes) == 0
     assert prediction.supplier_name.value is None
     assert len(prediction.supplier_company_registrations) == 0
     assert prediction.supplier_address.value is None
     assert prediction.supplier_phone_number.value is None
+    assert prediction.receipt_number.value is None
     assert len(prediction.line_items) == 0
```

### Comparing `mindee-4.6.0/tests/product/receipt/test_receipt_v5_regression.py` & `mindee-4.7.0/tests/product/receipt/test_receipt_v5_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/resume/test_resume_v1.py` & `mindee-4.7.0/tests/product/resume/test_resume_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1.py` & `mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/us/bank_check/test_bank_check_v1_regression.py` & `mindee-4.7.0/tests/product/us/bank_check/test_bank_check_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1.py` & `mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/us/driver_license/test_driver_license_v1_regression.py` & `mindee-4.7.0/tests/product/us/driver_license/test_driver_license_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/us/w9/test_w9_v1.py` & `mindee-4.7.0/tests/product/us/w9/test_w9_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/product/us/w9/test_w9_v1_regression.py` & `mindee-4.7.0/tests/product/us/w9/test_w9_v1_regression.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/test_cli.py` & `mindee-4.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/test_client.py` & `mindee-4.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/test_geometry.py` & `mindee-4.7.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/test_inputs.py` & `mindee-4.7.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-4.6.0/tests/test_pkg_versions.py` & `mindee-4.7.0/tests/test_pkg_versions.py`

 * *Files identical despite different names*

