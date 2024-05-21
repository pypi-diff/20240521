# Comparing `tmp/nextflow-23.4.3.tar.gz` & `tmp/nextflow-23.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextflow-23.4.3.tar", last modified: Wed Aug 16 06:44:04 2023, max compression
+gzip compressed data, was "nextflow-23.4.4.tar", last modified: Tue Sep 26 04:23:31 2023, max compression
```

## Comparing `nextflow-23.4.3.tar` & `nextflow-23.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-08-16 06:44:04.190284 nextflow-23.4.3/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1378 2023-08-16 06:44:04.190284 nextflow-23.4.3/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-23.4.3/README.md
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-08-16 06:44:04.190284 nextflow-23.4.3/launcher/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14760 2023-08-16 06:44:03.000000 nextflow-23.4.3/launcher/nextflow
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-08-16 06:44:04.190284 nextflow-23.4.3/nextflow.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1378 2023-08-16 06:44:04.000000 nextflow-23.4.3/nextflow.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2023-08-16 06:44:04.000000 nextflow-23.4.3/nextflow.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-08-16 06:44:04.000000 nextflow-23.4.3/nextflow.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-08-16 06:44:04.000000 nextflow-23.4.3/nextflow.egg-info/top_level.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-08-16 06:44:04.190284 nextflow-23.4.3/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      805 2023-08-16 06:42:59.000000 nextflow-23.4.3/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-09-26 04:23:31.633639 nextflow-23.4.4/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1378 2023-09-26 04:23:31.633639 nextflow-23.4.4/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      877 2023-01-24 06:27:33.000000 nextflow-23.4.4/README.md
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-09-26 04:23:31.633639 nextflow-23.4.4/launcher/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14760 2023-09-26 04:23:31.000000 nextflow-23.4.4/launcher/nextflow
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-09-26 04:23:31.633639 nextflow-23.4.4/nextflow.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1378 2023-09-26 04:23:31.000000 nextflow-23.4.4/nextflow.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      164 2023-09-26 04:23:31.000000 nextflow-23.4.4/nextflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-09-26 04:23:31.000000 nextflow-23.4.4/nextflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-09-26 04:23:31.000000 nextflow-23.4.4/nextflow.egg-info/top_level.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       38 2023-09-26 04:23:31.633639 nextflow-23.4.4/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      805 2023-09-26 04:22:29.000000 nextflow-23.4.4/setup.py
```

### Comparing `nextflow-23.4.3/PKG-INFO` & `nextflow-23.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 23.4.3
+Version: 23.4.4
 Summary: A Python wrapper that installs the Nextflow launcher
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: pipeline,workflow,nextflow
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nextflow-23.4.3/README.md` & `nextflow-23.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nextflow-23.4.3/launcher/nextflow` & `nextflow-23.4.4/launcher/nextflow`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [[ "$NXF_DEBUG" == 'x' ]] && set -x
-NXF_VER=${NXF_VER:-'23.04.3'}
+NXF_VER=${NXF_VER:-'23.04.4'}
 NXF_ORG=${NXF_ORG:-'nextflow-io'}
 NXF_HOME=${NXF_HOME:-$HOME/.nextflow}
 NXF_PROT=${NXF_PROT:-'https'}
 NXF_BASE=${NXF_BASE:-$NXF_PROT://www.nextflow.io/releases}
 NXF_TEMP=${NXF_TEMP:-$TMPDIR}
 NXF_DIST=${NXF_DIST:-$NXF_HOME/framework}
 NXF_CLI="$0 $@"
```

### Comparing `nextflow-23.4.3/nextflow.egg-info/PKG-INFO` & `nextflow-23.4.4/nextflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextflow
-Version: 23.4.3
+Version: 23.4.4
 Summary: A Python wrapper that installs the Nextflow launcher
 Author: Jordi Deu-Pons
 License: Apache License 2.0
 Keywords: pipeline,workflow,nextflow
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `nextflow-23.4.3/setup.py` & `nextflow-23.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = '23.04.3'
+__version__ = '23.04.4'
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
```

