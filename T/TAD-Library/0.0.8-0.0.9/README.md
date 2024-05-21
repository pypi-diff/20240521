# Comparing `tmp/TAD_Library-0.0.8.tar.gz` & `tmp/TAD_Library-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TAD_Library-0.0.8.tar", last modified: Tue Nov 28 01:55:26 2023, max compression
+gzip compressed data, was "TAD_Library-0.0.9.tar", last modified: Tue Nov 28 03:04:12 2023, max compression
```

## Comparing `TAD_Library-0.0.8.tar` & `TAD_Library-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-11-28 01:55:26.380258 TAD_Library-0.0.8/
--rw-rw-rw-   0        0        0        0 2022-02-15 02:46:55.000000 TAD_Library-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       34 2022-02-15 02:49:51.000000 TAD_Library-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      307 2023-11-28 01:55:26.380258 TAD_Library-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-11-08 06:33:51.000000 TAD_Library-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-28 01:55:26.362306 TAD_Library-0.0.8/TAD_Library/
--rw-rw-rw-   0        0        0     4598 2023-11-28 01:28:19.000000 TAD_Library-0.0.8/TAD_Library/Common.py
--rw-rw-rw-   0        0        0      487 2023-11-28 01:54:56.000000 TAD_Library-0.0.8/TAD_Library/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-28 01:55:26.378263 TAD_Library-0.0.8/TAD_Library.egg-info/
--rw-rw-rw-   0        0        0      307 2023-11-28 01:55:26.000000 TAD_Library-0.0.8/TAD_Library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-11-28 01:55:26.000000 TAD_Library-0.0.8/TAD_Library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-28 01:55:26.000000 TAD_Library-0.0.8/TAD_Library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-11-28 01:55:26.000000 TAD_Library-0.0.8/TAD_Library.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-11-28 01:55:26.000000 TAD_Library-0.0.8/TAD_Library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-11-28 01:55:26.386242 TAD_Library-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1038 2023-11-28 01:55:08.000000 TAD_Library-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-28 03:04:12.455312 TAD_Library-0.0.9/
+-rw-rw-rw-   0        0        0        0 2022-02-15 02:46:55.000000 TAD_Library-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-02-15 02:49:51.000000 TAD_Library-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      307 2023-11-28 03:04:12.454315 TAD_Library-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2023-11-08 06:33:51.000000 TAD_Library-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-28 03:04:12.427387 TAD_Library-0.0.9/TAD_Library/
+-rw-rw-rw-   0        0        0     4837 2023-11-28 03:01:13.000000 TAD_Library-0.0.9/TAD_Library/Common.py
+-rw-rw-rw-   0        0        0      487 2023-11-28 03:03:18.000000 TAD_Library-0.0.9/TAD_Library/__init__.py
+drwxrwxrwx   0        0        0        0 2023-11-28 03:04:12.453318 TAD_Library-0.0.9/TAD_Library.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-11-28 03:04:12.000000 TAD_Library-0.0.9/TAD_Library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-11-28 03:04:12.000000 TAD_Library-0.0.9/TAD_Library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-28 03:04:12.000000 TAD_Library-0.0.9/TAD_Library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-11-28 03:04:12.000000 TAD_Library-0.0.9/TAD_Library.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-11-28 03:04:12.000000 TAD_Library-0.0.9/TAD_Library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-11-28 03:04:12.461296 TAD_Library-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-11-28 03:03:26.000000 TAD_Library-0.0.9/setup.py
```

### Comparing `TAD_Library-0.0.8/TAD_Library/Common.py` & `TAD_Library-0.0.9/TAD_Library/Common.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,18 +185,30 @@
    """
    global client_socket
 
    data = bytearray([0x11, 0x02, 0x08])
 
    return TM_SendCmd(data)
 
-def TM_CurrMeasurementGet(unit_value):
+def TM_CurrMeasurementGet():
    """
        미세 전류 측정 값 읽기 함수 입니다.
 
        :returns : Measurment Value
    """
    global client_socket
 
-   data = bytearray([0x11, 0x02, 0x09, unit_value])
+   data = bytearray([0x11, 0x02, 0x09])
 
-   return TM_SendCmd(data)
+   return TM_SendCmd(data)
+
+def TM_CurrSetUnit(unit_value):
+    """
+       미세 전류 단위 설정 함수 입니다.
+
+       :returns : Pass (1) / Fail (0)
+    """
+    global client_socket
+
+    data = bytearray([0x11, 0x02, 0x0A, unit_value])
+
+    return TM_SendCmd(data)
```

### Comparing `TAD_Library-0.0.8/setup.py` & `TAD_Library-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='TAD_Library',# 프로젝트 명을 입력합니다.
-      version='0.0.8',      # 프로젝트 버전을 입력합니다.
+      version='0.0.9',      # 프로젝트 버전을 입력합니다.
       url='',      # 홈페이지 주소를 입력합니다.
       author='CHAKOON',      # 프로젝트 담당자 혹은 작성자를 입력합니다.
       author_email='yhkim@chakoon.com',      # 프로젝트 담당자 혹은 작성자의 이메일 주소를 입력합니다.
       description='TAD TT API',      # 프로젝트에 대한 간단한 설명을 입력합니다.
       packages=setuptools.find_packages(),      # 기본 프로젝트 폴더 외에 추가로 입력할 폴더를 입력합니다.
       long_description=open('README.md').read(),      # 프로젝트에 대한 설명을 입력합니다. 보통 README.md로 관리합니다.
       zip_safe=False,
```

