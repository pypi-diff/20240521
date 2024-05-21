# Comparing `tmp/secured-0.1.2.tar.gz` & `tmp/secured-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secured-0.1.2.tar", max compression
+gzip compressed data, was "secured-0.1.3.tar", max compression
```

## Comparing `secured-0.1.2.tar` & `secured-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1094 2024-04-27 16:49:32.066690 secured-0.1.2/LICENSE
--rw-r--r--   0        0        0     2133 2024-04-27 16:49:32.066690 secured-0.1.2/README.md
--rw-r--r--   0        0        0      462 2024-04-27 16:49:32.066690 secured-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 16:49:32.066690 secured-0.1.2/secured/__init__.py
--rw-r--r--   0        0        0     3885 2024-04-27 16:49:32.070690 secured-0.1.2/secured/attribute.py
--rw-r--r--   0        0        0     1172 2024-04-27 16:49:32.070690 secured-0.1.2/secured/log_manager.py
--rw-r--r--   0        0        0     2077 2024-04-27 16:49:32.070690 secured-0.1.2/secured/secure.py
--rw-r--r--   0        0        0     4748 2024-04-27 16:49:32.070690 secured-0.1.2/secured/secured.py
--rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 secured-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-21 07:55:57.759338 secured-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3532 2024-05-21 07:55:57.759338 secured-0.1.3/README.md
+-rw-r--r--   0        0        0      485 2024-05-21 07:55:57.759338 secured-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-21 07:55:57.759338 secured-0.1.3/secured/__init__.py
+-rw-r--r--   0        0        0     4721 2024-05-21 07:55:57.759338 secured-0.1.3/secured/attribute.py
+-rw-r--r--   0        0        0     1172 2024-05-21 07:55:57.759338 secured-0.1.3/secured/log_manager.py
+-rw-r--r--   0        0        0     2274 2024-05-21 07:55:57.759338 secured-0.1.3/secured/secure.py
+-rw-r--r--   0        0        0     6880 2024-05-21 07:55:57.759338 secured-0.1.3/secured/secured.py
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 secured-0.1.3/PKG-INFO
```

### Comparing `secured-0.1.2/LICENSE` & `secured-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secured-0.1.2/README.md` & `secured-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/secured)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/secured)
 ![PyPI](https://img.shields.io/pypi/v/secured)
+[![codecov](https://codecov.io/gh/Joaopeuko/secured/graph/badge.svg?token=W5MF118U50)](https://codecov.io/gh/Joaopeuko/secured)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/secured)
 ![PyPI - License](https://img.shields.io/pypi/l/secured)
 
 # Secured
 
 - [Secured](#secured)
   - [Installation](#installation)
   - [Usage](#usage)
     - [Example 1: Basic Usage](#example-1-basic-usage)
     - [Example 2: Custom Usage](#example-2-custom-usage)
+    - [Example 3: Config Usage](#example-3-config-usage)
+    - [Example 4: Compose](#example-4-compose)
   - [Features](#features)
 
 Secure your Python data structures and secrets with Secured. This package provides a straightforward solution for obscuring sensitive data in applications. It's specifically designed for developers who need to protect API keys, database credentials, and other critical configuration details from accidental exposure. Featuring customizable security measures, our tool allows you to control how sensitive information is represented and managed securely. It's ideal for projects that demand high data confidentiality and integrity. Please note that this provides a thin layer of protection.
 
 ## Installation
 
 To install Secured, run the following command:
@@ -49,12 +52,47 @@
 API_KEY = "12345-abcdef-67890-ghijk"
 secure_api_key = Secure(API_KEY, "API Key Protected")
 
 # Usage in code
 print(secure_api_key)  # Output: API Key Protected
 ```
 
+### Example 3: Config Usage
+
+The `Secured` class allows you to securely read configuration files containing sensitive data. Here's how you can use it:
+
+```python
+from secured.secured import Secured
+
+# Create a Secured object to read a YAML configuration file
+secured = Secured('config.yaml', secure=True)
+
+# Access configuration attributes securely
+print(secured.config.name)  # Using dot notation
+print(secured.config["name"])  # Using dictionary-like notation
+```
+
+### Example 4: Compose
+
+```python
+from secured.secured import Secured
+
+# Define the custom secure message
+message = "🔒 <Data Secured> 🔒"
+
+# Example secured object
+CONFIG_PATH = "examples/config.yaml"
+DATABASE_URL = "mysql://{user}:{password}@localhost/dbname"
+secure = Secured(CONFIG_PATH, secure=True, message=message)
+
+# Usage in code
+secure_database_url = secure.compose(DATABASE_URL, user="guest", password="guest_password")
+print(secure_database_url)  # Output: 🔒 <Data Secured> 🔒
+print(secure_database_url.get_original()) # Careful! This will print the original data, do not use it.
+print(secure_database_url == "mysql://guest:guest_password@localhost/dbname")  # Output: True
+```
+
 ## Features
 
 - **Data Protection**: Helps prevent the accidental logging or display of sensitive information.
 - **Customizable Representations**: Set how your data is displayed when being secured.
 - **Ease of Use**: Integrate seamlessly into existing Python applications.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `secured-0.1.2/secured/attribute.py` & `secured-0.1.3/secured/attribute.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Any, TypeVar
+from typing import Any, TypeVar, Union
 from .secure import Secure
 
-# A type variable that can be any type.
 T = TypeVar('T')
 
-class AttrDict(dict): # type: ignore
+class AttrDict(dict):  # type: ignore
     """
     A dictionary subclass that allows attribute-style access and can optionally secure its leaf values.
 
     This class extends the standard dictionary to support access via attributes as well as keys. If initialized
     with `secure=True`, all non-dictionary values are wrapped using the Secure class to obscure sensitive information
     with an optional custom message.
 
@@ -19,15 +18,15 @@
     Examples:
         >>> ad = AttrDict(secure=True, message="<Custom Secured>")
         >>> ad['password'] = 'my_secret'
         >>> print(ad.password)
         '<Custom Secured>'
     """
 
-    def __init__(self, *args, secure: bool = False, message: str = "<Sensitive data secured>", **kwargs) -> None: # type: ignore
+    def __init__(self, *args, secure: bool = False, message: str = "<Sensitive data secured>", **kwargs) -> None:  # type: ignore
         """
         Initialize the AttrDict with the same arguments as a normal dict, plus options to secure.
 
         Args:
             *args: Variable length argument list for dictionary items.
             secure: If True, non-dict values will be wrapped by the Secure class with the given message.
             message: Custom message used when values are secured.
@@ -39,31 +38,55 @@
         self._convert_dicts()
 
     def _convert_dicts(self) -> None:
         """Recursively converts nested dictionaries into AttrDict instances and secures values if required."""
         for key, value in list(self.items()):
             self[key] = self._convert_value(value)
 
-    def _convert_value(self, value: dict | str) -> Secure | str: # type: ignore
+    def _convert_value(self, value: Union[dict, str, Any]) -> Union[Secure, 'AttrDict', Any]:
         """
         Converts and possibly secures the value based on its type and the secure setting.
 
         Args:
             value: The value to be converted and possibly secured.
 
         Returns:
             The converted value, secured if `secure` is True and not a dictionary.
         """
         if isinstance(value, dict):
-            return AttrDict(value, secure=self.secure, message=self.message)  # type: ignore
-        elif self.secure:
-            return Secure(value, self.message)
+            value = AttrDict(value, secure=self.secure, message=self.message)  # type: ignore
+        elif self.secure and not isinstance(value, Secure):
+            value = Secure(value, self.message)
         return value
 
-    def __getattr__(self, item: str) -> Secure:
+    def _get_original(self, item: str) -> Any:
+        """
+        Retrieves the original value of the specified item, without any securing.
+
+        Args:
+            item: The attribute/key name to access.
+
+        Returns:
+            The original value associated with 'item'.
+
+        Raises:
+            AttributeError: If the attribute does not exist.
+        """
+        if item in self:
+            value = self[item]
+            if isinstance(value, Secure):
+                return value._get_original()
+            elif isinstance(value, AttrDict):
+                return {k: v._get_original() if isinstance(v, Secure) else v for k, v in value.items()}
+            else:
+                return value
+        else:
+            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{item}'")
+
+    def __getattr__(self, item: str) -> Any:
         """
         Enables attribute-style access to dictionary keys.
 
         Args:
             item: The attribute/key name to access.
 
         Returns:
```

### Comparing `secured-0.1.2/secured/log_manager.py` & `secured-0.1.3/secured/log_manager.py`

 * *Files identical despite different names*

### Comparing `secured-0.1.2/secured/secure.py` & `secured-0.1.3/secured/secure.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,7 +59,16 @@
         Returns:
             Union[float, str]: The float value of the original data, or the custom message if conversion fails.
         """
         try:
             return float(self._original)
         except ValueError:
             return self._message
+
+    def _get_original(self) -> str:
+        """
+        Retrieve the original secured data.
+
+        Returns:
+            str: The original data.
+        """
+        return self._original
```

### Comparing `secured-0.1.2/secured/secured.py` & `secured-0.1.3/secured/secured.py`

 * *Files 25% similar despite different names*

```diff
@@ -111,7 +111,47 @@
         Args:
             use: Flag indicating whether to use AttrDict.
         """
         self.as_attrdict = use
         for key, value in self.__dict__.items():
             if isinstance(value, (AttrDict, dict)):
                 self.__dict__[key] = AttrDict(value, secure=self.secure) if use else dict(value) # type: ignore
+
+    def compose(self, composition: str, **secured_secrets) -> Secure:
+        """
+        Combines multiple secure secrets into a single secure string.
+
+        This method takes a format string and a variable number of keyword arguments,
+        each representing a secure secret. It replaces placeholders in the format string
+        with the original values of the secure secrets and returns a new `Secure` instance
+        containing the combined secret.
+
+        Args:
+            composition: The format string used to combine the secure secrets.
+                This string can contain placeholders in curly braces that correspond to
+                the names of the secure secrets provided as keyword arguments.
+            **secured_secrets: Arbitrary keyword arguments representing the secure secrets.
+                Each keyword should be the name of a secure secret, and its value should
+                be an instance of the `Secure` class.
+
+        Returns:
+            Secure: A new `Secure` instance containing the combined secret.
+
+        Raises:
+            ValueError: If any of the provided keyword arguments is not an instance of `Secure`.
+
+        Example:
+            secured_host = Secure('db-server.local')
+            secured_password = Secure('password123')
+            combined_secure = secured_host.compose("Connection to {host} with password {password}", host=secured_host, password=secured_password)
+            print(combined_secure)  # Output: <Sensitive data secured>
+            print(combined_secure._get_original())  # Output: Connection to db-server.local with password password123
+        """
+        # Create a context with the original values of Secure objects
+        context = {key: value._get_original() if isinstance(value, Secure) else value
+                for key, value in secured_secrets.items()}
+
+        # Replace Secure objects in the format string with their original values
+        composed = composition.format(**context)
+
+        # Return a new Secure instance with the combined secret
+        return Secure(composed, self.message)
```

