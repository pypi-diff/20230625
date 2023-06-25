# Comparing `tmp/zcc-helper-3.0rc1.tar.gz` & `tmp/zcc-helper-3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcc-helper-3.0rc1.tar", last modified: Sat Jun 18 00:00:03 2022, max compression
+gzip compressed data, was "zcc-helper-3.1rc1.tar", last modified: Sun Jun 25 05:21:52 2023, max compression
```

## Comparing `zcc-helper-3.0rc1.tar` & `zcc-helper-3.1rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2022-06-18 00:00:03.097619 zcc-helper-3.0rc1/
--rw-r--r--   0 mark       (501) staff       (20)     9422 2022-06-18 00:00:03.096944 zcc-helper-3.0rc1/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     9136 2022-03-23 21:54:32.000000 zcc-helper-3.0rc1/README.md
--rw-r--r--   0 mark       (501) staff       (20)       38 2022-06-18 00:00:03.097673 zcc-helper-3.0rc1/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.0rc1/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2022-06-18 00:00:03.093263 zcc-helper-3.0rc1/zcc/
--rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.0rc1/zcc/__init__.py
--rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.0rc1/zcc/__main__.py
--rw-r--r--   0 mark       (501) staff       (20)      247 2022-06-17 05:35:17.000000 zcc-helper-3.0rc1/zcc/constants.py
--rw-r--r--   0 mark       (501) staff       (20)    17515 2022-06-17 23:53:10.000000 zcc-helper-3.0rc1/zcc/controller.py
--rw-r--r--   0 mark       (501) staff       (20)      354 2022-02-22 10:48:42.000000 zcc-helper-3.0rc1/zcc/description.py
--rw-r--r--   0 mark       (501) staff       (20)     9729 2022-04-18 11:00:22.000000 zcc-helper-3.0rc1/zcc/device.py
--rw-r--r--   0 mark       (501) staff       (20)     4134 2022-05-02 21:53:31.000000 zcc-helper-3.0rc1/zcc/discovery.py
--rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.0rc1/zcc/errors.py
--rw-r--r--   0 mark       (501) staff       (20)     3732 2022-06-13 11:56:05.000000 zcc-helper-3.0rc1/zcc/protocol.py
--rw-r--r--   0 mark       (501) staff       (20)     6372 2022-06-17 23:52:30.000000 zcc-helper-3.0rc1/zcc/socket.py
--rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.0rc1/zcc/trace.py
--rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.0rc1/zcc/watchdog.py
--rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.0rc1/zcc.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2022-06-18 00:00:03.096590 zcc-helper-3.0rc1/zcc_helper.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     9422 2022-06-18 00:00:02.000000 zcc-helper-3.0rc1/zcc_helper.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      351 2022-06-18 00:00:02.000000 zcc-helper-3.0rc1/zcc_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2022-06-18 00:00:02.000000 zcc-helper-3.0rc1/zcc_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        4 2022-06-18 00:00:02.000000 zcc-helper-3.0rc1/zcc_helper.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 05:21:52.802554 zcc-helper-3.1rc1/
+-rw-r--r--   0 mark       (501) staff       (20)    10153 2023-06-25 05:21:52.802220 zcc-helper-3.1rc1/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     9867 2022-06-20 04:14:44.000000 zcc-helper-3.1rc1/README.md
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-25 05:21:52.802625 zcc-helper-3.1rc1/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)      661 2022-03-20 04:59:07.000000 zcc-helper-3.1rc1/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 05:21:52.798601 zcc-helper-3.1rc1/zcc/
+-rw-r--r--   0 mark       (501) staff       (20)      313 2022-05-23 13:52:19.000000 zcc-helper-3.1rc1/zcc/__init__.py
+-rwxr-xr-x   0 mark       (501) staff       (20)     4633 2022-06-17 23:28:44.000000 zcc-helper-3.1rc1/zcc/__main__.py
+-rw-r--r--   0 mark       (501) staff       (20)      247 2023-06-25 05:21:32.000000 zcc-helper-3.1rc1/zcc/constants.py
+-rw-r--r--   0 mark       (501) staff       (20)    17770 2023-06-25 05:17:16.000000 zcc-helper-3.1rc1/zcc/controller.py
+-rw-r--r--   0 mark       (501) staff       (20)      417 2023-06-25 05:04:27.000000 zcc-helper-3.1rc1/zcc/description.py
+-rw-r--r--   0 mark       (501) staff       (20)     9773 2023-06-25 04:59:02.000000 zcc-helper-3.1rc1/zcc/device.py
+-rw-r--r--   0 mark       (501) staff       (20)     4430 2023-06-25 05:05:22.000000 zcc-helper-3.1rc1/zcc/discovery.py
+-rw-r--r--   0 mark       (501) staff       (20)      114 2022-02-14 13:53:41.000000 zcc-helper-3.1rc1/zcc/errors.py
+-rw-r--r--   0 mark       (501) staff       (20)     3732 2022-06-18 00:10:40.000000 zcc-helper-3.1rc1/zcc/protocol.py
+-rw-r--r--   0 mark       (501) staff       (20)     6372 2022-06-18 00:10:40.000000 zcc-helper-3.1rc1/zcc/socket.py
+-rw-r--r--   0 mark       (501) staff       (20)     1954 2022-06-13 11:55:47.000000 zcc-helper-3.1rc1/zcc/trace.py
+-rw-r--r--   0 mark       (501) staff       (20)      971 2022-06-13 11:55:47.000000 zcc-helper-3.1rc1/zcc/watchdog.py
+-rwxr-xr-x   0 mark       (501) staff       (20)       29 2021-10-12 07:44:33.000000 zcc-helper-3.1rc1/zcc.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-25 05:21:52.801369 zcc-helper-3.1rc1/zcc_helper.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)    10153 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      351 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        4 2023-06-25 05:21:52.000000 zcc-helper-3.1rc1/zcc_helper.egg-info/top_level.txt
```

### Comparing `zcc-helper-3.0rc1/PKG-INFO` & `zcc-helper-3.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.0rc1
+Version: 3.1rc1
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -216,22 +216,37 @@
     def room(self) -> str:
         '''Gets a descriptive string of the device room'''
 
     def type(self) -> str:
         '''Gets a descriptive string of the device type'''
 ```
 
-In addition, you can subscribe to a notification for changes to the device state by using:
+In addition, you can subscribe to a notification for changes to the device state by using the following methods of the device object.
 
-```
-device.subscribe(observer)
+```python
+    def subscribe(self, observer):
+        '''Subscribe an observer object for state changes.
+        Observer object must include notify(self, observable, *args, **kwargs) method.'''
+
+    def unsubscribe(self, observer):
+        '''Unsubscribe an observer object.'''
 ```
 
 The observer object must have a notify(observable) method.
 
+Finally, you can initiate a watchdog function that will periodically refresh the device states from the ZCC.   This can be useful for long lived connections that may time-out as it will trigger a re-connection if needed.
+
+```python
+    def start_watchdog(self, timer: int):
+        '''Start a periodic timeout that resets every time a status update is received.'''
+
+    def stop_watchdog(self):
+        '''Stop the periodic timeout.'''
+
+```
 ### Command Line Program
 
 ZCC can also be used as a command line tool to discover ZCC devices and/or execute actions upon them.
 
 ```
 $ python3 -m zcc
 usage: zcc [-h] [--verbosity VERBOSITY] (--discover | --execute) [--host HOST] [--port PORT] [--timeout TIMEOUT] [--device DEVICE]
```

### Comparing `zcc-helper-3.0rc1/README.md` & `zcc-helper-3.1rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -204,22 +204,37 @@
     def room(self) -> str:
         '''Gets a descriptive string of the device room'''
 
     def type(self) -> str:
         '''Gets a descriptive string of the device type'''
 ```
 
-In addition, you can subscribe to a notification for changes to the device state by using:
+In addition, you can subscribe to a notification for changes to the device state by using the following methods of the device object.
 
-```
-device.subscribe(observer)
+```python
+    def subscribe(self, observer):
+        '''Subscribe an observer object for state changes.
+        Observer object must include notify(self, observable, *args, **kwargs) method.'''
+
+    def unsubscribe(self, observer):
+        '''Unsubscribe an observer object.'''
 ```
 
 The observer object must have a notify(observable) method.
 
+Finally, you can initiate a watchdog function that will periodically refresh the device states from the ZCC.   This can be useful for long lived connections that may time-out as it will trigger a re-connection if needed.
+
+```python
+    def start_watchdog(self, timer: int):
+        '''Start a periodic timeout that resets every time a status update is received.'''
+
+    def stop_watchdog(self):
+        '''Stop the periodic timeout.'''
+
+```
 ### Command Line Program
 
 ZCC can also be used as a command line tool to discover ZCC devices and/or execute actions upon them.
 
 ```
 $ python3 -m zcc
 usage: zcc [-h] [--verbosity VERBOSITY] (--discover | --execute) [--host HOST] [--port PORT] [--timeout TIMEOUT] [--device DEVICE]
```

### Comparing `zcc-helper-3.0rc1/setup.py` & `zcc-helper-3.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.0rc1/zcc/__main__.py` & `zcc-helper-3.1rc1/zcc/__main__.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.0rc1/zcc/controller.py` & `zcc-helper-3.1rc1/zcc/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         self.logger.info(
             'Setting up %s version %s', NAME, VERSION)
 
         self.brand = description.brand
         self.product = description.product
         self.mac = description.mac
         self.available_tcps = description.available_tcps
+        self.api_version = description.api_version
+        self.firmware_version = description.firmware_version
 
         self.timeout = timeout
         self.verbosity = verbosity
 
         self.devices: Dict[ControlPointDevice] = {}
 
         self.actions_received = 0
@@ -178,18 +180,20 @@
         self.disconnect()
 
     def describe(self) -> str:
         '''Return a string representation of ZCC including devices'''
         header = '+' + '-' * 130 + '+'
         if self.host:
             description = header + '\n'
-            description += '| ControlPoint: %12s        %8s %8s %27s devices        %16s:%-6d %s Tcps    |\n' % (
+            description += '| ControlPoint: %12s %8s %8s api: %4s fw: %12s %7s devices %16s:%-6d %s Tcps    |\n' % (
                 self.mac if self.mac else "n/a",
                 self.product if self.product else 'n/a',
                 self.brand if self.brand else 'n/a',
+                self.api_version if self.api_version else 'n/a',
+                self.firmware_version if self.firmware_version else 'n/a',
                 str(len(self.devices)),
                 self.host,
                 self.port,
                 str(self.available_tcps) if self.available_tcps else "n/a")
             description += header + '\n'
             for key in self.devices:
                 description += self.devices[key].describe()
```

### Comparing `zcc-helper-3.0rc1/zcc/device.py` & `zcc-helper-3.1rc1/zcc/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
             description += "On" if state.get('isOn', False) else "Off"
             brightness = state.get('brightness', None)
             if brightness:
                 description += '/' + str(brightness)
             fan_speed = state.get('fanspeed', None)
             if fan_speed:
                 description += '/' + str(fan_speed)
+        except IndexError:
+            pass
         except KeyError:
             pass
         return description
 
     @property
     def battery_level(self) -> int | None:
         '''Return the battery level of an attached sensor.'''
```

### Comparing `zcc-helper-3.0rc1/zcc/discovery.py` & `zcc-helper-3.1rc1/zcc/discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,18 @@
                 if response:
                     self.discovery_result.brand = response['brand']
                     self.discovery_result.product = response['product']
                     self.discovery_result.mac = response['mac']
                     self.discovery_result.host = addr[0]
                     self.discovery_result.port = response['tcp']
                     self.discovery_result.available_tcps = response['availableTcps']
+                    if api_version := response.get('apiVersion'):
+                        self.discovery_result.api_version = api_version
+                    if firmware_version := response.get('firmwareVersion'):
+                        self.discovery_result.firmware_version = firmware_version
                     self.discovery_complete.set_result(True)
             except JSONDecodeError:
                 break
 
         return super().datagram_received(data, addr)
```

### Comparing `zcc-helper-3.0rc1/zcc/protocol.py` & `zcc-helper-3.1rc1/zcc/protocol.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.0rc1/zcc/socket.py` & `zcc-helper-3.1rc1/zcc/socket.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.0rc1/zcc/trace.py` & `zcc-helper-3.1rc1/zcc/trace.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.0rc1/zcc/watchdog.py` & `zcc-helper-3.1rc1/zcc/watchdog.py`

 * *Files identical despite different names*

### Comparing `zcc-helper-3.0rc1/zcc_helper.egg-info/PKG-INFO` & `zcc-helper-3.1rc1/zcc_helper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcc-helper
-Version: 3.0rc1
+Version: 3.1rc1
 Summary: ZIMI ZCC helper module
 Home-page: UNKNOWN
 Author: Mark Hannon
 Author-email: mark.hannon@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -216,22 +216,37 @@
     def room(self) -> str:
         '''Gets a descriptive string of the device room'''
 
     def type(self) -> str:
         '''Gets a descriptive string of the device type'''
 ```
 
-In addition, you can subscribe to a notification for changes to the device state by using:
+In addition, you can subscribe to a notification for changes to the device state by using the following methods of the device object.
 
-```
-device.subscribe(observer)
+```python
+    def subscribe(self, observer):
+        '''Subscribe an observer object for state changes.
+        Observer object must include notify(self, observable, *args, **kwargs) method.'''
+
+    def unsubscribe(self, observer):
+        '''Unsubscribe an observer object.'''
 ```
 
 The observer object must have a notify(observable) method.
 
+Finally, you can initiate a watchdog function that will periodically refresh the device states from the ZCC.   This can be useful for long lived connections that may time-out as it will trigger a re-connection if needed.
+
+```python
+    def start_watchdog(self, timer: int):
+        '''Start a periodic timeout that resets every time a status update is received.'''
+
+    def stop_watchdog(self):
+        '''Stop the periodic timeout.'''
+
+```
 ### Command Line Program
 
 ZCC can also be used as a command line tool to discover ZCC devices and/or execute actions upon them.
 
 ```
 $ python3 -m zcc
 usage: zcc [-h] [--verbosity VERBOSITY] (--discover | --execute) [--host HOST] [--port PORT] [--timeout TIMEOUT] [--device DEVICE]
```

