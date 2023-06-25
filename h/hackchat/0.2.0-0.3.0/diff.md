# Comparing `tmp/hackchat-0.2.0.tar.gz` & `tmp/hackchat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hackchat-0.2.0.tar", last modified: Sun Jun  4 12:51:15 2017, max compression
+gzip compressed data, was "hackchat-0.3.0.tar", last modified: Sun Jun 25 20:37:29 2023, max compression
```

## Comparing `hackchat-0.2.0.tar` & `hackchat-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2017-06-04 12:51:15.000000 hackchat-0.2.0/
-drwxr-xr-x   0 leonardo  (1000) leonardo  (1000)        0 2017-06-04 12:51:15.000000 hackchat-0.2.0/hackchat.egg-info/
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       17 2017-06-04 12:51:15.000000 hackchat-0.2.0/hackchat.egg-info/requires.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)        9 2017-06-04 12:51:15.000000 hackchat-0.2.0/hackchat.egg-info/top_level.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      303 2017-06-04 12:51:15.000000 hackchat-0.2.0/hackchat.egg-info/PKG-INFO
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)        1 2017-06-04 12:51:15.000000 hackchat-0.2.0/hackchat.egg-info/dependency_links.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      179 2017-06-04 12:51:15.000000 hackchat-0.2.0/hackchat.egg-info/SOURCES.txt
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      303 2017-06-04 12:51:15.000000 hackchat-0.2.0/PKG-INFO
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)      404 2017-06-04 12:50:16.000000 hackchat-0.2.0/setup.py
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)     2557 2017-06-04 12:44:32.000000 hackchat-0.2.0/hackchat.py
--rw-r--r--   0 leonardo  (1000) leonardo  (1000)       38 2017-06-04 12:51:15.000000 hackchat-0.2.0/setup.cfg
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-06-25 20:37:29.173645 hackchat-0.3.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)     1065 2023-06-25 20:35:56.000000 hackchat-0.3.0/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      269 2023-06-25 20:37:29.173645 hackchat-0.3.0/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      597 2023-06-25 20:35:56.000000 hackchat-0.3.0/README.md
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-06-25 20:37:29.173645 hackchat-0.3.0/hackchat.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      269 2023-06-25 20:37:29.000000 hackchat-0.3.0/hackchat.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      197 2023-06-25 20:37:29.000000 hackchat-0.3.0/hackchat.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-06-25 20:37:29.000000 hackchat-0.3.0/hackchat.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       17 2023-06-25 20:37:29.000000 hackchat-0.3.0/hackchat.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        9 2023-06-25 20:37:29.000000 hackchat-0.3.0/hackchat.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)     3289 2023-06-25 20:35:56.000000 hackchat-0.3.0/hackchat.py
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-06-25 20:37:29.173645 hackchat-0.3.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      404 2023-06-25 20:37:14.000000 hackchat-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hackchat-0.2.0/hackchat.py` & `hackchat-0.3.0/hackchat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import threading
 import time
 import websocket
 
+
 class HackChat:
     """A library to connect to https://hack.chat.
 
     <on_message> is <list> of callback functions to receive data from
     https://hack.chat. Add your callback functions to this attribute.
     e.g., on_message += [my_callback]
     The callback function should have 3 parameters, the first for the
@@ -21,29 +22,45 @@
         nick -- <str>; the nickname to use upon joining the channel
         channel -- <str>; the channel to connect to on https://hack.chat
         """
         self.nick = nick
         self.channel = channel
         self.online_users = []
         self.on_message = []
+        self.on_whisper = []
         self.on_join = []
         self.on_leave = []
         self.ws = websocket.create_connection("wss://hack.chat/chat-ws")
         self._send_packet({"cmd": "join", "channel": channel, "nick": nick})
-        threading.Thread(target = self._ping_thread).start()
+        threading.Thread(target=self._ping_thread).start()
 
     def send_message(self, msg):
         """Sends a message on the channel."""
         self._send_packet({"cmd": "chat", "text": msg})
 
+    def send_to(self, target, msg):
+        self._send_packet({"cmd": "whisper", "nick": target, "text": msg})
+
+    def move(self, new_channel):
+        self.channel = new_channel
+        self._send_packet({"cmd": "move", "channel": new_channel})
+
+    def change_nick(self, new_nick):
+        self.nick = new_nick
+        self._send_packet({"cmd": "changenick", "nick": new_nick})
+
     def _send_packet(self, packet):
         """Sends <packet> (<dict>) to https://hack.chat."""
         encoded = json.dumps(packet)
         self.ws.send(encoded)
 
+    def daemon(self):
+        self.daemon_thread=threading.Thread(target=self.run)
+        self.daemon_thread.start()
+
     def run(self):
         """Sends data to the callback functions."""
         while True:
             result = json.loads(self.ws.recv())
             if result["cmd"] == "chat" and not result["nick"] == self.nick:
                 for handler in list(self.on_message):
                     handler(self, result["text"], result["nick"])
@@ -54,13 +71,16 @@
             elif result["cmd"] == "onlineRemove":
                 self.online_users.remove(result["nick"])
                 for handler in list(self.on_leave):
                     handler(self, result["nick"])
             elif result["cmd"] == "onlineSet":
                 for nick in result["nicks"]:
                     self.online_users.append(nick)
+            elif result["cmd"] == "info" and result.get("type") == "whisper":
+                for handler in list(self.on_whisper):
+                    handler(self,result["text"],result["from"],result)
 
     def _ping_thread(self):
         """Retains the websocket connection."""
         while self.ws.connected:
             self._send_packet({"cmd": "ping"})
             time.sleep(60)
```

