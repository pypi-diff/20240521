# Comparing `tmp/pih-gateway-0.11.tar.gz` & `tmp/pih-gateway-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-gateway-0.11.tar", last modified: Wed Apr 10 01:42:22 2024, max compression
+gzip compressed data, was "pih-gateway-0.13.tar", last modified: Tue May 21 19:33:03 2024, max compression
```

## Comparing `pih-gateway-0.11.tar` & `pih-gateway-0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:42:22.443123 pih-gateway-0.11/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:42:22.011056 pih-gateway-0.11/GatewayService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-gateway-0.11/GatewayService/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-08 23:28:10.000000 pih-gateway-0.11/GatewayService/__main__.py
--rw-rw-rw-   0        0        0      735 2023-12-28 01:43:14.000000 pih-gateway-0.11/GatewayService/collection.py
--rw-rw-rw-   0        0        0      531 2024-04-10 00:27:07.000000 pih-gateway-0.11/GatewayService/const.py
--rw-rw-rw-   0        0        0     8627 2024-04-09 03:05:30.000000 pih-gateway-0.11/GatewayService/service.py
--rw-rw-rw-   0        0        0      354 2024-04-10 01:42:22.411850 pih-gateway-0.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:42:22.362889 pih-gateway-0.11/pih_gateway.egg-info/
--rw-rw-rw-   0        0        0      354 2024-04-10 01:42:21.000000 pih-gateway-0.11/pih_gateway.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2024-04-10 01:42:21.000000 pih-gateway-0.11/pih_gateway.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:42:21.000000 pih-gateway-0.11/pih_gateway.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-10 01:42:21.000000 pih-gateway-0.11/pih_gateway.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-04-10 01:42:21.000000 pih-gateway-0.11/pih_gateway.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 01:42:21.000000 pih-gateway-0.11/pih_gateway.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:42:22.458750 pih-gateway-0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 19:33:03.835732 pih-gateway-0.13/
+drwxrwxrwx   0        0        0        0 2024-05-21 19:33:03.253531 pih-gateway-0.13/GatewayService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-gateway-0.13/GatewayService/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-08 23:28:10.000000 pih-gateway-0.13/GatewayService/__main__.py
+-rw-rw-rw-   0        0        0      735 2023-12-28 01:43:14.000000 pih-gateway-0.13/GatewayService/collection.py
+-rw-rw-rw-   0        0        0      560 2024-05-21 19:32:47.000000 pih-gateway-0.13/GatewayService/const.py
+-rw-rw-rw-   0        0        0    11348 2024-05-21 00:09:04.000000 pih-gateway-0.13/GatewayService/service.py
+-rw-rw-rw-   0        0        0      354 2024-05-21 19:33:03.803891 pih-gateway-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 19:33:03.772659 pih-gateway-0.13/pih_gateway.egg-info/
+-rw-rw-rw-   0        0        0      354 2024-05-21 19:33:02.000000 pih-gateway-0.13/pih_gateway.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-21 19:33:03.000000 pih-gateway-0.13/pih_gateway.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:33:02.000000 pih-gateway-0.13/pih_gateway.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-21 19:33:02.000000 pih-gateway-0.13/pih_gateway.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-05-21 19:33:02.000000 pih-gateway-0.13/pih_gateway.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 19:33:02.000000 pih-gateway-0.13/pih_gateway.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:33:03.851371 pih-gateway-0.13/setup.cfg
```

### Comparing `pih-gateway-0.11/GatewayService/collection.py` & `pih-gateway-0.13/GatewayService/collection.py`

 * *Files identical despite different names*

### Comparing `pih-gateway-0.11/GatewayService/const.py` & `pih-gateway-0.13/GatewayService/const.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from pih.collections.service import ServiceDescription
 from pih.consts.hosts import Hosts
 
 NAME: str = "Gateway"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.11"
+VERSION: str = "0.13"
 
 PACKAGES: tuple[str, ...] = ("fastapi", "uvicorn")
 
+ALISA_TIMEOUT: int = 4100
+
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Whatsapp message and Alisa command gateway service",
     host=HOST.NAME,
     host_changeable=False,
     version=VERSION,
     standalone_name="gateway",
```

### Comparing `pih-gateway-0.11/GatewayService/service.py` & `pih-gateway-0.13/GatewayService/service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 import ipih
 
-from pih import A, PIHThread
-from GatewayService.const import SD
+from pih import A, PIHThread, strdict
+from GatewayService.const import SD, ALISA_TIMEOUT
+
+from typing import Any
+from time import time_ns
+from collections import defaultdict
+
 
 SC = A.CT_SC
 
+SD.host_changeable = True
+
 ISOLATED: bool = False
 
+message_list_holder: dict[str, list[strdict]] = defaultdict(list)
+message_list_break: dict[str, bool] = {}
+
+
+class DH:
+    current_time: float = 0.0
+
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
 
         from GatewayService.collection import WappiRawMessage
-        from pih.tools import j, js, ne, e, nl, esc, lw, nns, nnl
         from pih.collections import WhatsAppMessage, BarcodeInformation
+        from pih.tools import j, js, ne, e, nl, esc, lw, jnl, nns, nnl, ParameterList
 
         from fastapi import FastAPI, Body, Request
         from fastapi.responses import HTMLResponse
         import uvicorn
 
         fast_api = FastAPI()
 
@@ -27,15 +41,58 @@
             version: str = A.V.value
             return HTMLResponse(
                 js((nl(nns(SD.description), normal=False), "Version:", version))
             )
 
         @fast_api.post("/alisa_gateway")
         def alisa_command_receive_handler(request: Request, message_body=Body(...)):
-            command: str = message_body["request"]["command"]
+            message: strdict = message_body["request"]
+
+            command: str = str(
+                message["payload"]
+                if "type" in message and message["type"] == "ButtonPressed"
+                else js(message["nlu"]["tokens"]) or "pih"
+            )
+            DH.current_time = time_ns()
+            recipient: str = A.D_TN.by_login("nak")
+            message_list_holder[recipient] = []
+            message_list_break[recipient] = False
+            A.A_MIO.send_outside(command, recipient)
+            while not message_list_break[recipient]:
+                if (time_ns() - DH.current_time) // 1_000_000 > ALISA_TIMEOUT:
+                    return {"text": "Долго"}
+            message_list: list[strdict] = message_list_holder[recipient]
+            text: str = jnl(
+                A.D.map(
+                    A.D_F.as_plain_message,
+                    A.D.map(
+                        lambda item: item["value"],
+                        A.D.filter(
+                            lambda item: item["type"] != "index_item",
+                            message_list,
+                        ),
+                    ),
+                )
+            )
+            result: strdict = {"text": text}
+            buttons: list[strdict] = A.D.filter(
+                lambda item: item["type"] == "index_item",
+                message_list,
+            )
+            if ne(buttons):
+                result["buttons"] = A.D.map(
+                    lambda item: {
+                        "title": A.D_F.as_plain_message(item["text"]),
+                        "payload": item["value"],
+                        "hide": True,
+                    },
+                    A.D.sort(lambda item: item["value"], buttons),
+                )
+
+            return result
 
         @fast_api.post("/message_gateway")
         def wappi_whatsapp_message_receive_handler(
             request: Request, message_body=Body(...)
         ):
             wh_type: str = message_body["wh_type"]
             if wh_type == "incoming_message":
@@ -155,17 +212,31 @@
         def service_starts_handler() -> None:
             A.SYS.kill_process_by_port(A.CT_PORT.HTTP)
             PIHThread(run_fastapi_server)
 
         def run_fastapi_server() -> None:
             uvicorn.run(fast_api, host="0.0.0.0", port=A.CT_PORT.HTTP)
 
+        def listener(pl: ParameterList) -> None:
+            message_list: list[strdict] = A.D.rpc_decode(pl.next())
+            for message in message_list:
+                recipient: str = message["recipient"]
+                message_type: str = message["type"]
+                message_list_holder[recipient].append(message)
+                message_list_break[recipient] = message_type == "break"
+            print("time", (time_ns() - DH.current_time) // 1_000_000)
+
+        def service_call_handler(sc: SC, pl: ParameterList) -> Any:
+            if sc == SC.serve_command:
+                listener(pl)
+
         A.SRV_A.serve(
             SD,
-            starts_handler=service_starts_handler,  # type: ignore
+            service_call_handler,
+            service_starts_handler,  # type: ignore
             isolate=ISOLATED,
             as_standalone=as_standalone,
         )
 
 
 if __name__ == "__main__":
     start()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

