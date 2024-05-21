# Comparing `tmp/django_allauth_ui-0.3.0.tar.gz` & `tmp/django_allauth_ui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_ui-0.3.0.tar", max compression
+gzip compressed data, was "django_allauth_ui-0.3.1.tar", max compression
```

## Comparing `django_allauth_ui-0.3.0.tar` & `django_allauth_ui-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/LICENSE
--rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/__init__.py
--rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/apps.py
--rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/input.css
--rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/output.css
--rw-r--r--   0        0        0     1383 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/_button.html
--rw-r--r--   0        0        0      254 2023-10-23 20:51:46.098003 django_allauth_ui-0.3.0/allauth_ui/templates/account/_links.html
--rw-r--r--   0        0        0      224 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/_non_field_errors.html
--rw-r--r--   0        0        0      840 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/_render_form.html
--rw-r--r--   0        0        0      984 2023-01-29 13:57:46.486760 django_allauth_ui-0.3.0/allauth_ui/templates/account/base.html
--rw-r--r--   0        0        0     1001 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/email_confirm.html
--rw-r--r--   0        0        0     2226 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/login.html
--rw-r--r--   0        0        0      392 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/logout.html
--rw-r--r--   0        0        0      664 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset.html
--rw-r--r--   0        0        0     1221 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     1150 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      508 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      595 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/signup.html
--rw-r--r--   0        0        0      605 2024-01-31 08:24:49.504001 django_allauth_ui-0.3.0/allauth_ui/templates/account/signup_closed.html
--rw-r--r--   0        0        0      765 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/verification_sent.html
--rw-r--r--   0        0        0      677 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0       33 2024-01-29 10:34:33.647135 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/base.html
--rw-r--r--   0        0        0     1649 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1213 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/login.html
--rw-r--r--   0        0        0      731 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/signup.html
--rw-r--r--   0        0        0      774 2022-12-20 01:48:32.803185 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      624 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templatetags/allauth_ui.py
--rw-r--r--   0        0        0      943 2024-05-18 21:09:30.733159 django_allauth_ui-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.0/setup.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.1/LICENSE
+-rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.1/allauth_ui/__init__.py
+-rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.1/allauth_ui/apps.py
+-rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.1/allauth_ui/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.1/allauth_ui/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/input.css
+-rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/output.css
+-rw-r--r--   0        0        0     1428 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_button.html
+-rw-r--r--   0        0        0      267 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_links.html
+-rw-r--r--   0        0        0      242 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_non_field_errors.html
+-rw-r--r--   0        0        0      925 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/_render_form.html
+-rw-r--r--   0        0        0     1197 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/base.html
+-rw-r--r--   0        0        0     1128 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     2289 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/login.html
+-rw-r--r--   0        0        0      445 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/logout.html
+-rw-r--r--   0        0        0      752 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset.html
+-rw-r--r--   0        0        0     1416 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     1329 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      554 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      686 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/signup.html
+-rw-r--r--   0        0        0      643 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      830 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      749 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0       34 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/base.html
+-rw-r--r--   0        0        0     2140 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1396 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      808 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0      796 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      560 2024-05-21 02:37:06.322356 django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/social_login.html
+-rw-r--r--   0        0        0      786 2024-05-21 01:59:06.184416 django_allauth_ui-0.3.1/allauth_ui/templatetags/allauth_ui.py
+-rw-r--r--   0        0        0     1147 2024-05-21 02:37:11.874358 django_allauth_ui-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.1/PKG-INFO
```

### Comparing `django_allauth_ui-0.3.0/LICENSE` & `django_allauth_ui-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.0/allauth_ui/locale/es/LC_MESSAGES/django.po` & `django_allauth_ui-0.3.1/allauth_ui/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.0/allauth_ui/locale/fr/LC_MESSAGES/django.po` & `django_allauth_ui-0.3.1/allauth_ui/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/input.css` & `django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/input.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/output.css` & `django_allauth_ui-0.3.1/allauth_ui/static/allauth_ui/output.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/_button.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/_button.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 {% with base_color=base_color|default:"bg-blue" %}
-<button type="submit" class="flex items-center justify-center w-64 h-12 px-6 mt-8 text-lg text-white uppercase {{ base_color }}-600 rounded text-bold hover:{{ base_color }}-700">
-  <svg class="hidden w-5 h-5 mr-3 animate-spin" viewBox="0 0 24 24">
-    <path
-      className="opacity-25"
-      fill="currentColor"
-      d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"
-    ></path>
-  </svg>
-  {{ text }}
-
-   <script>
+    <button type="submit"
+            class="flex items-center justify-center w-64 h-12 px-6 mt-8 text-lg text-white uppercase {{ base_color }}-600 rounded text-bold hover:{{ base_color }}-700">
+        <svg class="hidden w-5 h-5 mr-3 animate-spin" viewBox="0 0 24 24">
+            <path className="opacity-25" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z">
+            </path>
+        </svg>
+        {{ text }}
+        <script>
     const script = document.currentScript;
     const button = script.parentElement;
     const form = button.closest("form");
     const loader = button.querySelector("svg");
 
     const toggle = () => {
       button.classList.toggle("{{ base_color }}-600");
@@ -32,10 +29,10 @@
       // Clear on timeout
       setTimeout(() => {
         toggle();
         button.removeAttribute("disabled");
         loader.classList.toggle("hidden");
       }, 3000);
     }, true);
-   </script>
-</button>
+        </script>
+    </button>
 {% endwith %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/_render_form.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/_render_form.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 {% load widget_tweaks %}
-
 {% csrf_token %}
-
 {% if redirect_field_value %}
-<input type="hidden" name="{{ redirect_field_name }}" value="{{ redirect_field_value }}"/>
+    <input type="hidden"
+           name="{{ redirect_field_name }}"
+           value="{{ redirect_field_value }}" />
 {% endif %}
-
 {% include "account/_non_field_errors.html" %}
-
 {% for field in form.visible_fields %}
-  <div class="mb-4">
-  {{ field|add_label_class:"font-semibold text-xs" }}
-  {% if field.errors %}
-  {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 border-red-500 rounded focus:outline-none focus:ring-2" %}
-  {% else %}
-  {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 rounded focus:outline-none focus:ring-2" %}
-  {% endif %}
-  {% for error in field.errors %}
-  <span class="flex items-center max-w-xs mt-1 ml-1 text-xs font-medium tracking-wide text-red-500">
-    {{ error }}
-  </span>
-  {% endfor %}
-  </div>
+    <div class="mb-4">
+        {{ field|add_label_class:"font-semibold text-xs" }}
+        {% if field.errors %}
+            {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 border-red-500 rounded focus:outline-none focus:ring-2" %}
+        {% else %}
+            {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 rounded focus:outline-none focus:ring-2" %}
+        {% endif %}
+        {% for error in field.errors %}
+            <span class="flex items-center max-w-xs mt-1 ml-1 text-xs font-medium tracking-wide text-red-500">{{ error }}</span>
+        {% endfor %}
+    </div>
 {% endfor %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/base.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/base.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 {% load static %}
 <!DOCTYPE html>
 <html>
-  <head>
-    <meta charset="UTF-8">
-    <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>{% block head_title %}{% endblock %}</title>
-    <link rel="stylesheet" href="{% static 'allauth_ui/output.css' %}">
-    {% block extra_head %}
-    {% endblock %}
-  </head>
-  <body>
-    {% if messages %}
-    <div>
-      {% for message in messages %}
-      <div class="flex items-center px-4 py-3 text-sm font-bold text-white bg-blue-500" role="alert">
-        <p>{{ message }}</p>
-      </div>
-      {% endfor %}
-    </div>
-    {% endif %}
-    {% block content %}
-    <div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
-      <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg grow-0">
-        {% block whitebox %}
+    <head>
+        <meta charset="UTF-8">
+        <meta http-equiv="X-UA-Compatible" content="IE=edge">
+        <meta name="viewport" content="width=device-width, initial-scale=1.0">
+        <title>
+            {% block head_title %}{% endblock %}
+        </title>
+        <link rel="stylesheet" href="{% static 'allauth_ui/output.css' %}">
+        {% block extra_head %}{% endblock %}
+    </head>
+    <body>
+        {% if messages %}
+            <div>
+                {% for message in messages %}
+                    <div class="flex items-center px-4 py-3 text-sm font-bold text-white bg-blue-500"
+                         role="alert">
+                        <p>{{ message }}</p>
+                    </div>
+                {% endfor %}
+            </div>
+        {% endif %}
+        {% block content %}
+            <div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
+                <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg grow-0">
+                    {% block whitebox %}{% endblock %}
+                </div>
+            </div>
         {% endblock %}
-    </div>
-  </div>
-    {% endblock %}
-  </body>
+    </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load static %}
-{% block extra_head %} {% endblock %}
+{% block extra_head %}{% endblock %}
 {% if messages %}
 {% for message in messages %}
 {{ message }}
 {% endfor %}
 {% endif %} {% block content %}
-{% block whitebox %} {% endblock %}
+{% block whitebox %}{% endblock %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/login.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/login.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,47 @@
 {% extends "account/base.html" %}
-{% load i18n %}
-{% load widget_tweaks %}
-{% load account socialaccount %}
-
+{% load i18n account allauth_ui widget_tweaks %}
 {% block head_title %}
-  {% translate "Sign in" %}
+    {% translate "Sign in" %}
 {% endblock %}
-
 {% block whitebox %}
-<h1 class="mb-5 text-3xl text-center">Sign in</h1>
-<form method="POST" action="{% url 'account_login' %}" class="flex flex-col items-center grow-0">
-  {% csrf_token %}
-
-  {% include "account/_non_field_errors.html" %}
-
-  {% for field in form.visible_fields %}
-    {% if field.name != "remember" %}
-    <div class="mb-4">
-    {{ field|add_label_class:"font-semibold text-xs" }}
-    {% if field.errors %}
-    {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 border-red-500 rounded focus:outline-none focus:ring-2" %}
-    {% else %}
-    {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 rounded focus:outline-none focus:ring-2" %}
+    <h1 class="mb-5 text-3xl text-center">Sign in</h1>
+    <form method="POST"
+          action="{% url 'account_login' %}"
+          class="flex flex-col items-center grow-0">
+        {% csrf_token %}
+        {% include "account/_non_field_errors.html" %}
+        {% for field in form.visible_fields %}
+            {% if field.name != "remember" %}
+                <div class="mb-4">
+                    {{ field|add_label_class:"font-semibold text-xs" }}
+                    {% if field.errors %}
+                        {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 border-red-500 rounded focus:outline-none focus:ring-2" %}
+                    {% else %}
+                        {% render_field field class="flex items-center w-64 h-12 px-4 pb-2 mt-2 rounded focus:outline-none focus:ring-2" %}
+                    {% endif %}
+                    {% for error in field.errors %}
+                        <span class="flex items-center max-w-xs mt-1 ml-1 text-xs font-medium tracking-wide text-red-500">{{ error }}</span>
+                    {% endfor %}
+                </div>
+            {% endif %}
+        {% endfor %}
+        {% translate "Login" as login_text %}
+        {% include "account/_button.html" with text=login_text %}
+        <div class="flex justify-center mt-6 text-xs">
+            <a class="text-blue-400 hover:text-blue-500"
+               href="{% url 'account_reset_password' %}">{% translate "Forgot Password" %}</a>
+            <span class="mx-2 text-gray-300">/</span>
+            <a class="text-blue-400 hover:text-blue-500"
+               href="{% url 'account_signup' %}">{% translate "Sign Up" %}</a>
+        </div>
+        {% if redirect_field_value %}
+            <input type="hidden"
+                   name="{{ redirect_field_name }}"
+                   value="{{ redirect_field_value }}" />
+        {% endif %}
+    </form>
+    {% check_allauth_socialaccount_installed as is_allauth_socialaccount_installed %}
+    {% if is_allauth_socialaccount_installed %}
+        {% include "socialaccount/snippets/social_login.html" %}
     {% endif %}
-    {% for error in field.errors %}
-    <span class="flex items-center max-w-xs mt-1 ml-1 text-xs font-medium tracking-wide text-red-500">
-      {{ error }}
-    </span>
-    {% endfor %}
-    </div>
-    {% endif %}
-  {% endfor %}
-
-  {% translate "Login" as login_text %}
-  {% include "account/_button.html" with text=login_text %}
-
-  <div class="flex justify-center mt-6 text-xs">
-    <a class="text-blue-400 hover:text-blue-500" href="{% url 'account_reset_password' %}">{% translate "Forgot Password" %}
-    </a>
-    <span class="mx-2 text-gray-300">/</span>
-    <a class="text-blue-400 hover:text-blue-500" href="{% url 'account_signup' %}">{% translate "Sign Up" %}</a>
-  </div>
-
-  {% if redirect_field_value %}
-  <input type="hidden" name="{{ redirect_field_name }}" value="{{ redirect_field_value }}" />
-  {% endif %}
-</form>
-{% get_providers as socialaccount_providers %}
-{% if socialaccount_providers %}
-<div class="flex items-center self-stretch justify-between pt-3 mt-3">
-  <hr class="w-full">
-  <span class="p-2 mb-1 text-gray-400">OR</span>
-  <hr class="w-full">
-</div>
-
-<p class="text-xs text-center text-gray-500">{% translate "Sign in with a third party" %}</p>
-
-{% include "socialaccount/snippets/provider_list.html" with process="login" %}
-{% endif %}
-
-{% include "socialaccount/snippets/login_extra.html" %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 {% extends "account/base.html" %}
-
-{% block head_title %}{% translate "Password Reset" %}{% endblock %}
-
+{% load i18n %}
+{% block head_title %}
+    {% translate "Password Reset" %}
+{% endblock %}
 {% block whitebox %}
-<h1 class="mb-5 text-3xl text-center">{% translate "Password Reset" %}</h1>
-<p class="mb-5 text-sm text-center">
-  {% translate "Enter your user account's verified email address and we will send you a password reset link." %}
-</p>
-<form method="POST" action="{% url 'account_reset_password' %}" class="flex flex-col mt-4">
-  {% include "account/_render_form.html" %}
-  {% translate "Reset my password" as reset_text %}
-  {% include "account/_button.html" with text=reset_text %}
-</form>
-{% include "account/_links.html" %}
+    <h1 class="mb-5 text-3xl text-center">{% translate "Password Reset" %}</h1>
+    <p class="mb-5 text-sm text-center">
+        {% translate "Enter your user account's verified email address and we will send you a password reset link." %}
+    </p>
+    <form method="POST"
+          action="{% url 'account_reset_password' %}"
+          class="flex flex-col mt-4">
+        {% include "account/_render_form.html" %}
+        {% translate "Reset my password" as reset_text %}
+        {% include "account/_button.html" with text=reset_text %}
+    </form>
+    {% include "account/_links.html" %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_done.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_done.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 {% extends "account/base.html" %}
-
-{% block head_title %}{% translate "Password Reset" %}{% endblock %}
-
+{% load i18n %}
+{% block head_title %}
+    {% translate "Password Reset" %}
+{% endblock %}
 {% block content %}
-<div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
-  <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg">
-    <h1 class="mb-8 text-3xl text-center">{% translate "Reset email sent" %}</h1>
-  <p class="flex items-center px-4 py-3 text-sm font-bold text-white bg-blue-500 rounded" role="alert">
-    <svg class="w-4 h-4 mr-2 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z"/></svg>
-      {% translate "We have sent you an e-mail. Please contact us if you do not receive it within a few minutes." %}
-  </p>
-
-  {% include "account/_links.html" %}
-  </div>
-</div>
+    <div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
+        <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg">
+            <h1 class="mb-8 text-3xl text-center">{% translate "Reset email sent" %}</h1>
+            <p class="flex items-center px-4 py-3 text-sm font-bold text-white bg-blue-500 rounded"
+               role="alert">
+                <svg class="w-4 h-4 mr-2 fill-current"
+                     xmlns="http://www.w3.org/2000/svg"
+                     viewBox="0 0 20 20">
+                    <path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z" />
+                </svg>
+                {% translate "We have sent you an e-mail. Please contact us if you do not receive it within a few minutes." %}
+            </p>
+            {% include "account/_links.html" %}
+        </div>
+    </div>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_from_key.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/password_reset_from_key.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 {% extends "account/base.html" %}
-
 {% load i18n %}
-
-{% block head_title %}{% translate "Change Password" %}{% endblock %}
-
+{% block head_title %}
+    {% translate "Change Password" %}
+{% endblock %}
 {% block whitebox %}
-<h1 class="mb-5 text-3xl">{% if token_fail %}{% trans "Bad Token" %}{% else %}{% trans "Change Password" %}{% endif %}</h1>
-{% if token_fail %}
-    <div class="px-4 py-3" role="alert">
-      <strong class="font-bold">Invalid token!</strong>
-      <span class="block text-black">
-        {% url 'account_reset_password' as passwd_reset_url %}
-        {% blocktrans %}The password reset link was invalid, possibly because it has already been used. <br>
+    <h1 class="mb-5 text-3xl">
+        {% if token_fail %}
+            {% trans "Bad Token" %}
+        {% else %}
+            {% trans "Change Password" %}
+        {% endif %}
+    </h1>
+    {% if token_fail %}
+        <div class="px-4 py-3" role="alert">
+            <strong class="font-bold">Invalid token!</strong>
+            <span class="block text-black">
+                {% url 'account_reset_password' as passwd_reset_url %}
+                {% blocktrans %}The password reset link was invalid, possibly because it has already been used. <br>
         Please request a
         <a class="text-blue-400 hover:text-blue-500" href="{{ passwd_reset_url }}">new password reset</a>.{% endblocktrans %}
-      </span>
-    </div>
-{% else %}
-  {% if form %}
-      <form method="POST" action="{{ action_url }}">
-        {% include "account/_render_form.html" %}
-        {% translate "Change password" as change_text %}
-        {% include "account/_button.html" with text=change_text %}
-      </form>
-  {% else %}
-      <p>{% trans 'Your password is now changed.' %}</p>
-  {% endif %}
-{% endif %}
+            </span>
+        </div>
+    {% else %}
+        {% if form %}
+            <form method="POST" action="{{ action_url }}">
+                {% include "account/_render_form.html" %}
+                {% translate "Change password" as change_text %}
+                {% include "account/_button.html" with text=change_text %}
+            </form>
+        {% else %}
+            <p>{% trans 'Your password is now changed.' %}</p>
+        {% endif %}
+    {% endif %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/account/verification_sent.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/account/verification_sent.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 {% extends "account/base.html" %}
-
 {% load i18n %}
-
-{% block head_title %}{% trans "Verify Your E-mail Address" %}{% endblock %}
-
+{% block head_title %}
+    {% trans "Verify Your E-mail Address" %}
+{% endblock %}
 {% block content %}
-<div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
-  <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg md:w-7/12 xl:w-5/12">
-    <h1 class="mb-5 text-3xl text-center">{% trans "Verify Your E-mail Address" %}</h1>
-    <p class="py-3">
-      {% blocktrans %}
+    <div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
+        <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg md:w-7/12 xl:w-5/12">
+            <h1 class="mb-5 text-3xl text-center">{% trans "Verify Your E-mail Address" %}</h1>
+            <p class="py-3">
+                {% blocktrans %}
       We have sent an e-mail to you for verification. Follow the link provided to finalize the signup process.
       Please contact us if you do not receive it within a few minutes.
       {% endblocktrans %}
-    </p>
-    {% include "account/_links.html" %}
-  </div>
-</div>
+            </p>
+            {% include "account/_links.html" %}
+        </div>
+    </div>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/authentication_error.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/authentication_error.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 {% extends "socialaccount/base.html" %}
-
 {% load i18n %}
-
-{% block head_title %}{% trans "Social Network Login Failure" %}{% endblock %}
-
+{% block head_title %}
+    {% trans "Social Network Login Failure" %}
+{% endblock %}
 {% block content %}
-<div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
-  <div class="inline-flex flex-col items-center p-12 bg-white rounded shadow-lg">
-    <h1 class="mb-5 text-3xl text-center">{% trans "Social Network Login Failure" %}</h1>
-
-    <p>
-      {% trans "An error occurred while attempting to login via your social network account." %}
-    </p>
-    <p><strong>Code: {{ auth_error.code }}</strong></p>
-    <p>Error: {{ auth_error.exception }}</p>
-  </div>
-</div>
+    <div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
+        <div class="inline-flex flex-col items-center p-12 bg-white rounded shadow-lg">
+            <h1 class="mb-5 text-3xl text-center">{% trans "Social Network Login Failure" %}</h1>
+            <p>{% trans "An error occurred while attempting to login via your social network account." %}</p>
+            <p>
+                <strong>Code: {{ auth_error.code }}</strong>
+            </p>
+            <p>Error: {{ auth_error.exception }}</p>
+        </div>
+    </div>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/login.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/login.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 {% extends "socialaccount/base.html" %}
-
+{% load i18n %}
 {% block whitebox %}
-<div class="flex items-center px-4 py-3 text-sm text-white bg-blue-500 rounded" role="alert">
-  <svg class="w-4 h-4 mr-2 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z"/></svg>
-  <p>
-    {% if process == "connect" %}
-    {% translate "You are about to connect a new third party account from" %} {{ provider.name }}.
-    {% else %}
-    {% translate "You are about to sign in using a third party account from" %} {{ provider.name }}.
-    {% endif %}
-  </p>
-</div>
-<form method="POST" class="flex flex-col items-center justify-center pt-5 py-10">
-  {% csrf_token %}
-  {% translate "Continue" as continue_text %}
-  {% include "account/_button.html" with text=continue_text %}
-</form>
+    <div class="flex items-center px-4 py-3 text-sm text-white bg-blue-500 rounded"
+         role="alert">
+        <svg class="w-4 h-4 mr-2 fill-current"
+             xmlns="http://www.w3.org/2000/svg"
+             viewBox="0 0 20 20">
+            <path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z" />
+        </svg>
+        <p>
+            {% if process == "connect" %}
+                {% translate "You are about to connect a new third party account from" %} {{ provider.name }}.
+            {% else %}
+                {% translate "You are about to sign in using a third party account from" %} {{ provider.name }}.
+            {% endif %}
+        </p>
+    </div>
+    <form method="POST"
+          class="flex flex-col items-center justify-center pt-5 py-10">
+        {% csrf_token %}
+        {% translate "Continue" as continue_text %}
+        {% include "account/_button.html" with text=continue_text %}
+    </form>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/signup.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/signup.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% extends "socialaccount/base.html" %}
-
 {% load i18n %}
-
-{% block head_title %}{% trans "Sign Up" %}{% endblock %}
-
+{% block head_title %}
+    {% trans "Sign Up" %}
+{% endblock %}
 {% block whitebox %}
-<h1 class="mb-5 text-3xl text-center">{% trans "Sign Up" %}</h1>
-
-<p class="my-5">
-{% blocktrans with provider_name=account.get_provider.name site_name=site.name %}
+    <h1 class="mb-5 text-3xl text-center">{% trans "Sign Up" %}</h1>
+    <p class="my-5">
+        {% blocktrans with provider_name=account.get_provider.name site_name=site.name %}
   You are about to use your {{provider_name}} account to login to
   {{site_name}}. As a final step, please complete the following form:
 {% endblocktrans %}
-</p>
-
-<form class="signup" id="signup_form" method="post" action="{% url 'socialaccount_signup' %}">
-  {% include "account/_render_form.html" %}
-  {% translate "Sign up" as signup_text %}
-  {% include "account/_button.html" with text=signup_text %}
-</form>
+    </p>
+    <form class="signup"
+          id="signup_form"
+          method="post"
+          action="{% url 'socialaccount_signup' %}">
+        {% include "account/_render_form.html" %}
+        {% translate "Sign up" as signup_text %}
+        {% include "account/_button.html" with text=signup_text %}
+    </form>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/snippets/provider_list.html` & `django_allauth_ui-0.3.1/allauth_ui/templates/socialaccount/snippets/provider_list.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 {% load socialaccount %}
 {% load allauth_ui %}
-
 {% get_providers as socialaccount_providers %}
-
 {% for provider in socialaccount_providers %}
-   {% if provider.id == "openid" %}
-   {% for brand in provider.get_brands %}
-      <a class="flex items-center self-stretch justify-center h-12 mt-3 text-white uppercase rounded bg-stone-900 hover:bg-black"
-        href="{% provider_login_url provider.id  openid=brand.openid_url process=process  %}">{{brand.name}}</a>
-   {% endfor %}
-   {% endif %}
-      <a class="flex items-center justify-center h-12 mt-3 text-white uppercase self-stretch rounded {{ provider | socialprovider_color }}"
-        href="{% provider_login_url provider.id process=process scope=scope auth_params=auth_params %}">{{provider.name}}</a>
-
+    {% if provider.id == "openid" %}
+        {% for brand in provider.get_brands %}
+            <a class="flex items-center self-stretch justify-center h-12 mt-3 text-white uppercase rounded bg-stone-900 hover:bg-black"
+               href="{% provider_login_url provider.id  openid=brand.openid_url process=process %}">{{ brand.name }}</a>
+        {% endfor %}
+    {% endif %}
+    <a class="flex items-center justify-center h-12 mt-3 text-white uppercase self-stretch rounded {{ provider | socialprovider_color }}"
+       href="{% provider_login_url provider.id process=process scope=scope auth_params=auth_params %}">{{ provider.name }}</a>
 {% endfor %}
```

### Comparing `django_allauth_ui-0.3.0/allauth_ui/templatetags/allauth_ui.py` & `django_allauth_ui-0.3.1/allauth_ui/templatetags/allauth_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from pathlib import Path
 
 from django import template
-
+from django.conf import settings
 
 register = template.Library()
 
 input_css_path = Path(__file__).parent / ".." / "static" / "allauth_ui" / "input.css"
 social_colors = []
 
 with open(input_css_path, encoding="utf8") as f:
@@ -18,7 +18,12 @@
 
 @register.filter()
 def socialprovider_color(socialprovider):
     name = socialprovider.name.lower()
     if name in social_colors:
         return f"social-{name}"
     return "bg-stone-900 hover:bg-black"
+
+
+@register.simple_tag
+def check_allauth_socialaccount_installed():
+    return "allauth.socialaccount" in settings.INSTALLED_APPS
```

