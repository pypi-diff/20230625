# Comparing `tmp/voicemeeter-api-1.0.0.tar.gz` & `tmp/voicemeeter-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-api-1.0.0.tar", max compression
+gzip compressed data, was "voicemeeter-api-2.0.0.tar", max compression
```

## Comparing `voicemeeter-api-1.0.0.tar` & `voicemeeter-api-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter-api-1.0.0/LICENSE
--rw-r--r--   0        0        0      835 2023-06-19 19:13:47.663268 voicemeeter-api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    14994 2022-10-18 18:16:01.000112 voicemeeter-api-1.0.0/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter-api-1.0.0/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8094 2022-10-16 16:28:43.116181 voicemeeter-api-1.0.0/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     3590 2022-08-08 13:33:38.443073 voicemeeter-api-1.0.0/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1249 2022-07-22 14:05:44.167922 voicemeeter-api-1.0.0/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5547 2022-09-28 22:57:08.807371 voicemeeter-api-1.0.0/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter-api-1.0.0/voicemeeterlib/device.py
--rw-r--r--   0        0        0      251 2022-07-07 14:44:58.387087 voicemeeter-api-1.0.0/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2044 2022-10-06 16:39:46.744854 voicemeeter-api-1.0.0/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7525 2023-06-19 18:13:07.464008 voicemeeter-api-1.0.0/voicemeeterlib/factory.py
--rw-r--r--   0        0        0      988 2022-07-07 14:44:58.388087 voicemeeter-api-1.0.0/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1140 2022-10-11 11:49:25.582533 voicemeeter-api-1.0.0/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2302 2022-08-08 13:33:38.445073 voicemeeter-api-1.0.0/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1091 2022-10-16 16:37:25.001225 voicemeeter-api-1.0.0/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1126 2022-10-11 11:06:58.539729 voicemeeter-api-1.0.0/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6192 2022-09-28 23:00:10.867422 voicemeeter-api-1.0.0/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     1972 2022-07-22 14:04:26.664193 voicemeeter-api-1.0.0/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0     9860 2023-06-19 18:13:07.485347 voicemeeter-api-1.0.0/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    11421 2022-10-27 07:42:21.310552 voicemeeter-api-1.0.0/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     1389 2022-09-29 10:29:54.452484 voicemeeter-api-1.0.0/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2025 2022-10-04 12:36:39.540193 voicemeeter-api-1.0.0/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2022-08-08 13:33:38.447073 voicemeeter-api-1.0.0/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4470 2022-08-08 13:33:38.448073 voicemeeter-api-1.0.0/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    16024 2023-06-19 19:14:33.802225 voicemeeter-api-1.0.0/setup.py
--rw-r--r--   0        0        0    14900 2023-06-19 19:14:33.803230 voicemeeter-api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter-api-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1111 2023-06-24 18:24:26.154130 voicemeeter-api-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    16337 2023-06-23 20:30:05.514700 voicemeeter-api-2.0.0/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter-api-2.0.0/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-06-23 19:51:19.906407 voicemeeter-api-2.0.0/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4239 2023-06-22 23:20:33.622570 voicemeeter-api-2.0.0/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-06-22 23:31:24.097081 voicemeeter-api-2.0.0/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5819 2023-06-22 09:43:14.446510 voicemeeter-api-2.0.0/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter-api-2.0.0/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      273 2023-06-23 00:41:14.485078 voicemeeter-api-2.0.0/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter-api-2.0.0/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-06-24 14:44:36.324150 voicemeeter-api-2.0.0/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-06-22 23:31:40.238138 voicemeeter-api-2.0.0/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-06-23 20:52:02.185334 voicemeeter-api-2.0.0/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2352 2023-06-22 02:21:02.337418 voicemeeter-api-2.0.0/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1063 2023-06-22 23:31:57.569332 voicemeeter-api-2.0.0/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter-api-2.0.0/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6192 2022-09-28 23:00:10.867422 voicemeeter-api-2.0.0/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     1968 2023-06-21 12:25:36.590976 voicemeeter-api-2.0.0/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    11015 2023-06-24 13:58:45.428941 voicemeeter-api-2.0.0/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15325 2023-06-23 19:51:13.562428 voicemeeter-api-2.0.0/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-23 16:22:05.659320 voicemeeter-api-2.0.0/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2988 2023-06-23 14:21:43.420787 voicemeeter-api-2.0.0/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     1971 2023-06-24 14:44:29.680645 voicemeeter-api-2.0.0/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4470 2022-08-08 13:33:38.448073 voicemeeter-api-2.0.0/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    17514 2023-06-24 22:58:48.695033 voicemeeter-api-2.0.0/setup.py
+-rw-r--r--   0        0        0    16169 2023-06-24 22:58:48.696033 voicemeeter-api-2.0.0/PKG-INFO
```

### Comparing `voicemeeter-api-1.0.0/LICENSE` & `voicemeeter-api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-1.0.0/README.md` & `voicemeeter-api-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -48,51 +48,52 @@
         self.vm.strip[0].mute = True
         print(
             f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"
         )
 
     def other_things(self):
         self.vm.bus[3].gain = -6.3
-        self.vm.bus[4].eq = True
+        self.vm.bus[4].eq.on = True
         info = (
             f"bus 3 gain has been set to {self.vm.bus[3].gain}",
-            f"bus 4 eq has been set to {self.vm.bus[4].eq}",
+            f"bus 4 eq has been set to {self.vm.bus[4].eq.on}",
         )
         print("\n".join(info))
 
 
 def main():
-    with voicemeeterlib.api(kind_id) as vm:
+    KIND_ID = "banana"
+
+    with voicemeeterlib.api(KIND_ID) as vm:
         do = ManyThings(vm)
         do.things()
         do.other_things()
 
         # set many parameters at once
         vm.apply(
             {
                 "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-                "bus-2": {"mute": True},
+                "bus-2": {"mute": True, "eq": {"on": True}},
                 "button-0": {"state": True},
                 "vban-in-0": {"on": True},
                 "vban-out-1": {"name": "streamname"},
             }
         )
 
 
 if __name__ == "__main__":
-    kind_id = "banana"
-
     main()
+
 ```
 
 Otherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.
 
-## `kind_id`
+## `KIND_ID`
 
-Pass the kind of Voicemeeter as an argument. kind_id may be:
+Pass the kind of Voicemeeter as an argument. KIND_ID may be:
 
 -   `basic`
 -   `banana`
 -   `potato`
 
 ## `Available commands`
 
@@ -100,16 +101,14 @@
 
 The following properties are available.
 
 -   `mono`: boolean
 -   `solo`: boolean
 -   `mute`: boolean
 -   `gain`: float, from -60.0 to 12.0
--   `comp`: float, from 0.0 to 10.0
--   `gate`: float, from 0.0 to 10.0
 -   `audibility`: float, from 0.0 to 10.0
 -   `limit`: int, from -40 to 12
 -   `A1 - A5`, `B1 - B3`: boolean
 -   `label`: string
 -   `mc`: boolean
 -   `k`: int, from 0 to 4
 -   `bass`: float, from -12.0 to 12.0
@@ -150,27 +149,92 @@
 example:
 
 ```python
 vm.strip[5].appmute("Spotify", True)
 vm.strip[5].appgain("Spotify", 0.5)
 ```
 
-##### Gainlayers
+#### Strip.Comp
+
+-   `knob`: float, from 0.0 to 10.0
+-   `gainin`: float, from -24.0 to 24.0
+-   `ratio`: float, from 1.0 to 8.0
+-   `threshold`: float, from -40.0 to -3.0
+-   `attack`: float, from 0.0 to 200.0
+-   `release`: float, from 0.0 to 5000.0
+-   `knee`: float, from 0.0 to 1.0
+-   `gainout`: float, from -24.0 to 24.0
+-   `makeup`: boolean
+
+example:
+
+```python
+print(vm.strip[4].comp.knob)
+```
+
+Strip Comp parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.Gate
+
+-   `knob`: float, from 0.0 to 10.0
+-   `threshold`: float, from -60.0 to -10.0
+-   `damping`: float, from -60.0 to -10.0
+-   `bpsidechain`: int, from 100 to 4000
+-   `attack`: float, from 0.0 to 1000.0
+-   `hold`: float, from 0.0 to 5000.0
+-   `release`: float, from 0.0 to 5000.0
+
+example:
+
+```python
+vm.strip[2].gate.attack = 300.8
+```
+
+Strip Gate parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.Denoiser
+
+-   `knob`: float, from 0.0 to 10.0
+
+example:
+
+```python
+vm.strip[0].denoiser.knob = 0.5
+```
+
+Strip Denoiser parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+example:
+
+```python
+vm.strip[0].eq.ab = True
+```
+
+Strip EQ parameters are defined for PhysicalStrips, potato version only.
+
+##### Strip.Gainlayers
 
 -   `gain`: float, from -60.0 to 12.0
 
 example:
 
 ```python
 vm.strip[3].gainlayer[3].gain = 3.7
 ```
 
 Gainlayers are defined for potato version only.
 
-##### Levels
+##### Strip.Levels
 
 The following properties are available.
 
 -   `prefader`
 -   `postfader`
 -   `postmute`
 
@@ -183,16 +247,14 @@
 Level properties will return -200.0 if no audio detected.
 
 ### Bus
 
 The following properties are available.
 
 -   `mono`: boolean
--   `eq`: boolean
--   `eq_ab`: boolean
 -   `mute`: boolean
 -   `sel`: boolean
 -   `gain`: float, from -60.0 to 12.0
 -   `label`: string
 -   `returnreverb`: float, from 0.0 to 10.0
 -   `returndelay`: float, from 0.0 to 10.0
 -   `returnfx1`: float, from 0.0 to 10.0
@@ -204,15 +266,28 @@
 ```python
 vm.bus[3].gain = 3.7
 print(vm.bus[0].label)
 
 vm.bus[4].mono = True
 ```
 
-##### Modes
+##### Bus.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+example:
+
+```python
+vm.bus[3].eq.on = True
+```
+
+##### Bus.Modes
 
 The following properties are available.
 
 -   `normal`: boolean
 -   `amix`: boolean
 -   `bmix`: boolean
 -   `composite`: boolean
@@ -232,15 +307,15 @@
 
 ```python
 vm.bus[4].mode.amix = True
 
 print(vm.bus[2].mode.get())
 ```
 
-##### Levels
+##### Bus.Levels
 
 The following properties are available.
 
 -   `all`
 
 example:
 
@@ -405,15 +480,15 @@
 -   `ins` `outs` : Returns the number of input/output devices
 -   `input(i)` `output(i)` : Returns a dict of device properties for device[i]
 
 example:
 
 ```python
 import voicemeeterlib
-with voicemeeterlib.api(kind_id) as vm:
+with voicemeeterlib.api(KIND_ID) as vm:
     for i in range(vm.device.ins):
         print(vm.device.input(i))
 ```
 
 ### FX
 
 The following properties are available:
@@ -558,15 +633,15 @@
 -   `apply`
     Set many strip/bus/macrobutton/vban parameters at once, for example:
 
 ```python
 vm.apply(
     {
         "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-        "bus-2": {"mute": True},
+        "bus-2": {"mute": True, "eq": {"on": True}},
         "button-0": {"state": True},
         "vban-in-0": {"on": True},
         "vban-out-1": {"name": "streamname"},
     }
 )
 ```
 
@@ -591,42 +666,42 @@
     vm.apply_config('example')
 ```
 
 will load a user config file at configs/banana/example.toml for Voicemeeter Banana.
 
 ## Events
 
-Level updates are considered high volume, by default they are NOT listened for. Use subs keyword arg to initialize event updates.
+By default, NO events are listened for. Use events kwargs to enable specific event types.
 
 example:
 
 ```python
 import voicemeeterlib
-# Set updates to occur every 50ms
-# Listen for level updates but disable midi updates
-with voicemeeterlib.api('banana', ratelimit=0.05, subs={"ldirty": True, "midi": False}) as vm:
+# Set event updates to occur every 50ms
+# Listen for level updates only
+with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True}) as vm:
     ...
 ```
 
-#### `vm.subject`
+#### `vm.observer`
 
 Use the Subject class to register an app as event observer.
 
 The following methods are available:
 
 -   `add`: registers an app as an event observer
 -   `remove`: deregisters an app as an event observer
 
 example:
 
 ```python
 # register an app to receive updates
 class App():
     def __init__(self, vm):
-        vm.subject.add(self)
+        vm.observer.add(self)
         ...
 ```
 
 #### `vm.event`
 
 Use the event class to toggle updates as necessary.
 
@@ -660,25 +735,24 @@
 
 # get a list of currently subscribed
 print(vm.event.get())
 ```
 
 ## Remote class
 
-`voicemeeterlib.api(kind_id: str)`
+`voicemeeterlib.api(KIND_ID: str)`
 
 You may pass the following optional keyword arguments:
 
 -   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.
 -   `ratelimit`: float=0.033, how often to check for updates in ms.
--   `subs`: dict={"pdirty": True, "mdirty": True, "midi": True, "ldirty": False}, initialize which event updates to listen for.
-    -   `pdirty`: parameter updates
-    -   `mdirty`: macrobutton updates
-    -   `midi`: midi updates
-    -   `ldirty`: level updates
+-   `pdirty`: boolean=False, parameter updates
+-   `mdirty`: boolean=False, macrobutton updates
+-   `midi`: boolean=False, midi updates
+-   `ldirty`: boolean=False, level updates
 
 Access to lower level Getters and Setters are provided with these functions:
 
 -   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.
 -   `vm.set(param, value)`: For setting the value of any parameter.
 
 Access to lower level polling functions are provided with these functions:
@@ -701,8 +775,8 @@
 
 ```
 pytest -v
 ```
 
 ### Official Documentation
 
--   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/main/VoicemeeterRemoteAPI.pdf)
+-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/bus.py` & `voicemeeter-api-2.0.0/voicemeeterlib/bus.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,30 +43,14 @@
         return self.getter("mono") == 1
 
     @mono.setter
     def mono(self, val: bool):
         self.setter("mono", 1 if val else 0)
 
     @property
-    def eq(self) -> bool:
-        return self.getter("eq.On") == 1
-
-    @eq.setter
-    def eq(self, val: bool):
-        self.setter("eq.On", 1 if val else 0)
-
-    @property
-    def eq_ab(self) -> bool:
-        return self.getter("eq.ab") == 1
-
-    @eq_ab.setter
-    def eq_ab(self, val: bool):
-        self.setter("eq.ab", 1 if val else 0)
-
-    @property
     def sel(self) -> bool:
         return self.getter("sel") == 1
 
     @sel.setter
     def sel(self, val: bool):
         self.setter("sel", 1 if val else 0)
 
@@ -99,14 +83,36 @@
         time.sleep(self._remote.DELAY)
 
     def fadeby(self, change: float, time_: int):
         self.setter("FadeBy", f"({change}, {time_})")
         time.sleep(self._remote.DELAY)
 
 
+class BusEQ(IRemote):
+    @property
+    def identifier(self) -> str:
+        return f"Bus[{self.index}].eq"
+
+    @property
+    def on(self) -> bool:
+        return self.getter("on") == 1
+
+    @on.setter
+    def on(self, val: bool):
+        self.setter("on", 1 if val else 0)
+
+    @property
+    def ab(self) -> bool:
+        return self.getter("ab") == 1
+
+    @ab.setter
+    def ab(self, val: bool):
+        self.setter("ab", 1 if val else 0)
+
+
 class PhysicalBus(Bus):
     @classmethod
     def make(cls, remote, i, kind):
         """
         Factory method for PhysicalBus.
 
         Returns a PhysicalBus class.
@@ -305,14 +311,15 @@
     BUSMODEMIXIN_cls = _make_bus_mode_mixin()
     return type(
         f"{BUS_cls.__name__}{remote.kind}",
         (BUS_cls,),
         {
             "levels": BusLevel(remote, i),
             "mode": BUSMODEMIXIN_cls(remote, i),
+            "eq": BusEQ(remote, i),
         },
     )(remote, i)
 
 
 def request_bus_obj(phys_bus, remote, i) -> Bus:
     """
     Bus entry point. Wraps factory method.
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/command.py` & `voicemeeter-api-2.0.0/voicemeeterlib/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from .error import VMError
 from .iremote import IRemote
-from .meta import action_prop
+from .meta import action_fn
 
 
 class Command(IRemote):
     """
     Implements the common interface
 
     Defines concrete implementation for command
@@ -18,18 +17,17 @@
         Returns a Command class of a kind.
         """
         CMD_cls = type(
             f"Command{remote.kind}",
             (cls,),
             {
                 **{
-                    param: action_prop(param)
-                    for param in ["show", "shutdown", "restart"]
+                    param: action_fn(param) for param in ["show", "shutdown", "restart"]
                 },
-                "hide": action_prop("show", val=0),
+                "hide": action_fn("show", val=0),
             },
         )
         return CMD_cls(remote)
 
     def __str__(self):
         return f"{type(self).__name__}"
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/config.py` & `voicemeeter-api-2.0.0/voicemeeterlib/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import itertools
 import logging
 from pathlib import Path
 
+from .error import VMError
+
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
 from .kinds import request_kind_map as kindmap
 
+logger = logging.getLogger(__name__)
+
 
 class TOMLStrBuilder:
     """builds a config profile, as a string, for the toml parser"""
 
     def __init__(self, kind):
         self.kind = kind
         self.higher = itertools.chain(
@@ -28,18 +32,25 @@
                 "solo = false",
                 "gain = 0.0",
             ]
             + [f"A{i} = false" for i in range(1, self.kind.phys_out + 1)]
             + [f"B{i} = false" for i in range(1, self.kind.virt_out + 1)]
         )
         self.phys_strip_params = self.virt_strip_params + [
-            "comp = 0.0",
-            "gate = 0.0",
+            "comp.knob = 0.0",
+            "gate.knob = 0.0",
+            "denoiser.knob = 0.0",
+            "eq.on = false",
+        ]
+        self.bus_params = [
+            "mono = false",
+            "eq.on = false",
+            "mute = false",
+            "gain = 0.0",
         ]
-        self.bus_bool = ["mono = false", "eq = false", "mute = false"]
 
         if profile == "reset":
             self.reset_config()
 
     def reset_config(self):
         self.phys_strip_params = list(
             map(lambda x: x.replace("B1 = false", "B1 = true"), self.phys_strip_params)
@@ -62,15 +73,15 @@
             case "strip":
                 toml_str += ("\n").join(
                     self.phys_strip_params
                     if int(index) < self.kind.phys_in
                     else self.virt_strip_params
                 )
             case "bus":
-                toml_str += ("\n").join(self.bus_bool)
+                toml_str += ("\n").join(self.bus_params)
             case _:
                 pass
         return toml_str + "\n"
 
 
 class TOMLDataExtractor:
     def __init__(self, file):
@@ -115,18 +126,17 @@
     invokes the parser
 
     checks if config already in memory
 
     loads data into memory if not found
     """
 
-    logger = logging.getLogger("config.Loader")
-
     def __init__(self, kind):
         self._kind = kind
+        self.logger = logger.getChild(self.__class__.__name__)
         self._configs = dict()
         self.defaults(kind)
         self.parser = None
 
     def defaults(self, kind):
         self.builder = TOMLStrBuilder(kind)
         toml_str = self.builder.build()
@@ -162,24 +172,24 @@
     """
     traverses defined paths for config files
 
     directs the loader
 
     returns configs loaded into memory
     """
-    logger = logging.getLogger("config.loader")
+    logger_loader = logger.getChild("loader")
     loader = Loader(kind)
 
     for path in (
         Path.cwd() / "configs" / kind.name,
-        Path(__file__).parent / "configs" / kind.name,
-        Path.home() / "Documents/Voicemeeter" / "configs" / kind.name,
+        Path.home() / ".config" / "voicemeeter" / kind.name,
+        Path.home() / "Documents" / "Voicemeeter" / "configs" / kind.name,
     ):
         if path.is_dir():
-            logger.info(f"Checking [{path}] for TOML config files:")
+            logger_loader.info(f"Checking [{path}] for TOML config files:")
             for file in path.glob("*.toml"):
                 identifier = file.with_suffix("").stem
                 if loader.parse(identifier, file):
                     loader.register(identifier)
     return loader.configs
 
 
@@ -188,9 +198,9 @@
     config entry point.
 
     Returns all configs loaded into memory for a kind
     """
     try:
         configs = loader(kindmap(kind_id))
     except KeyError as e:
-        print(f"Unknown Voicemeeter kind '{kind_id}'")
+        raise VMError(f"Unknown Voicemeeter kind {kind_id}") from e
     return configs
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/device.py` & `voicemeeter-api-2.0.0/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/event.py` & `voicemeeter-api-2.0.0/voicemeeterlib/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from typing import Iterable, Union
 
+logger = logging.getLogger(__name__)
+
 
 class Event:
     """Keeps track of event subscriptions"""
 
-    logger = logging.getLogger("event.event")
-
     def __init__(self, subs: dict):
         self.subs = subs
+        self.logger = logger.getChild(self.__class__.__name__)
 
     def info(self, msg=None):
         info = (f"{msg} events",) if msg else ()
         if self.any():
             info += (f"now listening for {', '.join(self.get())} events",)
         else:
             info += (f"not listening for any events",)
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/factory.py` & `voicemeeter-api-2.0.0/voicemeeterlib/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 from typing import Iterable, NoReturn
 
 from . import misc
 from .bus import request_bus_obj as bus
 from .command import Command
 from .config import request_config as configs
 from .device import Device
+from .error import VMError
 from .kinds import KindMapClass
 from .kinds import request_kind_map as kindmap
 from .macrobutton import MacroButton
 from .recorder import Recorder
 from .remote import Remote
 from .strip import request_strip_obj as strip
 from .vban import request_vban_obj as vban
 
+logger = logging.getLogger(__name__)
+
 
 class FactoryBuilder:
     """
     Builder class for factories.
 
     Separates construction from representation.
     """
 
-    logger = logging.getLogger("remote.factorybuilder")
     BuilderProgress = IntEnum(
         "BuilderProgress",
         "strip bus command macrobutton vban device option recorder patch fx",
         start=0,
     )
 
     def __init__(self, factory, kind: KindMapClass):
@@ -43,19 +45,20 @@
             f"Finished building vban in/out streams for {self._factory}",
             f"Finished building device for {self._factory}",
             f"Finished building option for {self._factory}",
             f"Finished building recorder for {self._factory}",
             f"Finished building patch for {self._factory}",
             f"Finished building fx for {self._factory}",
         )
+        self.logger = logger.getChild(self.__class__.__name__)
 
     def _pinfo(self, name: str) -> NoReturn:
         """prints progress status for each step"""
         name = name.split("_")[1]
-        self.logger.info(self._info[int(getattr(self.BuilderProgress, name))])
+        self.logger.debug(self._info[int(getattr(self.BuilderProgress, name))])
 
     def make_strip(self):
         self._factory.strip = tuple(
             strip(i < self.kind.phys_in, self._factory, i)
             for i in range(self.kind.num_strip)
         )
         return self
@@ -100,18 +103,24 @@
         return self
 
 
 class FactoryBase(Remote):
     """Base class for factories, subclasses Remote."""
 
     def __init__(self, kind_id: str, **kwargs):
-        defaultevents = {"pdirty": True, "mdirty": True, "midi": True, "ldirty": False}
+        defaultkwargs = {
+            "sync": False,
+            "ratelimit": 0.033,
+            "pdirty": False,
+            "mdirty": False,
+            "midi": False,
+            "ldirty": False,
+        }
         if "subs" in kwargs:
-            defaultevents = defaultevents | kwargs.pop("subs")
-        defaultkwargs = {"sync": False, "ratelimit": 0.033, "subs": defaultevents}
+            defaultkwargs |= kwargs.pop("subs")  # for backwards compatibility
         kwargs = defaultkwargs | kwargs
         self.kind = kindmap(kind_id)
         super().__init__(**kwargs)
         self.builder = FactoryBuilder(self, self.kind)
         self._steps = (
             self.builder.make_strip,
             self.builder.make_bus,
@@ -227,13 +236,17 @@
 
 def request_remote_obj(kind_id: str, **kwargs) -> Remote:
     """
     Interface entry point. Wraps factory method and handles errors
 
     Returns a reference to a Remote class of a kind
     """
+
+    logger_entry = logger.getChild("request_remote_obj")
+
     REMOTE_obj = None
     try:
         REMOTE_obj = remote_factory(kind_id, **kwargs)
     except (ValueError, TypeError) as e:
-        raise SystemExit(e)
+        logger_entry.exception(f"{type(e).__name__}: {e}")
+        raise VMError(str(e)) from e
     return REMOTE_obj
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/inst.py` & `voicemeeter-api-2.0.0/voicemeeterlib/inst.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 )
 
 
 def get_vmpath():
     with winreg.OpenKey(
         winreg.HKEY_LOCAL_MACHINE, r"{}".format(REG_KEY + "\\" + VM_KEY)
     ) as vm_key:
-        path = winreg.QueryValueEx(vm_key, r"UninstallString")[0]
-    return path
+        return winreg.QueryValueEx(vm_key, r"UninstallString")[0]
 
 
-vm_path = Path(get_vmpath())
+try:
+    vm_path = Path(get_vmpath())
+except FileNotFoundError as e:
+    raise InstallError(f"Unable to fetch DLL path from the registry") from e
 vm_parent = vm_path.parent
 
 DLL_NAME = f'VoicemeeterRemote{"64" if bits == 64 else ""}.dll'
 
 dll_path = vm_parent.joinpath(DLL_NAME)
 if not dll_path.is_file():
-    raise InstallError(f"Could not find {DLL_NAME}")
+    raise InstallError(f"Could not find {dll_path}")
 
 libc = ct.CDLL(str(dll_path))
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/kinds.py` & `voicemeeter-api-2.0.0/voicemeeterlib/kinds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 
+from .error import VMError
+
 
 @unique
 class KindId(Enum):
     BASIC = 1
     BANANA = 2
     POTATO = 3
 
@@ -101,12 +103,12 @@
 
 
 def request_kind_map(kind_id):
     KIND_obj = None
     try:
         KIND_obj = kind_factory(kind_id)
     except ValueError as e:
-        print(e)
+        raise VMError(str(e)) from e
     return KIND_obj
 
 
 kinds_all = list(request_kind_map(kind_id.name.lower()) for kind_id in KindId)
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/macrobutton.py` & `voicemeeter-api-2.0.0/voicemeeterlib/macrobutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .error import VMError
 from .iremote import IRemote
 
 
 class Adapter(IRemote):
     """Adapter to the common interface."""
 
     def identifier(self):
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/meta.py` & `voicemeeter-api-2.0.0/voicemeeterlib/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
     def fset(self, val):
         self.setter(param, val)
 
     return property(fget, fset)
 
 
-def action_prop(param, val: int = 1):
-    """A param that performs an action"""
+def action_fn(param, val: int = 1):
+    """meta function that performs an action"""
 
     def fdo(self):
         self.setter(param, val)
 
     return fdo
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/misc.py` & `voicemeeter-api-2.0.0/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/recorder.py` & `voicemeeter-api-2.0.0/voicemeeterlib/recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .error import VMError
 from .iremote import IRemote
 from .kinds import kinds_all
-from .meta import action_prop, bool_prop
+from .meta import action_fn, bool_prop
 
 
 class Recorder(IRemote):
     """
     Implements the common interface
 
     Defines concrete implementation for recorder
@@ -20,15 +20,15 @@
         """
         CHANNELOUTMIXIN_cls = _make_channelout_mixins[remote.kind.name]
         REC_cls = type(
             f"Recorder{remote.kind}",
             (cls, CHANNELOUTMIXIN_cls),
             {
                 **{
-                    param: action_prop(param)
+                    param: action_fn(param)
                     for param in [
                         "play",
                         "stop",
                         "pause",
                         "replay",
                         "record",
                         "ff",
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/remote.py` & `voicemeeter-api-2.0.0/voicemeeterlib/remote.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,205 +1,226 @@
 import ctypes as ct
 import logging
 import time
 from abc import abstractmethod
-from functools import partial
+from queue import Queue
 from typing import Iterable, NoReturn, Optional, Union
 
 from .cbindings import CBindings
 from .error import CAPIError, VMError
 from .event import Event
 from .inst import bits
 from .kinds import KindId
 from .misc import Midi
 from .subject import Subject
-from .updater import Updater
+from .updater import Producer, Updater
 from .util import grouper, polling, script
 
+logger = logging.getLogger(__name__)
+
 
 class Remote(CBindings):
     """Base class responsible for wrapping the C Remote API"""
 
-    logger = logging.getLogger("remote.remote")
     DELAY = 0.001
 
     def __init__(self, **kwargs):
         self.strip_mode = 0
         self.cache = {}
-        self.cache["strip_level"], self.cache["bus_level"] = self._get_levels()
         self.midi = Midi()
-        self.subject = Subject()
-        self.running = None
+        self.subject = self.observer = Subject()
+        self.running = False
+        self.event = Event(
+            {k: kwargs.pop(k) for k in ("pdirty", "mdirty", "midi", "ldirty")}
+        )
+        self.logger = logger.getChild(self.__class__.__name__)
 
         for attr, val in kwargs.items():
             setattr(self, attr, val)
 
-        self.event = Event(self.subs)
-
     def __enter__(self):
         """setup procedures"""
         self.login()
-        self.init_thread()
+        if self.event.any():
+            self.init_thread()
         return self
 
     @abstractmethod
     def __str__(self):
         """Ensure subclasses override str magic method"""
         pass
 
     def init_thread(self):
         """Starts updates thread."""
         self.running = True
         self.event.info()
 
-        self.updater = Updater(self)
+        self.logger.debug("initiating events thread")
+        queue = Queue()
+        self.updater = Updater(self, queue)
         self.updater.start()
+        self.producer = Producer(self, queue)
+        self.producer.start()
 
     def login(self) -> NoReturn:
         """Login to the API, initialize dirty parameters"""
-        res = self.vm_login()
+        res = self.call(self.vm_login, ok=(0, 1))
         if res == 1:
+            self.logger.info(
+                "Voicemeeter engine running but GUI not launched. Launching the GUI now."
+            )
             self.run_voicemeeter(self.kind.name)
-        elif res != 0:
-            raise CAPIError(f"VBVMR_Login returned {res}")
         self.logger.info(f"{type(self).__name__}: Successfully logged into {self}")
         self.clear_dirty()
 
     def run_voicemeeter(self, kind_id: str) -> NoReturn:
         if kind_id not in (kind.name.lower() for kind in KindId):
             raise VMError(f"Unexpected Voicemeeter type: '{kind_id}'")
         if kind_id == "potato" and bits == 8:
             value = KindId[kind_id.upper()].value + 3
         else:
             value = KindId[kind_id.upper()].value
-        self.vm_runvm(value)
+        self.call(self.vm_runvm, value)
         time.sleep(1)
 
     @property
     def type(self) -> str:
         """Returns the type of Voicemeeter installation (basic, banana, potato)."""
         type_ = ct.c_long()
-        self.vm_get_type(ct.byref(type_))
+        self.call(self.vm_get_type, ct.byref(type_))
         return KindId(type_.value).name.lower()
 
     @property
     def version(self) -> str:
         """Returns Voicemeeter's version as a string"""
         ver = ct.c_long()
-        self.vm_get_version(ct.byref(ver))
+        self.call(self.vm_get_version, ct.byref(ver))
         return "{}.{}.{}.{}".format(
             (ver.value & 0xFF000000) >> 24,
             (ver.value & 0x00FF0000) >> 16,
             (ver.value & 0x0000FF00) >> 8,
             ver.value & 0x000000FF,
         )
 
     @property
     def pdirty(self) -> bool:
         """True iff UI parameters have been updated."""
-        return self.vm_pdirty() == 1
+        return self.call(self.vm_pdirty, ok=(0, 1)) == 1
 
     @property
     def mdirty(self) -> bool:
         """True iff MB parameters have been updated."""
-        return self.vm_mdirty() == 1
+        try:
+            return self.call(self.vm_mdirty, ok=(0, 1)) == 1
+        except AttributeError as e:
+            self.logger.exception(f"{type(e).__name__}: {e}")
+            raise CAPIError(
+                "no bind for VBVMR_MacroButton_IsDirty. are you using an old version of the API?"
+            ) from e
 
     @property
     def ldirty(self) -> bool:
         """True iff levels have been updated."""
         self._strip_buf, self._bus_buf = self._get_levels()
         return not (
             self.cache.get("strip_level") == self._strip_buf
             and self.cache.get("bus_level") == self._bus_buf
         )
 
-    def clear_dirty(self):
-        while self.pdirty or self.mdirty:
-            pass
+    def clear_dirty(self) -> NoReturn:
+        try:
+            while self.pdirty or self.mdirty:
+                pass
+        except CAPIError:
+            self.logger.error("no bind for mdirty, clearing pdirty only")
+            while self.pdirty:
+                pass
 
     @polling
     def get(self, param: str, is_string: Optional[bool] = False) -> Union[str, float]:
         """Gets a string or float parameter"""
         if is_string:
             buf = ct.create_unicode_buffer(512)
-            self.call(
-                partial(self.vm_get_parameter_string, param.encode(), ct.byref(buf))
-            )
+            self.call(self.vm_get_parameter_string, param.encode(), ct.byref(buf))
         else:
             buf = ct.c_float()
-            self.call(
-                partial(self.vm_get_parameter_float, param.encode(), ct.byref(buf))
-            )
+            self.call(self.vm_get_parameter_float, param.encode(), ct.byref(buf))
         return buf.value
 
     def set(self, param: str, val: Union[str, float]) -> NoReturn:
         """Sets a string or float parameter. Caches value"""
         if isinstance(val, str):
             if len(val) >= 512:
                 raise VMError("String is too long")
-            self.call(
-                partial(self.vm_set_parameter_string, param.encode(), ct.c_wchar_p(val))
-            )
+            self.call(self.vm_set_parameter_string, param.encode(), ct.c_wchar_p(val))
         else:
             self.call(
-                partial(
-                    self.vm_set_parameter_float, param.encode(), ct.c_float(float(val))
-                )
+                self.vm_set_parameter_float, param.encode(), ct.c_float(float(val))
             )
         self.cache[param] = val
 
     @polling
     def get_buttonstatus(self, id: int, mode: int) -> int:
         """Gets a macrobutton parameter"""
         state = ct.c_float()
-        self.call(
-            partial(
+        try:
+            self.call(
                 self.vm_get_buttonstatus,
                 ct.c_long(id),
                 ct.byref(state),
                 ct.c_long(mode),
             )
-        )
+        except AttributeError as e:
+            self.logger.exception(f"{type(e).__name__}: {e}")
+            raise CAPIError(
+                "no bind for VBVMR_MacroButton_GetStatus. are you using an old version of the API?"
+            ) from e
         return int(state.value)
 
     def set_buttonstatus(self, id: int, state: int, mode: int) -> NoReturn:
         """Sets a macrobutton parameter. Caches value"""
         c_state = ct.c_float(float(state))
-        self.call(
-            partial(self.vm_set_buttonstatus, ct.c_long(id), c_state, ct.c_long(mode))
-        )
+        try:
+            self.call(self.vm_set_buttonstatus, ct.c_long(id), c_state, ct.c_long(mode))
+        except AttributeError as e:
+            self.logger.exception(f"{type(e).__name__}: {e}")
+            raise CAPIError(
+                "no bind for VBVMR_MacroButton_SetStatus. are you using an old version of the API?"
+            ) from e
         self.cache[f"mb_{id}_{mode}"] = int(c_state.value)
 
     def get_num_devices(self, direction: str = None) -> int:
         """Retrieves number of physical devices connected"""
         if direction not in ("in", "out"):
             raise VMError("Expected a direction: in or out")
         func = getattr(self, f"vm_get_num_{direction}devices")
-        return func()
+        res = self.call(func, ok_exp=lambda r: r >= 0)
+        return res
 
     def get_device_description(self, index: int, direction: str = None) -> tuple:
         """Returns a tuple of device parameters"""
         if direction not in ("in", "out"):
             raise VMError("Expected a direction: in or out")
         type_ = ct.c_long()
         name = ct.create_unicode_buffer(256)
         hwid = ct.create_unicode_buffer(256)
         func = getattr(self, f"vm_get_desc_{direction}devices")
-        func(
+        self.call(
+            func,
             ct.c_long(index),
             ct.byref(type_),
             ct.byref(name),
             ct.byref(hwid),
         )
         return (name.value, type_.value, hwid.value)
 
     def get_level(self, type_: int, index: int) -> float:
         """Retrieves a single level value"""
         val = ct.c_float()
-        self.vm_get_level(ct.c_long(type_), ct.c_long(index), ct.byref(val))
+        self.call(self.vm_get_level, ct.c_long(type_), ct.c_long(index), ct.byref(val))
         return val.value
 
     def _get_levels(self) -> Iterable:
         """
         returns both level arrays (strip_levels, bus_levels) BEFORE math conversion
         """
         return (
@@ -212,35 +233,33 @@
                 for i in range(8 * (self.kind.phys_out + self.kind.virt_out))
             ),
         )
 
     def get_midi_message(self):
         n = ct.c_long(1024)
         buf = ct.create_string_buffer(1024)
-        res = self.vm_get_midi_message(ct.byref(buf), n)
+        res = self.vm_get_midi_message(ct.byref(buf), n, ok_exp=lambda r: r >= 0)
         if res > 0:
             vals = tuple(
                 grouper(3, (int.from_bytes(buf[i], "little") for i in range(res)))
             )
             for msg in vals:
                 ch, pitch, vel = msg
                 if not self.midi._channel or self.midi._channel != ch:
                     self.midi._channel = ch
                 self.midi._most_recent = pitch
                 self.midi._set(pitch, vel)
             return True
-        elif res == -1 or res == -2:
-            raise CAPIError(f"VBVMR_GetMidiMessage returned {res}")
 
     @script
     def sendtext(self, script: str):
         """Sets many parameters from a script"""
         if len(script) > 48000:
             raise ValueError("Script too large, max size 48kB")
-        self.call(partial(self.vm_set_parameter_multi, script.encode()))
+        self.call(self.vm_set_parameter_multi, script.encode())
         time.sleep(self.DELAY * 5)
 
     def apply(self, data: dict):
         """
         Sets all parameters of a dict
 
         minor delay between each recursion
@@ -262,26 +281,25 @@
         error_msg = (
             f"No config with name '{name}' is loaded into memory",
             f"Known configs: {list(self.configs.keys())}",
         )
         try:
             self.apply(self.configs[name])
             self.logger.info(f"Profile '{name}' applied!")
-        except KeyError as e:
+        except KeyError:
             self.logger.error(("\n").join(error_msg))
 
     def logout(self) -> NoReturn:
         """Wait for dirty parameters to clear, then logout of the API"""
         self.clear_dirty()
         time.sleep(0.1)
-        res = self.vm_logout()
-        if res != 0:
-            raise CAPIError(f"VBVMR_Logout returned {res}")
+        self.call(self.vm_logout)
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
 
     def end_thread(self):
+        self.logger.debug("events thread shutdown started")
         self.running = False
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> NoReturn:
         """teardown procedures"""
         self.end_thread()
         self.logout()
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/strip.py` & `voicemeeter-api-2.0.0/voicemeeterlib/strip.py`

 * *Files 16% similar despite different names*

```diff
@@ -89,44 +89,208 @@
         Returns a PhysicalStrip class.
         """
         EFFECTS_cls = _make_effects_mixins(is_phys)[remote.kind.name]
         return type(
             f"PhysicalStrip",
             (cls, EFFECTS_cls),
             {
+                "comp": StripComp(remote, i),
+                "gate": StripGate(remote, i),
+                "denoiser": StripDenoiser(remote, i),
+                "eq": StripEQ(remote, i),
                 "device": StripDevice.make(remote, i),
             },
         )
 
     def __str__(self):
         return f"{type(self).__name__}{self.index}"
 
     @property
-    def comp(self) -> float:
-        return round(self.getter("Comp"), 1)
+    def audibility(self) -> float:
+        return round(self.getter("audibility"), 1)
+
+    @audibility.setter
+    def audibility(self, val: float):
+        self.setter("audibility", val)
+
 
-    @comp.setter
-    def comp(self, val: float):
-        self.setter("Comp", val)
+class StripComp(IRemote):
+    @property
+    def identifier(self) -> str:
+        return f"Strip[{self.index}].comp"
 
     @property
-    def gate(self) -> float:
-        return round(self.getter("Gate"), 1)
+    def knob(self) -> float:
+        return round(self.getter(""), 1)
 
-    @gate.setter
-    def gate(self, val: float):
-        self.setter("Gate", val)
+    @knob.setter
+    def knob(self, val: float):
+        self.setter("", val)
 
     @property
-    def audibility(self) -> float:
-        return round(self.getter("audibility"), 1)
+    def gainin(self) -> float:
+        return round(self.getter("GainIn"), 1)
 
-    @audibility.setter
-    def audibility(self, val: float):
-        self.setter("audibility", val)
+    @gainin.setter
+    def gainin(self, val: float):
+        self.setter("GainIn", val)
+
+    @property
+    def ratio(self) -> float:
+        return round(self.getter("Ratio"), 1)
+
+    @ratio.setter
+    def ratio(self, val: float):
+        self.setter("Ratio", val)
+
+    @property
+    def threshold(self) -> float:
+        return round(self.getter("Threshold"), 1)
+
+    @threshold.setter
+    def threshold(self, val: float):
+        self.setter("Threshold", val)
+
+    @property
+    def attack(self) -> float:
+        return round(self.getter("Attack"), 1)
+
+    @attack.setter
+    def attack(self, val: float):
+        self.setter("Attack", val)
+
+    @property
+    def release(self) -> float:
+        return round(self.getter("Release"), 1)
+
+    @release.setter
+    def release(self, val: float):
+        self.setter("Release", val)
+
+    @property
+    def knee(self) -> float:
+        return round(self.getter("Knee"), 1)
+
+    @knee.setter
+    def knee(self, val: float):
+        self.setter("Knee", val)
+
+    @property
+    def gainout(self) -> float:
+        return round(self.getter("GainOut"), 1)
+
+    @gainout.setter
+    def gainout(self, val: float):
+        self.setter("GainOut", val)
+
+    @property
+    def makeup(self) -> bool:
+        return self.getter("makeup") == 1
+
+    @makeup.setter
+    def makeup(self, val: bool):
+        self.setter("makeup", 1 if val else 0)
+
+
+class StripGate(IRemote):
+    @property
+    def identifier(self) -> str:
+        return f"Strip[{self.index}].gate"
+
+    @property
+    def knob(self) -> float:
+        return round(self.getter(""), 1)
+
+    @knob.setter
+    def knob(self, val: float):
+        self.setter("", val)
+
+    @property
+    def threshold(self) -> float:
+        return round(self.getter("Threshold"), 1)
+
+    @threshold.setter
+    def threshold(self, val: float):
+        self.setter("Threshold", val)
+
+    @property
+    def damping(self) -> float:
+        return round(self.getter("Damping"), 1)
+
+    @damping.setter
+    def damping(self, val: float):
+        self.setter("Damping", val)
+
+    @property
+    def bpsidechain(self) -> int:
+        return int(self.getter("BPSidechain"))
+
+    @bpsidechain.setter
+    def bpsidechain(self, val: int):
+        self.setter("BPSidechain", val)
+
+    @property
+    def attack(self) -> float:
+        return round(self.getter("Attack"), 1)
+
+    @attack.setter
+    def attack(self, val: float):
+        self.setter("Attack", val)
+
+    @property
+    def hold(self) -> float:
+        return round(self.getter("Hold"), 1)
+
+    @hold.setter
+    def hold(self, val: float):
+        self.setter("Hold", val)
+
+    @property
+    def release(self) -> float:
+        return round(self.getter("Release"), 1)
+
+    @release.setter
+    def release(self, val: float):
+        self.setter("Release", val)
+
+
+class StripDenoiser(IRemote):
+    @property
+    def identifier(self) -> str:
+        return f"Strip[{self.index}].denoiser"
+
+    @property
+    def knob(self) -> float:
+        return round(self.getter(""), 1)
+
+    @knob.setter
+    def knob(self, val: float):
+        self.setter("", val)
+
+
+class StripEQ(IRemote):
+    @property
+    def identifier(self) -> str:
+        return f"Strip[{self.index}].eq"
+
+    @property
+    def on(self) -> bool:
+        return self.getter("on") == 1
+
+    @on.setter
+    def on(self, val: bool):
+        self.setter("on", 1 if val else 0)
+
+    @property
+    def ab(self) -> bool:
+        return self.getter("ab") == 1
+
+    @ab.setter
+    def ab(self, val: bool):
+        self.setter("ab", 1 if val else 0)
 
 
 class StripDevice(IRemote):
     @classmethod
     def make(cls, remote, i):
         """
         Factory function for strip.device.
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/updater.py` & `voicemeeter-api-2.0.0/voicemeeterlib/updater.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,77 @@
+import logging
 import threading
 import time
 
 from .util import comp
 
+logger = logging.getLogger(__name__)
+
+
+class Producer(threading.Thread):
+    """Continously send job queue to the Updater thread at a rate of self._remote.ratelimit."""
+
+    def __init__(self, remote, queue):
+        super().__init__(name="producer", daemon=True)
+        self._remote = remote
+        self.queue = queue
+        self.logger = logger.getChild(self.__class__.__name__)
+
+    def run(self):
+        while self._remote.running:
+            if self._remote.event.pdirty:
+                self.queue.put("pdirty")
+            if self._remote.event.mdirty:
+                self.queue.put("mdirty")
+            if self._remote.event.midi:
+                self.queue.put("midi")
+            if self._remote.event.ldirty:
+                self.queue.put("ldirty")
+            time.sleep(self._remote.ratelimit)
+        self.logger.debug(f"terminating {self.getName()} thread")
+        self.queue.put(None)
+
 
 class Updater(threading.Thread):
-    def __init__(self, remote):
-        super().__init__(name="updater", target=self.update, daemon=True)
+    def __init__(self, remote, queue):
+        super().__init__(name="updater", daemon=True)
         self._remote = remote
+        self.queue = queue
         self._remote._strip_comp = [False] * (
             2 * self._remote.kind.phys_in + 8 * self._remote.kind.virt_in
         )
         self._remote._bus_comp = [False] * (self._remote.kind.num_bus * 8)
+        (
+            self._remote.cache["strip_level"],
+            self._remote.cache["bus_level"],
+        ) = self._remote._get_levels()
+        self.logger = logger.getChild(self.__class__.__name__)
 
     def _update_comps(self, strip_level, bus_level):
         self._remote._strip_comp, self._remote._bus_comp = (
             tuple(not x for x in comp(self._remote.cache["strip_level"], strip_level)),
             tuple(not x for x in comp(self._remote.cache["bus_level"], bus_level)),
         )
 
-    def update(self):
+    def run(self):
         """
         Continously update observers of dirty states.
 
         Generate _strip_comp, _bus_comp and update level cache if ldirty.
-
-        Runs updates at a rate of self.ratelimit.
         """
-        while self._remote.running:
-            start = time.time()
-            if self._remote.event.pdirty and self._remote.pdirty:
-                self._remote.subject.notify("pdirty")
-            if self._remote.event.mdirty and self._remote.mdirty:
-                self._remote.subject.notify("mdirty")
-            if self._remote.event.midi and self._remote.get_midi_message():
-                self._remote.subject.notify("midi")
-            if self._remote.event.ldirty and self._remote.ldirty:
+        while True:
+            event = self.queue.get()
+            if event is None:
+                self.logger.debug(f"terminating {self.getName()} thread")
+                break
+
+            if event == "pdirty" and self._remote.pdirty:
+                self._remote.subject.notify(event)
+            elif event == "mdirty" and self._remote.mdirty:
+                self._remote.subject.notify(event)
+            elif event == "midi" and self._remote.get_midi_message():
+                self._remote.subject.notify(event)
+            elif event == "ldirty" and self._remote.ldirty:
                 self._update_comps(self._remote._strip_buf, self._remote._bus_buf)
                 self._remote.cache["strip_level"] = self._remote._strip_buf
                 self._remote.cache["bus_level"] = self._remote._bus_buf
-                self._remote.subject.notify("ldirty")
-
-            elapsed = time.time() - start
-            if self._remote.event.any() and self._remote.ratelimit - elapsed > 0:
-                time.sleep(self._remote.ratelimit - elapsed)
-            else:
-                time.sleep(0.1)
+                self._remote.subject.notify(event)
```

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/util.py` & `voicemeeter-api-2.0.0/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-1.0.0/voicemeeterlib/vban.py` & `voicemeeter-api-2.0.0/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-1.0.0/setup.py` & `voicemeeter-api-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['dsl = scripts:ex_dsl',
+                     'events = scripts:ex_events',
+                     'gui = scripts:ex_gui',
+                     'levels = scripts:ex_levels',
                      'midi = scripts:ex_midi',
                      'obs = scripts:ex_obs',
                      'observer = scripts:ex_observer',
                      'test = scripts:test']}
 
 setup_kwargs = {
     'name': 'voicemeeter-api',
-    'version': '1.0.0',
+    'version': '2.0.0',
     'description': 'A Python wrapper for the Voiceemeter API',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-api.svg)](https://badge.fury.io/py/voicemeeter-api)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-api-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# Python Wrapper for Voicemeeter API\n\nThis package offers a Python interface for the Voicemeeter Remote C API.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.4\n-   Banana 2.0.6.4\n-   Potato 3.0.2.4\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install voicemeeter-api`\n\n## `Use`\n\nSimplest use case, use a context manager to request a Remote class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n#### `__main__.py`\n\n```python\nimport voicemeeterlib\n\n\nclass ManyThings:\n    def __init__(self, vm):\n        self.vm = vm\n\n    def things(self):\n        self.vm.strip[0].label = "podmic"\n        self.vm.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vm.bus[3].gain = -6.3\n        self.vm.bus[4].eq = True\n        info = (\n            f"bus 3 gain has been set to {self.vm.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vm.bus[4].eq}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    with voicemeeterlib.api(kind_id) as vm:\n        do = ManyThings(vm)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vm.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True},\n                "button-0": {"state": True},\n                "vban-in-0": {"on": True},\n                "vban-out-1": {"name": "streamname"},\n            }\n        )\n\n\nif __name__ == "__main__":\n    kind_id = "banana"\n\n    main()\n```\n\nOtherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.\n\n## `kind_id`\n\nPass the kind of Voicemeeter as an argument. kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `comp`: float, from 0.0 to 10.0\n-   `gate`: float, from 0.0 to 10.0\n-   `audibility`: float, from 0.0 to 10.0\n-   `limit`: int, from -40 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `label`: string\n-   `mc`: boolean\n-   `k`: int, from 0 to 4\n-   `bass`: float, from -12.0 to 12.0\n-   `mid`: float, from -12.0 to 12.0\n-   `treble`: float, from -12.0 to 12.0\n-   `reverb`: float, from 0.0 to 10.0\n-   `delay`: float, from 0.0 to 10.0\n-   `fx1`: float, from 0.0 to 10.0\n-   `fx2`: float, from 0.0 to 10.0\n-   `pan_x`: float, from -0.5 to 0.5\n-   `pan_y`: float, from 0.0 to 1.0\n-   `color_x`: float, from -0.5 to 0.5\n-   `color_y`: float, from 0.0 to 1.0\n-   `fx_x`: float, from -0.5 to 0.5\n-   `fx_y`: float, from 0.0 to 1.0\n-   `postreverb`: boolean\n-   `postdelay`: boolean\n-   `postfx1`: boolean\n-   `postfx2`: boolean\n\nexample:\n\n```python\nvm.strip[3].gain = 3.7\nprint(vm.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvm.strip[5].appmute("Spotify", True)\nvm.strip[5].appgain("Spotify", 0.5)\n```\n\n##### Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvm.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Levels\n\nThe following properties are available.\n\n-   `prefader`\n-   `postfader`\n-   `postmute`\n\nexample:\n\n```python\nprint(vm.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `eq`: boolean\n-   `eq_ab`: boolean\n-   `mute`: boolean\n-   `sel`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `label`: string\n-   `returnreverb`: float, from 0.0 to 10.0\n-   `returndelay`: float, from 0.0 to 10.0\n-   `returnfx1`: float, from 0.0 to 10.0\n-   `returnfx2`: float, from 0.0 to 10.0\n-   `monitor`: boolean\n\nexample:\n\n```python\nvm.bus[3].gain = 3.7\nprint(vm.bus[0].label)\n\nvm.bus[4].mono = True\n```\n\n##### Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvm.bus[4].mode.amix = True\n\nprint(vm.bus[2].mode.get())\n```\n\n##### Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vm.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvm.strip[0].fadeto(-10.3, 1000)\nvm.bus[3].fadeby(-5.6, 500)\n```\n\n#### Strip.Device | Bus.Device\n\nThe following properties are available\n\n-   `name`: str\n-   `sr`: int\n-   `wdm`: str\n-   `ks`: str\n-   `mme`: str\n-   `asio`: str\n\nexample:\n\n```python\nprint(vm.strip[0].device.name)\nvm.bus[0].device.asio = "Audient USB Audio ASIO Driver"\n```\n\nstrip|bus device parameters are defined for physical channels only.\n\nname, sr are read only. wdm, ks, mme, asio are write only.\n\n### Macrobuttons\n\nThe following properties are available.\n\n-   `state`: boolean\n-   `stateonly`: boolean\n-   `trigger`: boolean\n\nexample:\n\n```python\nvm.button[37].state = True\nvm.button[55].trigger = False\n```\n\n### Recorder\n\nThe following methods are available\n\n-   `play()`\n-   `stop()`\n-   `pause()`\n-   `record()`\n-   `ff()`\n-   `rew()`\n-   `load(<filepath>)`: string\n\nThe following properties are available\n\n-   `loop`: boolean\n-   `A1 - A5`: boolean\n-   `B1 - A3`: boolean\n\nexample:\n\n```python\nvm.recorder.play()\nvm.recorder.stop()\n\n# Enable loop play\nvm.recorder.loop = True\n\n# Disable recorder out channel B2\nvm.recorder.B2 = False\n\n# filepath as raw string\nvm.recorder.load(r\'C:\\music\\mytune.mp3\')\n```\n\nRecorder properties are defined as write only.\n\n### VBAN\n\n-   `vm.vban.enable()` `vm.vban.disable()` Turn VBAN on or off\n\n##### Instream | Outstream\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `name`: string\n-   `ip`: string\n-   `port`: int, range from 1024 to 65535\n-   `sr`: int, (11025, 16000, 22050, 24000, 32000, 44100, 48000, 64000, 88200, 96000)\n-   `channel`: int, from 1 to 8\n-   `bit`: int, 16 or 24\n-   `quality`: int, from 0 to 4\n-   `route`: int, from 0 to 8\n\n`SR`, `channel` and `bit` are defined as:\n\n-   readonly for instreams.\n-   read and write for outstreams.\n\nexample:\n\n```python\n# turn VBAN on\nvm.vban.enable()\n\n# turn on vban instream 0\nvm.vban.instream[0].on = True\n\n# set bit property for outstream 3 to 24\nvm.vban.outstream[3].bit = 24\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values.\n\nThe following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are available.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvm.command.restart()\nvm.command.showvbanchat = True\n```\n\n`showvbanchat` and `lock` are write only.\n\n### Device\n\n-   `ins` `outs` : Returns the number of input/output devices\n-   `input(i)` `output(i)` : Returns a dict of device properties for device[i]\n\nexample:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(kind_id) as vm:\n    for i in range(vm.device.ins):\n        print(vm.device.input(i))\n```\n\n### FX\n\nThe following properties are available:\n\n-   `reverb`: boolean\n-   `reverb_ab`: boolean\n-   `delay`: boolean\n-   `delay_ab`: boolean\n\nexample:\n\n```python\nvm.fx.reverb_ab = True\n```\n\n### Patch\n\nThe following properties are available:\n\n-   `postfadercomposite`: boolean\n-   `postfxinsert`: boolean\n\nexample:\n\n```python\nvm.patch.postfxinsert = False\n```\n\n##### asio[i]\n\n-   `get()`: int\n-   `set(patch_in)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.asio[3].set(4)\n```\n\ni, from 0 to 10\n\n##### A2[i] - A5[i]\n\n-   `get()`: int\n-   `set(patch_out)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.A3[5].set(3)\n```\n\ni, from 0 to 8.\n\n##### composite[i]\n\n-   `get()`: int\n-   `set(channel)`: int, from 0 up to number of channels depending on version.\n\nexample:\n\n```python\nvm.patch.composite[7].set(4)\n```\n\ni, from 0 to 8.\n\n##### insert[i]\n\n-   `on`: boolean\n\nexample:\n\n```python\nvm.patch.insert[18].on = True\n```\n\ni, from 0 up to number of channels depending on version.\n\n### Option\n\nThe following properties are available:\n\n-   `sr`: int\n-   `asiosr`: boolean\n-   `monitoronsel`: boolean\n\nexample:\n\n```python\nvm.option.sr = 48000\n```\n\nThe following methods are available:\n\n-   `buffer(driver, buffer)` : Set buffer size for particular audio driver.\n\nexample:\n\n```python\nvm.option.buffer("wdm", 512)\n```\n\ndriver defined as one of ("mme", "wdm", "ks", "asio")\n\nbuffer, from 128 to 2048\n\n##### delay[i]\n\n-   `get()`: int\n-   `set(delay)`: int, from 0 to 500\n\nexample:\n\n```python\nvm.option.delay[4].set(30)\n```\n\ni, from 0 up to 4.\n\n### Midi\n\nThe following properties are available:\n\n-   `channel`: int, returns the midi channel\n-   `current`: int, returns the current (or most recently pressed) key\n\nThe following methods are available:\n\n-   `get(key)`: int, returns most recent velocity value for a key\n\nexample:\n\n```python\nprint(vm.midi.get(12))\n```\n\nget() may return None if no value for requested key in midi cache\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus/macrobutton/vban parameters at once, for example:\n\n```python\nvm.apply(\n    {\n        "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-2": {"mute": True},\n        "button-0": {"state": True},\n        "vban-in-0": {"on": True},\n        "vban-out-1": {"name": "streamname"},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvm.strip[0].apply(mute: True, gain: 3.2, A1: True)\nvm.vban.outstream[0].apply(on: True, name: \'streamname\', bit: 24)\n```\n\n## Config Files\n\n`vm.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(\'banana\') as vm:\n    vm.apply_config(\'example\')\n```\n\nwill load a user config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nLevel updates are considered high volume, by default they are NOT listened for. Use subs keyword arg to initialize event updates.\n\nexample:\n\n```python\nimport voicemeeterlib\n# Set updates to occur every 50ms\n# Listen for level updates but disable midi updates\nwith voicemeeterlib.api(\'banana\', ratelimit=0.05, subs={"ldirty": True, "midi": False}) as vm:\n    ...\n```\n\n#### `vm.subject`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vm):\n        vm.subject.add(self)\n        ...\n```\n\n#### `vm.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `mdirty`: boolean\n-   `midi`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvm.event.ldirty = True\n\nvm.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvm.event.remove(["pdirty", "mdirty", "midi"])\n\n# get a list of currently subscribed\nprint(vm.event.get())\n```\n\n## Remote class\n\n`voicemeeterlib.api(kind_id: str)`\n\nYou may pass the following optional keyword arguments:\n\n-   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.\n-   `ratelimit`: float=0.033, how often to check for updates in ms.\n-   `subs`: dict={"pdirty": True, "mdirty": True, "midi": True, "ldirty": False}, initialize which event updates to listen for.\n    -   `pdirty`: parameter updates\n    -   `mdirty`: macrobutton updates\n    -   `midi`: midi updates\n    -   `ldirty`: level updates\n\nAccess to lower level Getters and Setters are provided with these functions:\n\n-   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.\n-   `vm.set(param, value)`: For setting the value of any parameter.\n\nAccess to lower level polling functions are provided with these functions:\n\n-   `vm.pdirty()`: Returns True if a parameter has been updated.\n-   `vm.mdirty()`: Returns True if a macrobutton has been updated.\n-   `vm.ldirty()`: Returns True if a level has been updated.\n\nexample:\n\n```python\nvm.get(\'Strip[2].Mute\')\nvm.set(\'Strip[4].Label\', \'stripname\')\nvm.set(\'Strip[0].Gain\', -3.6)\n```\n\n### Run tests\n\nTo run all tests:\n\n```\npytest -v\n```\n\n### Official Documentation\n\n-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/main/VoicemeeterRemoteAPI.pdf)\n',
+    'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-api.svg)](https://badge.fury.io/py/voicemeeter-api)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-api-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# Python Wrapper for Voicemeeter API\n\nThis package offers a Python interface for the Voicemeeter Remote C API.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.4\n-   Banana 2.0.6.4\n-   Potato 3.0.2.4\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install voicemeeter-api`\n\n## `Use`\n\nSimplest use case, use a context manager to request a Remote class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n#### `__main__.py`\n\n```python\nimport voicemeeterlib\n\n\nclass ManyThings:\n    def __init__(self, vm):\n        self.vm = vm\n\n    def things(self):\n        self.vm.strip[0].label = "podmic"\n        self.vm.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vm.bus[3].gain = -6.3\n        self.vm.bus[4].eq.on = True\n        info = (\n            f"bus 3 gain has been set to {self.vm.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vm.bus[4].eq.on}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    KIND_ID = "banana"\n\n    with voicemeeterlib.api(KIND_ID) as vm:\n        do = ManyThings(vm)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vm.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True, "eq": {"on": True}},\n                "button-0": {"state": True},\n                "vban-in-0": {"on": True},\n                "vban-out-1": {"name": "streamname"},\n            }\n        )\n\n\nif __name__ == "__main__":\n    main()\n\n```\n\nOtherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.\n\n## `KIND_ID`\n\nPass the kind of Voicemeeter as an argument. KIND_ID may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `audibility`: float, from 0.0 to 10.0\n-   `limit`: int, from -40 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `label`: string\n-   `mc`: boolean\n-   `k`: int, from 0 to 4\n-   `bass`: float, from -12.0 to 12.0\n-   `mid`: float, from -12.0 to 12.0\n-   `treble`: float, from -12.0 to 12.0\n-   `reverb`: float, from 0.0 to 10.0\n-   `delay`: float, from 0.0 to 10.0\n-   `fx1`: float, from 0.0 to 10.0\n-   `fx2`: float, from 0.0 to 10.0\n-   `pan_x`: float, from -0.5 to 0.5\n-   `pan_y`: float, from 0.0 to 1.0\n-   `color_x`: float, from -0.5 to 0.5\n-   `color_y`: float, from 0.0 to 1.0\n-   `fx_x`: float, from -0.5 to 0.5\n-   `fx_y`: float, from 0.0 to 1.0\n-   `postreverb`: boolean\n-   `postdelay`: boolean\n-   `postfx1`: boolean\n-   `postfx2`: boolean\n\nexample:\n\n```python\nvm.strip[3].gain = 3.7\nprint(vm.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvm.strip[5].appmute("Spotify", True)\nvm.strip[5].appgain("Spotify", 0.5)\n```\n\n#### Strip.Comp\n\n-   `knob`: float, from 0.0 to 10.0\n-   `gainin`: float, from -24.0 to 24.0\n-   `ratio`: float, from 1.0 to 8.0\n-   `threshold`: float, from -40.0 to -3.0\n-   `attack`: float, from 0.0 to 200.0\n-   `release`: float, from 0.0 to 5000.0\n-   `knee`: float, from 0.0 to 1.0\n-   `gainout`: float, from -24.0 to 24.0\n-   `makeup`: boolean\n\nexample:\n\n```python\nprint(vm.strip[4].comp.knob)\n```\n\nStrip Comp parameters are defined for PhysicalStrips, potato version only.\n\n#### Strip.Gate\n\n-   `knob`: float, from 0.0 to 10.0\n-   `threshold`: float, from -60.0 to -10.0\n-   `damping`: float, from -60.0 to -10.0\n-   `bpsidechain`: int, from 100 to 4000\n-   `attack`: float, from 0.0 to 1000.0\n-   `hold`: float, from 0.0 to 5000.0\n-   `release`: float, from 0.0 to 5000.0\n\nexample:\n\n```python\nvm.strip[2].gate.attack = 300.8\n```\n\nStrip Gate parameters are defined for PhysicalStrips, potato version only.\n\n#### Strip.Denoiser\n\n-   `knob`: float, from 0.0 to 10.0\n\nexample:\n\n```python\nvm.strip[0].denoiser.knob = 0.5\n```\n\nStrip Denoiser parameters are defined for PhysicalStrips, potato version only.\n\n#### Strip.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\nexample:\n\n```python\nvm.strip[0].eq.ab = True\n```\n\nStrip EQ parameters are defined for PhysicalStrips, potato version only.\n\n##### Strip.Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvm.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Strip.Levels\n\nThe following properties are available.\n\n-   `prefader`\n-   `postfader`\n-   `postmute`\n\nexample:\n\n```python\nprint(vm.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `mute`: boolean\n-   `sel`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `label`: string\n-   `returnreverb`: float, from 0.0 to 10.0\n-   `returndelay`: float, from 0.0 to 10.0\n-   `returnfx1`: float, from 0.0 to 10.0\n-   `returnfx2`: float, from 0.0 to 10.0\n-   `monitor`: boolean\n\nexample:\n\n```python\nvm.bus[3].gain = 3.7\nprint(vm.bus[0].label)\n\nvm.bus[4].mono = True\n```\n\n##### Bus.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\nexample:\n\n```python\nvm.bus[3].eq.on = True\n```\n\n##### Bus.Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvm.bus[4].mode.amix = True\n\nprint(vm.bus[2].mode.get())\n```\n\n##### Bus.Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vm.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvm.strip[0].fadeto(-10.3, 1000)\nvm.bus[3].fadeby(-5.6, 500)\n```\n\n#### Strip.Device | Bus.Device\n\nThe following properties are available\n\n-   `name`: str\n-   `sr`: int\n-   `wdm`: str\n-   `ks`: str\n-   `mme`: str\n-   `asio`: str\n\nexample:\n\n```python\nprint(vm.strip[0].device.name)\nvm.bus[0].device.asio = "Audient USB Audio ASIO Driver"\n```\n\nstrip|bus device parameters are defined for physical channels only.\n\nname, sr are read only. wdm, ks, mme, asio are write only.\n\n### Macrobuttons\n\nThe following properties are available.\n\n-   `state`: boolean\n-   `stateonly`: boolean\n-   `trigger`: boolean\n\nexample:\n\n```python\nvm.button[37].state = True\nvm.button[55].trigger = False\n```\n\n### Recorder\n\nThe following methods are available\n\n-   `play()`\n-   `stop()`\n-   `pause()`\n-   `record()`\n-   `ff()`\n-   `rew()`\n-   `load(<filepath>)`: string\n\nThe following properties are available\n\n-   `loop`: boolean\n-   `A1 - A5`: boolean\n-   `B1 - A3`: boolean\n\nexample:\n\n```python\nvm.recorder.play()\nvm.recorder.stop()\n\n# Enable loop play\nvm.recorder.loop = True\n\n# Disable recorder out channel B2\nvm.recorder.B2 = False\n\n# filepath as raw string\nvm.recorder.load(r\'C:\\music\\mytune.mp3\')\n```\n\nRecorder properties are defined as write only.\n\n### VBAN\n\n-   `vm.vban.enable()` `vm.vban.disable()` Turn VBAN on or off\n\n##### Instream | Outstream\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `name`: string\n-   `ip`: string\n-   `port`: int, range from 1024 to 65535\n-   `sr`: int, (11025, 16000, 22050, 24000, 32000, 44100, 48000, 64000, 88200, 96000)\n-   `channel`: int, from 1 to 8\n-   `bit`: int, 16 or 24\n-   `quality`: int, from 0 to 4\n-   `route`: int, from 0 to 8\n\n`SR`, `channel` and `bit` are defined as:\n\n-   readonly for instreams.\n-   read and write for outstreams.\n\nexample:\n\n```python\n# turn VBAN on\nvm.vban.enable()\n\n# turn on vban instream 0\nvm.vban.instream[0].on = True\n\n# set bit property for outstream 3 to 24\nvm.vban.outstream[3].bit = 24\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values.\n\nThe following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are available.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvm.command.restart()\nvm.command.showvbanchat = True\n```\n\n`showvbanchat` and `lock` are write only.\n\n### Device\n\n-   `ins` `outs` : Returns the number of input/output devices\n-   `input(i)` `output(i)` : Returns a dict of device properties for device[i]\n\nexample:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(KIND_ID) as vm:\n    for i in range(vm.device.ins):\n        print(vm.device.input(i))\n```\n\n### FX\n\nThe following properties are available:\n\n-   `reverb`: boolean\n-   `reverb_ab`: boolean\n-   `delay`: boolean\n-   `delay_ab`: boolean\n\nexample:\n\n```python\nvm.fx.reverb_ab = True\n```\n\n### Patch\n\nThe following properties are available:\n\n-   `postfadercomposite`: boolean\n-   `postfxinsert`: boolean\n\nexample:\n\n```python\nvm.patch.postfxinsert = False\n```\n\n##### asio[i]\n\n-   `get()`: int\n-   `set(patch_in)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.asio[3].set(4)\n```\n\ni, from 0 to 10\n\n##### A2[i] - A5[i]\n\n-   `get()`: int\n-   `set(patch_out)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.A3[5].set(3)\n```\n\ni, from 0 to 8.\n\n##### composite[i]\n\n-   `get()`: int\n-   `set(channel)`: int, from 0 up to number of channels depending on version.\n\nexample:\n\n```python\nvm.patch.composite[7].set(4)\n```\n\ni, from 0 to 8.\n\n##### insert[i]\n\n-   `on`: boolean\n\nexample:\n\n```python\nvm.patch.insert[18].on = True\n```\n\ni, from 0 up to number of channels depending on version.\n\n### Option\n\nThe following properties are available:\n\n-   `sr`: int\n-   `asiosr`: boolean\n-   `monitoronsel`: boolean\n\nexample:\n\n```python\nvm.option.sr = 48000\n```\n\nThe following methods are available:\n\n-   `buffer(driver, buffer)` : Set buffer size for particular audio driver.\n\nexample:\n\n```python\nvm.option.buffer("wdm", 512)\n```\n\ndriver defined as one of ("mme", "wdm", "ks", "asio")\n\nbuffer, from 128 to 2048\n\n##### delay[i]\n\n-   `get()`: int\n-   `set(delay)`: int, from 0 to 500\n\nexample:\n\n```python\nvm.option.delay[4].set(30)\n```\n\ni, from 0 up to 4.\n\n### Midi\n\nThe following properties are available:\n\n-   `channel`: int, returns the midi channel\n-   `current`: int, returns the current (or most recently pressed) key\n\nThe following methods are available:\n\n-   `get(key)`: int, returns most recent velocity value for a key\n\nexample:\n\n```python\nprint(vm.midi.get(12))\n```\n\nget() may return None if no value for requested key in midi cache\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus/macrobutton/vban parameters at once, for example:\n\n```python\nvm.apply(\n    {\n        "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-2": {"mute": True, "eq": {"on": True}},\n        "button-0": {"state": True},\n        "vban-in-0": {"on": True},\n        "vban-out-1": {"name": "streamname"},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvm.strip[0].apply(mute: True, gain: 3.2, A1: True)\nvm.vban.outstream[0].apply(on: True, name: \'streamname\', bit: 24)\n```\n\n## Config Files\n\n`vm.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(\'banana\') as vm:\n    vm.apply_config(\'example\')\n```\n\nwill load a user config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nBy default, NO events are listened for. Use events kwargs to enable specific event types.\n\nexample:\n\n```python\nimport voicemeeterlib\n# Set event updates to occur every 50ms\n# Listen for level updates only\nwith voicemeeterlib.api(\'banana\', ratelimit=0.05, ldirty=True}) as vm:\n    ...\n```\n\n#### `vm.observer`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vm):\n        vm.observer.add(self)\n        ...\n```\n\n#### `vm.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `mdirty`: boolean\n-   `midi`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvm.event.ldirty = True\n\nvm.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvm.event.remove(["pdirty", "mdirty", "midi"])\n\n# get a list of currently subscribed\nprint(vm.event.get())\n```\n\n## Remote class\n\n`voicemeeterlib.api(KIND_ID: str)`\n\nYou may pass the following optional keyword arguments:\n\n-   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.\n-   `ratelimit`: float=0.033, how often to check for updates in ms.\n-   `pdirty`: boolean=False, parameter updates\n-   `mdirty`: boolean=False, macrobutton updates\n-   `midi`: boolean=False, midi updates\n-   `ldirty`: boolean=False, level updates\n\nAccess to lower level Getters and Setters are provided with these functions:\n\n-   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.\n-   `vm.set(param, value)`: For setting the value of any parameter.\n\nAccess to lower level polling functions are provided with these functions:\n\n-   `vm.pdirty()`: Returns True if a parameter has been updated.\n-   `vm.mdirty()`: Returns True if a macrobutton has been updated.\n-   `vm.ldirty()`: Returns True if a level has been updated.\n\nexample:\n\n```python\nvm.get(\'Strip[2].Mute\')\nvm.set(\'Strip[4].Label\', \'stripname\')\nvm.set(\'Strip[0].Gain\', -3.6)\n```\n\n### Run tests\n\nTo run all tests:\n\n```\npytest -v\n```\n\n### Official Documentation\n\n-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/voicemeeter-api-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `voicemeeter-api-1.0.0/PKG-INFO` & `voicemeeter-api-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 1.0.0
+Version: 2.0.0
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -64,51 +64,52 @@
         self.vm.strip[0].mute = True
         print(
             f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"
         )
 
     def other_things(self):
         self.vm.bus[3].gain = -6.3
-        self.vm.bus[4].eq = True
+        self.vm.bus[4].eq.on = True
         info = (
             f"bus 3 gain has been set to {self.vm.bus[3].gain}",
-            f"bus 4 eq has been set to {self.vm.bus[4].eq}",
+            f"bus 4 eq has been set to {self.vm.bus[4].eq.on}",
         )
         print("\n".join(info))
 
 
 def main():
-    with voicemeeterlib.api(kind_id) as vm:
+    KIND_ID = "banana"
+
+    with voicemeeterlib.api(KIND_ID) as vm:
         do = ManyThings(vm)
         do.things()
         do.other_things()
 
         # set many parameters at once
         vm.apply(
             {
                 "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-                "bus-2": {"mute": True},
+                "bus-2": {"mute": True, "eq": {"on": True}},
                 "button-0": {"state": True},
                 "vban-in-0": {"on": True},
                 "vban-out-1": {"name": "streamname"},
             }
         )
 
 
 if __name__ == "__main__":
-    kind_id = "banana"
-
     main()
+
 ```
 
 Otherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.
 
-## `kind_id`
+## `KIND_ID`
 
-Pass the kind of Voicemeeter as an argument. kind_id may be:
+Pass the kind of Voicemeeter as an argument. KIND_ID may be:
 
 -   `basic`
 -   `banana`
 -   `potato`
 
 ## `Available commands`
 
@@ -116,16 +117,14 @@
 
 The following properties are available.
 
 -   `mono`: boolean
 -   `solo`: boolean
 -   `mute`: boolean
 -   `gain`: float, from -60.0 to 12.0
--   `comp`: float, from 0.0 to 10.0
--   `gate`: float, from 0.0 to 10.0
 -   `audibility`: float, from 0.0 to 10.0
 -   `limit`: int, from -40 to 12
 -   `A1 - A5`, `B1 - B3`: boolean
 -   `label`: string
 -   `mc`: boolean
 -   `k`: int, from 0 to 4
 -   `bass`: float, from -12.0 to 12.0
@@ -166,27 +165,92 @@
 example:
 
 ```python
 vm.strip[5].appmute("Spotify", True)
 vm.strip[5].appgain("Spotify", 0.5)
 ```
 
-##### Gainlayers
+#### Strip.Comp
+
+-   `knob`: float, from 0.0 to 10.0
+-   `gainin`: float, from -24.0 to 24.0
+-   `ratio`: float, from 1.0 to 8.0
+-   `threshold`: float, from -40.0 to -3.0
+-   `attack`: float, from 0.0 to 200.0
+-   `release`: float, from 0.0 to 5000.0
+-   `knee`: float, from 0.0 to 1.0
+-   `gainout`: float, from -24.0 to 24.0
+-   `makeup`: boolean
+
+example:
+
+```python
+print(vm.strip[4].comp.knob)
+```
+
+Strip Comp parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.Gate
+
+-   `knob`: float, from 0.0 to 10.0
+-   `threshold`: float, from -60.0 to -10.0
+-   `damping`: float, from -60.0 to -10.0
+-   `bpsidechain`: int, from 100 to 4000
+-   `attack`: float, from 0.0 to 1000.0
+-   `hold`: float, from 0.0 to 5000.0
+-   `release`: float, from 0.0 to 5000.0
+
+example:
+
+```python
+vm.strip[2].gate.attack = 300.8
+```
+
+Strip Gate parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.Denoiser
+
+-   `knob`: float, from 0.0 to 10.0
+
+example:
+
+```python
+vm.strip[0].denoiser.knob = 0.5
+```
+
+Strip Denoiser parameters are defined for PhysicalStrips, potato version only.
+
+#### Strip.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+example:
+
+```python
+vm.strip[0].eq.ab = True
+```
+
+Strip EQ parameters are defined for PhysicalStrips, potato version only.
+
+##### Strip.Gainlayers
 
 -   `gain`: float, from -60.0 to 12.0
 
 example:
 
 ```python
 vm.strip[3].gainlayer[3].gain = 3.7
 ```
 
 Gainlayers are defined for potato version only.
 
-##### Levels
+##### Strip.Levels
 
 The following properties are available.
 
 -   `prefader`
 -   `postfader`
 -   `postmute`
 
@@ -199,16 +263,14 @@
 Level properties will return -200.0 if no audio detected.
 
 ### Bus
 
 The following properties are available.
 
 -   `mono`: boolean
--   `eq`: boolean
--   `eq_ab`: boolean
 -   `mute`: boolean
 -   `sel`: boolean
 -   `gain`: float, from -60.0 to 12.0
 -   `label`: string
 -   `returnreverb`: float, from 0.0 to 10.0
 -   `returndelay`: float, from 0.0 to 10.0
 -   `returnfx1`: float, from 0.0 to 10.0
@@ -220,15 +282,28 @@
 ```python
 vm.bus[3].gain = 3.7
 print(vm.bus[0].label)
 
 vm.bus[4].mono = True
 ```
 
-##### Modes
+##### Bus.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+example:
+
+```python
+vm.bus[3].eq.on = True
+```
+
+##### Bus.Modes
 
 The following properties are available.
 
 -   `normal`: boolean
 -   `amix`: boolean
 -   `bmix`: boolean
 -   `composite`: boolean
@@ -248,15 +323,15 @@
 
 ```python
 vm.bus[4].mode.amix = True
 
 print(vm.bus[2].mode.get())
 ```
 
-##### Levels
+##### Bus.Levels
 
 The following properties are available.
 
 -   `all`
 
 example:
 
@@ -421,15 +496,15 @@
 -   `ins` `outs` : Returns the number of input/output devices
 -   `input(i)` `output(i)` : Returns a dict of device properties for device[i]
 
 example:
 
 ```python
 import voicemeeterlib
-with voicemeeterlib.api(kind_id) as vm:
+with voicemeeterlib.api(KIND_ID) as vm:
     for i in range(vm.device.ins):
         print(vm.device.input(i))
 ```
 
 ### FX
 
 The following properties are available:
@@ -574,15 +649,15 @@
 -   `apply`
     Set many strip/bus/macrobutton/vban parameters at once, for example:
 
 ```python
 vm.apply(
     {
         "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-        "bus-2": {"mute": True},
+        "bus-2": {"mute": True, "eq": {"on": True}},
         "button-0": {"state": True},
         "vban-in-0": {"on": True},
         "vban-out-1": {"name": "streamname"},
     }
 )
 ```
 
@@ -607,42 +682,42 @@
     vm.apply_config('example')
 ```
 
 will load a user config file at configs/banana/example.toml for Voicemeeter Banana.
 
 ## Events
 
-Level updates are considered high volume, by default they are NOT listened for. Use subs keyword arg to initialize event updates.
+By default, NO events are listened for. Use events kwargs to enable specific event types.
 
 example:
 
 ```python
 import voicemeeterlib
-# Set updates to occur every 50ms
-# Listen for level updates but disable midi updates
-with voicemeeterlib.api('banana', ratelimit=0.05, subs={"ldirty": True, "midi": False}) as vm:
+# Set event updates to occur every 50ms
+# Listen for level updates only
+with voicemeeterlib.api('banana', ratelimit=0.05, ldirty=True}) as vm:
     ...
 ```
 
-#### `vm.subject`
+#### `vm.observer`
 
 Use the Subject class to register an app as event observer.
 
 The following methods are available:
 
 -   `add`: registers an app as an event observer
 -   `remove`: deregisters an app as an event observer
 
 example:
 
 ```python
 # register an app to receive updates
 class App():
     def __init__(self, vm):
-        vm.subject.add(self)
+        vm.observer.add(self)
         ...
 ```
 
 #### `vm.event`
 
 Use the event class to toggle updates as necessary.
 
@@ -676,25 +751,24 @@
 
 # get a list of currently subscribed
 print(vm.event.get())
 ```
 
 ## Remote class
 
-`voicemeeterlib.api(kind_id: str)`
+`voicemeeterlib.api(KIND_ID: str)`
 
 You may pass the following optional keyword arguments:
 
 -   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.
 -   `ratelimit`: float=0.033, how often to check for updates in ms.
--   `subs`: dict={"pdirty": True, "mdirty": True, "midi": True, "ldirty": False}, initialize which event updates to listen for.
-    -   `pdirty`: parameter updates
-    -   `mdirty`: macrobutton updates
-    -   `midi`: midi updates
-    -   `ldirty`: level updates
+-   `pdirty`: boolean=False, parameter updates
+-   `mdirty`: boolean=False, macrobutton updates
+-   `midi`: boolean=False, midi updates
+-   `ldirty`: boolean=False, level updates
 
 Access to lower level Getters and Setters are provided with these functions:
 
 -   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.
 -   `vm.set(param, value)`: For setting the value of any parameter.
 
 Access to lower level polling functions are provided with these functions:
@@ -717,9 +791,9 @@
 
 ```
 pytest -v
 ```
 
 ### Official Documentation
 
--   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/main/VoicemeeterRemoteAPI.pdf)
+-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/update-docs/VoicemeeterRemoteAPI.pdf)
```

