# Comparing `tmp/vban-cmd-1.8.1.tar.gz` & `tmp/vban-cmd-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban-cmd-1.8.1.tar", max compression
+gzip compressed data, was "vban-cmd-2.0.0.tar", max compression
```

## Comparing `vban-cmd-1.8.1.tar` & `vban-cmd-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban-cmd-1.8.1/LICENSE
--rw-r--r--   0        0        0      630 2022-10-19 13:32:40.225756 vban-cmd-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     9842 2022-10-18 18:22:21.482759 vban-cmd-1.8.1/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban-cmd-1.8.1/vban_cmd/__init__.py
--rw-r--r--   0        0        0     4913 2022-10-06 17:44:33.004589 vban-cmd-1.8.1/vban_cmd/bus.py
--rw-r--r--   0        0        0     1154 2022-09-24 06:36:12.324473 vban-cmd-1.8.1/vban_cmd/command.py
--rw-r--r--   0        0        0     5547 2022-09-28 16:11:23.308349 vban-cmd-1.8.1/vban_cmd/config.py
--rw-r--r--   0        0        0       70 2022-09-24 06:34:57.996729 vban-cmd-1.8.1/vban_cmd/error.py
--rw-r--r--   0        0        0     1566 2022-10-06 16:44:37.408995 vban-cmd-1.8.1/vban_cmd/event.py
--rw-r--r--   0        0        0     5863 2022-10-07 16:59:11.880300 vban-cmd-1.8.1/vban_cmd/factory.py
--rw-r--r--   0        0        0     3454 2022-10-18 18:19:40.713818 vban-cmd-1.8.1/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2124 2022-07-12 16:30:51.965399 vban-cmd-1.8.1/vban_cmd/kinds.py
--rw-r--r--   0        0        0     3009 2022-09-24 06:36:16.268859 vban-cmd-1.8.1/vban_cmd/meta.py
--rw-r--r--   0        0        0     9011 2022-10-04 14:31:27.264624 vban-cmd-1.8.1/vban_cmd/packet.py
--rw-r--r--   0        0        0     6545 2022-10-06 17:39:53.904261 vban-cmd-1.8.1/vban_cmd/strip.py
--rw-r--r--   0        0        0     1443 2022-09-28 15:52:46.390068 vban-cmd-1.8.1/vban_cmd/subject.py
--rw-r--r--   0        0        0     2060 2022-10-18 17:24:11.660337 vban-cmd-1.8.1/vban_cmd/util.py
--rw-r--r--   0        0        0     5500 2022-10-19 13:32:25.366689 vban-cmd-1.8.1/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     5822 2022-10-18 20:09:00.698228 vban-cmd-1.8.1/vban_cmd/worker.py
--rw-r--r--   0        0        0    10569 2022-10-19 13:33:09.889405 vban-cmd-1.8.1/setup.py
--rw-r--r--   0        0        0    10019 2022-10-19 13:33:09.890374 vban-cmd-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban-cmd-2.0.0/LICENSE
+-rw-r--r--   0        0        0      951 2023-06-25 12:12:54.738275 vban-cmd-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11211 2023-06-25 17:44:51.494900 vban-cmd-2.0.0/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban-cmd-2.0.0/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban-cmd-2.0.0/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban-cmd-2.0.0/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-06-25 10:36:21.413563 vban-cmd-2.0.0/vban_cmd/config.py
+-rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban-cmd-2.0.0/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban-cmd-2.0.0/vban_cmd/event.py
+-rw-r--r--   0        0        0     6101 2023-06-25 02:42:35.162285 vban-cmd-2.0.0/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4168 2023-06-24 12:48:05.367943 vban-cmd-2.0.0/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2184 2023-06-22 02:29:18.843450 vban-cmd-2.0.0/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban-cmd-2.0.0/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9644 2023-06-25 14:59:01.896621 vban-cmd-2.0.0/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban-cmd-2.0.0/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban-cmd-2.0.0/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2060 2023-06-25 10:36:42.302165 vban-cmd-2.0.0/vban_cmd/util.py
+-rw-r--r--   0        0        0     6680 2023-06-25 10:52:32.659395 vban-cmd-2.0.0/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6905 2023-06-25 14:54:55.684238 vban-cmd-2.0.0/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12178 2023-06-25 20:58:40.663927 vban-cmd-2.0.0/setup.py
+-rw-r--r--   0        0        0    11322 2023-06-25 20:58:40.664927 vban-cmd-2.0.0/PKG-INFO
```

### Comparing `vban-cmd-1.8.1/LICENSE` & `vban-cmd-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vban-cmd-1.8.1/README.md` & `vban-cmd-2.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 There is no support for audio transfer in this package, only parameters.
 
 For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
 
 ## Tested against
 
--   Basic 1.0.8.4
--   Banana 2.0.6.4
--   Potato 3.0.2.4
+-   Basic 1.0.8.8
+-   Banana 2.0.6.8
+-   Potato 3.0.2.8
 
 ## Requirements
 
 -   [Voicemeeter](https://voicemeeter.com/)
 -   Python 3.10 or greater
 
 ## Installation
@@ -67,48 +67,50 @@
         self.vban.strip[0].mute = True
         print(
             f"strip 0 ({self.vban.strip[0].label}) mute has been set to {self.vban.strip[0].mute}"
         )
 
     def other_things(self):
         self.vban.bus[3].gain = -6.3
-        self.vban.bus[4].eq = True
+        self.vban.bus[4].eq.on = True
         info = (
             f"bus 3 gain has been set to {self.vban.bus[3].gain}",
-            f"bus 4 eq has been set to {self.vban.bus[4].eq}",
+            f"bus 4 eq has been set to {self.vban.bus[4].eq.on}",
         )
         print("\n".join(info))
 
 
 def main():
-    with vban_cmd.api(kind_id, ip="gamepc.local", port=6980, streamname="Command1") as vban:
+    KIND_ID = "banana"
+
+    with vban_cmd.api(
+        KIND_ID, ip="gamepc.local", port=6980, streamname="Command1"
+    ) as vban:
         do = ManyThings(vban)
         do.things()
         do.other_things()
 
         # set many parameters at once
         vban.apply(
             {
                 "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-                "bus-2": {"mute": True},
+                "bus-2": {"mute": True, "eq": {"on": True}},
             }
         )
 
 
 if __name__ == "__main__":
-    kind_id = "banana"
-
     main()
 ```
 
 Otherwise you must remember to call `vban.login()`, `vban.logout()` at the start/end of your code.
 
-## `kind_id`
+## `KIND_ID`
 
-Pass the kind of Voicemeeter as an argument. kind_id may be:
+Pass the kind of Voicemeeter as an argument. KIND_ID may be:
 
 -   `basic`
 -   `banana`
 -   `potato`
 
 ## `Available commands`
 
@@ -118,16 +120,14 @@
 
 -   `mono`: boolean
 -   `solo`: boolean
 -   `mute`: boolean
 -   `label`: string
 -   `gain`: float, -60 to 12
 -   `A1 - A5`, `B1 - B3`: boolean
--   `comp`: float, from 0.0 to 10.0
--   `gate`: float, from 0.0 to 10.0
 -   `limit`: int, from -40 to 12
 
 example:
 
 ```python
 vban.strip[3].gain = 3.7
 print(vban.strip[0].label)
@@ -146,14 +146,77 @@
 example:
 
 ```python
 vban.strip[5].appmute("Spotify", True)
 vban.strip[5].appgain("Spotify", 0.5)
 ```
 
+##### Strip.Comp
+
+The following properties are available.
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
+Strip Comp properties are defined as write only.
+
+`knob` defined for all versions, all other parameters potato only.
+
+##### Strip.Gate
+
+The following properties are available.
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
+Strip Gate properties are defined as write only, potato version only.
+
+`knob` defined for all versions, all other parameters potato only.
+
+##### Strip.Denoiser
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+
+strip.denoiser properties are defined as write only, potato version only.
+
+##### Strip.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+Strip EQ properties are defined as write only, potato version only.
+
 ##### Gainlayers
 
 -   `gain`: float, from -60.0 to 12.0
 
 example:
 
 ```python
@@ -177,27 +240,32 @@
 Level properties will return -200.0 if no audio detected.
 
 ### Bus
 
 The following properties are available.
 
 -   `mono`: boolean
--   `eq`: boolean
--   `eq_ab`: boolean
 -   `mute`: boolean
 -   `label`: string
 -   `gain`: float, -60 to 12
 
 example:
 
 ```python
 vban.bus[4].eq = true
 print(vban.bus[0].label)
 ```
 
+##### Bus.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
 ##### Modes
 
 The following properties are available.
 
 -   `normal`: boolean
 -   `amix`: boolean
 -   `bmix`: boolean
@@ -277,25 +345,25 @@
 
 -   `apply`
     Set many strip/bus parameters at once, for example:
 
 ```python
 vban.apply(
     {
-        "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-        "bus-2": {"mute": True},
+        "strip-0": {"A1": True, "B1": True, "gain": -6.0},
+        "bus-1": {"mute": True, "mode": "composite"},
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
 vban.strip[0].apply(mute: true, gain: 3.2, A1: true)
-vban.vban.outstream[0].apply(on: true, name: 'streamname', bit: 24)
+vban.bus[0].apply(A1: true)
 ```
 
 ## Config Files
 
 `vban.apply_config(<configname>)`
 
 You may load config files in TOML format.
@@ -319,17 +387,16 @@
 ```python
 import vban_cmd
 # Listen for level updates
 opts = {
     "ip": "<ip address>",
     "streamname": "Command1",
     "port": 6980,
-    "subs": {"ldirty": True},
 }
-with vban_cmd.api('banana', **opts) as vban:
+with vban_cmd.api('banana', ldirty=True, **opts) as vban:
     ...
 ```
 
 #### `vban.subject`
 
 Use the Subject class to register an app as event observer.
 
@@ -380,24 +447,23 @@
 
 # get a list of currently subscribed
 print(vban.event.get())
 ```
 
 ## VbanCmd class
 
-`vban_cmd.api(kind_id: str, **opts: dict)`
+`vban_cmd.api(kind_id: str, **opts)`
 
 You may pass the following optional keyword arguments:
 
 -   `ip`: str, ip or hostname of remote machine
 -   `streamname`: str, name of the stream to connect to.
 -   `port`: int=6980, vban udp port of remote machine.
--   `subs`: dict={"pdirty": True, "ldirty": False}, controls which updates to listen for.
-    -   `pdirty`: parameter updates
-    -   `ldirty`: level updates
+-   `pdirty`: parameter updates
+-   `ldirty`: level updates
 
 #### `vban.pdirty`
 
 True iff a parameter has been changed.
 
 #### `vban.ldirty`
 
@@ -409,15 +475,15 @@
 
 ```python
 vban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")
 ```
 
 #### `vban.public_packet`
 
-Returns a Voicemeeter rt data packet object. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).
+Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).
 
 ### `Errors`
 
 -   `errors.VBANCMDError`: Base VMCMD error class.
 
 ### `Tests`
```

### Comparing `vban-cmd-1.8.1/vban_cmd/bus.py` & `vban-cmd-2.0.0/vban_cmd/bus.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,31 @@
         time.sleep(self._remote.DELAY)
 
     def fadeby(self, change: float, time_: int):
         self.setter("FadeBy", f"({change}, {time_})")
         time.sleep(self._remote.DELAY)
 
 
+class BusEQ(IRemote):
+    @classmethod
+    def make(cls, remote, index):
+        BUSEQ_cls = type(
+            f"BusEQ{remote.kind}",
+            (cls,),
+            {
+                **{param: channel_bool_prop(param) for param in ["on", "ab"]},
+            },
+        )
+        return BUSEQ_cls(remote, index)
+
+    @property
+    def identifier(self) -> str:
+        return f"Bus[{self.index}].eq"
+
+
 class PhysicalBus(Bus):
     def __str__(self):
         return f"{type(self).__name__}{self.index}"
 
     @property
     def device(self) -> str:
         return
@@ -163,19 +180,18 @@
     """
     BUS_cls = PhysicalBus if phys_bus else VirtualBus
     BUSMODEMIXIN_cls = _make_bus_mode_mixin()
     return type(
         f"{BUS_cls.__name__}{remote.kind}",
         (BUS_cls,),
         {
+            "eq": BusEQ.make(remote, i),
             "levels": BusLevel(remote, i),
             "mode": BUSMODEMIXIN_cls(remote, i),
             **{param: channel_bool_prop(param) for param in ["mute", "mono"]},
-            "eq": channel_bool_prop("eq.On"),
-            "eq_ab": channel_bool_prop("eq.ab"),
             "label": channel_label_prop(),
         },
     )(remote, i)
 
 
 def request_bus_obj(phys_bus, remote, i) -> Bus:
     """
```

### Comparing `vban-cmd-1.8.1/vban_cmd/command.py` & `vban-cmd-2.0.0/vban_cmd/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .iremote import IRemote
-from .meta import action_prop
+from .meta import action_fn
 
 
 class Command(IRemote):
     """
     Implements the common interface
 
     Defines concrete implementation for command
@@ -17,18 +17,17 @@
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
 
     @property
     def identifier(self) -> str:
         return "Command"
```

### Comparing `vban-cmd-1.8.1/vban_cmd/config.py` & `vban-cmd-2.0.0/vban_cmd/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import itertools
 import logging
 from pathlib import Path
 
+from .error import VBANCMDError
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
@@ -28,18 +32,26 @@
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
+        self.bus_float = ["gain = 0.0"]
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
@@ -62,15 +74,15 @@
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
@@ -115,18 +127,17 @@
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
@@ -162,24 +173,24 @@
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
+        Path.home() / ".config" / "vban-cmd" / kind.name,
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
 
 
@@ -187,10 +198,10 @@
     """
     config entry point.
 
     Returns all configs loaded into memory for a kind
     """
     try:
         configs = loader(kindmap(kind_id))
-    except KeyError as e:
-        print(f"Unknown Voicemeeter kind '{kind_id}'")
+    except KeyError:
+        raise VBANCMDError(f"Unknown Voicemeeter kind {kind_id}")
     return configs
```

### Comparing `vban-cmd-1.8.1/vban_cmd/event.py` & `vban-cmd-2.0.0/vban_cmd/event.py`

 * *Files 15% similar despite different names*

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

### Comparing `vban-cmd-1.8.1/vban_cmd/factory.py` & `vban-cmd-2.0.0/vban_cmd/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 from enum import IntEnum
 from functools import cached_property
 from typing import Iterable, NoReturn
 
 from .bus import request_bus_obj as bus
 from .command import Command
 from .config import request_config as configs
+from .error import VBANCMDError
 from .kinds import KindMapClass
 from .kinds import request_kind_map as kindmap
 from .strip import request_strip_obj as strip
 from .vbancmd import VbanCmd
 
+logger = logging.getLogger(__name__)
+
 
 class FactoryBuilder:
     """
     Builder class for factories.
 
     Separates construction from representation.
     """
 
-    logger = logging.getLogger("vbancmd.factorybuilder")
     BuilderProgress = IntEnum("BuilderProgress", "strip bus command", start=0)
 
     def __init__(self, factory, kind: KindMapClass):
         self._factory = factory
         self.kind = kind
         self._info = (
             f"Finished building strips for {self._factory}",
             f"Finished building buses for {self._factory}",
             f"Finished building commands for {self._factory}",
         )
+        self.logger = logger.getChild(self.__class__.__name__)
 
     def _pinfo(self, name: str) -> NoReturn:
         """prints progress status for each step"""
         name = name.split("_")[1]
         self.logger.info(self._info[int(getattr(self.BuilderProgress, name))])
 
     def make_strip(self):
@@ -56,27 +59,28 @@
         return self
 
 
 class FactoryBase(VbanCmd):
     """Base class for factories, subclasses VbanCmd."""
 
     def __init__(self, kind_id: str, **kwargs):
-        defaultsubs = {"pdirty": True, "ldirty": False}
-        if "subs" in kwargs:
-            defaultsubs = defaultsubs | kwargs.pop("subs")
         defaultkwargs = {
             "ip": None,
             "port": 6980,
             "streamname": "Command1",
             "bps": 0,
             "channel": 0,
             "ratelimit": 0.01,
+            "timeout": 5,
             "sync": False,
-            "subs": defaultsubs,
+            "pdirty": False,
+            "ldirty": False,
         }
+        if "subs" in kwargs:
+            defaultkwargs |= kwargs.pop("subs")  # for backwards compatibility
         kwargs = defaultkwargs | kwargs
         self.kind = kindmap(kind_id)
         super().__init__(**kwargs)
         self.builder = FactoryBuilder(self, self.kind)
         self._steps = (
             self.builder.make_strip,
             self.builder.make_bus,
@@ -184,13 +188,16 @@
 
 def request_vbancmd_obj(kind_id: str, **kwargs) -> VbanCmd:
     """
     Interface entry point. Wraps factory method and handles errors
 
     Returns a reference to a VbanCmd class of a kind
     """
+    logger_entry = logger.getChild("factory.request_vbancmd_obj")
+
     VBANCMD_obj = None
     try:
         VBANCMD_obj = vbancmd_factory(kind_id, **kwargs)
     except (ValueError, TypeError) as e:
-        raise SystemExit(e)
+        logger_entry.exception(f"{type(e).__name__}: {e}")
+        raise VBANCMDError(str(e)) from e
     return VBANCMD_obj
```

### Comparing `vban-cmd-1.8.1/vban_cmd/iremote.py` & `vban-cmd-2.0.0/vban_cmd/iremote.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import logging
 import time
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class Modes:
     """Channel Modes"""
 
     _mute: hex = 0x00000001
     _solo: hex = 0x00000002
@@ -22,17 +25,17 @@
     _upmix61: hex = 0x00000080
     _centeronly: hex = 0x00000090
     _lfeonly: hex = 0x000000A0
     _rearonly: hex = 0x000000B0
 
     _mask: hex = 0x000000F0
 
-    _eq_on: hex = 0x00000100
+    _on: hex = 0x00000100  # eq.on
     _cross: hex = 0x00000200
-    _eq_ab: hex = 0x00000800
+    _ab: hex = 0x00000800  # eq.ab
 
     _busa: hex = 0x00001000
     _busa1: hex = 0x00001000
     _busa2: hex = 0x00002000
     _busa3: hex = 0x00004000
     _busa4: hex = 0x00008000
     _busa5: hex = 0x00080000
@@ -81,26 +84,35 @@
 
     Provides some default implementation
     """
 
     def __init__(self, remote, index=None):
         self._remote = remote
         self.index = index
+        self.logger = logger.getChild(self.__class__.__name__)
         self._modes = Modes()
 
     def getter(self, param):
-        cmd = f"{self.identifier}.{param}"
+        cmd = self._cmd(param)
+        self.logger.debug(f"getter: {cmd}")
         if cmd in self._remote.cache:
             return self._remote.cache.pop(cmd)
         if self._remote.sync:
             self._remote.clear_dirty()
 
     def setter(self, param, val):
         """Sends a string request RT packet."""
-        self._remote._set_rt(f"{self.identifier}", param, val)
+        self.logger.debug(f"setter: {self._cmd(param)}={val}")
+        self._remote._set_rt(self.identifier, param, val)
+
+    def _cmd(self, param):
+        cmd = (self.identifier,)
+        if param:
+            cmd += (f".{param}",)
+        return "".join(cmd)
 
     @abstractmethod
     def identifier(self):
         pass
 
     @property
     def public_packet(self):
@@ -109,24 +121,30 @@
 
     def apply(self, data):
         """Sets all parameters of a dict for the channel."""
 
         def fget(attr, val):
             if attr == "mode":
                 return (f"mode.{val}", 1)
+            elif attr == "knob":
+                return ("", val)
             return (attr, val)
 
-        script = str()
         for attr, val in data.items():
-            if hasattr(self, attr):
-                attr, val = fget(attr, val)
-                if isinstance(val, bool):
-                    val = 1 if val else 0
-
-                self._remote.cache[f"{self.identifier}.{attr}"] = val
-                script += f"{self.identifier}.{attr}={val};"
-
-        self._remote.sendtext(script)
+            if not isinstance(val, dict):
+                if attr in dir(self):  # avoid calling getattr (with hasattr)
+                    attr, val = fget(attr, val)
+                    if isinstance(val, bool):
+                        val = 1 if val else 0
+
+                    self._remote.cache[self._cmd(attr)] = val
+                    self._remote._script += f"{self._cmd(attr)}={val};"
+            else:
+                target = getattr(self, attr)
+                target.apply(val)
         return self
 
     def then_wait(self):
+        self.logger.debug(self._remote._script)
+        self._remote.sendtext(self._remote._script)
+        self._remote._script = str()
         time.sleep(self._remote.DELAY)
```

### Comparing `vban-cmd-1.8.1/vban_cmd/kinds.py` & `vban-cmd-2.0.0/vban_cmd/kinds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum, unique
 
+from .error import VBANCMDError
+
 
 @unique
 class KindId(Enum):
     BASIC = 1
     BANANA = 2
     POTATO = 3
 
@@ -93,12 +95,12 @@
 
 
 def request_kind_map(kind_id):
     KIND_obj = None
     try:
         KIND_obj = kind_factory(kind_id)
     except ValueError as e:
-        print(e)
+        raise VBANCMDError(str(e)) from e
     return KIND_obj
 
 
 kinds_all = list(request_kind_map(kind_id.name.lower()) for kind_id in KindId)
```

### Comparing `vban-cmd-1.8.1/vban_cmd/meta.py` & `vban-cmd-2.0.0/vban_cmd/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             not int.from_bytes(
                 getattr(
                     self.public_packet,
                     f"{'strip' if 'strip' in type(self).__name__.lower() else 'bus'}state",
                 )[self.index],
                 "little",
             )
-            & getattr(self._modes, f'_{param.replace(".", "_").lower()}')
+            & getattr(self._modes, f"_{param.lower()}")
             == 0
         )
 
     def fset(self, val):
         self.setter(param, 1 if val else 0)
 
     return property(fget, fset)
@@ -87,14 +87,14 @@
 
     def fset(self, val):
         self.setter(param, 1 if val else 0)
 
     return property(fget, fset)
 
 
-def action_prop(param, val=1):
-    """A param that performs an action"""
+def action_fn(param, val=1):
+    """A function that performs an action"""
 
     def fdo(self):
         self.setter(param, val)
 
     return fdo
```

### Comparing `vban-cmd-1.8.1/vban_cmd/packet.py` & `vban-cmd-2.0.0/vban_cmd/packet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 from dataclasses import dataclass
-from typing import Generator
 
+from .kinds import KindMapClass
 from .util import comp
 
 VBAN_SERVICE_RTPACKETREGISTER = 32
 VBAN_SERVICE_RTPACKET = 33
 MAX_PACKET_SIZE = 1436
 HEADER_SIZE = 4 + 1 + 1 + 1 + 1 + 16 + 4
 
 
 @dataclass
 class VbanRtPacket:
     """Represents the body of a VBAN RT data packet"""
 
-    def __init__(self, **kwargs):
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-        self._strip_level = self._generate_levels(self._inputLeveldB100)
-        self._bus_level = self._generate_levels(self._outputLeveldB100)
+    _kind: KindMapClass
+    _voicemeeterType: bytes
+    _reserved: bytes
+    _buffersize: bytes
+    _voicemeeterVersion: bytes
+    _optionBits: bytes
+    _samplerate: bytes
+    _inputLeveldB100: bytes
+    _outputLeveldB100: bytes
+    _TransportBit: bytes
+    _stripState: bytes
+    _busState: bytes
+    _stripGaindB100Layer1: bytes
+    _stripGaindB100Layer2: bytes
+    _stripGaindB100Layer3: bytes
+    _stripGaindB100Layer4: bytes
+    _stripGaindB100Layer5: bytes
+    _stripGaindB100Layer6: bytes
+    _stripGaindB100Layer7: bytes
+    _stripGaindB100Layer8: bytes
+    _busGaindB100: bytes
+    _stripLabelUTF8c60: bytes
+    _busLabelUTF8c60: bytes
 
     def _generate_levels(self, levelarray) -> tuple:
         return tuple(
             int.from_bytes(levelarray[i : i + 2], "little")
             for i in range(0, len(levelarray), 2)
         )
 
+    @property
+    def strip_levels(self):
+        return self._generate_levels(self._inputLeveldB100)
+
+    @property
+    def bus_levels(self):
+        return self._generate_levels(self._outputLeveldB100)
+
     def pdirty(self, other) -> bool:
         """True iff any defined parameter has changed"""
 
         return not (
             self._stripState == other._stripState
             and self._busState == other._busState
             and self._stripGaindB100Layer1 == other._stripGaindB100Layer1
@@ -42,16 +68,16 @@
             and self._busGaindB100 == other._busGaindB100
             and self._stripLabelUTF8c60 == other._stripLabelUTF8c60
             and self._busLabelUTF8c60 == other._busLabelUTF8c60
         )
 
     def ldirty(self, strip_cache, bus_cache) -> bool:
         self._strip_comp, self._bus_comp = (
-            tuple(not val for val in comp(strip_cache, self._strip_level)),
-            tuple(not val for val in comp(bus_cache, self._bus_level)),
+            tuple(not val for val in comp(strip_cache, self.strip_levels)),
+            tuple(not val for val in comp(bus_cache, self.bus_levels)),
         )
         return any(any(l) for l in (self._strip_comp, self._bus_comp))
 
     @property
     def voicemeetertype(self) -> str:
         """returns voicemeeter type as a string"""
         type_ = ("basic", "banana", "potato")
@@ -73,20 +99,20 @@
     def samplerate(self) -> int:
         """returns samplerate as an int"""
         return int.from_bytes(self._samplerate, "little")
 
     @property
     def inputlevels(self) -> tuple:
         """returns the entire level array across all inputs for a kind"""
-        return self._strip_level[0 : (2 * self._kind.phys_in + 8 * self._kind.virt_in)]
+        return self.strip_levels[0 : (2 * self._kind.phys_in + 8 * self._kind.virt_in)]
 
     @property
     def outputlevels(self) -> tuple:
         """returns the entire level array across all outputs for a kind"""
-        return self._bus_level[0 : 8 * self._kind.num_bus]
+        return self.bus_levels[0 : 8 * self._kind.num_bus]
 
     @property
     def stripstate(self) -> tuple:
         """returns tuple of strip states accessable through bit modes"""
         return tuple(self._stripState[i : i + 4] for i in range(0, 32, 4))
 
     @property
```

### Comparing `vban-cmd-1.8.1/vban_cmd/util.py` & `vban-cmd-2.0.0/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban-cmd-1.8.1/vban_cmd/vbancmd.py` & `vban-cmd-2.0.0/vban_cmd/vbancmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,110 +1,137 @@
 import logging
 import socket
 import time
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
+from queue import Queue
 from typing import Iterable, Optional, Union
 
-try:
-    import tomllib
-except ModuleNotFoundError:
-    import tomli as tomllib
-
+from .error import VBANCMDError
 from .event import Event
 from .packet import RequestHeader
 from .subject import Subject
 from .util import Socket, script
-from .worker import Subscriber, Updater
+from .worker import Producer, Subscriber, Updater
+
+logger = logging.getLogger(__name__)
 
 
 class VbanCmd(metaclass=ABCMeta):
     """Base class responsible for communicating with the VBAN RT Packet Service"""
 
     DELAY = 0.001
     # fmt: off
     BPS_OPTS = [
         0, 110, 150, 300, 600, 1200, 2400, 4800, 9600, 14400, 19200, 31250,
         38400, 57600, 115200, 128000, 230400, 250000, 256000, 460800, 921600,
         1000000, 1500000, 2000000, 3000000,
     ]
     # fmt: on
-    logger = logging.getLogger("vbancmd.vbancmd")
 
     def __init__(self, **kwargs):
+        self.logger = logger.getChild(self.__class__.__name__)
+        self.event = Event({k: kwargs.pop(k) for k in ("pdirty", "ldirty")})
+        if not kwargs["ip"]:
+            kwargs |= self._conn_from_toml()
         for attr, val in kwargs.items():
             setattr(self, attr, val)
-        if self.ip is None:
-            conn = self._conn_from_toml()
-            for attr, val in conn.items():
-                setattr(self, attr, val)
 
         self.packet_request = RequestHeader(
             name=self.streamname,
             bps_index=self.BPS_OPTS.index(self.bps),
             channel=self.channel,
         )
         self.socks = tuple(
             socket.socket(socket.AF_INET, socket.SOCK_DGRAM) for _ in Socket
         )
-        self.subject = Subject()
+        self.subject = self.observer = Subject()
         self.cache = {}
-        self.event = Event(self.subs)
         self._pdirty = False
         self._ldirty = False
 
     @abstractmethod
     def __str__(self):
         """Ensure subclasses override str magic method"""
         pass
 
-    def _conn_from_toml(self) -> str:
-        filepath = Path.cwd() / "vban.toml"
-        with open(filepath, "rb") as f:
-            conn = tomllib.load(f)
-        return conn["connection"]
+    def _conn_from_toml(self) -> dict:
+        try:
+            import tomllib
+        except ModuleNotFoundError:
+            import tomli as tomllib
+
+        def get_filepath():
+            filepaths = [
+                Path.cwd() / "vban.toml",
+                Path.home() / ".config" / "vban-cmd" / "vban.toml",
+                Path.home() / "Documents" / "Voicemeeter" / "vban.toml",
+            ]
+            for filepath in filepaths:
+                if filepath.exists():
+                    return filepath
+
+        if filepath := get_filepath():
+            with open(filepath, "rb") as f:
+                conn = tomllib.load(f)
+                assert (
+                    "ip" in conn["connection"]
+                ), "please provide ip, by kwarg or config"
+            return conn["connection"]
+        else:
+            raise VBANCMDError("no ip provided and no vban.toml located.")
 
     def __enter__(self):
         self.login()
         return self
 
     def login(self):
         """Starts the subscriber and updater threads"""
         self.running = True
         self.event.info()
 
         self.subscriber = Subscriber(self)
         self.subscriber.start()
 
-        self.updater = Updater(self)
+        queue = Queue()
+        self.updater = Updater(self, queue)
         self.updater.start()
+        self.producer = Producer(self, queue)
+        self.producer.start()
 
         self.logger.info(f"{type(self).__name__}: Successfully logged into {self}")
 
     def _set_rt(
         self,
         id_: str,
         param: Optional[str] = None,
         val: Optional[Union[int, float]] = None,
     ):
         """Sends a string request command over a network."""
-        cmd = id_ if not param else f"{id_}.{param}={val};"
+        cmd = f"{id_}={val};" if not param else f"{id_}.{param}={val};"
         self.socks[Socket.request].sendto(
             self.packet_request.header + cmd.encode(),
             (socket.gethostbyname(self.ip), self.port),
         )
-        count = int.from_bytes(self.packet_request.framecounter, "little") + 1
-        self.packet_request.framecounter = count.to_bytes(4, "little")
+        self.packet_request.framecounter = (
+            int.from_bytes(self.packet_request.framecounter, "little") + 1
+        ).to_bytes(4, "little")
         if param:
             self.cache[f"{id_}.{param}"] = val
 
     @script
     def sendtext(self, cmd):
         """Sends a multiple parameter string over a network."""
-        self._set_rt(cmd)
+        self.socks[Socket.request].sendto(
+            self.packet_request.header + cmd.encode(),
+            (socket.gethostbyname(self.ip), self.port),
+        )
+        self.packet_request.framecounter = (
+            int.from_bytes(self.packet_request.framecounter, "little") + 1
+        ).to_bytes(4, "little")
         time.sleep(self.DELAY)
 
     @property
     def type(self) -> str:
         """Returns the type of Voicemeeter installation."""
         return self.public_packet.voicemeetertype
 
@@ -153,26 +180,27 @@
             obj, m2, *rem = key.split("-")
             index = int(m2) if m2.isnumeric() else int(*rem)
             if obj in ("strip", "bus"):
                 return getattr(self, obj)[index]
             else:
                 raise ValueError(obj)
 
+        self._script = str()
         [param(key).apply(datum).then_wait() for key, datum in data.items()]
 
     def apply_config(self, name):
         """applies a config from memory"""
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
 
     def logout(self):
         self.running = False
         time.sleep(0.2)
         [sock.close() for sock in self.socks]
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
```

### Comparing `vban-cmd-1.8.1/vban_cmd/worker.py` & `vban-cmd-2.0.0/vban_cmd/worker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,81 @@
 import logging
 import socket
 import threading
 import time
 from typing import Optional
 
-from .error import VBANCMDError
+from .error import VBANCMDConnectionError
 from .packet import HEADER_SIZE, SubscribeHeader, VbanRtPacket, VbanRtPacketHeader
-from .util import Socket, comp
+from .util import Socket
+
+logger = logging.getLogger(__name__)
 
 
 class Subscriber(threading.Thread):
     """fire a subscription packet every 10 seconds"""
 
     def __init__(self, remote):
-        super().__init__(name="subscriber", target=self.subscribe, daemon=True)
+        super().__init__(name="subscriber", daemon=True)
         self._remote = remote
+        self.logger = logger.getChild(self.__class__.__name__)
         self.packet = SubscribeHeader()
 
-    def subscribe(self):
+    def run(self):
         while self._remote.running:
             try:
                 self._remote.socks[Socket.register].sendto(
                     self.packet.header,
                     (socket.gethostbyname(self._remote.ip), self._remote.port),
                 )
-                count = int.from_bytes(self.packet.framecounter, "little") + 1
-                self.packet.framecounter = count.to_bytes(4, "little")
+                self.packet.framecounter = (
+                    int.from_bytes(self.packet.framecounter, "little") + 1
+                ).to_bytes(4, "little")
                 time.sleep(10)
-            except socket.gaierror:
-                err_msg = f"Unable to resolve hostname {self._remote.ip}"
-                print(err_msg)
-                raise VBANCMDError(err_msg)
-
-
-class Updater(threading.Thread):
-    """
-    continously updates the public packet
+            except socket.gaierror as e:
+                self.logger.exception(f"{type(e).__name__}: {e}")
+                raise VBANCMDConnectionError(
+                    f"unable to resolve hostname {self._remote.ip}"
+                ) from e
 
-    notifies observers of event updates
-    """
 
-    logger = logging.getLogger("worker.updater")
+class Producer(threading.Thread):
+    """Continously send job queue to the Updater thread at a rate of self._remote.ratelimit."""
 
-    def __init__(self, remote):
-        super().__init__(name="updater", target=self.update, daemon=True)
+    def __init__(self, remote, queue):
+        super().__init__(name="producer", daemon=True)
         self._remote = remote
-        self._remote.socks[Socket.response].settimeout(5)
-        self._remote.socks[Socket.response].bind(
-            (socket.gethostbyname(socket.gethostname()), self._remote.port)
-        )
+        self.queue = queue
+        self.logger = logger.getChild(self.__class__.__name__)
         self.packet_expected = VbanRtPacketHeader()
         self._remote._public_packet = self._get_rt()
         (
             self._remote.cache["strip_level"],
             self._remote.cache["bus_level"],
         ) = self._remote._get_levels(self._remote.public_packet)
-        p_in, v_in = self._remote.kind.ins
-        self._remote._strip_comp = [False] * (2 * p_in + 8 * v_in)
-        self._remote._bus_comp = [False] * (self._remote.kind.num_bus * 8)
+
+    def _get_rt(self) -> VbanRtPacket:
+        """Attempt to fetch data packet until a valid one found"""
+
+        def fget():
+            data = None
+            while not data:
+                data = self._fetch_rt_packet()
+                time.sleep(self._remote.DELAY)
+            return data
+
+        return fget()
 
     def _fetch_rt_packet(self) -> Optional[VbanRtPacket]:
         try:
             data, _ = self._remote.socks[Socket.response].recvfrom(2048)
             # check for packet data
             if len(data) > HEADER_SIZE:
                 # check if packet is of type rt packet response
                 if self.packet_expected.header == data[: HEADER_SIZE - 4]:
-                    self.logger.debug("valid packet received")
                     return VbanRtPacket(
                         _kind=self._remote.kind,
                         _voicemeeterType=data[28:29],
                         _reserved=data[29:30],
                         _buffersize=data[30:32],
                         _voicemeeterVersion=data[32:36],
                         _optionBits=data[36:40],
@@ -88,55 +93,82 @@
                         _stripGaindB100Layer6=data[388:404],
                         _stripGaindB100Layer7=data[404:420],
                         _stripGaindB100Layer8=data[420:436],
                         _busGaindB100=data[436:452],
                         _stripLabelUTF8c60=data[452:932],
                         _busLabelUTF8c60=data[932:1412],
                     )
-        except TimeoutError:
-            err_msg = f"Unable to establish connection with {self._remote.ip}"
-            print(err_msg)
-            raise VBANCMDError(err_msg)
+        except TimeoutError as e:
+            self.logger.exception(f"{type(e).__name__}: {e}")
+            raise VBANCMDConnectionError(
+                f"timeout waiting for RtPacket from {self._remote.ip}"
+            ) from e
 
-    def _get_rt(self) -> VbanRtPacket:
-        """Attempt to fetch data packet until a valid one found"""
-
-        def fget():
-            data = None
-            while not data:
-                data = self._fetch_rt_packet()
-                time.sleep(self._remote.DELAY)
-            return data
-
-        return fget()
-
-    def update(self):
+    def run(self):
         while self._remote.running:
-            start = time.time()
             _pp = self._get_rt()
             pdirty = _pp.pdirty(self._remote.public_packet)
             ldirty = _pp.ldirty(
                 self._remote.cache["strip_level"], self._remote.cache["bus_level"]
             )
 
             if pdirty or ldirty:
-                self.logger.debug("dirty state, updating public packet")
                 self._remote._public_packet = _pp
-                self._remote._pdirty = pdirty
-                self._remote._ldirty = ldirty
+            self._remote._pdirty = pdirty
+            self._remote._ldirty = ldirty
+
+            if self._remote.event.pdirty:
+                self.queue.put("pdirty")
+            if self._remote.event.ldirty:
+                self.queue.put("ldirty")
+            time.sleep(self._remote.ratelimit)
+        self.logger.debug(f"terminating {self.name} thread")
+        self.queue.put(None)
+
+
+class Updater(threading.Thread):
+    """
+    continously updates the public packet
+
+    notifies observers of event updates
+    """
+
+    def __init__(self, remote, queue):
+        super().__init__(name="updater", daemon=True)
+        self._remote = remote
+        self.queue = queue
+        self.logger = logger.getChild(self.__class__.__name__)
+        self._remote.socks[Socket.response].settimeout(self._remote.timeout)
+        self._remote.socks[Socket.response].bind(
+            (socket.gethostbyname(socket.gethostname()), self._remote.port)
+        )
+        p_in, v_in = self._remote.kind.ins
+        self._remote._strip_comp = [False] * (2 * p_in + 8 * v_in)
+        self._remote._bus_comp = [False] * (self._remote.kind.num_bus * 8)
 
-            if self._remote.event.pdirty and self._remote.pdirty:
-                self._remote.subject.notify("pdirty")
-            if self._remote.event.ldirty and self._remote.ldirty:
+    def run(self):
+        """
+        Continously update observers of dirty states.
+
+        Generate _strip_comp, _bus_comp and update level cache if ldirty.
+        """
+        while True:
+            event = self.queue.get()
+            if event is None:
+                self.logger.debug(f"terminating {self.name} thread")
+                break
+
+            if event == "pdirty" and self._remote.pdirty:
+                self._remote.subject.notify(event)
+            elif event == "ldirty" and self._remote.ldirty:
                 self._remote._strip_comp, self._remote._bus_comp = (
-                    _pp._strip_comp,
-                    _pp._bus_comp,
+                    self._remote._public_packet._strip_comp,
+                    self._remote._public_packet._bus_comp,
                 )
-                self._remote.cache["strip_level"], self._remote.cache["bus_level"] = (
-                    _pp.inputlevels,
-                    _pp.outputlevels,
+                (
+                    self._remote.cache["strip_level"],
+                    self._remote.cache["bus_level"],
+                ) = (
+                    self._remote._public_packet.inputlevels,
+                    self._remote._public_packet.outputlevels,
                 )
-                self._remote.subject.notify("ldirty")
-
-            elapsed = time.time() - start
-            if self._remote.ratelimit - elapsed > 0:
-                time.sleep(self._remote.ratelimit - elapsed)
+                self._remote.subject.notify(event)
```

### Comparing `vban-cmd-1.8.1/setup.py` & `vban-cmd-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,25 +6,32 @@
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
+entry_points = \
+{'console_scripts': ['gui = scripts:ex_gui',
+                     'obs = scripts:ex_obs',
+                     'observer = scripts:ex_observer',
+                     'test = scripts:test']}
+
 setup_kwargs = {
     'name': 'vban-cmd',
-    'version': '1.8.1',
+    'version': '2.0.0',
     'description': 'Python interface for the VBAN RT Packet Service (Sendtext)',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/vban-cmd.svg)](https://badge.fury.io/py/vban-cmd)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/vban-cmd-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# VBAN CMD\n\nThis python interface allows you to get and set Voicemeeter parameter values over a network.\n\nIt may be used standalone or to extend the [Voicemeeter Remote Python API](https://github.com/onyx-and-iris/voicemeeter-api-python)\n\nThere is no support for audio transfer in this package, only parameters.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.4\n-   Banana 2.0.6.4\n-   Potato 3.0.2.4\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install vban-cmd`\n\n## `Use`\n\n#### Connection\n\nLoad VBAN connection info from toml config. A valid `vban.toml` might look like this:\n\n```toml\n[connection]\nip = "gamepc.local"\nport = 6980\nstreamname = "Command1"\n```\n\nIt should be placed next to your `__main__.py` file.\n\nAlternatively you may pass `ip`, `port`, `streamname` as keyword arguments.\n\n#### `__main__.py`\n\nSimplest use case, use a context manager to request a VbanCmd class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n```python\nimport vban_cmd\n\n\nclass ManyThings:\n    def __init__(self, vban):\n        self.vban = vban\n\n    def things(self):\n        self.vban.strip[0].label = "podmic"\n        self.vban.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vban.strip[0].label}) mute has been set to {self.vban.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vban.bus[3].gain = -6.3\n        self.vban.bus[4].eq = True\n        info = (\n            f"bus 3 gain has been set to {self.vban.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vban.bus[4].eq}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    with vban_cmd.api(kind_id, ip="gamepc.local", port=6980, streamname="Command1") as vban:\n        do = ManyThings(vban)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vban.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True},\n            }\n        )\n\n\nif __name__ == "__main__":\n    kind_id = "banana"\n\n    main()\n```\n\nOtherwise you must remember to call `vban.login()`, `vban.logout()` at the start/end of your code.\n\n## `kind_id`\n\nPass the kind of Voicemeeter as an argument. kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `label`: string\n-   `gain`: float, -60 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `comp`: float, from 0.0 to 10.0\n-   `gate`: float, from 0.0 to 10.0\n-   `limit`: int, from -40 to 12\n\nexample:\n\n```python\nvban.strip[3].gain = 3.7\nprint(vban.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvban.strip[5].appmute("Spotify", True)\nvban.strip[5].appgain("Spotify", 0.5)\n```\n\n##### Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvban.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Levels\n\nThe following properties are available.\n\n-   `prefader`\n\nexample:\n\n```python\nprint(vban.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `eq`: boolean\n-   `eq_ab`: boolean\n-   `mute`: boolean\n-   `label`: string\n-   `gain`: float, -60 to 12\n\nexample:\n\n```python\nvban.bus[4].eq = true\nprint(vban.bus[0].label)\n```\n\n##### Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvban.bus[4].mode.amix = True\n\nprint(vban.bus[2].mode.get())\n```\n\n##### Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vban.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvban.strip[0].fadeto(-10.3, 1000)\nvban.bus[3].fadeby(-5.6, 500)\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values. The following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are write only and accept boolean values.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvban.command.restart()\nvban.command.showvbanchat = true\n```\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus parameters at once, for example:\n\n```python\nvban.apply(\n    {\n        "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-2": {"mute": True},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvban.strip[0].apply(mute: true, gain: 3.2, A1: true)\nvban.vban.outstream[0].apply(on: true, name: \'streamname\', bit: 24)\n```\n\n## Config Files\n\n`vban.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport vban_cmd\nwith vban_cmd.api(\'banana\') as vban:\n    vban.apply_config(\'example\')\n```\n\nwill load a config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nLevel updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.\n\nexample:\n\n```python\nimport vban_cmd\n# Listen for level updates\nopts = {\n    "ip": "<ip address>",\n    "streamname": "Command1",\n    "port": 6980,\n    "subs": {"ldirty": True},\n}\nwith vban_cmd.api(\'banana\', **opts) as vban:\n    ...\n```\n\n#### `vban.subject`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vban):\n        vban.subject.add(self)\n        ...\n```\n\n#### `vban.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvban.event.ldirty = True\n\nvban.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvban.event.remove(["pdirty", "ldirty"])\n\n# get a list of currently subscribed\nprint(vban.event.get())\n```\n\n## VbanCmd class\n\n`vban_cmd.api(kind_id: str, **opts: dict)`\n\nYou may pass the following optional keyword arguments:\n\n-   `ip`: str, ip or hostname of remote machine\n-   `streamname`: str, name of the stream to connect to.\n-   `port`: int=6980, vban udp port of remote machine.\n-   `subs`: dict={"pdirty": True, "ldirty": False}, controls which updates to listen for.\n    -   `pdirty`: parameter updates\n    -   `ldirty`: level updates\n\n#### `vban.pdirty`\n\nTrue iff a parameter has been changed.\n\n#### `vban.ldirty`\n\nTrue iff a level value has been changed.\n\n#### `vban.sendtext(script)`\n\nSends a script block as a string request, for example:\n\n```python\nvban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")\n```\n\n#### `vban.public_packet`\n\nReturns a Voicemeeter rt data packet object. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).\n\n### `Errors`\n\n-   `errors.VBANCMDError`: Base VMCMD error class.\n\n### `Tests`\n\nFirst make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)\n\nThen from tests directory:\n\n`pytest -v`\n\n## Resources\n\n-   [Voicemeeter VBAN TEXT](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=19)\n\n-   [Voicemeeter RT Packet Service](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=27)\n',
+    'long_description': '[![PyPI version](https://badge.fury.io/py/vban-cmd.svg)](https://badge.fury.io/py/vban-cmd)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/vban-cmd-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# VBAN CMD\n\nThis python interface allows you to get and set Voicemeeter parameter values over a network.\n\nIt may be used standalone or to extend the [Voicemeeter Remote Python API](https://github.com/onyx-and-iris/voicemeeter-api-python)\n\nThere is no support for audio transfer in this package, only parameters.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.8\n-   Banana 2.0.6.8\n-   Potato 3.0.2.8\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install vban-cmd`\n\n## `Use`\n\n#### Connection\n\nLoad VBAN connection info from toml config. A valid `vban.toml` might look like this:\n\n```toml\n[connection]\nip = "gamepc.local"\nport = 6980\nstreamname = "Command1"\n```\n\nIt should be placed next to your `__main__.py` file.\n\nAlternatively you may pass `ip`, `port`, `streamname` as keyword arguments.\n\n#### `__main__.py`\n\nSimplest use case, use a context manager to request a VbanCmd class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n```python\nimport vban_cmd\n\n\nclass ManyThings:\n    def __init__(self, vban):\n        self.vban = vban\n\n    def things(self):\n        self.vban.strip[0].label = "podmic"\n        self.vban.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vban.strip[0].label}) mute has been set to {self.vban.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vban.bus[3].gain = -6.3\n        self.vban.bus[4].eq.on = True\n        info = (\n            f"bus 3 gain has been set to {self.vban.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vban.bus[4].eq.on}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    KIND_ID = "banana"\n\n    with vban_cmd.api(\n        KIND_ID, ip="gamepc.local", port=6980, streamname="Command1"\n    ) as vban:\n        do = ManyThings(vban)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vban.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True, "eq": {"on": True}},\n            }\n        )\n\n\nif __name__ == "__main__":\n    main()\n```\n\nOtherwise you must remember to call `vban.login()`, `vban.logout()` at the start/end of your code.\n\n## `KIND_ID`\n\nPass the kind of Voicemeeter as an argument. KIND_ID may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `label`: string\n-   `gain`: float, -60 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `limit`: int, from -40 to 12\n\nexample:\n\n```python\nvban.strip[3].gain = 3.7\nprint(vban.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvban.strip[5].appmute("Spotify", True)\nvban.strip[5].appgain("Spotify", 0.5)\n```\n\n##### Strip.Comp\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n-   `gainin`: float, from -24.0 to 24.0\n-   `ratio`: float, from 1.0 to 8.0\n-   `threshold`: float, from -40.0 to -3.0\n-   `attack`: float, from 0.0 to 200.0\n-   `release`: float, from 0.0 to 5000.0\n-   `knee`: float, from 0.0 to 1.0\n-   `gainout`: float, from -24.0 to 24.0\n-   `makeup`: boolean\n\nexample:\n\n```python\nprint(vm.strip[4].comp.knob)\n```\n\nStrip Comp properties are defined as write only.\n\n`knob` defined for all versions, all other parameters potato only.\n\n##### Strip.Gate\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n-   `threshold`: float, from -60.0 to -10.0\n-   `damping`: float, from -60.0 to -10.0\n-   `bpsidechain`: int, from 100 to 4000\n-   `attack`: float, from 0.0 to 1000.0\n-   `hold`: float, from 0.0 to 5000.0\n-   `release`: float, from 0.0 to 5000.0\n\nexample:\n\n```python\nvm.strip[2].gate.attack = 300.8\n```\n\nStrip Gate properties are defined as write only, potato version only.\n\n`knob` defined for all versions, all other parameters potato only.\n\n##### Strip.Denoiser\n\nThe following properties are available.\n\n-   `knob`: float, from 0.0 to 10.0\n\nstrip.denoiser properties are defined as write only, potato version only.\n\n##### Strip.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\nStrip EQ properties are defined as write only, potato version only.\n\n##### Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvban.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Levels\n\nThe following properties are available.\n\n-   `prefader`\n\nexample:\n\n```python\nprint(vban.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `mute`: boolean\n-   `label`: string\n-   `gain`: float, -60 to 12\n\nexample:\n\n```python\nvban.bus[4].eq = true\nprint(vban.bus[0].label)\n```\n\n##### Bus.EQ\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `ab`: boolean\n\n##### Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvban.bus[4].mode.amix = True\n\nprint(vban.bus[2].mode.get())\n```\n\n##### Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vban.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvban.strip[0].fadeto(-10.3, 1000)\nvban.bus[3].fadeby(-5.6, 500)\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values. The following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are write only and accept boolean values.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvban.command.restart()\nvban.command.showvbanchat = true\n```\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus parameters at once, for example:\n\n```python\nvban.apply(\n    {\n        "strip-0": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-1": {"mute": True, "mode": "composite"},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvban.strip[0].apply(mute: true, gain: 3.2, A1: true)\nvban.bus[0].apply(A1: true)\n```\n\n## Config Files\n\n`vban.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport vban_cmd\nwith vban_cmd.api(\'banana\') as vban:\n    vban.apply_config(\'example\')\n```\n\nwill load a config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nLevel updates are considered high volume, by default they are NOT listened for. Use `subs` keyword arg to initialize event updates.\n\nexample:\n\n```python\nimport vban_cmd\n# Listen for level updates\nopts = {\n    "ip": "<ip address>",\n    "streamname": "Command1",\n    "port": 6980,\n}\nwith vban_cmd.api(\'banana\', ldirty=True, **opts) as vban:\n    ...\n```\n\n#### `vban.subject`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vban):\n        vban.subject.add(self)\n        ...\n```\n\n#### `vban.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvban.event.ldirty = True\n\nvban.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvban.event.remove(["pdirty", "ldirty"])\n\n# get a list of currently subscribed\nprint(vban.event.get())\n```\n\n## VbanCmd class\n\n`vban_cmd.api(kind_id: str, **opts)`\n\nYou may pass the following optional keyword arguments:\n\n-   `ip`: str, ip or hostname of remote machine\n-   `streamname`: str, name of the stream to connect to.\n-   `port`: int=6980, vban udp port of remote machine.\n-   `pdirty`: parameter updates\n-   `ldirty`: level updates\n\n#### `vban.pdirty`\n\nTrue iff a parameter has been changed.\n\n#### `vban.ldirty`\n\nTrue iff a level value has been changed.\n\n#### `vban.sendtext(script)`\n\nSends a script block as a string request, for example:\n\n```python\nvban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")\n```\n\n#### `vban.public_packet`\n\nReturns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).\n\n### `Errors`\n\n-   `errors.VBANCMDError`: Base VMCMD error class.\n\n### `Tests`\n\nFirst make sure you installed the [development dependencies](https://github.com/onyx-and-iris/vban-cmd-python#installation)\n\nThen from tests directory:\n\n`pytest -v`\n\n## Resources\n\n-   [Voicemeeter VBAN TEXT](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=19)\n\n-   [Voicemeeter RT Packet Service](https://vb-audio.com/Voicemeeter/VBANProtocol_Specifications.pdf#page=27)\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/vban-cmd-python',
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `vban-cmd-1.8.1/PKG-INFO` & `vban-cmd-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 1.8.1
+Version: 2.0.0
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -30,17 +30,17 @@
 
 There is no support for audio transfer in this package, only parameters.
 
 For an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)
 
 ## Tested against
 
--   Basic 1.0.8.4
--   Banana 2.0.6.4
--   Potato 3.0.2.4
+-   Basic 1.0.8.8
+-   Banana 2.0.6.8
+-   Potato 3.0.2.8
 
 ## Requirements
 
 -   [Voicemeeter](https://voicemeeter.com/)
 -   Python 3.10 or greater
 
 ## Installation
@@ -83,48 +83,50 @@
         self.vban.strip[0].mute = True
         print(
             f"strip 0 ({self.vban.strip[0].label}) mute has been set to {self.vban.strip[0].mute}"
         )
 
     def other_things(self):
         self.vban.bus[3].gain = -6.3
-        self.vban.bus[4].eq = True
+        self.vban.bus[4].eq.on = True
         info = (
             f"bus 3 gain has been set to {self.vban.bus[3].gain}",
-            f"bus 4 eq has been set to {self.vban.bus[4].eq}",
+            f"bus 4 eq has been set to {self.vban.bus[4].eq.on}",
         )
         print("\n".join(info))
 
 
 def main():
-    with vban_cmd.api(kind_id, ip="gamepc.local", port=6980, streamname="Command1") as vban:
+    KIND_ID = "banana"
+
+    with vban_cmd.api(
+        KIND_ID, ip="gamepc.local", port=6980, streamname="Command1"
+    ) as vban:
         do = ManyThings(vban)
         do.things()
         do.other_things()
 
         # set many parameters at once
         vban.apply(
             {
                 "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-                "bus-2": {"mute": True},
+                "bus-2": {"mute": True, "eq": {"on": True}},
             }
         )
 
 
 if __name__ == "__main__":
-    kind_id = "banana"
-
     main()
 ```
 
 Otherwise you must remember to call `vban.login()`, `vban.logout()` at the start/end of your code.
 
-## `kind_id`
+## `KIND_ID`
 
-Pass the kind of Voicemeeter as an argument. kind_id may be:
+Pass the kind of Voicemeeter as an argument. KIND_ID may be:
 
 -   `basic`
 -   `banana`
 -   `potato`
 
 ## `Available commands`
 
@@ -134,16 +136,14 @@
 
 -   `mono`: boolean
 -   `solo`: boolean
 -   `mute`: boolean
 -   `label`: string
 -   `gain`: float, -60 to 12
 -   `A1 - A5`, `B1 - B3`: boolean
--   `comp`: float, from 0.0 to 10.0
--   `gate`: float, from 0.0 to 10.0
 -   `limit`: int, from -40 to 12
 
 example:
 
 ```python
 vban.strip[3].gain = 3.7
 print(vban.strip[0].label)
@@ -162,14 +162,77 @@
 example:
 
 ```python
 vban.strip[5].appmute("Spotify", True)
 vban.strip[5].appgain("Spotify", 0.5)
 ```
 
+##### Strip.Comp
+
+The following properties are available.
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
+Strip Comp properties are defined as write only.
+
+`knob` defined for all versions, all other parameters potato only.
+
+##### Strip.Gate
+
+The following properties are available.
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
+Strip Gate properties are defined as write only, potato version only.
+
+`knob` defined for all versions, all other parameters potato only.
+
+##### Strip.Denoiser
+
+The following properties are available.
+
+-   `knob`: float, from 0.0 to 10.0
+
+strip.denoiser properties are defined as write only, potato version only.
+
+##### Strip.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
+Strip EQ properties are defined as write only, potato version only.
+
 ##### Gainlayers
 
 -   `gain`: float, from -60.0 to 12.0
 
 example:
 
 ```python
@@ -193,27 +256,32 @@
 Level properties will return -200.0 if no audio detected.
 
 ### Bus
 
 The following properties are available.
 
 -   `mono`: boolean
--   `eq`: boolean
--   `eq_ab`: boolean
 -   `mute`: boolean
 -   `label`: string
 -   `gain`: float, -60 to 12
 
 example:
 
 ```python
 vban.bus[4].eq = true
 print(vban.bus[0].label)
 ```
 
+##### Bus.EQ
+
+The following properties are available.
+
+-   `on`: boolean
+-   `ab`: boolean
+
 ##### Modes
 
 The following properties are available.
 
 -   `normal`: boolean
 -   `amix`: boolean
 -   `bmix`: boolean
@@ -293,25 +361,25 @@
 
 -   `apply`
     Set many strip/bus parameters at once, for example:
 
 ```python
 vban.apply(
     {
-        "strip-2": {"A1": True, "B1": True, "gain": -6.0},
-        "bus-2": {"mute": True},
+        "strip-0": {"A1": True, "B1": True, "gain": -6.0},
+        "bus-1": {"mute": True, "mode": "composite"},
     }
 )
 ```
 
 Or for each class you may do:
 
 ```python
 vban.strip[0].apply(mute: true, gain: 3.2, A1: true)
-vban.vban.outstream[0].apply(on: true, name: 'streamname', bit: 24)
+vban.bus[0].apply(A1: true)
 ```
 
 ## Config Files
 
 `vban.apply_config(<configname>)`
 
 You may load config files in TOML format.
@@ -335,17 +403,16 @@
 ```python
 import vban_cmd
 # Listen for level updates
 opts = {
     "ip": "<ip address>",
     "streamname": "Command1",
     "port": 6980,
-    "subs": {"ldirty": True},
 }
-with vban_cmd.api('banana', **opts) as vban:
+with vban_cmd.api('banana', ldirty=True, **opts) as vban:
     ...
 ```
 
 #### `vban.subject`
 
 Use the Subject class to register an app as event observer.
 
@@ -396,24 +463,23 @@
 
 # get a list of currently subscribed
 print(vban.event.get())
 ```
 
 ## VbanCmd class
 
-`vban_cmd.api(kind_id: str, **opts: dict)`
+`vban_cmd.api(kind_id: str, **opts)`
 
 You may pass the following optional keyword arguments:
 
 -   `ip`: str, ip or hostname of remote machine
 -   `streamname`: str, name of the stream to connect to.
 -   `port`: int=6980, vban udp port of remote machine.
--   `subs`: dict={"pdirty": True, "ldirty": False}, controls which updates to listen for.
-    -   `pdirty`: parameter updates
-    -   `ldirty`: level updates
+-   `pdirty`: parameter updates
+-   `ldirty`: level updates
 
 #### `vban.pdirty`
 
 True iff a parameter has been changed.
 
 #### `vban.ldirty`
 
@@ -425,15 +491,15 @@
 
 ```python
 vban.sendtext("Strip[0].Mute=1;Bus[0].Mono=1")
 ```
 
 #### `vban.public_packet`
 
-Returns a Voicemeeter rt data packet object. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).
+Returns a `VbanRtPacket`. Designed to be used internally by the interface but available for parsing through this read only property object. States not guaranteed to be current (requires use of dirty parameters to confirm).
 
 ### `Errors`
 
 -   `errors.VBANCMDError`: Base VMCMD error class.
 
 ### `Tests`
```

