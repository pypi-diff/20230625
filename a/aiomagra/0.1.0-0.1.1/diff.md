# Comparing `tmp/aiomagra-0.1.0.tar.gz` & `tmp/aiomagra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomagra-0.1.0.tar", max compression
+gzip compressed data, was "aiomagra-0.1.1.tar", max compression
```

## Comparing `aiomagra-0.1.0.tar` & `aiomagra-0.1.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0       12 2023-06-25 13:29:06.484907 aiomagra-0.1.0/README.md
--rw-r--r--   0        0        0      282 2023-06-25 13:46:40.994049 aiomagra-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/__init__.py
--rw-r--r--   0        0        0      366 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/accelerometer.proto
--rw-r--r--   0        0        0     1498 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/accelerometer_pb2.py
--rw-r--r--   0        0        0      745 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/addon.proto
--rw-r--r--   0        0        0     2400 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/addon_pb2.py
--rw-r--r--   0        0        0      566 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/admin.proto
--rw-r--r--   0        0        0     1864 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/admin_pb2.py
--rw-r--r--   0        0        0      460 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/battery.proto
--rw-r--r--   0        0        0     1649 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/battery_pb2.py
--rw-r--r--   0        0        0      417 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/ble.proto
--rw-r--r--   0        0        0     1497 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/ble_pb2.py
--rw-r--r--   0        0        0      507 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/bsensor.proto
--rw-r--r--   0        0        0     1860 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/bsensor_pb2.py
--rw-r--r--   0        0        0      894 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/carbon_dioxide.proto
--rw-r--r--   0        0        0     2356 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/carbon_dioxide_pb2.py
--rw-r--r--   0        0        0     1326 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/carbon_monoxide.proto
--rw-r--r--   0        0        0     3383 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/carbon_monoxide_pb2.py
--rw-r--r--   0        0        0     5204 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/client.py
--rw-r--r--   0        0        0      778 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/color.proto
--rw-r--r--   0        0        0     2288 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/color_pb2.py
--rw-r--r--   0        0        0     2116 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/configuration.proto
--rw-r--r--   0        0        0     4789 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/configuration_pb2.py
--rw-r--r--   0        0        0       79 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/const.py
--rw-r--r--   0        0        0     3883 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/devices.proto
--rw-r--r--   0        0        0    10232 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/devices_pb2.py
--rw-r--r--   0        0        0      327 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/door.proto
--rw-r--r--   0        0        0     1323 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/door_pb2.py
--rw-r--r--   0        0        0      276 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/doorbell.proto
--rw-r--r--   0        0        0     1313 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/doorbell_pb2.py
--rw-r--r--   0        0        0      329 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/emergency.proto
--rw-r--r--   0        0        0     1359 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/emergency_pb2.py
--rw-r--r--   0        0        0     1349 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/firmware.proto
--rw-r--r--   0        0        0     3574 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/firmware_pb2.py
--rw-r--r--   0        0        0      272 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/flood.proto
--rw-r--r--   0        0        0     1281 2023-06-25 13:29:06.474907 aiomagra-0.1.0/src/aiomagra/flood_pb2.py
--rw-r--r--   0        0        0      622 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/gate.proto
--rw-r--r--   0        0        0     1949 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/gate_pb2.py
--rw-r--r--   0        0        0      617 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/gateway.proto
--rw-r--r--   0        0        0     2049 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/gateway_pb2.py
--rw-r--r--   0        0        0      300 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/heartbeat.proto
--rw-r--r--   0        0        0     1253 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/heartbeat_pb2.py
--rw-r--r--   0        0        0      424 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/info.proto
--rw-r--r--   0        0        0     1494 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/info_pb2.py
--rw-r--r--   0        0        0     1080 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/level.proto
--rw-r--r--   0        0        0     2779 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/level_pb2.py
--rw-r--r--   0        0        0      639 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/lock.proto
--rw-r--r--   0        0        0     1991 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/lock_pb2.py
--rw-r--r--   0        0        0      405 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/messaging.proto
--rw-r--r--   0        0        0     1459 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/messaging_pb2.py
--rw-r--r--   0        0        0      678 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/metadata.proto
--rw-r--r--   0        0        0     2250 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/metadata_pb2.py
--rw-r--r--   0        0        0      689 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/meter.proto
--rw-r--r--   0        0        0     2196 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/meter_pb2.py
--rw-r--r--   0        0        0      303 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/mqtt.proto
--rw-r--r--   0        0        0     1212 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/mqtt_pb2.py
--rw-r--r--   0        0        0      647 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/power_source.proto
--rw-r--r--   0        0        0     1908 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/power_source_pb2.py
--rw-r--r--   0        0        0    11060 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/pubsub.proto
--rw-r--r--   0        0        0    18842 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/pubsub_pb2.py
--rw-r--r--   0        0        0      622 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/remote.proto
--rw-r--r--   0        0        0     2030 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/remote_pb2.py
--rw-r--r--   0        0        0     3457 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/reports.proto
--rw-r--r--   0        0        0     6738 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/reports_pb2.py
--rw-r--r--   0        0        0      724 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/roller_shutter.proto
--rw-r--r--   0        0        0     2150 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/roller_shutter_pb2.py
--rw-r--r--   0        0        0      357 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/seismic.proto
--rw-r--r--   0        0        0     1434 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/seismic_pb2.py
--rw-r--r--   0        0        0      410 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/sensor.proto
--rw-r--r--   0        0        0     1595 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/sensor_pb2.py
--rw-r--r--   0        0        0     2040 2023-06-25 13:29:06.478240 aiomagra-0.1.0/src/aiomagra/siren.proto
--rw-r--r--   0        0        0     5427 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/siren_pb2.py
--rw-r--r--   0        0        0      827 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/smoke.proto
--rw-r--r--   0        0        0     2224 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/smoke_pb2.py
--rw-r--r--   0        0        0      510 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/status.proto
--rw-r--r--   0        0        0     1802 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/status_pb2.py
--rw-r--r--   0        0        0      574 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/structure.proto
--rw-r--r--   0        0        0     1909 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/structure_pb2.py
--rw-r--r--   0        0        0      562 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/switch.proto
--rw-r--r--   0        0        0     1855 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/switch_pb2.py
--rw-r--r--   0        0        0      327 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/tamper.proto
--rw-r--r--   0        0        0     1328 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/tamper_pb2.py
--rw-r--r--   0        0        0      222 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/taptap.proto
--rw-r--r--   0        0        0     1096 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/taptap_pb2.py
--rw-r--r--   0        0        0      575 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/temperature.proto
--rw-r--r--   0        0        0     1890 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/temperature_pb2.py
--rw-r--r--   0        0        0     2051 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/thermostat.proto
--rw-r--r--   0        0        0     5104 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/thermostat_pb2.py
--rw-r--r--   0        0        0      562 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/ultraviolet.proto
--rw-r--r--   0        0        0     1869 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/ultraviolet_pb2.py
--rw-r--r--   0        0        0     8927 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/units.proto
--rw-r--r--   0        0        0     1627 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/units_pb2.py
--rw-r--r--   0        0        0      390 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/websocket.proto
--rw-r--r--   0        0        0     1398 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/websocket_pb2.py
--rw-r--r--   0        0        0     1130 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/wifi.proto
--rw-r--r--   0        0        0     3028 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/wifi_pb2.py
--rw-r--r--   0        0        0      909 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/zigbee.proto
--rw-r--r--   0        0        0     2577 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/zigbee_pb2.py
--rw-r--r--   0        0        0     6499 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/zwave.proto
--rw-r--r--   0        0        0    15749 2023-06-25 13:29:06.481573 aiomagra-0.1.0/src/aiomagra/zwave_pb2.py
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 aiomagra-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-06-25 13:29:06.484907 aiomagra-0.1.1/README.md
+-rw-r--r--   0        0        0      282 2023-06-25 14:02:45.807002 aiomagra-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/__init__.py
+-rw-r--r--   0        0        0      366 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/accelerometer.proto
+-rw-r--r--   0        0        0     1498 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/accelerometer_pb2.py
+-rw-r--r--   0        0        0      745 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/addon.proto
+-rw-r--r--   0        0        0     2400 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/addon_pb2.py
+-rw-r--r--   0        0        0      566 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/admin.proto
+-rw-r--r--   0        0        0     1864 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/admin_pb2.py
+-rw-r--r--   0        0        0      460 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/battery.proto
+-rw-r--r--   0        0        0     1649 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/battery_pb2.py
+-rw-r--r--   0        0        0      417 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/ble.proto
+-rw-r--r--   0        0        0     1497 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/ble_pb2.py
+-rw-r--r--   0        0        0      507 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/bsensor.proto
+-rw-r--r--   0        0        0     1860 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/bsensor_pb2.py
+-rw-r--r--   0        0        0      894 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_dioxide.proto
+-rw-r--r--   0        0        0     2356 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_dioxide_pb2.py
+-rw-r--r--   0        0        0     1326 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_monoxide.proto
+-rw-r--r--   0        0        0     3383 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_monoxide_pb2.py
+-rw-r--r--   0        0        0     5204 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/client.py
+-rw-r--r--   0        0        0      778 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/color.proto
+-rw-r--r--   0        0        0     2288 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/color_pb2.py
+-rw-r--r--   0        0        0     2116 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/configuration.proto
+-rw-r--r--   0        0        0     4789 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/configuration_pb2.py
+-rw-r--r--   0        0        0       79 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/const.py
+-rw-r--r--   0        0        0     3883 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/devices.proto
+-rw-r--r--   0        0        0    10232 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/devices_pb2.py
+-rw-r--r--   0        0        0      327 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/door.proto
+-rw-r--r--   0        0        0     1323 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/door_pb2.py
+-rw-r--r--   0        0        0      276 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/doorbell.proto
+-rw-r--r--   0        0        0     1313 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/doorbell_pb2.py
+-rw-r--r--   0        0        0      329 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/emergency.proto
+-rw-r--r--   0        0        0     1359 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/emergency_pb2.py
+-rw-r--r--   0        0        0     1349 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/firmware.proto
+-rw-r--r--   0        0        0     3574 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/firmware_pb2.py
+-rw-r--r--   0        0        0      272 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/flood.proto
+-rw-r--r--   0        0        0     1281 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/flood_pb2.py
+-rw-r--r--   0        0        0      622 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gate.proto
+-rw-r--r--   0        0        0     1949 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gate_pb2.py
+-rw-r--r--   0        0        0      617 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gateway.proto
+-rw-r--r--   0        0        0     2049 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gateway_pb2.py
+-rw-r--r--   0        0        0      300 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/heartbeat.proto
+-rw-r--r--   0        0        0     1253 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/heartbeat_pb2.py
+-rw-r--r--   0        0        0      424 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/info.proto
+-rw-r--r--   0        0        0     1494 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/info_pb2.py
+-rw-r--r--   0        0        0     1080 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/level.proto
+-rw-r--r--   0        0        0     2779 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/level_pb2.py
+-rw-r--r--   0        0        0      639 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/lock.proto
+-rw-r--r--   0        0        0     1991 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/lock_pb2.py
+-rw-r--r--   0        0        0      405 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/messaging.proto
+-rw-r--r--   0        0        0     1459 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/messaging_pb2.py
+-rw-r--r--   0        0        0      678 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/metadata.proto
+-rw-r--r--   0        0        0     2250 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/metadata_pb2.py
+-rw-r--r--   0        0        0      689 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/meter.proto
+-rw-r--r--   0        0        0     2196 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/meter_pb2.py
+-rw-r--r--   0        0        0      303 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/mqtt.proto
+-rw-r--r--   0        0        0     1212 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/mqtt_pb2.py
+-rw-r--r--   0        0        0      647 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/power_source.proto
+-rw-r--r--   0        0        0     1908 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/power_source_pb2.py
+-rw-r--r--   0        0        0    11060 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/pubsub.proto
+-rw-r--r--   0        0        0    18842 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/pubsub_pb2.py
+-rw-r--r--   0        0        0      622 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/remote.proto
+-rw-r--r--   0        0        0     2030 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/remote_pb2.py
+-rw-r--r--   0        0        0     3457 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/reports.proto
+-rw-r--r--   0        0        0     6738 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/reports_pb2.py
+-rw-r--r--   0        0        0      724 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/roller_shutter.proto
+-rw-r--r--   0        0        0     2150 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/roller_shutter_pb2.py
+-rw-r--r--   0        0        0      357 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/seismic.proto
+-rw-r--r--   0        0        0     1434 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/seismic_pb2.py
+-rw-r--r--   0        0        0      410 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/sensor.proto
+-rw-r--r--   0        0        0     1595 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/sensor_pb2.py
+-rw-r--r--   0        0        0     2040 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/siren.proto
+-rw-r--r--   0        0        0     5427 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/siren_pb2.py
+-rw-r--r--   0        0        0      827 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/smoke.proto
+-rw-r--r--   0        0        0     2224 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/smoke_pb2.py
+-rw-r--r--   0        0        0      510 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/status.proto
+-rw-r--r--   0        0        0     1802 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/status_pb2.py
+-rw-r--r--   0        0        0      574 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/structure.proto
+-rw-r--r--   0        0        0     1909 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/structure_pb2.py
+-rw-r--r--   0        0        0      562 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/switch.proto
+-rw-r--r--   0        0        0     1855 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/switch_pb2.py
+-rw-r--r--   0        0        0      327 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/tamper.proto
+-rw-r--r--   0        0        0     1328 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/tamper_pb2.py
+-rw-r--r--   0        0        0      222 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/taptap.proto
+-rw-r--r--   0        0        0     1096 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/taptap_pb2.py
+-rw-r--r--   0        0        0      575 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/temperature.proto
+-rw-r--r--   0        0        0     1890 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/temperature_pb2.py
+-rw-r--r--   0        0        0     2051 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/thermostat.proto
+-rw-r--r--   0        0        0     5104 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/thermostat_pb2.py
+-rw-r--r--   0        0        0      562 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/ultraviolet.proto
+-rw-r--r--   0        0        0     1869 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/ultraviolet_pb2.py
+-rw-r--r--   0        0        0     8927 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/units.proto
+-rw-r--r--   0        0        0     1627 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/units_pb2.py
+-rw-r--r--   0        0        0      390 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/websocket.proto
+-rw-r--r--   0        0        0     1398 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/websocket_pb2.py
+-rw-r--r--   0        0        0     1130 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/wifi.proto
+-rw-r--r--   0        0        0     3028 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/wifi_pb2.py
+-rw-r--r--   0        0        0      909 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zigbee.proto
+-rw-r--r--   0        0        0     2577 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zigbee_pb2.py
+-rw-r--r--   0        0        0     6499 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zwave.proto
+-rw-r--r--   0        0        0    15749 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zwave_pb2.py
+-rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 aiomagra-0.1.1/PKG-INFO
```

### Comparing `aiomagra-0.1.0/src/aiomagra/accelerometer_pb2.py` & `aiomagra-0.1.1/src/aiomagra/accelerometer_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/addon.proto` & `aiomagra-0.1.1/src/aiomagra/addon.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/addon_pb2.py` & `aiomagra-0.1.1/src/aiomagra/addon_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/admin.proto` & `aiomagra-0.1.1/src/aiomagra/admin.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/admin_pb2.py` & `aiomagra-0.1.1/src/aiomagra/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/battery_pb2.py` & `aiomagra-0.1.1/src/aiomagra/battery_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/ble_pb2.py` & `aiomagra-0.1.1/src/aiomagra/ble_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/bsensor_pb2.py` & `aiomagra-0.1.1/src/aiomagra/bsensor_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/carbon_dioxide.proto` & `aiomagra-0.1.1/src/aiomagra/carbon_dioxide.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/carbon_dioxide_pb2.py` & `aiomagra-0.1.1/src/aiomagra/carbon_dioxide_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/carbon_monoxide.proto` & `aiomagra-0.1.1/src/aiomagra/carbon_monoxide.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/carbon_monoxide_pb2.py` & `aiomagra-0.1.1/src/aiomagra/carbon_monoxide_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/client.py` & `aiomagra-0.1.1/src/aiomagra/client.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/color.proto` & `aiomagra-0.1.1/src/aiomagra/color.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/color_pb2.py` & `aiomagra-0.1.1/src/aiomagra/color_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/configuration.proto` & `aiomagra-0.1.1/src/aiomagra/configuration.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/configuration_pb2.py` & `aiomagra-0.1.1/src/aiomagra/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/devices.proto` & `aiomagra-0.1.1/src/aiomagra/devices.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/devices_pb2.py` & `aiomagra-0.1.1/src/aiomagra/devices_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/door_pb2.py` & `aiomagra-0.1.1/src/aiomagra/door_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/doorbell_pb2.py` & `aiomagra-0.1.1/src/aiomagra/doorbell_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/emergency_pb2.py` & `aiomagra-0.1.1/src/aiomagra/emergency_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/firmware.proto` & `aiomagra-0.1.1/src/aiomagra/firmware.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/firmware_pb2.py` & `aiomagra-0.1.1/src/aiomagra/firmware_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/flood_pb2.py` & `aiomagra-0.1.1/src/aiomagra/flood_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/gate.proto` & `aiomagra-0.1.1/src/aiomagra/gate.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/gate_pb2.py` & `aiomagra-0.1.1/src/aiomagra/gate_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/gateway.proto` & `aiomagra-0.1.1/src/aiomagra/gateway.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/gateway_pb2.py` & `aiomagra-0.1.1/src/aiomagra/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/heartbeat_pb2.py` & `aiomagra-0.1.1/src/aiomagra/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/info_pb2.py` & `aiomagra-0.1.1/src/aiomagra/info_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/level.proto` & `aiomagra-0.1.1/src/aiomagra/level.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/level_pb2.py` & `aiomagra-0.1.1/src/aiomagra/level_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/lock.proto` & `aiomagra-0.1.1/src/aiomagra/lock.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/lock_pb2.py` & `aiomagra-0.1.1/src/aiomagra/lock_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/messaging_pb2.py` & `aiomagra-0.1.1/src/aiomagra/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/metadata.proto` & `aiomagra-0.1.1/src/aiomagra/metadata.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/metadata_pb2.py` & `aiomagra-0.1.1/src/aiomagra/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/meter.proto` & `aiomagra-0.1.1/src/aiomagra/meter.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/meter_pb2.py` & `aiomagra-0.1.1/src/aiomagra/meter_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/mqtt_pb2.py` & `aiomagra-0.1.1/src/aiomagra/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/power_source.proto` & `aiomagra-0.1.1/src/aiomagra/power_source.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/power_source_pb2.py` & `aiomagra-0.1.1/src/aiomagra/power_source_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/pubsub.proto` & `aiomagra-0.1.1/src/aiomagra/pubsub.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/pubsub_pb2.py` & `aiomagra-0.1.1/src/aiomagra/pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/remote.proto` & `aiomagra-0.1.1/src/aiomagra/remote.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/remote_pb2.py` & `aiomagra-0.1.1/src/aiomagra/remote_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/reports.proto` & `aiomagra-0.1.1/src/aiomagra/reports.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/reports_pb2.py` & `aiomagra-0.1.1/src/aiomagra/reports_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/roller_shutter.proto` & `aiomagra-0.1.1/src/aiomagra/roller_shutter.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/roller_shutter_pb2.py` & `aiomagra-0.1.1/src/aiomagra/roller_shutter_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/seismic_pb2.py` & `aiomagra-0.1.1/src/aiomagra/seismic_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/sensor_pb2.py` & `aiomagra-0.1.1/src/aiomagra/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/siren.proto` & `aiomagra-0.1.1/src/aiomagra/siren.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/siren_pb2.py` & `aiomagra-0.1.1/src/aiomagra/siren_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/smoke.proto` & `aiomagra-0.1.1/src/aiomagra/smoke.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/smoke_pb2.py` & `aiomagra-0.1.1/src/aiomagra/smoke_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/status_pb2.py` & `aiomagra-0.1.1/src/aiomagra/status_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/structure.proto` & `aiomagra-0.1.1/src/aiomagra/structure.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/structure_pb2.py` & `aiomagra-0.1.1/src/aiomagra/structure_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/switch.proto` & `aiomagra-0.1.1/src/aiomagra/switch.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/switch_pb2.py` & `aiomagra-0.1.1/src/aiomagra/switch_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/tamper_pb2.py` & `aiomagra-0.1.1/src/aiomagra/tamper_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/taptap_pb2.py` & `aiomagra-0.1.1/src/aiomagra/taptap_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/temperature.proto` & `aiomagra-0.1.1/src/aiomagra/temperature.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/temperature_pb2.py` & `aiomagra-0.1.1/src/aiomagra/temperature_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/thermostat.proto` & `aiomagra-0.1.1/src/aiomagra/thermostat.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/thermostat_pb2.py` & `aiomagra-0.1.1/src/aiomagra/thermostat_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/ultraviolet.proto` & `aiomagra-0.1.1/src/aiomagra/ultraviolet.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/ultraviolet_pb2.py` & `aiomagra-0.1.1/src/aiomagra/ultraviolet_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/units.proto` & `aiomagra-0.1.1/src/aiomagra/units.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/units_pb2.py` & `aiomagra-0.1.1/src/aiomagra/units_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/websocket_pb2.py` & `aiomagra-0.1.1/src/aiomagra/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/wifi.proto` & `aiomagra-0.1.1/src/aiomagra/wifi.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/wifi_pb2.py` & `aiomagra-0.1.1/src/aiomagra/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/zigbee.proto` & `aiomagra-0.1.1/src/aiomagra/zigbee.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/zigbee_pb2.py` & `aiomagra-0.1.1/src/aiomagra/zigbee_pb2.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/zwave.proto` & `aiomagra-0.1.1/src/aiomagra/zwave.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.0/src/aiomagra/zwave_pb2.py` & `aiomagra-0.1.1/src/aiomagra/zwave_pb2.py`

 * *Files identical despite different names*

