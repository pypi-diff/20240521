# Comparing `tmp/fastapi_keycloak_middleware-0.4.2.tar.gz` & `tmp/fastapi_keycloak_middleware-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_keycloak_middleware-0.4.2.tar", max compression
+gzip compressed data, was "fastapi_keycloak_middleware-1.0.1.tar", max compression
```

## Comparing `fastapi_keycloak_middleware-0.4.2.tar` & `fastapi_keycloak_middleware-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1063 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/LICENSE
--rw-r--r--   0        0        0     4422 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/README.md
--rw-r--r--   0        0        0     1481 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/__init__.py
--rw-r--r--   0        0        0     5058 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/require_permission.py
--rw-r--r--   0        0        0      856 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/strip_request.py
--rw-r--r--   0        0        0      352 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/dependencies/__init__.py
--rw-r--r--   0        0        0      467 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
--rw-r--r--   0        0        0      420 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/dependencies/get_user.py
--rw-r--r--   0        0        0      703 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/exceptions.py
--rw-r--r--   0        0        0     1042 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/fast_api_user.py
--rw-r--r--   0        0        0     7932 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/keycloak_backend.py
--rw-r--r--   0        0        0     8195 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/middleware.py
--rw-r--r--   0        0        0        0 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/__init__.py
--rw-r--r--   0        0        0      523 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_methods.py
--rw-r--r--   0        0        0     1257 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_result.py
--rw-r--r--   0        0        0      232 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/exception_response.py
--rw-r--r--   0        0        0     7178 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
--rw-r--r--   0        0        0      581 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/match_strategy.py
--rw-r--r--   0        0        0     5761 2024-05-18 10:18:49.381028 fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/setup.py
--rw-r--r--   0        0        0     1618 2024-05-18 10:18:49.385028 fastapi_keycloak_middleware-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5393 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.2/setup.py
--rw-r--r--   0        0        0     4970 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4422 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/README.md
+-rw-r--r--   0        0        0     1481 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/decorators/__init__.py
+-rw-r--r--   0        0        0     5058 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/decorators/require_permission.py
+-rw-r--r--   0        0        0      856 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/decorators/strip_request.py
+-rw-r--r--   0        0        0      352 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/dependencies/__init__.py
+-rw-r--r--   0        0        0      467 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/dependencies/get_authorization_result.py
+-rw-r--r--   0        0        0      420 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/dependencies/get_user.py
+-rw-r--r--   0        0        0      612 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/exceptions.py
+-rw-r--r--   0        0        0     1042 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/fast_api_user.py
+-rw-r--r--   0        0        0     7090 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/keycloak_backend.py
+-rw-r--r--   0        0        0     7330 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/authorization_methods.py
+-rw-r--r--   0        0        0     1257 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/authorization_result.py
+-rw-r--r--   0        0        0      232 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/exception_response.py
+-rw-r--r--   0        0        0     7478 2024-05-21 08:53:25.295151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py
+-rw-r--r--   0        0        0      581 2024-05-21 08:53:25.299151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/match_strategy.py
+-rw-r--r--   0        0        0     5761 2024-05-21 08:53:25.299151 fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/setup.py
+-rw-r--r--   0        0        0     1594 2024-05-21 08:53:25.299151 fastapi_keycloak_middleware-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-1.0.1/setup.py
+-rw-r--r--   0        0        0     4933 1970-01-01 00:00:00.000000 fastapi_keycloak_middleware-1.0.1/PKG-INFO
```

### Comparing `fastapi_keycloak_middleware-0.4.2/LICENSE` & `fastapi_keycloak_middleware-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/README.md` & `fastapi_keycloak_middleware-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/__init__.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Middleware for FastAPI that supports authenticating users against Keycloak
 """
 
-__version__ = "0.4.2"
+__version__ = "1.0.1"
 
 import logging
 
 from fastapi_keycloak_middleware.decorators.require_permission import require_permission
 from fastapi_keycloak_middleware.decorators.strip_request import strip_request
 from fastapi_keycloak_middleware.dependencies.get_authorization_result import (
     get_authorization_result,
```

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/require_permission.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/decorators/require_permission.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/decorators/strip_request.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/decorators/strip_request.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/fast_api_user.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/fast_api_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/keycloak_backend.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/keycloak_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 It is used by the middleware to perform the actual authentication.
 """
 
 import logging
 import typing
 
 import keycloak
-from jose import ExpiredSignatureError, JWTError
-from jose.exceptions import JWTClaimsError
 from keycloak import KeycloakOpenID
-from starlette.authentication import AuthCredentials, AuthenticationBackend, BaseUser
+from starlette.authentication import AuthenticationBackend, BaseUser
 from starlette.requests import HTTPConnection
 
 from fastapi_keycloak_middleware.exceptions import (
     AuthClaimMissing,
     AuthHeaderMissing,
     AuthInvalidToken,
     AuthKeycloakError,
-    AuthTokenExpired,
     AuthUserError,
 )
 from fastapi_keycloak_middleware.fast_api_user import FastApiUser
 from fastapi_keycloak_middleware.schemas.authorization_methods import (
     AuthorizationMethod,
 )
 from fastapi_keycloak_middleware.schemas.keycloak_configuration import (
@@ -40,55 +37,46 @@
 
     def __init__(
         self,
         keycloak_configuration: KeycloakConfiguration,
         user_mapper: typing.Callable[[typing.Dict[str, typing.Any]], typing.Awaitable[typing.Any]],
     ):
         self.keycloak_configuration = keycloak_configuration
-        self.keycloak_openid = self._get_keycloak_openid(keycloak_configuration)
-        self.get_user = user_mapper if user_mapper else self._get_user
+        self.keycloak_openid = self._get_keycloak_openid()
+        self.get_user = user_mapper if user_mapper else KeycloakBackend._get_user
 
-        # Fetch KC public key if needed
-        if not keycloak_configuration.use_introspection_endpoint:
-            self.keycloak_public_key = (
-                "-----BEGIN PUBLIC KEY-----\n"
-                + self.keycloak_openid.public_key()
-                + "\n-----END PUBLIC KEY-----"
-            )
-
-    def _get_keycloak_openid(self, keycloak_configuration: KeycloakConfiguration) -> KeycloakOpenID:
+    def _get_keycloak_openid(self) -> KeycloakOpenID:
         """
         Instance-scoped KeycloakOpenID object
         """
         return KeycloakOpenID(
             server_url=self.keycloak_configuration.url,
             client_id=self.keycloak_configuration.client_id,
             realm_name=self.keycloak_configuration.realm,
             client_secret_key=self.keycloak_configuration.client_secret,
             verify=self.keycloak_configuration.verify,
         )
 
-    async def _get_user(self, userinfo: typing.Dict[str, typing.Any]) -> BaseUser:
+    @staticmethod
+    async def _get_user(userinfo: typing.Dict[str, typing.Any]) -> BaseUser:
         """
         Default implementation of the get_user method.
         """
         return FastApiUser(
             first_name=userinfo.get("given_name", ""),
             last_name=userinfo.get("family_name", ""),
             user_id=userinfo.get("user_id", ""),
         )
 
-    async def authenticate(self, conn: HTTPConnection) -> tuple[AuthCredentials, BaseUser | None]:
+    async def authenticate(self, conn: HTTPConnection) -> tuple[list[str], BaseUser | None]:
         """
         The authenticate method is invoked each time a route is called that
         the middleware is applied to.
         """
 
-        auth_header = None
-
         # If this is a websocket connection, we can extract the token
         # from the cookies
         if (
             self.keycloak_configuration.enable_websocket_support
             and conn.headers.get("upgrade") == "websocket"
         ):
             auth_header = conn.cookies.get(self.keycloak_configuration.websocket_cookie_name, None)
@@ -99,40 +87,31 @@
             raise AuthHeaderMissing
 
         # Check if token starts with the authentication scheme
         token = auth_header.split(" ")
         if len(token) != 2 or token[0] != self.keycloak_configuration.authentication_scheme:
             raise AuthInvalidToken
 
-        token_info = None
-
         # Depending on the chosen method by the user, either
         # use the introspection endpoint or decode the token
         if self.keycloak_configuration.use_introspection_endpoint:
             log.debug("Using introspection endpoint to validate token")
             # Call introspect endpoint to check if token is valid
             try:
                 token_info = self.keycloak_openid.introspect(token[1])
             except keycloak.exceptions.KeycloakPostError as exc:
                 raise AuthKeycloakError from exc
         else:
             log.debug("Using keycloak public key to validate token")
             # Decode Token locally using the public key
-            try:
-                token_info = self.keycloak_openid.decode_token(
-                    token[1],
-                    key=self.keycloak_public_key,
-                    options=self.keycloak_configuration.decode_options,
-                )
-            except ExpiredSignatureError as exc:
-                raise AuthTokenExpired from exc
-            except JWTClaimsError as exc:
-                raise AuthClaimMissing from exc
-            except JWTError as exc:
-                raise AuthInvalidToken from exc
+            token_info = self.keycloak_openid.decode_token(
+                token[1],
+                self.keycloak_configuration.validate_token,
+                **self.keycloak_configuration.validation_options,
+            )
 
         # Calculate claims to extract
         # Default is user configured claims
         claims = self.keycloak_configuration.claims
         # If device auth is enabled + device claim is present...
         if (
             self.keycloak_configuration.enable_device_authentication
```

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/middleware.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 here: https://github.com/code-specialist/fastapi-auth-middleware
 """
 
 import logging
 import re
 import typing
 
+from jwcrypto.common import JWException
 from starlette.requests import HTTPConnection
 from starlette.responses import JSONResponse
 from starlette.types import ASGIApp, Receive, Scope, Send
 
 from fastapi_keycloak_middleware.exceptions import (
     AuthHeaderMissing,
     AuthInvalidToken,
-    AuthTokenExpired,
     AuthUserError,
 )
 from fastapi_keycloak_middleware.keycloak_backend import KeycloakBackend
 from fastapi_keycloak_middleware.schemas.keycloak_configuration import (
     KeycloakConfiguration,
 )
 
@@ -140,77 +140,52 @@
             if self.scope_mapper:
                 log.debug("Calling user provided scope mapper")
                 auth = await self.scope_mapper(auth)
 
             scope["auth"], scope["user"] = auth, user
 
         except AuthHeaderMissing:  # Request has no 'Authorization' HTTP Header
-            response = self._auth_header_missing()
+            response = JSONResponse(
+                {"detail": "Your request is missing an 'Authorization' HTTP header"},
+                status_code=401,
+            )
             log.warning("Request is missing an 'Authorization' HTTP header")
             await response(scope, receive, send)
             return
 
-        except AuthTokenExpired:  # Token has expired
-            response = self._token_has_expired()
-            log.warning("Provided token has expired")
-            await response(scope, receive, send)
-            return
-
         except AuthUserError:
-            response = self._user_not_found()
+            response = JSONResponse(
+                {"detail": "Could not find a user based on this token"}, status_code=401
+            )
             log.warning("Could not find a user based on the provided token")
             await response(scope, receive, send)
             return
 
         except AuthInvalidToken:
-            response = self._invalid_token()
+            response = JSONResponse(
+                {"detail": "Unable to verify provided access token"}, status_code=401
+            )
             log.warning("Provided access token could not be validated")
             await response(scope, receive, send)
             return
 
+        except JWException as exc:
+            response = JSONResponse(
+                {"detail": f"Error while validating access token: {exc}"},
+                status_code=401,
+            )
+            log.warning("An error occurred while validating the token")
+            await response(scope, receive, send)
+            return
+
         except Exception as exc:  # pylint: disable=broad-except
             response = JSONResponse(
                 {"detail": f"An error occurred: {exc.__class__.__name__}"},
                 status_code=401,
             )
             log.error("An error occurred while authenticating the user")
+            log.exception(exc)
             await response(scope, receive, send)
             return
 
         log.debug("Sending request to next middleware")
         await self.app(scope, receive, send)  # Token is valid
-
-    @staticmethod
-    def _auth_header_missing(*args, **kwargs):  # pylint: disable=unused-argument
-        """
-        Returns a response notifying the user that the request
-        is missing an 'Authorization' HTTP header.
-        """
-        return JSONResponse(
-            {"detail": "Your request is missing an 'Authorization' HTTP header"},
-            status_code=401,
-        )
-
-    @staticmethod
-    def _token_has_expired(*args, **kwargs):  # pylint: disable=unused-argument
-        """
-        Returns a response notifying the user that the token has expired.
-        """
-        return JSONResponse(
-            {"detail": "Your 'Authorization' HTTP header is invalid"}, status_code=401
-        )
-
-    @staticmethod
-    def _user_not_found(*args, **kwargs):  # pylint: disable=unused-argument
-        """
-        Returns a response notifying the user that the user was not found.
-        """
-        return JSONResponse(
-            {"detail": "Could not find a user based on this token"}, status_code=401
-        )
-
-    @staticmethod
-    def _invalid_token(*args, **kwargs):  # pylint: disable=unused-argument
-        """
-        Returns a response notifying the user that the acess token is invalid.
-        """
-        return JSONResponse({"detail": "Unable to verify provided access token"}, status_code=401)
```

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_methods.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/authorization_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/authorization_result.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/authorization_result.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/keycloak_configuration.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/keycloak_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module contains the schema to configure Keycloak.
 """
 
 from typing import Optional, Union
 
+from jwcrypto import jwk
 from pydantic import BaseModel, Field
 
 from fastapi_keycloak_middleware.schemas.authorization_methods import (
     AuthorizationMethod,
 )
 
 
@@ -54,20 +55,21 @@
     :param device_authentication_claim: This claim will be used to check if the token
         is a device token. Defaults to ``is_device``. This is only used if
         ``enable_device_authentication`` is set to ``True``. The value
         is extracted from the claim and checked if its a truthy value.
         To be specific, ``bool(value)`` must evaluate to ``True``.
     :param verify: Whether to verify SSL connection. Defaults to ``True``
     :type verify: Union[bool,str], optional
-    :param decode_options: Defines options to be passed to `python-jose`'s `decode``
-        function. Defaults to ``{"verify_signature": True, "verify_aud": True,
-        "verify_exp": True}``. See the following project for an overview of
-        acceptable options:
-        https://github.com/mpdavis/python-jose/blob/4b0701b46a8d00988afcc5168c2b3a1fd60d15d8/jose/jwt.py#L81
-    :type decode_options: Dict[str, Union[bool,int]], optional
+    :param validate_token: Whether to validate the token. Defaults to ``True``.
+    :type validate_token: bool, optional
+    :param validation_options: Decode options that are passed to `JWCrypto`'s JWT
+        constructor. Defaults to ``{}``. See the following project for an overview of
+        acceptable options: https://jwcrypto.readthedocs.io/en/latest/jwt.html
+    :type validation_options: dict[str, Union[str, dict[str, Union[None, str]], list[str]]],
+        optional
     :param enable_websocket_support: Whether to enable WebSocket support. Defaults to ``True``.
     :type enable_websocket_support: bool, optional
     :param websocket_cookie_name: Name of the cookie that contains the access token.
         Defaults to ``access_token``.
     :type websocket_cookie_name: str, optional
     """
 
@@ -132,26 +134,35 @@
         " true, the device authentication will be applied for the request.",
     )
     verify: Union[bool, str] = Field(
         default=True,
         title="Verify",
         description="Whether to verify the SSL connection",
     )
-    decode_options: dict[str, Union[bool, int]] = Field(
-        default={
-            "verify_signature": True,
-            "verify_aud": True,
-            "verify_exp": True,
-        },
-        title="JWT Decode Options",
-        description="Decode options that are passed to python-jose decode function.",
+    validate_token: bool = Field(
+        default=True,
+        title="Validate Token",
+        description="Whether to validate the token.",
+    )
+    validation_options: dict[
+        str, Union[str, dict[str, Union[None, str]], list[str], jwk.JWK, jwk.JWKSet]
+    ] = Field(
+        default={},
+        title="JWCrypto JWT Options",
+        description="Decode options that are passed to jwcrypto's JWT constructor.",
+        skip_validation=True,
     )
     enable_websocket_support: bool = Field(
         default=True,
         title="Enable WebSocket Support",
         description="if enabled, websocket connections are also checked for valid tokens.",
     )
     websocket_cookie_name: str = Field(
         default="access_token",
         title="WebSocket Cookie Name",
         description="The name of the cookie that contains the access token.",
     )
+
+    class Config:
+        """Pydantic configuration"""
+
+        arbitrary_types_allowed = True
```

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/schemas/match_strategy.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/schemas/match_strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/fastapi_keycloak_middleware/setup.py` & `fastapi_keycloak_middleware-1.0.1/fastapi_keycloak_middleware/setup.py`

 * *Files identical despite different names*

### Comparing `fastapi_keycloak_middleware-0.4.2/pyproject.toml` & `fastapi_keycloak_middleware-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "fastapi-keycloak-middleware"
-version = "0.4.2"
+version = "1.0.1"
 description = "Middleware for FastAPI to authenticate a user against keycloak"
 authors = ["Daniel Herrmann <daniel.herrmann1@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "fastapi_keycloak_middleware" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = ">=0.73.0"
-python-keycloak = ">2.14.0,<3.9.1"
-ruff = "^0.4.2"
+python-keycloak = "^4.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
-ruff = "^0.4.0"
 ruff-lsp = "^0.0.53"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py310"
```

### Comparing `fastapi_keycloak_middleware-0.4.2/setup.py` & `fastapi_keycloak_middleware-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,19 @@
  'fastapi_keycloak_middleware.dependencies',
  'fastapi_keycloak_middleware.schemas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.73.0', 'python-keycloak>2.14.0,<3.9.1', 'ruff>=0.4.2,<0.5.0']
+['fastapi>=0.73.0', 'python-keycloak>=4.0.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-keycloak-middleware',
-    'version': '0.4.2',
+    'version': '1.0.1',
     'description': 'Middleware for FastAPI to authenticate a user against keycloak',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)\n[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)\n![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)\n![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/waza-ari/fastapi-keycloak-middleware/development.svg)](https://results.pre-commit.ci/latest/github/waza-ari/fastapi-keycloak-middleware/development)\n\n\n# FastAPI Keycloak Middleware\n\n**Full documentation** is [available at Read The Docs](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/)\n\nThis package provides a middleware for [FastAPI](http://fastapi.tiangolo.com)  that\nsimplifies integrating with [Keycloak](http://keycloak.org) for\nauthentication and authorization. It supports OIDC and supports validating access\ntokens, reading roles and basic authentication. In addition it provides several\ndecorators and dependencies to easily integrate into your FastAPI application.\n\nIt relies on the [python-keycloak](http://python-keycloak.readthedocs.io) package,\nwhich is the only dependency outside of the FastAPI ecosystem which would be installed\nanyway. Shoutout to the author of [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich served as inspiration for this package and some of its code.\n\nIn the future, I plan to add support for fine grained authorization using Keycloak\nAuthorization services.\n\n## Motivation\n\nUsing FastAPI and Keycloak quite a lot, and keeping to repeat myself quite a lot when\nit comes to authentiating users, I decided to create this library to help with this.\n\nThere is a clear separation between the authentication and authorization:\n\n- **Authentication** is about verifying the identity of the user\n  (who they are). This is done by an authentication backend\n  that verifies the users access token obtained from the\n  identity provider (Keycloak in this case).\n- **Authorization** is about deciding which resources can be\n  accessed. This package providers convenience decoraters to\n  enforce certain roles or permissions on FastAPI endpoints.\n\n## Installation\n\nInstall the package using poetry:\n\n```bash\npoetry add fastapi-keycloak-middleware\n```\n\nor `pip`:\n\n```bash\npip install fastapi-keycloak-middleware\n```\n\n## Features\n\nThe package helps with:\n\n* An easy to use middleware that validates the request for an access token\n* Validation can done in one of two ways:\n   * Validate locally using the public key obtained from Keycloak\n   * Validate using the Keycloak token introspection endpoint\n* Using Starlette authentication mechanisms to store both the user object as well as the authorization scopes in the Request object\n* Ability to provide custom callback functions to retrieve the user object (e.g. from your database) and to provide an arbitrary mapping to authentication scopes (e.g. roles to permissions)\n* A decorator to use previously stored information to enforce certain roles or permissions on FastAPI endpoints\n* Convenience dependencies to retrieve the user object or the authorization result after evaluation within the FastAPI endpoint\n\n## Acknowledgements\n\nThis package is heavily inspired by [fastapi-auth-middleware](https://github.com/code-specialist/fastapi-auth-middleware)\nwhich provides some of the same functionality but without the direct integration\ninto Keycloak. Thanks for writing and providing this great piece of software!\n\n## Contributing\n\nThe client is written in pure Python.\nAny changes or pull requests are more than welcome, but please adhere to the code style.\n\nRuff is used both for code formatting and linting. Before committing, please run the following command to ensure\nthat your code is properly formatted:\n\n```bash\nruff check .\nruff format .\n```\n\nA pre-commit hook configuration is supplied as part of the project.\n\n## Development\n\nThis project is using [Act](https://github.com/nektos/act) to handle local development tasks. It is used\nto work locally and also to test Github actions before deploying them.\n',
     'author': 'Daniel Herrmann',
     'author_email': 'daniel.herrmann1@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fastapi_keycloak_middleware-0.4.2/PKG-INFO` & `fastapi_keycloak_middleware-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-keycloak-middleware
-Version: 0.4.2
+Version: 1.0.1
 Summary: Middleware for FastAPI to authenticate a user against keycloak
 Author: Daniel Herrmann
 Author-email: daniel.herrmann1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.73.0)
-Requires-Dist: python-keycloak (>2.14.0,<3.9.1)
-Requires-Dist: ruff (>=0.4.2,<0.5.0)
+Requires-Dist: python-keycloak (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/fastapi-keycloak-middleware/badge/?version=latest)](https://fastapi-keycloak-middleware.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 ![GitHub issues](https://img.shields.io/github/issues/waza-ari/fastapi-keycloak-middleware)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/waza-ari/fastapi-keycloak-middleware)
 ![GitHub top language](https://img.shields.io/github/languages/top/waza-ari/fastapi-keycloak-middleware)
```

