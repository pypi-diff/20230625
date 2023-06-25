# Comparing `tmp/ltchiptool_terminal-1.1.0.tar.gz` & `tmp/ltchiptool_terminal-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool_terminal-1.1.0.tar", max compression
+gzip compressed data, was "ltchiptool_terminal-1.2.0.tar", max compression
```

## Comparing `ltchiptool_terminal-1.1.0.tar` & `ltchiptool_terminal-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      253 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/README.md
--rw-r--r--   0        0        0      648 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/__init__.py
--rw-r--r--   0        0        0    13754 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/gui.py
--rw-r--r--   0        0        0     4217 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.wxui
--rw-r--r--   0        0        0     5485 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.xrc
--rw-r--r--   0        0        0     3744 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/ltctplugin/terminal/work.py
--rw-r--r--   0        0        0      491 2023-06-21 19:05:03.767670 ltchiptool_terminal-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 ltchiptool_terminal-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      253 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/README.md
+-rw-r--r--   0        0        0      648 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/ltctplugin/terminal/__init__.py
+-rw-r--r--   0        0        0    13840 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/ltctplugin/terminal/gui.py
+-rw-r--r--   0        0        0     4217 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/ltctplugin/terminal/terminal.wxui
+-rw-r--r--   0        0        0     5485 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/ltctplugin/terminal/terminal.xrc
+-rw-r--r--   0        0        0     3744 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/ltctplugin/terminal/work.py
+-rw-r--r--   0        0        0      491 2023-06-25 13:02:30.770891 ltchiptool_terminal-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 ltchiptool_terminal-1.2.0/PKG-INFO
```

### Comparing `ltchiptool_terminal-1.1.0/ltctplugin/terminal/__init__.py` & `ltchiptool_terminal-1.2.0/ltctplugin/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.1.0/ltctplugin/terminal/gui.py` & `ltchiptool_terminal-1.2.0/ltctplugin/terminal/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         ...
 
     def close_real_terminal(self):
         ...
 
 
 class SerialHook:
-    def on_serial_receive(self, data: bytes) -> bool | None:
+    def on_serial_receive(self, data: bytes) -> bytes | None:
         pass
 
     def on_serial_open(self, port: str) -> None:
         pass
 
     def on_serial_close(self, port: str) -> None:
         pass
@@ -294,16 +294,19 @@
             if self.echo:
                 self.Text.AppendText(text)
             text = text.encode("utf-8", "ignore")
         self.serial.write(text)
 
     def OnSerialData(self, data: bytes) -> None:
         for hook in self.hooks:
-            if hook.on_serial_receive(data) is True:
-                return
+            data_new = hook.on_serial_receive(data)
+            if data_new is not None:
+                data = data_new
+        if not data:
+            return
         data = data.replace(b"\r\n", b"\n")
         data = data.replace(b"\r", b"")
         text = data.decode("utf-8", errors="replace")
         self.Text.AppendText(text)
 
     def OnControlData(self, data: bytes) -> None:
         if not (data.startswith(b"\x1B[") and data.endswith(b"m")):
```

### Comparing `ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.wxui` & `ltchiptool_terminal-1.2.0/ltctplugin/terminal/terminal.wxui`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.1.0/ltctplugin/terminal/terminal.xrc` & `ltchiptool_terminal-1.2.0/ltctplugin/terminal/terminal.xrc`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.1.0/ltctplugin/terminal/work.py` & `ltchiptool_terminal-1.2.0/ltctplugin/terminal/work.py`

 * *Files identical despite different names*

### Comparing `ltchiptool_terminal-1.1.0/PKG-INFO` & `ltchiptool_terminal-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltchiptool-terminal
-Version: 1.1.0
+Version: 1.2.0
 Summary: Serial terminal plugin for ltchiptool
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

