# Comparing `tmp/fleece_network-0.1.0.tar.gz` & `tmp/fleece_network-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleece_network-0.1.0.tar", max compression
+gzip compressed data, was "fleece_network-0.2.0rc0.tar", max compression
```

## Comparing `fleece_network-0.1.0.tar` & `fleece_network-0.2.0rc0.tar`

### file list

```diff
@@ -1,8 +1,31 @@
--rw-r--r--   0        0        0     1045 2024-04-02 05:25:27.743857 fleece_network-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 05:25:27.743857 fleece_network-0.1.0/peerrtc/__init__.py
--rw-r--r--   0        0        0      736 2024-04-02 05:25:27.743857 fleece_network-0.1.0/peerrtc/messages.py
--rw-r--r--   0        0        0    19762 2024-04-02 05:25:27.743857 fleece_network-0.1.0/peerrtc/peer.py
--rw-r--r--   0        0        0        0 2024-04-02 05:25:27.743857 fleece_network-0.1.0/peerrtc/py.typed
--rw-r--r--   0        0        0     2151 2024-04-02 05:25:27.743857 fleece_network-0.1.0/peerrtc/signaling.py
--rw-r--r--   0        0        0      430 2024-04-02 05:25:27.743857 fleece_network-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1666 1970-01-01 00:00:00.000000 fleece_network-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1045 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/candidate.py
+-rw-r--r--   0        0        0    41179 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/ice.py
+-rw-r--r--   0        0        0     6655 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/mdns.py
+-rw-r--r--   0        0        0    12121 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/stun.py
+-rw-r--r--   0        0        0    14905 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/turn.py
+-rw-r--r--   0        0        0      264 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/utils.py
+-rw-r--r--   0        0        0     1226 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/clock.py
+-rw-r--r--   0        0        0      180 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/exceptions.py
+-rw-r--r--   0        0        0    21027 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/rate.py
+-rw-r--r--   0        0        0     1040 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcconfiguration.py
+-rw-r--r--   0        0        0     6531 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcdatachannel.py
+-rw-r--r--   0        0        0    13595 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcdtlstransport.py
+-rw-r--r--   0        0        0    11425 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcicetransport.py
+-rw-r--r--   0        0        0    32180 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcpeerconnection.py
+-rw-r--r--   0        0        0     4612 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcrtpparameters.py
+-rw-r--r--   0        0        0    61599 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcsctptransport.py
+-rw-r--r--   0        0        0      500 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcsessiondescription.py
+-rw-r--r--   0        0        0    24050 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtp.py
+-rw-r--r--   0        0        0    21763 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/sdp.py
+-rw-r--r--   0        0        0     2879 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/stats.py
+-rw-r--r--   0        0        0      978 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/utils.py
+-rw-r--r--   0        0        0      716 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/messages.py
+-rw-r--r--   0        0        0    21346 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/peer.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/py.typed
+-rw-r--r--   0        0        0     2144 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/signaling.py
+-rw-r--r--   0        0        0      479 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc0/PKG-INFO
```

### Comparing `fleece_network-0.1.0/README.md` & `fleece_network-0.2.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `fleece_network-0.1.0/peerrtc/messages.py` & `fleece_network-0.2.0rc0/fleece_network/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
-from typing import Any, Generic, Optional, TypeVar
-from aiortc import RTCSessionDescription  # type: ignore
+from typing import Generic, Optional, TypeVar
+from .aiortc import RTCSessionDescription
 from fastapi import Response
 from pydantic import BaseModel  # type: ignore
 
 
 @dataclass
 class RegisterRequest:
     worker_id: str
```

### Comparing `fleece_network-0.1.0/peerrtc/peer.py` & `fleece_network-0.2.0rc0/fleece_network/peer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,132 +1,157 @@
 from abc import ABC, abstractmethod
+import asyncio
+import functools
 import inspect
 import anyio
 from anyio import Event, create_memory_object_stream, to_thread
 from anyio.abc import TaskGroup
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 import logging
 import pickle
-from typing import Any, Callable, Coroutine, Generic, Optional, TypeVar
+from typing import (
+    Any,
+    Callable,
+    Coroutine,
+    Optional,
+    Protocol,
+    TypeVar,
+    Union,
+    get_type_hints,
+)
 from aiortc import (  # type: ignore
     RTCPeerConnection,
     RTCConfiguration,
     RTCIceServer,
     RTCDataChannel,
     RTCSessionDescription,
 )
 from fastapi import HTTPException, Response
-from pydantic import BaseModel, validate_call
+from pydantic import BaseModel
 import websockets
 
-from peerrtc.messages import (
+from .messages import (
     ConnectReply,
     ConnectRequest,
     SimpleReply,
     SimpleRequest,
     RegisterRequest,
 )
 
 logger = logging.getLogger(__name__)
 
-Handler = Callable[[BaseModel], Response]
-AsyncHandler = Callable[[BaseModel], Coroutine[Any, Any, Response]]
+
+class Encodable(Protocol):
+    @abstractmethod
+    def encode(self, charset: str) -> bytes: ...
+
+
+P = TypeVar("P", bound=BaseModel)
+E = TypeVar("E", bound=Encodable)
+R = Union[E, str]
+SyncHandler = Callable[[P], R]
+AsyncHandler = Callable[[P], Coroutine[Any, Any, R]]
 
 
 class Outward(ABC):
     @abstractmethod
     def label(self) -> str:
         pass
 
     @abstractmethod
-    async def send(self, op: str, data: BaseModel) -> Response:
+    async def send(self, op: str, data: P) -> Response:
         pass
 
     @abstractmethod
     def close(self):
         pass
 
 
 class Inward(ABC):
     def __init__(
         self,
-        hooks: dict[str, Handler | AsyncHandler],
+        hooks: dict[str, SyncHandler | AsyncHandler],
     ):
         self.hooks = hooks
 
     @abstractmethod
     def label(self) -> str:
         pass
 
     @abstractmethod
     async def _send(self, id: int, reply: Response):
         pass
 
-    async def handle(self, id: int, op: str, data: BaseModel):
+    async def handle(self, id: int, op: str, data: P):
         callback = self.hooks.get(op)
 
         async def ahandler(callback: AsyncHandler):
             return await callback(data)
 
-        async def handler(callback: Handler):
+        async def handler(callback: SyncHandler):
             return await to_thread.run_sync(callback, data)
 
         if callback is not None:
             if not inspect.isfunction(callback):  # assertion
                 raise ValueError("Invalid callback type")
-
             try:
                 if inspect.iscoroutinefunction(callback):
                     result = await ahandler(callback)
                 else:
                     result = await handler(callback)
             except HTTPException as e:
                 await self._send(id, Response(e.detail, e.status_code, e.headers))
             else:
-                await self._send(id, Response(result))
+                if isinstance(result, BaseModel):
+                    await self._send(id, Response(result.model_dump_json()))
+                elif isinstance(result, str):
+                    await self._send(id, Response(result))
+                else:  # assertion
+                    raise ValueError("Invalid result type")
 
 
 class Connection(ABC):
     @abstractmethod
-    async def send(self, op: str, data: BaseModel) -> Response:
+    async def send(self, op: str, data: P) -> Response:
         pass
 
 
 class OutwardDataChannel(Outward):
     def __init__(self, channel: RTCDataChannel):
         self._logger = logging.getLogger(self.__class__.__name__)
         self.channel = channel
         self.isopen = Event()
         self.lock = anyio.Lock()
         self.map: dict[int, MemoryObjectSendStream[Response]] = {}
         self.counter = 0
 
-        @channel.on("open")
         def on_open():
             self.isopen.set()
             self._logger.info("Outward data channel %s opens", self.label())
 
-        @channel.on("message")
         async def on_message(raw: bytes):
             self._logger.info(
                 "Outward data channel %s receives message: %s", self.label(), raw
             )
             reply: SimpleReply = pickle.loads(raw)
             async with self.lock:
                 send_stream = self.map.pop(reply.id)
                 await send_stream.send(reply.data)
 
-        @channel.on("close")
         async def on_close():
             self._logger.warning("Outward data channel %s closes", self.label())
 
+        channel.on("open", on_open)
+        channel.on("message", on_message)
+        channel.on("close", on_close)
+
     def label(self) -> str:
         return self.channel.label
 
-    async def send(self, op: str, data: BaseModel) -> Response:
+    async def send(self, op: str, data: P) -> Response:
         await self.isopen.wait()
         send_stream, recv_stream = create_memory_object_stream[Response]()
         async with self.lock:
             id = self.counter
             self.counter += 1
             self.map[id] = send_stream
         self.channel.send(pickle.dumps(SimpleRequest(id, op, data)))
@@ -139,48 +164,49 @@
         self.channel.close()
 
 
 class InwardDataChannel(Inward):
     def __init__(
         self,
         channel: RTCDataChannel,
-        hooks: dict[str, Handler | AsyncHandler],
+        hooks: dict[str, SyncHandler | AsyncHandler],
     ):
         super().__init__(hooks)
         self._logger = logging.getLogger(self.__class__.__name__)
         self.channel = channel
 
-        @channel.on("open")
         async def on_open():
             self._logger.info("Inward data channel opened: %s", self.label())
 
-        @channel.on("message")
         async def on_message(raw: bytes):
             message: SimpleRequest = pickle.loads(raw)
             await self.handle(message.id, message.op, message.data)
 
-        @channel.on("close")
         async def on_close():
             self._logger.warning("Inward data channel %s closes", self.label())
 
+        channel.on("open", on_open)
+        channel.on("message", on_message)
+        channel.on("close", on_close)
+
     def label(self) -> str:
         return self.channel.label
 
     async def _send(self, id: int, reply: Response):
         """Although it's not an async function, it requires the existence of an event loop."""
 
         self._logger.info("Channel %s sends message: %s", self.label(), reply)
         self.channel.send(pickle.dumps(SimpleReply(id, reply)))
 
 
 class OutwardLoopback(Outward):
     def __init__(
         self,
         label: str,
-        send_stream: MemoryObjectSendStream[tuple[int, str, BaseModel]],
+        send_stream: MemoryObjectSendStream[tuple[int, str, P]],
         recv_stream: MemoryObjectReceiveStream[tuple[int, Response]],
         tg: TaskGroup,
     ):
         self._logger = logging.getLogger(self.__class__.__name__)
         self._label = label
 
         self.send_stream = send_stream
@@ -201,15 +227,15 @@
                 tg.start_soon(send_stream.send, reply)
 
         tg.start_soon(onmessage)
 
     def label(self) -> str:
         return self._label
 
-    async def send(self, op: str, data: BaseModel) -> Response:
+    async def send(self, op: str, data: P) -> Response:
         send_stream, recv_stream = create_memory_object_stream[Response]()
         async with self.lock:
             id = self.counter
             self.counter += 1
             self.map[id] = send_stream
         await self.send_stream.send((id, op, data))
         return await recv_stream.receive()
@@ -219,17 +245,17 @@
         self.recv_stream.close()
 
 
 class InwardLoopback(Inward):
     def __init__(
         self,
         label: str,
-        recv_stream: MemoryObjectReceiveStream[tuple[int, str, BaseModel]],
+        recv_stream: MemoryObjectReceiveStream[tuple[int, str, P]],
         send_stream: MemoryObjectSendStream[tuple[int, Response]],
-        hooks: dict[str, Handler | AsyncHandler],
+        hooks: dict[str, SyncHandler | AsyncHandler],
         tg: TaskGroup,
     ):
         super().__init__(hooks)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._label = label
         self.send_stream = send_stream
         self.recv_stream = recv_stream
@@ -258,15 +284,15 @@
         CONNECTED = 3
 
     def __init__(
         self,
         from_id: str,
         to_id: str,
         configs: list[tuple[str, Optional[str], Optional[str]]],
-        hooks: dict[str, AsyncHandler | Handler],
+        hooks: dict[str, AsyncHandler | SyncHandler],
         tg: TaskGroup,
     ):
         self._logger = logging.getLogger(self.__class__.__name__)
         self.from_id = from_id
         self.to_id = to_id
         self.configs = configs
         self.inner: Optional[RTCPeerConnection] = None  # changed with state
@@ -296,21 +322,19 @@
                     for config in self.configs
                 ]
             )
         )
         self.out_channel = OutwardDataChannel(pc.createDataChannel(self.from_id))
         self.inner = pc
 
-        @pc.on("datachannel")
         async def on_datachannel(channel: RTCDataChannel):
             async with self.lock:
                 self.in_channel = InwardDataChannel(channel, self.hooks)
                 self._logger.info("Data channel created: %s", self.in_channel.label())
 
-        @pc.on("connectionstatechange")
         async def on_connectionstatechange():
             async with self.condition:
                 if pc.connectionState == "connected":
                     self.state = PeerConnection.State.CONNECTED
                     self.condition.notify_all()
 
                     self._logger.info(
@@ -323,14 +347,17 @@
 
                     self._logger.info(
                         "Connection (%s, %s) changes state to FAILED",
                         self.from_id,
                         self.to_id,
                     )
 
+        pc.on("datachannel", on_datachannel)
+        pc.on("connectionstatechange", on_connectionstatechange)
+
         return pc
 
     async def send_through_ws(
         self, ws: websockets.WebSocketClientProtocol, sdp: RTCSessionDescription
     ):
         try:
             if sdp.type == "offer":
@@ -356,14 +383,15 @@
                 self._logger.info("No need to create offer")
                 return False
 
             self.state = PeerConnection.State.OFFERED
             pc = await self._init_inner()
             await pc.setLocalDescription(await pc.createOffer())
             offer = pc.localDescription
+            assert offer
 
             self._logger.info("Create offer with %s", offer)
 
         self.tg.start_soon(self.send_through_ws, ws, offer)
 
         return True
 
@@ -398,14 +426,15 @@
                     )
 
             self.state = PeerConnection.State.WAITING
             pc = await self._init_inner()
             await pc.setRemoteDescription(sdp)
             await pc.setLocalDescription(await pc.createAnswer())
             answer = pc.localDescription
+            assert answer
 
         self.tg.start_soon(self.send_through_ws, ws, answer)
 
         return True
 
     async def set_answer(self, sdp: Optional[RTCSessionDescription]):
         async with self.lock:
@@ -427,15 +456,15 @@
                 self.state = PeerConnection.State.WAITING
                 pc = self.inner
                 if pc is not None:
                     await pc.setRemoteDescription(sdp)
                 else:
                     self._logger.error("No inner peer connection")
 
-    async def send(self, op: str, data: BaseModel) -> Response:
+    async def send(self, op: str, data: P) -> Response:
         while True:
             async with self.condition:
                 if self.state == PeerConnection.State.CONNECTED:
                     if self.out_channel is not None:
                         self._logger.info("Sending message: %s", op)
                         channel = self.out_channel
                         break
@@ -451,59 +480,88 @@
         return await channel.send(op, data)
 
 
 class SelfConnection(Connection):
     def __init__(
         self,
         id: str,
-        hooks: dict[str, AsyncHandler | Handler],
+        hooks: dict[str, AsyncHandler | SyncHandler],
         tg: TaskGroup,
     ):
         req_send, req_recv = create_memory_object_stream[tuple[int, str, BaseModel]]()
         rep_send, rep_recv = create_memory_object_stream[tuple[int, Response]]()
         self.out_loop = OutwardLoopback(id, req_send, rep_recv, tg)
         self.in_loop = InwardLoopback(id, req_recv, rep_send, hooks, tg)
 
-    async def send(self, op: str, data: BaseModel) -> Response:
+    async def send(self, op: str, data: P) -> Response:
         return await self.out_loop.send(op, data)
 
 
 class Peer:
     def __init__(
         self,
         worker_id: str,
         signaling_url: str,
         ice_configs: list[tuple[str, Optional[str], Optional[str]]],
-        hooks: dict[str, AsyncHandler | Handler],
+        hooks: dict[str, AsyncHandler | SyncHandler],
         tg: TaskGroup,
     ):
 
         self._logger = logging.getLogger(self.__class__.__name__)
         self.worker_id = worker_id
         """A unique id for worker. Only for identification."""
 
         self.signaling_url = signaling_url
         """The signaling server url should not contain the protocol."""
 
         self.ws: Optional[websockets.WebSocketClientProtocol] = None
         """The websocket connection to the signaling server. Use to send offer."""
 
-        self.hooks = {name: validate_call(hook) for name, hook in hooks.items()}
+        self.hooks = {name: Peer.jsonargs(hook) for name, hook in hooks.items()}
         """Every time a new channel is created by peer (not by our), this handler will be called."""
 
         self.tg = tg
 
         self.ice_configs = ice_configs
 
         self.conns: dict[str, PeerConnection] = {}
         self.lo = SelfConnection(worker_id, self.hooks, tg)
         self.lock = anyio.Lock()
 
         self.tg.start_soon(self._register)
 
+    @staticmethod
+    def jsonargs(
+        func: Callable[..., Any]
+    ) -> Callable[..., Any | Coroutine[Any, Any, Any]]:
+        @functools.wraps(func)
+        def wrapper(*args: Any) -> Any | Coroutine[Any, Any, Any]:
+            signature = inspect.signature(func)
+            type_hints = get_type_hints(func)
+
+            parsed_args = []
+            for param_name, arg in zip(signature.parameters, args):
+                model_cls = type_hints[param_name]
+                if isinstance(arg, (str, bytes)):
+                    parsed_arg = model_cls.parse_raw(arg)
+                else:
+                    parsed_arg = arg
+                parsed_args.append(parsed_arg)
+            return func(*parsed_args)
+
+        if asyncio.iscoroutinefunction(func):
+
+            @functools.wraps(func)
+            async def async_wrapper(*args: Any) -> Any:
+                return await wrapper(*args)
+
+            return async_wrapper
+        else:
+            return wrapper
+
     async def _answer(
         self, ws: websockets.WebSocketClientProtocol, request: ConnectRequest
     ):
         from_worker_id = request.from_worker_id
         self._logger.info("Received offer from %s", from_worker_id)
 
         async with self.lock:
```

### Comparing `fleece_network-0.1.0/peerrtc/signaling.py` & `fleece_network-0.2.0rc0/fleece_network/signaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import uvicorn
 import logging
 import pickle
 from typing import Dict
 from fastapi import FastAPI, WebSocket, WebSocketDisconnect
-from peerrtc.messages import (
+from .messages import (
     ConnectReply,
     ConnectRequest,
     RegisterReply,
     RegisterRequest,
 )
```

### Comparing `fleece_network-0.1.0/PKG-INFO` & `fleece_network-0.2.0rc0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: fleece-network
-Version: 0.1.0
+Version: 0.2.0rc0
 Summary: P2P socket built on aiortc.
 Author: Linyu Wu
 Author-email: celve03@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aioconsole (>=0.7.0,<0.8.0)
-Requires-Dist: aiortc2 (>=1.8.0,<2.0.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0)
+Requires-Dist: fastapi (>=0.110.1,<0.111.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # Nameless
```

