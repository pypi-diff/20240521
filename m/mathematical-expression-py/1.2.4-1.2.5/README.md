# Comparing `tmp/mathematical-expression-py-1.2.4.tar.gz` & `tmp/mathematical_expression_py-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathematical-expression-py-1.2.4.tar", last modified: Wed Apr  3 10:24:33 2024, max compression
+gzip compressed data, was "mathematical_expression_py-1.2.5.tar", last modified: Tue May 21 03:29:49 2024, max compression
```

## Comparing `mathematical-expression-py-1.2.4.tar` & `mathematical_expression_py-1.2.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:33.206839 mathematical-expression-py-1.2.4/
--rw-rw-rw-   0        0        0    11558 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    26748 2024-04-03 10:24:33.191262 mathematical-expression-py-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    26111 2024-04-03 09:35:27.000000 mathematical-expression-py-1.2.4/README.md
--rw-rw-rw-   0        0        0      631 2024-04-03 09:44:48.000000 mathematical-expression-py-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 10:24:33.206839 mathematical-expression-py-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.503444 mathematical-expression-py-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.581616 mathematical-expression-py-1.2.4/src/mathematical_expression/
--rw-rw-rw-   0        0        0     2843 2024-04-03 08:43:37.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.581616 mathematical-expression-py-1.2.4/src/mathematical_expression/core/
--rw-rw-rw-   0        0        0       51 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.660077 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/
--rw-rw-rw-   0        0        0     1616 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/Calculation.py
--rw-rw-rw-   0        0        0      843 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/SharedCalculation.py
--rw-rw-rw-   0        0        0       45 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.722515 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/__init__.py
--rw-rw-rw-   0        0        0     3060 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation.py
--rw-rw-rw-   0        0        0     4326 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.722515 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/
--rw-rw-rw-   0        0        0     5468 2024-04-03 10:16:14.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/ExpressionFunction.py
--rw-rw-rw-   0        0        0     1254 2024-04-03 08:33:19.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/Function.py
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.753762 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/__init__.py
--rw-rw-rw-   0        0        0     1580 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation.py
--rw-rw-rw-   0        0        0     4374 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py
--rw-rw-rw-   0        0        0     4336 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py
--rw-rw-rw-   0        0        0     2202 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py
--rw-rw-rw-   0        0        0     6380 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py
--rw-rw-rw-   0        0        0     6315 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py
--rw-rw-rw-   0        0        0     8006 2024-04-03 10:23:22.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py
--rw-rw-rw-   0        0        0     3222 2024-04-03 08:45:17.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/numberCalculation.py
--rw-rw-rw-   0        0        0     6184 2024-01-08 06:09:44.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.769382 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/
--rw-rw-rw-   0        0        0     1525 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationBooleanResults.py
--rw-rw-rw-   0        0        0     2205 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationNumberResults.py
--rw-rw-rw-   0        0        0     1741 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationResults.py
--rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.769382 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/
--rw-rw-rw-   0        0        0     5177 2024-04-03 08:57:06.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/CalculationManagement.py
--rw-rw-rw-   0        0        0     5113 2024-04-03 09:44:48.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/ConstantRegion.py
--rw-rw-rw-   0        0        0      762 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:32.956866 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/
--rw-rw-rw-   0        0        0      510 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/AbnormalOperation.py
--rw-rw-rw-   0        0        0      443 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/ExtractException.py
--rw-rw-rw-   0        0        0      450 2024-04-03 08:23:31.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/UnsupportedOperationException.py
--rw-rw-rw-   0        0        0      493 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/WrongFormat.py
--rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/exceptional/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:33.019359 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/
--rw-rw-rw-   0        0        0     5867 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/NumberUtils.py
--rw-rw-rw-   0        0        0     3123 2024-04-03 09:34:50.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/StrUtils.py
--rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical-expression-py-1.2.4/src/mathematical_expression/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:24:33.191262 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/
--rw-rw-rw-   0        0        0    26748 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2594 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-03 10:24:32.000000 mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.596694 mathematical_expression_py-1.2.5/
+-rw-rw-rw-   0        0        0    11558 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    26764 2024-05-21 03:29:49.594188 mathematical_expression_py-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    26127 2024-05-21 03:07:14.000000 mathematical_expression_py-1.2.5/README.md
+-rw-rw-rw-   0        0        0      631 2024-05-21 03:28:16.000000 mathematical_expression_py-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 03:29:49.596694 mathematical_expression_py-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:48.868843 mathematical_expression_py-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:48.933925 mathematical_expression_py-1.2.5/src/mathematical_expression/
+-rw-rw-rw-   0        0        0     2843 2024-04-03 08:43:37.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:48.939941 mathematical_expression_py-1.2.5/src/mathematical_expression/core/
+-rw-rw-rw-   0        0        0       51 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.000459 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/
+-rw-rw-rw-   0        0        0     1616 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/Calculation.py
+-rw-rw-rw-   0        0        0      843 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/SharedCalculation.py
+-rw-rw-rw-   0        0        0       45 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.070414 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/bool/
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/bool/__init__.py
+-rw-rw-rw-   0        0        0     3060 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/bool/booleanCalculation.py
+-rw-rw-rw-   0        0        0     4326 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.091303 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/function/
+-rw-rw-rw-   0        0        0     5468 2024-04-03 10:16:14.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/function/ExpressionFunction.py
+-rw-rw-rw-   0        0        0     1254 2024-04-03 08:33:19.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/function/Function.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/function/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.120368 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/__init__.py
+-rw-rw-rw-   0        0        0     1580 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/bracketsCalculation.py
+-rw-rw-rw-   0        0        0     4374 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py
+-rw-rw-rw-   0        0        0     4336 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py
+-rw-rw-rw-   0        0        0     2202 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py
+-rw-rw-rw-   0        0        0     6380 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py
+-rw-rw-rw-   0        0        0     6315 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py
+-rw-rw-rw-   0        0        0     8006 2024-04-03 10:23:22.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py
+-rw-rw-rw-   0        0        0     3222 2024-04-03 08:45:17.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/numberCalculation.py
+-rw-rw-rw-   0        0        0     6216 2024-05-13 02:48:02.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.129963 mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/
+-rw-rw-rw-   0        0        0     1525 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/CalculationBooleanResults.py
+-rw-rw-rw-   0        0        0     2205 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/CalculationNumberResults.py
+-rw-rw-rw-   0        0        0     1741 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/CalculationResults.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.140275 mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/
+-rw-rw-rw-   0        0        0     5177 2024-04-03 08:57:06.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/CalculationManagement.py
+-rw-rw-rw-   0        0        0     5185 2024-05-21 03:17:35.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/ConstantRegion.py
+-rw-rw-rw-   0        0        0      762 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.370267 mathematical_expression_py-1.2.5/src/mathematical_expression/exceptional/
+-rw-rw-rw-   0        0        0      510 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/exceptional/AbnormalOperation.py
+-rw-rw-rw-   0        0        0      443 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/exceptional/ExtractException.py
+-rw-rw-rw-   0        0        0      450 2024-04-03 08:23:31.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/exceptional/UnsupportedOperationException.py
+-rw-rw-rw-   0        0        0      493 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/exceptional/WrongFormat.py
+-rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/exceptional/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.415104 mathematical_expression_py-1.2.5/src/mathematical_expression/utils/
+-rw-rw-rw-   0        0        0     6127 2024-05-13 03:15:30.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/utils/NumberUtils.py
+-rw-rw-rw-   0        0        0     3123 2024-04-03 09:34:50.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/utils/StrUtils.py
+-rw-rw-rw-   0        0        0      168 2023-11-02 09:26:47.000000 mathematical_expression_py-1.2.5/src/mathematical_expression/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:29:49.586351 mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/
+-rw-rw-rw-   0        0        0    26764 2024-05-21 03:29:48.000000 mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2594 2024-05-21 03:29:48.000000 mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 03:29:48.000000 mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-21 03:29:48.000000 mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/top_level.txt
```

### Comparing `mathematical-expression-py-1.2.4/LICENSE` & `mathematical_expression_py-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/PKG-INFO` & `mathematical_expression_py-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathematical-expression-py
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python API concise framework for parsing string mathematical expressions
 Author-email: BeardedManZhao <liming7887@qq.com>
 Project-URL: Homepage, https://github.com/BeardedManZhao/mathematical-expression-py
 Project-URL: Bug Tracker, https://github.com/BeardedManZhao/mathematical-expression-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -191,15 +191,15 @@
   This component is designed for a mathematical expression without parentheses, but with operations such as addition,
   subtraction, multiplication, division and remainder. This component can realize the function with priority
   calculation, in which the prefix expression is used to parse and calculate, and the operand and operator are stored on
   the stack together with the calculation priority comparison If the current priority is low, first operate the previous
   operand and operator with the current operand to form a new value, and then put it on the stack.
 - API Usage Example
 
-  The operators supported by this component are： a+b a-b a*b a/b a%b
+  The operators supported by this component are： `a+b` `a-b` `a*b` `a/b` `a%b` `a^b`
 
 ```python
 # This is a sample Python script.
 from mathematical_expression.core.calculation.number import prefixExpressionOperation
 from mathematical_expression.core.calculation.number.prefixExpressionOperation import PrefixExpressionOperation
 from mathematical_expression.core.container.CalculationNumberResults import CalculationNumberResults
```

### Comparing `mathematical-expression-py-1.2.4/README.md` & `mathematical_expression_py-1.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
   This component is designed for a mathematical expression without parentheses, but with operations such as addition,
   subtraction, multiplication, division and remainder. This component can realize the function with priority
   calculation, in which the prefix expression is used to parse and calculate, and the operand and operator are stored on
   the stack together with the calculation priority comparison If the current priority is low, first operate the previous
   operand and operator with the current operand to form a new value, and then put it on the stack.
 - API Usage Example
 
-  The operators supported by this component are： a+b a-b a*b a/b a%b
+  The operators supported by this component are： `a+b` `a-b` `a*b` `a/b` `a%b` `a^b`
 
 ```python
 # This is a sample Python script.
 from mathematical_expression.core.calculation.number import prefixExpressionOperation
 from mathematical_expression.core.calculation.number.prefixExpressionOperation import PrefixExpressionOperation
 from mathematical_expression.core.container.CalculationNumberResults import CalculationNumberResults
```

### Comparing `mathematical-expression-py-1.2.4/pyproject.toml` & `mathematical_expression_py-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mathematical-expression-py"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
     { name = "BeardedManZhao", email = "liming7887@qq.com" },
 ]
 description = "Python API concise framework for parsing string mathematical expressions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/__init__.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/Calculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/Calculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/SharedCalculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/SharedCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/bool/booleanCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/bool/booleanCalculation2.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/ExpressionFunction.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/function/ExpressionFunction.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/function/Function.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/function/Function.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/bracketsCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/bracketsCalculation2.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/cumulativeCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/fastMultiplyOfIntervalsBrackets.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/fastSumOfIntervalsBrackets.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/functionFormulaCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/functionFormulaCalculation2.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/numberCalculation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/numberCalculation.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/calculation/number/prefixExpressionOperation.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         temp: str = ConstantRegion.NO_CHAR
         # 创建标记点 标记上一个是否是操作符
         back_is_opt = True
         # 迭代表达式中的每一个字符
         for c in new_formula:
             if (not back_is_opt) and (c == ConstantRegion.PLUS_SIGN or c == ConstantRegion.MINUS_SIGN or
                                       c == ConstantRegion.MULTIPLICATION_SIGN or c == ConstantRegion.DIVISION_SIGN or
-                                      c == ConstantRegion.REMAINDER_SIGN):
+                                      c == ConstantRegion.REMAINDER_SIGN or c == ConstantRegion.POW_SIGN):
                 length: int = len(str_stack)
                 back_is_opt = True
                 # 如果上一个不是运算符，且当前是运算符，就将上一个字符串缓冲转换成为数值，稍后用于栈的添加
                 number: float = StrUtils.string_to_double(temp)
                 # 清理所有缓冲区字符
                 temp = ConstantRegion.NO_CHAR
                 if length == 0:
```

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationBooleanResults.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/CalculationBooleanResults.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationNumberResults.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/CalculationNumberResults.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/container/CalculationResults.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/container/CalculationResults.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/CalculationManagement.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/CalculationManagement.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/ConstantRegion.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/ConstantRegion.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @File : ConstantRegion.py
 # @Project : mathematical-expression-py
 # 这里是框架的常量数据池，不建议更改，如果更改了的话，很可能造成运行混乱
 # 如果针对具有固定格式要求的数学公式需要对此处的参数进行配置，请在修改之后进行re_fresh函数的调用
 import logging
 from typing import List
 
-VERSION: float = 1.24
+VERSION: float = 1.25
 STRING_NULL: str = "null"
 LEFT_BRACKET: str = '('
 RIGHT_BRACKET: str = ')'
 DECIMAL_POINT: str = '.'
 EMPTY: str = ' '
 NO_CHAR: str = ''
 COMMA = ','
@@ -22,14 +22,15 @@
 SA_ASCII: int = 0b1100001
 SZ_ASCII: int = 0b1111010
 PLUS_SIGN: str = '+'
 MINUS_SIGN: str = '-'
 MULTIPLICATION_SIGN: str = '*'
 DIVISION_SIGN: str = '/'
 REMAINDER_SIGN: str = '%'
+POW_SIGN = '^'
 GREATER_THAN_SIGN: str = ">"
 LESS_THAN_SIGN: str = "<"
 EQUAL_SIGN1: str = "="
 EQUAL_SIGN2: str = EQUAL_SIGN1 + EQUAL_SIGN1
 NEGATE_SIGN: str = "!"
 NOT_EQUAL_SIGN1: str = NEGATE_SIGN + EQUAL_SIGN1
 NOT_EQUAL_SIGN2: str = LESS_THAN_SIGN + GREATER_THAN_SIGN
@@ -51,45 +52,47 @@
 LOG_INFO_UNREGISTER_FUNCTION: str = "Prepare the logoff of a function. Function name:"
 LOG_INFO_SHARED_POOL: str = "Use shared pool data. The identity of the data is: "
 # python特有的常量数据
 LOG_LEVEL: int = logging.INFO
 REGULAR_CONTAINS_ADDSUB: str = "\\+" + MINUS_SIGN + "|" + MINUS_SIGN + "\\+" \
     if PLUS_SIGN == '+' else \
     PLUS_SIGN + MINUS_SIGN + '|' + MINUS_SIGN + PLUS_SIGN
-ARITHMETIC_OPERATOR_STRING: str = PLUS_SIGN.join([MINUS_SIGN, MULTIPLICATION_SIGN, DIVISION_SIGN, REMAINDER_SIGN])
+ARITHMETIC_OPERATOR_STRING: str = PLUS_SIGN.join(
+    [MINUS_SIGN, MULTIPLICATION_SIGN, DIVISION_SIGN, REMAINDER_SIGN, POW_SIGN])
 
 NUMBER_SET: List[str] = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', RIGHT_BRACKET]
 
 LEGAL_CHARACTERS: set = {'0', '1', '2', '3', '4', '5', '6', '7', '8', '9',
                          EMPTY, PLUS_SIGN, MINUS_SIGN,
                          MULTIPLICATION_SIGN, DIVISION_SIGN,
-                         REMAINDER_SIGN,
+                         REMAINDER_SIGN, POW_SIGN,
                          LEFT_BRACKET, RIGHT_BRACKET, DECIMAL_POINT}
 
 
 def re_fresh():
     """
     刷新常量配置
     """
     global REGULAR_CONTAINS_ADDSUB, ARITHMETIC_OPERATOR_STRING, EQUAL_SIGN2, NOT_EQUAL_SIGN1, NOT_EQUAL_SIGN2
     global GREATER_THAN_OR_EQUAL_TO_SIGN, LESS_THAN_OR_EQUAL_TO_SIGN
     global REGULAR_COMPARISON_OPERATOR, LEGAL_CHARACTERS
     REGULAR_CONTAINS_ADDSUB = "\\+" + MINUS_SIGN + "|" + MINUS_SIGN + "\\+" \
         if PLUS_SIGN == '+' else \
         PLUS_SIGN + MINUS_SIGN + '|' + MINUS_SIGN + PLUS_SIGN
-    ARITHMETIC_OPERATOR_STRING = PLUS_SIGN.join([MINUS_SIGN, MULTIPLICATION_SIGN, DIVISION_SIGN, REMAINDER_SIGN])
+    ARITHMETIC_OPERATOR_STRING = PLUS_SIGN.join(
+        [MINUS_SIGN, MULTIPLICATION_SIGN, DIVISION_SIGN, REMAINDER_SIGN, POW_SIGN])
     EQUAL_SIGN2 = EQUAL_SIGN1 + EQUAL_SIGN1
     NOT_EQUAL_SIGN1 = NEGATE_SIGN + EQUAL_SIGN1
     NOT_EQUAL_SIGN2 = LESS_THAN_SIGN + GREATER_THAN_SIGN
     GREATER_THAN_OR_EQUAL_TO_SIGN = GREATER_THAN_SIGN + EQUAL_SIGN1
     LESS_THAN_OR_EQUAL_TO_SIGN = LESS_THAN_SIGN + EQUAL_SIGN1
     REGULAR_COMPARISON_OPERATOR = "{0}|{1}|{2}|{3}|{4}|[{5}{6}{7}]".format(LESS_THAN_OR_EQUAL_TO_SIGN,
                                                                            GREATER_THAN_OR_EQUAL_TO_SIGN,
                                                                            NOT_EQUAL_SIGN1, NOT_EQUAL_SIGN2,
                                                                            EQUAL_SIGN2, LESS_THAN_SIGN,
                                                                            EQUAL_SIGN1,
                                                                            GREATER_THAN_SIGN)
     LEGAL_CHARACTERS = {'0', '1', '2', '3', '4', '5', '6', '7', '8', '9',
                         EMPTY, PLUS_SIGN, MINUS_SIGN,
                         MULTIPLICATION_SIGN, DIVISION_SIGN,
-                        REMAINDER_SIGN,
+                        REMAINDER_SIGN, POW_SIGN,
                         LEFT_BRACKET, RIGHT_BRACKET, DECIMAL_POINT}
```

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/core/manager/__init__.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/core/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression/utils/StrUtils.py` & `mathematical_expression_py-1.2.5/src/mathematical_expression/utils/StrUtils.py`

 * *Files identical despite different names*

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/PKG-INFO` & `mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathematical-expression-py
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python API concise framework for parsing string mathematical expressions
 Author-email: BeardedManZhao <liming7887@qq.com>
 Project-URL: Homepage, https://github.com/BeardedManZhao/mathematical-expression-py
 Project-URL: Bug Tracker, https://github.com/BeardedManZhao/mathematical-expression-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -191,15 +191,15 @@
   This component is designed for a mathematical expression without parentheses, but with operations such as addition,
   subtraction, multiplication, division and remainder. This component can realize the function with priority
   calculation, in which the prefix expression is used to parse and calculate, and the operand and operator are stored on
   the stack together with the calculation priority comparison If the current priority is low, first operate the previous
   operand and operator with the current operand to form a new value, and then put it on the stack.
 - API Usage Example
 
-  The operators supported by this component are： a+b a-b a*b a/b a%b
+  The operators supported by this component are： `a+b` `a-b` `a*b` `a/b` `a%b` `a^b`
 
 ```python
 # This is a sample Python script.
 from mathematical_expression.core.calculation.number import prefixExpressionOperation
 from mathematical_expression.core.calculation.number.prefixExpressionOperation import PrefixExpressionOperation
 from mathematical_expression.core.container.CalculationNumberResults import CalculationNumberResults
```

### Comparing `mathematical-expression-py-1.2.4/src/mathematical_expression_py.egg-info/SOURCES.txt` & `mathematical_expression_py-1.2.5/src/mathematical_expression_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

