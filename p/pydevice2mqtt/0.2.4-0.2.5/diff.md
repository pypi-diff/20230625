# Comparing `tmp/pydevice2mqtt-0.2.4.tar.gz` & `tmp/pydevice2mqtt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydevice2mqtt-0.2.4.tar", last modified: Thu Apr 27 19:18:04 2023, max compression
+gzip compressed data, was "pydevice2mqtt-0.2.5.tar", last modified: Sun Jun 25 19:02:38 2023, max compression
```

## Comparing `pydevice2mqtt-0.2.4.tar` & `pydevice2mqtt-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.4/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.4/.gitignore
--rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.4/LICENSE
--rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.4/README.md
--rw-r--r--   0        0        0     1019 2023-04-27 19:17:58.434145 pydevice2mqtt-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.4/src/pydevice2mqtt/__init__.py
--rw-r--r--   0        0        0     8729 2023-04-27 14:59:29.570632 pydevice2mqtt-0.2.4/src/pydevice2mqtt/pydevice2mqtt.py
--rw-r--r--   0        0        0    19853 2023-04-27 19:15:40.305270 pydevice2mqtt-0.2.4/src/pydevice2mqtt/remote_devices.py
--rw-r--r--   0        0        0     7258 2023-04-27 15:14:55.747429 pydevice2mqtt-0.2.4/test/pydevice2mqtt_test.py
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.5/README.md
+-rw-r--r--   0        0        0     1019 2023-06-25 19:02:04.200555 pydevice2mqtt-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.5/src/pydevice2mqtt/__init__.py
+-rw-r--r--   0        0        0     8729 2023-04-27 14:59:29.570632 pydevice2mqtt-0.2.5/src/pydevice2mqtt/pydevice2mqtt.py
+-rw-r--r--   0        0        0    20866 2023-06-25 11:43:07.472319 pydevice2mqtt-0.2.5/src/pydevice2mqtt/remote_devices.py
+-rw-r--r--   0        0        0     8692 2023-06-25 11:45:40.361927 pydevice2mqtt-0.2.5/test/pydevice2mqtt_test.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.5/PKG-INFO
```

### Comparing `pydevice2mqtt-0.2.4/.github/workflows/python-app.yml` & `pydevice2mqtt-0.2.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.4/.gitignore` & `pydevice2mqtt-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.4/LICENSE` & `pydevice2mqtt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.4/README.md` & `pydevice2mqtt-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.4/pyproject.toml` & `pydevice2mqtt-0.2.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 2e0d 0a20 2020 2053 7570 706f 7274 7320  ...    Supports 
 00000090: 7468 6520 4861 7373 6f20 6175 746f 2063  the Hasso auto c
 000000a0: 6f6e 6669 6775 7261 7469 6f6e 2070 726f  onfiguration pro
 000000b0: 746f 636f 6c0d 0a20 2020 2027 2727 0d0a  tocol..    '''..
 000000c0: 2020 2020 6c69 6365 6e73 6520 3d20 7b66      license = {f
 000000d0: 696c 6520 3d20 224c 4943 454e 5345 227d  ile = "LICENSE"}
 000000e0: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
-000000f0: 2230 2e32 2e34 220d 0a20 2020 2072 6561  "0.2.4"..    rea
+000000f0: 2230 2e32 2e35 220d 0a20 2020 2072 6561  "0.2.5"..    rea
 00000100: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 00000110: 220d 0a20 2020 2072 6571 7569 7265 732d  "..    requires-
 00000120: 7079 7468 6f6e 203d 2022 3e3d 332e 3722  python = ">=3.7"
 00000130: 0d0a 2020 2020 6175 7468 6f72 7320 3d20  ..    authors = 
 00000140: 5b7b 6e61 6d65 3d22 4869 6768 496d 7022  [{name="HighImp"
 00000150: 2c20 656d 6169 6c3d 2241 6e79 4869 6768  , email="AnyHigh
 00000160: 5a40 676d 6169 6c2e 636f 6d22 7d5d 0d0a  Z@gmail.com"}]..
```

### Comparing `pydevice2mqtt-0.2.4/src/pydevice2mqtt/pydevice2mqtt.py` & `pydevice2mqtt-0.2.5/src/pydevice2mqtt/pydevice2mqtt.py`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.4/src/pydevice2mqtt/remote_devices.py` & `pydevice2mqtt-0.2.5/src/pydevice2mqtt/remote_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,43 @@
             return
 
         self._update(channel_name="state_topic",
                      message=json.dumps({"value": value}))
         self._last_value = value
 
 
+class Switch(RemoteDevice):
+    """Arbitrary Switch
+    Switches are by now the only devices who can trigger
+    an alexa routine. Its possible to connect a function to set or get the value,
+    but its written to use devices as boolean variables
+    """
+
+    def __init__(self, device_settings, mqtt_settings):
+        device_settings["device_class"] = "switch"
+        super().__init__(device_settings, mqtt_settings)
+        self._state: str = "OFF"
+        self._add_channel(channel_name="command_topic",
+                          sub_topic="set",
+                          on_message=self.set_value)
+        self._config["payload_off"] = "OFF"
+        self._config["payload_on"] = "ON"
+
+    def set_value(self, value):
+        if value and value != "OFF":
+            self._state = "ON"
+        else:
+            self._state = "OFF"
+        self._update(channel_name="state_topic",
+                     message=self._state)
+
+    def get_value(self):
+        return self._state
+
+
 class RpiGpio(RemoteDevice):
     """
     Raspberry PI Remote Gpio device
     Remote device to configure and control GPIOs of an Raspberry Pi via MQTT and
     especially in hassio via auto configuration, supporting switch and binary sensor format
     """
```

### Comparing `pydevice2mqtt-0.2.4/test/pydevice2mqtt_test.py` & `pydevice2mqtt-0.2.5/test/pydevice2mqtt_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -128,14 +128,43 @@
     assert len(mqtt_client.mock_calls) == 4
     set_value_call_kwargs = mqtt_client.mock_calls[-1].kwargs
     try:
         assert set_value_call_kwargs["payload"] == '{"value": 1}'
     except TypeError:
         print(set_value_call_kwargs)
 
+def test_switch(mocker):
+    import pydevice2mqtt
+    mqtt_client: MagicMock = mocker.patch("pydevice2mqtt.pydevice2mqtt.mqtt.Client")
+    mocker.patch("pydevice2mqtt.remote_devices.espeak")
+    mocker.patch("pydevice2mqtt.remote_devices.gpiozero")
+
+    device_class = {"Switch": pydevice2mqtt.remote_devices.Switch}
+    my_bridge: pydevice2mqtt.DeviceBridge = create_device_bridge(mocked_module=pydevice2mqtt,
+                                                                 device_classes=device_class)
+    switch_instance: pydevice2mqtt.remote_devices.Switch
+    expected_dev_id = f"Switch_{EXAMPLE_DATA[str]}"
+    switch_instance = my_bridge.get_devices()[expected_dev_id]
+    assert switch_instance.get_id() == expected_dev_id
+    assert switch_instance.get_object_id() == EXAMPLE_DATA[str]
+    assert switch_instance.get_name() == EXAMPLE_DATA[str]
+    assert len(mqtt_client.mock_calls) == 3
+    for set_value in ["ON", 1, True]:
+        switch_instance.set_value(set_value)
+        assert switch_instance.get_value() == "ON"
+        switch_instance.set_value("OFF")
+        assert switch_instance.get_value() == "OFF"
+
+    for set_value in ["OFF", 0, False, None]:
+        switch_instance.set_value(set_value)
+        assert switch_instance.get_value() == "OFF"
+        switch_instance.set_value("ON")
+        assert switch_instance.get_value() == "ON"
+
+    print(switch_instance.get_discovery())
 
 def test_additional_config(mocker):
     import pydevice2mqtt
 
     mocker.patch("pydevice2mqtt.pydevice2mqtt.mqtt.Client")
     mocker.patch("pydevice2mqtt.remote_devices.espeak")
     mocker.patch("pydevice2mqtt.remote_devices.gpiozero")
```

### Comparing `pydevice2mqtt-0.2.4/PKG-INFO` & `pydevice2mqtt-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydevice2mqtt
-Version: 0.2.4
+Version: 0.2.5
 Summary:     This project provides a simplified control of devices via MQTT.
             Supports the Hasso auto configuration protocol
             
 Keywords: hassio,mqtt,homeassistent,homeautomation
 Author-email: HighImp <AnyHighZ@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

