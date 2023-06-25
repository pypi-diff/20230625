# Comparing `tmp/pydns3-0.0.7.tar.gz` & `tmp/pydns3-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydns3-0.0.7.tar", last modified: Tue Apr 18 21:34:59 2023, max compression
+gzip compressed data, was "pydns3-0.0.8.tar", last modified: Sun Jun 25 08:03:48 2023, max compression
```

## Comparing `pydns3-0.0.7.tar` & `pydns3-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-04-18 21:34:59.377124 pydns3-0.0.7/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      243 2023-03-26 23:42:47.000000 pydns3-0.0.7/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      562 2023-04-18 21:16:11.000000 pydns3-0.0.7/pydns/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2967 2023-04-18 21:26:07.000000 pydns3-0.0.7/pydns/answer.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/client/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1173 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/client/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1073 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/client/https.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3070 2023-03-29 22:16:54.000000 pydns3-0.0.7/pydns/client/standard.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2388 2023-04-18 21:26:19.000000 pydns3-0.0.7/pydns/content.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/edns/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      197 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/edns/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1450 2023-04-18 21:10:55.000000 pydns3-0.0.7/pydns/edns/record.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2591 2023-03-29 22:05:52.000000 pydns3-0.0.7/pydns/enum.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1406 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/exceptions.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2107 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/flags.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4206 2023-04-18 21:11:10.000000 pydns3-0.0.7/pydns/message.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      398 2023-04-18 21:11:13.000000 pydns3-0.0.7/pydns/question.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/server/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      132 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/server/__init__.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/server/backend/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      994 2023-03-30 07:56:17.000000 pydns3-0.0.7/pydns/server/backend/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5293 2023-03-30 08:28:49.000000 pydns3-0.0.7/pydns/server/backend/blacklist.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4062 2023-03-30 07:56:43.000000 pydns3-0.0.7/pydns/server/backend/cache.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1278 2023-03-30 07:26:09.000000 pydns3-0.0.7/pydns/server/backend/forwarder.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2647 2023-03-30 08:23:38.000000 pydns3-0.0.7/pydns/server/backend/memory.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5159 2023-03-29 00:23:06.000000 pydns3-0.0.7/pydns/server/server.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      628 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       58 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-18 21:34:59.377124 pydns3-0.0.7/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      813 2023-04-18 21:34:36.000000 pydns3-0.0.7/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.356862 pydns3-0.0.8/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-06-25 08:03:48.356862 pydns3-0.0.8/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      243 2023-03-26 23:42:47.000000 pydns3-0.0.8/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.352862 pydns3-0.0.8/pydns/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      562 2023-04-18 21:16:11.000000 pydns3-0.0.8/pydns/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3031 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/answer.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.352862 pydns3-0.0.8/pydns/client/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1173 2023-03-26 23:42:47.000000 pydns3-0.0.8/pydns/client/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1083 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/client/https.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3148 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/client/standard.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2335 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/content.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.352862 pydns3-0.0.8/pydns/edns/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      197 2023-03-26 23:42:47.000000 pydns3-0.0.8/pydns/edns/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1468 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/edns/record.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2591 2023-03-29 22:05:52.000000 pydns3-0.0.8/pydns/enum.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1406 2023-03-26 23:42:47.000000 pydns3-0.0.8/pydns/exceptions.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2117 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/flags.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4158 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/message.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      467 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/question.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.352862 pydns3-0.0.8/pydns/server/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      132 2023-03-26 23:42:47.000000 pydns3-0.0.8/pydns/server/__init__.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.352862 pydns3-0.0.8/pydns/server/backend/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      994 2023-03-30 07:56:17.000000 pydns3-0.0.8/pydns/server/backend/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5253 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/server/backend/blacklist.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4060 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/server/backend/cache.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1250 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/server/backend/forwarder.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2647 2023-03-30 08:23:38.000000 pydns3-0.0.8/pydns/server/backend/memory.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5156 2023-06-25 08:01:07.000000 pydns3-0.0.8/pydns/server/server.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:03:48.356862 pydns3-0.0.8/pydns3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-06-25 08:03:48.000000 pydns3-0.0.8/pydns3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      628 2023-06-25 08:03:48.000000 pydns3-0.0.8/pydns3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-25 08:03:48.000000 pydns3-0.0.8/pydns3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       56 2023-06-25 08:03:48.000000 pydns3-0.0.8/pydns3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-06-25 08:03:48.000000 pydns3-0.0.8/pydns3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-25 08:03:48.356862 pydns3-0.0.8/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      811 2023-06-25 08:03:25.000000 pydns3-0.0.8/setup.py
```

### Comparing `pydns3-0.0.7/PKG-INFO` & `pydns3-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydns3
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple Python DNS Library. DNS Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydns
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydns3-0.0.7/pydns/__init__.py` & `pydns3-0.0.8/pydns/__init__.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/pydns/answer.py` & `pydns3-0.0.8/pydns/answer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 DNS Answer Record Instance/Format
 """
 from typing import Optional, Type
 from abc import abstractmethod
-from dataclasses import dataclass, field
 from typing import Protocol
-from typing_extensions import Self
+from typing_extensions import Annotated, Self
 
-from pystructs import Context, Domain, Int, Int16, Int32, struct
+from pyderive import dataclass, field
+from pystructs import Context, Struct, Domain, U16, U32, Wrap
 
 from .content import Content, Literal
 from .enum import RType, RClass
 from . import content
 
 #** Variables **#
 __all__ = ['BaseAnswer', 'Answer', 'PreRequisite', 'Update']
@@ -32,20 +32,19 @@
     # else just encapsulate in sized-bytes object
     if size is not None:
         return Literal[rtype, size]
     raise ValueError(f'unsupported rtype: {rtype.name!r}')
 
 #** Classes **#
 
-@struct
-class Header:
+class Header(Struct):
     name:   Domain
-    rtype:  Int[16, RType, 'RType']
-    rclass: Int[16, RClass, 'RClass']
-    ttl:    Int32
+    rtype:  Annotated[RType, Wrap[U16, RType]]
+    rclass: Annotated[RClass, Wrap[U16, RClass]]
+    ttl:    U32
 
 class BaseAnswer(Protocol):
     """Baseclass for defining `Answer` objects"""
     name: bytes
     
     @property
     @abstractmethod
@@ -57,22 +56,22 @@
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def decode(cls, ctx: Context, raw: bytes) -> Self:
         raise NotImplementedError
 
-@dataclass
+@dataclass(slots=True)
 class Answer(BaseAnswer):
     """Standard DNS Answer Implementation"""
     name:    bytes
     ttl:     int
     content: Content
     rclass:  RClass  = RClass.IN
-    
+ 
     @property
     def rtype(self) -> RType:
         return self.content.rtype
 
     def encode(self, ctx: Context) -> bytes:
         head = Header(self.name, self.rtype, self.rclass, self.ttl).encode(ctx)
         ctx.index += 2 # pre-increment index since body-size goes before content
@@ -80,21 +79,21 @@
         size = len(body).to_bytes(2, 'big')
         return head + size + body
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> Self:
         # parse header and size of body
         header = Header.decode(ctx, raw)
-        size   = Int16.decode(ctx, raw)
+        size   = int.from_bytes(ctx.slice(raw, 2), 'big')
         # determine content-type based on rtype in header
         rclass  = get_rclass(header.rtype, size)
         content = rclass.decode(ctx, raw)
         return cls(header.name, header.ttl, content, header.rclass)
 
-@dataclass
+@dataclass(slots=True)
 class PreRequisite(Answer):
     """Alias for Answer in UPDATE action DNS Requests with Sensible Defaults"""
     ttl:     int = 0
     content: Content = field(default=content.ANY)
 
 class Update(Answer):
     """Alias of Answer in UPDATE action DNS Requests"""
```

### Comparing `pydns3-0.0.7/pydns/client/__init__.py` & `pydns3-0.0.8/pydns/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/pydns/client/https.py` & `pydns3-0.0.8/pydns/client/https.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Web HTTP Based DNS Client
 """
 from urllib.request import Request, urlopen
-from dataclasses import dataclass
 from typing import Optional
 
+from pyderive import dataclass
+
 from . import BaseClient, Message
 
 #** Variables **#
 __all__ = ['HttpsClient']
 
 #** Classes **#
 
-@dataclass
+@dataclass(slots=True)
 class HttpsClient(BaseClient):
     url:     str           = 'https://cloudflare-dns.com/dns-query'
     timeout: Optional[int] = None
 
     def __post_init__(self):
         self.headers = {
             'Accept':       'application/dns-message',
```

### Comparing `pydns3-0.0.7/pydns/client/standard.py` & `pydns3-0.0.8/pydns/client/standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 """
 Standard UDP/TCP Client Implementations
 """
 import random
 import socket
-from dataclasses import dataclass
+from abc import ABC, abstractmethod
 from typing import List, Optional
 
 from pypool import Pool
 from pyserve import RawAddr
+from pyderive import dataclass
 
 from . import BaseClient, Message
 
 #** Variables **#
 __all__ = ['UdpClient', 'TcpClient']
 
 #** Classes **#
 
 class SocketPool(Pool[socket.socket]):
     pass
 
-@dataclass
-class Client(BaseClient):
+@dataclass(slots=True)
+class Client(BaseClient, ABC):
     addresses:  List[RawAddr]
     block_size: int           = 8192
     pool_size:  Optional[int] = None
     expiration: Optional[int] = None
     timeout:    int           = 10
 
     def __post_init__(self):
         self.pool = SocketPool(
             factory=self.newsock,
             cleanup=self.cleanup,
             max_size=self.pool_size, 
             expiration=self.expiration)
-    
+   
+    @abstractmethod
     def newsock(self) -> socket.socket:
         raise NotImplementedError
 
+    @abstractmethod
     def cleanup(self, sock: socket.socket):
         raise NotImplementedError
 
     def pickaddr(self) -> RawAddr:
         """pick random address from list of addresses"""
         return random.choice(self.addresses)
     
     def drain(self):
         """drain socket pool"""
         self.pool.drain()
 
-@dataclass
 class UdpClient(Client):
    
     def newsock(self) -> socket.socket:
         """spawn new socket for the socket pool"""
         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         sock.settimeout(self.timeout)
         return sock
```

### Comparing `pydns3-0.0.7/pydns/edns/record.py` & `pydns3-0.0.8/pydns/edns/record.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """
 EDNS OPT Answer Varient Implementation
 """
-from dataclasses import dataclass
-from typing_extensions import Self
+from typing_extensions import Annotated, Self
 
-from pystructs import Context, Domain, Int, Int8, Int16, struct
+from pyderive import dataclass
+from pystructs import Context, Struct, Domain, U8, U16, Wrap
 
 from ..enum import RType
 from ..answer import BaseAnswer
 
 #** Variables **#
 __all__ = ['ROOT', 'EdnsAnswer']
 
 #: root domain (according to EDNS)
 ROOT = b''
 
 #** Classes **#
 
-@struct
-class Header:
+class Header(Struct):
     name:           Domain
-    rtype:          Int[16, RType, 'RType']
-    payload_size:   Int16
-    extended_rcode: Int8
-    version:        Int8
-    z:              Int16
-    data_length:    Int16
+    rtype:          Annotated[RType, Wrap[U16, RType]]
+    payload_size:   U16
+    extended_rcode: U8
+    version:        U8
+    z:              U16
+    data_length:    U16
 
-@dataclass
+@dataclass(slots=True)
 class EdnsAnswer(BaseAnswer):
     name:     bytes  = ROOT
     version:  int    = 0
     content:  bytes  = b''
     udp_size: int    = 512
 
     @property
```

### Comparing `pydns3-0.0.7/pydns/enum.py` & `pydns3-0.0.8/pydns/enum.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/pydns/exceptions.py` & `pydns3-0.0.8/pydns/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/pydns/flags.py` & `pydns3-0.0.8/pydns/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 DNS Flags Implementation
 """
 from enum import IntFlag
-from dataclasses import dataclass
 from typing_extensions import Self
 
+from pyderive import dataclass
+
 from .enum import QR, OpCode, RCode
 
 #** Variables **#
 __all__ = ['Flags']
 
 #** Functions **#
 
@@ -27,15 +28,15 @@
     Authorative      = 1 << 10
     Truncated        = 1 << 9
     RDesired         = 1 << 8
     RAvailable       = 1 << 7
     Authenticated    = 1 << 5
     CheckingDisabled = 1 << 4
 
-@dataclass
+@dataclass(slots=True)
 class Flags:
     qr:                   QR
     op:                   OpCode
     authorative:          bool  = False
     truncated:            bool  = False
     recursion_desired:    bool  = True
     recursion_available:  bool  = False
```

### Comparing `pydns3-0.0.7/pydns/message.py` & `pydns3-0.0.8/pydns/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 DNS Message Object
 """
 from typing import List
-from dataclasses import dataclass, field
 from typing import Type
 from typing_extensions import Self
 
-from pystructs import Context, Domain, Int, Int16, struct
+from pystructs import *
+from pyderive import dataclass, field
 
 from .enum import OpCode, RType, RCode
 from .flags import Flags
 from .answer import BaseAnswer, Answer, PreRequisite, Update
 from .question import Question, Zone
 from .edns import EdnsAnswer
 from .exceptions import make_error
@@ -44,37 +44,35 @@
         # decode answer class accordingly
         new = newcls.decode(ctx, raw)
         objects.append(new)
     return objects
 
 #** Classes **#
 
-@struct
-class PeekHeader:
+class PeekHeader(Struct):
     name:  Domain
-    rtype: Int[16, RType, 'RType']
+    rtype: Wrap[U16, RType]
 
-@struct
-class Header:
-    id:             Int16
-    flags:          Int16 
-    num_questions:  Int16
-    num_answers:    Int16
-    num_authority:  Int16
-    num_additional: Int16
+class Header(Struct):
+    id:             U16
+    flags:          U16 
+    num_questions:  U16
+    num_answers:    U16
+    num_authority:  U16
+    num_additional: U16
 
-@dataclass
+@dataclass(slots=True)
 class Message:
     id:         int
     flags:      Flags
     questions:  List[Question]   = field(default_factory=list)
     answers:    List[Answer]     = field(default_factory=list)
     authority:  List[Answer]     = field(default_factory=list)
     additional: List[BaseAnswer] = field(default_factory=list)
-    
+ 
     def raise_on_error(self):
         """raise exception if message contains an error"""
         if self.flags.rcode != RCode.NoError:
             domains = list({q.name for q in self.questions})
             domains = domains[0] if len(domains) == 1 else domains
             make_error(self.flags.rcode, domains or None)
 
@@ -108,15 +106,15 @@
         :param raw: raw bytes to decode as a DNS message
         :return:    dns message object
         """
         # parse header for message information
         ctx = Context()
         raw = bytes(raw)
         header = Header.decode(ctx, raw)
-        flags  = Flags.fromint(header.flags) 
+        flags  = Flags.fromint(header.flags)
         # determine classes to parse content
         qclass, anclass, auclass = (Question, Answer, Answer) \
                 if flags.op != OpCode.Update else \
                 (Zone, PreRequisite, Update)
         # parse body content w/ determined classes
         questions  = decode_list(qclass, header.num_questions, ctx, raw)
         answers    = decode_answers(anclass, header.num_answers, ctx, raw)
```

### Comparing `pydns3-0.0.7/pydns/server/backend/__init__.py` & `pydns3-0.0.8/pydns/server/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/pydns/server/backend/blacklist.py` & `pydns3-0.0.8/pydns/server/backend/blacklist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Backend Domain Blacklist Extension
 """
 import os
 import re
 import dbm
 from abc import abstractmethod
-from dataclasses import dataclass
 from typing import Protocol, Generator, TextIO, ClassVar, Set, Optional
 
+from pyderive import dataclass
+
 from . import Answers, Backend, RType
 
 #** Variables **#
 __all__ = [
     'is_domain',
     'parse_blacklist',
 
@@ -130,20 +131,19 @@
             self.ingest(name.encode(), src, validate=False)
             self.dbm[fpath] = str(time).encode()
 
     def contains(self, domain: bytes) -> bool:
         """check if domain is contained within the dbm key/value store"""
         return domain in self.dbm
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class Blacklist(Backend):
     """
     Blacklist Backend Extension. Block all Records for Associated Domains
     """
-    __slots__ = ('backend', 'blacklist', 'empty')
     source: ClassVar[str] = 'Blacklist'
 
     backend:   Backend
     blacklist: Set[bytes]
     database:  Optional[BlockDB] = None
     
     def __post_init__(self):
```

### Comparing `pydns3-0.0.7/pydns/server/backend/cache.py` & `pydns3-0.0.8/pydns/server/backend/cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,70 @@
 """
 Backend Extension to support In-Memory Answer Caching
 """
 import time
 import math
-import threading
-from dataclasses import dataclass, field
+from threading import Lock
 from typing import List, Set, Dict, ClassVar
 
+from pyderive import dataclass, field
+
 from . import Answers, Backend, RType, Answer
 from .memory import MemoryBackend
 from .blacklist import Blacklist
 
 #** Variables **#
 __all__ = ['Cache']
 
 #: default set of other backend sources to ignore
 IGNORE = {MemoryBackend.source, Blacklist.source}
 
 #** Classes **#
 
-@dataclass
+@dataclass(slots=True)
 class CacheRecord:
     """
     Record Entry for In-Memory Cache
     """
-    __slots__ = ('answers', 'expiration', 'ttl', 'lifetime_mod')
-
-    answers:    List[Answer]
-    expiration: float
-    ttl:        int
-
-    def __post_init__(self):
-        self.lifetime_mod = 0
+    answers:      List[Answer]
+    expiration:   float
+    ttl:          int
+    lifetime_mod: int = field(default=0, init=False)
 
     def lifetime(self):
         """calculate lifetime remaining of record"""
         return int(math.floor(self.expiration - time.time()))
 
     def ttl_mod(self, lifetime: int) -> int:
         """calculate ttl modifier based on the given lifetime"""
         elapsed = self.ttl - lifetime
         ttl_mod = elapsed - self.lifetime_mod
         self.lifetime_mod = elapsed
         return ttl_mod
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class Cache(Backend):
     """
     In-Memory Cache Extension for Backend Results
     """
     source: ClassVar[str] = 'Cache'
-    __slots__ = (
-        'recursion_available',
-
-        'backend', 
-        'mutex', 
-        'authorities', 
-        'cache', 
-    )
 
     backend:    Backend
     expiration: int = 30
     maxsize:    int = 10000
     ignore:     Set[str] = field(default_factory=lambda: IGNORE)
+ 
+    mutex:       Lock                   = field(default_factory=Lock, init=False)
+    cache:       Dict[str, CacheRecord] = field(default_factory=dict, init=False)
+    authorities: Dict[bytes, bool]      = field(default_factory=dict, init=False)
 
+    recursion_available: bool = field(default=False, init=False)
+ 
     def __post_init__(self):
         self.recursion_available = self.backend.recursion_available
-        self.mutex = threading.Lock()
-        self.authorities: Dict[bytes, bool]      = {}
-        self.cache:       Dict[str, CacheRecord] = {}
 
     def is_authority(self, domain: bytes) -> bool:
         """
         retrieve if domain is authority from cache before checking backend
         """
         # check cache before querying backend
         if domain in self.authorities:
```

### Comparing `pydns3-0.0.7/pydns/server/backend/forwarder.py` & `pydns3-0.0.8/pydns/server/backend/forwarder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Backend Recursive Client-Forwarder Extension
 """
-from dataclasses import dataclass
 from typing import ClassVar
 
+from pyderive import dataclass
+
 from . import Answers, Backend
 from ...client import BaseClient
 from ... import RType, Answer, Question
 
 #** Variables **#
 __all__ = ['Forwarder']
 
 #** Classes **#
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class Forwarder(Backend):
     """
     Recursive Dns-Client Lookup Forwarder when Backend returns no Results
     """
-    __slots__ = ('backend', 'client')
     source: ClassVar[str] = 'Forwarder'
     recursion_available: ClassVar[bool] = True
 
     backend: Backend
     client:  BaseClient
 
     def is_authority(self, domain: bytes) -> bool:
```

### Comparing `pydns3-0.0.7/pydns/server/backend/memory.py` & `pydns3-0.0.8/pydns/server/backend/memory.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/pydns/server/server.py` & `pydns3-0.0.8/pydns/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import IntEnum
 from logging import Logger, getLogger
-from dataclasses import dataclass, field
 from typing import Optional
 
 from pyserve import Address, Writer
 from pyserve import Session as BaseSession
+from pyderive import dataclass, field
 
 from .backend import Backend
 from ..enum import QR, OpCode, RType, RCode
 from ..message import Message
 from ..edns import EdnsAnswer
 from ..exceptions import DnsError, NotImplemented
```

### Comparing `pydns3-0.0.7/pydns3.egg-info/PKG-INFO` & `pydns3-0.0.8/pydns3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydns3
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple Python DNS Library. DNS Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydns
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydns3-0.0.7/pydns3.egg-info/SOURCES.txt` & `pydns3-0.0.8/pydns3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.7/setup.py` & `pydns3-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='pydns3',
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/pydns',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description='Simple Python DNS Library. DNS Packet-Parsing/Client/Server',
     python_requires='>=3.7',
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=[
         'pypool3',
         'pyserve3',
+        'pyderive3',
         'pystructs3',
-        'dataclasses',
         'typing_extensions',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```

