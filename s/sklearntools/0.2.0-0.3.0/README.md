# Comparing `tmp/sklearntools-0.2.0.tar.gz` & `tmp/sklearntools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-0.2.0.tar", last modified: Tue May 21 10:29:57 2024, max compression
+gzip compressed data, was "sklearntools-0.3.0.tar", last modified: Tue May 21 10:55:39 2024, max compression
```

## Comparing `sklearntools-0.2.0.tar` & `sklearntools-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:57.751247 sklearntools-0.2.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:29:57.750534 sklearntools-0.2.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.2.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 10:29:57.751534 sklearntools-0.2.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 10:29:53.000000 sklearntools-0.2.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:57.744905 sklearntools-0.2.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     4883 2024-05-21 10:27:59.000000 sklearntools-0.2.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:29:57.749514 sklearntools-0.2.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:29:05.000000 sklearntools-0.2.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 10:29:57.000000 sklearntools-0.2.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:55:39.964308 sklearntools-0.3.0/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:55:39.963662 sklearntools-0.3.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.3.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 10:55:39.964582 sklearntools-0.3.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 10:55:30.000000 sklearntools-0.3.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:55:39.958923 sklearntools-0.3.0/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     5089 2024-05-21 10:52:41.000000 sklearntools-0.3.0/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:55:39.962786 sklearntools-0.3.0/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-0.2.0/PKG-INFO` & `sklearntools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

### Comparing `sklearntools-0.2.0/README.rst` & `sklearntools-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-0.2.0/setup.py` & `sklearntools-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
     description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.2.0',
+    version='0.3.0',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-0.2.0/sklearntools/__init__.py` & `sklearntools-0.3.0/sklearntools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from collections import Counter
 from joblib import Parallel, delayed
 from sklearn.metrics import accuracy_score
 from sklearn.model_selection import ParameterGrid
 from sklearn.model_selection import train_test_split
+from logging import basicConfig, INFO, getLogger
+
+logger = getLogger(__name__)
+basicConfig(level=INFO, format='[%(asctime)s %(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
 def train_evaluate(model, X_train, X_test, y_train, y_test, describe='准确率', return_predict=False):
 	"""Train and evaluate a model
 
 	Parameters
     ----------
@@ -34,19 +38,19 @@
     >>> train_evaluate(model, X_train, X_test, y_train, y_test)
     0.88
 	"""
 	model.fit(X_train, y_train)
 	if return_predict:
 		prediction = model.predict(X_test, y_test)
 		score = accuracy_score(y_test, prediction)
-		print(f'{describe}: {score:.1%}')
+		logger.info(f'{describe}: {score:.1%}')
 		return score, prediction
 	else:
 		score = model.score(X_test, y_test)
-		print(f'{describe}: {score:.1%}')
+		logger.info(f'{describe}: {score:.1%}')
 		return score
 
 
 def train_evaluate_split(model, X, y, test_size=0.2, describe='准确率', return_predict=False, random_state=42):
 	"""Train and evaluate a model
 
 	Parameters
@@ -101,15 +105,15 @@
 	>>> X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3)
 	>>> param_grid = {'n_estimators': np.arange(800, 820, 1), 'bootstrap': [False, True]}
 	>>> search_model_params(RandomForestClassifier, X_train, X_test, y_train, y_test, param_grid, result_num=3)
 	"""
 	results = Parallel(n_jobs=-1)(delayed(_search_params)(model_name, X_train, X_test, y_train, y_test, params) for params in ParameterGrid(param_grid))
 	results = sorted(results, key=lambda x: x[1], reverse=True)[:result_num]
 	for param, score in results:
-		print(f'param: {param}\t准确率: {score:.1%}')
+		logger.info(f'param: {param}\t准确率: {score:.1%}')
 		_evaluate_params(model_name, X_train, X_test, y_train, y_test, param, iter_num)
 
 
 def search_model_params_split(model_name, X, y, param_grid, test_size=0.2, result_num=5, iter_num=8, random_state=42):
 	"""Train and evaluate a model
 
 	Parameters
@@ -143,8 +147,8 @@
 	return params, score
 
 
 def _evaluate_params(model_name, X_train, X_test, y_train, y_test, param, iter_num):
 	results = Parallel(n_jobs=-1)(delayed(_search_params)(model_name, X_train, X_test, y_train, y_test, param) for _ in range(iter_num))
 	counter = Counter([result[1] for result in results])
 	for score, count in sorted(counter.items(), key=lambda x: x[0], reverse=True):
-		print(f'\tscore: {score}\tcount: {count}')
+		logger.info(f'\tscore: {score}\tcount: {count}')
```

### Comparing `sklearntools-0.2.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-0.3.0/sklearntools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

