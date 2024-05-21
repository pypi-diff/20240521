# Comparing `tmp/docsible-0.6.1.tar.gz` & `tmp/docsible-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docsible-0.6.1.tar", max compression
+gzip compressed data, was "docsible-0.6.2.tar", max compression
```

## Comparing `docsible-0.6.1.tar` & `docsible-0.6.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.6.1/LICENSE
--rw-r--r--   0        0        0     4478 2024-04-24 22:33:33.753996 docsible-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.6.1/docsible/__init__.py
--rw-r--r--   0        0        0     9952 2024-05-03 00:32:09.500714 docsible-0.6.1/docsible/cli.py
--rw-r--r--   0        0        0     6708 2024-05-02 23:22:22.429711 docsible-0.6.1/docsible/markdown_template.py
--rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.6.1/docsible/utils/__init__.py
--rw-r--r--   0        0        0    12952 2024-05-03 00:32:09.500714 docsible-0.6.1/docsible/utils/mermaid.py
--rw-r--r--   0        0        0     1823 2024-01-24 19:17:56.690945 docsible-0.6.1/docsible/utils/special_tasks_keys.py
--rw-r--r--   0        0        0     4749 2024-04-23 17:40:53.516849 docsible-0.6.1/docsible/utils/yaml.py
--rw-r--r--   0        0        0      860 2024-05-03 00:32:09.500714 docsible-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 docsible-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-09-05 22:49:19.991131 docsible-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4478 2024-05-21 16:02:16.433270 docsible-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-09-05 22:00:43.145585 docsible-0.6.2/docsible/__init__.py
+-rw-r--r--   0        0        0     9952 2024-05-21 16:51:35.355275 docsible-0.6.2/docsible/cli.py
+-rw-r--r--   0        0        0     6796 2024-05-21 16:50:52.231653 docsible-0.6.2/docsible/markdown_template.py
+-rw-r--r--   0        0        0        0 2023-09-11 08:20:14.156264 docsible-0.6.2/docsible/utils/__init__.py
+-rw-r--r--   0        0        0    12952 2024-05-21 16:02:16.433270 docsible-0.6.2/docsible/utils/mermaid.py
+-rw-r--r--   0        0        0     1823 2024-05-21 16:02:16.433270 docsible-0.6.2/docsible/utils/special_tasks_keys.py
+-rw-r--r--   0        0        0     4749 2024-05-21 16:02:16.437269 docsible-0.6.2/docsible/utils/yaml.py
+-rw-r--r--   0        0        0      860 2024-05-21 16:51:35.355275 docsible-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5542 1970-01-01 00:00:00.000000 docsible-0.6.2/PKG-INFO
```

### Comparing `docsible-0.6.1/LICENSE` & `docsible-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docsible-0.6.1/README.md` & `docsible-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `docsible-0.6.1/docsible/cli.py` & `docsible-0.6.2/docsible/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jinja2 import Environment, BaseLoader, FileSystemLoader 
 from docsible.markdown_template import static_template, collection_template
 from docsible.utils.mermaid import generate_mermaid_playbook, generate_mermaid_role_tasks_per_file
 from docsible.utils.yaml import load_yaml_generic, load_yaml_files_from_dir_custom, get_task_commensts
 from docsible.utils.special_tasks_keys import process_special_task_keys
 
 def get_version():
-    return "0.6.1"
+    return "0.6.2"
 
 def manage_docsible_file_keys(docsible_path):
     default_data = {
         'description': None,
         'requester': None,
         'users': None,
         'dt_dev': None,
```

### Comparing `docsible-0.6.1/docsible/markdown_template.py` & `docsible-0.6.2/docsible/markdown_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 {# Cicle used for decide to set Title and Required Column #}
 {% set ns = namespace (details_required = false) %}{% set ns = namespace (details_title = false) %}
 {% for key, details in defaultfile.data.items() %}{% if details.required is not none %}{% set ns.details_required = true %}{% endif %}{% if details.title is not none %}{% set ns.details_title = true %}{% endif %}{% endfor %}
 | Var          | Type         | Value       |{% if ns.details_required %}Required    |{% endif %}{% if ns.details_title %} Title       |{% endif %}
 |--------------|--------------|-------------|{% if ns.details_required %}-------------|{% endif %}{% if ns.details_title %}-------------|{% endif %}
 {%- for key, details in defaultfile.data.items() %}
 {%- set var_type = details.value.__class__.__name__ %}
-| [{{ key }}](defaults/{{ defaultfile.file }}#L{{details.line}})   | {{ var_type }}   | {{ details.value }}  | {% if ns.details_required %} {{ details.required }}  |{% endif %} {% if ns.details_title %} {{ details.title }} |{% endif %}
+| [{{ key }}](defaults/{{ defaultfile.file }}#L{{details.line}})   | {{ var_type }}   | `{{ details.value | replace('|', '\|') }}`  | {% if ns.details_required %} {{ details.required }}  |{% endif %} {% if ns.details_title %} {{ details.title | replace('|', '\|') }} |{% endif %}
 {%- endfor %}
 {%- endfor %}
 {%- else %}
 {%- endif %}
 
 
 {% if role.vars|length > 0 -%}
@@ -65,15 +65,15 @@
 #### File: {{ varsfile.file }}
 {# Cicle used for decide to set Title and Required Column #}
 {% set ns = namespace (details_required = false) %}{% set ns = namespace (details_title = false) %}{% for key, details in varsfile.data.items() %}{% if details.required is not none %}{% set ns.details_required = true %}{% endif %}{% if details.title is not none %}{% set ns.details_title = true %}{% endif %}{% endfor %}
 | Var          | Type         | Value       |{% if ns.details_required %} Required    |{% endif %}{% if ns.details_title %} Title       |{% endif %}
 |--------------|--------------|-------------|{% if ns.details_required %}-------------|{% endif %}{% if ns.details_title %}-------------|{% endif %}
 {%- for key, details in varsfile.data.items() %}
 {%- set var_type = details.value.__class__.__name__ %}
-| [{{ key }}](vars/{{ varsfile.file }}#L{{details.line}})    | {{ var_type }}   | {{ details.value }}  |{% if ns.details_required %} {{ details.required }} |{% endif %}{% if ns.details_title %} {{ details.title }} |{% endif %}
+| [{{ key }}](vars/{{ varsfile.file }}#L{{details.line}})    | {{ var_type }}   | `{{ details.value | replace('|', '\|') }}`  |{% if ns.details_required %} {{ details.required }} |{% endif %}{% if ns.details_title %} {{ details.title | replace('|', '\|') }} |{% endif %}
 {%- endfor %}
 {%- endfor %}
 {%- else %}
 {%- endif %}
 
 
 ### Tasks
```

### Comparing `docsible-0.6.1/docsible/utils/mermaid.py` & `docsible-0.6.2/docsible/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.1/docsible/utils/special_tasks_keys.py` & `docsible-0.6.2/docsible/utils/special_tasks_keys.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.1/docsible/utils/yaml.py` & `docsible-0.6.2/docsible/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `docsible-0.6.1/pyproject.toml` & `docsible-0.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docsible"
-version = "0.6.1"
+version = "0.6.2"
 description = "Document generator for ansible role/collection"
 authors = ["Lucian BLETAN <neuraluc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
```

### Comparing `docsible-0.6.1/PKG-INFO` & `docsible-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docsible
-Version: 0.6.1
+Version: 0.6.2
 Summary: Document generator for ansible role/collection
 License: MIT
 Author: Lucian BLETAN
 Author-email: neuraluc@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

