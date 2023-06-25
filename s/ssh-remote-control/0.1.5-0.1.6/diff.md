# Comparing `tmp/ssh_remote_control-0.1.5.tar.gz` & `tmp/ssh_remote_control-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.5.tar", last modified: Sat Jun 24 10:04:33 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.6.tar", last modified: Sun Jun 25 04:10:15 2023, max compression
```

## Comparing `ssh_remote_control-0.1.5.tar` & `ssh_remote_control-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.629782 ssh_remote_control-0.1.5/
--rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1569 2023-06-24 10:04:33.628780 ssh_remote_control-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-06-20 06:12:24.000000 ssh_remote_control-0.1.5/README.md
--rw-rw-rw-   0        0        0      846 2023-06-24 10:00:35.000000 ssh_remote_control-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 10:04:33.630780 ssh_remote_control-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.530780 ssh_remote_control-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.573779 ssh_remote_control-0.1.5/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10709 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6661 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/command.py
--rw-rw-rw-   0        0        0     3533 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/command_set.py
-drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.625786 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/
--rw-rw-rw-   0        0        0      163 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/const.py
--rw-rw-rw-   0        0        0     3987 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/linux.py
--rw-rw-rw-   0        0        0     3822 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_cmd.py
--rw-rw-rw-   0        0        0     4087 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_ps.py
--rw-rw-rw-   0        0        0      645 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      222 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     3830 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     6787 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.611776 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1569 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.549109 ssh_remote_control-0.1.6/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-25 04:10:15.548107 ssh_remote_control-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-24 10:20:33.000000 ssh_remote_control-0.1.6/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-25 04:08:58.000000 ssh_remote_control-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 04:10:15.550104 ssh_remote_control-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.438638 ssh_remote_control-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.480322 ssh_remote_control-0.1.6/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10704 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     6659 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/command.py
+-rw-rw-rw-   0        0        0     3503 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/command_set.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.546105 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/
+-rw-rw-rw-   0        0        0      161 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/const.py
+-rw-rw-rw-   0        0        0     3978 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/linux.py
+-rw-rw-rw-   0        0        0     3813 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_cmd.py
+-rw-rw-rw-   0        0        0     4078 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_ps.py
+-rw-rw-rw-   0        0        0      645 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      222 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     3824 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     6757 2023-06-25 04:03:54.000000 ssh_remote_control-0.1.6/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-25 04:10:15.527110 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-25 04:10:15.000000 ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.5/LICENSE` & `ssh_remote_control-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.5/PKG-INFO` & `ssh_remote_control-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_remote_control
-Version: 0.1.5
+Version: 0.1.6
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.5/README.md` & `ssh_remote_control-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.5/pyproject.toml` & `ssh_remote_control-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 import async_timeout
 import icmplib
 import paramiko
 import wakeonlan
 
 from .command import (
+    ActionCommand,
     Command,
     CommandFormatError,
     CommandOutput,
     SensorCommand,
-    ServiceCommand,
 )
 from .command_set import CommandSet
-from .default_command_sets import SensorKey, ServiceKey
+from .default_command_sets import ActionKey, SensorKey
 from .event import Event
 from .helpers import name_to_key
 from .manager import DEFAULT_COMMAND_TIMEOUT, CommandExecuteError, Manager
 from .sensor import DynamicSensor, Sensor
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -316,15 +316,15 @@
         Raises:
             CommandFormatError
             CommandExecuteError
         """
         if self.allow_turn_off is False:
             return
 
-        await self.async_call_service(ServiceKey.TURN_OFF)
+        await self.async_run_action(ActionKey.TURN_OFF)
 
 
 class OfflineError(Exception):
     """Error to indicate host is offline."""
 
 
 class SSHAuthError(Exception):
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
             output.stderr,
             output.code,
         )
 
         return output
 
 
-class ServiceCommand(Command):
-    """The ServiceCommand class."""
+class ActionCommand(Command):
+    """The ActionCommand class."""
 
     def __init__(
         self,
         string: str,
         name: str | None = None,
         key: str | None = None,
         *,
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/command_set.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/command_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from copy import deepcopy
 
-from .command import SensorCommand, ServiceCommand
+from .command import ActionCommand, SensorCommand
 from .sensor import Sensor
 
 
 class CommandSet:
     """The CommandSet class."""
 
-    service_commands: list[ServiceCommand]
+    action_commands: list[ActionCommand]
     sensor_commands: list[SensorCommand]
 
     def __init__(
         self,
         name: str,
-        service_commands: list[ServiceCommand] | None = None,
+        action_commands: list[ActionCommand] | None = None,
         sensor_commands: list[SensorCommand] | None = None,
     ) -> None:
         self.name = name
-        self.set_service_commands(service_commands or [])
+        self.set_action_commands(action_commands or [])
         self.set_sensor_commands(sensor_commands or [])
 
     @property
-    def service_commands_by_key(self) -> dict[str, ServiceCommand]:
-        """Service commands by key."""
-        return {command.key: command for command in self.service_commands}
+    def action_commands_by_key(self) -> dict[str, ActionCommand]:
+        """Action commands by key."""
+        return {command.key: command for command in self.action_commands}
 
     @property
     def sensor_commands_by_sensor_key(self) -> dict[str, SensorCommand]:
         """Sensor commands by sensor key."""
         return {
             key: command
             for command in self.sensor_commands
@@ -39,63 +39,63 @@
         """Sensors by key."""
         return {
             key: sensor
             for command in self.sensor_commands
             for key, sensor in command.sensors_by_key.items()
         }
 
-    def set_service_commands(self, service_commands: list[ServiceCommand]) -> None:
-        """Set service commands."""
-        self.service_commands = []
-        for command in service_commands:
-            self.add_service_command(command)
+    def set_action_commands(self, action_commands: list[ActionCommand]) -> None:
+        """Set action commands."""
+        self.action_commands = []
+        for command in action_commands:
+            self.add_action_command(command)
 
     def set_sensor_commands(self, sensor_commands: list[SensorCommand]) -> None:
         """Set sensor commands."""
         self.sensor_commands = []
         for command in sensor_commands:
             self.add_sensor_command(command)
 
-    def add_service_command(self, command: ServiceCommand) -> None:
-        """Add a service command.
+    def add_action_command(self, command: ActionCommand) -> None:
+        """Add an action command.
 
-        Remove existing service command with the same key.
+        Remove existing action command with the same key.
         """
-        if command.key in self.service_commands_by_key:
-            self.remove_service_command(command.key)
+        if command.key in self.action_commands_by_key:
+            self.remove_action_command(command.key)
 
-        self.service_commands.append(deepcopy(command))
+        self.action_commands.append(deepcopy(command))
 
     def add_sensor_command(self, command: SensorCommand) -> None:
         """Add a sensor command.
 
         Remove existing sensors with the same keys.
         """
         for sensor in command.sensors:
             if sensor.key in self.sensors_by_key:
                 self.remove_sensor(sensor.key)
 
         self.sensor_commands.append(deepcopy(command))
 
-    def get_service_command(self, key: str) -> ServiceCommand:
-        """Get a service command."""
-        return self.service_commands_by_key[key]
+    def get_action_command(self, key: str) -> ActionCommand:
+        """Get an action command."""
+        return self.action_commands_by_key[key]
 
     def get_sensor_command(self, key: str) -> SensorCommand:
         """Get a sensor command."""
         return self.sensor_commands_by_sensor_key[key]
 
     def get_sensor(self, key: str) -> Sensor:
         """Get a sensor."""
         return self.sensors_by_key[key]
 
-    def remove_service_command(self, key: str) -> None:
-        """Remove a service command."""
-        command = self.get_service_command(key)
-        self.service_commands.remove(command)
+    def remove_action_command(self, key: str) -> None:
+        """Remove an action command."""
+        command = self.get_action_command(key)
+        self.action_commands.remove(command)
 
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor.
 
         Remove the sensor command as well if it doesnt have any other sensors.
         """
         command = self.get_sensor_command(key)
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/const.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-class ServiceKey:
+class ActionKey:
     TURN_OFF = "turn_off"
     RESTART = "restart"
 
 
-class ServiceName:
+class ActionName:
     TURN_OFF = "Turn off"
     RESTART = "Restart"
 
 
 class SensorKey:
     INTERFACE = "interface"
     MAC_ADDRESS = "mac_address"
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/linux.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/linux.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from ..command import Command, SensorCommand, ServiceCommand
+from ..command import ActionCommand, Command, SensorCommand
 from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
-from .const import SensorKey, SensorName, ServiceKey, ServiceName
+from .const import ActionKey, ActionName, SensorKey, SensorName
 
 linux = CommandSet(
     "Linux",
     [
-        ServiceCommand(
+        ActionCommand(
             "/sbin/shutdown -h now",
-            ServiceName.TURN_OFF,
-            ServiceKey.TURN_OFF,
+            ActionName.TURN_OFF,
+            ActionKey.TURN_OFF,
         ),
-        ServiceCommand(
+        ActionCommand(
             "/sbin/shutdown -r now",
-            ServiceName.RESTART,
-            ServiceKey.RESTART,
+            ActionName.RESTART,
+            ActionKey.RESTART,
         ),
     ],
     [
         SensorCommand(
             "cat /sys/class/net/{interface}/address",
             [
                 Sensor(
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_cmd.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from ..command import SensorCommand, ServiceCommand
+from ..command import ActionCommand, SensorCommand
 from ..command_set import CommandSet
 from ..sensor import Sensor
-from .const import SensorKey, SensorName, ServiceKey, ServiceName
+from .const import ActionKey, ActionName, SensorKey, SensorName
 
 windows_cmd = CommandSet(
     "Windows",
     [
-        ServiceCommand(
+        ActionCommand(
             "shutdown -t 0",
-            ServiceName.TURN_OFF,
-            ServiceKey.TURN_OFF,
+            ActionName.TURN_OFF,
+            ActionKey.TURN_OFF,
         ),
-        ServiceCommand(
+        ActionCommand(
             "shutdown -r -t 0",
-            ServiceName.RESTART,
-            ServiceKey.RESTART,
+            ActionName.RESTART,
+            ActionKey.RESTART,
         ),
     ],
     [
         # TODO: MAC_ADDRESS
         # TODO: WOL_SUPPORT
         # TODO: INTERFACE
         SensorCommand(
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_ps.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/default_command_sets/windows_ps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from ..command import SensorCommand, ServiceCommand
+from ..command import ActionCommand, SensorCommand
 from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
-from .const import SensorKey, SensorName, ServiceKey, ServiceName
+from .const import ActionKey, ActionName, SensorKey, SensorName
 
 windows_ps = CommandSet(
     "Windows (Power Shell)",
     [
-        ServiceCommand(
+        ActionCommand(
             "Stop-Computer -Force",
-            ServiceName.TURN_OFF,
-            ServiceKey.TURN_OFF,
+            ActionName.TURN_OFF,
+            ActionKey.TURN_OFF,
         ),
-        ServiceCommand(
+        ActionCommand(
             "Restart-Computer -Force",
-            ServiceName.RESTART,
-            ServiceKey.RESTART,
+            ActionName.RESTART,
+            ActionKey.RESTART,
         ),
     ],
     [
         # TODO: MAC_ADDRESS
         # TODO: WOL_SUPPORT
         # TODO: INTERFACE
         SensorCommand(
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/manager.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ) -> None:
         Locker.__init__(self)
         CommandSet.__init__(self, name)
         self.command_timeout = command_timeout
         self.logger = logger
 
         if command_set:
-            self.set_service_commands(command_set.service_commands)
+            self.set_action_commands(command_set.action_commands)
             self.set_sensor_commands(command_set.sensor_commands)
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         """Execute a command string.
 
@@ -51,24 +51,24 @@
 
         Raises:
             CommandFormatError
             CommandExecuteError
         """
         await command.async_execute(self, context)
 
-    async def async_call_service(
+    async def async_run_action(
         self, key: str, context: dict | None = None
     ) -> CommandOutput:
-        """Call a service.
+        """Run an action.
 
         Raises:
             CommandFormatError
             CommandExecuteError
         """
-        command = self.get_service_command(key)
+        command = self.get_action_command(key)
         return await self.async_execute_command(command, context)
 
     async def async_poll_sensor(self, key: str, *, validate: bool = False) -> Sensor:
         """Poll a sensor.
 
         Raises:
             CommandFormatError (validate)
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.6/src/ssh_remote_control/sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 
 
 class DynamicData:
     """The DynamicData class"""
 
     def __init__(
         self,
-        sensor_name: str | None,
-        sensor_key: str,
-        data_value: str,
+        parent_name: str | None,
+        parent_key: str,
+        data_value_string: str,
         data_name: str,
         data_id: str | None = None,
     ) -> None:
-        self.value_string = data_value
-        self.child_name = f"{sensor_name} {data_name}" if sensor_name else data_name
-        self.child_key = f"{sensor_key}_{name_to_key(data_name)}"
-        self.child_id = data_id or data_name
+        self.id = data_id or data_name
+        self.key = f"{parent_key}_{name_to_key(self.id)}"
+        self.name = f"{parent_name} {data_name}" if parent_name else data_name
+        self.value_string = data_value_string
 
 
 class Sensor:
     """The Sensor class."""
 
     value: Any | None = None
     last_known_value: Any | None = None
@@ -178,15 +178,15 @@
         dynamic_data_list = [
             DynamicData(self.name, self.key, *data_items)
             for data_items in [line.split(self.separator, 2) for line in data]
             if len(data_items) >= 2
         ]
 
         dynamic_data_by_key = {
-            dynamic_data.child_key: dynamic_data for dynamic_data in dynamic_data_list
+            dynamic_data.key: dynamic_data for dynamic_data in dynamic_data_list
         }
 
         for key, dynamic_data in dynamic_data_by_key.items():
             if key not in self.children_by_key:
                 self.add_child(dynamic_data)
 
         for child in self.value:
@@ -197,17 +197,17 @@
                 self.remove_child(child)
 
         self.on_update.notify(self)
 
     def add_child(self, dynamic_data: DynamicData) -> None:
         """Add a child."""
         child = Sensor(
-            dynamic_data.child_name,
-            dynamic_data.child_key,
-            dynamic_data.child_id,
+            dynamic_data.name,
+            dynamic_data.key,
+            dynamic_data.id,
             value_type=self.value_type,
             value_unit=self.value_unit,
             value_renderer=self.value_renderer,
             switch_on=self.switch_on,
             switch_off=self.switch_off,
             payload_on=self.payload_on,
             payload_off=self.payload_off,
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-remote-control
-Version: 0.1.5
+Version: 0.1.6
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.6/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

