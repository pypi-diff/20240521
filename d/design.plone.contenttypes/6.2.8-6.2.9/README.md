# Comparing `tmp/design.plone.contenttypes-6.2.8.tar.gz` & `tmp/design_plone_contenttypes-6.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.contenttypes-6.2.8.tar", last modified: Mon Apr 22 12:15:12 2024, max compression
+gzip compressed data, was "design_plone_contenttypes-6.2.9.tar", last modified: Tue May 21 15:00:05 2024, max compression
```

## Comparing `design.plone.contenttypes-6.2.8.tar` & `design_plone_contenttypes-6.2.9.tar`

### file list

```diff
@@ -1,376 +1,377 @@
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.680142 design.plone.contenttypes-6.2.8/
--rw-r--r--   0 lucabel    (501) staff       (20)    24235 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/CHANGES.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/CONTRIBUTORS.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      585 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/DEVELOP.rst
--rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/LICENSE.GPL
--rw-r--r--   0 lucabel    (501) staff       (20)      665 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/LICENSE.rst
--rw-r--r--   0 lucabel    (501) staff       (20)      174 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/MANIFEST.in
--rw-r--r--   0 lucabel    (501) staff       (20)    41492 2024-04-22 12:15:12.680324 design.plone.contenttypes-6.2.8/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    15960 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/README.md
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.594873 design.plone.contenttypes-6.2.8/docs/
--rw-r--r--   0 lucabel    (501) staff       (20)     7993 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/docs/conf.py
--rw-r--r--   0 lucabel    (501) staff       (20)       98 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/docs/index.rst
--rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/requirements.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      383 2024-04-22 12:15:12.680777 design.plone.contenttypes-6.2.8/setup.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3005 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/setup.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.584062 design.plone.contenttypes-6.2.8/src/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.595151 design.plone.contenttypes-6.2.8/src/design/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.598097 design.plone.contenttypes-6.2.8/src/design/plone/
--rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.600363 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/
--rw-r--r--   0 lucabel    (501) staff       (20)      668 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.601979 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      892 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      421 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/interfaces.py
--rw-r--r--   0 lucabel    (501) staff       (20)      930 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/query.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
--rw-r--r--   0 lucabel    (501) staff       (20)      231 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/servizi_correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.607864 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1354 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/additional_help_infos.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2403 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/address.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8986 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11818 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     6469 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/contatti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1589 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/dataset_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2679 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6212 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1060 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/exclude_from_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1657 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/geolocation.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2388 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/info_testata.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2739 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6540 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1606 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/multi_file.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4439 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/news_additional_fields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1787 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/servizi_correlati.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1357 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1648 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/strutture_correlate.py
--rw-r--r--   0 lucabel    (501) staff       (20)    10452 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/trasparenza.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1165 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/update_note.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.608657 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1333 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.608950 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/overrides/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/overrides/.gitkeep
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.585276 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/static/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.609180 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/static/js/
--rw-r--r--   0 lucabel    (501) staff       (20)      262 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/static/js/move_content.js
--rw-r--r--   0 lucabel    (501) staff       (20)      469 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/trasparenza.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.612510 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3898 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8270 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_documenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7290 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_eventi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7550 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_luoghi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8729 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_notizie.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8573 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_persone.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14364 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_servizi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7594 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_uo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3467 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1571 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/export_incarichi.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2796 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/move_news_items.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.615248 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/
--rw-r--r--   0 lucabel    (501) staff       (20)     3360 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6399 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6372 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6388 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     8600 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6167 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     9903 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     6177 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     4760 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3797 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/utils.pt
--rw-r--r--   0 lucabel    (501) staff       (20)     3122 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.619904 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      315 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)      246 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)      210 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/evento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      215 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      229 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)      271 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      272 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/content/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.620980 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      737 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1382 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3865 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/settings.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.622562 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5779 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/document.py
--rw-r--r--   0 lucabel    (501) staff       (20)      536 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)      969 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/pagina_argomento.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.625774 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      458 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1119 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/common.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1803 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      411 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/events.py
--rw-r--r--   0 lucabel    (501) staff       (20)      921 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)      621 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)      829 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)      741 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)      470 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      445 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/uo.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.630866 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/
--rw-r--r--   0 lucabel    (501) staff       (20)      419 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6263 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)      699 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)      857 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/dataset.py
--rw-r--r--   0 lucabel    (501) staff       (20)     8557 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4724 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/documento_personale.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5442 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/incarico.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1487 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/messaggio.py
--rw-r--r--   0 lucabel    (501) staff       (20)      205 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2560 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5028 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1781 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2850 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1864 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
--rw-r--r--   0 lucabel    (501) staff       (20)    18229 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7946 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.632444 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/
--rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/README.rst
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/__init__.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.586850 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/__pycache__/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.632681 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    82355 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)    82310 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.587124 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/en/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.633141 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)    82335 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.587397 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.634267 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
--rw-r--r--   0 lucabel    (501) staff       (20)     1243 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
--rw-r--r--   0 lucabel    (501) staff       (20)    83275 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
--rw-r--r--   0 lucabel    (501) staff       (20)     7287 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/plone.pot
--rw-r--r--   0 lucabel    (501) staff       (20)     1597 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/update.py
--rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/update.sh
--rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/overrides.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.635637 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/
--rw-r--r--   0 lucabel    (501) staff       (20)      516 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3716 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/baseserializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)      483 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      343 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/patches.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2751 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/permissions.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.588879 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.587953 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.642978 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
--rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3401 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      331 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     4370 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      286 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2870 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      372 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     8078 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      300 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2156 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      313 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    13732 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      398 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     5133 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      292 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1042 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      303 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2196 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      265 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)    15346 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      322 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     1015 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      355 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     3138 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      342 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
--rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.645200 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/
--rw-r--r--   0 lucabel    (501) staff       (20)      799 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/actions.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      193 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/browserlayer.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2919 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/catalog.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1040 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1219 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/diff_tool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      595 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/metadata.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.645770 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/registry/
--rw-r--r--   0 lucabel    (501) staff       (20)    19836 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/registry/settings.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1139 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/repositorytool.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     4491 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/rolemap.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.650842 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/
--rw-r--r--   0 lucabel    (501) staff       (20)     1155 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Bando.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3563 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3327 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Document.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3747 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Documento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3321 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2501 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Event.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      345 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Folder.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3427 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      506 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Link.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3199 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2908 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3456 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3430 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Persona.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3178 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3342 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3149 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3829 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     3775 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     2212 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Venue.xml
--rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.651073 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/fix_syndication/
--rw-r--r--   0 lucabel    (501) staff       (20)      520 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.651632 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/to_3000/
--rw-r--r--   0 lucabel    (501) staff       (20)      377 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
--rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/to_3000/registry.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.651871 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/uninstall/
--rw-r--r--   0 lucabel    (501) staff       (20)      128 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.652973 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      663 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      504 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/converters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      702 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/correlati.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.655537 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      760 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5795 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6060 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5743 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1658 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5844 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5999 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6016 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.659868 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1548 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2086 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1976 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2102 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2860 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7597 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/dxfields.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1407 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2360 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3800 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1763 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2502 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/relationfield.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1660 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    17062 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/summary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5316 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3769 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/venue.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.660601 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      601 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/configure.zcml
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.661419 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/content/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/content/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      664 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/content/add.py
--rw-r--r--   0 lucabel    (501) staff       (20)      368 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/content/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)      653 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/controlpanel.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.662110 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/modulistica_items/
--rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      605 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     2915 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.662759 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/navigation/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/navigation/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      558 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1254 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/navigation/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.663406 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/scadenziario/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1200 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    11504 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.664055 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/trasparenza/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      884 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     3351 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.664698 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)    11248 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/types/get.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.665368 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/types/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/types/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3805 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/types/adapters.py
--rw-r--r--   0 lucabel    (501) staff       (20)      394 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/types/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1628 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/schema_overrides.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2315 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/setuphandlers.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4083 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/testing.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.674758 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11218 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/example.pdf
--rw-r--r--   0 lucabel    (501) staff       (20)    10503 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/example.png
--rw-r--r--   0 lucabel    (501) staff       (20)     1997 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_argomenti.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2330 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_base_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1564 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4707 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2563 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_update_note.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1889 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_change_news_type.py
--rw-r--r--   0 lucabel    (501) staff       (20)     7543 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_bando.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5613 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6203 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_document.py
--rw-r--r--   0 lucabel    (501) staff       (20)    11615 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_documento.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13149 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_event.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1640 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_folder.py
--rw-r--r--   0 lucabel    (501) staff       (20)    14823 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_luogo.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_modulo.py
--rw-r--r--   0 lucabel    (501) staff       (20)    12271 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_news.py
--rw-r--r--   0 lucabel    (501) staff       (20)     5903 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
--rw-r--r--   0 lucabel    (501) staff       (20)     9850 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_persona.py
--rw-r--r--   0 lucabel    (501) staff       (20)    19255 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_servizio.py
--rw-r--r--   0 lucabel    (501) staff       (20)    17028 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2926 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_custom_service_navigation.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2708 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2526 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_move_news_items_view.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6638 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2798 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_service_scadenziario.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1381 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
--rw-r--r--   0 lucabel    (501) staff       (20)     3533 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_setup.py
--rw-r--r--   0 lucabel    (501) staff       (20)    13785 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_substructure_creation.py
--rw-r--r--   0 lucabel    (501) staff       (20)    12464 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4714 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6351 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_vocabularies.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.676888 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)    25023 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     5033 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/draftjs_converter.py
--rw-r--r--   0 lucabel    (501) staff       (20)    12517 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/to_7001.py
--rw-r--r--   0 lucabel    (501) staff       (20)     6007 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/to_7002.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1808 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/to_7300.py
--rw-r--r--   0 lucabel    (501) staff       (20)    57526 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/upgrades.py
--rw-r--r--   0 lucabel    (501) staff       (20)      862 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/utils.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.679911 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/
--rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/__init__.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1308 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1573 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1694 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/configure.zcml
--rw-r--r--   0 lucabel    (501) staff       (20)     1466 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1895 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1704 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/mockup.py
--rw-r--r--   0 lucabel    (501) staff       (20)     2223 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
--rw-r--r--   0 lucabel    (501) staff       (20)     1623 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
--rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
-drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-04-22 12:15:12.597803 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/
--rw-r--r--   0 lucabel    (501) staff       (20)    41492 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/PKG-INFO
--rw-r--r--   0 lucabel    (501) staff       (20)    19438 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/SOURCES.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/dependency_links.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      130 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/entry_points.txt
--rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/namespace_packages.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/not-zip-safe
--rw-r--r--   0 lucabel    (501) staff       (20)      451 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/requires.txt
--rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/top_level.txt
--rw-r--r--   0 lucabel    (501) staff       (20)      659 2024-04-22 12:15:12.000000 design.plone.contenttypes-6.2.8/tox.ini
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.068441 design_plone_contenttypes-6.2.9/
+-rw-r--r--   0 lucabel    (501) staff       (20)    24514 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/CHANGES.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       67 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/CONTRIBUTORS.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      585 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/DEVELOP.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)    18092 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/LICENSE.GPL
+-rw-r--r--   0 lucabel    (501) staff       (20)      665 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/LICENSE.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)      174 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/MANIFEST.in
+-rw-r--r--   0 lucabel    (501) staff       (20)    42645 2024-05-21 15:00:05.068291 design_plone_contenttypes-6.2.9/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    15960 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/README.md
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.974654 design_plone_contenttypes-6.2.9/docs/
+-rw-r--r--   0 lucabel    (501) staff       (20)     7993 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/docs/conf.py
+-rw-r--r--   0 lucabel    (501) staff       (20)       98 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/docs/index.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)       62 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/requirements.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      383 2024-05-21 15:00:05.068867 design_plone_contenttypes-6.2.9/setup.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3030 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/setup.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.963645 design_plone_contenttypes-6.2.9/src/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.974938 design_plone_contenttypes-6.2.9/src/design/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.977852 design_plone_contenttypes-6.2.9/src/design/plone/
+-rw-r--r--   0 lucabel    (501) staff       (20)       80 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.980129 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/
+-rw-r--r--   0 lucabel    (501) staff       (20)      668 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.981814 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      892 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      421 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/interfaces.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      930 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/query.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/searchabletext_indexers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      231 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/servizi_correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.987233 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1354 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/additional_help_infos.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2403 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/address.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8986 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11818 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     6469 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/contatti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1589 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/dataset_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2679 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6212 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1060 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/exclude_from_search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1657 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/geolocation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2388 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/info_testata.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2739 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/luoghi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6540 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1606 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/multi_file.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4439 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/news_additional_fields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1787 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/servizi_correlati.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1357 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1648 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/strutture_correlate.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    10452 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/trasparenza.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1165 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/update_note.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.987949 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1333 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.988196 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/overrides/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/overrides/.gitkeep
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.964876 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/static/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.988397 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/static/js/
+-rw-r--r--   0 lucabel    (501) staff       (20)      262 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/static/js/move_content.js
+-rw-r--r--   0 lucabel    (501) staff       (20)      469 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/trasparenza.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.991957 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3898 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8270 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_documenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7290 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_eventi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7550 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_luoghi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8729 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_notizie.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8573 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_persone.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13677 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_servizi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7594 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_uo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3467 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1571 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/export_incarichi.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2796 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/move_news_items.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.996108 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/
+-rw-r--r--   0 lucabel    (501) staff       (20)     3360 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6399 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6372 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6388 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     8600 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6167 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     9903 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     6177 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     4760 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     3797 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/utils.pt
+-rw-r--r--   0 lucabel    (501) staff       (20)     3122 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.002785 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      315 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      246 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      210 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/evento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      215 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      229 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      271 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      238 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      272 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      279 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      242 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      283 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/content/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.003893 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      737 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1382 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3865 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/settings.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.005548 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5933 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1189 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      536 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      969 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/pagina_argomento.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.008390 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      458 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1119 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/common.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1803 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      411 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/events.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      921 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1224 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      829 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      741 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      470 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      445 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/uo.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.012737 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/
+-rw-r--r--   0 lucabel    (501) staff       (20)      419 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6263 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      699 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      857 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/dataset.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     8557 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4724 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/documento_personale.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5442 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/incarico.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1487 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/messaggio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      205 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2560 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5028 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1781 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2850 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1864 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    18229 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7946 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/unita_organizzativa.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.014410 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/
+-rw-r--r--   0 lucabel    (501) staff       (20)      611 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/README.rst
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/__init__.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.966370 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/__pycache__/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.014696 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    82355 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    82310 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.966633 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/en/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.015056 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/en/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)    82335 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.966894 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.016011 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1243 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po
+-rw-r--r--   0 lucabel    (501) staff       (20)    83275 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po
+-rw-r--r--   0 lucabel    (501) staff       (20)     7287 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/plone.pot
+-rw-r--r--   0 lucabel    (501) staff       (20)     1597 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/update.py
+-rwxr-xr-x   0 lucabel    (501) staff       (20)      512 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/update.sh
+-rw-r--r--   0 lucabel    (501) staff       (20)      712 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/overrides.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.016975 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/
+-rw-r--r--   0 lucabel    (501) staff       (20)      516 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3716 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/baseserializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      483 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      343 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/patches.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2751 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/permissions.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.968322 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.967428 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.024028 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/
+-rw-r--r--   0 lucabel    (501) staff       (20)      314 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3401 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      331 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     4370 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      286 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2870 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      372 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     8078 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      300 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2156 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      313 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    13732 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      398 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     5133 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      292 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1042 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      303 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2196 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      265 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)    15346 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      322 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     1015 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      355 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     3138 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      342 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      344 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.cfg
+-rw-r--r--   0 lucabel    (501) staff       (20)     2275 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.026852 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/
+-rw-r--r--   0 lucabel    (501) staff       (20)      799 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/actions.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      193 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/browserlayer.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2919 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/catalog.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1040 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1219 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/diff_tool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      595 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/metadata.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.027545 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/registry/
+-rw-r--r--   0 lucabel    (501) staff       (20)    19836 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/registry/criteria.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      618 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/registry/settings.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1139 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/repositorytool.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     4491 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/rolemap.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.033897 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)     1155 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Bando.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      503 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Bando_Folder_Deepening.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3563 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3327 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Dataset.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1001 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Document.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3747 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Documento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3321 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2501 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Event.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      345 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Folder.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3427 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Incarico.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      506 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Link.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3199 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2908 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Modulo.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/News_Item.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3456 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3430 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Persona.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3178 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Pratica.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3342 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3149 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3829 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Servizio.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3775 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2212 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Venue.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1194 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.034172 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/fix_syndication/
+-rw-r--r--   0 lucabel    (501) staff       (20)      520 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.034669 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/to_3000/
+-rw-r--r--   0 lucabel    (501) staff       (20)      377 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/to_3000/controlpanel.xml
+-rw-r--r--   0 lucabel    (501) staff       (20)      275 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/to_3000/registry.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.034953 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/uninstall/
+-rw-r--r--   0 lucabel    (501) staff       (20)      128 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.035853 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      663 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      504 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/converters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      702 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/correlati.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.038236 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      760 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5146 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6060 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5094 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1658 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5195 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5349 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5367 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.043000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1548 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2086 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1976 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2102 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2860 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/dxcontent.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7597 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/dxfields.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1407 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2360 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3800 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1763 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2502 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/relationfield.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1660 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    17556 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/summary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5316 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3769 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/venue.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.044196 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      601 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/configure.zcml
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.045309 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/content/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/content/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      664 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/content/add.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      368 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/content/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)      653 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/controlpanel.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.046194 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/modulistica_items/
+-rw-r--r--   0 lucabel    (501) staff       (20)       24 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/modulistica_items/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      605 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     2915 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.047092 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/navigation/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/navigation/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      558 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1254 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/navigation/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.047930 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/scadenziario/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/scadenziario/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1200 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    11504 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/scadenziario/post.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.048850 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/trasparenza/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/trasparenza/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      884 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     3351 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/trasparenza/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.049679 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      404 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)    11248 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/types/get.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.050527 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/types/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/types/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3805 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/types/adapters.py
+-rw-r--r--   0 lucabel    (501) staff       (20)      394 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/types/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1628 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/schema_overrides.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2315 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/setuphandlers.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4083 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/testing.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.061576 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11218 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/example.pdf
+-rw-r--r--   0 lucabel    (501) staff       (20)    10503 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/example.png
+-rw-r--r--   0 lucabel    (501) staff       (20)     1997 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_argomenti.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2330 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_base_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1564 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4707 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3169 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2563 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_show_modified.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1755 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_update_note.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1889 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_change_news_type.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     7543 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_bando.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5613 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6203 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_document.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    11615 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_documento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    13149 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_event.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1640 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_folder.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    14823 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_luogo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_modulo.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    12271 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_news.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     5903 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     9850 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_persona.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    19255 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_servizio.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    17028 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2926 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_custom_service_navigation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2708 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2526 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_move_news_items_view.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6638 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2798 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_service_scadenziario.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1381 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     3533 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_setup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    14380 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_substructure_creation.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    12464 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4968 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6351 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_vocabularies.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.063823 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    25231 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     5033 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/draftjs_converter.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    12517 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_7001.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     6007 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_7002.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1807 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_7300.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1465 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_730x.py
+-rw-r--r--   0 lucabel    (501) staff       (20)    57526 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/upgrades.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2035 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/utils.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.066676 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/
+-rw-r--r--   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/__init__.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1308 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1573 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1694 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/configure.zcml
+-rw-r--r--   0 lucabel    (501) staff       (20)     1466 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1895 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1704 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/mockup.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     2223 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/people_vocabulary.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     1623 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py
+-rw-r--r--   0 lucabel    (501) staff       (20)     4225 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py
+drwxr-xr-x   0 lucabel    (501) staff       (20)        0 2024-05-21 15:00:05.067229 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/
+-rw-r--r--   0 lucabel    (501) staff       (20)    42645 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/PKG-INFO
+-rw-r--r--   0 lucabel    (501) staff       (20)    19488 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/SOURCES.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/dependency_links.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      130 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/entry_points.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)       20 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        1 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/not-zip-safe
+-rw-r--r--   0 lucabel    (501) staff       (20)      465 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/requires.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)        7 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/top_level.txt
+-rw-r--r--   0 lucabel    (501) staff       (20)      659 2024-05-21 15:00:04.000000 design_plone_contenttypes-6.2.9/tox.ini
```

### Comparing `design.plone.contenttypes-6.2.8/CHANGES.rst` & `design_plone_contenttypes-6.2.9/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+6.2.9 (2024-05-21)
+------------------
+
+- Add this folder "Altri Documenti" under "Persona pubblica"
+  [lucabel]
+- Code porting to work with both plone 6.0.10.x and 6.0.11
+  due to some core egg update
+  Code porting to work with the new plone.restapi 9.6.1 version
+  [lucabel]
+
+
 6.2.8 (2024-04-22)
 ------------------
 
 - Add start metadata to event summary serialization;
   useful when create event with children event: in items list we
   have subevents with missing start date
   [lucabel]
```

### Comparing `design.plone.contenttypes-6.2.8/DEVELOP.rst` & `design_plone_contenttypes-6.2.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/LICENSE.GPL` & `design_plone_contenttypes-6.2.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/LICENSE.rst` & `design_plone_contenttypes-6.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/PKG-INFO` & `design_plone_contenttypes-6.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.2.8
+Version: 6.2.9
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,17 +20,38 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.app.dexterity>2.6.9
+Requires-Dist: collective.venue[geolocation]
+Requires-Dist: collective.volto.blocksfield
+Requires-Dist: collective.z3cform.datagridfield
+Requires-Dist: plone.formwidget.geolocation
+Requires-Dist: redturtle.volto>=5.0.0
+Requires-Dist: redturtle.bandi
+Requires-Dist: z3c.unconfigure
+Requires-Dist: plone.restapi
+Requires-Dist: eea.api.taxonomy
+Requires-Dist: openpyxl
+Requires-Dist: collective.volto.enhancedlinks
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: collective.volto.blocksfield; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: collective.MockMailHost; extra == "test"
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Tests](https://github.com/RedTurtle/design.plone.contenttypes/actions/workflows/tests.yml/badge.svg)](https://github.com/RedTurtle/design.plone.contenttypes/actions)
 [![Coverage](https://coveralls.io/repos/github/RedTurtle/design.plone.contenttypes/badge.svg?branch=main)](https://coveralls.io/github/RedTurtle/design.plone.contenttypes?branch=main)
@@ -498,14 +519,25 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.2.9 (2024-05-21)
+------------------
+
+- Add this folder "Altri Documenti" under "Persona pubblica"
+  [lucabel]
+- Code porting to work with both plone 6.0.10.x and 6.0.11
+  due to some core egg update
+  Code porting to work with the new plone.restapi 9.6.1 version
+  [lucabel]
+
+
 6.2.8 (2024-04-22)
 ------------------
 
 - Add start metadata to event summary serialization;
   useful when create event with children event: in items list we
   have subevents with missing start date
   [lucabel]
```

### Comparing `design.plone.contenttypes-6.2.8/README.md` & `design_plone_contenttypes-6.2.9/README.md`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/docs/conf.py` & `design_plone_contenttypes-6.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/setup.py` & `design_plone_contenttypes-6.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.contenttypes",
-    version="6.2.8",
+    version="6.2.9",
     description="DesignItalia contenty types",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
@@ -60,14 +60,15 @@
         "collective.venue[geolocation]",
         "collective.volto.blocksfield",
         "collective.z3cform.datagridfield",
         "plone.formwidget.geolocation",
         "redturtle.volto>=5.0.0",
         "redturtle.bandi",
         "z3c.unconfigure",
+        "plone.restapi",
         "eea.api.taxonomy",
         "openpyxl",
         "collective.volto.enhancedlinks",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/__init__.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/query.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/query.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/adapters/searchabletext_indexers.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/adapters/searchabletext_indexers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/additional_help_infos.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/additional_help_infos.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/address.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/address.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/argomenti.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/contatti.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/contatti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/dataset_correlati.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/dataset_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/descrizione_estesa.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/evento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/evento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/exclude_from_search.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/exclude_from_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/geolocation.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/geolocation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/info_testata.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/info_testata.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/luoghi_correlati.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/luoghi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/luogo.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/multi_file.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/multi_file.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/news_additional_fields.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/news_additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/servizi_correlati.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/servizi_correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/show_modified.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/strutture_correlate.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/strutture_correlate.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/trasparenza.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/behaviors/update_note.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/behaviors/update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/change_news_type.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_documenti.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_documenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_eventi.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_eventi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_luoghi.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_luoghi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_notizie.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_notizie.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_persone.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_persone.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_servizi.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_servizi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,24 @@
 # -*- coding: utf-8 -*-
 from DateTime import DateTime
+from design.plone.contenttypes.utils import text_in_block
 from openpyxl import Workbook
 from openpyxl.styles import Alignment
 from openpyxl.styles import Font
 from openpyxl.styles import PatternFill
 from openpyxl.utils import get_column_letter
 from plone import api
-from plone.restapi.behaviors import IBlocks
-from plone.restapi.indexers import SearchableText_blocks
 from Products.Five import BrowserView
-from zope.interface import implementer
 
 import io
 
 
 FLAG = '<i class="fa-solid fa-check"></i>'
 
 
-def text_in_block(blocks):
-    @implementer(IBlocks)
-    class FakeObject(object):
-        """
-        We use a fake object to use SearchableText Indexer
-        """
-
-        def Subject(self):
-            return ""
-
-        def __init__(self, blocks, blocks_layout):
-            self.blocks = blocks
-            self.blocks_layout = blocks_layout
-            self.id = ""
-            self.title = ""
-            self.description = ""
-
-    if not blocks:
-        return None
-    fakeObj = FakeObject(blocks.get("blocks", ""), blocks.get("blocks_layout", ""))
-    return SearchableText_blocks(fakeObj)()
-
-
 class CheckServizi(BrowserView):
     cds = None
 
     def is_anonymous(self):
         return api.user.is_anonymous()
 
     def get_canale_accesso_info(self, servizio):
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/check_uo.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/check_uo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/export_incarichi.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/export_incarichi.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/move_news_items.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/move_news_items.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/change_news_type.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_documenti.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_eventi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_luoghi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_notizie.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_persone.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_servizi.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/check_uo.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/move_news_items.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/browser/utils/templates/utils.pt` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/browser/utils/templates/utils.pt`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/geolocation_defaults.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/controlpanels/settings.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/controlpanels/settings.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/common.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,19 @@
         {
             "id": "variazione-situazione-patrimoniale",
             "title": "Variazione situazione patrimoniale",
             "allowed_types": ("File",),
         },
         {"id": "altre-cariche", "title": "Altre cariche", "allowed_types": ("File",)},
         {"id": "incarichi", "title": "Incarichi", "allowed_types": ("Incarico",)},
+        {
+            "id": "altri-documenti",
+            "title": "Altri documenti",
+            "allowed_types": ("File", "Image", "Link"),
+        },
     ],
     "Pratica": [
         {
             "id": "allegati",
             "title": "Allegati",
             "type": "Folder",
             "allowed_types": ("File",),
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/document.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/incarico.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/events/pagina_argomento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/events/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/common.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/common.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/news.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/persona.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/indexers/punto_di_contatto.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/indexers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/bando.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/cartella_modulistica.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/dataset.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/dataset.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/documento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/documento_personale.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/documento_personale.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/incarico.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/incarico.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/messaggio.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/messaggio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/pagina_argomento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/persona.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/pratica.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/punto_di_contatto.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/ricevuta_pagamento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/servizio.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/interfaces/unita_organizzativa.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/interfaces/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/README.rst` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/__pycache__/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/design.plone.contenttypes.pot`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/en/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/collective.geolocationbehavior.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/design.plone.contenttypes.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/update.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/locales/update.sh` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/locales/update.sh`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/overrides.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/overrides.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/__init__.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/patches/baseserializer.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/patches/baseserializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/permissions.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/permissions.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/business_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/person_life_events.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/temi_dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documenti_albopretorio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_evento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_frequenza_aggiornamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_licenze.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_luogo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_notizia.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_organizzazione.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_pdc.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/behaviors/taxonomies/tipologia_stati_pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/actions.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/catalog.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/controlpanel.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/diff_tool.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/diff_tool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/metadata.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>7300</version>
+  <version>7301</version>
   <dependencies>
     <dependency>profile-redturtle.bandi:default</dependency>
     <dependency>profile-collective.venue:default</dependency>
     <dependency>profile-redturtle.volto:default</dependency>
     <dependency>profile-eea.api.taxonomy:default</dependency>
     <dependency>profile-collective.z3cform.datagridfield:default</dependency>
     <dependency>profile-design.plone.contenttypes:taxonomy</dependency>
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/registry/criteria.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/registry/settings.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/repositorytool.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/repositorytool.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/rolemap.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Bando.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Bando.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/CartellaModulistica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Dataset.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Dataset.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Document.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Document.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Documento.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Documento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Documento_Personale.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Event.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Event.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Incarico.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Incarico.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Messaggio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Modulo.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Modulo.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/News_Item.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/News_Item.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Pagina_Argomento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Persona.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Persona.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Pratica.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Pratica.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/PuntoDiContatto.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/RicevutaPagamento.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Servizio.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Servizio.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/UnitaOrganizzativa.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types/Venue.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types/Venue.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/default/types.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/profiles/fix_syndication/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/correlati.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/correlati.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/documento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/news.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,49 @@
 # -*- coding: utf-8 -*-
-from design.plone.contenttypes.interfaces.documento import IDocumento
-from plone.restapi.behaviors import IBlocks
+from design.plone.contenttypes.utils import text_in_block
+from plone.app.contenttypes.interfaces import INewsItem
 from plone.restapi.deserializer import json_body
 from plone.restapi.deserializer.dxcontent import DeserializeFromJson
-from plone.restapi.indexers import SearchableText_blocks
 from plone.restapi.interfaces import IDeserializeFromJson
 from zExceptions import BadRequest
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 TITLE_MAX_LEN = 255
 DESCRIPTION_MAX_LEN = 255
 EMPTY_BLOCK_MARKER = {"@type": "text"}
 MANDATORY_RICH_TEXT_FIELDS = [
-    # "descrizione_estesa",
-    "formati_disponibili",
+    "descrizione_estesa",
 ]
 
 
 def new_error(message):
     return {"error": "ValidationError", "message": message}
 
 
-def text_in_block(blocks):
-    @implementer(IBlocks)
-    class FakeObject(object):
-        """
-        We use a fake object to use SearchableText Indexer
-        """
-
-        def Subject(self):
-            return ""
-
-        def __init__(self, blocks, blocks_layout):
-            self.blocks = blocks
-            self.blocks_layout = blocks_layout
-            self.id = ""
-            self.title = ""
-            self.description = ""
-
-    if not blocks:
-        return None
-
-    fakeObj = FakeObject(blocks.get("blocks", ""), blocks.get("blocks_layout", ""))
-    return SearchableText_blocks(fakeObj)()
-
-
 @implementer(IDeserializeFromJson)
-@adapter(IDocumento, Interface)
-class DeserializeDocumentoFromJson(DeserializeFromJson):
+@adapter(INewsItem, Interface)
+class DeserializeNewsFromJson(DeserializeFromJson):
     def __call__(
         self, validate_all=False, data=None, create=False
     ):  # noqa: ignore=C901
         if data is None:
             data = json_body(self.request)
 
         method = self.request.get("method")
         is_post = method == "POST"
         is_patch = method == "PATCH"
         errors = []
 
         if list(data.keys()) != ["ordering"]:
             title = data.get("title")
             description = data.get("description")
+
             if is_post:
                 # Title validation
                 if not title:
                     errors.append(new_error("Il titolo è obbligatorio"))
                 elif len(title) > TITLE_MAX_LEN:
                     errors.append(
                         new_error(
@@ -140,10 +115,11 @@
                     ):
                         errors.append(
                             new_error("Il campo {} è obbligatorio".format(field))
                         )
 
         if errors:
             raise BadRequest(errors)
-        return super(DeserializeDocumentoFromJson, self).__call__(
+
+        return super(DeserializeNewsFromJson, self).__call__(
             validate_all=False, data=data, create=False
         )
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/dxfields.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/news.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,68 @@
 # -*- coding: utf-8 -*-
-from plone.app.contenttypes.interfaces import INewsItem
-from plone.restapi.behaviors import IBlocks
+from design.plone.contenttypes.interfaces.unita_organizzativa import IUnitaOrganizzativa
+from design.plone.contenttypes.utils import text_in_block
 from plone.restapi.deserializer import json_body
 from plone.restapi.deserializer.dxcontent import DeserializeFromJson
-from plone.restapi.indexers import SearchableText_blocks
 from plone.restapi.interfaces import IDeserializeFromJson
 from zExceptions import BadRequest
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 TITLE_MAX_LEN = 255
 DESCRIPTION_MAX_LEN = 255
 EMPTY_BLOCK_MARKER = {"@type": "text"}
-MANDATORY_RICH_TEXT_FIELDS = [
-    "descrizione_estesa",
-]
+MANDATORY_RICH_TEXT_FIELDS = ["competenze"]
 
 
 def new_error(message):
     return {"error": "ValidationError", "message": message}
 
 
-def text_in_block(blocks):
-    @implementer(IBlocks)
-    class FakeObject(object):
-        """
-        We use a fake object to use SearchableText Indexer
-        """
-
-        def Subject(self):
-            return ""
-
-        def __init__(self, blocks, blocks_layout):
-            self.blocks = blocks
-            self.blocks_layout = blocks_layout
-            self.id = ""
-            self.title = ""
-            self.description = ""
-
-    if not blocks:
-        return None
-
-    fakeObj = FakeObject(blocks.get("blocks", ""), blocks.get("blocks_layout", ""))
-    return SearchableText_blocks(fakeObj)()
-
-
 @implementer(IDeserializeFromJson)
-@adapter(INewsItem, Interface)
-class DeserializeNewsFromJson(DeserializeFromJson):
+@adapter(IUnitaOrganizzativa, Interface)
+class DeserializeUnitaOrganizzativaFromJson(DeserializeFromJson):
     def __call__(
         self, validate_all=False, data=None, create=False
     ):  # noqa: ignore=C901
         if data is None:
             data = json_body(self.request)
 
         method = self.request.get("method")
         is_post = method == "POST"
         is_patch = method == "PATCH"
         errors = []
-
         if list(data.keys()) != ["ordering"]:
             title = data.get("title")
             description = data.get("description")
 
             if is_post:
                 # Title validation
                 if not title:
-                    errors.append(new_error("Il titolo è obbligatorio"))
+                    errors.append(
+                        new_error("Il titolo dell'unità organizzativa è obbligatorio")
+                    )
                 elif len(title) > TITLE_MAX_LEN:
                     errors.append(
                         new_error(
                             "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
                                 TITLE_MAX_LEN
                             )
                         )
                     )
 
                 # description validation
                 if not description:
-                    errors.append(new_error("La descrizione è obbligatoria"))
+                    errors.append(
+                        new_error(
+                            "La descrizione dell'unità organizzativa è obbligatorio"
+                        )
+                    )
                 elif len(description) > DESCRIPTION_MAX_LEN:
                     errors.append(
                         new_error(
                             "La descrizione deve avere una lunghezza di massimo {} caratteri".format(  # noqa
                                 DESCRIPTION_MAX_LEN
                             )
                         )
@@ -100,14 +78,15 @@
                             new_error("Il campo {} è obbligatorio".format(field))
                         )
 
             if is_patch:
                 # Title validation
                 if "title" in data and not title:
                     errors.append(new_error("Il titolo è obbligatorio"))
+
                 if title and len(title) > TITLE_MAX_LEN:
                     errors.append(
                         new_error(
                             "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
                                 TITLE_MAX_LEN
                             )
                         )
@@ -119,32 +98,33 @@
                     errors.append(
                         new_error(
                             "La descrizione deve avere una lunghezza di massimo {} caratteri".format(  # noqa
                                 DESCRIPTION_MAX_LEN
                             )
                         )
                     )
+
                 if "description" not in data and not self.context.description:
                     errors.append(new_error("La descrizione è obbligatoria"))
 
                 for field in MANDATORY_RICH_TEXT_FIELDS:
                     if field in data and not text_in_block(data.get(field)):
                         errors.append(
                             new_error("Il campo {} è obbligatorio".format(field))
                         )
+
                     # Se siamo nella patch siamo in modifica. Se siamo in modifica e
                     # siamo su un sito che ha avuto upgrade alla versione pnrr può
                     # essere che dei campi obbligatori un tempo non lo fossero e quindi
                     # arriviamo fino a qui
                     if field not in data and not text_in_block(
                         getattr(self.context, field)
                     ):
                         errors.append(
                             new_error("Il campo {} è obbligatorio".format(field))
                         )
 
         if errors:
             raise BadRequest(errors)
-
-        return super(DeserializeNewsFromJson, self).__call__(
+        return super(DeserializeUnitaOrganizzativaFromJson, self).__call__(
             validate_all=False, data=data, create=False
         )
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/persona.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/servizio.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/servizio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 from design.plone.contenttypes.interfaces.servizio import IServizio
-from plone.restapi.behaviors import IBlocks
+from design.plone.contenttypes.utils import text_in_block
 from plone.restapi.deserializer import json_body
 from plone.restapi.deserializer.dxcontent import DeserializeFromJson
-from plone.restapi.indexers import SearchableText_blocks
 from plone.restapi.interfaces import IDeserializeFromJson
 from zExceptions import BadRequest
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
@@ -23,38 +22,14 @@
 ]
 
 
 def new_error(message):
     return {"error": "ValidationError", "message": message}
 
 
-def text_in_block(blocks):
-    @implementer(IBlocks)
-    class FakeObject(object):
-        """
-        We use a fake object to use SearchableText Indexer
-        """
-
-        def Subject(self):
-            return ""
-
-        def __init__(self, blocks, blocks_layout):
-            self.blocks = blocks
-            self.blocks_layout = blocks_layout
-            self.id = ""
-            self.title = ""
-            self.description = ""
-
-    if not blocks:
-        return None
-
-    fakeObj = FakeObject(blocks.get("blocks", ""), blocks.get("blocks_layout", ""))
-    return SearchableText_blocks(fakeObj)()
-
-
 @implementer(IDeserializeFromJson)
 @adapter(IServizio, Interface)
 class DeserializeServizioFromJson(DeserializeFromJson):
     def __call__(
         self, validate_all=False, data=None, create=False
     ):  # noqa: ignore=C901
         if data is None:
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/unitaorganizzativa.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/venue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,136 @@
 # -*- coding: utf-8 -*-
-from design.plone.contenttypes.interfaces.unita_organizzativa import IUnitaOrganizzativa
-from plone.restapi.behaviors import IBlocks
+from collective.venue.interfaces import IVenue
+from design.plone.contenttypes.utils import text_in_block
 from plone.restapi.deserializer import json_body
 from plone.restapi.deserializer.dxcontent import DeserializeFromJson
-from plone.restapi.indexers import SearchableText_blocks
 from plone.restapi.interfaces import IDeserializeFromJson
 from zExceptions import BadRequest
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 TITLE_MAX_LEN = 255
 DESCRIPTION_MAX_LEN = 255
 EMPTY_BLOCK_MARKER = {"@type": "text"}
-MANDATORY_RICH_TEXT_FIELDS = ["competenze"]
+MANDATORY_RICH_TEXT_FIELDS = ["modalita_accesso"]
 
 
 def new_error(message):
     return {"error": "ValidationError", "message": message}
 
 
-def text_in_block(blocks):
-    @implementer(IBlocks)
-    class FakeObject(object):
-        """
-        We use a fake object to use SearchableText Indexer
-        """
-
-        def Subject(self):
-            return ""
-
-        def __init__(self, blocks, blocks_layout):
-            self.blocks = blocks
-            self.blocks_layout = blocks_layout
-            self.id = ""
-            self.title = ""
-            self.description = ""
-
-    if not blocks:
-        return None
-
-    fakeObj = FakeObject(blocks.get("blocks", ""), blocks.get("blocks_layout", ""))
-    return SearchableText_blocks(fakeObj)()
-
-
 @implementer(IDeserializeFromJson)
-@adapter(IUnitaOrganizzativa, Interface)
-class DeserializeUnitaOrganizzativaFromJson(DeserializeFromJson):
+@adapter(IVenue, Interface)
+class DeserializeLuogoFromJson(DeserializeFromJson):
     def __call__(
         self, validate_all=False, data=None, create=False
     ):  # noqa: ignore=C901
         if data is None:
             data = json_body(self.request)
 
         method = self.request.get("method")
         is_post = method == "POST"
         is_patch = method == "PATCH"
         errors = []
 
-        if list(data.keys()) != ["ordering"]:
-            title = data.get("title")
-            description = data.get("description")
-
-            if is_post:
-                # Title validation
-                if not title:
-                    errors.append(
-                        new_error("Il titolo dell'unità organizzativa è obbligatorio")
-                    )
-                elif len(title) > TITLE_MAX_LEN:
-                    errors.append(
-                        new_error(
-                            "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
-                                TITLE_MAX_LEN
-                            )
-                        )
-                    )
-
-                # description validation
-                if not description:
-                    errors.append(
-                        new_error(
-                            "La descrizione dell'unità organizzativa è obbligatorio"
-                        )
-                    )
-                elif len(description) > DESCRIPTION_MAX_LEN:
-                    errors.append(
-                        new_error(
-                            "La descrizione deve avere una lunghezza di massimo {} caratteri".format(  # noqa
-                                DESCRIPTION_MAX_LEN
-                            )
-                        )
-                    )
-
-                for field in MANDATORY_RICH_TEXT_FIELDS:
-                    if field not in data:
-                        errors.append(
-                            new_error("Il campo {} è obbligatorio".format(field))
-                        )
-                    elif field in data and not text_in_block(data.get(field)):
-                        errors.append(
-                            new_error("Il campo {} è obbligatorio".format(field))
-                        )
-
-            if is_patch:
-                # Title validation
-                if "title" in data and not title:
-                    errors.append(new_error("Il titolo è obbligatorio"))
-
-                if title and len(title) > TITLE_MAX_LEN:
-                    errors.append(
-                        new_error(
-                            "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
-                                TITLE_MAX_LEN
-                            )
-                        )
-                    )
-                # description validation
-                if "description" in data and not description:
-                    errors.append(new_error("La descrizione è obbligatoria"))
-                if description and len(description) > DESCRIPTION_MAX_LEN:
-                    errors.append(
-                        new_error(
-                            "La descrizione deve avere una lunghezza di massimo {} caratteri".format(  # noqa
-                                DESCRIPTION_MAX_LEN
-                            )
-                        )
-                    )
-
-                if "description" not in data and not self.context.description:
-                    errors.append(new_error("La descrizione è obbligatoria"))
-
-                for field in MANDATORY_RICH_TEXT_FIELDS:
-                    if field in data and not text_in_block(data.get(field)):
-                        errors.append(
-                            new_error("Il campo {} è obbligatorio".format(field))
-                        )
-
-                    # Se siamo nella patch siamo in modifica. Se siamo in modifica e
-                    # siamo su un sito che ha avuto upgrade alla versione pnrr può
-                    # essere che dei campi obbligatori un tempo non lo fossero e quindi
-                    # arriviamo fino a qui
-                    if field not in data and not text_in_block(
-                        getattr(self.context, field)
-                    ):
-                        errors.append(
-                            new_error("Il campo {} è obbligatorio".format(field))
-                        )
+        title = data.get("title")
+        description = data.get("description")
+        geolocation = data.get("geolocation")
+
+        if is_post:
+            # Title validation
+            if not title:
+                errors.append(new_error("Il titolo del luogo è obbligatorio"))
+            elif len(title) > TITLE_MAX_LEN:
+                errors.append(
+                    new_error(
+                        "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
+                            TITLE_MAX_LEN
+                        )
+                    )
+                )
+
+            # description validation
+            if not description:
+                errors.append(new_error("La descrizione del luogo è obbligatorio"))
+            elif len(description) > DESCRIPTION_MAX_LEN:
+                errors.append(
+                    new_error(
+                        "La descrizione del luogo deve avere una lunghezza di massimo {} caratteri".format(  # noqa
+                            DESCRIPTION_MAX_LEN
+                        )
+                    )
+                )
+
+            if (
+                not geolocation
+                or not geolocation.get("latitude")
+                or not geolocation.get("longitude")
+            ):
+                errors.append(
+                    new_error("La geolocalizzazione del luogo è un dato obbligatorio")
+                )
+
+            for field in MANDATORY_RICH_TEXT_FIELDS:
+                if field not in data:
+                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
+                elif field in data and not text_in_block(data.get(field)):
+                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
+
+        if is_patch:
+            # Title validation
+            if "title" in data and not title:
+                errors.append(new_error("Il titolo del luogo è obbligatorio"))
+            if title and len(title) > TITLE_MAX_LEN:
+                errors.append(
+                    new_error(
+                        "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
+                            TITLE_MAX_LEN
+                        )
+                    )
+                )
+            # description validation
+            if "description" in data and not description:
+                errors.append(new_error("La descrizione del luogo è obbligatorio"))
+            if description and len(description) > DESCRIPTION_MAX_LEN:
+                errors.append(
+                    new_error(
+                        "La descrizione del luogo deve avere una lunghezza di massimo {} caratteri".format(  # noqa
+                            DESCRIPTION_MAX_LEN
+                        )
+                    )
+                )
+
+            if "geolocation" in data and (
+                not geolocation
+                or not geolocation.get("latitude")
+                or not geolocation.get("longitude")
+            ):
+                errors.append(
+                    new_error("La geolocalizzazione del luogo è un dato obbligatorio")
+                )
+
+            for field in MANDATORY_RICH_TEXT_FIELDS:
+                if field in data and not text_in_block(data.get(field)):
+                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
+
+                # Se siamo nella patch siamo in modifica. Se siamo in modifica e siamo
+                # su un sito che ha avuto upgrade alla versione pnrr può essere che dei
+                # campi obbligatori #un tempo non lo fossero e quindi arriviamo fino a
+                # qui
+                if field not in data and not text_in_block(
+                    getattr(self.context, field)
+                ):
+                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
+
+            if "geolocation" not in data and not getattr(self.context, "geolocation"):
+                errors.append(
+                    new_error("La geolocalizzazione del luogo è un dato obbligatorio")
+                )
 
         if errors:
             raise BadRequest(errors)
-        return super(DeserializeUnitaOrganizzativaFromJson, self).__call__(
+        return super(DeserializeLuogoFromJson, self).__call__(
             validate_all=False, data=data, create=False
         )
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/deserializers/venue.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/deserializers/documento.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,161 +1,124 @@
 # -*- coding: utf-8 -*-
-from collective.venue.interfaces import IVenue
-from plone.restapi.behaviors import IBlocks
+from design.plone.contenttypes.interfaces.documento import IDocumento
+from design.plone.contenttypes.utils import text_in_block
 from plone.restapi.deserializer import json_body
 from plone.restapi.deserializer.dxcontent import DeserializeFromJson
-from plone.restapi.indexers import SearchableText_blocks
 from plone.restapi.interfaces import IDeserializeFromJson
 from zExceptions import BadRequest
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
 TITLE_MAX_LEN = 255
 DESCRIPTION_MAX_LEN = 255
 EMPTY_BLOCK_MARKER = {"@type": "text"}
-MANDATORY_RICH_TEXT_FIELDS = ["modalita_accesso"]
+MANDATORY_RICH_TEXT_FIELDS = [
+    # "descrizione_estesa",
+    "formati_disponibili",
+]
 
 
 def new_error(message):
     return {"error": "ValidationError", "message": message}
 
 
-def text_in_block(blocks):
-    @implementer(IBlocks)
-    class FakeObject(object):
-        """
-        We use a fake object to use SearchableText Indexer
-        """
-
-        def Subject(self):
-            return ""
-
-        def __init__(self, blocks, blocks_layout):
-            self.blocks = blocks
-            self.blocks_layout = blocks_layout
-            self.id = ""
-            self.title = ""
-            self.description = ""
-
-    if not blocks:
-        return None
-
-    fakeObj = FakeObject(blocks.get("blocks", ""), blocks.get("blocks_layout", ""))
-    return SearchableText_blocks(fakeObj)()
-
-
 @implementer(IDeserializeFromJson)
-@adapter(IVenue, Interface)
-class DeserializeLuogoFromJson(DeserializeFromJson):
+@adapter(IDocumento, Interface)
+class DeserializeDocumentoFromJson(DeserializeFromJson):
     def __call__(
         self, validate_all=False, data=None, create=False
     ):  # noqa: ignore=C901
         if data is None:
             data = json_body(self.request)
 
         method = self.request.get("method")
         is_post = method == "POST"
         is_patch = method == "PATCH"
         errors = []
 
-        title = data.get("title")
-        description = data.get("description")
-        geolocation = data.get("geolocation")
-
-        if is_post:
-            # Title validation
-            if not title:
-                errors.append(new_error("Il titolo del luogo è obbligatorio"))
-            elif len(title) > TITLE_MAX_LEN:
-                errors.append(
-                    new_error(
-                        "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
-                            TITLE_MAX_LEN
+        if list(data.keys()) != ["ordering"]:
+            title = data.get("title")
+            description = data.get("description")
+            if is_post:
+                # Title validation
+                if not title:
+                    errors.append(new_error("Il titolo è obbligatorio"))
+                elif len(title) > TITLE_MAX_LEN:
+                    errors.append(
+                        new_error(
+                            "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
+                                TITLE_MAX_LEN
+                            )
                         )
                     )
-                )
 
-            # description validation
-            if not description:
-                errors.append(new_error("La descrizione del luogo è obbligatorio"))
-            elif len(description) > DESCRIPTION_MAX_LEN:
-                errors.append(
-                    new_error(
-                        "La descrizione del luogo deve avere una lunghezza di massimo {} caratteri".format(  # noqa
-                            DESCRIPTION_MAX_LEN
+                # description validation
+                if not description:
+                    errors.append(new_error("La descrizione è obbligatoria"))
+                elif len(description) > DESCRIPTION_MAX_LEN:
+                    errors.append(
+                        new_error(
+                            "La descrizione deve avere una lunghezza di massimo {} caratteri".format(  # noqa
+                                DESCRIPTION_MAX_LEN
+                            )
                         )
                     )
-                )
 
-            if (
-                not geolocation
-                or not geolocation.get("latitude")
-                or not geolocation.get("longitude")
-            ):
-                errors.append(
-                    new_error("La geolocalizzazione del luogo è un dato obbligatorio")
-                )
-
-            for field in MANDATORY_RICH_TEXT_FIELDS:
-                if field not in data:
-                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
-                elif field in data and not text_in_block(data.get(field)):
-                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
-
-        if is_patch:
-            # Title validation
-            if "title" in data and not title:
-                errors.append(new_error("Il titolo del luogo è obbligatorio"))
-            if title and len(title) > TITLE_MAX_LEN:
-                errors.append(
-                    new_error(
-                        "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
-                            TITLE_MAX_LEN
+                for field in MANDATORY_RICH_TEXT_FIELDS:
+                    if field not in data:
+                        errors.append(
+                            new_error("Il campo {} è obbligatorio".format(field))
+                        )
+                    elif field in data and not text_in_block(data.get(field)):
+                        errors.append(
+                            new_error("Il campo {} è obbligatorio".format(field))
+                        )
+
+            if is_patch:
+                # Title validation
+                if "title" in data and not title:
+                    errors.append(new_error("Il titolo è obbligatorio"))
+                if title and len(title) > TITLE_MAX_LEN:
+                    errors.append(
+                        new_error(
+                            "Il titolo può avere una lunghezza di massimo {} caratteri".format(  # noqa
+                                TITLE_MAX_LEN
+                            )
                         )
                     )
-                )
-            # description validation
-            if "description" in data and not description:
-                errors.append(new_error("La descrizione del luogo è obbligatorio"))
-            if description and len(description) > DESCRIPTION_MAX_LEN:
-                errors.append(
-                    new_error(
-                        "La descrizione del luogo deve avere una lunghezza di massimo {} caratteri".format(  # noqa
-                            DESCRIPTION_MAX_LEN
+                # description validation
+                if "description" in data and not description:
+                    errors.append(new_error("La descrizione è obbligatoria"))
+                if description and len(description) > DESCRIPTION_MAX_LEN:
+                    errors.append(
+                        new_error(
+                            "La descrizione deve avere una lunghezza di massimo {} caratteri".format(  # noqa
+                                DESCRIPTION_MAX_LEN
+                            )
                         )
                     )
-                )
+                if "description" not in data and not self.context.description:
+                    errors.append(new_error("La descrizione è obbligatoria"))
 
-            if "geolocation" in data and (
-                not geolocation
-                or not geolocation.get("latitude")
-                or not geolocation.get("longitude")
-            ):
-                errors.append(
-                    new_error("La geolocalizzazione del luogo è un dato obbligatorio")
-                )
-
-            for field in MANDATORY_RICH_TEXT_FIELDS:
-                if field in data and not text_in_block(data.get(field)):
-                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
-
-                # Se siamo nella patch siamo in modifica. Se siamo in modifica e siamo
-                # su un sito che ha avuto upgrade alla versione pnrr può essere che dei
-                # campi obbligatori #un tempo non lo fossero e quindi arriviamo fino a
-                # qui
-                if field not in data and not text_in_block(
-                    getattr(self.context, field)
-                ):
-                    errors.append(new_error("Il campo {} è obbligatorio".format(field)))
-
-            if "geolocation" not in data and not getattr(self.context, "geolocation"):
-                errors.append(
-                    new_error("La geolocalizzazione del luogo è un dato obbligatorio")
-                )
+                for field in MANDATORY_RICH_TEXT_FIELDS:
+                    if field in data and not text_in_block(data.get(field)):
+                        errors.append(
+                            new_error("Il campo {} è obbligatorio".format(field))
+                        )
+                    # Se siamo nella patch siamo in modifica. Se siamo in modifica e
+                    # siamo su un sito che ha avuto upgrade alla versione pnrr può
+                    # essere che dei campi obbligatori un tempo non lo fossero e quindi
+                    # arriviamo fino a qui
+                    if field not in data and not text_in_block(
+                        getattr(self.context, field)
+                    ):
+                        errors.append(
+                            new_error("Il campo {} è obbligatorio".format(field))
+                        )
 
         if errors:
             raise BadRequest(errors)
-        return super(DeserializeLuogoFromJson, self).__call__(
+        return super(DeserializeDocumentoFromJson, self).__call__(
             validate_all=False, data=data, create=False
         )
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/bando.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/documento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/dxcontent.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/dxcontent.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/dxfields.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/dxfields.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/modulo.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/persona.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/punto_di_contatto.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/related_news_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/relationfield.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/relationfield.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/servizio.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/summary.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,30 +179,36 @@
             if res["tassonomia_argomenti"]:
                 res["tassonomia_argomenti"] = self.expand_tassonomia_argomenti()
 
         get_taxonomy_information_by_type(res, self.context)
 
         if self.is_get_call():
             res["has_children"] = self.has_children()
-
         if force_images:
             # TODO: verificare se non c'è il campo o se il campo è null/vuoto ?
             if not res.get("image_scales") and not res.get("image_field"):
                 adapter = queryMultiAdapter(
                     (self.context, self.request), IImageScalesAdapter
                 )
                 if adapter:
                     scales = adapter()
                     if scales:
                         res["image_scales"] = scales
                     if "preview_image" in scales:
                         res["image_field"] = "preview_image"
                     elif "image" in scales:
                         res["image_field"] = "image"
-
+            # plone.app.contentlisting 3.0.5 sembra fissare un accessor che ci
+            # fa arrivare uno scale senza image_field.
+            # avremmo questo problema una volta passati a plone 6.0.11
+            elif res.get("image_scales") and not res.get("image_field"):
+                if "preview_image" in res["image_scales"]:
+                    res["image_field"] = "preview_image"
+                elif "image" in res["image_scales"]:
+                    res["image_field"] = "image"
         return res
 
     def has_children(self):
         try:
             obj = self.context.getObject()
         except AttributeError:
             obj = self.context
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/serializers/venue.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/serializers/venue.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/content/add.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/content/add.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/controlpanel.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/controlpanel.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/modulistica_items/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/modulistica_items/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/navigation/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/navigation/get.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/navigation/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/scadenziario/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/scadenziario/post.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/scadenziario/post.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/trasparenza/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/trasparenza/get.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/trasparenza/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/services/types/get.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/services/types/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/restapi/types/adapters.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/restapi/types/adapters.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/schema_overrides.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/schema_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/setuphandlers.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/testing.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/example.pdf` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/example.pdf`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/example.png` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/example.png`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_argomenti.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_argomenti.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_base_serializer.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_base_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_descrizione_estesa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_exclude_from_search.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_luogo.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_show_modified.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_show_modified.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_behavior_update_note.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_behavior_update_note.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_change_news_type.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_change_news_type.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_bando.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_bando.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_cartella_modulistica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_document.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_document.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_documento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_documento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_event.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_event.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_folder.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_luogo.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_luogo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_modulo.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_modulo.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_news.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_news.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_pagina_argomento.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_persona.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_persona.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_servizio.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_ct_unita_organizzativa.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_custom_service_navigation.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_custom_service_navigation.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_filefield_custom_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_move_news_items_view.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_move_news_items_view.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_relateditems_with_dates.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_service_scadenziario.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_service_scadenziario.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_settings_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_setup.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_substructure_creation.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_substructure_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,15 @@
         - curriculum-vitae
         - situazione-patrimoniale
         - dichiarazione-dei-redditi
         - spese-elettorali
         - spese-elettorali
         - variazione-situazione-patrimoniale" "altre-cariche
         - incarichi
+        - altri-documenti
         """
         item = api.content.create(
             container=self.portal,
             type="Persona",
             title="Test",
         )
 
@@ -235,14 +236,15 @@
                 "curriculum-vitae",
                 "situazione-patrimoniale",
                 "dichiarazione-dei-redditi",
                 "spese-elettorali",
                 "variazione-situazione-patrimoniale",
                 "altre-cariche",
                 "incarichi",
+                "altri-documenti",
             ],
         )
 
         self.assertEqual(item["foto-e-attivita-politica"].portal_type, "Document")
         self.assertEqual(
             api.content.get_state(item["foto-e-attivita-politica"]), "private"
         )
@@ -313,14 +315,22 @@
 
         self.assertEqual(item["incarichi"].portal_type, "Document")
         self.assertEqual(api.content.get_state(item["incarichi"]), "private")
         self.assertEqual(item["incarichi"].constrain_types_mode, 1)
         self.assertEqual(item["incarichi"].locally_allowed_types, ("Incarico",))
         self.assertTrue(item["incarichi"].exclude_from_search)
 
+        self.assertEqual(item["altri-documenti"].portal_type, "Document")
+        self.assertEqual(api.content.get_state(item["altri-documenti"]), "private")
+        self.assertEqual(item["altri-documenti"].constrain_types_mode, 1)
+        self.assertIn("File", item["altri-documenti"].locally_allowed_types)
+        self.assertIn("Link", item["altri-documenti"].locally_allowed_types)
+        self.assertIn("Image", item["altri-documenti"].locally_allowed_types)
+        self.assertTrue(item["altri-documenti"].exclude_from_search)
+
     def test_servizio_substructure_created(self):
         """
         Should have:
         - modulistica
         - allegati
         """
         item = api.content.create(
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_summary_serializer.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_summary_serializer.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_uo_summary_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,19 @@
             title="UO",
         )
         commit()
         response = self.api_session.get(uo.absolute_url())
         res = response.json()
         uo_children = res["uo_children"][0]
         self.assertEqual(uo_children["image_field"], None)
-        self.assertEqual(uo_children["image_scales"], None)
+        # Plone 6.0.10.1 due to a bug in plone.app.contentlisting (#64
+        # from github issue) return None
+        # Plone 6.0.11 upgrades plone.app.contentlisting to a version
+        # fixing the problem and the changing the return value to {}
+        self.assertIn(uo_children["image_scales"], (None, {}))
 
         # now, add a preview image
         filename = os.path.join(os.path.dirname(__file__), "example.png")
         uo2.preview_image = NamedBlobImage(
             data=open(filename, "rb").read(),
             filename="example.png",
             contentType="image/png",
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/tests/test_vocabularies.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/configure.zcml`

 * *Files 0% similar despite different names*

```diff
@@ -580,15 +580,15 @@
     <genericsetup:upgradeStep
         title="Add new index for Argomenti UID"
         handler=".upgrades.to_5500"
         />
   </genericsetup:upgradeSteps>
   <genericsetup:upgradeSteps
       profile="design.plone.contenttypes:default"
-      source="6000"
+      source="5500"
       destination="6000"
       >
     <genericsetup:upgradeStep
         title="Plone6 and pip"
         handler=".upgrades.to_6000"
         />
   </genericsetup:upgradeSteps>
@@ -852,9 +852,16 @@
   <genericsetup:upgradeStep
       title="Migrate from File/Image Field to BlobField"
       profile="design.plone.contenttypes:default"
       source="7200"
       destination="7300"
       handler=".to_7300.to_7300"
       />
+  <genericsetup:upgradeStep
+      title="Add new folder to persona ct"
+      profile="design.plone.contenttypes:default"
+      source="7300"
+      destination="7301"
+      handler=".to_730x.to_7301"
+      />
 
 </configure>
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/draftjs_converter.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/draftjs_converter.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/to_7001.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_7001.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/to_7002.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_7002.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/to_7300.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/to_7300.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .upgrades import logger
 from Acquisition import aq_base
 from plone import api
 from plone.namedfile import file
 
 
 def to_7300(context):
-
     mapping = {
         # portal_type
         "Documento Personale": {
             # field: "type"
             "immagine": "image",
             "pratica_associata": "file",
         },
```

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/upgrades/upgrades.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/configure.zcml` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/mockup.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/mockup.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/people_vocabulary.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/people_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/reference_vocabularies.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py` & `design_plone_contenttypes-6.2.9/src/design/plone/contenttypes/vocabularies/tags_vocabulary.py`

 * *Files identical despite different names*

### Comparing `design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/PKG-INFO` & `design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.contenttypes
-Version: 6.2.8
+Version: 6.2.9
 Summary: DesignItalia contenty types
 Home-page: https://github.com/collective/design.plone.contenttypes
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.contenttypes
 Project-URL: Source, https://github.com/RedTurtle/design.plone.contenttypes
@@ -20,17 +20,38 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: z3c.jbot
+Requires-Dist: plone.api>=1.8.4
+Requires-Dist: plone.app.dexterity>2.6.9
+Requires-Dist: collective.venue[geolocation]
+Requires-Dist: collective.volto.blocksfield
+Requires-Dist: collective.z3cform.datagridfield
+Requires-Dist: plone.formwidget.geolocation
+Requires-Dist: redturtle.volto>=5.0.0
+Requires-Dist: redturtle.bandi
+Requires-Dist: z3c.unconfigure
+Requires-Dist: plone.restapi
+Requires-Dist: eea.api.taxonomy
+Requires-Dist: openpyxl
+Requires-Dist: collective.volto.enhancedlinks
+Provides-Extra: test
+Requires-Dist: plone.app.testing; extra == "test"
+Requires-Dist: collective.volto.blocksfield; extra == "test"
+Requires-Dist: plone.testing>=5.0.0; extra == "test"
+Requires-Dist: plone.app.contenttypes; extra == "test"
+Requires-Dist: plone.app.robotframework[debug]; extra == "test"
+Requires-Dist: collective.MockMailHost; extra == "test"
 
 [![Latest Version](https://img.shields.io/pypi/v/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Supported - Python Versions](https://img.shields.io/pypi/pyversions/design.plone.contenttypes.svg?style=plastic)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![License](https://img.shields.io/pypi/l/design.plone.contenttypes.svg)](https://pypi.python.org/pypi/design.plone.contenttypes/)
 [![Tests](https://github.com/RedTurtle/design.plone.contenttypes/actions/workflows/tests.yml/badge.svg)](https://github.com/RedTurtle/design.plone.contenttypes/actions)
 [![Coverage](https://coveralls.io/repos/github/RedTurtle/design.plone.contenttypes/badge.svg?branch=main)](https://coveralls.io/github/RedTurtle/design.plone.contenttypes?branch=main)
@@ -498,14 +519,25 @@
 
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
+6.2.9 (2024-05-21)
+------------------
+
+- Add this folder "Altri Documenti" under "Persona pubblica"
+  [lucabel]
+- Code porting to work with both plone 6.0.10.x and 6.0.11
+  due to some core egg update
+  Code porting to work with the new plone.restapi 9.6.1 version
+  [lucabel]
+
+
 6.2.8 (2024-04-22)
 ------------------
 
 - Add start metadata to event summary serialization;
   useful when create event with children event: in items list we
   have subevents with missing start date
   [lucabel]
```

### Comparing `design.plone.contenttypes-6.2.8/src/design.plone.contenttypes.egg-info/SOURCES.txt` & `design_plone_contenttypes-6.2.9/src/design.plone.contenttypes.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -307,14 +307,15 @@
 src/design/plone/contenttypes/tests/test_vocabularies.py
 src/design/plone/contenttypes/upgrades/__init__.py
 src/design/plone/contenttypes/upgrades/configure.zcml
 src/design/plone/contenttypes/upgrades/draftjs_converter.py
 src/design/plone/contenttypes/upgrades/to_7001.py
 src/design/plone/contenttypes/upgrades/to_7002.py
 src/design/plone/contenttypes/upgrades/to_7300.py
+src/design/plone/contenttypes/upgrades/to_730x.py
 src/design/plone/contenttypes/upgrades/upgrades.py
 src/design/plone/contenttypes/vocabularies/__init__.py
 src/design/plone/contenttypes/vocabularies/argomenti_vocabulary.py
 src/design/plone/contenttypes/vocabularies/available_services_vocabulary.py
 src/design/plone/contenttypes/vocabularies/configure.zcml
 src/design/plone/contenttypes/vocabularies/controlapanel_vocabularies.py
 src/design/plone/contenttypes/vocabularies/lista_azioni_pratica.py
```

### Comparing `design.plone.contenttypes-6.2.8/tox.ini` & `design_plone_contenttypes-6.2.9/tox.ini`

 * *Files identical despite different names*

