# Comparing `tmp/pydhcp3-0.0.2.tar.gz` & `tmp/pydhcp3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydhcp3-0.0.2.tar", last modified: Wed Apr 26 00:57:16 2023, max compression
+gzip compressed data, was "pydhcp3-0.0.4.tar", last modified: Sun Jun 25 08:07:51 2023, max compression
```

## Comparing `pydhcp3-0.0.2.tar` & `pydhcp3-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-24 00:15:16.000000 pydhcp3-0.0.2/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      249 2023-04-24 00:07:53.000000 pydhcp3-0.0.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/
--rw-r--r--   0 andrew    (1000) andrew    (1000)       37 2023-04-21 08:22:54.000000 pydhcp3-0.0.2/pydhcp/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2334 2023-04-26 00:55:45.000000 pydhcp3-0.0.2/pydhcp/base.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2023-04-20 03:29:25.000000 pydhcp3-0.0.2/pydhcp/enum.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1549 2023-04-22 23:15:15.000000 pydhcp3-0.0.2/pydhcp/exceptions.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/v4/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      672 2023-04-26 00:40:44.000000 pydhcp3-0.0.2/pydhcp/v4/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7975 2023-04-23 23:22:58.000000 pydhcp3-0.0.2/pydhcp/v4/enum.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5180 2023-04-26 00:49:02.000000 pydhcp3-0.0.2/pydhcp/v4/message.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4486 2023-04-26 00:47:50.000000 pydhcp3-0.0.2/pydhcp/v4/options.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/v4/server/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      155 2023-04-23 02:15:39.000000 pydhcp3-0.0.2/pydhcp/v4/server/__init__.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.568669 pydhcp3-0.0.2/pydhcp/v4/server/backend/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2324 2023-04-23 23:56:13.000000 pydhcp3-0.0.2/pydhcp/v4/server/backend/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2612 2023-04-23 23:40:22.000000 pydhcp3-0.0.2/pydhcp/v4/server/backend/cache.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8039 2023-04-26 00:39:20.000000 pydhcp3-0.0.2/pydhcp/v4/server/server.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/pydhcp/v6/
--rw-r--r--   0 andrew    (1000) andrew    (1000)        0 2023-04-21 00:36:00.000000 pydhcp3-0.0.2/pydhcp/v6/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2354 2023-04-21 07:58:15.000000 pydhcp3-0.0.2/pydhcp/v6/duid.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1452 2023-04-21 08:20:56.000000 pydhcp3-0.0.2/pydhcp/v6/enum.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4381 2023-04-21 08:16:49.000000 pydhcp3-0.0.2/pydhcp/v6/message.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5065 2023-04-21 08:20:18.000000 pydhcp3-0.0.2/pydhcp/v6/options.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/pydhcp3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      559 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       41 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-04-26 00:57:16.000000 pydhcp3-0.0.2/pydhcp3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-26 00:57:16.572669 pydhcp3-0.0.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      777 2023-04-26 00:56:58.000000 pydhcp3-0.0.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:07:51.724495 pydhcp3-0.0.4/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-24 00:15:16.000000 pydhcp3-0.0.4/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-06-25 08:07:51.724495 pydhcp3-0.0.4/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      249 2023-04-24 00:07:53.000000 pydhcp3-0.0.4/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:07:51.720495 pydhcp3-0.0.4/pydhcp/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       37 2023-04-21 08:22:54.000000 pydhcp3-0.0.4/pydhcp/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3818 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/base.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2476 2023-04-20 03:29:25.000000 pydhcp3-0.0.4/pydhcp/enum.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1735 2023-05-04 21:09:56.000000 pydhcp3-0.0.4/pydhcp/exceptions.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:07:51.720495 pydhcp3-0.0.4/pydhcp/v4/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      758 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     8923 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/enum.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5219 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/message.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5074 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/options.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:07:51.724495 pydhcp3-0.0.4/pydhcp/v4/server/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      350 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/server/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     8408 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/server/handlers.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    10219 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v4/server/server.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:07:51.724495 pydhcp3-0.0.4/pydhcp/v6/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      682 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v6/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2372 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v6/duid.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1452 2023-04-21 08:20:56.000000 pydhcp3-0.0.4/pydhcp/v6/enum.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4332 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v6/message.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5039 2023-06-25 08:07:07.000000 pydhcp3-0.0.4/pydhcp/v6/options.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 08:07:51.724495 pydhcp3-0.0.4/pydhcp3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      720 2023-06-25 08:07:51.000000 pydhcp3-0.0.4/pydhcp3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      517 2023-06-25 08:07:51.000000 pydhcp3-0.0.4/pydhcp3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-25 08:07:51.000000 pydhcp3-0.0.4/pydhcp3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       48 2023-06-25 08:07:51.000000 pydhcp3-0.0.4/pydhcp3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        7 2023-06-25 08:07:51.000000 pydhcp3-0.0.4/pydhcp3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-25 08:07:51.724495 pydhcp3-0.0.4/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      795 2023-06-25 08:07:26.000000 pydhcp3-0.0.4/setup.py
```

### Comparing `pydhcp3-0.0.2/LICENSE` & `pydhcp3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.2/PKG-INFO` & `pydhcp3-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydhcp3
-Version: 0.0.2
+Version: 0.0.4
 Summary: Simple Python DHCP Library. DHCP Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydhcp
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydhcp3-0.0.2/pydhcp/enum.py` & `pydhcp3-0.0.4/pydhcp/enum.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.2/pydhcp/exceptions.py` & `pydhcp3-0.0.4/pydhcp/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 #** Variables **#
 __all__ = [
     'make_error',
 
     'DhcpError',
     'NoAddrsAvailable',
     'NotAllowed',
+    'NotSupported',
     'MalformedQuery',
     'Terminated',
+    'UnknownQueryType',
 ]
 
 _EXCEPTIONS: Dict[StatusCode, Type[Exception]] = {}
 
 #** Functions **#
 
 def make_error(code: StatusCode, message: Any = None):
@@ -50,12 +52,18 @@
 
 class NoAddrsAvailable(DhcpError):
     code = StatusCode.NoAddrsAvail
 
 class NotAllowed(DhcpError):
     code = StatusCode.NotAllowed
 
+class NotSupported(DhcpError):
+    code = StatusCode.NotSupported
+
 class MalformedQuery(DhcpError):
     code = StatusCode.MalformedQuery
 
+class UnknownQueryType(DhcpError):
+    code = StatusCode.UnknownQueryType
+
 class Terminated(DhcpError):
     code = StatusCode.QueryTerminated
```

### Comparing `pydhcp3-0.0.2/pydhcp/v4/__init__.py` & `pydhcp3-0.0.4/pydhcp/v4/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,25 +11,29 @@
     'Message',
 
     'Option',
     'OptionList',
     'OptEnd',
     'OptServerId',
     'OptSubnetMask',
+    'OptBroadcast',
     'OptRouter',
     'OptDNS',
     'OptRequestedAddr',
     'OptIPLeaseTime',
+    'OptRenwalTime',
+    'OptRebindTime',
     'OptMessageType',
     'OptParamRequestList',
     'OptMaxMessageSize',
     'OptClassIdentifier',
     'OptTFTPServerName',
     'OptTFTPServerIP',
     'OptBootFile',
+    'OptPXEPathPrefix',
     'OptUserClassInfo',
     'OptClientSystemArch',
     'OptClientNetworkIface',
     'OptClientMachineID',
     'OptEtherBoot',
 ]
```

### Comparing `pydhcp3-0.0.2/pydhcp/v4/enum.py` & `pydhcp3-0.0.4/pydhcp/v4/enum.py`

 * *Files 9% similar despite different names*

```diff
@@ -125,14 +125,16 @@
     # Option 96 returned in RFC 3679
     ClientMachineIdentifier     = 97
     OpenGroupUserAuthentication = 98
     GeoConfCivic                = 99
     IEEE10031TZString           = 100
     ReferenceToTZDatabase       = 101
     # Options 102-111 returned in RFC 3679
+    Ipv6OnlyPreferred          = 108 # [RFC8925]
+    OPTION_DHCP4O6_S46_SADDR   = 109 # [RFC8539]
     NetInfoParentServerAddress = 112
     NetInfoParentServerTag     = 113
     URL                        = 114
     # Option 115 returned in RFC 3679
     AutoConfigure                   = 116
     NameServiceSearch               = 117
     SubnetSelection                 = 118
@@ -157,33 +159,48 @@
     CAPWAPAccessControllerAddresses       = 138
     OPTIONIPv4AddressMoS                  = 139
     OPTIONIPv4FQDNMoS                     = 140
     SIPUAConfigurationServiceDomains      = 141
     OPTIONIPv4AddressANDSF                = 142
     OPTIONIPv6AddressANDSF                = 143
     # Options 144-149 returned in RFC 3679
-    TFTPServerAddress = 150
-    StatusCode        = 151
-    BaseTime          = 152
-    StartTimeOfState  = 153
-    QueryStartTime    = 154
-    QueryEndTime      = 155
-    DHCPState         = 156
-    DataSource        = 157
+    GeoLoc                   = 144 #[RFC6225]
+    FORCERENEW_NONCE_CAPABLE = 145 #[RFC6704]
+    RDNSSSelection           = 146 #[RFC6731]
+    OPTION_V4_DOTS_RI        = 147 #[RFC8973]
+    OPTION_V4_DOTS_ADDRESS   = 148 #[RFC8973]
+    TFTPServerAddress        = 150
+    StatusCode               = 151
+    BaseTime                 = 152
+    StartTimeOfState         = 153
+    QueryStartTime           = 154
+    QueryEndTime             = 155
+    DHCPState                = 156
+    DataSource               = 157
     # Options 158-174 returned in RFC 3679
+    OPTION_V4_PCP_SERVER             = 158 #[RFC7291]
+    OPTION_V4_PORTPARAMS             = 159 #[RFC7618]
+    OPTION_MUD_URL_V4                = 161 #[RFC8520]
+    OPTION_V4_DNR                    = 162 #[RFC-ietf-add-dnr-13] 
     Etherboot                        = 175
     IPTelephone                      = 176
     EtherbootPacketCableAndCableHome = 177
     # Options 178-207 returned in RFC 3679
+    HPDMServer           = 202 #[HP Device-Manager 4.7]
+    HPDMGateway          = 203 #[HP Device-Manager 4.7]
     PXELinuxMagicString  = 208
     PXELinuxConfigFile   = 209
     PXELinuxPathPrefix   = 210
     PXELinuxRebootTime   = 211
     OPTION6RD            = 212
     OPTIONv4AccessDomain = 213
     # Options 214-219 returned in RFC 3679
     SubnetAllocation        = 220
     VirtualSubnetAllocation = 221
     # Options 222-223 returned in RFC 3679
     # Options 224-254 are reserved for private use
-    ProxyAutoDiscover = 252
-    End               = 255
+    FortinetManagerIP      = 240 #[FortiNet FortiManager]
+    FortinetManagerDomain  = 241 #[FortiNet FortiManager]
+    MSClasslessStaticRoute = 249
+    MSEncodingLongOption   = 250
+    ProxyAutoDiscover      = 252 #[RFC-draft-ietf-wrec-wpad-01]
+    End                    = 255
```

### Comparing `pydhcp3-0.0.2/pydhcp/v4/message.py` & `pydhcp3-0.0.4/pydhcp/v4/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,78 @@
 """
 DHCPv4 Message Implementation
 """
-from dataclasses import dataclass
 from ipaddress import IPv4Address
-from typing import Union, List, Optional
-from typing_extensions import Self
+from typing import List, Optional
+from typing_extensions import Annotated, Self
 
 from pystructs import *
+from pyderive import dataclass
 
 from .enum import MessageType, OpCode, OptionCode
 from .options import OptionList, read_option, write_option
 from ..enum import HwType
 
 #** Variables **#
 __all__ = ['Message']
 
 #: magic cookie to include in DHCP message
 MAGIC_COOKIE = bytes([0x63, 0x82, 0x53, 0x63])
 
 #: zeroed ip-address default for message values
 ZeroIp = IPv4Address('0.0.0.0')
 
-#: valid types supported for ip-address assignment
-IpType = Union[str, bytes, IPv4Address]
-
 #** Functions **#
 
 def get_ip(op: OptionCode, options: OptionList) -> Optional[IPv4Address]:
     """translate option value into ipv4-address"""
     option = options.get(op)
     if not option:
         return
     ip = option.value
     if not isinstance(ip, IPv4Address):
         ip = IPv4Address(ip)
     return ip
 
 #** Classes **#
 
-@struct
-class Header:
+class Header(Struct):
     """DHCPv4 Message Header Group"""
-    opcode:       Int[8, OpCode, 'OpCode']
-    hw_type:      Int[8, HwType, 'HwType'] 
-    hw_length:    Int8
-    hops:         Int8
-    message_id:   Int32
-    seconds:      Int16
-    flags:        Int16
-    client_addr:  Ipv4
-    your_addr:    Ipv4
-    server_addr:  Ipv4
-    gateway_addr: Ipv4
-    hw_addr:      StaticBytes[16]
-    server_name:  StaticBytes[64]
-    boot_file:    StaticBytes[128]
-    magic_cookie: Const[MAGIC_COOKIE]
+    opcode:       Annotated[OpCode, Wrap[U8, OpCode]]
+    hw_type:      Annotated[HwType, Wrap[U8, HwType]]
+    hw_length:    U8
+    hops:         U8
+    message_id:   U32
+    seconds:      U16
+    flags:        U16
+    client_addr:  IPv4
+    your_addr:    IPv4
+    server_addr:  IPv4
+    gateway_addr: IPv4
+    hw_addr:      Annotated[bytes, StaticBytes[16]]
+    server_name:  Annotated[bytes, StaticBytes[64]]
+    boot_file:    Annotated[bytes, StaticBytes[128]]
+    magic_cookie: Annotated[bytes, Const[MAGIC_COOKIE]] = MAGIC_COOKIE
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class Message:
     op:           OpCode
     id:           int
     client_hw:    bytes
     options:      OptionList
-    hw_type:      HwType = HwType.Ethernet
-    hops:         int    = 0
-    seconds:      int    = 0
-    flags:        int    = 0
-    client_addr:  IpType = ZeroIp
-    your_addr:    IpType = ZeroIp
-    server_addr:  IpType = ZeroIp
-    gateway_addr: IpType = ZeroIp 
-    server_name:  bytes  = b''
-    boot_file:    bytes  = b''
+    hw_type:      HwType   = HwType.Ethernet
+    hops:         int      = 0
+    seconds:      int      = 0
+    flags:        int      = 0
+    client_addr:  Ipv4Type = ZeroIp
+    your_addr:    Ipv4Type = ZeroIp
+    server_addr:  Ipv4Type = ZeroIp
+    gateway_addr: Ipv4Type = ZeroIp 
+    server_name:  bytes    = b''
+    boot_file:    bytes    = b''
  
     def __repr__(self) -> str:
         cname = self.__class__.__name__
         op    = self.op.name
         htype = self.hw_type.name 
         return f'{cname}(op={op}, id={self.id!r}, hwtype={htype})'
```

### Comparing `pydhcp3-0.0.2/pydhcp/v4/options.py` & `pydhcp3-0.0.4/pydhcp/v6/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 """
-DHCPv4 Option Implementations
+DHCPv6 Option Implementations
 """
-from dataclasses import dataclass
 from typing import ClassVar
+from typing_extensions import Annotated, Self
 
 from pystructs import *
+from pyderive import dataclass
 
-from .enum import OptionCode, MessageType
-from ..enum import Arch, StatusCode
-from ..base import DHCPOption, DHCPOptionList, Timedelta
+from .duid import DUID, read_duid, write_duid
+from .enum import OptionCode
+from ..enum import StatusCode
+from ..base import DHCPOption, DHCPOptionList, Microseconds, Seconds
 
 #** Variables **#
 __all__ = [
     'read_option',
 
     'Option',
     'OptionList',
-    'OptEnd',
-    'OptServerId',
-    'OptSubnetMask',
-    'OptRouter',
-    'OptDNS',
-    'OptRequestedAddr',
+    'OptClientIdentifier',
+    'OptServerIdentifier',
+    'OptNonTemporaryAddr',
+    'OptTemporaryAddress',
+    'OptAddress',
+    'OptRequestList',
+    'OptPreference',
+    'OptElapsed',
+    'OptRelay',
+    'OptAuth',
+    'OptUnicast',
     'OptStatusCode',
-    'OptIPLeaseTime',
-    'OptMessageType',
-    'OptParamRequestList',
-    'OptMaxMessageSize',
-    'OptClassIdentifier',
-    'OptTFTPServerName',
-    'OptTFTPServerIP',
-    'OptBootFile',
-    'OptUserClassInfo',
-    'OptClientSystemArch',
-    'OptClientNetworkIface',
-    'OptClientMachineID',
-    'OptEtherBoot',
+    'OptIdAssocPrefixDeleg',
+    'OptIAPrefix',
 ]
 
-#: codec to parse Int8 as OptionCode
-OptionCodeInt = Int[8, OptionCode, 'OptionCode']
+#: integer codec ot parse option-code
+OptionCodeInt = Annotated[OptionCode, Wrap[U16, OptionCode]]
 
 #** Functions **#
 
 def read_option(ctx: Context, raw: bytes) -> 'Option':
     """
     read and deserialize best option-class to match option content
     
@@ -57,134 +53,137 @@
     # parse option w/ it's own sub-context
     subctx = Context()
     option = oclass.decode(subctx, opt.value)
     if oclass is Option:
         oclass.opcode = opt.code
     return option
 
-def write_option(ctx: Context, option) -> bytes:
+def write_option(ctx: Context, option: 'Option') -> bytes:
     """
     write and serialize option-class into raw-bytes
     
     :param ctx: serialization context
     :param raw: option object to serialize
     :return:    serialized bytes
     """
     # serialize option into bytes
     subctx  = Context()
     content = option.encode(subctx)
     return OptStruct(option.opcode, content).encode(ctx)
 
 #** Classes **#
 
-@struct
-class OptStruct:
+class OptStruct(Struct):
     code:  OptionCodeInt
-    value: SizedBytes[8]
+    value: Annotated[bytes, SizedBytes[U16]]
 
-@dataclass
 class Option(DHCPOption):
-    """DHCPv4 BaseClass Option Definition"""
-    opcode: ClassVar[OptionCode] = OptionCode.OptionPad
+    """DHCPv6 BaseClass Option Definition"""
+    opcode: ClassVar[OptionCode] = OptionCode.UNKNOWKN
 
 class OptionList(DHCPOptionList):
-    """DHCPv4 DHCPOptionList Implementation"""
+    """DHCPv6 DHCPOptionList Implementation"""
     pass
 
-### SubClasses
+class _DuidOption(Option):
+    """BaseClass to Support DUID Option Implementations"""
+    opcode: ClassVar[OptionCode]
+    value:  DUID
 
-class OptEnd(Option):
-    opcode = OptionCode.End
+    def encode(self, ctx: Context) -> bytes:
+        return write_duid(self.value)
 
-class OptHostName(Option):
-    opcode = OptionCode.HostName
+    @classmethod
+    def decode(cls, ctx: Context, value: bytes) -> Self:
+        return cls(read_duid(value))
 
-@struct
-class _Ipv4Option(Option):
-    opcode: ClassVar[OptionCode]
-    value:  Ipv4
+class OptClientIdentifier(_DuidOption):
+    opcode = OptionCode.ClientIdentifier
 
-class OptServerId(_Ipv4Option):
+class OptServerIdentifier(_DuidOption):
     opcode = OptionCode.ServerIdentifier
 
-class OptSubnetMask(_Ipv4Option):
-    opcode = OptionCode.SubnetMask
+class OptNonTemporaryAddr(Option):
+    opcode = OptionCode.NonTemporaryAddress
+    value:   U32
+    t1:      U32
+    t2:      U32
+    options: GreedyBytes
+
+class OptTemporaryAddress(Option):
+    opcode = OptionCode.TemporaryAddress
+    value:   U32
+    options: GreedyBytes
+
+class OptAddress(Option):
+    opcode = OptionCode.Address
+    value:          IPv6
+    pref_lifetime:  Annotated[Seconds, Wrap[U32, Seconds]]
+    valid_lifetime: Annotated[Seconds, Wrap[U32, Seconds]]
+    options:        GreedyBytes
 
-class OptRouter(_Ipv4Option):
-    opcode = OptionCode.Router
-
-class OptDNS(_Ipv4Option):
-    opcode = OptionCode.DomainNameServer
+class OptRequestList(Option):
+    opcode = OptionCode.OptionRequest
+    value: GreedyList[OptionCodeInt]
 
-class OptRequestedAddr(_Ipv4Option):
-    opcode = OptionCode.RequestedIPAddress
+class OptPreference(Option):
+    opcode = OptionCode.Preference
+    value: U8
+
+class OptElapsed(Option):
+    opcode = OptionCode.ElapsedTime
+    value: Annotated[Microseconds, Wrap[U16, Microseconds]]
+
+class OptRelay(Option):
+    opcode = OptionCode.RelayMessage
+    value: GreedyBytes
+
+class OptAuth(Option):
+    value: ClassVar[int] # remove value as init-arg
+    opcode = OptionCode.Authentication
+    protocol:   U8
+    algorithm:  U8
+    rdm:        U8
+    replay_det: StaticBytes[8]
+    info:       GreedyBytes
+
+class OptUnicast(Option):
+    opcode = OptionCode.ServerUnicast
+    value: IPv6
 
-@struct
 class OptStatusCode(Option):
     opcode = OptionCode.StatusCode
-    value:   Int[8, StatusCode, 'StatusCode']
+    value:   Annotated[StatusCode, Wrap[U16, StatusCode]]
     message: GreedyBytes
 
-@struct
-class OptIPLeaseTime(Option):
-    opcode = OptionCode.IPAddressLeaseTime
-    value: Int[32, Timedelta['seconds'], 'Lease']
-
-@struct
-class OptMessageType(Option):
-    opcode = OptionCode.DHCPMessageType
-    value: Int[8, MessageType, 'MessageType']
-
-@struct
-class OptParamRequestList(Option):
-    opcode = OptionCode.ParameterRequestList
-    value: GreedyList[OptionCodeInt]
-
-@struct
-class OptMaxMessageSize(Option):
-    opcode = OptionCode.MaximumDHCPMessageSize
-    value: Int16
-
-class OptClassIdentifier(Option):
-    opcode = OptionCode.ClassIdentifier
-
-class OptTFTPServerName(Option):
-    opcode = OptionCode.TFTPServerName
-
-class OptTFTPServerIP(Option):
-    opcode = OptionCode.TFTPServerIPAddress
-
-class OptBootFile(Option):
-    opcode = OptionCode.BootfileName
-
-class OptUserClassInfo(Option):
-    opcode = OptionCode.UserClassInformation
-
-@struct
-class OptClientSystemArch(Option):
-    opcode = OptionCode.ClientSystemArchitectureType
-    value: GreedyList[Int[16, Arch, 'Arch']]
-
-@struct
-class OptClientNetworkIface(Option):
-    opcode = OptionCode.ClientNetworkInterfaceIdentifier
-    value: Const[b'\x01']
-    major: Int8
-    minor: Int8
-
-@struct
-class OptClientMachineID(Option):
-    opcode = OptionCode.ClientMachineIdentifier
-    prefix: Const[b'\x00']
-    value:  GreedyBytes
-
-class OptEtherBoot(Option):
-    opcode = OptionCode.Etherboot
+class OptIdAssocPrefixDeleg(Option):
+    opcode = OptionCode.IdAssocPrefixDeleg
+    value:   U32
+    t1:      Annotated[Seconds, Wrap[U32, Seconds]]
+    t2:      Annotated[Seconds, Wrap[U32, Seconds]]
+    options: GreedyBytes
+ 
+    def read_options(self) -> OptionList:
+        ctx = Context()
+        options = OptionList()
+        while ctx.index < len(self.options):
+            option = read_option(ctx, self.options)
+            options.append(option)
+        return options
+
+class OptIAPrefix(Option):
+    value: ClassVar[int]
+    opcode = OptionCode.IAPrefix
+    pref_lifetime:  Annotated[Seconds, Wrap[U32, Seconds]]
+    valid_lifetime: Annotated[Seconds, Wrap[U32, Seconds]]
+    prefix_length:  U8
+    ipv6_prefix:    IPv6
+    options:        GreedyBytes
 
 #** Init **#
 
 #: map of option-codes to option-subclasses
 OPTIONS = {
     value.opcode:value
-    for value in globals().values()
-    if isinstance(value, type) and issubclass(value, Option) 
+    for name, value in globals().items()
+    if not name.startswith('_') and isinstance(value, type) and issubclass(value, Option) 
 }
```

### Comparing `pydhcp3-0.0.2/pydhcp/v4/server/server.py` & `pydhcp3-0.0.4/pydhcp/v4/server/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,79 @@
 """
 PyServe Session DHCPv4 Implementation
 """
 from abc import ABC, abstractmethod
 from ipaddress import IPv4Address
 from logging import Logger, getLogger
-from dataclasses import dataclass, field
-from typing import Optional
+from typing import Callable, List, NamedTuple, Optional
 
-from pyserve import Address, Writer
+from pyserve import Address, UdpWriter
 from pyserve import Session as BaseSession
+from pyderive import dataclass, field
 
-from .backend import Backend
-from ..enum import MessageType, OpCode
-from ..message import Message
+from ..enum import MessageType, OpCode, OptionCode
+from ..message import IpType, Message
 from ..options import *
 from ...enum import StatusCode
-from ...exceptions import DhcpError, NotAllowed, MalformedQuery
+from ...exceptions import DhcpError, NotAllowed, UnknownQueryType
 
 #** Variables **#
-__all__ = ['Session', 'SimpleSession']
+__all__ = ['HandlerFunc', 'Context', 'Session', 'SimpleSession']
+
+#: dhcp response port
+PORT = 68
 
 #: broadcast request for responding to messages
-BROADCAST = '255.255.255.255'
+BROADCAST = IPv4Address('255.255.255.255')
+
+#: required opcodes to preserve even when not requested
+REQUIRED = {
+    OptionCode.DHCPMessageType, 
+    OptionCode.ServerIdentifier,
+    OptionCode.IPAddressLeaseTime,
+}
+
+#: function definition for session processing callback
+HandlerFunc = Callable[['Context'], None]
+
+#: logger generation function
+logger = getLogger('pydhcp.v4')
 
 #** Functions **#
 
+def is_zero(host: IpType) -> bool:
+    """check if host-ip is zeroed"""
+    return len(IPv4Address(host).packed.strip(b'\x00')) == 0
+
+def find_host(*ips: IpType) -> IPv4Address:
+    """search through available ips to find first non-zero available"""
+    for ip in (IPv4Address(ip) for ip in ips):
+        if not is_zero(ip):
+            return ip
+    raise RuntimeError(f'No NonZero IPs: {ips!r}')
+
 def mac_address(hwaddr: bytes) -> str:
     """translate hardware address to mac"""
     return ':'.join(f'{c:02x}' for c in hwaddr)
 
+def validate_options(ctx: 'Context'):
+    """validate and filter options based on requested operation-codes"""
+    options   = OptionList()
+    requested = set(ctx.request.requested_options())
+    for option in ctx.response.options:
+        if option.opcode in requested or option.opcode in REQUIRED:
+            options.append(option)
+    options.sort()
+    ctx.response.options = options
+
 #** Classes **#
 
 @dataclass
 class Session(BaseSession, ABC):
-    backend:   Backend
-    logger:    Logger = field(default_factory=lambda: getLogger('pydhcp'))
-    server_id: Optional[IPv4Address] = None
+    logger: Logger = logger
 
     ## Overrides
 
     @abstractmethod
     def process_discover(self, req: Message) -> Optional[Message]:
         raise NotImplementedError 
 
@@ -67,18 +101,36 @@
         """Generate Default DHCP Response"""
         return Message(
             op=OpCode.BootReply,
             id=req.id,
             client_hw=req.client_hw,
             options=OptionList(),
         )
+ 
+    def send(self, request: Message, response: Message):
+        """send completed response message"""
+        hosts = (
+            request.gateway_addr,
+            request.client_addr,
+            IPv4Address(self.addr.host),
+            BROADCAST,
+        )
+        # encode and send response
+        data = response.encode()
+        for ipv4 in hosts:
+            if is_zero(ipv4):
+                continue
+            host = str(ipv4)
+            info = f'{self.addr_str} | sent {len(data)} bytes to {host}:{PORT}'
+            self.logger.debug(info)
+            self.writer.write(data, addr=(host, PORT))
 
     ## Session Impl
 
-    def connection_made(self, addr: Address, writer: Writer):
+    def connection_made(self, addr: Address, writer: UdpWriter):
         """handle session initialization on connection-made"""
         self.addr      = addr
         self.writer    = writer
         self.addr_str  = '%s:%d' % self.addr
 
     def data_recieved(self, data: bytes):
         """recieve DHCPv4 request and generate response"""
@@ -111,100 +163,120 @@
         except Exception as e:
             nak      = OptMessageType(MessageType.Nak)
             status   = OptStatusCode(StatusCode.UnspecFail, str(e).encode())
             response = response or self.default_response(request)
             response.options.extend([nak, status])
             raise e
         finally:
-            if response is None:
+            if response is not None:
+                self.send(request, response)
+            else:
                 self.logger.error(f'{self.addr_str} | No Response Given.')
                 self.writer.close()
-            else:
-                # apply server-identifier when given
-                if self.server_id:
-                    response.options.append(OptServerId(self.server_id))
-                # encode and send response
-                data = response.encode()
-                self.logger.debug(f'{self.addr_str} | sent {len(data)} bytes')
-                self.writer.write(data, addr=(BROADCAST, self.addr.port))
 
     def connection_lost(self, err: Optional[Exception]):
         """debug log connection lost"""
-        self.logger.debug(f'{self.addr_str} | connection-lost err={err}')
+        msg = f'{self.addr_str} | connection-lost err={err}'
+        log = self.logger.warning if err is not None else self.logger.debug
+        log(msg)
+
+class Context(NamedTuple):
+    """Session Context to Pass to Handler Functions"""
+    session:  Session
+    request:  Message
+    response: Message
 
-@dataclass
+@dataclass(slots=True)
 class SimpleSession(Session):
-    backend: Backend
-    logger:  Logger = field(default_factory=lambda: getLogger('pydhcp'))
+    """Simplified DHCP Server Implementation"""
+    logger:    Logger
+    server_id: IPv4Address
+    handlers:  List[HandlerFunc] = field(default_factory=list)
+    releasers: List[HandlerFunc] = field(default_factory=list)
+ 
+    def __post_init__(self):
+        if not self.handlers:
+            raise ValueError('SimpleSession Handlers Empty!')
 
     def process_discover(self, req: Message) -> Optional[Message]:
-        """process discover according to backend"""
-        # retrieve and log assignment
-        mac    = req.client_hw.hex()
-        answer = self.backend.get_assignment(req.client_hw)
-        assign = answer.assign
-        self.logger.info(f'{self.addr_str} | DISCOVER {mac} {answer}')
-        # offer assignment on discover 
+        """process incoming discover request"""
+        msg = OptMessageType(MessageType.Offer)
         res = self.default_response(req)
-        res.your_addr = assign.your_addr
-        res.options.extend([
-            OptMessageType(MessageType.Offer),
-            OptDNS(assign.dns),
-            OptRouter(assign.gateway),
-            OptSubnetMask(assign.netmask),
-            OptIPLeaseTime(assign.lease_seconds),
-        ])
+        ctx = Context(self, req, res)
+        res.server_addr = self.server_id
+        for func in self.handlers:
+            func(ctx)
+        res.options.setdefault(OptServerId(self.server_id))
+        res.options.setdefault(msg)
+        validate_options(ctx)
+        res.options.move_to_start(msg.opcode)
+        # ensure your-ip is set during exchange
+        if not res.your_addr:
+            raise RuntimeError(f'Handlers Failed to Assign Client-IP')
         return res
 
     def process_request(self, req: Message) -> Optional[Message]:
-        """process request according to backend"""
-        # retrieve and log assignment
-        mac    = req.client_hw.hex()
-        answer = self.backend.get_assignment(req.client_hw)
-        assign = answer.assign
-        self.logger.info(f'{self.addr_str} | REQUEST {mac} {answer}')
-        # build standard response
+        """process incoming dhcp request"""
+        msg = OptMessageType(MessageType.Ack)
         res = self.default_response(req)
-        res.your_addr = assign.your_addr
-        res.options.extend([
-            OptMessageType(MessageType.Ack),
-            OptDNS(assign.dns),
-            OptRouter(assign.gateway),
-            OptSubnetMask(assign.netmask),
-            OptIPLeaseTime(assign.lease_seconds),
-        ])
-        # check if request conflicts with server assignment
+        ctx = Context(self, req, res)
+        res.server_addr = self.server_id
+        for handler in self.handlers:
+            handler(ctx)
+        res.options.setdefault(OptServerId(self.server_id))
+        res.options.setdefault(msg)
+        validate_options(ctx)
+        res.options.move_to_start(msg.opcode)
+        # ensure your-ip is set during exchange
+        if not res.your_addr:
+            raise RuntimeError(f'Handlers Failed to Assign Client-IP')
+        # ensure assignment matches request
+        netmask  = res.options.get(OptSubnetMask.opcode)
+        netmask  = netmask.value if netmask else None
         req_addr = req.requested_address()
-        conflict = req_addr != assign.your_addr
-        conflict = conflict or req.broadcast_address() == assign.netmask
+        req_cast = req.broadcast_address()
+        conflict = req_addr and req_addr != res.your_addr
+        conflict = conflict or req_cast and req_cast != netmask
         if conflict:
             self.logger.warning(f'{self.addr_str} | REQUEST NAK {req_addr!r}')
             nak = OptMessageType(MessageType.Nak)
-            res.options.set(nak.opcode, nak)
+            res.options.set(nak)
         return res
 
     def process_decline(self, req: Message) -> Optional[Message]:
-        """process decline message according to backend"""
-        mac    = mac_address(req.client_hw)
-        assign = self.backend.get_assignment(req.client_hw).assign
-        self.logger.info(f'{self.addr_str} | DECLINE {mac} {assign.client}')
-        self.backend.del_assignment(req.client_hw)
+        """process incoming decline response"""
+        mac = mac_address(req.client_hw)
         res = self.default_response(req)
-        res.options.append(OptMessageType(MessageType.Nak))
+        msg = OptMessageType(MessageType.Nak)
+        ctx = Context(self, req, res)
+        res.server_addr = self.server_id
+        self.logger.info(f'{self.addr_str} | DECLINE {mac} {req.client_addr}')
+        for func in self.releasers:
+            func(ctx)
+        res.options.setdefault(OptServerId(self.server_id))
+        res.options.setdefault(msg)
+        validate_options(ctx)
+        res.options.move_to_start(msg.opcode)
         return res
 
     def process_release(self, req: Message) -> Optional[Message]:
-        """process release message according to backend"""
-        mac    = mac_address(req.client_hw)
-        assign = self.backend.get_assignment(req.client_hw).assign
-        self.logger.info(f'{self.addr_str} | RELEASE {mac} {assign.client}')
-        self.backend.del_assignment(req.client_hw)
+        """process incoming release request"""
+        mac = mac_address(req.client_hw)
         res = self.default_response(req)
-        res.options.append(OptMessageType(MessageType.Ack))
+        msg = OptMessageType(MessageType.Ack)
+        ctx = Context(self, req, res)
+        res.server_addr = self.server_id
+        self.logger.info(f'{self.addr_str} | RELEASE {mac} {req.client_addr}')
+        for func in self.releasers:
+            func(ctx)
+        res.options.setdefault(OptServerId(self.server_id))
+        res.options.setdefault(msg)
+        validate_options(ctx)
+        res.options.move_to_start(msg.opcode)
         return res
 
-    def process_inform(self, req: Message) -> Optional[Message]:
-        """process inform message according to backend"""
+    def process_inform(self, _: Message) -> Optional[Message]:
+        """process incoming inform request"""
         raise NotAllowed('Inform not Allowed')
  
-    def process_unknown(self, req: Message) -> Optional[Message]:
-        raise MalformedQuery('Unsupported MessageType')
+    def process_unknown(self, _: Message) -> Optional[Message]:
+        raise UnknownQueryType('Unsupported MessageType')
```

### Comparing `pydhcp3-0.0.2/pydhcp/v6/duid.py` & `pydhcp3-0.0.4/pydhcp/v6/duid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 DHCP Unique Identifier (DUID) Implementations (rfc8415 section-11)
 """
 from datetime import datetime, timedelta, timezone
 from typing import ClassVar
+from typing_extensions import Annotated
 
 from pystructs import *
 
 from .enum import DuidType
 from ..enum import HwType
 
 #** Variables **#
@@ -18,38 +19,38 @@
     'LinkLayerPlusTime',
     'EnterpriseNumber',
     'LinkLayer',
     'UniqueIdentifier',
 ]
 
 #: codec handler for HwType enum
-HwInt = Int[16, HwType, 'HwType']
+HwInt = Annotated[HwType, Wrap[U16, HwType]]
 
 #: January 1, 2000 UTC
 EPOCH = datetime(year=2000, month=1, day=1, tzinfo=timezone.utc)
 
 #** Functions **#
 
 def read_duid(raw: bytes) -> 'DUID':
     """
     read duid struct from raw bytes
     """
     ctx    = Context()
-    duid   = DuidType(Int16.decode(ctx, raw))
+    duid   = DuidType(decode(ctx, raw, U8))
     dclass = DUIDS.get(duid, None)
     if dclass is None:
         raise ValueError(f'Unsupported DUID: {duid!r}')
     return dclass.decode(ctx, raw)
 
 def write_duid(duid: 'DUID'):
     """
     serialize duid struct into raw bytes
     """
     ctx = Context()
-    return Int16.encode(ctx, duid.duid) + duid.encode(ctx)
+    return encode(ctx, U16, duid.duid) + duid.encode(ctx)
 
 #** Classes **#
 
 class Datetime(datetime):
  
     def __new__(cls, time: int, *args):
         # support standard datetime actions when extra vars are passed
@@ -62,35 +63,31 @@
 
     def __int__(self) -> int:
         return int(self.timestamp())
 
 class DUID(Struct):
     duid: ClassVar[DuidType]
 
-@struct
 class LinkLayerPlusTime(DUID):
     duid = DuidType.LinkLayerPlusTime
     hw_type: HwInt
-    time:    Int[32, Datetime, 'Datetime']
+    time:    Annotated[int, Wrap[U32, Datetime]]
     address: GreedyBytes
 
-@struct
 class EnterpriseNumber(DUID):
     duid = DuidType.EnterpriseNumber
-    en:         Int16
-    en_contd:   Int16
+    en:         U16
+    en_contd:   U16
     identifier: GreedyBytes
 
-@struct
 class LinkLayer(DUID):
     duid = DuidType.LinkLayer
     hw_type: HwInt
     address: GreedyBytes
 
-@struct
 class UniqueIdentifier(DUID):
     duid = DuidType.UniqueIdentifier
     uuid: StaticBytes[128]
 
 #** Classes **#
 
 #: map of duid enum to valid subclasses
```

### Comparing `pydhcp3-0.0.2/pydhcp/v6/enum.py` & `pydhcp3-0.0.4/pydhcp/v6/enum.py`

 * *Files identical despite different names*

### Comparing `pydhcp3-0.0.2/pydhcp/v6/message.py` & `pydhcp3-0.0.4/pydhcp/v6/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 DHCPv6 Message Implementation
 """
-from dataclasses import dataclass, field, asdict
 from ipaddress import IPv6Address
 from typing import Union
-from typing_extensions import Self
+from typing_extensions import Annotated, Self
 
-from pystructs import Context, Int, Int16, Ipv6, struct
+from pystructs import *
+from pyderive import dataclass, field, asdict
 
 from .enum import MessageType
 from .options import OptionList, read_option
 
 #** Variables **#
 __all__ = ['Message']
 
 #: codec type to support MessageType
-MessageInt = Int[8, MessageType, 'MessageType']
-
-#: valid types supported for ipv6-address
-IpType = Union[str, bytes, IPv6Address]
+MessageInt = Annotated[MessageType, Wrap[U8, MessageType]]
 
 #** Functions **#
 
 def read_options(ctx: Context, raw: bytes) -> OptionList:
     """read options from raw-bytes and return options-list"""
     options = OptionList()
     while ctx.index < len(raw):
@@ -33,33 +30,30 @@
 def write_options(ctx: Context, data: bytearray, options: OptionList):
     """serialize options into bytearray"""
     for option in options:
         data += option.encode(ctx)
 
 #** Classes **#
 
-@struct
-class MsgHeader:
+class MsgHeader(Struct):
     op: MessageInt
-    id: Int[24]
+    id: U24
 
-@struct
-class RelayForwardHeader:
+class RelayForwardHeader(Struct):
     op:        MessageInt
-    hops:      Int16
-    link_addr: Ipv6
-    peer_addr: Ipv6
+    hops:      U16
+    link_addr: IPv6
+    peer_addr: IPv6
 
-@struct
-class RelayReplyHeader:
+class RelayReplyHeader(Struct):
     op:        MessageInt
-    link_addr: Ipv6
-    peer_addr: Ipv6 
+    link_addr: IPv6
+    peer_addr: IPv6
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class Message:
     op:      MessageType
     id:      int
     options: OptionList = field(default_factory=OptionList)
  
     def __repr__(self) -> str:
         cname = self.__class__.__name__
@@ -81,20 +75,19 @@
         Decode DHCPv6 client/server message from bytes
         """
         ctx     = Context()
         header  = MsgHeader.decode(ctx, raw)
         options = read_options(ctx, raw)
         return cls(header.op, header.id, options)
 
-
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class RelayReplyMessage:
     op:        MessageType
-    link_addr: IpType
-    peer_addr: IpType
+    link_addr: Ipv6Type
+    peer_addr: Ipv6Type
     options:   OptionList 
 
     def __repr__(self) -> str:
         cname  = self.__class__.__name__
         values = ' '.join(f'{k}={v}' for k, v in {
             'op':  self.op.name,
             'hops':getattr(self, 'hops', None), 
@@ -108,35 +101,35 @@
         Encode DHCPv6 RelayReply message into bytes
         """
         fields = asdict(self)
         fields.pop('options', None)
         # serialize content
         ctx   = Context()
         data  = bytearray()
-        data += RelayForwardHeader(**fields).encode(ctx)
+        data += RelayReplyHeader(**fields).encode(ctx)
         write_options(ctx, data, self.options)
         return bytes(data)
-    
+ 
     @classmethod
     def decode(cls, raw: bytes) -> Self:
         """
         Decode DHCPv6 RelayReply message from bytes
         """
         ctx     = Context()
-        header  = MsgHeader.decode(ctx, raw)
+        header  = RelayReplyHeader.decode(ctx, raw)
         fields  = asdict(header) #type: ignore
         options = read_options(ctx, raw)
         return cls(options=options, **fields)
 
-@dataclass(repr=False)
+@dataclass(slots=True, repr=False)
 class RelayForwardMessage(RelayReplyMessage):
     op:        MessageType
     hops:      int
-    link_addr: IpType
-    peer_addr: IpType
+    link_addr: Ipv6Type
+    peer_addr: Ipv6Type
     options:   OptionList
 
     def encode(self) -> bytes:
         """
         Encode DHCPv6 RelayForward message into bytes
         """
         ctx   = Context()
@@ -148,15 +141,15 @@
 
     @classmethod
     def decode(cls, raw: bytes) -> Self:
         """
         Decode DHCPv6 RelayForward message from bytes
         """
         ctx     = Context()
-        header  = MsgHeader.decode(ctx, raw)
+        header  = RelayForwardHeader.decode(ctx, raw)
         options = read_options(ctx, raw)
         return cls(
             op=header.op, 
             hops=header.hops, 
             link_addr=header.link_addr, 
             peer_addr=header.peer_addr, 
             options=options
```

### Comparing `pydhcp3-0.0.2/pydhcp3.egg-info/PKG-INFO` & `pydhcp3-0.0.4/pydhcp3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydhcp3
-Version: 0.0.2
+Version: 0.0.4
 Summary: Simple Python DHCP Library. DHCP Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydhcp
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydhcp3-0.0.2/pydhcp3.egg-info/SOURCES.txt` & `pydhcp3-0.0.4/pydhcp3.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 pydhcp/enum.py
 pydhcp/exceptions.py
 pydhcp/v4/__init__.py
 pydhcp/v4/enum.py
 pydhcp/v4/message.py
 pydhcp/v4/options.py
 pydhcp/v4/server/__init__.py
+pydhcp/v4/server/handlers.py
 pydhcp/v4/server/server.py
-pydhcp/v4/server/backend/__init__.py
-pydhcp/v4/server/backend/cache.py
 pydhcp/v6/__init__.py
 pydhcp/v6/duid.py
 pydhcp/v6/enum.py
 pydhcp/v6/message.py
 pydhcp/v6/options.py
 pydhcp3.egg-info/PKG-INFO
 pydhcp3.egg-info/SOURCES.txt
```

### Comparing `pydhcp3-0.0.2/setup.py` & `pydhcp3-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pydhcp3',
-    version='0.0.2',
+    version='0.0.4',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pydhcp',
     description="Simple Python DHCP Library. DHCP Packet-Parsing/Client/Server",
     long_description=readme,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     packages=find_packages(),
     install_requires=[
+        'pyserve3',
+        'pyderive3',
         'pystructs3',
-        'dataclasses',
         'typing_extensions'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```

