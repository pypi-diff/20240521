# Comparing `tmp/esupar-1.7.1-py3-none-any.whl.zip` & `tmp/esupar-1.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 59907 bytes, number of entries: 13
+Zip file size: 59908 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       25 b- defN 21-Sep-17 12:30 esupar/__init__.py
 -rw-r--r--  2.0 unx     2922 b- defN 23-Feb-06 04:16 esupar/ainu.py
--rw-r--r--  2.0 unx    10852 b- defN 24-May-09 02:24 esupar/esupar.py
+-rw-r--r--  2.0 unx    10856 b- defN 24-May-20 23:29 esupar/esupar.py
 -rw-r--r--  2.0 unx    35949 b- defN 22-Nov-30 11:18 esupar/hangul.py
 -rw-r--r--  2.0 unx     1202 b- defN 23-Nov-05 09:09 esupar/mecab.py
 -rw-r--r--  2.0 unx    48825 b- defN 24-Feb-29 02:30 esupar/simplify.py
 -rw-r--r--  2.0 unx    19301 b- defN 24-Feb-29 02:31 esupar/tradify.py
 -rw-r--r--  2.0 unx    11241 b- defN 24-Feb-06 04:22 esupar/train.py
--rw-r--r--  2.0 unx     1071 b- defN 24-May-09 02:25 esupar-1.7.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6856 b- defN 24-May-09 02:25 esupar-1.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 02:25 esupar-1.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-May-09 02:25 esupar-1.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      972 b- defN 24-May-09 02:25 esupar-1.7.1.dist-info/RECORD
-13 files, 139315 bytes uncompressed, 58323 bytes compressed:  58.1%
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-20 23:30 esupar-1.7.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6864 b- defN 24-May-20 23:30 esupar-1.7.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 23:30 esupar-1.7.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-20 23:30 esupar-1.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      972 b- defN 24-May-20 23:30 esupar-1.7.2.dist-info/RECORD
+13 files, 139327 bytes uncompressed, 58324 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: esupar/tradify.py
 Comment: 
 
 Filename: esupar/train.py
 Comment: 
 
-Filename: esupar-1.7.1.dist-info/LICENSE.txt
+Filename: esupar-1.7.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: esupar-1.7.1.dist-info/METADATA
+Filename: esupar-1.7.2.dist-info/METADATA
 Comment: 
 
-Filename: esupar-1.7.1.dist-info/WHEEL
+Filename: esupar-1.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: esupar-1.7.1.dist-info/top_level.txt
+Filename: esupar-1.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: esupar-1.7.1.dist-info/RECORD
+Filename: esupar-1.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## esupar/esupar.py

```diff
@@ -23,15 +23,15 @@
   "ko_morph":"KoichiYasuoka/roberta-base-korean-morph-upos",
   "ko_morph_base":"KoichiYasuoka/roberta-base-korean-morph-upos",
   "ko_morph_large":"KoichiYasuoka/roberta-large-korean-morph-upos",
   "lzh":"KoichiYasuoka/roberta-classical-chinese-base-upos",
   "lzh_base":"KoichiYasuoka/roberta-classical-chinese-base-upos",
   "lzh_large":"KoichiYasuoka/roberta-classical-chinese-large-upos",
   "sr":"KoichiYasuoka/roberta-base-serbian-upos",
-  "th":"KoichiYasuoka/deberta-base-thai-upos",
+  "th":"KoichiYasuoka/roberta-base-thai-spm-upos",
   "vi":"KoichiYasuoka/bert-base-vietnamese-upos",
   "zh":"KoichiYasuoka/chinese-bert-wwm-ext-upos",
   "zh_bert":"KoichiYasuoka/chinese-bert-wwm-ext-upos",
   "zh_base":"KoichiYasuoka/chinese-roberta-base-upos",
   "zh_large":"KoichiYasuoka/chinese-roberta-large-upos"
 }
 LEMMATIZE={
```

## Comparing `esupar-1.7.1.dist-info/LICENSE.txt` & `esupar-1.7.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `esupar-1.7.1.dist-info/METADATA` & `esupar-1.7.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esupar
-Version: 1.7.1
+Version: 1.7.2
 Summary: Tokenizer POS-tagger and Dependency-parser with BERT/RoBERTa/DeBERTa models for Japanese and other languages
 Home-page: https://github.com/KoichiYasuoka/esupar
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: Source, https://github.com/KoichiYasuoka/esupar
 Project-URL: Tracker, https://github.com/KoichiYasuoka/esupar/issues
@@ -85,15 +85,15 @@
 * `model="ko_morph_base"` Korean morpheme model [roberta-base-korean-morph-upos](https://huggingface.co/KoichiYasuoka/roberta-base-korean-morph-upos)
 * `model="ko_morph_large"` Korean morpheme model [roberta-large-korean-morph-upos](https://huggingface.co/KoichiYasuoka/roberta-large-korean-morph-upos)
 * `model="zh"` Chinese model [chinese-bert-wwm-ext-upos](https://huggingface.co/KoichiYasuoka/chinese-bert-wwm-ext-upos)
 * `model="zh_base"` Chinese model [chinese-roberta-base-upos](https://huggingface.co/KoichiYasuoka/chinese-roberta-base-upos)
 * `model="zh_large"` Chinese model [chinese-roberta-large-upos](https://huggingface.co/KoichiYasuoka/chinese-roberta-large-upos)
 * `model="lzh"` Classical Chinese model [roberta-classical-chinese-base-upos](https://huggingface.co/KoichiYasuoka/roberta-classical-chinese-base-upos)
 * `model="lzh_large"` Classical Chinese model [roberta-classical-chinese-large-upos](https://huggingface.co/KoichiYasuoka/roberta-classical-chinese-large-upos)
-* `model="th"` Thai model [deberta-base-thai-upos](https://huggingface.co/KoichiYasuoka/deberta-base-thai-upos)
+* `model="th"` Thai model [roberta-base-thai-spm-upos](https://huggingface.co/KoichiYasuoka/roberta-base-thai-spm-upos)
 * `model="vi"` Vietnamese model [bert-base-vietnamese-upos](https://huggingface.co/KoichiYasuoka/bert-base-vietnamese-upos)
 * `model="en"` English model [roberta-base-english-upos](https://huggingface.co/KoichiYasuoka/roberta-base-english-upos)
 * `model="en_large"` English model [roberta-large-english-upos](https://huggingface.co/KoichiYasuoka/roberta-large-english-upos)
 * `model="de"` German model [bert-base-german-upos](https://huggingface.co/KoichiYasuoka/bert-base-german-upos)
 * `model="de_large"` German model [bert-large-german-upos](https://huggingface.co/KoichiYasuoka/bert-large-german-upos)
 * `model="sr"` Serbian (Cyrillic and Latin) model [roberta-base-serbian-upos](https://huggingface.co/KoichiYasuoka/roberta-base-serbian-upos)
 * `model="cop"` Coptic model [roberta-base-coptic-upos](https://huggingface.co/KoichiYasuoka/roberta-base-coptic-upos)
```

## Comparing `esupar-1.7.1.dist-info/RECORD` & `esupar-1.7.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 esupar/__init__.py,sha256=WFHrDfbc3mwVJWPVIsRhF8RWkFX_WHFkHlyfESJg_TE,25
 esupar/ainu.py,sha256=qxfj8LtRlG9Z0TyQkyn0W9EoW-a_e3h10HwTRNqGBp8,2922
-esupar/esupar.py,sha256=7B2FP4buxFC2alIzGVdzk0QO22GrUFJmjAW7I0S6O8o,10852
+esupar/esupar.py,sha256=itCNPvxmAyFqQe06kZxZjlnojRIZIHN3SQBOmIcHReI,10856
 esupar/hangul.py,sha256=kZV0_pkhTGqi1FWrLUm_oBg-6pcLEhtGVJlp5-bKC80,35949
 esupar/mecab.py,sha256=MXvtduJn4vYhSMqNO3CHh4-DNAJwq8-DwsQOQHLHDAw,1202
 esupar/simplify.py,sha256=KQEmWS0MfpbKf4xfrs5xe6LdManlQ-rq7BsJwm7Wvvk,48825
 esupar/tradify.py,sha256=5WNwRmbbPezauQ_yd7_hsgr2x2PpsMIqU9H154F_6e0,19301
 esupar/train.py,sha256=pGneN0SYBF9j95dKFqtm8yUvj3wEy2eVwN9M5TDk5qY,11241
-esupar-1.7.1.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
-esupar-1.7.1.dist-info/METADATA,sha256=7EqbYDI1ScQvK_J08oc35-4hny4XXDetYio9xItkVqQ,6856
-esupar-1.7.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-esupar-1.7.1.dist-info/top_level.txt,sha256=Ps1TtlXQ41i0vydx2GN32ODNxAdE9Jw7cAWHFqBo5Pk,7
-esupar-1.7.1.dist-info/RECORD,,
+esupar-1.7.2.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
+esupar-1.7.2.dist-info/METADATA,sha256=cYXuVz3NxfjZ_Nj96lps43qpkP0p7wQc1ys-_QlkD-E,6864
+esupar-1.7.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+esupar-1.7.2.dist-info/top_level.txt,sha256=Ps1TtlXQ41i0vydx2GN32ODNxAdE9Jw7cAWHFqBo5Pk,7
+esupar-1.7.2.dist-info/RECORD,,
```

