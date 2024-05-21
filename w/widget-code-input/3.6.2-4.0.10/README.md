# Comparing `tmp/widget_code_input-3.6.2.tar.gz` & `tmp/widget_code_input-4.0.10.tar.gz`

## Comparing `widget_code_input-3.6.2.tar` & `widget_code_input-4.0.10.tar`

### file list

```diff
@@ -1,81 +1,10 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.prettierrc
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/babel.config.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/codecov.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/install.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/jest.config.js
--rw-r--r--   0        0        0   511804 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/package-lock.json
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/package.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/tsconfig.json
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/webpack.config.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input.json
--rw-r--r--   0        0        0   320441 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/yarn.lock
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/binder/environment.yml
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/binder/postBuild
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/eclipse.css
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/idea.css
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/material.css
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/midnight.css
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/monokai.css
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/nord.css
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/solarized.css
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/css/widget.css
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/Makefile
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/environment.yml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/make.bat
--rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/conf.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/develop-install.rst
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/index.rst
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/examples/introduction.ipynb
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/extension.ts
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/index.ts
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/plugin.ts
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/version.ts
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/widget.ts
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/_frontend.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/_version.py
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/utils.py
--rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/widget_code_input.py
--rw-r--r--   0        0        0    21478 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/build_log.json
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/package.json
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/lib_index_js.cfb07d945e63bf1241be.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/lib_index_js.cfb07d945e63bf1241be.js.map
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/lib_plugin_js.459fed25698cae2280d6.js
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/lib_plugin_js.459fed25698cae2280d6.js.map
--rw-r--r--   0        0        0    46792 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/lib_widget_js.d093be75398280f00c19.js
--rw-r--r--   0        0        0    49049 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/lib_widget_js.d093be75398280f00c19.js.map
--rw-r--r--   0        0        0    28453 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/remoteEntry.33261d86eee5e6a3f173.js
--rw-r--r--   0        0        0    27267 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/remoteEntry.33261d86eee5e6a3f173.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/style.js
--rw-r--r--   0        0        0   402126 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/vendors-node_modules_codemirror_lib_codemirror_js.bb6b46d7694642f92bea.js
--rw-r--r--   0        0        0   480036 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/vendors-node_modules_codemirror_lib_codemirror_js.bb6b46d7694642f92bea.js.map
--rw-r--r--   0        0        0   379899 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/vendors-node_modules_codemirror_mode_css_css_js-node_modules_codemirror_mode_javascript_javas-026992.b1598f2ebb8d1a1d158b.js
--rw-r--r--   0        0        0   247606 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/labextension/static/vendors-node_modules_codemirror_mode_css_css_js-node_modules_codemirror_mode_javascript_javas-026992.b1598f2ebb8d1a1d158b.js.map
--rw-r--r--   0        0        0   278947 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/nbextension/index.js
--rw-r--r--   0        0        0  1038195 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/tests/__init__.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/tests/conftest.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/tests/test_example.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/widget_code_input/tests/test_nbextension_path.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/.gitignore
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/LICENSE.txt
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/README.md
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/pyproject.toml
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 widget_code_input-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0   927450 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/src/widget_code_input/static/index.js
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/src/widget_code_input/static/styles.css
+-rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/widget_code_input/CodeInputWidget.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/widget_code_input/frontend.py
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/widget_code_input/utils.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/.gitignore
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/LICENSE.txt
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/pyproject.toml
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 widget_code_input-4.0.10/PKG-INFO
```

### Comparing `widget_code_input-3.6.2/widget_code_input/utils.py` & `widget_code_input-4.0.10/widget_code_input/utils.py`

 * *Files identical despite different names*

### Comparing `widget_code_input-3.6.2/widget_code_input/widget_code_input.py` & `widget_code_input-4.0.10/widget_code_input/CodeInputWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,164 +1,176 @@
-#!/usr/bin/env python
-# coding: utf-8
-
-# Copyright (c) Dou Du.
-# Distributed under the terms of the Modified BSD License.
-
-
+# hello_widget/__init__.py
 from __future__ import absolute_import
 from functools import wraps
-import ipywidgets as widgets 
-from ipywidgets import DOMWidget 
+import pathlib
+import anywidget
+import traitlets
+import os
 from traitlets import Unicode, validate, TraitError
-from ._frontend import module_name, module_version 
+from .frontend import module_name, module_version 
+
 from .utils import (
     CodeValidationError,
     build_function,
     build_signature,
     is_valid_variable_name,
     format_syntax_error_msg,
     format_generic_error_msg,
 )
 
 
-@widgets.register
-class WidgetCodeInput(DOMWidget):
-    """A widget to input code in a text box, validate it and run in in a sandboxed environment."""
-
-    _model_name = Unicode('WidgetCodeModel').tag(sync=True)
-    _model_module = Unicode(module_name).tag(sync=True)
-    _model_module_version = Unicode(module_version).tag(sync=True)
-    _view_name = Unicode('WidgetCodeView').tag(sync=True)
-    _view_module = Unicode(module_name).tag(sync=True)
-    _view_module_version = Unicode(module_version).tag(sync=True)
-    function_name = Unicode('example').tag(sync=True)
-    function_parameters = Unicode('').tag(sync=True)
-    docstring = Unicode('\n').tag(sync=True)
-    function_body = Unicode('').tag(sync=True)
-    code_theme = Unicode('').tag(sync=True)  
-
-    @validate('function_name')
-    def _valid_function_name(self, function_name):
-        """
-        Validate that the function name is a valid python variable name
-        """
-        if not is_valid_variable_name(function_name["value"]):
-            raise TraitError(
-                "Invalid variable name '{}'".format(function_name["value"])
-            )
-        return function_name["value"]
+bundler_output_dir = pathlib.Path(os.path.dirname(os.path.abspath(__file__))) / "./static"
+
 
-    @validate('function_parameters')
-    def _valid_function_parameters(self, function_parameters):
-        """
-        Validate that the function parameters do not contain newlines
-
-        These might allow string injection, and would be difficult to indent
-        properly.
-        """
-        if '\n' in function_parameters['value']:
-            raise TraitError("The function parameters cannot contain newlines")
-        return function_parameters['value']
-
-    @validate('docstring')
-    def _valid_docstring(self, docstring):
-        """
-        Validate that the docstring do not contain triple double quotes
-        """
-        if '"""' in docstring['value']:
-            raise TraitError('The docstring cannot contain triple double quotes (""")')
-        return docstring['value']
+class CodeInputWidget(anywidget.AnyWidget):
+        widget_instance_count=0 # counter to keep track of number of widget instances in use
+        
+        function_name = Unicode('example').tag(sync=True)
+        function_parameters = Unicode('').tag(sync=True)
+        docstring = Unicode('\n').tag(sync=True)
+        function_body = Unicode('').tag(sync=True)
+        code_theme = Unicode('').tag(sync=True)
+        widget_instance_count_trait = Unicode(f'').tag(sync=True)
+        
+
+        @validate('function_name')
+        def _valid_function_name(self, function_name):
+            """
+            Validate that the function name is a valid python variable name
+            """
+            if not is_valid_variable_name(function_name["value"]):
+                raise TraitError(
+                    "Invalid variable name '{}'".format(function_name["value"])
+                )
+            return function_name["value"]
+        
+        @validate('function_parameters')
+        def _valid_function_parameters(self, function_parameters):
+            """
+            Validate that the function parameters do not contain newlines
+
+            These might allow string injection, and would be difficult to indent
+            properly.
+            """
+            if '\n' in function_parameters['value']:
+                raise TraitError("The function parameters cannot contain newlines")
+            return function_parameters['value']
+           
+        @validate('docstring')
+        def _valid_docstring(self, docstring):
+            """
+            Validate that the docstring do not contain triple double quotes
+            """
+            if '"""' in docstring['value']:
+                raise TraitError('The docstring cannot contain triple double quotes (""")')
+            return docstring['value']
 
-    def __init__(  # pylint: disable=too-many-arguments
+
+
+        
+        def __init__(  # pylint: disable=too-many-arguments
         self,
         function_name,
         function_parameters="",
         docstring="\n",
         function_body="",
-        code_theme="nord",
+        code_theme="",
     ):
-        """
-        Creates a new widget to show a box to enter code.
+            """
+            Creates a new widget to show a box to enter code.
 
-        :param function_name: the name of the function
-        :param function_parameters: the parameters of the function (whatever
-            would be within brackets in the function signature line).
-            It MUST be on a single line.
-        :param docstring: the docstring of the function. It cannot contain
-            triple double quotes (").
-        :param function_body: the content of the function body.
-        :param code_theme: the code theme of the code input box.
-        """
-        super(WidgetCodeInput, self).__init__()
-        self.function_name = function_name
-        self.function_parameters = function_parameters
-        self.docstring = docstring
-        self.function_body = function_body
-        self.code_theme = code_theme
-    
-    @property
-    def full_function_code(self):
-        """
-        The full code of this function (with a default indentation of 4 spaces)
-        including signature, docstring and body
-        """
-        return build_function(
-            self.function_signature, self.docstring, self.function_body
-        )
-
-    @property
-    def function_signature(self):
-        """
-        The function signature (first line of the function, containing 'def')
-        """
-        return build_signature(self.function_name, self.function_parameters)
-
-    def get_function_object(self):
-        """
-        Return the compiled function object.
-
-        This can be assigned to a variable and then called, for instance::
-
-          func = widget.get_function_object() # This can raise a SyntaxError
-          retval = func(parameters)
-
-        :raise SyntaxError: if the function code has syntax errors (or if
-          the function name is not a valid identifier)
-        """
-        globals_dict = {
-            "__builtins__": globals()["__builtins__"],
-            "__name__": "__main__",
-            "__doc__": None,
-            "__package__": None,
-        }
-
-        if not is_valid_variable_name(self.function_name):
-            raise SyntaxError("Invalid function name '{}'".format(self.function_name))
-
-        # Optionally one could do a ast.parse here already, to check syntax before execution
-        try:
-            exec(
-                compile(self.full_function_code, __name__, "exec", dont_inherit=True),
-                globals_dict,
+            :param function_name: the name of the function
+            :param function_parameters: the parameters of the function (whatever
+                would be within brackets in the function signature line).
+                It MUST be on a single line.
+            :param docstring: the docstring of the function. It cannot contain
+                triple double quotes (").
+            :param function_body: the content of the function body.
+            :param code_theme: the code theme of the code input box.
+            """
+
+            super(CodeInputWidget, self).__init__()
+            
+            self.function_name = function_name
+            self.function_parameters = function_parameters
+            self.docstring = docstring
+            self.function_body = function_body
+            self.code_theme = code_theme
+            self.widget_instance_count_trait=f"{CodeInputWidget.widget_instance_count}"
+            CodeInputWidget.widget_instance_count+=1
+
+
+        _esm = bundler_output_dir / "index.js"
+        _css = bundler_output_dir / "styles.css"
+        name = traitlets.Unicode().tag(sync=True)
+
+        
+
+        
+        @property
+        def full_function_code(self):
+            """
+            The full code of this function (with a default indentation of 4 spaces)
+            including signature, docstring and body
+            """
+            return build_function(
+                self.function_signature, self.docstring, self.function_body
             )
-        except SyntaxError as exc:
-            raise CodeValidationError(
-                format_syntax_error_msg(exc), orig_exc=exc
-            ) from exc
-
-        function_object = globals_dict[self.function_name]
-
-        def catch_exceptions(func):
-            @wraps(func)
-            def wrapper(*args, **kwargs):
-                """Wrap and check exceptions to return a longer and clearer exception."""
-
-                try:
-                    return func(*args, **kwargs)
-                except Exception as exc:
-                    err_msg = format_generic_error_msg(exc, code_widget=self)
-                    raise CodeValidationError(err_msg, orig_exc=exc) from exc
 
-            return wrapper
+        @property
+        def function_signature(self):
+            """
+            The function signature (first line of the function, containing 'def')
+            """
+            return build_signature(self.function_name, self.function_parameters)
+
+        def get_function_object(self):
+            """
+            Return the compiled function object.
+
+            This can be assigned to a variable and then called, for instance::
+
+              func = widget.get_function_object() # This can raise a SyntaxError
+              retval = func(parameters)
+
+            :raise SyntaxError: if the function code has syntax errors (or if
+              the function name is not a valid identifier)
+            """
+            globals_dict = {
+                "__builtins__": globals()["__builtins__"],
+                "__name__": "__main__",
+                "__doc__": None,
+                "__package__": None,
+            }
+
+            if not is_valid_variable_name(self.function_name):
+                raise SyntaxError("Invalid function name '{}'".format(self.function_name))
+
+            # Optionally one could do a ast.parse here already, to check syntax before execution
+            try:
+                exec(
+                    compile(self.full_function_code, __name__, "exec", dont_inherit=True),
+                    globals_dict,
+                )
+            except SyntaxError as exc:
+                raise CodeValidationError(
+                    format_syntax_error_msg(exc), orig_exc=exc
+                ) from exc
+
+            function_object = globals_dict[self.function_name]
+
+            def catch_exceptions(func):
+                @wraps(func)
+                def wrapper(*args, **kwargs):
+                    """Wrap and check exceptions to return a longer and clearer exception."""
+
+                    try:
+                        return func(*args, **kwargs)
+                    except Exception as exc:
+                        err_msg = format_generic_error_msg(exc, code_widget=self)
+                        raise CodeValidationError(err_msg, orig_exc=exc) from exc
+
+                return wrapper
+
+            return catch_exceptions(function_object)
+
 
-        return catch_exceptions(function_object)
```

### Comparing `widget_code_input-3.6.2/LICENSE.txt` & `widget_code_input-4.0.10/LICENSE.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,11 @@
-Copyright (c) 2022 Dou Du and Giovanni Pizzi
-All rights reserved.
+Copyright (c) 2022 Dou Du and Giovanni Pizzi All rights reserved.
 
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
+Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
+Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
+Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `widget_code_input-3.6.2/README.md` & `widget_code_input-4.0.10/README.md`

 * *Files identical despite different names*

