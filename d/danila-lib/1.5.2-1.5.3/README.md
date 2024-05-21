# Comparing `tmp/danila-lib-1.5.2.tar.gz` & `tmp/danila-lib-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.5.2.tar", last modified: Tue May 21 12:50:03 2024, max compression
+gzip compressed data, was "danila-lib-1.5.3.tar", last modified: Tue May 21 14:57:26 2024, max compression
```

## Comparing `danila-lib-1.5.2.tar` & `danila-lib-1.5.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:50:03.658581 danila-lib-1.5.2/
--rw-rw-rw-   0        0        0     9615 2024-05-21 12:50:03.658581 danila-lib-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 12:50:03.411686 danila-lib-1.5.2/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.2/danila/__init__.py
--rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.5.2/danila/danila.py
--rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.2/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.2/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10717 2024-05-20 13:08:10.000000 danila-lib-1.5.2/danila/danila_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:50:03.446530 danila-lib-1.5.2/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-21 12:50:03.000000 danila-lib-1.5.2/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-05-21 12:50:03.000000 danila-lib-1.5.2/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:50:03.000000 danila-lib-1.5.2/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-21 12:50:03.000000 danila-lib-1.5.2/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 12:50:03.000000 danila-lib-1.5.2/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 12:50:03.447524 danila-lib-1.5.2/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.2/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:50:03.560023 danila-lib-1.5.2/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.2/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.2/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.2/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.2/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.5.2/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.2/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.2/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      830 2024-05-21 12:49:39.000000 danila-lib-1.5.2/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.2/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 09:06:42.000000 danila-lib-1.5.2/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:50:03.657585 danila-lib-1.5.2/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.2/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.2/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.2/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.2/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.2/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.2/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.2/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.2/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.2/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.2/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.2/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-21 12:50:03.667540 danila-lib-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-21 12:50:01.000000 danila-lib-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:57:26.127897 danila-lib-1.5.3/
+-rw-rw-rw-   0        0        0     9615 2024-05-21 14:57:26.127897 danila-lib-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:57:26.096040 danila-lib-1.5.3/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.3/danila/__init__.py
+-rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.5.3/danila/danila.py
+-rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.3/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.3/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10717 2024-05-20 13:08:10.000000 danila-lib-1.5.3/danila/danila_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:57:26.114956 danila-lib-1.5.3/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-21 14:57:26.000000 danila-lib-1.5.3/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-05-21 14:57:26.000000 danila-lib-1.5.3/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:57:26.000000 danila-lib-1.5.3/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-21 14:57:26.000000 danila-lib-1.5.3/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 14:57:26.000000 danila-lib-1.5.3/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:57:26.114956 danila-lib-1.5.3/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:57:26.120929 danila-lib-1.5.3/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.3/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.3/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.3/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.3/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.5.3/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.3/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.3/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-21 14:57:11.000000 danila-lib-1.5.3/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.3/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4390 2024-05-21 14:55:03.000000 danila-lib-1.5.3/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:57:26.126901 danila-lib-1.5.3/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.3/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.3/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.3/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.3/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.3/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.3/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.3/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.3/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.3/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.3/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.3/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:57:26.131881 danila-lib-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-21 14:57:23.000000 danila-lib-1.5.3/setup.py
```

### Comparing `danila-lib-1.5.2/PKG-INFO` & `danila-lib-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.5.2
+Version: 1.5.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.5.2/README.md` & `danila-lib-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/danila/danila.py` & `danila-lib-1.5.3/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/danila/danila_v1.py` & `danila-lib-1.5.3/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/danila/danila_v2.py` & `danila-lib-1.5.3/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/danila/danila_v3.py` & `danila-lib-1.5.3/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.5.3/danila_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.5.2
+Version: 1.5.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.5.2/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.5.3/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/danila_lib.egg-info/requires.txt` & `danila-lib-1.5.3/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/Letters_recognize.py` & `danila-lib-1.5.3/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/Rama_classify_class.py` & `danila-lib-1.5.3/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/Rama_detect_class.py` & `danila-lib-1.5.3/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.5.3/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/Text_detect_class.py` & `danila-lib-1.5.3/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/letters_in_image.py` & `danila-lib-1.5.3/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/models.py` & `danila-lib-1.5.3/data/neuro/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,9 +2,9 @@
 RAMA_NO_SPRING_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/sE5iSXYWL3xEkQ'
 RAMA_SPRING_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/zAEw0_ALgtBg9Q'
 RAMA_SPRING_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/b4vCbEzg3t3mTg'
 RAMA_NO_SPRING_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/N3zsrlwDP5yeRg'
 LETTERS_RECOGNIZE = 'https://disk.yandex.ru/d/ooaMrpqxl_egoA'
 RAMA_NO_SPRING_RUZHIMMASH_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/b4vCbEzg3t3mTg'
 RAMA_SPRING_BEJICKAYA_TEXT_DETECT_MODEL_ADDRESS = 'https://disk.yandex.ru/d/N3zsrlwDP5yeRg'
-TEXT_RECOGNIZE_YOLO_MODEL_ADDRESS = 'https://disk.yandex.ru/d/HN5Cs2zffXipIg'
+TEXT_RECOGNIZE_YOLO_MODEL_ADDRESS = 'https://disk.yandex.ru/d/4gyOsWUOsa_XhA'
 RAMA_PROD_CLASSIFY_MODEL_ADDRESS = 'https://disk.yandex.ru/d/iV7PHQcN-c2G-Q'
```

### Comparing `danila-lib-1.5.2/data/neuro/objs_in_image.py` & `danila-lib-1.5.3/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/neuro/text_recognize_yolo.py` & `danila-lib-1.5.3/data/neuro/text_recognize_yolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         # print(download_response.content)
         with open(zip_path, 'wb') as f:
             f.write(download_response.content)
 
         with zipfile.ZipFile(zip_path, 'r') as zip_ref:
             zip_ref.extractall()
         # weights_file_path = model_name + '_weights.pt'
-        self.model = torch.hub.load(yolo_path, 'custom', 'best.pt', source='local')
+        self.model = torch.hub.load(yolo_path, 'custom', 'text_recognize_yolo.pt', source='local')
 
         # for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string
 
     def work_image_cuts(self, number_image_cuts, l, h, w):
         """for every text_class try to recognize text from all areas of text_class, length is depends on class and prod, returns string """
         str = ''
         for number_image_cut in number_image_cuts:
```

### Comparing `danila-lib-1.5.2/data/result/Image_text_areas.py` & `danila-lib-1.5.3/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/result/Rect.py` & `danila-lib-1.5.3/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/result/Text_area.py` & `danila-lib-1.5.3/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/data/result/Yolo_label_rect.py` & `danila-lib-1.5.3/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.2/setup.py` & `danila-lib-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.5.2',
+  version='1.5.3',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

