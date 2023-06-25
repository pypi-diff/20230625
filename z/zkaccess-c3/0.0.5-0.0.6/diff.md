# Comparing `tmp/zkaccess_c3-0.0.5.tar.gz` & `tmp/zkaccess_c3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkaccess_c3-0.0.5.tar", last modified: Wed Jun 14 20:29:04 2023, max compression
+gzip compressed data, was "zkaccess_c3-0.0.6.tar", last modified: Sun Jun 25 20:55:47 2023, max compression
```

## Comparing `zkaccess_c3-0.0.5.tar` & `zkaccess_c3-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/c3/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/controldevice.py
--rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/rtlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/c3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/cli/C3_CancelAlarms.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/cli/C3_Discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/cli/C3_GetDeviceParam.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/cli/C3_GetRTLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/cli/C3_OutputOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/tests/test_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/tests/test_controldevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/tests/test_crc16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/tests/test_rtlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-14 20:28:54.000000 zkaccess_c3-0.0.5/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:29:04.535470 zkaccess_c3-0.0.5/zkaccess_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-14 20:29:04.000000 zkaccess_c3-0.0.5/zkaccess_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-14 20:29:04.000000 zkaccess_c3-0.0.5/zkaccess_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:29:04.000000 zkaccess_c3-0.0.5/zkaccess_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 20:29:04.000000 zkaccess_c3-0.0.5/zkaccess_c3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.579343 zkaccess_c3-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/c3/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/c3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_CancelAlarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_Discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_GetDeviceParam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_GetRTLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/cli/C3_OutputOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 20:55:47.579343 zkaccess_c3-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_crc16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-25 20:55:35.000000 zkaccess_c3-0.0.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 20:55:47.575343 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-25 20:55:47.000000 zkaccess_c3-0.0.6/zkaccess_c3.egg-info/top_level.txt
```

### Comparing `zkaccess_c3-0.0.5/LICENSE` & `zkaccess_c3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/PKG-INFO` & `zkaccess_c3-0.0.6/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,78 @@
-Metadata-Version: 2.1
-Name: zkaccess_c3
-Version: 0.0.5
-Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
-Author-email: Vwout <vwout@users.noreply.github.com>
-Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
-Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # c3
 A native Python library for communicating with the ZKTeco ZKAccess C3 Access Control Panels.
 
 This library intends to implement the same functionality as provided by the ZKAccess C3 PullSDK API, but using native Python only.
 It is a port and extension of my (C3 Lua library)[../zkaccess-c3-lua].
 
 ## Usage
 To use the library, import the main class:
 ```
 from c3 import C3
 ```
 A panel connection can be created from the main class `C3`:
 ```
-    panel = C3()
-    if panel.connect(ip):
+    panel = C3(ip)
+    if panel.connect():
       panel.get_device_param(["~SerialNumber", "LockCount")
 ```
 To use the real-time log (RTLog), or control outputs, also include the helper classes from `controldevice` and `rtlog`.
 
+## Compatible devices
+The following devices are tested and known compatible:
+- C3-200 (firmware AC Ver 4.1.9 4609-03 Apr 7 2016)
+- C3-400 (firmware AC Ver 4.3.4 Apr 27 2017)
+
 ## Protocol
 The C3 access panels communicate using RS485 or TCP/IP.
 This library only support TCP/IP connections using IPv4.
 The connection is optionally secured by a password.
-Connections to C3 panels that use a password are not supported for this moment.
 
 The wire protocol for the access panels is binary, with the following datagram both for requests (from client to equipment) and responses:
 
 | Byte        | 0      | 1       | 2       | 3          | 4          | 5,6,7,8, ...  | n-2, n-1 | n       |
 |-------------|--------|---------|---------|------------|------------|---------------|----------|---------|
-| **Meaning** | Start  | Version | Command | Length Lsb | Length Msb | Data          | Checksum | End     |
+| **Meaning** | Start  | Version | Command | Length LSB | Length MSB | Data          | Checksum | End     |
 |  **Value**  | `0xAA` | `0x01`  |         |            |            |               |          | `0x55`  |
 
-The start bytes 0, 1 and last byte have a fixed value.
-The *Command* is one of the following (only listing commands supported by this library)
+- The start bytes 0, 1 and last byte have a fixed value.
+- The *Command* is one of the following (only listing commands supported by this library)
+
+  | Code   | Command                                            |
+  |--------|----------------------------------------------------|
+  | `0x01` | Connect (without session initiation)               |
+  | `0x76` | Connect (session initiation)                       |
+  | `0x02` | Disconnection (session end)                        |
+  | `0x05` | Device control command                             |
+  | `0x0B` | Retrieve realtime log                              |
+  | `0xC8` | Response (confirm successful execution of command) |
+
+- The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
+- The *Data* field (as of byte 5) may use 4 reserved bytes in front of actual payload:
+  - Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
+  - Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from -258 (the session initiation command) and is increased with every command send
+
+  | Byte         | 5             | 6             | 7              | 8              | ...      |
+  |--------------|---------------|---------------|----------------|----------------|----------|
+  |  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
 
-| Code   | Command                                             |
-|--------|-----------------------------------------------------|
-| `0x76` | Connect (session initiation)                        |
-| `0x02` | Disconnection (session end)                         |
-| `0x05` | Device control command                              |
-| `0x0B` | Retrieve realtime log                               |
-| `0xC8` | Response (confirm successful execution of command)  |
-
-The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
-The *Data* field (as of byte 5) typically has at least 4 bytes:
-- Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
-- Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from 0 (the session initiation command) and is increased with every command send
-
-| Byte         | 5             | 6             | 7              | 8              | ...      |
-|--------------|---------------|---------------|----------------|----------------|----------|
-|  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
+  Whether the Session Id and Message Number is used, depends on how the connection is made (using either command 0x01 or 0x76).
+  The support for these commands varies per panel / firmware combination.
 
-The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
+- The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
 
 ## API
 ### Connect
 ```
-connect(host, port=4370)
+connect(password)
 ```
 The method is used to connect a C3 device using TCP. 
 RS485 is not supported,  neither is using a password to secure the connection.
 This method must be called before any other method and initializes a C3 session.
+The parameter `password` is optional, when omitted, a connection attempt is made without password.
 Returns true in case of a successful connection.
 
 ### Disconnect
 ```
 disconnect()
 ```
```

### Comparing `zkaccess_c3-0.0.5/c3/consts.py` & `zkaccess_c3-0.0.6/c3/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 C3_PROTOCOL_VERSION = 0x01
 C3_DISCOVERY_MESSAGE = "CallSecurityDevice"
 
 
 class Command(IntEnum):
     """Enumeration of supported device_name interaction commands"""
     DISCOVER = 0x14
-    CONNECT = 0x76
+    CONNECT_SESSION = 0x76
+    CONNECT_SESSION_LESS = 0x01
     DISCONNECT = 0x02
     GETPARAM = 0x04
     DATATABLE_CFG = 0x06
     CONTROL = 0x05
     RTLOG = 0x0B
```

### Comparing `zkaccess_c3-0.0.5/c3/controldevice.py` & `zkaccess_c3-0.0.6/c3/controldevice.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/c3/core.py` & `zkaccess_c3-0.0.6/c3/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,17 @@
     log = logging.getLogger("C3")
     log.setLevel(logging.ERROR)
 
     def __init__(self, host: [str | C3DeviceInfo], port: int = consts.C3_PORT_DEFAULT) -> None:
         self._sock: socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self._sock.settimeout(2)
         self._connected: bool = False
-        self._session_id: int = 0
-        self._request_nr: int = 0
+        self._session_less = False
+        self._session_id: int = 0xFEFE
+        self._request_nr: int = -258
         self._status: C3PanelStatus = C3PanelStatus()
         if isinstance(host, C3DeviceInfo):
             self._device_info: C3DeviceInfo = host
         elif isinstance(host, str):
             self._device_info: C3DeviceInfo = C3DeviceInfo(host=host, port=port or consts.C3_PORT_DEFAULT)
 
     @classmethod
@@ -82,15 +83,15 @@
     def _construct_message(cls, session_id: Optional[int], request_nr: Optional[int], command: consts.Command,
                            data=None) -> bytes:
         message_length = len(data or []) + (4 if (session_id and request_nr) else 0)
         message = bytearray([consts.C3_PROTOCOL_VERSION,
                              command or 0x00,
                              utils.lsb(message_length),
                              utils.msb(message_length)])
-        if session_id and request_nr:
+        if session_id:
             message.append(utils.lsb(session_id))
             message.append(utils.msb(session_id))
             message.append(utils.lsb(request_nr))
             message.append(utils.msb(request_nr))
 
         if data:
             for byte in data:
@@ -106,15 +107,15 @@
         message.append(utils.msb(checksum))
 
         message.insert(0, consts.C3_MESSAGE_START)
         message.append(consts.C3_MESSAGE_END)
         return message
 
     def _send(self, command: consts.Command, data=None) -> int:
-        message = self._construct_message(self._session_id or 0, self._request_nr or 0, command, data)
+        message = self._construct_message(self._session_id, self._request_nr, command, data)
 
         self.log.debug("Sending: %s", message.hex())
 
         bytes_written = self._sock.send(message)
         self._request_nr = self._request_nr + 1
         return bytes_written
 
@@ -142,25 +143,27 @@
             data_size = 0
 
         return message, data_size
 
     def _send_receive(self, command: consts.Command, data=None) -> tuple[bytearray, int]:
         bytes_received = 0
         receive_data = bytearray()
+        session_offset = 0
 
         bytes_written = self._send(command, data)
         if bytes_written > 0:
             receive_data, bytes_received = self._receive()
-            if bytes_received > 2:
+            if not self._session_less and bytes_received > 2:
+                session_offset = 4
                 session_id = (receive_data[1] << 8) + receive_data[0]
                 # msg_seq = (receive_data[3] << 8) + receive_data[2]
                 if self._session_id != session_id:
                     raise ValueError("Data received with invalid session ID")
 
-        return receive_data[4:], bytes_received-4
+        return receive_data[session_offset:], bytes_received-session_offset
 
     def is_connected(self) -> bool:
         # try:
         #    # this will try to read bytes without blocking and also without removing them from buffer (peek only)
         #    data = self._sock.recv(1, socket.MSG_DONTWAIT | socket.MSG_PEEK)
         #    if len(data) == 0:
         #        return True
@@ -286,33 +289,56 @@
                             device_name=data.get("Device"),
                             firmware_version=data.get("Ver")
                         )))
             sock.close()
 
         return devices
 
-    def connect(self) -> bool:
+    def connect(self, password: Optional[str] = None) -> bool:
         """Connect to the C3 panel on the host/port provided in the constructor."""
         self._connected = False
-        self._session_id = 0
+        self._session_id = 0xFEFE
+        self._request_nr: -258
 
+        data = None
+        if password:
+            data = bytearray(password.encode('ascii'))
+
+        # Attempt to connect to panel with session initiation command
         try:
             self._sock.connect((self._device_info.host, self._device_info.port))
-            bytes_written = self._send(consts.Command.CONNECT)
+            bytes_written = self._send(consts.Command.CONNECT_SESSION, data)
             if bytes_written > 0:
                 receive_data, bytes_received = self._receive()
                 if bytes_received > 2:
                     self._session_id = (receive_data[1] << 8) + receive_data[0]
-                    self.log.debug("Connected with Session ID %x", self._session_id)
+                    self.log.debug("Connected with Session ID %04x", self._session_id)
+                    self._session_less = False
                     self._connected = True
         except ConnectionError as ex:
-            self.log.error("Connection to %s failed: %s", self._device_info.host, ex)
+            self.log.debug("Connection attempt with session to %s failed: %s", self._device_info.host, ex)
         except ValueError as ex:
             self.log.error("Reply from %s failed: %s", self._device_info.host, ex)
 
+        # Alternatively attempt to connect to panel without session initiation
+        if not self._connected:
+            try:
+                self._session_id = None
+                self._sock.connect((self._device_info.host, self._device_info.port))
+                bytes_written = self._send(consts.Command.CONNECT_SESSION_LESS, data)
+                if bytes_written > 0:
+                    self._receive()
+                    self.log.debug("Connected without session")
+                    self._session_less = True
+                    self._connected = True
+            except ConnectionError as ex:
+                self.log.debug("Connection attempt without session to %s failed: %s", self._device_info.host, ex)
+            except ValueError as ex:
+                self.log.error("Reply from %s failed: %s", self._device_info.host, ex)
+
         if self._connected:
             try:
                 params = self.get_device_param(["~SerialNumber", "LockCount", "AuxInCount", "AuxOutCount"])
                 self._device_info.serial_number = params.get("~SerialNumber", self._device_info.serial_number)
                 self._status.nr_of_locks = int(params.get("LockCount", self._status.nr_of_locks))
                 self._status.nr_aux_in = int(params.get("AuxInCount", self._status.nr_aux_in))
                 self._status.nr_aux_out = int(params.get("AuxOutCount", self._status.nr_aux_out))
@@ -326,16 +352,16 @@
     def disconnect(self):
         """Disconnect from C3 panel and end session."""
         if self.is_connected():
             self._send_receive(consts.Command.DISCONNECT)
             self._sock.close()
 
         self._connected = False
-        self._session_id = 0
-        self._request_nr = 0
+        self._session_id = None
+        self._request_nr: -258
 
     def get_device_param(self, request_parameters: list[str]) -> dict:
         """Retrieve the requested device parameter values."""
         if self.is_connected():
             message, _ = self._send_receive(consts.Command.GETPARAM, ','.join(request_parameters))
             parameter_values = self._parse_kv_from_message(message)
         else:
```

### Comparing `zkaccess_c3-0.0.5/c3/crc.py` & `zkaccess_c3-0.0.6/c3/crc.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/c3/rtlog.py` & `zkaccess_c3-0.0.6/c3/rtlog.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/c3/utils.py` & `zkaccess_c3-0.0.6/c3/utils.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/cli/C3_CancelAlarms.py` & `zkaccess_c3-0.0.6/cli/C3_CancelAlarms.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from c3 import C3
 from c3 import controldevice
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('host', help='C3 panel IP address or host name')
+    parser.add_argument('--password', help='Password')
     args = parser.parse_args()
 
     print("Connecting to %s" % args.host)
     panel = C3(args.host)
     panel.log.addHandler(logging.StreamHandler(sys.stdout))
     panel.log.setLevel(logging.DEBUG)
 
     try:
-        if panel.connect():
+        if panel.connect(args.password):
             panel.control_device(controldevice.ControlDeviceCancelAlarms())
     except Exception as e:
         print(f"Cancel alarms faied: {e}")
     finally:
         panel.disconnect()
```

### Comparing `zkaccess_c3-0.0.5/cli/C3_Discover.py` & `zkaccess_c3-0.0.6/cli/C3_Discover.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/cli/C3_GetDeviceParam.py` & `zkaccess_c3-0.0.6/cli/C3_GetDeviceParam.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from c3 import C3
 from c3.utils import C3DateTime
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('host', help='C3 panel IP address or host name')
+    parser.add_argument('--password', help='Password')
     args = parser.parse_args()
 
     print("Connecting to %s" % args.host)
     panel = C3(args.host)
     panel.log.addHandler(logging.StreamHandler(sys.stdout))
     panel.log.setLevel(logging.DEBUG)
 
     try:
-        if panel.connect():
+        if panel.connect(args.password):
             print("Device:")
             print(repr(panel))
 
             params = panel.get_device_param(["~ZKFPVersion",
                                              "~SerialNumber",
                                              "LockCount",
                                              "ReaderCount",
```

### Comparing `zkaccess_c3-0.0.5/cli/C3_GetRTLog.py` & `zkaccess_c3-0.0.6/cli/C3_GetRTLog.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from c3 import C3
 from c3 import rtlog
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('host', help='C3 panel IP address or host name')
+    parser.add_argument('--password', help='Password')
     args = parser.parse_args()
 
     print("Connecting to %s" % args.host)
     panel = C3(args.host)
     panel.log.addHandler(logging.StreamHandler(sys.stdout))
     panel.log.setLevel(logging.DEBUG)
 
-    if panel.connect():
+    if panel.connect(args.password):
         try:
             while True:
                 last_record_is_status = False
 
                 records = panel.get_rt_log()
                 for record in records:
                     print(repr(record))
```

### Comparing `zkaccess_c3-0.0.5/cli/C3_OutputOperation.py` & `zkaccess_c3-0.0.6/cli/C3_OutputOperation.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from c3 import consts
 from c3 import controldevice
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('host', help='C3 panel IP address or host name')
+    parser.add_argument('--password', help='Password')
     parser.add_argument('--output', choices=['door', 'aux'], required=True, help='Output is door or auxiliary')
     parser.add_argument('--number', type=int, required=True, help='Door or auxiliary output number')
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument('--open', action="store_true", help='Set state to normal open')
     group.add_argument('--close', action="store_true", help='Set state to closed')
     parser.add_argument('--duration', type=int, help='Duration to (temporarily) open the door')
     args = parser.parse_args()
@@ -24,15 +25,15 @@
 
     print("Connecting to %s" % args.host)
     panel = C3(args.host)
     panel.log.addHandler(logging.StreamHandler(sys.stdout))
     panel.log.setLevel(logging.DEBUG)
 
     try:
-        if panel.connect():
+        if panel.connect(args.password):
             operation = controldevice.ControlDeviceOutput(args.number,
                                                           consts.ControlOutputAddress.AUX_OUTPUT if args.output == 'aux'
                                                           else consts.ControlOutputAddress.DOOR_OUTPUT, duration)
             panel.control_device(operation)
     except Exception as e:
         print(f"Parameter retrieval failed: {e}")
     finally:
```

### Comparing `zkaccess_c3-0.0.5/pyproject.toml` & `zkaccess_c3-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zkaccess_c3"
-version = "0.0.5"
+version = "0.0.6"
 description = "A native Python library for communicating with the ZKAccess C3 Access Control Panels."
 authors = [
     {name = "Vwout", email="vwout@users.noreply.github.com"},
 ]
 #license = "GPL-3.0-or-later"
 readme = "readme.md"
 requires-python = ">=3.7"
```

### Comparing `zkaccess_c3-0.0.5/readme.md` & `zkaccess_c3-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,91 @@
+Metadata-Version: 2.1
+Name: zkaccess_c3
+Version: 0.0.6
+Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
+Author-email: Vwout <vwout@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
+Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # c3
 A native Python library for communicating with the ZKTeco ZKAccess C3 Access Control Panels.
 
 This library intends to implement the same functionality as provided by the ZKAccess C3 PullSDK API, but using native Python only.
 It is a port and extension of my (C3 Lua library)[../zkaccess-c3-lua].
 
 ## Usage
 To use the library, import the main class:
 ```
 from c3 import C3
 ```
 A panel connection can be created from the main class `C3`:
 ```
-    panel = C3()
-    if panel.connect(ip):
+    panel = C3(ip)
+    if panel.connect():
       panel.get_device_param(["~SerialNumber", "LockCount")
 ```
 To use the real-time log (RTLog), or control outputs, also include the helper classes from `controldevice` and `rtlog`.
 
+## Compatible devices
+The following devices are tested and known compatible:
+- C3-200 (firmware AC Ver 4.1.9 4609-03 Apr 7 2016)
+- C3-400 (firmware AC Ver 4.3.4 Apr 27 2017)
+
 ## Protocol
 The C3 access panels communicate using RS485 or TCP/IP.
 This library only support TCP/IP connections using IPv4.
 The connection is optionally secured by a password.
-Connections to C3 panels that use a password are not supported for this moment.
 
 The wire protocol for the access panels is binary, with the following datagram both for requests (from client to equipment) and responses:
 
 | Byte        | 0      | 1       | 2       | 3          | 4          | 5,6,7,8, ...  | n-2, n-1 | n       |
 |-------------|--------|---------|---------|------------|------------|---------------|----------|---------|
-| **Meaning** | Start  | Version | Command | Length Lsb | Length Msb | Data          | Checksum | End     |
+| **Meaning** | Start  | Version | Command | Length LSB | Length MSB | Data          | Checksum | End     |
 |  **Value**  | `0xAA` | `0x01`  |         |            |            |               |          | `0x55`  |
 
-The start bytes 0, 1 and last byte have a fixed value.
-The *Command* is one of the following (only listing commands supported by this library)
+- The start bytes 0, 1 and last byte have a fixed value.
+- The *Command* is one of the following (only listing commands supported by this library)
+
+  | Code   | Command                                            |
+  |--------|----------------------------------------------------|
+  | `0x01` | Connect (without session initiation)               |
+  | `0x76` | Connect (session initiation)                       |
+  | `0x02` | Disconnection (session end)                        |
+  | `0x05` | Device control command                             |
+  | `0x0B` | Retrieve realtime log                              |
+  | `0xC8` | Response (confirm successful execution of command) |
+
+- The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
+- The *Data* field (as of byte 5) may use 4 reserved bytes in front of actual payload:
+  - Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
+  - Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from -258 (the session initiation command) and is increased with every command send
+
+  | Byte         | 5             | 6             | 7              | 8              | ...      |
+  |--------------|---------------|---------------|----------------|----------------|----------|
+  |  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
 
-| Code   | Command                                             |
-|--------|-----------------------------------------------------|
-| `0x76` | Connect (session initiation)                        |
-| `0x02` | Disconnection (session end)                         |
-| `0x05` | Device control command                              |
-| `0x0B` | Retrieve realtime log                               |
-| `0xC8` | Response (confirm successful execution of command)  |
-
-The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
-The *Data* field (as of byte 5) typically has at least 4 bytes:
-- Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
-- Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from 0 (the session initiation command) and is increased with every command send
-
-| Byte         | 5             | 6             | 7              | 8              | ...      |
-|--------------|---------------|---------------|----------------|----------------|----------|
-|  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
+  Whether the Session Id and Message Number is used, depends on how the connection is made (using either command 0x01 or 0x76).
+  The support for these commands varies per panel / firmware combination.
 
-The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
+- The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
 
 ## API
 ### Connect
 ```
-connect(host, port=4370)
+connect(password)
 ```
 The method is used to connect a C3 device using TCP. 
 RS485 is not supported,  neither is using a password to secure the connection.
 This method must be called before any other method and initializes a C3 session.
+The parameter `password` is optional, when omitted, a connection attempt is made without password.
 Returns true in case of a successful connection.
 
 ### Disconnect
 ```
 disconnect()
 ```
```

### Comparing `zkaccess_c3-0.0.5/tests/test_consts.py` & `zkaccess_c3-0.0.6/tests/test_consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from c3.consts import *
 
 
 def test_commands():
-    connect_cmd = Command.CONNECT
+    connect_cmd = Command.CONNECT_SESSION
     assert 0x76 == connect_cmd
     connect_reply = C3_REPLY_OK
     assert 0xC8 == connect_reply
 
 
 def test_control_operation():
     cancel_alarm = ControlOperation.CANCEL_ALARM
```

### Comparing `zkaccess_c3-0.0.5/tests/test_controldevice.py` & `zkaccess_c3-0.0.6/tests/test_controldevice.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/tests/test_core.py` & `zkaccess_c3-0.0.6/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,36 @@
         assert params["~ZKFPVersion"] == "10"
         assert params["LockCount"] == "2"
         assert params["ReaderCount"] == "4"
         assert params["AuxInCount"] == "2"
         assert params["AuxOutCount"] == "2"
 
 
+def test_core_get_device_param_session_less():
+    with mock.patch('socket.socket') as mock_socket:
+        panel = C3('localhost')
+        mock_socket.return_value.send.return_value = 8
+        mock_socket.return_value.recv.side_effect = [
+            # Reject response to session connect attempt
+            bytes.fromhex("aa01c90100"), bytes.fromhex("f313d955"),
+            # Confirm session-less connection attempt
+            bytes.fromhex("aa01c80000"), bytes.fromhex("800255"),
+            # Session-less response to init-getparams
+            bytes.fromhex("aa01c84800"), bytes.fromhex("7e53657269616c4e756d6265723d4444473831333030313630393232303034"
+                                                       "30312c4c6f636b436f756e743d342c417578496e436f756e743d342c417578"
+                                                       "4f7574436f756e743d34c6be55"),
+        ]
+
+        assert panel.connect() is True
+        assert panel.serial_number == "DDG8130016092200401"
+        assert panel.nr_of_locks == 4
+        assert panel.nr_aux_out == 4
+        assert panel.nr_aux_in == 4
+
+
 def test_core_lock_status():
     with mock.patch('socket.socket') as mock_socket:
         panel = C3('localhost')
         mock_socket.return_value.send.return_value = 8
         mock_socket.return_value.recv.side_effect = [bytes.fromhex("aa01c80400"),
                                                      bytes.fromhex("eb6600005c7f55"),
                                                      bytes.fromhex("aa01c84600"),
```

### Comparing `zkaccess_c3-0.0.5/tests/test_crc16.py` & `zkaccess_c3-0.0.6/tests/test_crc16.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/tests/test_rtlog.py` & `zkaccess_c3-0.0.6/tests/test_rtlog.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/tests/test_utils.py` & `zkaccess_c3-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.5/zkaccess_c3.egg-info/PKG-INFO` & `zkaccess_c3-0.0.6/zkaccess_c3.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess-c3
-Version: 0.0.5
+Version: 0.0.6
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -20,63 +20,72 @@
 ## Usage
 To use the library, import the main class:
 ```
 from c3 import C3
 ```
 A panel connection can be created from the main class `C3`:
 ```
-    panel = C3()
-    if panel.connect(ip):
+    panel = C3(ip)
+    if panel.connect():
       panel.get_device_param(["~SerialNumber", "LockCount")
 ```
 To use the real-time log (RTLog), or control outputs, also include the helper classes from `controldevice` and `rtlog`.
 
+## Compatible devices
+The following devices are tested and known compatible:
+- C3-200 (firmware AC Ver 4.1.9 4609-03 Apr 7 2016)
+- C3-400 (firmware AC Ver 4.3.4 Apr 27 2017)
+
 ## Protocol
 The C3 access panels communicate using RS485 or TCP/IP.
 This library only support TCP/IP connections using IPv4.
 The connection is optionally secured by a password.
-Connections to C3 panels that use a password are not supported for this moment.
 
 The wire protocol for the access panels is binary, with the following datagram both for requests (from client to equipment) and responses:
 
 | Byte        | 0      | 1       | 2       | 3          | 4          | 5,6,7,8, ...  | n-2, n-1 | n       |
 |-------------|--------|---------|---------|------------|------------|---------------|----------|---------|
-| **Meaning** | Start  | Version | Command | Length Lsb | Length Msb | Data          | Checksum | End     |
+| **Meaning** | Start  | Version | Command | Length LSB | Length MSB | Data          | Checksum | End     |
 |  **Value**  | `0xAA` | `0x01`  |         |            |            |               |          | `0x55`  |
 
-The start bytes 0, 1 and last byte have a fixed value.
-The *Command* is one of the following (only listing commands supported by this library)
+- The start bytes 0, 1 and last byte have a fixed value.
+- The *Command* is one of the following (only listing commands supported by this library)
+
+  | Code   | Command                                            |
+  |--------|----------------------------------------------------|
+  | `0x01` | Connect (without session initiation)               |
+  | `0x76` | Connect (session initiation)                       |
+  | `0x02` | Disconnection (session end)                        |
+  | `0x05` | Device control command                             |
+  | `0x0B` | Retrieve realtime log                              |
+  | `0xC8` | Response (confirm successful execution of command) |
+
+- The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
+- The *Data* field (as of byte 5) may use 4 reserved bytes in front of actual payload:
+  - Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
+  - Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from -258 (the session initiation command) and is increased with every command send
+
+  | Byte         | 5             | 6             | 7              | 8              | ...      |
+  |--------------|---------------|---------------|----------------|----------------|----------|
+  |  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
 
-| Code   | Command                                             |
-|--------|-----------------------------------------------------|
-| `0x76` | Connect (session initiation)                        |
-| `0x02` | Disconnection (session end)                         |
-| `0x05` | Device control command                              |
-| `0x0B` | Retrieve realtime log                               |
-| `0xC8` | Response (confirm successful execution of command)  |
-
-The *Length* field (2 bytes, in Little Endian encoding) contains the number of bytes of the *Data* field.
-The *Data* field (as of byte 5) typically has at least 4 bytes:
-- Session Id (2 bytes, in Little Endian encoding): The session identifier assigned by the equipment in response to a session initiation command
-- Message Number (2 bytes, in Little Endian encoding): A message sequence number that starts from 0 (the session initiation command) and is increased with every command send
-
-| Byte         | 5             | 6             | 7              | 8              | ...      |
-|--------------|---------------|---------------|----------------|----------------|----------|
-|  **Meaning** | SessionId Lsb | SessionId Msb | Message Nr Lsb | Message Nr Msb | Payload  |
+  Whether the Session Id and Message Number is used, depends on how the connection is made (using either command 0x01 or 0x76).
+  The support for these commands varies per panel / firmware combination.
 
-The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
+- The *Checksum* is a CRC-16 checksum calculated over the full message excluding the *Start* and *End* byte.
 
 ## API
 ### Connect
 ```
-connect(host, port=4370)
+connect(password)
 ```
 The method is used to connect a C3 device using TCP. 
 RS485 is not supported,  neither is using a password to secure the connection.
 This method must be called before any other method and initializes a C3 session.
+The parameter `password` is optional, when omitted, a connection attempt is made without password.
 Returns true in case of a successful connection.
 
 ### Disconnect
 ```
 disconnect()
 ```
```

### Comparing `zkaccess_c3-0.0.5/zkaccess_c3.egg-info/SOURCES.txt` & `zkaccess_c3-0.0.6/zkaccess_c3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

