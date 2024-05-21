# Comparing `tmp/jsonschema_gentypes-2.5.0.tar.gz` & `tmp/jsonschema_gentypes-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-2.5.0.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-2.6.0.tar", max compression
```

## Comparing `jsonschema_gentypes-2.5.0.tar` & `jsonschema_gentypes-2.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1304 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/LICENSE
--rw-r--r--   0        0        0     3358 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/README.md
--rw-r--r--   0        0        0    21579 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0    20430 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/api.py
--rw-r--r--   0        0        0    26611 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_04.py
--rw-r--r--   0        0        0     2909 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_06.py
--rw-r--r--   0        0        0      149 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_07.py
--rw-r--r--   0        0        0     4476 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_2019_09.py
--rw-r--r--   0        0        0     6083 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_2020_12.py
--rw-r--r--   0        0        0    15758 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2774 2024-02-12 16:54:50.004147 jsonschema_gentypes-2.5.0/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     5907 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_04.py
--rw-r--r--   0        0        0     5869 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_06.py
--rw-r--r--   0        0        0     6362 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_07.py
--rw-r--r--   0        0        0     7276 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
--rw-r--r--   0        0        0     2257 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
--rw-r--r--   0        0        0      427 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
--rw-r--r--   0        0        0     1253 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
--rw-r--r--   0        0        0      295 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
--rw-r--r--   0        0        0      966 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
--rw-r--r--   0        0        0     3095 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
--rw-r--r--   0        0        0     7124 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
--rw-r--r--   0        0        0     2126 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
--rw-r--r--   0        0        0      427 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
--rw-r--r--   0        0        0     1062 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
--rw-r--r--   0        0        0      966 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
--rw-r--r--   0        0        0     3096 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
--rw-r--r--   0        0        0        0 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     7332 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/resolver.py
--rw-r--r--   0        0        0     3067 2024-02-12 16:53:48.120275 jsonschema_gentypes-2.5.0/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     2562 2024-02-12 16:55:29.176077 jsonschema_gentypes-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1304 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/LICENSE
+-rw-r--r--   0        0        0     3358 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/README.md
+-rw-r--r--   0        0        0    21870 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0    21054 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/api.py
+-rw-r--r--   0        0        0    26755 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_04.py
+-rw-r--r--   0        0        0     2909 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_06.py
+-rw-r--r--   0        0        0      149 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_07.py
+-rw-r--r--   0        0        0     4476 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_2019_09.py
+-rw-r--r--   0        0        0     6083 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_2020_12.py
+-rw-r--r--   0        0        0    15758 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     3300 2024-05-21 15:52:54.908923 jsonschema_gentypes-2.6.0/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     5907 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_04.py
+-rw-r--r--   0        0        0     5869 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_06.py
+-rw-r--r--   0        0        0     6362 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_07.py
+-rw-r--r--   0        0        0     7276 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
+-rw-r--r--   0        0        0     2257 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
+-rw-r--r--   0        0        0      427 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
+-rw-r--r--   0        0        0     1253 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
+-rw-r--r--   0        0        0      295 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
+-rw-r--r--   0        0        0      966 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
+-rw-r--r--   0        0        0     3095 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
+-rw-r--r--   0        0        0     7124 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
+-rw-r--r--   0        0        0     2126 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
+-rw-r--r--   0        0        0      427 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
+-rw-r--r--   0        0        0     1062 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
+-rw-r--r--   0        0        0      966 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
+-rw-r--r--   0        0        0     3096 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
+-rw-r--r--   0        0        0        0 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     7332 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/resolver.py
+-rw-r--r--   0        0        0     3343 2024-05-21 15:52:17.188845 jsonschema_gentypes-2.6.0/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     2569 2024-05-21 15:53:36.080984 jsonschema_gentypes-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.6.0/PKG-INFO
```

### Comparing `jsonschema_gentypes-2.5.0/LICENSE` & `jsonschema_gentypes-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/README.md` & `jsonschema_gentypes-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/__init__.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,14 +669,15 @@
         Union[
             jsonschema_draft_04.JSONSchemaD4,
             jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
         ]
     ],
     proposed_name: Optional[str] = None,
     upper: bool = False,
+    get_name_properties: Optional[str] = None,
 ) -> str:
     """
     Get the name for an element.
 
     Parameter:
         schema: the concerned schema
         proposed_name: a name that we will use it the schema hasn't any title
@@ -690,14 +691,19 @@
 
     prefix = "" if has_title else "_"
     if upper:
         # Upper case
         name = name.upper()
         # Remove spaces
         return prefix + "".join(["_" if char.isspace() else char for char in name])
+    elif get_name_properties == "UpperFirst":
+        # Change just the first letter to upper case
+        name = name[0].upper() + name[1:]
+        # Remove spaces
+        return prefix + "".join([char for char in name if not char.isspace()])
     else:
         # Title case
         name = name.title()
         # Remove spaces
         return prefix + "".join([char for char in name if not char.isspace()])
```

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/api.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,22 @@
         \-> get_type_end()
     """
 
     def __init__(
         self,
         resolver: RefResolver,
         additional_properties: configuration.AdditionalProperties = configuration.ADDITIONALPROPERTIES_ONLY_EXPLICIT,
+        get_name_properties: configuration.GetNameProperties = configuration.GETNAMEPROPERTIES_TITLE,
     ) -> None:
         """
         Initialize with a resolver.
         """
         self.resolver = resolver
         self.additional_properties = additional_properties
+        self.get_name_properties = get_name_properties
         # types by reference
         self.ref_type: dict[str, Type] = {}
         self.root: Optional[TypeProxy] = None
 
     def get_type_handler(self, schema_type: str) -> Callable[
         [
             Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020],
@@ -166,35 +168,50 @@
             additional_description = the_type.comments()
             if description and additional_description:
                 description.append("")
             description += additional_description
             if description:
                 if not isinstance(the_type, NamedType):
                     if auto_alias:
-                        the_type = TypeAlias(get_name(schema_meta_data, proposed_name), the_type, description)
+                        the_type = TypeAlias(
+                            self.get_name(schema_meta_data, proposed_name), the_type, description
+                        )
                 the_type.set_comments(description)
 
         if "default" in schema_meta_data:
             the_type.add_depends_on(
                 Constant(
-                    f"{get_name(schema_meta_data, proposed_name, True)}_DEFAULT",
+                    f"{self.get_name(schema_meta_data, proposed_name, True)}_DEFAULT",
                     schema_meta_data["default"],
                     [f"Default value of the field path '{proposed_name}'"],
                 )
             )
 
         proxy.set_type(the_type)
         if root:
             assert self.root is not None
             self.root.set_type(the_type)
 
         self.get_type_end(schema, proxy)
 
         return the_type
 
+    def get_name(
+        self,
+        schema: Optional[
+            Union[
+                jsonschema_draft_04.JSONSchemaD4,
+                jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
+            ]
+        ],
+        proposed_name: Optional[str] = None,
+        upper: bool = False,
+    ) -> str:
+        return get_name(schema, proposed_name, upper, self.get_name_properties)
+
     def resolve_ref(
         self,
         schema: Union[
             jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
         ],
     ) -> Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020]:
         """Resolve a reference in the schema."""
@@ -338,15 +355,15 @@
             type_, named_types, _ = self.any_of(
                 schema,
                 schema["anyOf"],
                 proposed_name,
                 "anyof",
             )
             if not isinstance(type_, NamedType):
-                type_ = TypeAlias(get_name(schema_meta_data, proposed_name), type_)
+                type_ = TypeAlias(self.get_name(schema_meta_data, proposed_name), type_)
             elif type_.comments():
                 type_.comments().append("")
             type_.comments().append("Aggregation type: anyOf")
 
             if named_types:
                 for named_type in named_types:
                     type_.add_depends_on(named_type)
@@ -390,15 +407,15 @@
         if isinstance(schema_type, list) and len(schema_type) == 1:
             schema_type = schema_type[0]
 
         if isinstance(schema_type, list):
             if len(schema_type) == 0:
                 return BuiltinType("None")
             inner_types = []
-            name = get_name(schema_meta_data, proposed_name)
+            name = self.get_name(schema_meta_data, proposed_name)
             has_title = "title" in schema_meta_data
             proposed_name = schema_meta_data.get("title", proposed_name)
 
             schema_copy = cast(
                 Union[
                     jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020
                 ],
```

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_04.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_04.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 jsonschema_draft_04.JSONSchemaD4,
                 jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
             ],
             schema,
         )
 
         return TypeEnum(
-            get_name(schema_meta_data, proposed_name),
+            self.get_name(schema_meta_data, proposed_name),
             cast(list[Union[int, float, bool, str, None]], schema["enum"]),
             get_description(schema_meta_data),
         )
 
     def boolean(
         self,
         schema: Union[
@@ -95,15 +95,15 @@
                 jsonschema_draft_04.JSONSchemaD4,
                 jsonschema_draft_2020_12_validation.JSONSchemaItemD2020,
             ],
             schema,
         )
 
         std_dict = None
-        name = get_name(schema_meta_data, proposed_name)
+        name = self.get_name(schema_meta_data, proposed_name)
         schema.setdefault("used", set()).add("additionalProperties")  # type: ignore[typeddict-item]
         additional_properties = cast(
             Union[jsonschema_draft_04.JSONSchemaD4, jsonschema_draft_2020_12_applicator.JSONSchemaD2020],
             schema.get("additionalProperties"),
         )
         if (
             additional_properties is True
@@ -290,15 +290,17 @@
                             jsonschema_draft_04.JSONSchemaD4,
                             jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
                         ],
                         combined_schema,
                     )
                     if not isinstance(type_, NamedType):
                         type_ = TypeAlias(
-                            get_name(combined_schema_meta_data, proposed_name + " " + sub_name), type_, []
+                            self.get_name(combined_schema_meta_data, proposed_name + " " + sub_name),
+                            type_,
+                            [],
                         )
 
                     additional_types.append(type_)
                 inner_types.append(type_)
                 inner_types_schema.append(combined_schema)
             elif (
                 "anyOf" in sub_schema
@@ -322,15 +324,17 @@
                             jsonschema_draft_04.JSONSchemaD4,
                             jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
                         ],
                         combined_schemas,
                     )
                     if not isinstance(type_, NamedType):
                         type_ = TypeAlias(
-                            get_name(combined_schema_meta_data, proposed_name + " " + sub_name), type_, []
+                            self.get_name(combined_schema_meta_data, proposed_name + " " + sub_name),
+                            type_,
+                            [],
                         )
                     additional_types.append(type_)
                 inner_types.append(type_)
                 inner_types_schema += combined_schemas
             else:
                 sub_schema = self.combined_sub_type(schema, sub_schema)
                 inner_types_schema.append(sub_schema)
@@ -491,15 +495,15 @@
                             jsonschema_draft_04.JSONSchemaD4,
                             jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
                         ],
                         combined_schema,
                     )
                     if not isinstance(type_, NamedType):
                         type_ = TypeAlias(
-                            get_name(combined_schema_meta_data, f"{proposed_name} {sub_name}{index}"),
+                            self.get_name(combined_schema_meta_data, f"{proposed_name} {sub_name}{index}"),
                             type_,
                             [],
                         )
 
                     additional_types.append(type_)
                 all_schema = self.combined_base_type_all_of(all_schema, combined_schema)
             elif "anyOf" in new_schema or "oneOf" in new_schema:
@@ -518,15 +522,15 @@
                             jsonschema_draft_04.JSONSchemaD4,
                             jsonschema_draft_2019_09_meta_data.JSONSchemaItemD2019,
                         ],
                         combined_schemas,
                     )
                     if not isinstance(type_, NamedType):
                         type_ = TypeAlias(
-                            get_name(combined_schema_meta_data, f"{proposed_name} {sub_name}{index}"),
+                            self.get_name(combined_schema_meta_data, f"{proposed_name} {sub_name}{index}"),
                             type_,
                             [],
                         )
                     additional_types.append(type_)
                 for combined_schema in combined_schemas:
                     all_schema = self.combined_base_type_all_of(all_schema, combined_schema)
             else:
```

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_06.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_2019_09.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/api_draft_2020_12.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/api_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/cli.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,21 @@
     additional_properties: "AdditionalProperties"
     """
     Additional properties.
 
     Describe how to deal with additional properties
     """
 
+    get_name_properties: "GetNameProperties"
+    """
+    Get name properties.
+
+    Describe the rules to use to get the name of an element
+    """
+
 
 class Configuration(TypedDict, total=False):
     """
     Configuration.
 
     The JSON Schema generate Python types configuration
     """
@@ -97,14 +104,26 @@
     """
     vocabularies.
 
     Used to add some vocabularies
     """
 
 
+GetNameProperties = Union[Literal["Title"], Literal["UpperFirst"]]
+"""
+Get name properties.
+
+Describe the rules to use to get the name of an element
+"""
+GETNAMEPROPERTIES_TITLE: Literal["Title"] = "Title"
+"""The values for the 'Get name properties' enum"""
+GETNAMEPROPERTIES_UPPERFIRST: Literal["UpperFirst"] = "UpperFirst"
+"""The values for the 'Get name properties' enum"""
+
+
 PRE_COMMIT_ARGUMENTS_DEFAULT: list[Any] = []
 """ Default value of the field path 'Pre-commit configuration arguments' """
 
 
 PRE_COMMIT_ENABLE_DEFAULT = False
 """ Default value of the field path 'Pre-commit configuration enable' """
```

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_04.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_04.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_06.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_07.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_07.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/resolver.py` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/resolver.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.5.0/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-2.6.0/jsonschema_gentypes/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999992464795524%*

 * *Differences: {"'properties'": "{'generate': {'items': {'properties': {'api_arguments': {'properties': "*

 * *                 "{'get_name_properties': OrderedDict([('type', 'string'), ('title', 'Get name "*

 * *                 "properties'), ('description', 'Describe the rules to use to get the name of an "*

 * *                 "element'), ('enum', ['Title', 'UpperFirst'])])}}}}}}"}*

```diff
@@ -24,14 +24,23 @@
                                 "description": "Describe how to deal with additional properties",
                                 "enum": [
                                     "Always",
                                     "Only explicit"
                                 ],
                                 "title": "Additional properties",
                                 "type": "string"
+                            },
+                            "get_name_properties": {
+                                "description": "Describe the rules to use to get the name of an element",
+                                "enum": [
+                                    "Title",
+                                    "UpperFirst"
+                                ],
+                                "title": "Get name properties",
+                                "type": "string"
                             }
                         },
                         "title": "API arguments",
                         "type": "object"
                     },
                     "destination": {
                         "description": "The generated Python file name",
```

### Comparing `jsonschema_gentypes-2.5.0/pyproject.toml` & `jsonschema_gentypes-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "2.5.0"
+version = "2.6.0"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
@@ -37,36 +37,36 @@
 
 [tool.poetry.scripts]
 jsonschema-gentypes = "jsonschema_gentypes.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 jsonschema = "4.21.1"
-typing-extensions = "4.9.0"
+typing-extensions = "4.10.0"
 requests = "2.31.0"
 "PyYAML" = "6.0.1"
 pinyin = { version = "0.4.0", optional = true }
 romkan = { version = "0.2.1", optional = true }
 romanize = { version = "1.0.2", optional = true }
-pre-commit = { version = "3.6.0", optional = true }
-referencing = "0.33.0"
+pre-commit = { version = "3.7.0", optional = true }
+referencing = "0.34.0"
 
 [tool.poetry.extras]
 generate = []
 tools = ["pre-commit"]
 extra = ['pinyin', 'romkan', 'romanize']
 
 [tool.poetry.group.dev.dependencies]
 prospector = { extras = ["with_mypy", "with_bandit", "with_pyroma"], version = "1.10.3" }
-prospector-profile-duplicated = "0.5.1"
+prospector-profile-duplicated = "1.2.0"
 prospector-profile-utils = "1.7.2"
-pytest = "8.0.0"
-pytest-cov = "4.1.0"
-types-requests = "2.31.0.20240125"
-types-pyyaml = "6.0.12.12"
+pytest = "8.1.1"
+pytest-cov = "5.0.0"
+types-requests = "2.31.0.20240311"
+types-pyyaml = "6.0.12.20240311"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "poetry-plugin-tweak-dependencies-version", "poetry-plugin-drop-python-upper-constraint"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `jsonschema_gentypes-2.5.0/PKG-INFO` & `jsonschema_gentypes-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 2.5.0
+Version: 2.6.0
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.9
```

