# Comparing `tmp/widget_periodictable-4.1.1.tar.gz` & `tmp/widget_periodictable-4.1.2.tar.gz`

## Comparing `widget_periodictable-4.1.1.tar` & `widget_periodictable-4.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/__init__.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/utils.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/static/widget.css
--rw-r--r--   0        0        0   113467 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/src/widget_periodictable/static/widget.js
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/.gitignore
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/README.md
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 widget_periodictable-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/src/widget_periodictable/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/src/widget_periodictable/utils.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/src/widget_periodictable/static/widget.css
+-rw-r--r--   0        0        0   113467 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/src/widget_periodictable/static/widget.js
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/.gitignore
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/README.md
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 widget_periodictable-4.1.2/PKG-INFO
```

### Comparing `widget_periodictable-4.1.1/src/widget_periodictable/__init__.py` & `widget_periodictable-4.1.2/src/widget_periodictable/__init__.py`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.1/src/widget_periodictable/utils.py` & `widget_periodictable-4.1.2/src/widget_periodictable/utils.py`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.1/src/widget_periodictable/static/widget.css` & `widget_periodictable-4.1.2/src/widget_periodictable/static/widget.css`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.1/src/widget_periodictable/static/widget.js` & `widget_periodictable-4.1.2/src/widget_periodictable/static/widget.js`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.1/LICENSE.txt` & `widget_periodictable-4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.1/README.md` & `widget_periodictable-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `widget_periodictable-4.1.1/pyproject.toml` & `widget_periodictable-4.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "widget-periodictable"
 description = 'A jupyter widget of the periodic table of elements.'
-version = "4.1.1"
+version = "4.1.2"
 dependencies = ["anywidget~=0.9.10"]
 authors = [{ name = "The OSSCAR team" }]
 readme = "README.md"
 keywords = [
   'jupyter',
   'jupyterlab',
   'widget',
   'anywidget',
   'osscar',
   'mendeleev',
 ]
 classifiers = [
   'Development Status :: 5 - Production/Stable',
+  'Framework :: Jupyter',
+  'Framework :: Jupyter :: JupyterLab',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Topic :: Scientific/Engineering',
 ]
 license = { file = 'LICENSE.txt' }
@@ -51,15 +53,15 @@
 dependencies = ["hatch-jupyter-builder>=0.5.0"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 npm = "npm"
 build_cmd = "build"
 
 [tool.bumpver]
-current_version = "v4.1.1"
+current_version = "v4.1.2"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `widget_periodictable-4.1.1/PKG-INFO` & `widget_periodictable-4.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: widget-periodictable
-Version: 4.1.1
+Version: 4.1.2
 Summary: A jupyter widget of the periodic table of elements.
 Project-URL: Home, https://www.osscar.org/
 Project-URL: Source, https://github.com/osscar-org/widget-periodictable
 Author: The OSSCAR team
 License: BSD 3-Clause License
         
         Copyright (c) 2024, OSSCAR (Open Software Services for Classrooms and Research)
@@ -33,14 +33,16 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE.txt
 Keywords: anywidget,jupyter,jupyterlab,mendeleev,osscar,widget
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Requires-Dist: anywidget~=0.9.10
```

