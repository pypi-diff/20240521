# Comparing `tmp/dzidb-1.0.2.tar.gz` & `tmp/dzidb-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dzidb-1.0.2.tar", last modified: Tue May 21 08:05:51 2024, max compression
+gzip compressed data, was "dzidb-1.1.tar", last modified: Tue May 21 07:45:01 2024, max compression
```

## Comparing `dzidb-1.0.2.tar` & `dzidb-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 08:05:51.423312 dzidb-1.0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-20 06:49:44.000000 dzidb-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      208 2024-05-21 08:05:51.423312 dzidb-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       26 2024-05-20 06:49:44.000000 dzidb-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-21 08:05:51.421537 dzidb-1.0.2/dzidb.egg-info/
--rw-rw-rw-   0        0        0      208 2024-05-21 08:05:51.000000 dzidb-1.0.2/dzidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-21 08:05:51.000000 dzidb-1.0.2/dzidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 08:05:51.000000 dzidb-1.0.2/dzidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-21 08:05:51.000000 dzidb-1.0.2/dzidb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 08:05:51.000000 dzidb-1.0.2/dzidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3200 2024-05-21 08:00:03.000000 dzidb-1.0.2/dzidb.py
--rw-rw-rw-   0        0        0       85 2024-05-21 08:05:51.424340 dzidb-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      348 2024-05-21 08:05:25.000000 dzidb-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 07:45:01.650020 dzidb-1.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-20 06:49:44.000000 dzidb-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      206 2024-05-21 07:45:01.650020 dzidb-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2024-05-20 06:49:44.000000 dzidb-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-21 07:45:01.648025 dzidb-1.1/dzidb.egg-info/
+-rw-rw-rw-   0        0        0      206 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 07:45:01.000000 dzidb-1.1/dzidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3245 2024-05-21 07:23:52.000000 dzidb-1.1/dzidb.py
+-rw-rw-rw-   0        0        0       85 2024-05-21 07:45:01.651016 dzidb-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      346 2024-05-21 07:39:01.000000 dzidb-1.1/setup.py
```

### Comparing `dzidb-1.0.2/LICENSE.txt` & `dzidb-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dzidb-1.0.2/dzidb.py` & `dzidb-1.1/dzidb.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,24 +52,25 @@
         if isinstance(obj, bytes):
             return base64.b64encode(obj).decode()
         else:
             return str(obj)
 
     print(json.dumps(value, indent=4, ensure_ascii=False, default=_bytes_hook))
 
-commands = [
+# 定义一个字典来映射命令到函数
+commands = {
     dict(action=cmd_devices,
          command="devices",
          flags=[
              dict(args=['-l'],
                   action='store_true',
                   help='output one entry per line')
          ],
-         help="show connected iOS devices"),
-]
+         help="show connected iOS devices")
+}
 
 def main():
     parser = argparse.ArgumentParser(
         description='Custom adb-like tool.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     subparsers = parser.add_subparsers(dest='subparser')
     actions = {}
```

