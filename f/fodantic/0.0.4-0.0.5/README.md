# Comparing `tmp/fodantic-0.0.4.tar.gz` & `tmp/fodantic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fodantic-0.0.4.tar", last modified: Tue Apr  2 01:24:29 2024, max compression
+gzip compressed data, was "fodantic-0.0.5.tar", last modified: Mon May 20 22:03:01 2024, max compression
```

## Comparing `fodantic-0.0.4.tar` & `fodantic-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.524685 fodantic-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 01:24:21.000000 fodantic-0.0.4/MIT-LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-02 01:24:29.524685 fodantic-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-02 01:24:21.000000 fodantic-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 01:24:21.000000 fodantic-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:24:29.524685 fodantic-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.520684 fodantic-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.520684 fodantic-0.0.4/src/fodantic/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/form_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.524685 fodantic-0.0.4/src/fodantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:03:01.608338 fodantic-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 22:02:53.000000 fodantic-0.0.5/MIT-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-20 22:03:01.608338 fodantic-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-20 22:02:53.000000 fodantic-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-20 22:02:53.000000 fodantic-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:03:01.608338 fodantic-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:03:01.604338 fodantic-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:03:01.604338 fodantic-0.0.5/src/fodantic/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 22:02:53.000000 fodantic-0.0.5/src/fodantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-20 22:02:53.000000 fodantic-0.0.5/src/fodantic/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-20 22:02:53.000000 fodantic-0.0.5/src/fodantic/form_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-20 22:02:53.000000 fodantic-0.0.5/src/fodantic/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:03:01.608338 fodantic-0.0.5/src/fodantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-20 22:03:01.000000 fodantic-0.0.5/src/fodantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 22:03:01.000000 fodantic-0.0.5/src/fodantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:03:01.000000 fodantic-0.0.5/src/fodantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 22:03:01.000000 fodantic-0.0.5/src/fodantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 22:03:01.000000 fodantic-0.0.5/src/fodantic.egg-info/top_level.txt
```

### Comparing `fodantic-0.0.4/MIT-LICENSE` & `fodantic-0.0.5/MIT-LICENSE`

 * *Files identical despite different names*

### Comparing `fodantic-0.0.4/pyproject.toml` & `fodantic-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 
 
 [project]
 name = "fodantic"
-version = "0.0.4"
+version = "0.0.5"
 description = "Pydantic-based HTTP forms"
 authors = [
   {name = "Juan-Pablo Scaletti", email = "juanpablo@jpscaletti.com"},
 ]
 license = { "file" = "MIT-LICENSE" }
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `fodantic-0.0.4/src/fodantic/form.py` & `fodantic-0.0.5/src/fodantic/form.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,95 +31,95 @@
         *,
         model_cls: t.Type[BaseModel],
         object: t.Any = None,
         prefix: str = "",
         orm_cls: t.Any = None,
     ):
         """
-        A form handler that integrates pydantic models for data validation and can
-        interact with ORM models.
+        A form handler that integrates pydantic models for data validation
+        and can interact with ORM models.
 
-        ## Arguments:
-
-        - reqdata:
-            Optional request data used for form submission.
-        - model_cls:
-            The pydantic model class for data validation.
-        - object:
-            Optional ORM model instance to fill the form and be updated when saving.
-        - prefix:
-            An optional prefix to prepend to field names (separated with a dot).
-            Defaults to an empty string.
-        - orm_cls:
-            The ORM model class for database interaction. If `None`, the `Form.save()`
-            returns a dict when the form is valid.
-
-        ## Attributes:
-
-        - model_cls (t.Type[pydantic.BaseModel]):
-            The pydantic model class for data validation.
-        - orm_cls (Any, optional):
-            The ORM model class for database interaction. Defaults to None.
-
-        - prefix (str):
-            Optional prefix used in form field names. Defaults to an empty string.
-        - fields (dict[str, FormField]):
-            Dictionary mapping field names to FormField instances.
-        - is_valid (bool):
-            Indicates whether the form data passed validation. Defaults to True.
-        - is_invalid (bool):
-            The opposite to `is_valid`.
-        - is_empty (bool):
-            If the form was initialized with request or object data
-        - errors (list[ErrorDetails]):
-            List of validation errors encountered.
-        - model (pydantic.BaseModel | None):
-            The instantiated pydantic model after validation. Defaults to None.
-
-        ## Example:
-
-        ```python
-        from fodantic import formable
-
-        @formable
-        class UserForm(pydantic.BaseModel):
-            name: str
-            age: int
-            tags: list[str]
-
-
-        empty_form = UserForm()
-        valid_form = UserForm({"name": "joe", "age": 33})
-        invalid_form = UserForm({"age": "nan"})
-
-        print(empty_form.fields)
-        '''
-        {
-           'name': FormField(name='name', annotation=str, is_required=True),
-           'age': FormField(name='age', annotation=int, is_required=True),
-           'tags': FormField(name='tags', annotation=list[str], is_required=True),
-        }
-        '''
-
-        print(empty_form.fields["age"].value)
-        #> ''
+        Args:
+            reqdata:
+                Optional request data used for form submission.
+            model_cls:
+                The pydantic model class for data validation.
+            object:
+                Optional ORM model instance to fill the form and be updated
+                when saving.
+            prefix:
+                An optional prefix to prepend to field names (separated with
+                a dot). Defaults to an empty string.
+            orm_cls:
+                The ORM model class for database interaction. If `None`,
+                the `Form.save()` returns a dict when the form is valid.
+
+        Attributes:
+            model_cls:
+                The pydantic model class for data validation.
+            orm_cls:
+                The ORM model class for database interaction.
+                Defaults to `None`.
+            prefix:
+                Optional prefix used in form field names.
+                Defaults to an empty string.
+            fields:
+                Dictionary mapping field names to `FormField` instances.
+            is_valid:
+                Indicates whether the form data passed validation.
+                Defaults to True.
+            is_invalid:
+                The opposite to `is_valid`.
+            is_empty:
+                If the form was initialized with request or object data
+            errors:
+                List of validation errors encountered.
+            model:
+                The instantiated pydantic model after validation.
+                Defaults to `None`.
+
+        Example:
+            ```python
+            from fodantic import formable
+
+            @formable
+            class UserForm(pydantic.BaseModel):
+                name: str
+                age: int
+                tags: list[str]
+
+
+            empty_form = UserForm()
+            valid_form = UserForm({"name": "joe", "age": 33})
+            invalid_form = UserForm({"age": "nan"})
+
+            print(empty_form.fields)
+            '''
+            {
+            'name': FormField(name='name', annotation=str, is_required=True),
+            'age': FormField(name='age', annotation=int, is_required=True),
+            'tags': FormField(name='tags', annotation=list[str], is_required=True),
+            }
+            '''
 
-        print(valid_form.fields["age"].value)
-        #> 33
+            print(empty_form.fields["age"].value)
+            #> ''
 
-        print(empty_form.save())
-        #> ValueError
+            print(valid_form.fields["age"].value)
+            #> 33
 
-        print(valid_form.save())
-        #> {'name': 'joe', 'age': 3, 'tags': []}
+            print(empty_form.save())
+            #> ValueError
 
-        print(invalid_form.save())
-        #> ValueError
+            print(valid_form.save())
+            #> {'name': 'joe', 'age': 3, 'tags': []}
 
-        ```
+            print(invalid_form.save())
+            #> ValueError
+            ```
 
         """
         self.model_cls = model_cls
         self.orm_cls = orm_cls
 
         self.prefix = f"{prefix}." if prefix else ""
         self.errors = []
@@ -252,17 +252,16 @@
     *,
     orm: t.Any = None,
 ) -> FBM | t.Callable[[BM], FBM]:
     """
     Decorator to add a `as_form` class method to a Pydantic model.
     This decorator can be used with or without parenthesis.
 
-    Arguments:
-
-    - orm: Optional class of an ORM model
+    Args:
+        orm: Optional class of an ORM model
 
     """
 
     def decorator(model_cls: BM) -> FBM:
         """The actual decorator logic that adds the `as_form` method."""
 
         def as_form(
```

### Comparing `fodantic-0.0.4/src/fodantic/form_field.py` & `fodantic-0.0.5/src/fodantic/form_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,48 +20,48 @@
     is_multiple: bool
     value: str | list[str] | bool
 
     def __init__(self, *, name: str, info: "FieldInfo", form: "Form"):
         """
         A form field
 
-        ## Attributes:
-
-        - model_name:
-            The name used in the pydantic Model (different than the one in the
-            HTML form if a prefix is used).
-        - name:
-            The name, maybe with a prefix, used in the HTML form.
-        - value:
-            The current (potentially invalid) field value.
-        - is_required:
-            Whether the field is required or optional.
-        - is_multiple:
-            Whether the field expects a list of values instead of just one.
-        - is_bool:
-            Whether the field is of type boolean.
-
-        - annotation:
-            The type annotation of the field.
-        - alias:
-            The alias name of the field.
-        - alias_name:
-            The alias, maybe with a prefix, that can be also used in the HTML form.
-        - alias_priority:
-            The priority of the field's alias.
-        - default:
-            The default value of the field.
-        - default_factory:
-            The factory function used to construct the default for the field.
-        - description:
-            The description of the field.
-        - examples:
-            List of examples of the field.
-        - title:
-            The title of the field.
+        Attributes:
+            model_name:
+                The name used in the pydantic Model (different than the one in
+                the HTML form if a prefix is used).
+            name:
+                The name, maybe with a prefix, used in the HTML form.
+            value:
+                The current (potentially invalid) field value.
+            is_required:
+                Whether the field is required or optional.
+            is_multiple:
+                Whether the field expects a list of values instead of just one.
+            is_bool:
+                Whether the field is of type boolean.
+
+            annotation:
+                The type annotation of the field.
+            alias:
+                The alias name of the field.
+            alias_name:
+                The alias, maybe with a prefix, that can be also used in the
+                HTML form.
+            alias_priority:
+                The priority of the field's alias.
+            default:
+                The default value of the field.
+            default_factory:
+                The factory function used to construct the default for the field.
+            description:
+                The description of the field.
+            examples:
+                List of examples of the field.
+            title:
+                The title of the field.
 
         """
         self._form = form
         self.model_name = name
         self.is_required = info.is_required()
 
         annotation_origin = t.get_origin(info.annotation)
```

### Comparing `fodantic-0.0.4/src/fodantic/wrappers.py` & `fodantic-0.0.5/src/fodantic/wrappers.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,38 @@
 
 class DataWrapper:
     def __init__(self, source: t.Any):
         """
         A utility class for wrapping request data and providing a consistent interface
         for updating, accessing single values, or lists of values.
 
-        ## Arguments:
-
-        - source: The underlying data source. Can be a Multidict implementation
-            or a regular dict.
+        Args:
+            source:
+                The underlying data source. Can be a Multidict
+                implementation or a regular dict.
 
         """
         self.source: t.Any = {} if source is None else source
-        self.get = self._find_get_method()
-        self.getall = self._find_getall_method()
+        self._get_method = self._find_get_method()
+        self._getall_method = self._find_getall_method()
 
     def __contains__(self, __name: str) -> bool:
         return __name in self.source
 
+    def get(self, key, *args, **kwargs):
+        return self._get_method(key, *args, **kwargs)
+
+    def getall(self, key, *args, **kwargs):
+        """This method always returns a list, even if the
+        key doesn't exists."""
+        try:
+            return self._getall_method(key, *args, **kwargs)
+        except KeyError:
+            return []
+
     def _find_get_method(self) -> t.Callable[[str], t.Any]:
         if hasattr(self.source, "get"):
             return self.source.get
 
         def get_fallback(name: str) -> t.Any:
             return getattr(self.source, name, None)
 
@@ -54,18 +65,18 @@
 
 class ObjectWrapper:
     def __init__(self, source: t.Any):
         """
         A utility class for wrapping request data and providing a consistent interface
         for updating, accessing single values, or lists of values.
 
-        ## Arguments:
-
-        - source: The underlying data source. Can be a Multidict implementation
-            or a regular dict.
+        Args:
+            source:
+                The underlying data source. Can be a Multidict
+                implementation or a regular dict.
 
         """
         self.source: t.Any = {} if source is None else source
         self.is_dict = isinstance(source, dict)
         self.get = self._find_get_method()
 
     def _find_get_method(self) -> t.Callable[[str], t.Any]:
```

