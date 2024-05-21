# Comparing `tmp/ruaccent-1.5.6.3.tar.gz` & `tmp/ruaccent-1.5.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruaccent-1.5.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ruaccent-1.5.6.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ruaccent-1.5.6.3.tar` & `ruaccent-1.5.6.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rwxr-xr-x   0        0        0      552 2024-03-16 16:48:46.914515 ruaccent-1.5.6.3/LICENSE
--rwxr-xr-x   0        0        0     2190 2024-03-14 17:27:50.064584 ruaccent-1.5.6.3/README.md
--rwxr-xr-x   0        0        0      539 2024-03-16 16:08:59.058722 ruaccent-1.5.6.3/pyproject.toml
--rwxr-xr-x   0        0        0     4539 2024-03-26 08:18:20.244439 ruaccent-1.5.6.3/ruaccent/.ipynb_checkpoints/rule_accent_engine-checkpoint.py
--rwxr-xr-x   0        0        0       83 2024-03-26 08:17:12.663815 ruaccent-1.5.6.3/ruaccent/__init__.py
--rwxr-xr-x   0        0        0     1722 2024-03-14 16:22:36.039466 ruaccent-1.5.6.3/ruaccent/accent_model.py
--rwxr-xr-x   0        0        0     2999 2024-03-14 16:22:35.973356 ruaccent-1.5.6.3/ruaccent/char_tokenizer.py
--rwxr-xr-x   0        0        0     5105 2024-03-14 16:54:59.012852 ruaccent-1.5.6.3/ruaccent/omograph_model.py
--rwxr-xr-x   0        0        0    10101 2024-03-16 16:31:44.869284 ruaccent-1.5.6.3/ruaccent/ruaccent.py
--rwxr-xr-x   0        0        0     4539 2024-03-26 08:18:20.244439 ruaccent-1.5.6.3/ruaccent/rule_accent_engine.py
--rwxr-xr-x   0        0        0     4777 2024-03-14 16:22:36.039372 ruaccent-1.5.6.3/ruaccent/stress_usage_model.py
--rwxr-xr-x   0        0        0     4906 2024-03-14 16:22:36.039564 ruaccent-1.5.6.3/ruaccent/text_split.py
--rwxr-xr-x   0        0        0     4740 2024-03-14 16:22:30.916368 ruaccent-1.5.6.3/ruaccent/yo_homograph_model.py
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 ruaccent-1.5.6.3/PKG-INFO
+-rwxr-xr-x   0        0        0      552 2024-03-16 16:48:46.914515 ruaccent-1.5.6.4/LICENSE
+-rwxr-xr-x   0        0        0     2205 2024-05-21 09:36:45.577600 ruaccent-1.5.6.4/README.md
+-rwxr-xr-x   0        0        0      552 2024-05-21 09:52:52.080930 ruaccent-1.5.6.4/pyproject.toml
+-rwxr-xr-x   0        0        0       83 2024-05-21 09:37:08.541434 ruaccent-1.5.6.4/ruaccent/__init__.py
+-rwxr-xr-x   0        0        0     1722 2024-03-14 16:22:36.039466 ruaccent-1.5.6.4/ruaccent/accent_model.py
+-rwxr-xr-x   0        0        0     2999 2024-03-14 16:22:35.973356 ruaccent-1.5.6.4/ruaccent/char_tokenizer.py
+-rwxr-xr-x   0        0        0     5105 2024-03-14 16:54:59.012852 ruaccent-1.5.6.4/ruaccent/omograph_model.py
+-rwxr-xr-x   0        0        0    10307 2024-05-21 09:52:27.955130 ruaccent-1.5.6.4/ruaccent/ruaccent.py
+-rwxr-xr-x   0        0        0     4575 2024-05-21 09:37:44.967704 ruaccent-1.5.6.4/ruaccent/rule_accent_engine.py
+-rwxr-xr-x   0        0        0     4777 2024-03-14 16:22:36.039372 ruaccent-1.5.6.4/ruaccent/stress_usage_model.py
+-rwxr-xr-x   0        0        0     4906 2024-03-14 16:22:36.039564 ruaccent-1.5.6.4/ruaccent/text_split.py
+-rwxr-xr-x   0        0        0     4740 2024-03-14 16:22:30.916368 ruaccent-1.5.6.4/ruaccent/yo_homograph_model.py
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 ruaccent-1.5.6.4/PKG-INFO
```

### Comparing `ruaccent-1.5.6.3/LICENSE` & `ruaccent-1.5.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/README.md` & `ruaccent-1.5.6.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
    ```
    pip install git+https://github.com/Den4ikAI/ruaccent.git
    ```
 ## Параметры работы
 
     load(omograph_model_size='turbo', use_dictionary=True, custom_dict={}, device="CPU", workdir=None)
 
- - На данный момент доступно 4 модели - **turbo**, **big_poetry**, **medium_poetry**, **small_poetry**
+ - На данный момент доступно 5 моделей - **turbo2**, **turbo**, **big_poetry**, **medium_poetry**, **small_poetry**
  - Переменная **use_dictionary** отвечает за загрузку всего словаря (требуется больше ОЗУ), иначе все ударения расставляет нейросеть. 
  - Функция **custom_dict** отвечает за добавление своих вариантов ударений в словарь. Формат такой: `{'слово': 'сл+ово с удар+ением'}`
 - Выбор устройства CPU или CUDA. **Для работы с CUDA требуется установить onnxruntime-gpu и CUDA.**
 - workdir - принимает строку. Является путём, куда скачиваются модели.
     
     **Для стабильной работы требуется минимум 3 гигабайта ОЗУ**
 ## Пример использования
 ```python
 from ruaccent import RUAccent
 
 accentizer = RUAccent()
-accentizer.load(omograph_model_size='turbo', use_dictionary=True)
+accentizer.load(omograph_model_size='turbo2', use_dictionary=True)
 
 text = 'на двери висит замок.'
 print(accentizer.process_all(text))
 ```
 
 Файлы моделей и словарей располагаются по [ссылке](https://huggingface.co/ruaccent/accentuator). Мы будем признательны фидбеку на [telegram аккаунт](https://t.me/chckdskeasfsd)
```

### Comparing `ruaccent-1.5.6.3/pyproject.toml` & `ruaccent-1.5.6.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 dependencies = [
     "huggingface_hub",
     "onnxruntime",
     "transformers",
     "sentencepiece",
     "numpy",
     "python-crfsuite",
+    "razdel"
 ]
 
 [project.urls]
 Home = "https://github.com/Den4ikAI/ruaccent"
```

### Comparing `ruaccent-1.5.6.3/ruaccent/.ipynb_checkpoints/rule_accent_engine-checkpoint.py` & `ruaccent-1.5.6.4/ruaccent/rule_accent_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 class RuleEngine:
     def __init__(self):
         self.wordforms = {}
         self.forms_dict = {}
 
     def load(self, path):
-        with open(file=join_path(path, "accents.json"), mode='r') as f:
+        with open(file=join_path(path, "accents.json"), mode='r', encoding="utf-8") as f:
             self.wordforms = json.load(f)
-        with open(file=join_path(path, "forms.json"), mode='r') as f:
+        with open(file=join_path(path, "forms.json"), mode='r', encoding="utf-8") as f:
             self.forms_dict = json.load(f)
         self.lemmatizer = Lemmatizer()
         self.lemmatizer.load()
         self.tagger = RuPosTagger()
         self.tagger.load()
     def split_by_words(self, string):
         string = string.replace(" - ",' ~ ')
```

### Comparing `ruaccent-1.5.6.3/ruaccent/accent_model.py` & `ruaccent-1.5.6.4/ruaccent/accent_model.py`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/ruaccent/char_tokenizer.py` & `ruaccent-1.5.6.4/ruaccent/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/ruaccent/omograph_model.py` & `ruaccent-1.5.6.4/ruaccent/omograph_model.py`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/ruaccent/ruaccent.py` & `ruaccent-1.5.6.4/ruaccent/ruaccent.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import gzip
 from os.path import join as join_path
 from .omograph_model import OmographModel
 from .accent_model import AccentModel
 from .stress_usage_model import StressUsagePredictorModel
 from .yo_homograph_model import YoHomographModel
-from .text_split import split_by_sentences
+from razdel import sentenize
 import re
 
 
 
 class RUAccent:
     def __init__(self):
         self.omograph_model = OmographModel()
@@ -23,22 +23,23 @@
         self.normalize = re.compile(r"[^a-zA-Z0-9\sа-яА-ЯёЁ.,!?:;""''(){}\[\]«»„“”-]")
         self.omograph_models_paths = {'big': '/nn/nn_omograph/big', 
                                       'medium': '/nn/nn_omograph/medium', 
                                       'small': '/nn/nn_omograph/small', 
                                       'big_poetry': '/nn/nn_omograph/big_poetry', 
                                       'medium_poetry': '/nn/nn_omograph/medium_poetry', 
                                       'small_poetry': '/nn/nn_omograph/small_poetry',
-                                      'turbo': '/nn/nn_omograph/turbo'}
+                                      'turbo': '/nn/nn_omograph/turbo',
+                                      'turbo2': '/nn/nn_omograph/turbo2'}
     
         self.accentuator_paths = ['/nn/nn_accent', '/nn/nn_stress_usage_predictor','/nn/nn_yo_homograph_resolver', '/dictionary', '/dictionary/rule_engine']
         self.letters_accent = {'о': '+о', 'О': '+О'}
         self.koziev_paths = ["/koziev/rulemma", "/koziev/rupostagger", "/koziev/rupostagger/database"]
     def load(
         self,
-        omograph_model_size="big_poetry",
+        omograph_model_size="turbo2",
         use_dictionary=False,
         custom_dict={},
         custom_homographs={},
         device="CPU",
         repo="ruaccent/accentuator",
         workdir=None
         ):
@@ -108,14 +109,18 @@
         self.rule_accent.load(join_path(self.workdir, "dictionary","rule_engine"))
 
     def split_by_words(self, string):
         string = string.replace(" - ",' ~ ')
         result = re.findall(r"\w*(?:\+\w+)*|[^\w\s]+", string.lower())
         return [res for res in result if res]
 
+    def split_by_sentences(self, string):
+        result = list(sentenize(text))
+        result = [_.text for _ in result]
+        return result
 
     def count_vowels(self, text):
         vowels = "аеёиоуыэюяАЕЁИОУЫЭЮЯ"
         return sum(1 for char in text if char in vowels)
 
     def has_punctuation(self, text):
         for char in text:
@@ -212,15 +217,15 @@
             processed_text = " ".join(processed_text)
             processed_text = self.delete_spaces_before_punc(processed_text)
             outputs.append(processed_text)
         return " ".join(outputs)
     
     def process_all(self, text):
         text = re.sub(self.normalize, "", text)
-        sentences = split_by_sentences(text)
+        sentences = self.split_by_sentences(text)
         outputs = []
         for sentence in sentences:
             text = self.split_by_words(sentence)
             accented_tokens = self.rule_accent.accentuate(sentence)
             if len(accented_tokens) == len(text):
                 for i in range(len(text)):
                     if '+' in accented_tokens[i]:
```

### Comparing `ruaccent-1.5.6.3/ruaccent/stress_usage_model.py` & `ruaccent-1.5.6.4/ruaccent/stress_usage_model.py`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/ruaccent/text_split.py` & `ruaccent-1.5.6.4/ruaccent/text_split.py`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/ruaccent/yo_homograph_model.py` & `ruaccent-1.5.6.4/ruaccent/yo_homograph_model.py`

 * *Files identical despite different names*

### Comparing `ruaccent-1.5.6.3/PKG-INFO` & `ruaccent-1.5.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ruaccent
-Version: 1.5.6.3
+Version: 1.5.6.4
 Summary: Russian accentizer
 Author-email: Denis Petrov <arduino4b@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: huggingface_hub
 Requires-Dist: onnxruntime
 Requires-Dist: transformers
 Requires-Dist: sentencepiece
 Requires-Dist: numpy
 Requires-Dist: python-crfsuite
+Requires-Dist: razdel
 Project-URL: Home, https://github.com/Den4ikAI/ruaccent
 
 # RUAccent
 
 RUAccent - это библиотека для автоматической расстановки ударений на русском языке.
 
 **Внимание!!! Смена лицензии на Apache 2.0**
@@ -29,27 +30,27 @@
    ```
    pip install git+https://github.com/Den4ikAI/ruaccent.git
    ```
 ## Параметры работы
 
     load(omograph_model_size='turbo', use_dictionary=True, custom_dict={}, device="CPU", workdir=None)
 
- - На данный момент доступно 4 модели - **turbo**, **big_poetry**, **medium_poetry**, **small_poetry**
+ - На данный момент доступно 5 моделей - **turbo2**, **turbo**, **big_poetry**, **medium_poetry**, **small_poetry**
  - Переменная **use_dictionary** отвечает за загрузку всего словаря (требуется больше ОЗУ), иначе все ударения расставляет нейросеть. 
  - Функция **custom_dict** отвечает за добавление своих вариантов ударений в словарь. Формат такой: `{'слово': 'сл+ово с удар+ением'}`
 - Выбор устройства CPU или CUDA. **Для работы с CUDA требуется установить onnxruntime-gpu и CUDA.**
 - workdir - принимает строку. Является путём, куда скачиваются модели.
     
     **Для стабильной работы требуется минимум 3 гигабайта ОЗУ**
 ## Пример использования
 ```python
 from ruaccent import RUAccent
 
 accentizer = RUAccent()
-accentizer.load(omograph_model_size='turbo', use_dictionary=True)
+accentizer.load(omograph_model_size='turbo2', use_dictionary=True)
 
 text = 'на двери висит замок.'
 print(accentizer.process_all(text))
 ```
 
 Файлы моделей и словарей располагаются по [ссылке](https://huggingface.co/ruaccent/accentuator). Мы будем признательны фидбеку на [telegram аккаунт](https://t.me/chckdskeasfsd)
```

