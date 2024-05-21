# Comparing `tmp/RTS_Tunnel-0.3.tar.gz` & `tmp/RTS_Tunnel-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS_Tunnel-0.3.tar", last modified: Mon May 13 18:57:52 2024, max compression
+gzip compressed data, was "RTS_Tunnel-0.4.tar", last modified: Tue May 21 14:52:56 2024, max compression
```

## Comparing `RTS_Tunnel-0.3.tar` & `RTS_Tunnel-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 18:57:52.333748 RTS_Tunnel-0.3/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_Tunnel-0.3/LICENCE
--rw-rw-rw-   0        0        0      716 2024-05-13 18:57:52.332729 RTS_Tunnel-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-05-13 18:35:24.000000 RTS_Tunnel-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 18:57:52.314860 RTS_Tunnel-0.3/RTS_Remotetummelsystem/
--rw-rw-rw-   0        0        0        0 2024-05-13 18:57:34.000000 RTS_Tunnel-0.3/RTS_Remotetummelsystem/__init__.py
--rw-rw-rw-   0        0        0     5961 2024-05-13 18:45:45.000000 RTS_Tunnel-0.3/RTS_Remotetummelsystem/client.py
--rw-rw-rw-   0        0        0     8509 2024-05-13 18:52:26.000000 RTS_Tunnel-0.3/RTS_Remotetummelsystem/server.py
--rw-rw-rw-   0        0        0      562 2024-05-13 18:36:47.000000 RTS_Tunnel-0.3/RTS_Remotetummelsystem/snowflake.py
-drwxrwxrwx   0        0        0        0 2024-05-13 18:57:52.331690 RTS_Tunnel-0.3/RTS_Tunnel.egg-info/
--rw-rw-rw-   0        0        0      716 2024-05-13 18:57:52.000000 RTS_Tunnel-0.3/RTS_Tunnel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-05-13 18:57:52.000000 RTS_Tunnel-0.3/RTS_Tunnel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 18:57:52.000000 RTS_Tunnel-0.3/RTS_Tunnel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 18:57:52.000000 RTS_Tunnel-0.3/RTS_Tunnel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-13 18:57:52.000000 RTS_Tunnel-0.3/RTS_Tunnel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 18:57:52.333748 RTS_Tunnel-0.3/setup.cfg
--rw-rw-rw-   0        0        0      894 2024-05-13 18:57:48.000000 RTS_Tunnel-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:52:56.678417 RTS_Tunnel-0.4/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_Tunnel-0.4/LICENCE
+-rw-rw-rw-   0        0        0      716 2024-05-21 14:52:56.678417 RTS_Tunnel-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-05-13 18:35:24.000000 RTS_Tunnel-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:52:56.664331 RTS_Tunnel-0.4/RTS_Remotetummelsystem/
+-rw-rw-rw-   0        0        0        0 2024-05-13 18:57:34.000000 RTS_Tunnel-0.4/RTS_Remotetummelsystem/__init__.py
+-rw-rw-rw-   0        0        0     7647 2024-05-21 14:52:28.000000 RTS_Tunnel-0.4/RTS_Remotetummelsystem/client.py
+-rw-rw-rw-   0        0        0     8581 2024-05-21 14:52:07.000000 RTS_Tunnel-0.4/RTS_Remotetummelsystem/server.py
+-rw-rw-rw-   0        0        0      562 2024-05-13 18:36:47.000000 RTS_Tunnel-0.4/RTS_Remotetummelsystem/snowflake.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:52:56.676909 RTS_Tunnel-0.4/RTS_Tunnel.egg-info/
+-rw-rw-rw-   0        0        0      716 2024-05-21 14:52:56.000000 RTS_Tunnel-0.4/RTS_Tunnel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-05-21 14:52:56.000000 RTS_Tunnel-0.4/RTS_Tunnel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:52:56.000000 RTS_Tunnel-0.4/RTS_Tunnel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-21 14:52:56.000000 RTS_Tunnel-0.4/RTS_Tunnel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-21 14:52:56.000000 RTS_Tunnel-0.4/RTS_Tunnel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:52:56.679489 RTS_Tunnel-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      910 2024-05-18 08:26:36.000000 RTS_Tunnel-0.4/setup.py
```

### Comparing `RTS_Tunnel-0.3/LICENCE` & `RTS_Tunnel-0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS_Tunnel-0.3/PKG-INFO` & `RTS_Tunnel-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS_Tunnel
-Version: 0.3
+Version: 0.4
 Summary: Work in progress, a tunneling system for RTS_DataBase.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTS_Tunnel-0.3/RTS_Remotetummelsystem/server.py` & `RTS_Tunnel-0.4/RTS_Remotetummelsystem/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 import re
 import sys
 import logging
 import ssl
 from scapy.all import Raw
 from snowflake import Snowflake
 from ExtraUtils import RateLimiter
-import ExtraUtils.asyncTokens as asyncToken
+import ExtraUtils.timeBasedToken as tbt
 logging.basicConfig(level=logging.DEBUG,filename="server.log",format="%(asctime)s - %(levelname)s - %(message)s")
 
 
 class Server:
-    def __init__(self, host, port, token,use_ssl=False, ssl_cert=None, ssl_key=None):
+    def __init__(self, host, port, token,use_ssl=False, ssl_cert=None, ssl_key=None, primary= None,special=None):
+        if not primary or not special:
+            raise ValueError("Primary or special not set")
         self.node = None
         self.host = host
         self.port = port
         self.token = token
         self.blocked_ips = set()
         self.ports_in_q = set()
         self.active = []
         self.active_requests = 0
+        self.TBT = tbt.TimeBasedToken(primary,special)
         self.ratelimit = RateLimiter(40,50,1,1)
         self.ssl_ports = [443,465,563,636,989,990,992,993,994,995,5061,8443,8531,9443,1194,1443,1443,18443,2443,4443,5443]
         self.prohibited_ports= [0,22,8888]
+        self.__recieved_goodbye = False
 
-        
-        self.key, self.pub = asyncToken.gen_keypair()
-        self.other_pub = None
         self.use_ssl = use_ssl
         if self.use_ssl:
             self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
             #self.ssl_context.options &= ~ssl.OP_NO_SSLv3 & ~ssl.OP_NO_TLSv1 & ~ssl.OP_NO_TLSv1_1
             self.ssl_context.load_cert_chain(certfile=ssl_cert, keyfile=ssl_key)
         else:
             self.ssl_context = None
@@ -45,72 +46,74 @@
         server.bind((self.host, self.port))
         self.active.append(server)
         server.listen(1)
         logging.info(f"Server listening on {self.host}:{self.port}")
 
         while True:
             cli, addr = server.accept()
+
             self.active.append(cli)
 
             if not cli:
                 continue
             self.ratelimit.increment()
             if self.ratelimit.hit:
                 cli.close()
+            
             hello = cli.recv(512)
+            logging.debug(hello)
             ip, port = addr
             if self.node:
                 cli.send(b"RTS_ERROR Connection occupied.")
                 logging.error(f"Connection from {ip}:{port} denied: Occupied_Error")
                 cli.close()
                 continue
             if port != self.port:
                 cli.send(f"RTS_ERROR Invalid connection port, expecting connection from port {self.port}".encode())
                 logging.error(f"Connetion blocked, invalid Port using {ip}:{port}")
                 cli.close()
                 continue
-            if not hello.startswith(b"RTS_HELLO "):
-                cli.send("RTS_ERROR No RTS_HELLO message recieved.".encode())
+            self.TBT.regenerate()
+            hello = self.TBT.decrypt(hello)
+            if not hello.startswith("RTS_HELLO "):
+                answer = self.TBT.encrypt("RTS_ERROR No RTS_HELLO message recieved.")
+                cli.send(answer.encode())
                 logging.error("Did not recieved RTS_HELLO")
                 cli.close()
                 continue
-            hello = hello.decode()
-            message_str = hello.replace("RTS_HELLO ", "")
-            pairs = message_str.split(";;")
-
-            hi = {}
-            for pair in pairs:
-                key, value = pair.split("=")
-                if key in ["ports", "blocked"]:
-                    value = ast.literal_eval(value)
-                hi[key] = value
-            print(hi)
-            #if hi.get("pub"):
-            #    self.other_pub = asyncToken.load(hi.get("pub"))
+            hello = hello[9:]
+
+            hello = hello.split('=')[1]
+            hello = hello.strip('[]')
+            self.ports_in_q = [port.strip('"').strip("'") for port in hello.split(',')] 
 
             self.node = cli
-            self.ports_in_q = hi["ports"]
             logging.info(f"\nAccepted connection from: {ip}:{port}\n")
-            print(self.other_pub)
-            #hello_msg = asyncToken.encrypt(f"RTS_HELLO pub={asyncToken.serial(self.pub)};;",self.other_pub)
-            hello_msg = f"RTS_HELLO pub=None;;"
+            
+            hello_msg = self.TBT.encrypt("RTS_HELLO")
             cli.send(hello_msg.encode())
             self.setup_ports()
             while True:
                 cli.settimeout(None)
                 try:
                     read = cli.recv(1024).decode()
-                    #read = asyncToken.decrypt(read,self.key)
+                    read = self.TBT.decrypt(read)
                 except socket.error as ser:
                     logging.error(ser)
                     cli.close()
                     self.node = None
-                if read.startswith("RTS_GOODBY"):
+                except ValueError as err:
+                    logging.error(err)
+                    cli.close()
+                    self.node = None
                     self.shutdown()
-                    sys.exit(1)
+                if read.startswith("RTS_GOODBYE"):
+                    self.__recieved_goodbye = True
+                    self.shutdown()
+                    break
 
 
     def setup_ports(self):
         if not self.ports_in_q:
             return
         for port in self.ports_in_q:
             if int(port) in self.prohibited_ports:
@@ -144,20 +147,20 @@
                 continue
             
             con.settimeout(5.0)
             
             if int(port) in self.ssl_ports:
                 try:
                     con = self.ssl_context.wrap_socket(con, server_side=True)
-                    #self.node.send(asyncToken.encrypt(f"RTS_PORTREG {port} as SSL",self.other_pub).encode())
-                    self.node.send(f"RTS_PORTREG {port} as SSL".encode())
+                    answ = self.TBT.encrypt("RTS_PORTREG {port} as SSL")
+                    self.node.send(answ.encode())
                 except ssl.SSLError as e:
                     logging.error(f"\n{add} caused an error: {e}\n")
-                    #self.node.send(asyncToken.encrypt(f"RTS_PORTREG {port} as SSL FAILED",self.other_pub).encode())
-                    self.node.send(f"RTS_PORTREG {port} as SSL FAILED".encode())
+                    answ = self.TBT.encrypt("RTS_ERROR {port} expected SSL connection")
+                    self.node.send(answ.encode())
                     con.close()
                     continue
 
             try:
                 data:bytes = con.recv(5120)
             except socket.timeout:
                 logging.warning(f"\n{add} timedout.\n")
@@ -167,23 +170,23 @@
                 continue
             
             data = data.decode()
             pack = Raw(load=data)
             logging.info(f"\n{pack.summary}\n")
 
             snow = Snowflake().generate_id()
-            send_msg = f"RTS_PUSH {port} ID {snow} RECIEVED {data}"
-            #end_msg = asyncToken.encrypt(send_msg,self.other_pub)  
+            send_msg = f"RTS_PUSH {port} ID {snow} RECIEVED {data}" 
+            send_msg = self.TBT.encrypt(send_msg)
             # RTS_RESPONSE {id} RETURNED
             logging.info(f"\n>>>OUTGOING source {add}\n{send_msg}\n")
             self.node.settimeout(5.0)
             self.node.send(send_msg.encode())
             try:
-                ret:bytes = self.node.recv(2048).decode()
-                #ret = asyncToken.decrypt(ret,self.key)
+                ret = self.node.recv(2048).decode()
+                ret = self.TBT.decrypt(ret)
             except socket.timeout:
                 logging.warning("Return message timed out\n")
                 con.close()
                 continue
             except socket.error as err:
                 logging.error(f"ServiceServer error:\n{err}\n")
                 con.close()
@@ -200,28 +203,29 @@
             if i:
                 ident = i.group(1)
             else:
                 raise ValueError("no id")
             kill = 23+len(ident)
             ret:str = ret[kill:]
             logging.info(f"\n>>>OUTGOING\n{ret}\n")
-            con.sendall(ret.encode())
+            if ident == snow:
+                con.sendall(ret.encode())
+
+            if ret.startswith("RTS_END") or ret.startswith("RTS_ERROR"):
+                re_end_ident = r'RTS_END (\d+)'
+                if re.search(re_end_ident,ret).group(1) == snow:
+                    con.close()
+                    continue
+                continue
     
 
 
 
     def shutdown(self):
+        if not self.__recieved_goodbye:
+            goodbye = self.TBT.encrypt("RTS_GOODBYE")
+            self.node.send(goodbye.encode())
         for a in self.active:
             logging.info(f"closing connection {a}")
+            a.shutdown(socket.SHUT_RDWR)
             a.close()
-
-
-# Beispielverwendung
-#try:
-serv = Server('0.0.0.0', 8883, "token",True,"/etc/letsencrypt/live/randomtime.tv/fullchain.pem","/etc/letsencrypt/live/randomtime.tv/privkey.pem")
-serv.start_server()
-#except KeyboardInterrupt:
-#    logging.info("shuting down")
-#    serv.shutdown()
-#except Exception as e:
-#    logging.critical(e)
-#    serv.shutdown()
+            sys.exit(0)
```

### Comparing `RTS_Tunnel-0.3/RTS_Remotetummelsystem/snowflake.py` & `RTS_Tunnel-0.4/RTS_Remotetummelsystem/snowflake.py`

 * *Files identical despite different names*

### Comparing `RTS_Tunnel-0.3/RTS_Tunnel.egg-info/PKG-INFO` & `RTS_Tunnel-0.4/RTS_Tunnel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-Tunnel
-Version: 0.3
+Version: 0.4
 Summary: Work in progress, a tunneling system for RTS_DataBase.
 Home-page: https://github.com/RandomTimeLP/RTS_DataBase/
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: database
 Platform: UNKNOWN
```

### Comparing `RTS_Tunnel-0.3/setup.py` & `RTS_Tunnel-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS_Tunnel',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='Work in progress, a tunneling system for RTS_DataBase.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
@@ -16,9 +16,9 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='database',
-    install_requires=["scapy","extrautilities", ],
+    install_requires=["scapy","extrautilities", "prompt_toolkit"],
 )
```

