# Comparing `tmp/ssh_remote_control-0.1.4.tar.gz` & `tmp/ssh_remote_control-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.4.tar", last modified: Thu Jun 22 08:15:17 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.5.tar", last modified: Sat Jun 24 10:04:33 2023, max compression
```

## Comparing `ssh_remote_control-0.1.4.tar` & `ssh_remote_control-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.497905 ssh_remote_control-0.1.4/
--rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1569 2023-06-22 08:15:17.495635 ssh_remote_control-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      973 2023-06-20 06:12:24.000000 ssh_remote_control-0.1.4/README.md
--rw-rw-rw-   0        0        0      846 2023-06-22 08:13:58.000000 ssh_remote_control-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 08:15:17.498638 ssh_remote_control-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.332215 ssh_remote_control-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.395080 ssh_remote_control-0.1.4/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10675 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6576 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/command.py
--rw-rw-rw-   0        0        0     2882 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/command_set.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.492650 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/
--rw-rw-rw-   0        0        0      163 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/const.py
--rw-rw-rw-   0        0        0     3987 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/linux.py
--rw-rw-rw-   0        0        0     3822 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_cmd.py
--rw-rw-rw-   0        0        0     4087 2023-06-22 08:11:22.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_ps.py
--rw-rw-rw-   0        0        0      645 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      159 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     3885 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     6667 2023-06-22 08:11:21.000000 ssh_remote_control-0.1.4/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-22 08:15:17.465634 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1569 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-22 08:15:17.000000 ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.629782 ssh_remote_control-0.1.5/
+-rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-24 10:04:33.628780 ssh_remote_control-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-20 06:12:24.000000 ssh_remote_control-0.1.5/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-24 10:00:35.000000 ssh_remote_control-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 10:04:33.630780 ssh_remote_control-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.530780 ssh_remote_control-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.573779 ssh_remote_control-0.1.5/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10709 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     6661 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/command.py
+-rw-rw-rw-   0        0        0     3533 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/command_set.py
+drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.625786 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/
+-rw-rw-rw-   0        0        0      163 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/const.py
+-rw-rw-rw-   0        0        0     3987 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/linux.py
+-rw-rw-rw-   0        0        0     3822 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_cmd.py
+-rw-rw-rw-   0        0        0     4087 2023-06-24 09:50:12.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_ps.py
+-rw-rw-rw-   0        0        0      645 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      222 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     3830 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     6787 2023-06-24 09:50:11.000000 ssh_remote_control-0.1.5/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-24 10:04:33.611776 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 10:04:33.000000 ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.4/LICENSE` & `ssh_remote_control-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/PKG-INFO` & `ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh_remote_control
-Version: 0.1.4
+Name: ssh-remote-control
+Version: 0.1.5
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.4/README.md` & `ssh_remote_control-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/pyproject.toml` & `ssh_remote_control-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     CommandOutput,
     SensorCommand,
     ServiceCommand,
 )
 from .command_set import CommandSet
 from .default_command_sets import SensorKey, ServiceKey
 from .event import Event
+from .helpers import name_to_key
 from .manager import DEFAULT_COMMAND_TIMEOUT, CommandExecuteError, Manager
 from .sensor import DynamicSensor, Sensor
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_SSH_PORT = 22
 DEFAULT_PING_TIMEOUT = 4
@@ -68,43 +69,43 @@
     """The Remote class."""
 
     def __init__(
         self,
         host: str,
         *,
         name: str | None = None,
-        command_set: CommandSet | None = None,
+        mac_address: str | None = None,
         add_host_keys: bool = DEFAULT_ADD_HOST_KEYS,
         ssh_port: int = DEFAULT_SSH_PORT,
         ssh_user: str | None = None,
         ssh_password: str | None = None,
         ssh_key_file: str | None = None,
         ssh_host_keys_file: str | None = None,
         ssh_timeout: int = DEFAULT_SSH_TIMEOUT,
         ping_timeout: int = DEFAULT_PING_TIMEOUT,
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
+        command_set: CommandSet | None = None,
         allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
-        mac_address: str | None = None,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         super().__init__(
             name=name or host,
-            command_set=command_set,
             command_timeout=command_timeout,
+            command_set=command_set,
             logger=logger,
         )
         self.host = host
+        self._mac_address = mac_address
         self.ssh_port = ssh_port
         self.ssh_user = ssh_user
         self.ssh_password = ssh_password
         self.ssh_key_file = ssh_key_file
         self.ssh_timeout = ssh_timeout
         self.ping_timeout = ping_timeout
         self.allow_turn_off = allow_turn_off
-        self._mac_address = mac_address
         self.state = State(self)
         self._ssh_client = paramiko.SSHClient()
         self._ssh_client.set_log_channel(self.logger.name)
         self._ssh_client.load_system_host_keys()
         self._ssh_client.set_missing_host_key_policy(
             paramiko.AutoAddPolicy if add_host_keys else CustomRejectPolicy
         )
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from .helpers import name_to_key
 from .sensor import DynamicSensor, Sensor
 
 if TYPE_CHECKING:
     from .manager import Manager
 
+PLACEHOLDER_KEY = "_"
+
 
 @dataclass(frozen=True)
 class CommandOutput:
     """The CommandOutput class."""
 
     timestamp: float
     stdout: list[str] | None = None
@@ -120,15 +122,15 @@
 
 class ServiceCommand(Command):
     """The ServiceCommand class."""
 
     def __init__(
         self,
         string: str,
-        name: str,
+        name: str | None = None,
         key: str | None = None,
         *,
         timeout: float | None = None,
         renderer: Callable[[str], str] | None = None,
         options: dict | None = None,
     ) -> None:
         super().__init__(string, timeout=timeout, renderer=renderer)
@@ -156,15 +158,15 @@
         self.interval = interval
 
     @property
     def sensors_by_key(self) -> dict[str, Sensor]:
         """Sensors by key."""
         result = {}
         for sensor in self.sensors:
-            if sensor.key:
+            if sensor.key != PLACEHOLDER_KEY:
                 result.update(
                     {sensor.key: sensor, **sensor.children_by_key}
                     if isinstance(sensor, DynamicSensor)
                     else {sensor.key: sensor}
                 )
         return result
 
@@ -181,15 +183,16 @@
         return self.last_update is None or (
             self.interval and time() - self.last_update >= self.interval
         )
 
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor."""
         self.sensors = [
-            Sensor("") if sensor.key == key else sensor for sensor in self.sensors
+            Sensor(key=PLACEHOLDER_KEY) if sensor.key == key else sensor
+            for sensor in self.sensors
         ]
 
     def set_sensor_values(self, output: CommandOutput | None) -> None:
         """Set sensor values."""
         if output and output.code == 0:
             self.last_update = output.timestamp
             data = output.stdout
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/command_set.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/command_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,84 @@
+from copy import deepcopy
+
 from .command import SensorCommand, ServiceCommand
 from .sensor import Sensor
 
 
 class CommandSet:
     """The CommandSet class."""
 
+    service_commands: list[ServiceCommand]
+    sensor_commands: list[SensorCommand]
+
     def __init__(
         self,
         name: str,
         service_commands: list[ServiceCommand] | None = None,
         sensor_commands: list[SensorCommand] | None = None,
     ) -> None:
         self.name = name
-        self.service_commands = service_commands or []
-        self.sensor_commands = sensor_commands or []
+        self.set_service_commands(service_commands or [])
+        self.set_sensor_commands(sensor_commands or [])
 
     @property
     def service_commands_by_key(self) -> dict[str, ServiceCommand]:
         """Service commands by key."""
         return {command.key: command for command in self.service_commands}
 
     @property
     def sensor_commands_by_sensor_key(self) -> dict[str, SensorCommand]:
         """Sensor commands by sensor key."""
-        result = {}
-        for command in self.sensor_commands:
-            result.update({key: command for key in command.sensors_by_key})
-        return result
+        return {
+            key: command
+            for command in self.sensor_commands
+            for key in command.sensors_by_key
+        }
 
     @property
     def sensors_by_key(self) -> dict[str, Sensor]:
         """Sensors by key."""
-        result = {}
-        for command in self.sensor_commands:
-            result.update(command.sensors_by_key)
-        return result
+        return {
+            key: sensor
+            for command in self.sensor_commands
+            for key, sensor in command.sensors_by_key.items()
+        }
+
+    def set_service_commands(self, service_commands: list[ServiceCommand]) -> None:
+        """Set service commands."""
+        self.service_commands = []
+        for command in service_commands:
+            self.add_service_command(command)
+
+    def set_sensor_commands(self, sensor_commands: list[SensorCommand]) -> None:
+        """Set sensor commands."""
+        self.sensor_commands = []
+        for command in sensor_commands:
+            self.add_sensor_command(command)
 
     def add_service_command(self, command: ServiceCommand) -> None:
         """Add a service command.
 
         Remove existing service command with the same key.
         """
         if command.key in self.service_commands_by_key:
             self.remove_service_command(command.key)
 
-        self.service_commands.append(command)
+        self.service_commands.append(deepcopy(command))
 
     def add_sensor_command(self, command: SensorCommand) -> None:
         """Add a sensor command.
 
         Remove existing sensors with the same keys.
         """
         for sensor in command.sensors:
             if sensor.key in self.sensors_by_key:
                 self.remove_sensor(sensor.key)
 
-        self.sensor_commands.append(command)
+        self.sensor_commands.append(deepcopy(command))
 
     def get_service_command(self, key: str) -> ServiceCommand:
         """Get a service command."""
         return self.service_commands_by_key[key]
 
     def get_sensor_command(self, key: str) -> SensorCommand:
         """Get a sensor command."""
@@ -73,14 +92,14 @@
         """Remove a service command."""
         command = self.get_service_command(key)
         self.service_commands.remove(command)
 
     def remove_sensor(self, key: str) -> None:
         """Remove a sensor.
 
-        Remove the sensor command if it doesnt have any other sensors.
+        Remove the sensor command as well if it doesnt have any other sensors.
         """
         command = self.get_sensor_command(key)
         command.remove_sensor(key)
 
         if not command.sensors_by_key:
             self.sensor_commands.remove(command)
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/const.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/linux.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/linux.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_cmd.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/default_command_sets/windows_ps.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/default_command_sets/windows_ps.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/event.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/manager.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from collections.abc import Sequence
-from copy import deepcopy
 import logging
 
 from .command import Command, CommandExecuteError, CommandFormatError, CommandOutput
 from .command_set import CommandSet
 from .locker import Locker
 from .sensor import Sensor
 
@@ -18,28 +17,27 @@
 class Manager(CommandSet, Locker):
     """The Manager class."""
 
     def __init__(
         self,
         *,
         name: str = DEFAULT_NAME,
-        command_set: CommandSet | None = None,
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
+        command_set: CommandSet | None = None,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         Locker.__init__(self)
-        CommandSet.__init__(
-            self,
-            name,
-            deepcopy(command_set.service_commands) if command_set else None,
-            deepcopy(command_set.sensor_commands) if command_set else None,
-        )
+        CommandSet.__init__(self, name)
         self.command_timeout = command_timeout
         self.logger = logger
 
+        if command_set:
+            self.set_service_commands(command_set.service_commands)
+            self.set_sensor_commands(command_set.sensor_commands)
+
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         """Execute a command string.
 
         Raises:
             CommandExecuteError
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.5/src/ssh_remote_control/sensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,36 +40,35 @@
 
 
 class DynamicData:
     """The DynamicData class"""
 
     def __init__(
         self,
-        sensor_name: str,
+        sensor_name: str | None,
         sensor_key: str,
         data_value: str,
         data_name: str,
         data_id: str | None = None,
     ) -> None:
-        data_key = name_to_key(data_name)
         self.value_string = data_value
-        self.child_name = f"{sensor_name} {data_name}"
-        self.child_key = f"{sensor_key}_{data_key}"
-        self.child_id = data_id or data_key
+        self.child_name = f"{sensor_name} {data_name}" if sensor_name else data_name
+        self.child_key = f"{sensor_key}_{name_to_key(data_name)}"
+        self.child_id = data_id or data_name
 
 
 class Sensor:
     """The Sensor class."""
 
     value: Any | None = None
     last_known_value: Any | None = None
 
     def __init__(
         self,
-        name: str,
+        name: str | None = None,
         key: str | None = None,
         child_id: str | None = None,
         *,
         value_type: type | None = None,
         value_unit: str | None = None,
         value_renderer: Callable[[str], str] | None = None,
         switch_on: Command | None = None,
@@ -130,15 +129,15 @@
 class DynamicSensor(Sensor):
     """The DynamicSensor class."""
 
     value: list[Sensor]
 
     def __init__(
         self,
-        name: str,
+        name: str | None = None,
         key: str | None = None,
         *,
         value_type: type | None = None,
         value_unit: str | None = None,
         value_renderer: Callable[[str], str] | None = None,
         switch_on: str | None = None,
         switch_off: str | None = None,
@@ -206,14 +205,16 @@
             dynamic_data.child_key,
             dynamic_data.child_id,
             value_type=self.value_type,
             value_unit=self.value_unit,
             value_renderer=self.value_renderer,
             switch_on=self.switch_on,
             switch_off=self.switch_off,
+            payload_on=self.payload_on,
+            payload_off=self.payload_off,
             options=self.options,
         )
         self.value.append(child)
         self.on_child_added.notify(self, child)
 
     def remove_child(self, child: Sensor) -> None:
         """Remove a child."""
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/PKG-INFO` & `ssh_remote_control-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh-remote-control
-Version: 0.1.4
+Name: ssh_remote_control
+Version: 0.1.5
 Summary: Control and monitor remote devices through SSH
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-remote-control
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-remote-control/issues
 Keywords: ssh,command line,remote control
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_remote_control-0.1.4/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.5/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

