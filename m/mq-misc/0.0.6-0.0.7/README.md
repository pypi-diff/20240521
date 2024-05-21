# Comparing `tmp/mq-misc-0.0.6.tar.gz` & `tmp/mq_misc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mq-misc-0.0.6.tar", last modified: Thu Sep 14 13:02:20 2023, max compression
+gzip compressed data, was "mq_misc-0.0.7.tar", last modified: Tue May 21 11:13:09 2024, max compression
```

## Comparing `mq-misc-0.0.6.tar` & `mq_misc-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2023-09-14 13:02:20.110278 mq-misc-0.0.6/
--rw-r--r--   0 gorinenko   (501) staff       (20)    11357 2022-09-30 08:13:25.000000 mq-misc-0.0.6/LICENSE
--rw-r--r--   0 gorinenko   (501) staff       (20)     3470 2023-09-14 13:02:20.109655 mq-misc-0.0.6/PKG-INFO
--rw-r--r--   0 gorinenko   (501) staff       (20)     2632 2023-09-14 12:56:20.000000 mq-misc-0.0.6/README.md
-drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2023-09-14 13:02:20.101661 mq-misc-0.0.6/mq_misc/
--rw-r--r--   0 gorinenko   (501) staff       (20)        0 2022-09-30 08:13:25.000000 mq-misc-0.0.6/mq_misc/__init__.py
--rw-r--r--   0 gorinenko   (501) staff       (20)    11131 2023-09-06 14:06:53.000000 mq-misc-0.0.6/mq_misc/amqp.py
--rw-r--r--   0 gorinenko   (501) staff       (20)       65 2022-09-30 08:13:25.000000 mq-misc-0.0.6/mq_misc/errors.py
-drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2023-09-14 13:02:20.106338 mq-misc-0.0.6/mq_misc/publish/
--rw-r--r--   0 gorinenko   (501) staff       (20)        0 2022-09-30 08:13:25.000000 mq-misc-0.0.6/mq_misc/publish/__init__.py
--rw-r--r--   0 gorinenko   (501) staff       (20)     3790 2023-09-14 13:01:38.000000 mq-misc-0.0.6/mq_misc/publish/__main__.py
-drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2023-09-14 13:02:20.105568 mq-misc-0.0.6/mq_misc.egg-info/
--rw-r--r--   0 gorinenko   (501) staff       (20)     3470 2023-09-14 13:02:20.000000 mq-misc-0.0.6/mq_misc.egg-info/PKG-INFO
--rw-r--r--   0 gorinenko   (501) staff       (20)      309 2023-09-14 13:02:20.000000 mq-misc-0.0.6/mq_misc.egg-info/SOURCES.txt
--rw-r--r--   0 gorinenko   (501) staff       (20)        1 2023-09-14 13:02:20.000000 mq-misc-0.0.6/mq_misc.egg-info/dependency_links.txt
--rw-r--r--   0 gorinenko   (501) staff       (20)      129 2023-09-14 13:02:20.000000 mq-misc-0.0.6/mq_misc.egg-info/requires.txt
--rw-r--r--   0 gorinenko   (501) staff       (20)        8 2023-09-14 13:02:20.000000 mq-misc-0.0.6/mq_misc.egg-info/top_level.txt
--rw-r--r--   0 gorinenko   (501) staff       (20)       38 2023-09-14 13:02:20.110406 mq-misc-0.0.6/setup.cfg
--rw-r--r--   0 gorinenko   (501) staff       (20)     1225 2023-09-14 13:02:18.000000 mq-misc-0.0.6/setup.py
-drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2023-09-14 13:02:20.107194 mq-misc-0.0.6/tests/
--rw-r--r--   0 gorinenko   (501) staff       (20)     2080 2023-09-06 14:10:13.000000 mq-misc-0.0.6/tests/test_amqp.py
+drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2024-05-21 11:13:09.307049 mq_misc-0.0.7/
+-rw-r--r--   0 gorinenko   (501) staff       (20)    11357 2022-09-30 08:13:25.000000 mq_misc-0.0.7/LICENSE
+-rw-r--r--   0 gorinenko   (501) staff       (20)     3542 2024-05-21 11:13:09.306163 mq_misc-0.0.7/PKG-INFO
+-rw-r--r--   0 gorinenko   (501) staff       (20)     2704 2024-05-20 09:00:47.000000 mq_misc-0.0.7/README.md
+drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2024-05-21 11:13:09.296559 mq_misc-0.0.7/mq_misc/
+-rw-r--r--   0 gorinenko   (501) staff       (20)        0 2024-05-20 11:33:56.000000 mq_misc-0.0.7/mq_misc/__init__.py
+-rw-r--r--   0 gorinenko   (501) staff       (20)    13306 2024-05-21 11:11:18.000000 mq_misc-0.0.7/mq_misc/amqp.py
+-rw-r--r--   0 gorinenko   (501) staff       (20)       65 2024-05-20 11:33:56.000000 mq_misc-0.0.7/mq_misc/errors.py
+drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2024-05-21 11:13:09.300443 mq_misc-0.0.7/mq_misc/publish/
+-rw-r--r--   0 gorinenko   (501) staff       (20)        0 2024-05-20 11:33:56.000000 mq_misc-0.0.7/mq_misc/publish/__init__.py
+-rw-r--r--   0 gorinenko   (501) staff       (20)     3800 2024-05-20 11:45:30.000000 mq_misc-0.0.7/mq_misc/publish/__main__.py
+drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2024-05-21 11:13:09.302211 mq_misc-0.0.7/mq_misc.egg-info/
+-rw-r--r--   0 gorinenko   (501) staff       (20)     3542 2024-05-21 11:13:09.000000 mq_misc-0.0.7/mq_misc.egg-info/PKG-INFO
+-rw-r--r--   0 gorinenko   (501) staff       (20)      309 2024-05-21 11:13:09.000000 mq_misc-0.0.7/mq_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 gorinenko   (501) staff       (20)        1 2024-05-21 11:13:09.000000 mq_misc-0.0.7/mq_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 gorinenko   (501) staff       (20)      129 2024-05-21 11:13:09.000000 mq_misc-0.0.7/mq_misc.egg-info/requires.txt
+-rw-r--r--   0 gorinenko   (501) staff       (20)        8 2024-05-21 11:13:09.000000 mq_misc-0.0.7/mq_misc.egg-info/top_level.txt
+-rw-r--r--   0 gorinenko   (501) staff       (20)       38 2024-05-21 11:13:09.307251 mq_misc-0.0.7/setup.cfg
+-rw-r--r--   0 gorinenko   (501) staff       (20)     1225 2024-05-20 11:33:56.000000 mq_misc-0.0.7/setup.py
+drwxr-xr-x   0 gorinenko   (501) staff       (20)        0 2024-05-21 11:13:09.301242 mq_misc-0.0.7/tests/
+-rw-r--r--   0 gorinenko   (501) staff       (20)     2110 2024-05-20 11:45:30.000000 mq_misc-0.0.7/tests/test_amqp.py
```

### Comparing `mq-misc-0.0.6/LICENSE` & `mq_misc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mq-misc-0.0.6/PKG-INFO` & `mq_misc-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mq-misc
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility package for working with rabbitmq
 Author: Anton Gorinenko
 Author-email: anton.gorinenko@gmail.com
 Keywords: python,asyncio,utils,mq,aio_pika,rabbit mq,rabbit
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -78,7 +78,13 @@
                         RMQ_ROUTING_KEY] (default: None)
 
 
 ```
 
 python -m mq_misc.publish --amqp-url "amqp://guest:guest@localhost:5672/" --exchange "exchange_1" --exchange_type "
 topic" --routing_key "log.error" --message-file "message.json"
+
+### Creating release tags
+
+```
+git tag -a 0.0.6 -m "Release 0.0.6"
+```
```

### Comparing `mq-misc-0.0.6/README.md` & `mq_misc-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -53,8 +53,14 @@
                         Routing key for publish message [env var:
                         RMQ_ROUTING_KEY] (default: None)
 
 
 ```
 
 python -m mq_misc.publish --amqp-url "amqp://guest:guest@localhost:5672/" --exchange "exchange_1" --exchange_type "
-topic" --routing_key "log.error" --message-file "message.json"
+topic" --routing_key "log.error" --message-file "message.json"
+
+### Creating release tags
+
+```
+git tag -a 0.0.6 -m "Release 0.0.6"
+```
```

### Comparing `mq-misc-0.0.6/mq_misc/amqp.py` & `mq_misc-0.0.7/mq_misc/amqp.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 import asyncio
 import json
 import logging
 import pprint
 import uuid
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, List
 
 import aio_pika
 from aio_pika import ExchangeType
 
 from mq_misc.errors import AdapterError
 
+DEFAULT_LOGGER = logging.getLogger(__name__)
+
 
 @asynccontextmanager
 async def create_weak_publisher(*args, **kwargs):
     """ Инициализация издателя """
     publisher_obj = Publisher(*args, **kwargs)
     await publisher_obj.create_connection(robust=False)
     try:
@@ -42,112 +44,130 @@
     Декодирование сообщения
     """
     message_data = message.body
     data = json.loads(message_data)
     return data
 
 
+def start_server(async_task, loop: Optional[asyncio.AbstractEventLoop] = None):
+    """
+    Старт задачи, в которой будет прослушиваться очередь
+    :param loop: event loop
+    :param async_task: задача
+    :return:
+    """
+    if loop is None:
+        loop = asyncio.get_event_loop()
+
+    loop.create_task(async_task(loop))
+
+    loop.run_forever()
+
+
 class BaseAdapter(ABC):
     """
     Базовый адаптер очереди сообщений
     """
 
     def __init__(self, url: str,
                  queue_name: Optional[str] = None,
                  exchange_name: Optional[str] = None,
                  exchange_type: Union[ExchangeType, str] = ExchangeType.DIRECT,
-                 loop: Optional[asyncio.AbstractEventLoop] = None):
+                 loop: Optional[asyncio.AbstractEventLoop] = None,
+                 logger: Optional[logging.Logger] = None):
         if loop is None:
             loop = asyncio.get_event_loop()
 
+        if logger is None:
+            self.logger = DEFAULT_LOGGER
+
         self.loop = loop
         self.url = url
         self.queue_name = queue_name
 
         self.connection = None
         self.channel = None
         self.exchange = None
         self.queue = None
 
         self.logger = logging.getLogger(__name__)
 
         self.exchange_name = exchange_name
         self.exchange_type = exchange_type
 
-    async def create_connection(self,
-                                robust: Optional[bool] = True,
-                                prefetch_count: Optional[int] = 0) -> aio_pika.Connection:
+    async def create_connection(self, robust: Optional[bool] = True,
+                                prefetch_count: Optional[int] = 0,
+                                ssl: Optional[bool] = False,
+                                ssl_options: Optional[dict] = None) -> aio_pika.Connection:
         """
         Создание подключения
         """
         if self.connection is None:
-            if robust:
-                self.connection = await aio_pika.connect_robust(
-                    self.url,
-                    loop=self.loop)
-            else:
-                self.connection = await aio_pika.connect(
-                    self.url,
-                    loop=self.loop)
+            connect_fn = aio_pika.connect_robust if robust else aio_pika.connect
+
+            self.connection = await connect_fn(self.url, loop=self.loop, ssl=ssl, ssl_options=ssl_options)
 
         if self.channel is None:
             self.channel = await self.connection.channel()
 
         self.exchange = self.channel.default_exchange
 
         await self.channel.set_qos(prefetch_count=prefetch_count)
 
         return self.connection
 
-    async def declare_exchange(self, **kwargs) -> aio_pika.Exchange:
+    async def declare_exchange(self, durable: Optional[bool] = None, internal: Optional[bool] = False,
+                               passive: Optional[bool] = False, auto_delete: Optional[bool] = False,
+                               arguments: Optional[dict] = None, timeout: Optional[Union[int, float]] = None,
+                               **kwargs) -> aio_pika.Exchange:
+        """
+        Определение обменника
+        """
         if not self.channel:
             raise AdapterError('Connection is not established: channel is none')
 
         if not self.exchange_name:
             raise ValueError('Exchange name is none or empty')
 
-        exchange_kwargs = dict(
-            durable=kwargs.get('durable'),
-            internal=kwargs.get('internal', False),
-            passive=kwargs.get('passive', False),
-            auto_delete=kwargs.get('auto_delete', False),
-            arguments=kwargs.get('arguments'),
-            timeout=kwargs.get('timeout')
-        )
+        exchange_kwargs = dict(durable=durable, internal=internal, passive=passive, auto_delete=auto_delete,
+                               arguments=arguments, timeout=timeout)
+
         if 'robust' in kwargs:
             exchange_kwargs['robust'] = kwargs['robust']
 
-        self.logger.debug('declare_exchange:\n%s', pprint.pformat(exchange_kwargs))
+        self.logger.debug('Declare exchange: %s', pprint.pformat(exchange_kwargs))
 
         self.exchange = await self.channel.declare_exchange(self.exchange_name, self.exchange_type, **exchange_kwargs)
 
         return self.exchange
 
-    async def declare_queue(self, **kwargs) -> aio_pika.Queue:
+    async def declare_queue(self, durable: Optional[bool] = None, exclusive: Optional[bool] = False,
+                            passive: Optional[bool] = False, auto_delete: Optional[bool] = False,
+                            arguments: Optional[dict] = None, timeout: Optional[Union[int, float]] = None,
+                            binding_keys: Optional[List[str]] = None, **kwargs) -> aio_pika.Queue:
         """
         Определение очереди
         """
         if not self.channel:
             raise AdapterError('Connection is not established: channel is none')
 
-        queue_kwargs = dict(
-            durable=kwargs.get('durable'),
-            exclusive=kwargs.get('exclusive', False),
-            passive=kwargs.get('passive', False),
-            auto_delete=kwargs.get('auto_delete', False),
-            arguments=kwargs.get('arguments'),
-            timeout=kwargs.get('timeout')
-        )
+        queue_kwargs = dict(durable=durable, exclusive=exclusive, passive=passive, auto_delete=auto_delete,
+                            arguments=arguments, timeout=timeout)
+
         if 'robust' in kwargs:
             queue_kwargs['robust'] = kwargs['robust']
 
-        self.logger.debug('declare_queue:\n%s', pprint.pformat(queue_kwargs))
+        self.logger.debug('Declare queue: %s', pprint.pformat(queue_kwargs))
 
         self.queue = await self.channel.declare_queue(self.queue_name, **queue_kwargs)
 
+        if binding_keys:
+            for binding_key in binding_keys:
+                await self.queue.bind(self.exchange, routing_key=binding_key)
+
         return self.queue
 
     async def close_channel(self) -> None:
         """
         Закрытие канала
         """
         if self.channel is not None:
@@ -165,73 +185,97 @@
 
 class BaseConsumer(BaseAdapter, ABC):
     """
     Базовый потребитель очереди сообщений
     """
 
     @abstractmethod
-    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage) -> None:
+    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage,
+                              message_id: Optional[uuid.UUID] = None) -> None:
         """
         Обработка подготовленного и провалидированного Json сообщения
         """
-        raise NotImplementedError("Not implemented process_message method")
+        raise NotImplementedError('Not implemented process_message method')
 
     async def create_consume_connection(self, robust: Optional[bool] = True,
                                         prefetch_count: Optional[int] = 0,
+                                        ssl: Optional[bool] = False,
+                                        ssl_options: Optional[dict] = None,
+                                        declare_exchange: Optional[bool] = False,
+                                        exchange_kwargs: Optional[dict] = None,
                                         **kwargs) -> aio_pika.Connection:
         """
         Создание подключения для потребителя
         """
         if robust:
             kwargs['robust'] = True
-        await self.create_connection(robust=robust, prefetch_count=prefetch_count)
+
+        await self.create_connection(robust=robust, prefetch_count=prefetch_count, ssl=ssl, ssl_options=ssl_options)
+
+        if declare_exchange:
+            exchange_kwargs = exchange_kwargs or {}
+            if robust:
+                exchange_kwargs['robust'] = True
+
+            if 'durable' in kwargs:
+                exchange_kwargs['durable'] = kwargs['durable']
+
+            await self.declare_exchange(**exchange_kwargs)
+
         await self.declare_queue(**kwargs)
 
         consume_kwargs = dict(
             no_ack=kwargs.get('no_ack', False)
         )
 
         if self.queue is None:
-            raise AdapterError("Connection is not established: queue is none")
+            raise AdapterError('Connection is not established: queue is none')
 
         await self.queue.consume(self._handle_delivery, **consume_kwargs)
 
         return self.connection
 
     async def _handle_delivery(self, message: aio_pika.IncomingMessage) -> None:
         """
         Обработка полученного сообщения
         """
+        message_id = uuid.uuid4()
+        self.logger.debug('[%s] Start message process', message_id)
+
         async with message.process():
             try:
                 message_json = decode_message(message)
 
-                await self.process_message(message_json, message)
+                self.logger.debug('[%s] routing_key: %s', message_id, message.routing_key)
+                self.logger.debug('[%s] body: %s', message_id, pprint.pformat(message_json))
+
+                await self.process_message(message_json, message, message_id)
+
             except Exception as ex:
                 await self._on_handle_delivery_error(ex, message)
+            finally:
+                self.logger.debug('[%s] End message process', message_id)
 
     async def _on_handle_delivery_error(self, ex: Exception,
                                         raw_message: aio_pika.IncomingMessage) -> None:
         """
         Произошла ошибка при обработке полученного сообщения
         """
         self.logger.error(ex, exc_info=True)
+        raise ex
 
     async def publish_response(self, incoming_message: aio_pika.IncomingMessage, message: Union[str, dict]):
         if self.channel is None:
             raise AdapterError("Connection is not established: channel is none")
 
         message_body = encode_message(message)
 
         await self.channel.default_exchange.publish(
-            aio_pika.Message(
-                message_body,
-                content_type="application/json",
-                correlation_id=incoming_message.correlation_id
-            ),
+            aio_pika.Message(message_body, content_type='application/json',
+                             correlation_id=incoming_message.correlation_id),
             routing_key=incoming_message.reply_to,
         )
 
 
 class Publisher(BaseAdapter):
     """
     Издатель очереди сообщений
@@ -247,22 +291,16 @@
         if self.exchange is None:
             raise AdapterError('Connection is not established: exchange is none')
 
         message_body = encode_message(message)
 
         routing_key = kwargs.pop('routing_key', self.queue_name)
 
-        await self.exchange.publish(
-            aio_pika.Message(
-                message_body,
-                content_type='application/json',
-                **kwargs
-            ),
-            routing_key=routing_key,
-        )
+        await self.exchange.publish(aio_pika.Message(message_body, content_type='application/json', **kwargs),
+                                    routing_key=routing_key)
 
 
 class ReplyToConsumer(BaseConsumer, ABC):
     """
     Reply-To потребитель,
     который может публиковать сообщение в произвольную очередь с указанием того, куда нужно вернуть ответ
     """
```

### Comparing `mq-misc-0.0.6/mq_misc/publish/__main__.py` & `mq_misc-0.0.7/mq_misc/publish/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 parser.add_argument('-id', '--correlation_id', help='Useful to correlate RPC responses with requests.', required=False)
 parser.add_argument('-w', '--waiting_response', action='store_true', help='Waiting reply_to response.')
 
 logger = logging.getLogger('PUBLISH MESSAGE')
 
 
 class SimpleReplyToConsumer(ReplyToConsumer):
-    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage) -> None:
+    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage, **kwargs) -> None:
         logger.info('Response...\n%s', pprint.pformat(body))
 
 
 async def async_main(args):
     try:
         url = args.amqp_url
         queue = args.queue
```

### Comparing `mq-misc-0.0.6/mq_misc.egg-info/PKG-INFO` & `mq_misc-0.0.7/mq_misc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mq-misc
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utility package for working with rabbitmq
 Author: Anton Gorinenko
 Author-email: anton.gorinenko@gmail.com
 Keywords: python,asyncio,utils,mq,aio_pika,rabbit mq,rabbit
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -78,7 +78,13 @@
                         RMQ_ROUTING_KEY] (default: None)
 
 
 ```
 
 python -m mq_misc.publish --amqp-url "amqp://guest:guest@localhost:5672/" --exchange "exchange_1" --exchange_type "
 topic" --routing_key "log.error" --message-file "message.json"
+
+### Creating release tags
+
+```
+git tag -a 0.0.6 -m "Release 0.0.6"
+```
```

### Comparing `mq-misc-0.0.6/setup.py` & `mq_misc-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 python -m twine upload dist/*
 """
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mq-misc",
-    version="0.0.6",
+    version="0.0.7",
     author="Anton Gorinenko",
     author_email="anton.gorinenko@gmail.com",
     description="Utility package for working with rabbitmq",
     long_description=long_description,
     keywords='python, asyncio, utils, mq, aio_pika, rabbit mq, rabbit',
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=['tests']),
```

### Comparing `mq-misc-0.0.6/tests/test_amqp.py` & `mq_misc-0.0.7/tests/test_amqp.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from mq_misc.amqp import BaseConsumer, ReplyToConsumer, create_weak_publisher
 
 url = 'amqp://guest:guest@localhost:5672/'
 queue_name = 'test'
 
 
 class ResponseConsumer(BaseConsumer):
-    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage) -> None:
+    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage, **kwargs) -> None:
         await self.publish_response(raw_message, {'response': True})
 
 
 class RequestConsumer(ReplyToConsumer):
-    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage) -> None:
+    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage, **kwargs) -> None:
         pass
 
 
 class MyTestConsumer(BaseConsumer):
-    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage) -> None:
+    async def process_message(self, body: dict, raw_message: aio_pika.IncomingMessage, **kwargs) -> None:
         pass
 
 
 async def test_consumer():
     consumer = MyTestConsumer(url, queue_name)
     consumer.process_message = AsyncMock(return_value=None)
     await consumer.create_consume_connection(robust=False)
```

