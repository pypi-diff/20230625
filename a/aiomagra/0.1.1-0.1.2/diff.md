# Comparing `tmp/aiomagra-0.1.1.tar.gz` & `tmp/aiomagra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomagra-0.1.1.tar", max compression
+gzip compressed data, was "aiomagra-0.1.2.tar", max compression
```

## Comparing `aiomagra-0.1.1.tar` & `aiomagra-0.1.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0       12 2023-06-25 13:29:06.484907 aiomagra-0.1.1/README.md
--rw-r--r--   0        0        0      282 2023-06-25 14:02:45.807002 aiomagra-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/__init__.py
--rw-r--r--   0        0        0      366 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/accelerometer.proto
--rw-r--r--   0        0        0     1498 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/accelerometer_pb2.py
--rw-r--r--   0        0        0      745 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/addon.proto
--rw-r--r--   0        0        0     2400 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/addon_pb2.py
--rw-r--r--   0        0        0      566 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/admin.proto
--rw-r--r--   0        0        0     1864 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/admin_pb2.py
--rw-r--r--   0        0        0      460 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/battery.proto
--rw-r--r--   0        0        0     1649 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/battery_pb2.py
--rw-r--r--   0        0        0      417 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/ble.proto
--rw-r--r--   0        0        0     1497 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/ble_pb2.py
--rw-r--r--   0        0        0      507 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/bsensor.proto
--rw-r--r--   0        0        0     1860 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/bsensor_pb2.py
--rw-r--r--   0        0        0      894 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_dioxide.proto
--rw-r--r--   0        0        0     2356 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_dioxide_pb2.py
--rw-r--r--   0        0        0     1326 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_monoxide.proto
--rw-r--r--   0        0        0     3383 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/carbon_monoxide_pb2.py
--rw-r--r--   0        0        0     5204 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/client.py
--rw-r--r--   0        0        0      778 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/color.proto
--rw-r--r--   0        0        0     2288 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/color_pb2.py
--rw-r--r--   0        0        0     2116 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/configuration.proto
--rw-r--r--   0        0        0     4789 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/configuration_pb2.py
--rw-r--r--   0        0        0       79 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/const.py
--rw-r--r--   0        0        0     3883 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/devices.proto
--rw-r--r--   0        0        0    10232 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/devices_pb2.py
--rw-r--r--   0        0        0      327 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/door.proto
--rw-r--r--   0        0        0     1323 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/door_pb2.py
--rw-r--r--   0        0        0      276 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/doorbell.proto
--rw-r--r--   0        0        0     1313 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/doorbell_pb2.py
--rw-r--r--   0        0        0      329 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/emergency.proto
--rw-r--r--   0        0        0     1359 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/emergency_pb2.py
--rw-r--r--   0        0        0     1349 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/firmware.proto
--rw-r--r--   0        0        0     3574 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/firmware_pb2.py
--rw-r--r--   0        0        0      272 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/flood.proto
--rw-r--r--   0        0        0     1281 2023-06-25 13:29:06.474907 aiomagra-0.1.1/src/aiomagra/flood_pb2.py
--rw-r--r--   0        0        0      622 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gate.proto
--rw-r--r--   0        0        0     1949 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gate_pb2.py
--rw-r--r--   0        0        0      617 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gateway.proto
--rw-r--r--   0        0        0     2049 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/gateway_pb2.py
--rw-r--r--   0        0        0      300 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/heartbeat.proto
--rw-r--r--   0        0        0     1253 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/heartbeat_pb2.py
--rw-r--r--   0        0        0      424 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/info.proto
--rw-r--r--   0        0        0     1494 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/info_pb2.py
--rw-r--r--   0        0        0     1080 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/level.proto
--rw-r--r--   0        0        0     2779 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/level_pb2.py
--rw-r--r--   0        0        0      639 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/lock.proto
--rw-r--r--   0        0        0     1991 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/lock_pb2.py
--rw-r--r--   0        0        0      405 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/messaging.proto
--rw-r--r--   0        0        0     1459 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/messaging_pb2.py
--rw-r--r--   0        0        0      678 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/metadata.proto
--rw-r--r--   0        0        0     2250 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/metadata_pb2.py
--rw-r--r--   0        0        0      689 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/meter.proto
--rw-r--r--   0        0        0     2196 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/meter_pb2.py
--rw-r--r--   0        0        0      303 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/mqtt.proto
--rw-r--r--   0        0        0     1212 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/mqtt_pb2.py
--rw-r--r--   0        0        0      647 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/power_source.proto
--rw-r--r--   0        0        0     1908 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/power_source_pb2.py
--rw-r--r--   0        0        0    11060 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/pubsub.proto
--rw-r--r--   0        0        0    18842 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/pubsub_pb2.py
--rw-r--r--   0        0        0      622 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/remote.proto
--rw-r--r--   0        0        0     2030 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/remote_pb2.py
--rw-r--r--   0        0        0     3457 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/reports.proto
--rw-r--r--   0        0        0     6738 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/reports_pb2.py
--rw-r--r--   0        0        0      724 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/roller_shutter.proto
--rw-r--r--   0        0        0     2150 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/roller_shutter_pb2.py
--rw-r--r--   0        0        0      357 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/seismic.proto
--rw-r--r--   0        0        0     1434 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/seismic_pb2.py
--rw-r--r--   0        0        0      410 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/sensor.proto
--rw-r--r--   0        0        0     1595 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/sensor_pb2.py
--rw-r--r--   0        0        0     2040 2023-06-25 13:29:06.478240 aiomagra-0.1.1/src/aiomagra/siren.proto
--rw-r--r--   0        0        0     5427 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/siren_pb2.py
--rw-r--r--   0        0        0      827 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/smoke.proto
--rw-r--r--   0        0        0     2224 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/smoke_pb2.py
--rw-r--r--   0        0        0      510 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/status.proto
--rw-r--r--   0        0        0     1802 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/status_pb2.py
--rw-r--r--   0        0        0      574 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/structure.proto
--rw-r--r--   0        0        0     1909 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/structure_pb2.py
--rw-r--r--   0        0        0      562 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/switch.proto
--rw-r--r--   0        0        0     1855 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/switch_pb2.py
--rw-r--r--   0        0        0      327 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/tamper.proto
--rw-r--r--   0        0        0     1328 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/tamper_pb2.py
--rw-r--r--   0        0        0      222 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/taptap.proto
--rw-r--r--   0        0        0     1096 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/taptap_pb2.py
--rw-r--r--   0        0        0      575 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/temperature.proto
--rw-r--r--   0        0        0     1890 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/temperature_pb2.py
--rw-r--r--   0        0        0     2051 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/thermostat.proto
--rw-r--r--   0        0        0     5104 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/thermostat_pb2.py
--rw-r--r--   0        0        0      562 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/ultraviolet.proto
--rw-r--r--   0        0        0     1869 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/ultraviolet_pb2.py
--rw-r--r--   0        0        0     8927 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/units.proto
--rw-r--r--   0        0        0     1627 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/units_pb2.py
--rw-r--r--   0        0        0      390 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/websocket.proto
--rw-r--r--   0        0        0     1398 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/websocket_pb2.py
--rw-r--r--   0        0        0     1130 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/wifi.proto
--rw-r--r--   0        0        0     3028 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/wifi_pb2.py
--rw-r--r--   0        0        0      909 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zigbee.proto
--rw-r--r--   0        0        0     2577 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zigbee_pb2.py
--rw-r--r--   0        0        0     6499 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zwave.proto
--rw-r--r--   0        0        0    15749 2023-06-25 13:29:06.481573 aiomagra-0.1.1/src/aiomagra/zwave_pb2.py
--rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 aiomagra-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-06-25 13:29:06.484907 aiomagra-0.1.2/README.md
+-rw-r--r--   0        0        0      281 2023-06-25 14:20:33.712395 aiomagra-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-06-25 13:29:06.474907 aiomagra-0.1.2/src/aiomagra/__init__.py
+-rw-r--r--   0        0        0      366 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/accelerometer.proto
+-rw-r--r--   0        0        0     1622 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/accelerometer_pb2.py
+-rw-r--r--   0        0        0      745 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/addon.proto
+-rw-r--r--   0        0        0     2466 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/addon_pb2.py
+-rw-r--r--   0        0        0      566 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/admin.proto
+-rw-r--r--   0        0        0     1930 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/admin_pb2.py
+-rw-r--r--   0        0        0      460 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/battery.proto
+-rw-r--r--   0        0        0     1779 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/battery_pb2.py
+-rw-r--r--   0        0        0      417 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/ble.proto
+-rw-r--r--   0        0        0     1563 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/ble_pb2.py
+-rw-r--r--   0        0        0      507 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/bsensor.proto
+-rw-r--r--   0        0        0     1926 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/bsensor_pb2.py
+-rw-r--r--   0        0        0      894 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/carbon_dioxide.proto
+-rw-r--r--   0        0        0     2422 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/carbon_dioxide_pb2.py
+-rw-r--r--   0        0        0     1326 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/carbon_monoxide.proto
+-rw-r--r--   0        0        0     3571 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/carbon_monoxide_pb2.py
+-rw-r--r--   0        0        0     5204 2023-06-25 13:29:06.474907 aiomagra-0.1.2/src/aiomagra/client.py
+-rw-r--r--   0        0        0      778 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/color.proto
+-rw-r--r--   0        0        0     2500 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/color_pb2.py
+-rw-r--r--   0        0        0     2116 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/configuration.proto
+-rw-r--r--   0        0        0     4919 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/configuration_pb2.py
+-rw-r--r--   0        0        0       79 2023-06-25 13:29:06.474907 aiomagra-0.1.2/src/aiomagra/const.py
+-rw-r--r--   0        0        0     3883 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/devices.proto
+-rw-r--r--   0        0        0    10693 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/devices_pb2.py
+-rw-r--r--   0        0        0      327 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/door.proto
+-rw-r--r--   0        0        0     1389 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/door_pb2.py
+-rw-r--r--   0        0        0      276 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/doorbell.proto
+-rw-r--r--   0        0        0     1379 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/doorbell_pb2.py
+-rw-r--r--   0        0        0      329 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/emergency.proto
+-rw-r--r--   0        0        0     1425 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/emergency_pb2.py
+-rw-r--r--   0        0        0     1349 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/firmware.proto
+-rw-r--r--   0        0        0     3640 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/firmware_pb2.py
+-rw-r--r--   0        0        0      272 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/flood.proto
+-rw-r--r--   0        0        0     1347 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/flood_pb2.py
+-rw-r--r--   0        0        0      622 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/gate.proto
+-rw-r--r--   0        0        0     2079 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/gate_pb2.py
+-rw-r--r--   0        0        0      617 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/gateway.proto
+-rw-r--r--   0        0        0     2115 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/gateway_pb2.py
+-rw-r--r--   0        0        0      300 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/heartbeat.proto
+-rw-r--r--   0        0        0     1319 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/heartbeat_pb2.py
+-rw-r--r--   0        0        0      424 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/info.proto
+-rw-r--r--   0        0        0     1560 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/info_pb2.py
+-rw-r--r--   0        0        0     1080 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/level.proto
+-rw-r--r--   0        0        0     2991 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/level_pb2.py
+-rw-r--r--   0        0        0      639 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/lock.proto
+-rw-r--r--   0        0        0     2121 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/lock_pb2.py
+-rw-r--r--   0        0        0      405 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/messaging.proto
+-rw-r--r--   0        0        0     1525 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/messaging_pb2.py
+-rw-r--r--   0        0        0      678 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/metadata.proto
+-rw-r--r--   0        0        0     2316 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/metadata_pb2.py
+-rw-r--r--   0        0        0      689 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/meter.proto
+-rw-r--r--   0        0        0     2384 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/meter_pb2.py
+-rw-r--r--   0        0        0      303 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/mqtt.proto
+-rw-r--r--   0        0        0     1338 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/mqtt_pb2.py
+-rw-r--r--   0        0        0      647 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/power_source.proto
+-rw-r--r--   0        0        0     1974 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/power_source_pb2.py
+-rw-r--r--   0        0        0    11060 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/pubsub.proto
+-rw-r--r--   0        0        0    20652 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/pubsub_pb2.py
+-rw-r--r--   0        0        0      622 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/remote.proto
+-rw-r--r--   0        0        0     2160 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/remote_pb2.py
+-rw-r--r--   0        0        0     3457 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/reports.proto
+-rw-r--r--   0        0        0     8944 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/reports_pb2.py
+-rw-r--r--   0        0        0      724 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/roller_shutter.proto
+-rw-r--r--   0        0        0     2280 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/roller_shutter_pb2.py
+-rw-r--r--   0        0        0      357 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/seismic.proto
+-rw-r--r--   0        0        0     1558 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/seismic_pb2.py
+-rw-r--r--   0        0        0      410 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/sensor.proto
+-rw-r--r--   0        0        0     1719 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/sensor_pb2.py
+-rw-r--r--   0        0        0     2040 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/siren.proto
+-rw-r--r--   0        0        0     5557 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/siren_pb2.py
+-rw-r--r--   0        0        0      827 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/smoke.proto
+-rw-r--r--   0        0        0     2290 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/smoke_pb2.py
+-rw-r--r--   0        0        0      510 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/status.proto
+-rw-r--r--   0        0        0     1868 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/status_pb2.py
+-rw-r--r--   0        0        0      574 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/structure.proto
+-rw-r--r--   0        0        0     1975 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/structure_pb2.py
+-rw-r--r--   0        0        0      562 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/switch.proto
+-rw-r--r--   0        0        0     1985 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/switch_pb2.py
+-rw-r--r--   0        0        0      327 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/tamper.proto
+-rw-r--r--   0        0        0     1394 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/tamper_pb2.py
+-rw-r--r--   0        0        0      222 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/taptap.proto
+-rw-r--r--   0        0        0     1162 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/taptap_pb2.py
+-rw-r--r--   0        0        0      575 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/temperature.proto
+-rw-r--r--   0        0        0     2078 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/temperature_pb2.py
+-rw-r--r--   0        0        0     2051 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/thermostat.proto
+-rw-r--r--   0        0        0     5292 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/thermostat_pb2.py
+-rw-r--r--   0        0        0      562 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/ultraviolet.proto
+-rw-r--r--   0        0        0     2057 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/ultraviolet_pb2.py
+-rw-r--r--   0        0        0     8927 2023-06-25 14:21:13.962522 aiomagra-0.1.2/src/aiomagra/units.proto
+-rw-r--r--   0        0        0     1693 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/units_pb2.py
+-rw-r--r--   0        0        0      390 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/websocket.proto
+-rw-r--r--   0        0        0     1586 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/websocket_pb2.py
+-rw-r--r--   0        0        0     1130 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/wifi.proto
+-rw-r--r--   0        0        0     3178 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/wifi_pb2.py
+-rw-r--r--   0        0        0      909 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/zigbee.proto
+-rw-r--r--   0        0        0     2769 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/zigbee_pb2.py
+-rw-r--r--   0        0        0     6499 2023-06-25 14:21:13.965855 aiomagra-0.1.2/src/aiomagra/zwave.proto
+-rw-r--r--   0        0        0    16023 2023-06-25 14:21:13.982522 aiomagra-0.1.2/src/aiomagra/zwave_pb2.py
+-rw-r--r--   0        0        0      327 1970-01-01 00:00:00.000000 aiomagra-0.1.2/PKG-INFO
```

### Comparing `aiomagra-0.1.1/src/aiomagra/accelerometer_pb2.py` & `aiomagra-0.1.2/src/aiomagra/accelerometer_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/accelerometer.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x61iomagra/accelerometer.proto\x12\x08vemmiopb\x1a\x14\x61iomagra/units.proto\"m\n\x13\x41\x63\x63\x65lerometerReport\x12)\n\x04\x61xis\x18\x01 \x01(\x0e\x32\x1b.vemmiopb.AccelerometerAxis\x12\x1c\n\x04unit\x18\x02 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x03 \x01(\x01*(\n\x11\x41\x63\x63\x65lerometerAxis\x12\x05\n\x01X\x10\x00\x12\x05\n\x01Y\x10\x01\x12\x05\n\x01Z\x10\x02\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.accelerometer_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ACCELEROMETERAXIS._serialized_start=175
   _ACCELEROMETERAXIS._serialized_end=215
   _ACCELEROMETERREPORT._serialized_start=64
   _ACCELEROMETERREPORT._serialized_end=173
```

### Comparing `aiomagra-0.1.1/src/aiomagra/addon.proto` & `aiomagra-0.1.2/src/aiomagra/addon.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/addon_pb2.py` & `aiomagra-0.1.2/src/aiomagra/addon_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/addon.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/addon.proto\x12\x08vemmiopb\"\x12\n\x10\x41\x64\x64onListRequest\"\x97\x01\n\x11\x41\x64\x64onListResponse\x12\x31\n\x06\x61\x64\x64ons\x18\x01 \x03(\x0b\x32!.vemmiopb.AddonListResponse.Addon\x1aO\n\x05\x41\x64\x64on\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12/\n\nthermostat\x18\x02 \x01(\x0b\x32\x19.vemmiopb.AddonThermostatH\x00\x42\x07\n\x05\x61\x64\x64on\"J\n\x19\x41\x64\x64onAddThermostatRequest\x12-\n\nthermostat\x18\x01 \x01(\x0b\x32\x19.vemmiopb.AddonThermostat\" \n\x10\x41\x64\x64onAddResponse\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"B\n\x0f\x41\x64\x64onThermostat\x12\x16\n\x0einput_filename\x18\x01 \x01(\t\x12\x17\n\x0foutput_filename\x18\x02 \x01(\t2\xa4\x01\n\x05\x41\x64\x64on\x12\x44\n\tAddonList\x12\x1a.vemmiopb.AddonListRequest\x1a\x1b.vemmiopb.AddonListResponse\x12U\n\x12\x41\x64\x64onAddThermostat\x12#.vemmiopb.AddonAddThermostatRequest\x1a\x1a.vemmiopb.AddonAddResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.addon_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ADDONLISTREQUEST._serialized_start=34
   _ADDONLISTREQUEST._serialized_end=52
   _ADDONLISTRESPONSE._serialized_start=55
   _ADDONLISTRESPONSE._serialized_end=206
```

### Comparing `aiomagra-0.1.1/src/aiomagra/admin.proto` & `aiomagra-0.1.2/src/aiomagra/admin.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/admin_pb2.py` & `aiomagra-0.1.2/src/aiomagra/admin_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/admin.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/admin.proto\x12\x08vemmiopb\"\x12\n\x10WalkNodesRequest\"!\n\x11WalkNodesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\",\n\x0bLogsRequest\x12\x0e\n\x06\x66ilter\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"\x19\n\tLogsChunk\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x32\xc5\x01\n\x05\x41\x64min\x12\x46\n\tWalkNodes\x12\x1a.vemmiopb.WalkNodesRequest\x1a\x1b.vemmiopb.WalkNodesResponse0\x01\x12\x38\n\x08ReadLogs\x12\x15.vemmiopb.LogsRequest\x1a\x13.vemmiopb.LogsChunk0\x01\x12:\n\nFollowLogs\x12\x15.vemmiopb.LogsRequest\x1a\x13.vemmiopb.LogsChunk0\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.admin_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _WALKNODESREQUEST._serialized_start=34
   _WALKNODESREQUEST._serialized_end=52
   _WALKNODESRESPONSE._serialized_start=54
   _WALKNODESRESPONSE._serialized_end=87
```

### Comparing `aiomagra-0.1.1/src/aiomagra/battery_pb2.py` & `aiomagra-0.1.2/src/aiomagra/battery_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/battery.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61iomagra/battery.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"?\n\x11\x42\x61tteryGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"#\n\x12\x42\x61tteryGetResponse\x12\r\n\x05level\x18\x01 \x01(\x05\"\x1e\n\rBatteryReport\x12\r\n\x05level\x18\x01 \x01(\x05\x32R\n\x07\x42\x61ttery\x12G\n\nBatteryGet\x12\x1b.vemmiopb.BatteryGetRequest\x1a\x1c.vemmiopb.BatteryGetResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.battery_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _BATTERYGETREQUEST._serialized_start=61
   _BATTERYGETREQUEST._serialized_end=124
   _BATTERYGETRESPONSE._serialized_start=126
   _BATTERYGETRESPONSE._serialized_end=161
```

### Comparing `aiomagra-0.1.1/src/aiomagra/ble_pb2.py` & `aiomagra-0.1.2/src/aiomagra/ble_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/ble.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61iomagra/ble.proto\x12\x08vemmiopb\"\x14\n\x12\x41\x64vertisingRequest\"\x15\n\x13\x41\x64vertisingResponse2\xb1\x01\n\nBLEService\x12P\n\x11\x45nableAdvertising\x12\x1c.vemmiopb.AdvertisingRequest\x1a\x1d.vemmiopb.AdvertisingResponse\x12Q\n\x12\x44isableAdvertising\x12\x1c.vemmiopb.AdvertisingRequest\x1a\x1d.vemmiopb.AdvertisingResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.ble_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ADVERTISINGREQUEST._serialized_start=32
   _ADVERTISINGREQUEST._serialized_end=52
   _ADVERTISINGRESPONSE._serialized_start=54
   _ADVERTISINGRESPONSE._serialized_end=75
```

### Comparing `aiomagra-0.1.1/src/aiomagra/bsensor_pb2.py` & `aiomagra-0.1.2/src/aiomagra/bsensor_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/bsensor.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61iomagra/bsensor.proto\x12\x08vemmiopb\":\n\x0fOpenCloseReport\x12\'\n\x05state\x18\x01 \x01(\x0e\x32\x18.vemmiopb.OpenCloseState\"\\\n\x0cMotionReport\x12+\n\x05state\x18\x01 \x01(\x0e\x32\x1c.vemmiopb.MotionReport.State\"\x1f\n\x05State\x12\x08\n\x04IDLE\x10\x00\x12\x0c\n\x08\x44\x45TECTED\x10\x01*H\n\x0eOpenCloseState\x12\x19\n\x15OPEN_CLOSE_STATE_OPEN\x10\x00\x12\x1b\n\x17OPEN_CLOSE_STATE_CLOSED\x10\x01*M\n\x11\x42inarySensorState\x12\x16\n\x12\x42SENSOR_STATE_IDLE\x10\x00\x12 \n\x1c\x42SENSOR_STATE_EVENT_DETECTED\x10\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.bsensor_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _OPENCLOSESTATE._serialized_start=190
   _OPENCLOSESTATE._serialized_end=262
   _BINARYSENSORSTATE._serialized_start=264
   _BINARYSENSORSTATE._serialized_end=341
```

### Comparing `aiomagra-0.1.1/src/aiomagra/carbon_dioxide.proto` & `aiomagra-0.1.2/src/aiomagra/carbon_dioxide.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/carbon_dioxide_pb2.py` & `aiomagra-0.1.2/src/aiomagra/carbon_dioxide_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/carbon_dioxide.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x61iomagra/carbon_dioxide.proto\x12\x08vemmiopb\"\xb4\x01\n\x13\x43\x61rbonDioxideReport\x12+\n\x05state\x18\x01 \x01(\x0e\x32\x1c.vemmiopb.CarbonDioxideState\x12\x37\n\x0breplacement\x18\x02 \x01(\x0e\x32\".vemmiopb.CarbonDioxideReplacement\x12\x37\n\x0bmaintenance\x18\x03 \x01(\x0e\x32\".vemmiopb.CarbonDioxideMaintenance*\x9d\x02\n\x12\x43\x61rbonDioxideState\x12$\n CARBON_DIOXIDE_STATE_UNSPECIFIED\x10\x00\x12\x1e\n\x1a\x43\x41RBON_DIOXIDE_STATE_CLEAR\x10\x01\x12!\n\x1d\x43\x41RBON_DIOXIDE_STATE_DETECTED\x10\x02\x12\x1d\n\x19\x43\x41RBON_DIOXIDE_STATE_TEST\x10\x03\x12!\n\x1d\x43\x41RBON_DIOXIDE_STATE_SILENCED\x10\x04\x12-\n)CARBON_DIOXIDE_STATE_REPLACEMENT_REQUIRED\x10\x05\x12-\n)CARBON_DIOXIDE_STATE_MAINTENANCE_REQUIRED\x10\x06*j\n\x18\x43\x61rbonDioxideReplacement\x12*\n&CARBON_DIOXIDE_REPLACEMENT_UNSPECIFIED\x10\x00\x12\"\n\x1e\x43\x41RBON_DIOXIDE_REPLACEMENT_EOL\x10\x01*z\n\x18\x43\x61rbonDioxideMaintenance\x12*\n&CARBON_DIOXIDE_MAINTENANCE_UNSPECIFIED\x10\x00\x12\x32\n.CARBON_DIOXIDE_MAINTENANCE_PERIODIC_INSPECTION\x10\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.carbon_dioxide_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _CARBONDIOXIDESTATE._serialized_start=227
   _CARBONDIOXIDESTATE._serialized_end=512
   _CARBONDIOXIDEREPLACEMENT._serialized_start=514
   _CARBONDIOXIDEREPLACEMENT._serialized_end=620
```

### Comparing `aiomagra-0.1.1/src/aiomagra/carbon_monoxide.proto` & `aiomagra-0.1.2/src/aiomagra/carbon_monoxide.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/carbon_monoxide_pb2.py` & `aiomagra-0.1.2/src/aiomagra/carbon_monoxide_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/carbon_monoxide.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x61iomagra/carbon_monoxide.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\x1a\x14\x61iomagra/units.proto\"F\n\x18\x43\x61rbonMonoxideGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"H\n\x19\x43\x61rbonMonoxideGetResponse\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"H\n\x19\x43\x61rbonMonoxideValueReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"\xbd\x01\n\x19\x43\x61rbonMonoxideStateReport\x12,\n\x05state\x18\x01 \x01(\x0e\x32\x1d.vemmiopb.CarbonMonoxideState\x12\x38\n\x0breplacement\x18\x02 \x01(\x0e\x32#.vemmiopb.CarbonMonoxideReplacement\x12\x38\n\x0bmaintenance\x18\x03 \x01(\x0e\x32#.vemmiopb.CarbonMonoxideMaintenance*\xa5\x02\n\x13\x43\x61rbonMonoxideState\x12%\n!CARBON_MONOXIDE_STATE_UNSPECIFIED\x10\x00\x12\x1f\n\x1b\x43\x41RBON_MONOXIDE_STATE_CLEAR\x10\x01\x12\"\n\x1e\x43\x41RBON_MONOXIDE_STATE_DETECTED\x10\x02\x12\x1e\n\x1a\x43\x41RBON_MONOXIDE_STATE_TEST\x10\x03\x12\"\n\x1e\x43\x41RBON_MONOXIDE_STATE_SILENCED\x10\x04\x12.\n*CARBON_MONOXIDE_STATE_REPLACEMENT_REQUIRED\x10\x05\x12.\n*CARBON_MONOXIDE_STATE_MAINTENANCE_REQUIRED\x10\x06*m\n\x19\x43\x61rbonMonoxideReplacement\x12+\n\'CARBON_MONOXIDE_REPLACEMENT_UNSPECIFIED\x10\x00\x12#\n\x1f\x43\x41RBON_MONOXIDE_REPLACEMENT_EOL\x10\x01*}\n\x19\x43\x61rbonMonoxideMaintenance\x12+\n\'CARBON_MONOXIDE_MAINTENANCE_UNSPECIFIED\x10\x00\x12\x33\n/CARBON_MONOXIDE_MAINTENANCE_PERIODIC_INSPECTION\x10\x01\x32u\n\x15\x43\x61rbonMonoxideService\x12\\\n\x11\x43\x61rbonMonoxideGet\x12\".vemmiopb.CarbonMonoxideGetRequest\x1a#.vemmiopb.CarbonMonoxideGetResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.carbon_monoxide_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _CARBONMONOXIDESTATE._serialized_start=504
   _CARBONMONOXIDESTATE._serialized_end=797
   _CARBONMONOXIDEREPLACEMENT._serialized_start=799
   _CARBONMONOXIDEREPLACEMENT._serialized_end=908
```

### Comparing `aiomagra-0.1.1/src/aiomagra/client.py` & `aiomagra-0.1.2/src/aiomagra/client.py`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/color.proto` & `aiomagra-0.1.2/src/aiomagra/color.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/color_pb2.py` & `aiomagra-0.1.2/src/aiomagra/color_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/color.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/color.proto\x12\x08vemmiopb\x1a\x1egoogle/protobuf/duration.proto\x1a\x17\x61iomagra/metadata.proto\"\x90\x01\n\x0f\x43olorSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12$\n\x06values\x18\x02 \x03(\x0b\x32\x14.vemmiopb.ColorValue\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x0f\n\rColorResponse\"3\n\x0b\x43olorReport\x12$\n\x06values\x18\x01 \x03(\x0b\x32\x14.vemmiopb.ColorValue\"H\n\nColorValue\x12+\n\tcomponent\x18\x01 \x01(\x0e\x32\x18.vemmiopb.ColorComponent\x12\r\n\x05value\x18\x02 \x01(\x05*\x83\x01\n\x0e\x43olorComponent\x12\x15\n\x11\x43OLOR_UNSPECIFIED\x10\x00\x12\x14\n\x10\x43OLOR_WARM_WHITE\x10\x01\x12\x14\n\x10\x43OLOR_COLD_WHITE\x10\x02\x12\r\n\tCOLOR_RED\x10\x03\x12\x0f\n\x0b\x43OLOR_GREEN\x10\x04\x12\x0e\n\nCOLOR_BLUE\x10\x05\x32G\n\x05\x43olor\x12>\n\x08\x43olorSet\x12\x19.vemmiopb.ColorSetRequest\x1a\x17.vemmiopb.ColorResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.color_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _COLORCOMPONENT._serialized_start=383
   _COLORCOMPONENT._serialized_end=514
   _COLORSETREQUEST._serialized_start=92
   _COLORSETREQUEST._serialized_end=236
```

### Comparing `aiomagra-0.1.1/src/aiomagra/configuration.proto` & `aiomagra-0.1.2/src/aiomagra/configuration.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/configuration_pb2.py` & `aiomagra-0.1.2/src/aiomagra/configuration_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/configuration.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x61iomagra/configuration.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"F\n\x18\x43onfigurationListRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"K\n\x19\x43onfigurationListResponse\x12.\n\x07options\x18\x01 \x03(\x0b\x32\x1d.vemmiopb.ConfigurationOption\"T\n\x17\x43onfigurationGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\r\n\x05index\x18\x02 \x01(\x05\"G\n\x18\x43onfigurationGetResponse\x12+\n\x05value\x18\x01 \x01(\x0b\x32\x1c.vemmiopb.ConfigurationValue\"\x81\x01\n\x17\x43onfigurationSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\r\n\x05index\x18\x02 \x01(\x05\x12+\n\x05value\x18\x03 \x01(\x0b\x32\x1c.vemmiopb.ConfigurationValue\"\x1a\n\x18\x43onfigurationSetResponse\"q\n\x13\x43onfigurationOption\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05label\x18\x02 \x01(\t\x12\x0c\n\x04help\x18\x03 \x01(\t\x12.\n\x04type\x18\x04 \x01(\x0e\x32 .vemmiopb.ConfigurationValueType\"S\n\x12\x43onfigurationValue\x12\x34\n\x06scalar\x18\x01 \x01(\x0b\x32\".vemmiopb.ConfigurationValueScalarH\x00\x42\x07\n\x05value\"\xbd\x02\n\x18\x43onfigurationValueScalar\x12\x14\n\nbool_value\x18\x01 \x01(\x08H\x00\x12\x15\n\x0buint8_value\x18\x02 \x01(\rH\x00\x12\x16\n\x0cuint16_value\x18\x03 \x01(\rH\x00\x12\x16\n\x0cuint32_value\x18\x04 \x01(\rH\x00\x12\x16\n\x0cuint64_value\x18\x05 \x01(\x04H\x00\x12\x14\n\nint8_value\x18\x06 \x01(\x05H\x00\x12\x15\n\x0bint16_value\x18\x07 \x01(\x05H\x00\x12\x15\n\x0bint32_value\x18\x08 \x01(\x05H\x00\x12\x15\n\x0bint64_value\x18\t \x01(\x03H\x00\x12\x17\n\rfloat32_value\x18\n \x01(\x02H\x00\x12\x17\n\rfloat64_value\x18\x0b \x01(\x01H\x00\x12\x16\n\x0cstring_value\x18\x0c \x01(\tH\x00\x42\x07\n\x05value*\xf6\x03\n\x16\x43onfigurationValueType\x12&\n\"CONFIGURATION_VALUE_TYPE_UNDEFINED\x10\x00\x12!\n\x1d\x43ONFIGURATION_VALUE_TYPE_BOOL\x10\x01\x12\"\n\x1e\x43ONFIGURATION_VALUE_TYPE_UINT8\x10\x02\x12#\n\x1f\x43ONFIGURATION_VALUE_TYPE_UINT16\x10\x03\x12#\n\x1f\x43ONFIGURATION_VALUE_TYPE_UINT32\x10\x04\x12#\n\x1f\x43ONFIGURATION_VALUE_TYPE_UINT64\x10\x05\x12!\n\x1d\x43ONFIGURATION_VALUE_TYPE_INT8\x10\x06\x12\"\n\x1e\x43ONFIGURATION_VALUE_TYPE_INT16\x10\x07\x12\"\n\x1e\x43ONFIGURATION_VALUE_TYPE_INT32\x10\x08\x12\"\n\x1e\x43ONFIGURATION_VALUE_TYPE_INT64\x10\t\x12$\n CONFIGURATION_VALUE_TYPE_FLOAT32\x10\n\x12$\n CONFIGURATION_VALUE_TYPE_FLOAT64\x10\x0b\x12#\n\x1f\x43ONFIGURATION_VALUE_TYPE_STRING\x10\x0c\x32\xa3\x02\n\rConfiguration\x12\\\n\x11\x43onfigurationList\x12\".vemmiopb.ConfigurationListRequest\x1a#.vemmiopb.ConfigurationListResponse\x12Y\n\x10\x43onfigurationGet\x12!.vemmiopb.ConfigurationGetRequest\x1a\".vemmiopb.ConfigurationGetResponse\x12Y\n\x10\x43onfigurationSet\x12!.vemmiopb.ConfigurationSetRequest\x1a\".vemmiopb.ConfigurationSetResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.configuration_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _CONFIGURATIONVALUETYPE._serialized_start=1056
   _CONFIGURATIONVALUETYPE._serialized_end=1558
   _CONFIGURATIONLISTREQUEST._serialized_start=67
   _CONFIGURATIONLISTREQUEST._serialized_end=137
```

### Comparing `aiomagra-0.1.1/src/aiomagra/devices.proto` & `aiomagra-0.1.2/src/aiomagra/devices.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/devices_pb2.py` & `aiomagra-0.1.2/src/aiomagra/devices_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/devices.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import accelerometer_pb2 as aiomagra_dot_accelerometer__pb2
+from aiomagra import color_pb2 as aiomagra_dot_color__pb2
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
+from aiomagra import power_source_pb2 as aiomagra_dot_power__source__pb2
+from aiomagra import thermostat_pb2 as aiomagra_dot_thermostat__pb2
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61iomagra/devices.proto\x12\x08vemmiopb\x1a\x1c\x61iomagra/accelerometer.proto\x1a\x14\x61iomagra/color.proto\x1a\x17\x61iomagra/metadata.proto\x1a\x1b\x61iomagra/power_source.proto\x1a\x19\x61iomagra/thermostat.proto\x1a\x14\x61iomagra/units.proto\"\x14\n\x12\x44\x65vicesListRequest\"8\n\x13\x44\x65vicesListResponse\x12!\n\x07\x64\x65vices\x18\x01 \x03(\x0b\x32\x10.vemmiopb.Device\"\xbf\x02\n\x06\x44\x65vice\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x08metadata\x18\x02 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12*\n\x0c\x63\x61pabilities\x18\x03 \x03(\x0b\x32\x14.vemmiopb.Capability\x12\x0c\n\x04i18n\x18\x04 \x01(\t\x12%\n\x05group\x18\x05 \x01(\x0e\x32\x16.vemmiopb.Device.Group\"\x99\x01\n\x05Group\x12\t\n\x05OTHER\x10\x00\x12\x0b\n\x07\x43LIMATE\x10\x01\x12\x0c\n\x08SECURITY\x10\x02\x12\t\n\x05POWER\x10\x03\x12\x13\n\x0fROLLER_SHUTTERS\x10\x04\x12\x0b\n\x07\x43\x41MERAS\x10\x05\x12\r\n\tDOORBELLS\x10\x06\x12\x0c\n\x08GATEWAYS\x10\x07\x12\n\n\x06LIGHTS\x10\x08\x12\t\n\x05GATES\x10\t\x12\t\n\x05SOUND\x10\n\"\xf5\r\n\nCapability\x12,\n\x06switch\x18\x01 \x01(\x0b\x32\x1a.vemmiopb.SwitchCapabilityH\x00\x12\x30\n\x0bpower_meter\x18\x02 \x01(\x0b\x32\x19.vemmiopb.MeterCapabilityH\x00\x12.\n\tgas_meter\x18\x03 \x01(\x0b\x32\x19.vemmiopb.MeterCapabilityH\x00\x12\x30\n\x0bwater_meter\x18\x04 \x01(\x0b\x32\x19.vemmiopb.MeterCapabilityH\x00\x12\x33\n\nopen_close\x18\x05 \x01(\x0b\x32\x1d.vemmiopb.OpenCloseCapabilityH\x00\x12;\n\x0esmoke_detector\x18\x06 \x01(\x0b\x32!.vemmiopb.SmokeDetectorCapabilityH\x00\x12=\n\x0fmotion_detector\x18\x07 \x01(\x0b\x32\".vemmiopb.MotionDetectorCapabilityH\x00\x12;\n\x0e\x66lood_detector\x18\x08 \x01(\x0b\x32!.vemmiopb.FloodDetectorCapabilityH\x00\x12N\n\x18\x63\x61rbon_monoxide_detector\x18\t \x01(\x0b\x32*.vemmiopb.CarbonMonoxideDetectorCapabilityH\x00\x12\x34\n\nthermostat\x18\n \x01(\x0b\x32\x1e.vemmiopb.ThermostatCapabilityH\x00\x12\x36\n\x0btemperature\x18\x0b \x01(\x0b\x32\x1f.vemmiopb.TemperatureCapabilityH\x00\x12\x30\n\x08humidity\x18\x0c \x01(\x0b\x32\x1c.vemmiopb.HumidityCapabilityH\x00\x12\x38\n\x0cillumination\x18\r \x01(\x0b\x32 .vemmiopb.IlluminationCapabilityH\x00\x12\x32\n\tdirection\x18\x0e \x01(\x0b\x32\x1d.vemmiopb.DirectionCapabilityH\x00\x12,\n\x06tamper\x18\x0f \x01(\x0b\x32\x1a.vemmiopb.TamperCapabilityH\x00\x12\x32\n\temergency\x18\x10 \x01(\x0b\x32\x1d.vemmiopb.EmergencyCapabilityH\x00\x12(\n\x04\x64oor\x18\x11 \x01(\x0b\x32\x18.vemmiopb.DoorCapabilityH\x00\x12-\n\x07tap_tap\x18\x12 \x01(\x0b\x32\x1a.vemmiopb.TapTapCapabilityH\x00\x12*\n\x05\x63olor\x18\x13 \x01(\x0b\x32\x19.vemmiopb.ColorCapabilityH\x00\x12*\n\x05level\x18\x14 \x01(\x0b\x32\x19.vemmiopb.LevelCapabilityH\x00\x12.\n\x07\x62\x61ttery\x18\x15 \x01(\x0b\x32\x1b.vemmiopb.BatteryCapabilityH\x00\x12(\n\x04lock\x18\x16 \x01(\x0b\x32\x18.vemmiopb.LockCapabilityH\x00\x12,\n\x06remote\x18\x17 \x01(\x0b\x32\x1a.vemmiopb.RemoteCapabilityH\x00\x12\x37\n\x0cpower_source\x18\x18 \x01(\x0b\x32\x1f.vemmiopb.PowerSourceCapabilityH\x00\x12;\n\x0eroller_shutter\x18\x19 \x01(\x0b\x32!.vemmiopb.RollerShutterCapabilityH\x00\x12:\n\rconfiguration\x18\x1a \x01(\x0b\x32!.vemmiopb.ConfigurationCapabilityH\x00\x12\x30\n\x08\x64oorbell\x18\x1b \x01(\x0b\x32\x1c.vemmiopb.DoorbellCapabilityH\x00\x12*\n\x05siren\x18\x1c \x01(\x0b\x32\x19.vemmiopb.SirenCapabilityH\x00\x12:\n\raccelerometer\x18\x1d \x01(\x0b\x32!.vemmiopb.AccelerometerCapabilityH\x00\x12.\n\x07seismic\x18\x1e \x01(\x0b\x32\x1b.vemmiopb.SeismicCapabilityH\x00\x12L\n\x17\x63\x61rbon_dioxide_detector\x18\x1f \x01(\x0b\x32).vemmiopb.CarbonDioxideDetectorCapabilityH\x00\x12.\n\x07voltage\x18  \x01(\x0b\x32\x1b.vemmiopb.VoltageCapabilityH\x00\x12\x36\n\x0bultraviolet\x18! \x01(\x0b\x32\x1f.vemmiopb.UltravioletCapabilityH\x00\x42\x0c\n\ncapability\"\x12\n\x10SwitchCapability\"?\n\x0fMeterCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05reset\x18\x02 \x01(\x08\"\x15\n\x13OpenCloseCapability\"\x19\n\x17SmokeDetectorCapability\"\x1a\n\x18MotionDetectorCapability\"\x19\n\x17\x46loodDetectorCapability\"A\n CarbonMonoxideDetectorCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\"!\n\x1f\x43\x61rbonDioxideDetectorCapability\"I\n\x14ThermostatCapability\x12\x31\n\x06ranges\x18\x01 \x03(\x0b\x32!.vemmiopb.ThermostatSetpointRange\"6\n\x15TemperatureCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\"3\n\x12HumidityCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\"7\n\x16IlluminationCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\"4\n\x13\x44irectionCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\"\x12\n\x10TamperCapability\"\x15\n\x13\x45mergencyCapability\"\x10\n\x0e\x44oorCapability\"\x12\n\x10TapTapCapability\"?\n\x0f\x43olorCapability\x12,\n\ncomponents\x18\x01 \x03(\x0e\x32\x18.vemmiopb.ColorComponent\"\x11\n\x0fLevelCapability\"\x13\n\x11\x42\x61tteryCapability\"\x10\n\x0eLockCapability\"\x12\n\x10RemoteCapability\"C\n\x15PowerSourceCapability\x12*\n\x06\x65vents\x18\x01 \x03(\x0e\x32\x1a.vemmiopb.PowerSourceEvent\"\x19\n\x17RollerShutterCapability\"\x19\n\x17\x43onfigurationCapability\"\x14\n\x12\x44oorbellCapability\"\x11\n\x0fSirenCapability\"\xa1\x01\n\x17\x41\x63\x63\x65lerometerCapability\x12\x34\n\x04\x61xes\x18\x01 \x03(\x0b\x32&.vemmiopb.AccelerometerCapability.Axis\x1aP\n\x04\x41xis\x12)\n\x04\x61xis\x18\x01 \x01(\x0e\x32\x1b.vemmiopb.AccelerometerAxis\x12\x1d\n\x05units\x18\x02 \x03(\x0e\x32\x0e.vemmiopb.Unit\"Y\n\x11SeismicCapability\x12!\n\tintensity\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\x12!\n\tmagnitude\x18\x02 \x03(\x0e\x32\x0e.vemmiopb.Unit\"2\n\x11VoltageCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit\"6\n\x15UltravioletCapability\x12\x1d\n\x05units\x18\x01 \x03(\x0e\x32\x0e.vemmiopb.Unit2U\n\x07\x44\x65vices\x12J\n\x0b\x44\x65vicesList\x12\x1c.vemmiopb.DevicesListRequest\x1a\x1d.vemmiopb.DevicesListResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.devices_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _DEVICESLISTREQUEST._serialized_start=191
   _DEVICESLISTREQUEST._serialized_end=211
   _DEVICESLISTRESPONSE._serialized_start=213
   _DEVICESLISTRESPONSE._serialized_end=269
```

### Comparing `aiomagra-0.1.1/src/aiomagra/door_pb2.py` & `aiomagra-0.1.2/src/aiomagra/door_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/door.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61iomagra/door.proto\x12\x08vemmiopb\"0\n\nDoorReport\x12\"\n\x05\x65vent\x18\x01 \x01(\x0e\x32\x13.vemmiopb.DoorEvent*V\n\tDoorEvent\x12\x18\n\x14\x44OOR_EVENT_INTRUSION\x10\x00\x12\x19\n\x15\x44OOR_EVENT_HARD_KNOCK\x10\x01\x12\x14\n\x10\x44OOR_EVENT_KNOCK\x10\x02\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.door_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _DOOREVENT._serialized_start=83
   _DOOREVENT._serialized_end=169
   _DOORREPORT._serialized_start=33
   _DOORREPORT._serialized_end=81
```

### Comparing `aiomagra-0.1.1/src/aiomagra/doorbell_pb2.py` & `aiomagra-0.1.2/src/aiomagra/doorbell_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/doorbell.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x61iomagra/doorbell.proto\x12\x08vemmiopb\"_\n\x0e\x44oorbellReport\x12-\n\x05state\x18\x01 \x01(\x0e\x32\x1e.vemmiopb.DoorbellReport.State\"\x1e\n\x05State\x12\t\n\x05\x43LEAR\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.doorbell_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _DOORBELLREPORT._serialized_start=37
   _DOORBELLREPORT._serialized_end=132
   _DOORBELLREPORT_STATE._serialized_start=102
   _DOORBELLREPORT_STATE._serialized_end=132
```

### Comparing `aiomagra-0.1.1/src/aiomagra/emergency_pb2.py` & `aiomagra-0.1.2/src/aiomagra/emergency_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/emergency.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61iomagra/emergency.proto\x12\x08vemmiopb\"8\n\x0f\x45mergencyReport\x12%\n\x04type\x18\x01 \x01(\x0e\x32\x17.vemmiopb.EmergencyType*P\n\rEmergencyType\x12\x14\n\x10\x45MERGENCY_POLICE\x10\x00\x12\x12\n\x0e\x45MERGENCY_FIRE\x10\x01\x12\x15\n\x11\x45MERGENCY_MEDICAL\x10\x02\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.emergency_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _EMERGENCYTYPE._serialized_start=96
   _EMERGENCYTYPE._serialized_end=176
   _EMERGENCYREPORT._serialized_start=38
   _EMERGENCYREPORT._serialized_end=94
```

### Comparing `aiomagra-0.1.1/src/aiomagra/firmware.proto` & `aiomagra-0.1.2/src/aiomagra/firmware.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/firmware_pb2.py` & `aiomagra-0.1.2/src/aiomagra/firmware_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/firmware.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x61iomagra/firmware.proto\x12\x08vemmiopb\",\n\rFirmwareChunk\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\r\n\x05index\x18\x02 \x01(\x05\"$\n\x10\x46irmwareChunkAck\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\":\n\x16\x46irmwareUpgradeRequest\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0e\n\x06sha256\x18\x02 \x01(\t\"\x14\n\x12\x46irmwareUpgradeAck\"(\n\x15\x46irmwareUpdateRequest\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x18\n\x16\x46irmwareUpdateResponse\"\x1e\n\x1c\x46irmwareLatestVersionRequest\"0\n\x1d\x46irmwareLatestVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"o\n\x1a\x46irmwareUpdateStatusReport\x12.\n\x06status\x18\x01 \x01(\x0e\x32\x1e.vemmiopb.FirmwareUpdateStatus\x12\x10\n\x08progress\x18\x02 \x01(\r\x12\x0f\n\x07version\x18\x03 \x01(\t*\xd1\x01\n\x14\x46irmwareUpdateStatus\x12\"\n\x1e\x46IRMWARE_UPDATE_STATUS_UNKNOWN\x10\x00\x12&\n\"FIRMWARE_UPDATE_STATUS_IN_PROGRESS\x10\x01\x12#\n\x1f\x46IRMWARE_UPDATE_STATUS_COMPLETE\x10\x02\x12!\n\x1d\x46IRMWARE_UPDATE_STATUS_FAILED\x10\x03\x12%\n!FIRMWARE_UPDATE_STATUS_UP_TO_DATE\x10\x04\x32\xac\x01\n\x08\x46irmware\x12I\n\x0e\x46irmwareUpload\x12\x17.vemmiopb.FirmwareChunk\x1a\x1a.vemmiopb.FirmwareChunkAck(\x01\x30\x01\x12U\n\x0f\x46irmwareUpgrade\x12 .vemmiopb.FirmwareUpgradeRequest\x1a\x1c.vemmiopb.FirmwareUpgradeAck(\x01\x30\x01\x32\xd0\x01\n\x0f\x46irmwareService\x12S\n\x0e\x46irmwareUpdate\x12\x1f.vemmiopb.FirmwareUpdateRequest\x1a .vemmiopb.FirmwareUpdateResponse\x12h\n\x15\x46irmwareLatestVersion\x12&.vemmiopb.FirmwareLatestVersionRequest\x1a\'.vemmiopb.FirmwareLatestVersionResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.firmware_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _FIRMWAREUPDATESTATUS._serialized_start=467
   _FIRMWAREUPDATESTATUS._serialized_end=676
   _FIRMWARECHUNK._serialized_start=37
   _FIRMWARECHUNK._serialized_end=81
```

### Comparing `aiomagra-0.1.1/src/aiomagra/flood_pb2.py` & `aiomagra-0.1.2/src/aiomagra/flood_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/flood.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/flood.proto\x12\x08vemmiopb\"X\n\x0b\x46loodReport\x12*\n\x05state\x18\x01 \x01(\x0e\x32\x1b.vemmiopb.FloodReport.State\"\x1d\n\x05State\x12\t\n\x05\x43LEAR\x10\x00\x12\t\n\x05\x46LOOD\x10\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.flood_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _FLOODREPORT._serialized_start=34
   _FLOODREPORT._serialized_end=122
   _FLOODREPORT_STATE._serialized_start=93
   _FLOODREPORT_STATE._serialized_end=122
```

### Comparing `aiomagra-0.1.1/src/aiomagra/gate.proto` & `aiomagra-0.1.2/src/aiomagra/gate.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/gate_pb2.py` & `aiomagra-0.1.2/src/aiomagra/gate_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/gate.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61iomagra/gate.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"9\n\x0bGateRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"\x0e\n\x0cGateResponse\"0\n\nGateReport\x12\"\n\x05state\x18\x01 \x01(\x0e\x32\x13.vemmiopb.GateState*P\n\tGateState\x12\x10\n\x0cGATE_UNKNOWN\x10\x00\x12\x0f\n\x0bGATE_OPENED\x10\x01\x12\x0f\n\x0bGATE_CLOSED\x10\x02\x12\x0f\n\x0bGATE_CYCLED\x10\x03\x32\xc0\x01\n\x0bGateService\x12\x39\n\x08GateOpen\x12\x15.vemmiopb.GateRequest\x1a\x16.vemmiopb.GateResponse\x12:\n\tGateClose\x12\x15.vemmiopb.GateRequest\x1a\x16.vemmiopb.GateResponse\x12:\n\tGateCycle\x12\x15.vemmiopb.GateRequest\x1a\x16.vemmiopb.GateResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.gate_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _GATESTATE._serialized_start=183
   _GATESTATE._serialized_end=263
   _GATEREQUEST._serialized_start=58
   _GATEREQUEST._serialized_end=115
```

### Comparing `aiomagra-0.1.1/src/aiomagra/gateway.proto` & `aiomagra-0.1.2/src/aiomagra/gateway.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/gateway_pb2.py` & `aiomagra-0.1.2/src/aiomagra/gateway_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/gateway.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61iomagra/gateway.proto\x12\x08vemmiopb\"\x0f\n\rRebootRequest\"\x10\n\x0eRebootResponse\"\x1e\n\x0eRestartRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x11\n\x0fRestartResponse\"\x10\n\x0eSupportRequest\"\x11\n\x0fSupportResponse2\x8f\x02\n\x07Gateway\x12;\n\x06Reboot\x12\x17.vemmiopb.RebootRequest\x1a\x18.vemmiopb.RebootResponse\x12>\n\x07Restart\x12\x18.vemmiopb.RestartRequest\x1a\x19.vemmiopb.RestartResponse\x12\x43\n\x0cStartSupport\x12\x18.vemmiopb.SupportRequest\x1a\x19.vemmiopb.SupportResponse\x12\x42\n\x0bStopSupport\x12\x18.vemmiopb.SupportRequest\x1a\x19.vemmiopb.SupportResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.gateway_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _REBOOTREQUEST._serialized_start=36
   _REBOOTREQUEST._serialized_end=51
   _REBOOTRESPONSE._serialized_start=53
   _REBOOTRESPONSE._serialized_end=69
```

### Comparing `aiomagra-0.1.1/src/aiomagra/heartbeat_pb2.py` & `aiomagra-0.1.2/src/aiomagra/heartbeat_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/heartbeat.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61iomagra/heartbeat.proto\x12\x08vemmiopb\"\x0e\n\x0cHeartbeatMsg2Q\n\tHeartbeat\x12\x44\n\x0eHeartbeatStart\x12\x16.vemmiopb.HeartbeatMsg\x1a\x16.vemmiopb.HeartbeatMsg(\x01\x30\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.heartbeat_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _HEARTBEATMSG._serialized_start=38
   _HEARTBEATMSG._serialized_end=52
   _HEARTBEAT._serialized_start=54
   _HEARTBEAT._serialized_end=135
```

### Comparing `aiomagra-0.1.1/src/aiomagra/info_pb2.py` & `aiomagra-0.1.2/src/aiomagra/info_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/info.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61iomagra/info.proto\x12\x08vemmiopb\"\r\n\x0bInfoRequest\"v\n\x0cInfoResponse\x12\x13\n\x0b\x63ommon_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\ngit_commit\x18\x03 \x01(\t\x12\x12\n\nbuild_time\x18\x04 \x01(\t\x12\x18\n\x10\x66irmware_version\x18\x05 \x01(\t2=\n\x04Info\x12\x35\n\x04Info\x12\x15.vemmiopb.InfoRequest\x1a\x16.vemmiopb.InfoResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.info_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _INFOREQUEST._serialized_start=33
   _INFOREQUEST._serialized_end=46
   _INFORESPONSE._serialized_start=48
   _INFORESPONSE._serialized_end=166
```

### Comparing `aiomagra-0.1.1/src/aiomagra/level.proto` & `aiomagra-0.1.2/src/aiomagra/level.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/level_pb2.py` & `aiomagra-0.1.2/src/aiomagra/level_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/level.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/level.proto\x12\x08vemmiopb\x1a\x1egoogle/protobuf/duration.proto\x1a\x17\x61iomagra/metadata.proto\":\n\x0cLevelRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"\x0f\n\rLevelResponse\"L\n\x0fLevelSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\r\n\x05value\x18\x02 \x01(\x05\"\x8f\x01\n\x10LevelStepRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12&\n\x03\x64im\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\'\n\x04\x64own\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"!\n\x10LevelGetResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1c\n\x0bLevelReport\x12\r\n\x05value\x18\x01 \x01(\x05\x32\xd9\x03\n\x05Level\x12>\n\x08LevelGet\x12\x16.vemmiopb.LevelRequest\x1a\x1a.vemmiopb.LevelGetResponse\x12\x42\n\x0cLevelGetStep\x12\x16.vemmiopb.LevelRequest\x1a\x1a.vemmiopb.LevelGetResponse\x12>\n\x08LevelSet\x12\x19.vemmiopb.LevelSetRequest\x1a\x17.vemmiopb.LevelResponse\x12>\n\x07LevelUp\x12\x1a.vemmiopb.LevelStepRequest\x1a\x17.vemmiopb.LevelResponse\x12@\n\tLevelDown\x12\x1a.vemmiopb.LevelStepRequest\x1a\x17.vemmiopb.LevelResponse\x12\x44\n\rLevelIncrease\x12\x1a.vemmiopb.LevelStepRequest\x1a\x17.vemmiopb.LevelResponse\x12\x44\n\rLevelDecrease\x12\x1a.vemmiopb.LevelStepRequest\x1a\x17.vemmiopb.LevelResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.level_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _LEVELREQUEST._serialized_start=91
   _LEVELREQUEST._serialized_end=149
   _LEVELRESPONSE._serialized_start=151
   _LEVELRESPONSE._serialized_end=166
```

### Comparing `aiomagra-0.1.1/src/aiomagra/lock.proto` & `aiomagra-0.1.2/src/aiomagra/lock.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/lock_pb2.py` & `aiomagra-0.1.2/src/aiomagra/lock_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/lock.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61iomagra/lock.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"^\n\x0eLockSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12 \n\x04mode\x18\x02 \x01(\x0e\x32\x12.vemmiopb.LockMode\"\x0e\n\x0cLockResponse\".\n\nLockReport\x12 \n\x04mode\x18\x01 \x01(\x0e\x32\x12.vemmiopb.LockMode*\xac\x01\n\x08LockMode\x12\x0e\n\nLOCK_UNSEC\x10\x00\x12\x14\n\x10LOCK_UNSEC_TMOUT\x10\x01\x12\x11\n\rLOCK_UNSEC_IN\x10\x10\x12\x17\n\x13LOCK_UNSEC_IN_TMOUT\x10\x11\x12\x12\n\x0eLOCK_UNSEC_OUT\x10 \x12\x18\n\x14LOCK_UNSEC_OUT_TMOUT\x10!\x12\x11\n\x0cLOCK_UNKNOWN\x10\xfe\x01\x12\r\n\x08LOCK_SEC\x10\xff\x01\x32\x43\n\x04Lock\x12;\n\x07LockSet\x12\x18.vemmiopb.LockSetRequest\x1a\x16.vemmiopb.LockResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.lock_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _LOCKMODE._serialized_start=219
   _LOCKMODE._serialized_end=391
   _LOCKSETREQUEST._serialized_start=58
   _LOCKSETREQUEST._serialized_end=152
```

### Comparing `aiomagra-0.1.1/src/aiomagra/messaging_pb2.py` & `aiomagra-0.1.2/src/aiomagra/sensor_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aiomagra/messaging.proto
+# source: aiomagra/sensor.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61iomagra/messaging.proto\x12\x08vemmiopb\"C\n\x0c\x45mailMessage\x12\x11\n\trecipient\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"`\n\x0bPushMessage\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x03 \x01(\x05\x12\x0f\n\x07site_id\x18\x04 \x01(\t\x12\x11\n\tsite_name\x18\x05 \x01(\tB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/sensor.proto\x12\x08vemmiopb\x1a\x14\x61iomagra/units.proto\"=\n\x0eHumidityReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"A\n\x12IlluminationReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\">\n\x0f\x44irectionReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x05\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.messaging_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.sensor_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
-  _EMAILMESSAGE._serialized_start=38
-  _EMAILMESSAGE._serialized_end=105
-  _PUSHMESSAGE._serialized_start=107
-  _PUSHMESSAGE._serialized_end=203
+  _HUMIDITYREPORT._serialized_start=57
+  _HUMIDITYREPORT._serialized_end=118
+  _ILLUMINATIONREPORT._serialized_start=120
+  _ILLUMINATIONREPORT._serialized_end=185
+  _DIRECTIONREPORT._serialized_start=187
+  _DIRECTIONREPORT._serialized_end=249
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aiomagra-0.1.1/src/aiomagra/metadata.proto` & `aiomagra-0.1.2/src/aiomagra/metadata.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/metadata_pb2.py` & `aiomagra-0.1.2/src/aiomagra/metadata_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/metadata.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x61iomagra/metadata.proto\x12\x08vemmiopb\"\xf4\x01\n\x0e\x44\x65viceMetadata\x12(\n\x05zwave\x18\x01 \x01(\x0b\x32\x17.vemmiopb.ZWaveMetadataH\x00\x12*\n\x06zigbee\x18\x02 \x01(\x0b\x32\x18.vemmiopb.ZigbeeMetadataH\x00\x12(\n\x05\x61\x64\x64on\x18\x03 \x01(\x0b\x32\x17.vemmiopb.AddonMetadataH\x00\x12(\n\x05\x61lias\x18\x05 \x01(\x0b\x32\x17.vemmiopb.AliasMetadataH\x00\x12&\n\x04mqtt\x18\x06 \x01(\x0b\x32\x16.vemmiopb.MQTTMetadataH\x00\x42\n\n\x08metadataJ\x04\x08\x04\x10\x05\"5\n\rZWaveMetadata\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x65ndpoint_id\x18\x02 \x01(\x05\"6\n\x0eZigbeeMetadata\x12\x12\n\neui64_addr\x18\x01 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x02 \x01(\x05\"\x1d\n\rAddonMetadata\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"\x1d\n\rAliasMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\"!\n\x0cMQTTMetadata\x12\x11\n\tdevice_id\x18\x01 \x01(\x0c\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.metadata_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _DEVICEMETADATA._serialized_start=38
   _DEVICEMETADATA._serialized_end=282
   _ZWAVEMETADATA._serialized_start=284
   _ZWAVEMETADATA._serialized_end=337
```

### Comparing `aiomagra-0.1.1/src/aiomagra/meter.proto` & `aiomagra-0.1.2/src/aiomagra/meter.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/meter_pb2.py` & `aiomagra-0.1.2/src/aiomagra/meter_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/meter.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/meter.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\x1a\x14\x61iomagra/units.proto\"[\n\x0fMeterGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\x1c\n\x04unit\x18\x02 \x01(\x0e\x32\x0e.vemmiopb.Unit\"?\n\x10MeterGetResponse\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"?\n\x11MeterResetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"\x14\n\x12MeterResetResponse\":\n\x0bMeterReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\x32\x93\x01\n\x05Meter\x12\x41\n\x08MeterGet\x12\x19.vemmiopb.MeterGetRequest\x1a\x1a.vemmiopb.MeterGetResponse\x12G\n\nMeterReset\x12\x1b.vemmiopb.MeterResetRequest\x1a\x1c.vemmiopb.MeterResetResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.meter_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _METERGETREQUEST._serialized_start=81
   _METERGETREQUEST._serialized_end=172
   _METERGETRESPONSE._serialized_start=174
   _METERGETRESPONSE._serialized_end=237
```

### Comparing `aiomagra-0.1.1/src/aiomagra/power_source.proto` & `aiomagra-0.1.2/src/aiomagra/power_source.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/power_source_pb2.py` & `aiomagra-0.1.2/src/aiomagra/power_source_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/power_source.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x61iomagra/power_source.proto\x12\x08vemmiopb\">\n\x11PowerSourceReport\x12)\n\x05\x65vent\x18\x01 \x01(\x0e\x32\x1a.vemmiopb.PowerSourceEvent*\xe8\x02\n\x10PowerSourceEvent\x12\t\n\x05\x43LEAR\x10\x00\x12\x11\n\rPOWER_APPLIED\x10\x01\x12\x11\n\rAC_POWER_LOST\x10\x02\x12\x15\n\x11\x41\x43_POWER_RESTORED\x10\x03\x12\x12\n\x0eSURGE_DETECTED\x10\x04\x12\x15\n\x11\x42ROWNOUT_DETECTED\x10\x05\x12\x19\n\x15OVER_CURRENT_DETECTED\x10\x06\x12\x19\n\x15OVER_VOLTAGE_DETECTED\x10\x07\x12\x16\n\x12OVER_LOAD_DETECTED\x10\x08\x12\x0e\n\nLOAD_ERROR\x10\t\x12\x18\n\x14\x42\x41TTERY_REPLACE_SOON\x10\n\x12\x17\n\x13\x42\x41TTERY_REPLACE_NOW\x10\x0b\x12\x14\n\x10\x42\x41TTERY_CHARGING\x10\x0c\x12\x13\n\x0f\x42\x41TTERY_CHARGED\x10\r\x12\x0f\n\x0b\x42\x41TTERY_LOW\x10\x0e\x12\x14\n\x10\x42\x41TTERY_CRITICAL\x10\x0f\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.power_source_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _POWERSOURCEEVENT._serialized_start=106
   _POWERSOURCEEVENT._serialized_end=466
   _POWERSOURCEREPORT._serialized_start=41
   _POWERSOURCEREPORT._serialized_end=103
```

### Comparing `aiomagra-0.1.1/src/aiomagra/pubsub.proto` & `aiomagra-0.1.2/src/aiomagra/pubsub.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/pubsub_pb2.py` & `aiomagra-0.1.2/src/aiomagra/pubsub_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,55 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/pubsub.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import addon_pb2 as aiomagra_dot_addon__pb2
+from aiomagra import admin_pb2 as aiomagra_dot_admin__pb2
+from aiomagra import battery_pb2 as aiomagra_dot_battery__pb2
+from aiomagra import ble_pb2 as aiomagra_dot_ble__pb2
+from aiomagra import carbon_monoxide_pb2 as aiomagra_dot_carbon__monoxide__pb2
+from aiomagra import color_pb2 as aiomagra_dot_color__pb2
+from aiomagra import configuration_pb2 as aiomagra_dot_configuration__pb2
+from aiomagra import devices_pb2 as aiomagra_dot_devices__pb2
+from aiomagra import firmware_pb2 as aiomagra_dot_firmware__pb2
+from aiomagra import gate_pb2 as aiomagra_dot_gate__pb2
+from aiomagra import gateway_pb2 as aiomagra_dot_gateway__pb2
+from aiomagra import info_pb2 as aiomagra_dot_info__pb2
+from aiomagra import level_pb2 as aiomagra_dot_level__pb2
+from aiomagra import lock_pb2 as aiomagra_dot_lock__pb2
+from aiomagra import messaging_pb2 as aiomagra_dot_messaging__pb2
+from aiomagra import meter_pb2 as aiomagra_dot_meter__pb2
+from aiomagra import remote_pb2 as aiomagra_dot_remote__pb2
+from aiomagra import roller_shutter_pb2 as aiomagra_dot_roller__shutter__pb2
+from aiomagra import siren_pb2 as aiomagra_dot_siren__pb2
+from aiomagra import status_pb2 as aiomagra_dot_status__pb2
+from aiomagra import structure_pb2 as aiomagra_dot_structure__pb2
+from aiomagra import switch_pb2 as aiomagra_dot_switch__pb2
+from aiomagra import temperature_pb2 as aiomagra_dot_temperature__pb2
+from aiomagra import thermostat_pb2 as aiomagra_dot_thermostat__pb2
+from aiomagra import ultraviolet_pb2 as aiomagra_dot_ultraviolet__pb2
+from aiomagra import wifi_pb2 as aiomagra_dot_wifi__pb2
+from aiomagra import zigbee_pb2 as aiomagra_dot_zigbee__pb2
+from aiomagra import zwave_pb2 as aiomagra_dot_zwave__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/pubsub.proto\x12\x08vemmiopb\x1a\x14\x61iomagra/addon.proto\x1a\x14\x61iomagra/admin.proto\x1a\x16\x61iomagra/battery.proto\x1a\x12\x61iomagra/ble.proto\x1a\x1e\x61iomagra/carbon_monoxide.proto\x1a\x14\x61iomagra/color.proto\x1a\x1c\x61iomagra/configuration.proto\x1a\x16\x61iomagra/devices.proto\x1a\x17\x61iomagra/firmware.proto\x1a\x13\x61iomagra/gate.proto\x1a\x16\x61iomagra/gateway.proto\x1a\x13\x61iomagra/info.proto\x1a\x14\x61iomagra/level.proto\x1a\x13\x61iomagra/lock.proto\x1a\x18\x61iomagra/messaging.proto\x1a\x14\x61iomagra/meter.proto\x1a\x15\x61iomagra/remote.proto\x1a\x1d\x61iomagra/roller_shutter.proto\x1a\x14\x61iomagra/siren.proto\x1a\x15\x61iomagra/status.proto\x1a\x18\x61iomagra/structure.proto\x1a\x15\x61iomagra/switch.proto\x1a\x1a\x61iomagra/temperature.proto\x1a\x19\x61iomagra/thermostat.proto\x1a\x1a\x61iomagra/ultraviolet.proto\x1a\x13\x61iomagra/wifi.proto\x1a\x15\x61iomagra/zigbee.proto\x1a\x14\x61iomagra/zwave.proto\"0\n\x13MetricsNotification\x12\x0b\n\x03mac\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x03(\x0c\"v\n\x14PresenceNotification\x12\x0b\n\x03mac\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\ngit_commit\x18\x03 \x01(\t\x12\x12\n\nbuild_time\x18\x04 \x01(\t\x12\x18\n\x10\x66irmware_version\x18\x05 \x01(\t\"\xba\x01\n\x0e\x43ommandRequest\x12\x0e\n\x06method\x18\x01 \x01(\t\x12*\n\x04type\x18\x02 \x01(\x0e\x32\x1c.vemmiopb.CommandRequestType\x12*\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1c.vemmiopb.CommandRequestData\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\x12/\n\x07options\x18\x05 \x03(\x0e\x32\x1e.vemmiopb.CommandRequestOption\"\x9f\x01\n\x0c\x43ommandReply\x12(\n\x04type\x18\x01 \x01(\x0e\x32\x1a.vemmiopb.CommandReplyType\x12*\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1b.vemmiopb.CommandReplyError\x12(\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1a.vemmiopb.CommandReplyData\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\"$\n\x11\x43ommandReplyError\x12\x0f\n\x07message\x18\x01 \x01(\t\"m\n\x10MessagingRequest\x12\'\n\x05\x65mail\x18\x01 \x01(\x0b\x32\x16.vemmiopb.EmailMessageH\x00\x12%\n\x04push\x18\x02 \x01(\x0b\x32\x15.vemmiopb.PushMessageH\x00\x42\t\n\x07message\"\xe3#\n\x12\x43ommandRequestData\x12/\n\tAddonList\x18\x01 \x01(\x0b\x32\x1a.vemmiopb.AddonListRequestH\x00\x12\x41\n\x12\x41\x64\x64onAddThermostat\x18\x02 \x01(\x0b\x32#.vemmiopb.AddonAddThermostatRequestH\x00\x12/\n\tWalkNodes\x18\x65 \x01(\x0b\x32\x1a.vemmiopb.WalkNodesRequestH\x00\x12)\n\x08ReadLogs\x18\x66 \x01(\x0b\x32\x15.vemmiopb.LogsRequestH\x00\x12+\n\nFollowLogs\x18g \x01(\x0b\x32\x15.vemmiopb.LogsRequestH\x00\x12\x32\n\nBatteryGet\x18\x91\x03 \x01(\x0b\x32\x1b.vemmiopb.BatteryGetRequestH\x00\x12.\n\x08\x43olorSet\x18\xf5\x03 \x01(\x0b\x32\x19.vemmiopb.ColorSetRequestH\x00\x12@\n\x11\x43onfigurationList\x18\xd9\x04 \x01(\x0b\x32\".vemmiopb.ConfigurationListRequestH\x00\x12>\n\x10\x43onfigurationGet\x18\xda\x04 \x01(\x0b\x32!.vemmiopb.ConfigurationGetRequestH\x00\x12>\n\x10\x43onfigurationSet\x18\xdb\x04 \x01(\x0b\x32!.vemmiopb.ConfigurationSetRequestH\x00\x12@\n\x11ThermostatModeSet\x18\xbd\x05 \x01(\x0b\x32\".vemmiopb.ThermostatModeSetRequestH\x00\x12\x46\n\x14ThermostatModeSupGet\x18\xbe\x05 \x01(\x0b\x32%.vemmiopb.ThermostatModeSupGetRequestH\x00\x12H\n\x15ThermostatSetpointSet\x18\xbf\x05 \x01(\x0b\x32&.vemmiopb.ThermostatSetpointSetRequestH\x00\x12\x46\n\x14ThermostatFanModeSet\x18\xc0\x05 \x01(\x0b\x32%.vemmiopb.ThermostatFanModeSetRequestH\x00\x12\x34\n\x0b\x44\x65vicesList\x18\xa1\x06 \x01(\x0b\x32\x1c.vemmiopb.DevicesListRequestH\x00\x12\x32\n\x0e\x46irmwareUpload\x18\x85\x07 \x01(\x0b\x32\x17.vemmiopb.FirmwareChunkH\x00\x12<\n\x0f\x46irmwareUpgrade\x18\x86\x07 \x01(\x0b\x32 .vemmiopb.FirmwareUpgradeRequestH\x00\x12:\n\x0e\x46irmwareUpdate\x18\x87\x07 \x01(\x0b\x32\x1f.vemmiopb.FirmwareUpdateRequestH\x00\x12H\n\x15\x46irmwareLatestVersion\x18\x88\x07 \x01(\x0b\x32&.vemmiopb.FirmwareLatestVersionRequestH\x00\x12*\n\x06Reboot\x18\xe9\x07 \x01(\x0b\x32\x17.vemmiopb.RebootRequestH\x00\x12,\n\x07Restart\x18\xea\x07 \x01(\x0b\x32\x18.vemmiopb.RestartRequestH\x00\x12\x31\n\x0cStartSupport\x18\xeb\x07 \x01(\x0b\x32\x18.vemmiopb.SupportRequestH\x00\x12\x30\n\x0bStopSupport\x18\xec\x07 \x01(\x0b\x32\x18.vemmiopb.SupportRequestH\x00\x12&\n\x04Info\x18\xcd\x08 \x01(\x0b\x32\x15.vemmiopb.InfoRequestH\x00\x12+\n\x08LevelGet\x18\xb1\t \x01(\x0b\x32\x16.vemmiopb.LevelRequestH\x00\x12/\n\x0cLevelGetStep\x18\xb2\t \x01(\x0b\x32\x16.vemmiopb.LevelRequestH\x00\x12.\n\x08LevelSet\x18\xb3\t \x01(\x0b\x32\x19.vemmiopb.LevelSetRequestH\x00\x12.\n\x07LevelUp\x18\xb4\t \x01(\x0b\x32\x1a.vemmiopb.LevelStepRequestH\x00\x12\x30\n\tLevelDown\x18\xb5\t \x01(\x0b\x32\x1a.vemmiopb.LevelStepRequestH\x00\x12\x34\n\rLevelIncrease\x18\xb6\t \x01(\x0b\x32\x1a.vemmiopb.LevelStepRequestH\x00\x12\x34\n\rLevelDecrease\x18\xb7\t \x01(\x0b\x32\x1a.vemmiopb.LevelStepRequestH\x00\x12,\n\x07LockSet\x18\x95\n \x01(\x0b\x32\x18.vemmiopb.LockSetRequestH\x00\x12.\n\x08MeterGet\x18\xf9\n \x01(\x0b\x32\x19.vemmiopb.MeterGetRequestH\x00\x12\x32\n\nMeterReset\x18\xfa\n \x01(\x0b\x32\x1b.vemmiopb.MeterResetRequestH\x00\x12<\n\x11RollerShutterOpen\x18\xdd\x0b \x01(\x0b\x32\x1e.vemmiopb.RollerShutterRequestH\x00\x12=\n\x12RollerShutterClose\x18\xde\x0b \x01(\x0b\x32\x1e.vemmiopb.RollerShutterRequestH\x00\x12>\n\x10RollerShutterSet\x18\xdf\x0b \x01(\x0b\x32!.vemmiopb.RollerShutterSetRequestH\x00\x12\x38\n\rSirenGetTones\x18\xc1\x0c \x01(\x0b\x32\x1e.vemmiopb.SirenGetTonesRequestH\x00\x12\x38\n\rSirenPlayTone\x18\xc2\x0c \x01(\x0b\x32\x1e.vemmiopb.SirenPlayToneRequestH\x00\x12\x46\n\x14SirenPlayDefaultTone\x18\xc3\x0c \x01(\x0b\x32%.vemmiopb.SirenPlayDefaultToneRequestH\x00\x12\x44\n\x13SirenGetDefaultTone\x18\xc4\x0c \x01(\x0b\x32$.vemmiopb.SirenGetDefaultToneRequestH\x00\x12\x44\n\x13SirenSetDefaultTone\x18\xc5\x0c \x01(\x0b\x32$.vemmiopb.SirenSetDefaultToneRequestH\x00\x12:\n\x0eSirenGetVolume\x18\xc6\x0c \x01(\x0b\x32\x1f.vemmiopb.SirenGetVolumeRequestH\x00\x12:\n\x0eSirenSetVolume\x18\xc7\x0c \x01(\x0b\x32\x1f.vemmiopb.SirenSetVolumeRequestH\x00\x12,\n\x08SwitchOn\x18\xa5\r \x01(\x0b\x32\x17.vemmiopb.SwitchRequestH\x00\x12-\n\tSwitchOff\x18\xa6\r \x01(\x0b\x32\x17.vemmiopb.SwitchRequestH\x00\x12:\n\x0eTemperatureGet\x18\x89\x0e \x01(\x0b\x32\x1f.vemmiopb.TemperatureGetRequestH\x00\x12\x30\n\tWiFiQuery\x18\xed\x0e \x01(\x0b\x32\x1a.vemmiopb.WiFiQueryRequestH\x00\x12.\n\x08WiFiScan\x18\xee\x0e \x01(\x0b\x32\x19.vemmiopb.WiFiScanRequestH\x00\x12\x34\n\x0bWiFiConnect\x18\xef\x0e \x01(\x0b\x32\x1c.vemmiopb.WiFiConnectRequestH\x00\x12\x38\n\rZigbeeInclude\x18\xd1\x0f \x01(\x0b\x32\x1e.vemmiopb.ZigbeeIncludeRequestH\x00\x12\x38\n\rZigbeeExclude\x18\xd2\x0f \x01(\x0b\x32\x1e.vemmiopb.ZigbeeExcludeRequestH\x00\x12\x37\n\x0eZigbeeGetNodes\x18\xd3\x0f \x01(\x0b\x32\x1c.vemmiopb.ZigbeeNodesRequestH\x00\x12\x36\n\x0cZWaveInclude\x18\xb5\x10 \x01(\x0b\x32\x1d.vemmiopb.ZWaveIncludeRequestH\x00\x12\x36\n\x0cZWaveExclude\x18\xb6\x10 \x01(\x0b\x32\x1d.vemmiopb.ZWaveExcludeRequestH\x00\x12\x32\n\nZWaveAbort\x18\xb7\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveAbortRequestH\x00\x12\x36\n\x0eZWaveReadNodes\x18\xb8\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveNodesRequestH\x00\x12\x34\n\x0bZWaveUpdate\x18\xbb\x10 \x01(\x0b\x32\x1c.vemmiopb.ZWaveUpdateRequestH\x00\x12<\n\x0fZWaveUpdateNode\x18\xbc\x10 \x01(\x0b\x32 .vemmiopb.ZWaveUpdateNodeRequestH\x00\x12\x32\n\nZWaveReset\x18\xbd\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveResetRequestH\x00\x12>\n\x10ZWaveListEntries\x18\xbe\x10 \x01(\x0b\x32!.vemmiopb.ZWaveListEntriesRequestH\x00\x12\x38\n\rZWaveAddEntry\x18\xbf\x10 \x01(\x0b\x32\x1e.vemmiopb.ZWaveAddEntryRequestH\x00\x12>\n\x10ZWaveRemoveEntry\x18\xc0\x10 \x01(\x0b\x32!.vemmiopb.ZWaveRemoveEntryRequestH\x00\x12J\n\x16ZWaveNotificationItems\x18\xc1\x10 \x01(\x0b\x32\'.vemmiopb.ZWaveNotificationItemsRequestH\x00\x12\x30\n\tZWaveTest\x18\xc2\x10 \x01(\x0b\x32\x1a.vemmiopb.ZWaveTestRequestH\x00\x12\x30\n\tZWaveHeal\x18\xc3\x10 \x01(\x0b\x32\x1a.vemmiopb.ZWaveHealRequestH\x00\x12\x42\n\x12ZWaveReplaceFailed\x18\xc4\x10 \x01(\x0b\x32#.vemmiopb.ZWaveReplaceFailedRequestH\x00\x12@\n\x11ZWaveRemoveFailed\x18\xc5\x10 \x01(\x0b\x32\".vemmiopb.ZWaveRemoveFailedRequestH\x00\x12>\n\x10ZWaveHealthCheck\x18\xc6\x10 \x01(\x0b\x32!.vemmiopb.ZWaveHealthCheckRequestH\x00\x12\x34\n\rZWaveReadNode\x18\xc7\x10 \x01(\x0b\x32\x1a.vemmiopb.ZWaveNodeRequestH\x00\x12@\n\x11\x43\x61rbonMonoxideGet\x18\x99\x11 \x01(\x0b\x32\".vemmiopb.CarbonMonoxideGetRequestH\x00\x12:\n\x11\x45nableAdvertising\x18\xfd\x11 \x01(\x0b\x32\x1c.vemmiopb.AdvertisingRequestH\x00\x12;\n\x12\x44isableAdvertising\x18\xfe\x11 \x01(\x0b\x32\x1c.vemmiopb.AdvertisingRequestH\x00\x12:\n\x0eUltravioletGet\x18\xe1\x12 \x01(\x0b\x32\x1f.vemmiopb.UltravioletGetRequestH\x00\x12)\n\x05KeyUp\x18\xc5\x13 \x01(\x0b\x32\x17.vemmiopb.RemoteRequestH\x00\x12+\n\x07KeyDown\x18\xc6\x13 \x01(\x0b\x32\x17.vemmiopb.RemoteRequestH\x00\x12*\n\x08GateOpen\x18\xa9\x14 \x01(\x0b\x32\x15.vemmiopb.GateRequestH\x00\x12+\n\tGateClose\x18\xaa\x14 \x01(\x0b\x32\x15.vemmiopb.GateRequestH\x00\x12+\n\tGateCycle\x18\xab\x14 \x01(\x0b\x32\x15.vemmiopb.GateRequestH\x00\x12\x34\n\x0bStatusCheck\x18\x8d\x15 \x01(\x0b\x32\x1c.vemmiopb.StatusCheckRequestH\x00\x12\x33\n\x0cGetStructure\x18\xf1\x15 \x01(\x0b\x32\x1a.vemmiopb.StructureRequestH\x00\x42\x06\n\x04\x64\x61ta\"\xe5#\n\x10\x43ommandReplyData\x12\x30\n\tAddonList\x18\x01 \x01(\x0b\x32\x1b.vemmiopb.AddonListResponseH\x00\x12\x38\n\x12\x41\x64\x64onAddThermostat\x18\x02 \x01(\x0b\x32\x1a.vemmiopb.AddonAddResponseH\x00\x12\x30\n\tWalkNodes\x18\x65 \x01(\x0b\x32\x1b.vemmiopb.WalkNodesResponseH\x00\x12\'\n\x08ReadLogs\x18\x66 \x01(\x0b\x32\x13.vemmiopb.LogsChunkH\x00\x12)\n\nFollowLogs\x18g \x01(\x0b\x32\x13.vemmiopb.LogsChunkH\x00\x12\x33\n\nBatteryGet\x18\x91\x03 \x01(\x0b\x32\x1c.vemmiopb.BatteryGetResponseH\x00\x12,\n\x08\x43olorSet\x18\xf5\x03 \x01(\x0b\x32\x17.vemmiopb.ColorResponseH\x00\x12\x41\n\x11\x43onfigurationList\x18\xd9\x04 \x01(\x0b\x32#.vemmiopb.ConfigurationListResponseH\x00\x12?\n\x10\x43onfigurationGet\x18\xda\x04 \x01(\x0b\x32\".vemmiopb.ConfigurationGetResponseH\x00\x12?\n\x10\x43onfigurationSet\x18\xdb\x04 \x01(\x0b\x32\".vemmiopb.ConfigurationSetResponseH\x00\x12:\n\x11ThermostatModeSet\x18\xbd\x05 \x01(\x0b\x32\x1c.vemmiopb.ThermostatResponseH\x00\x12G\n\x14ThermostatModeSupGet\x18\xbe\x05 \x01(\x0b\x32&.vemmiopb.ThermostatModeSupGetResponseH\x00\x12>\n\x15ThermostatSetpointSet\x18\xbf\x05 \x01(\x0b\x32\x1c.vemmiopb.ThermostatResponseH\x00\x12=\n\x14ThermostatFanModeSet\x18\xc0\x05 \x01(\x0b\x32\x1c.vemmiopb.ThermostatResponseH\x00\x12\x35\n\x0b\x44\x65vicesList\x18\xa1\x06 \x01(\x0b\x32\x1d.vemmiopb.DevicesListResponseH\x00\x12\x35\n\x0e\x46irmwareUpload\x18\x85\x07 \x01(\x0b\x32\x1a.vemmiopb.FirmwareChunkAckH\x00\x12\x38\n\x0f\x46irmwareUpgrade\x18\x86\x07 \x01(\x0b\x32\x1c.vemmiopb.FirmwareUpgradeAckH\x00\x12;\n\x0e\x46irmwareUpdate\x18\x87\x07 \x01(\x0b\x32 .vemmiopb.FirmwareUpdateResponseH\x00\x12I\n\x15\x46irmwareLatestVersion\x18\x88\x07 \x01(\x0b\x32\'.vemmiopb.FirmwareLatestVersionResponseH\x00\x12+\n\x06Reboot\x18\xe9\x07 \x01(\x0b\x32\x18.vemmiopb.RebootResponseH\x00\x12-\n\x07Restart\x18\xea\x07 \x01(\x0b\x32\x19.vemmiopb.RestartResponseH\x00\x12\x32\n\x0cStartSupport\x18\xeb\x07 \x01(\x0b\x32\x19.vemmiopb.SupportResponseH\x00\x12\x31\n\x0bStopSupport\x18\xec\x07 \x01(\x0b\x32\x19.vemmiopb.SupportResponseH\x00\x12\'\n\x04Info\x18\xcd\x08 \x01(\x0b\x32\x16.vemmiopb.InfoResponseH\x00\x12/\n\x08LevelGet\x18\xb1\t \x01(\x0b\x32\x1a.vemmiopb.LevelGetResponseH\x00\x12\x33\n\x0cLevelGetStep\x18\xb2\t \x01(\x0b\x32\x1a.vemmiopb.LevelGetResponseH\x00\x12,\n\x08LevelSet\x18\xb3\t \x01(\x0b\x32\x17.vemmiopb.LevelResponseH\x00\x12+\n\x07LevelUp\x18\xb4\t \x01(\x0b\x32\x17.vemmiopb.LevelResponseH\x00\x12-\n\tLevelDown\x18\xb5\t \x01(\x0b\x32\x17.vemmiopb.LevelResponseH\x00\x12\x31\n\rLevelIncrease\x18\xb6\t \x01(\x0b\x32\x17.vemmiopb.LevelResponseH\x00\x12\x31\n\rLevelDecrease\x18\xb7\t \x01(\x0b\x32\x17.vemmiopb.LevelResponseH\x00\x12*\n\x07LockSet\x18\x95\n \x01(\x0b\x32\x16.vemmiopb.LockResponseH\x00\x12/\n\x08MeterGet\x18\xf9\n \x01(\x0b\x32\x1a.vemmiopb.MeterGetResponseH\x00\x12\x33\n\nMeterReset\x18\xfa\n \x01(\x0b\x32\x1c.vemmiopb.MeterResetResponseH\x00\x12=\n\x11RollerShutterOpen\x18\xdd\x0b \x01(\x0b\x32\x1f.vemmiopb.RollerShutterResponseH\x00\x12>\n\x12RollerShutterClose\x18\xde\x0b \x01(\x0b\x32\x1f.vemmiopb.RollerShutterResponseH\x00\x12<\n\x10RollerShutterSet\x18\xdf\x0b \x01(\x0b\x32\x1f.vemmiopb.RollerShutterResponseH\x00\x12\x39\n\rSirenGetTones\x18\xc1\x0c \x01(\x0b\x32\x1f.vemmiopb.SirenGetTonesResponseH\x00\x12\x39\n\rSirenPlayTone\x18\xc2\x0c \x01(\x0b\x32\x1f.vemmiopb.SirenPlayToneResponseH\x00\x12G\n\x14SirenPlayDefaultTone\x18\xc3\x0c \x01(\x0b\x32&.vemmiopb.SirenPlayDefaultToneResponseH\x00\x12\x45\n\x13SirenGetDefaultTone\x18\xc4\x0c \x01(\x0b\x32%.vemmiopb.SirenGetDefaultToneResponseH\x00\x12\x45\n\x13SirenSetDefaultTone\x18\xc5\x0c \x01(\x0b\x32%.vemmiopb.SirenSetDefaultToneResponseH\x00\x12;\n\x0eSirenGetVolume\x18\xc6\x0c \x01(\x0b\x32 .vemmiopb.SirenGetVolumeResponseH\x00\x12;\n\x0eSirenSetVolume\x18\xc7\x0c \x01(\x0b\x32 .vemmiopb.SirenSetVolumeResponseH\x00\x12-\n\x08SwitchOn\x18\xa5\r \x01(\x0b\x32\x18.vemmiopb.SwitchResponseH\x00\x12.\n\tSwitchOff\x18\xa6\r \x01(\x0b\x32\x18.vemmiopb.SwitchResponseH\x00\x12;\n\x0eTemperatureGet\x18\x89\x0e \x01(\x0b\x32 .vemmiopb.TemperatureGetResponseH\x00\x12\x31\n\tWiFiQuery\x18\xed\x0e \x01(\x0b\x32\x1b.vemmiopb.WiFiQueryResponseH\x00\x12/\n\x08WiFiScan\x18\xee\x0e \x01(\x0b\x32\x1a.vemmiopb.WiFiScanResponseH\x00\x12\x35\n\x0bWiFiConnect\x18\xef\x0e \x01(\x0b\x32\x1d.vemmiopb.WiFiConnectResponseH\x00\x12\x39\n\rZigbeeInclude\x18\xd1\x0f \x01(\x0b\x32\x1f.vemmiopb.ZigbeeIncludeResponseH\x00\x12\x39\n\rZigbeeExclude\x18\xd2\x0f \x01(\x0b\x32\x1f.vemmiopb.ZigbeeExcludeResponseH\x00\x12\x38\n\x0eZigbeeGetNodes\x18\xd3\x0f \x01(\x0b\x32\x1d.vemmiopb.ZigbeeNodesResponseH\x00\x12\x35\n\x0cZWaveInclude\x18\xb5\x10 \x01(\x0b\x32\x1c.vemmiopb.ZWaveIncludeStatusH\x00\x12\x35\n\x0cZWaveExclude\x18\xb6\x10 \x01(\x0b\x32\x1c.vemmiopb.ZWaveExcludeStatusH\x00\x12\x33\n\nZWaveAbort\x18\xb7\x10 \x01(\x0b\x32\x1c.vemmiopb.ZWaveAbortResponseH\x00\x12\x37\n\x0eZWaveReadNodes\x18\xb8\x10 \x01(\x0b\x32\x1c.vemmiopb.ZWaveNodesResponseH\x00\x12\x33\n\x0bZWaveUpdate\x18\xbb\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveUpdateStatusH\x00\x12=\n\x0fZWaveUpdateNode\x18\xbc\x10 \x01(\x0b\x32!.vemmiopb.ZWaveUpdateNodeResponseH\x00\x12\x33\n\nZWaveReset\x18\xbd\x10 \x01(\x0b\x32\x1c.vemmiopb.ZWaveResetResponseH\x00\x12?\n\x10ZWaveListEntries\x18\xbe\x10 \x01(\x0b\x32\".vemmiopb.ZWaveListEntriesResponseH\x00\x12\x39\n\rZWaveAddEntry\x18\xbf\x10 \x01(\x0b\x32\x1f.vemmiopb.ZWaveAddEntryResponseH\x00\x12?\n\x10ZWaveRemoveEntry\x18\xc0\x10 \x01(\x0b\x32\".vemmiopb.ZWaveRemoveEntryResponseH\x00\x12K\n\x16ZWaveNotificationItems\x18\xc1\x10 \x01(\x0b\x32(.vemmiopb.ZWaveNotificationItemsResponseH\x00\x12\x31\n\tZWaveTest\x18\xc2\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveTestResponseH\x00\x12\x31\n\tZWaveHeal\x18\xc3\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveHealResponseH\x00\x12\x43\n\x12ZWaveReplaceFailed\x18\xc4\x10 \x01(\x0b\x32$.vemmiopb.ZWaveReplaceFailedResponseH\x00\x12\x41\n\x11ZWaveRemoveFailed\x18\xc5\x10 \x01(\x0b\x32#.vemmiopb.ZWaveRemoveFailedResponseH\x00\x12=\n\x10ZWaveHealthCheck\x18\xc6\x10 \x01(\x0b\x32 .vemmiopb.ZWaveHealthCheckStatusH\x00\x12\x35\n\rZWaveReadNode\x18\xc7\x10 \x01(\x0b\x32\x1b.vemmiopb.ZWaveNodeResponseH\x00\x12\x41\n\x11\x43\x61rbonMonoxideGet\x18\x99\x11 \x01(\x0b\x32#.vemmiopb.CarbonMonoxideGetResponseH\x00\x12;\n\x11\x45nableAdvertising\x18\xfd\x11 \x01(\x0b\x32\x1d.vemmiopb.AdvertisingResponseH\x00\x12<\n\x12\x44isableAdvertising\x18\xfe\x11 \x01(\x0b\x32\x1d.vemmiopb.AdvertisingResponseH\x00\x12;\n\x0eUltravioletGet\x18\xe1\x12 \x01(\x0b\x32 .vemmiopb.UltravioletGetResponseH\x00\x12*\n\x05KeyUp\x18\xc5\x13 \x01(\x0b\x32\x18.vemmiopb.RemoteResponseH\x00\x12,\n\x07KeyDown\x18\xc6\x13 \x01(\x0b\x32\x18.vemmiopb.RemoteResponseH\x00\x12+\n\x08GateOpen\x18\xa9\x14 \x01(\x0b\x32\x16.vemmiopb.GateResponseH\x00\x12,\n\tGateClose\x18\xaa\x14 \x01(\x0b\x32\x16.vemmiopb.GateResponseH\x00\x12,\n\tGateCycle\x18\xab\x14 \x01(\x0b\x32\x16.vemmiopb.GateResponseH\x00\x12\x35\n\x0bStatusCheck\x18\x8d\x15 \x01(\x0b\x32\x1d.vemmiopb.StatusCheckResponseH\x00\x12\x34\n\x0cGetStructure\x18\xf1\x15 \x01(\x0b\x32\x1b.vemmiopb.StructureResponseH\x00\x42\x06\n\x04\x64\x61ta*_\n\x12\x43ommandRequestType\x12\x1c\n\x18REQUEST_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11REQUEST_TYPE_DATA\x10\x01\x12\x14\n\x10REQUEST_TYPE_EOF\x10\x02*o\n\x14\x43ommandRequestOption\x12\x1e\n\x1aREQUEST_OPTION_UNSPECIFIED\x10\x00\x12\x18\n\x14REQUEST_OPTION_NOACK\x10\x01\x12\x1d\n\x19REQUEST_OPTION_NORESPONSE\x10\x02*\x81\x01\n\x10\x43ommandReplyType\x12\x1a\n\x16REPLY_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0eREPLY_TYPE_ACK\x10\x01\x12\x14\n\x10REPLY_TYPE_ERROR\x10\x02\x12\x12\n\x0eREPLY_TYPE_EOF\x10\x03\x12\x13\n\x0fREPLY_TYPE_DATA\x10\x04\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.pubsub_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _COMMANDREQUESTTYPE._serialized_start=10546
   _COMMANDREQUESTTYPE._serialized_end=10641
   _COMMANDREQUESTOPTION._serialized_start=10643
   _COMMANDREQUESTOPTION._serialized_end=10754
```

### Comparing `aiomagra-0.1.1/src/aiomagra/remote.proto` & `aiomagra-0.1.2/src/aiomagra/remote.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/remote_pb2.py` & `aiomagra-0.1.2/src/aiomagra/remote_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/remote.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/remote.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"H\n\rRemoteRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\x0b\n\x03key\x18\x02 \x01(\x05\"\x10\n\x0eRemoteResponse\"\x97\x01\n\x0cRemoteReport\x12+\n\x05\x65vent\x18\x01 \x01(\x0e\x32\x1c.vemmiopb.RemoteReport.Event\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\x12\x0b\n\x03key\x18\x03 \x01(\x05\">\n\x05\x45vent\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PRESSED\x10\x01\x12\x0c\n\x08RELEASED\x10\x02\x12\r\n\tHELD_DOWN\x10\x03\x32\x89\x01\n\rRemoteService\x12:\n\x05KeyUp\x12\x17.vemmiopb.RemoteRequest\x1a\x18.vemmiopb.RemoteResponse\x12<\n\x07KeyDown\x12\x17.vemmiopb.RemoteRequest\x1a\x18.vemmiopb.RemoteResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.remote_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _REMOTEREQUEST._serialized_start=60
   _REMOTEREQUEST._serialized_end=132
   _REMOTERESPONSE._serialized_start=134
   _REMOTERESPONSE._serialized_end=150
```

### Comparing `aiomagra-0.1.1/src/aiomagra/reports.proto` & `aiomagra-0.1.2/src/aiomagra/reports.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/roller_shutter.proto` & `aiomagra-0.1.2/src/aiomagra/roller_shutter.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/roller_shutter_pb2.py` & `aiomagra-0.1.2/src/aiomagra/roller_shutter_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/roller_shutter.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x61iomagra/roller_shutter.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"B\n\x14RollerShutterRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"T\n\x17RollerShutterSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\r\n\x05level\x18\x02 \x01(\x05\"\x17\n\x15RollerShutterResponse\")\n\x18RollerShutterLevelReport\x12\r\n\x05value\x18\x01 \x01(\x05\x32\x94\x02\n\rRollerShutter\x12T\n\x11RollerShutterOpen\x12\x1e.vemmiopb.RollerShutterRequest\x1a\x1f.vemmiopb.RollerShutterResponse\x12U\n\x12RollerShutterClose\x12\x1e.vemmiopb.RollerShutterRequest\x1a\x1f.vemmiopb.RollerShutterResponse\x12V\n\x10RollerShutterSet\x12!.vemmiopb.RollerShutterSetRequest\x1a\x1f.vemmiopb.RollerShutterResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.roller_shutter_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ROLLERSHUTTERREQUEST._serialized_start=68
   _ROLLERSHUTTERREQUEST._serialized_end=134
   _ROLLERSHUTTERSETREQUEST._serialized_start=136
   _ROLLERSHUTTERSETREQUEST._serialized_end=220
```

### Comparing `aiomagra-0.1.1/src/aiomagra/seismic_pb2.py` & `aiomagra-0.1.2/src/aiomagra/seismic_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/seismic.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61iomagra/seismic.proto\x12\x08vemmiopb\x1a\x14\x61iomagra/units.proto\"E\n\x16SeismicIntensityReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"E\n\x16SeismicMagnitudeReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.seismic_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _SEISMICINTENSITYREPORT._serialized_start=58
   _SEISMICINTENSITYREPORT._serialized_end=127
   _SEISMICMAGNITUDEREPORT._serialized_start=129
   _SEISMICMAGNITUDEREPORT._serialized_end=198
```

### Comparing `aiomagra-0.1.1/src/aiomagra/sensor_pb2.py` & `aiomagra-0.1.2/src/aiomagra/messaging_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aiomagra/sensor.proto
+# source: aiomagra/messaging.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/sensor.proto\x12\x08vemmiopb\x1a\x14\x61iomagra/units.proto\"=\n\x0eHumidityReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"A\n\x12IlluminationReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\">\n\x0f\x44irectionReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x05\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61iomagra/messaging.proto\x12\x08vemmiopb\"C\n\x0c\x45mailMessage\x12\x11\n\trecipient\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"`\n\x0bPushMessage\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x62\x61\x64ge\x18\x03 \x01(\x05\x12\x0f\n\x07site_id\x18\x04 \x01(\t\x12\x11\n\tsite_name\x18\x05 \x01(\tB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.sensor_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.messaging_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
-  _HUMIDITYREPORT._serialized_start=57
-  _HUMIDITYREPORT._serialized_end=118
-  _ILLUMINATIONREPORT._serialized_start=120
-  _ILLUMINATIONREPORT._serialized_end=185
-  _DIRECTIONREPORT._serialized_start=187
-  _DIRECTIONREPORT._serialized_end=249
+  _EMAILMESSAGE._serialized_start=38
+  _EMAILMESSAGE._serialized_end=105
+  _PUSHMESSAGE._serialized_start=107
+  _PUSHMESSAGE._serialized_end=203
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aiomagra-0.1.1/src/aiomagra/siren.proto` & `aiomagra-0.1.2/src/aiomagra/siren.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/siren_pb2.py` & `aiomagra-0.1.2/src/aiomagra/siren_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/siren.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/siren.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\"B\n\x14SirenGetTonesRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\";\n\x15SirenGetTonesResponse\x12\"\n\x05tones\x18\x01 \x03(\x0b\x32\x13.vemmiopb.SirenTone\"V\n\x14SirenPlayToneRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\x12\n\ntone_index\x18\x02 \x01(\x05\"\x17\n\x15SirenPlayToneResponse\"I\n\x1bSirenPlayDefaultToneRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"\x1e\n\x1cSirenPlayDefaultToneResponse\"H\n\x1aSirenGetDefaultToneRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"@\n\x1bSirenGetDefaultToneResponse\x12!\n\x04tone\x18\x01 \x01(\x0b\x32\x13.vemmiopb.SirenTone\"\\\n\x1aSirenSetDefaultToneRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\x12\n\ntone_index\x18\x02 \x01(\x05\"\x1d\n\x1bSirenSetDefaultToneResponse\"C\n\x15SirenGetVolumeRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"(\n\x16SirenGetVolumeResponse\x12\x0e\n\x06volume\x18\x01 \x01(\x05\"S\n\x15SirenSetVolumeRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\x0e\n\x06volume\x18\x02 \x01(\x05\"\x18\n\x16SirenSetVolumeResponse\")\n\tSirenTone\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05label\x18\x02 \x01(\t\"Y\n\x0bSirenReport\x12*\n\x05state\x18\x01 \x01(\x0e\x32\x1b.vemmiopb.SirenReport.State\"\x1e\n\x05State\x12\t\n\x05\x43LEAR\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\"{\n\nToneReport\x12)\n\x05state\x18\x01 \x01(\x0e\x32\x1a.vemmiopb.ToneReport.State\x12\x12\n\ntone_index\x18\x02 \x01(\x05\".\n\x05State\x12\x0c\n\x08INACTIVE\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x02\"\x1e\n\x0cVolumeReport\x12\x0e\n\x06volume\x18\x01 \x01(\x05\x32\x84\x05\n\x05Siren\x12P\n\rSirenGetTones\x12\x1e.vemmiopb.SirenGetTonesRequest\x1a\x1f.vemmiopb.SirenGetTonesResponse\x12P\n\rSirenPlayTone\x12\x1e.vemmiopb.SirenPlayToneRequest\x1a\x1f.vemmiopb.SirenPlayToneResponse\x12\x65\n\x14SirenPlayDefaultTone\x12%.vemmiopb.SirenPlayDefaultToneRequest\x1a&.vemmiopb.SirenPlayDefaultToneResponse\x12\x62\n\x13SirenGetDefaultTone\x12$.vemmiopb.SirenGetDefaultToneRequest\x1a%.vemmiopb.SirenGetDefaultToneResponse\x12\x62\n\x13SirenSetDefaultTone\x12$.vemmiopb.SirenSetDefaultToneRequest\x1a%.vemmiopb.SirenSetDefaultToneResponse\x12S\n\x0eSirenGetVolume\x12\x1f.vemmiopb.SirenGetVolumeRequest\x1a .vemmiopb.SirenGetVolumeResponse\x12S\n\x0eSirenSetVolume\x12\x1f.vemmiopb.SirenSetVolumeRequest\x1a .vemmiopb.SirenSetVolumeResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.siren_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _SIRENGETTONESREQUEST._serialized_start=59
   _SIRENGETTONESREQUEST._serialized_end=125
   _SIRENGETTONESRESPONSE._serialized_start=127
   _SIRENGETTONESRESPONSE._serialized_end=186
```

### Comparing `aiomagra-0.1.1/src/aiomagra/smoke.proto` & `aiomagra-0.1.2/src/aiomagra/smoke.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/smoke_pb2.py` & `aiomagra-0.1.2/src/aiomagra/smoke_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/smoke.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/smoke.proto\x12\x08vemmiopb\"\xac\x01\n\x0bSmokeReport\x12+\n\x05state\x18\x01 \x01(\x0e\x32\x1c.vemmiopb.SmokeDetectorState\x12\x37\n\x0breplacement\x18\x02 \x01(\x0e\x32\".vemmiopb.SmokeDetectorReplacement\x12\x37\n\x0bmaintenance\x18\x03 \x01(\x0e\x32\".vemmiopb.SmokeDetectorMaintenance*\xde\x01\n\x12SmokeDetectorState\x12\x1b\n\x17SMOKE_STATE_UNSPECIFIED\x10\x00\x12\x15\n\x11SMOKE_STATE_CLEAR\x10\x01\x12\x18\n\x14SMOKE_STATE_DETECTED\x10\x02\x12\x14\n\x10SMOKE_STATE_TEST\x10\x03\x12\x18\n\x14SMOKE_STATE_SILENCED\x10\x04\x12$\n SMOKE_STATE_REPLACEMENT_REQUIRED\x10\x05\x12$\n SMOKE_STATE_MAINTENANCE_REQUIRED\x10\x06*X\n\x18SmokeDetectorReplacement\x12!\n\x1dSMOKE_REPLACEMENT_UNSPECIFIED\x10\x00\x12\x19\n\x15SMOKE_REPLACEMENT_EOL\x10\x01*\x8e\x01\n\x18SmokeDetectorMaintenance\x12!\n\x1dSMOKE_MAINTENANCE_UNSPECIFIED\x10\x00\x12)\n%SMOKE_MAINTENANCE_PERIODIC_INSPECTION\x10\x01\x12$\n SMOKE_MAINTENANCE_DUST_IN_DEVICE\x10\x02\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.smoke_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _SMOKEDETECTORSTATE._serialized_start=210
   _SMOKEDETECTORSTATE._serialized_end=432
   _SMOKEDETECTORREPLACEMENT._serialized_start=434
   _SMOKEDETECTORREPLACEMENT._serialized_end=522
```

### Comparing `aiomagra-0.1.1/src/aiomagra/status_pb2.py` & `aiomagra-0.1.2/src/aiomagra/status_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/status.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/status.proto\x12\x08vemmiopb\"\x14\n\x12StatusCheckRequest\"\x15\n\x13StatusCheckResponse\"5\n\x11StatusCheckReport\x12 \n\x06status\x18\x01 \x01(\x0b\x32\x10.vemmiopb.Status\"[\n\x06Status\x12\x0b\n\x03mac\x18\x01 \x01(\t\x12\x18\n\x10\x66irmware_version\x18\x02 \x01(\t\x12\x17\n\x0f\x66irmware_update\x18\x03 \x01(\x08\x12\x11\n\twifi_rssi\x18\x04 \x01(\x05\x32[\n\rStatusService\x12J\n\x0bStatusCheck\x12\x1c.vemmiopb.StatusCheckRequest\x1a\x1d.vemmiopb.StatusCheckResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.status_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _STATUSCHECKREQUEST._serialized_start=35
   _STATUSCHECKREQUEST._serialized_end=55
   _STATUSCHECKRESPONSE._serialized_start=57
   _STATUSCHECKRESPONSE._serialized_end=78
```

### Comparing `aiomagra-0.1.1/src/aiomagra/structure.proto` & `aiomagra-0.1.2/src/aiomagra/structure.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/structure_pb2.py` & `aiomagra-0.1.2/src/aiomagra/structure_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/structure.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61iomagra/structure.proto\x12\x08vemmiopb\"\x12\n\x10StructureRequest\"A\n\x11StructureResponse\x12,\n\tstructure\x18\x01 \x01(\x0b\x32\x19.vemmiopb.StructureReport\"f\n\x0fStructureReport\x12\x0b\n\x03mac\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x10\n\x08revision\x18\x03 \x01(\t\x12&\n\x05nodes\x18\x04 \x03(\x0b\x32\x17.vemmiopb.StructureNode\"3\n\rStructureNode\x12\x0c\n\x04uuid\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63\x61pabilities\x18\x02 \x03(\t2[\n\x10StructureService\x12G\n\x0cGetStructure\x12\x1a.vemmiopb.StructureRequest\x1a\x1b.vemmiopb.StructureResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.structure_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _STRUCTUREREQUEST._serialized_start=38
   _STRUCTUREREQUEST._serialized_end=56
   _STRUCTURERESPONSE._serialized_start=58
   _STRUCTURERESPONSE._serialized_end=123
```

### Comparing `aiomagra-0.1.1/src/aiomagra/switch.proto` & `aiomagra-0.1.2/src/aiomagra/switch.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/switch_pb2.py` & `aiomagra-0.1.2/src/aiomagra/switch_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/switch.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/switch.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\";\n\rSwitchRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"\x10\n\x0eSwitchResponse\"4\n\x0cSwitchReport\x12$\n\x05value\x18\x01 \x01(\x0e\x32\x15.vemmiopb.SwitchValue*@\n\x0bSwitchValue\x12\x12\n\x0eSWITCH_UNKNOWN\x10\x00\x12\r\n\tSWITCH_ON\x10\x01\x12\x0e\n\nSWITCH_OFF\x10\x02\x32\x87\x01\n\x06Switch\x12=\n\x08SwitchOn\x12\x17.vemmiopb.SwitchRequest\x1a\x18.vemmiopb.SwitchResponse\x12>\n\tSwitchOff\x12\x17.vemmiopb.SwitchRequest\x1a\x18.vemmiopb.SwitchResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.switch_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _SWITCHVALUE._serialized_start=193
   _SWITCHVALUE._serialized_end=257
   _SWITCHREQUEST._serialized_start=60
   _SWITCHREQUEST._serialized_end=119
```

### Comparing `aiomagra-0.1.1/src/aiomagra/tamper_pb2.py` & `aiomagra-0.1.2/src/aiomagra/taptap_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aiomagra/tamper.proto
+# source: aiomagra/taptap.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/tamper.proto\x12\x08vemmiopb\"4\n\x0cTamperReport\x12$\n\x05state\x18\x01 \x01(\x0e\x32\x15.vemmiopb.TamperState*R\n\x0bTamperState\x12\x18\n\x14TAMPER_COVER_REMOVED\x10\x00\x12\x17\n\x13TAMPER_INVALID_CODE\x10\x01\x12\x10\n\x0cTAMPER_MOVED\x10\x02\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/taptap.proto\x12\x08vemmiopb\"\x1b\n\x0cTapTapReport\x12\x0b\n\x03num\x18\x01 \x01(\x05\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.tamper_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.taptap_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
-  _TAMPERSTATE._serialized_start=89
-  _TAMPERSTATE._serialized_end=171
-  _TAMPERREPORT._serialized_start=35
-  _TAMPERREPORT._serialized_end=87
+  _TAPTAPREPORT._serialized_start=35
+  _TAPTAPREPORT._serialized_end=62
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aiomagra-0.1.1/src/aiomagra/taptap_pb2.py` & `aiomagra-0.1.2/src/aiomagra/mqtt_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aiomagra/taptap.proto
+# source: aiomagra/mqtt.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import pubsub_pb2 as aiomagra_dot_pubsub__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/taptap.proto\x12\x08vemmiopb\"\x1b\n\x0cTapTapReport\x12\x0b\n\x03num\x18\x01 \x01(\x05\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61iomagra/mqtt.proto\x12\x08vemmiopb\x1a\x15\x61iomagra/pubsub.proto\"W\n\x12MQTTCommandRequest\x12)\n\x07request\x18\x01 \x01(\x0b\x32\x18.vemmiopb.CommandRequest\x12\x16\n\x0eresponse_topic\x18\x02 \x01(\tB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.taptap_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.mqtt_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
-  _TAPTAPREPORT._serialized_start=35
-  _TAPTAPREPORT._serialized_end=62
+  _MQTTCOMMANDREQUEST._serialized_start=56
+  _MQTTCOMMANDREQUEST._serialized_end=143
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aiomagra-0.1.1/src/aiomagra/temperature.proto` & `aiomagra-0.1.2/src/aiomagra/temperature.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/temperature_pb2.py` & `aiomagra-0.1.2/src/aiomagra/temperature_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/temperature.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x61iomagra/temperature.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\x1a\x14\x61iomagra/units.proto\"T\n\x15TemperatureGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12\x0f\n\x07refresh\x18\x02 \x01(\x08\"E\n\x16TemperatureGetResponse\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"@\n\x11TemperatureReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\x32\x62\n\x0bTemperature\x12S\n\x0eTemperatureGet\x12\x1f.vemmiopb.TemperatureGetRequest\x1a .vemmiopb.TemperatureGetResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.temperature_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _TEMPERATUREGETREQUEST._serialized_start=87
   _TEMPERATUREGETREQUEST._serialized_end=171
   _TEMPERATUREGETRESPONSE._serialized_start=173
   _TEMPERATUREGETRESPONSE._serialized_end=242
```

### Comparing `aiomagra-0.1.1/src/aiomagra/thermostat.proto` & `aiomagra-0.1.2/src/aiomagra/thermostat.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/thermostat_pb2.py` & `aiomagra-0.1.2/src/aiomagra/thermostat_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/thermostat.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x61iomagra/thermostat.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\x1a\x14\x61iomagra/units.proto\"n\n\x18ThermostatModeSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12&\n\x04mode\x18\x02 \x01(\x0e\x32\x18.vemmiopb.ThermostatMode\"I\n\x1bThermostatModeSupGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"G\n\x1cThermostatModeSupGetResponse\x12\'\n\x05modes\x18\x01 \x03(\x0e\x32\x18.vemmiopb.ThermostatMode\"\xaa\x01\n\x1cThermostatSetpointSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12.\n\x04type\x18\x02 \x01(\x0e\x32 .vemmiopb.ThermostatSetpointType\x12.\n\x08setpoint\x18\x03 \x01(\x0b\x32\x1c.vemmiopb.ThermostatSetpoint\"x\n\x1bThermostatFanModeSetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\x12-\n\x08\x66\x61n_mode\x18\x02 \x01(\x0e\x32\x1b.vemmiopb.ThermostatFanMode\"\x14\n\x12ThermostatResponse\">\n\x14ThermostatModeReport\x12&\n\x04mode\x18\x01 \x01(\x0e\x32\x18.vemmiopb.ThermostatMode\"J\n\x18ThermostatSetpointReport\x12.\n\x08setpoint\x18\x01 \x01(\x0b\x32\x1c.vemmiopb.ThermostatSetpoint\"H\n\x17ThermostatFanModeReport\x12-\n\x08\x66\x61n_mode\x18\x01 \x01(\x0e\x32\x1b.vemmiopb.ThermostatFanMode\"\x9f\x01\n\x17ThermostatSetpointRange\x12.\n\x04type\x18\x01 \x01(\x0e\x32 .vemmiopb.ThermostatSetpointType\x12)\n\x03min\x18\x02 \x01(\x0b\x32\x1c.vemmiopb.ThermostatSetpoint\x12)\n\x03max\x18\x03 \x01(\x0b\x32\x1c.vemmiopb.ThermostatSetpoint\"T\n\x12ThermostatSetpoint\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x1c\n\x04unit\x18\x02 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\x11\n\tprecision\x18\x03 \x01(\r*w\n\x0eThermostatMode\x12\x17\n\x13THERMOSTAT_MODE_OFF\x10\x00\x12\x18\n\x14THERMOSTAT_MODE_HEAT\x10\x01\x12\x18\n\x14THERMOSTAT_MODE_COOL\x10\x02\x12\x18\n\x14THERMOSTAT_MODE_AUTO\x10\x03*\x81\x01\n\x16ThermostatSetpointType\x12!\n\x1dTHERMOSTAT_SETPOINT_TYPE_HEAT\x10\x00\x12!\n\x1dTHERMOSTAT_SETPOINT_TYPE_COOL\x10\x01\x12!\n\x1dTHERMOSTAT_SETPOINT_TYPE_AUTO\x10\x02*\xb0\x01\n\x11ThermostatFanMode\x12\x1b\n\x17THERMOSTAT_FAN_MODE_OFF\x10\x00\x12 \n\x1cTHERMOSTAT_FAN_MODE_AUTO_LOW\x10\x01\x12\x1b\n\x17THERMOSTAT_FAN_MODE_LOW\x10\x02\x12!\n\x1dTHERMOSTAT_FAN_MODE_AUTO_HIGH\x10\x03\x12\x1c\n\x18THERMOSTAT_FAN_MODE_HIGH\x10\x04\x32\x86\x03\n\nThermostat\x12U\n\x11ThermostatModeSet\x12\".vemmiopb.ThermostatModeSetRequest\x1a\x1c.vemmiopb.ThermostatResponse\x12\x65\n\x14ThermostatModeSupGet\x12%.vemmiopb.ThermostatModeSupGetRequest\x1a&.vemmiopb.ThermostatModeSupGetResponse\x12]\n\x15ThermostatSetpointSet\x12&.vemmiopb.ThermostatSetpointSetRequest\x1a\x1c.vemmiopb.ThermostatResponse\x12[\n\x14ThermostatFanModeSet\x12%.vemmiopb.ThermostatFanModeSetRequest\x1a\x1c.vemmiopb.ThermostatResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.thermostat_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _THERMOSTATMODE._serialized_start=1125
   _THERMOSTATMODE._serialized_end=1244
   _THERMOSTATSETPOINTTYPE._serialized_start=1247
   _THERMOSTATSETPOINTTYPE._serialized_end=1376
```

### Comparing `aiomagra-0.1.1/src/aiomagra/ultraviolet.proto` & `aiomagra-0.1.2/src/aiomagra/ultraviolet.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/ultraviolet_pb2.py` & `aiomagra-0.1.2/src/aiomagra/ultraviolet_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/ultraviolet.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
+from aiomagra import units_pb2 as aiomagra_dot_units__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x61iomagra/ultraviolet.proto\x12\x08vemmiopb\x1a\x17\x61iomagra/metadata.proto\x1a\x14\x61iomagra/units.proto\"C\n\x15UltravioletGetRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.DeviceMetadata\"E\n\x16UltravioletGetResponse\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\"@\n\x11UltravioletReport\x12\x1c\n\x04unit\x18\x01 \x01(\x0e\x32\x0e.vemmiopb.Unit\x12\r\n\x05value\x18\x02 \x01(\x01\x32i\n\x12UltravioletService\x12S\n\x0eUltravioletGet\x12\x1f.vemmiopb.UltravioletGetRequest\x1a .vemmiopb.UltravioletGetResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.ultraviolet_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ULTRAVIOLETGETREQUEST._serialized_start=87
   _ULTRAVIOLETGETREQUEST._serialized_end=154
   _ULTRAVIOLETGETRESPONSE._serialized_start=156
   _ULTRAVIOLETGETRESPONSE._serialized_end=225
```

### Comparing `aiomagra-0.1.1/src/aiomagra/units.proto` & `aiomagra-0.1.2/src/aiomagra/units.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/units_pb2.py` & `aiomagra-0.1.2/src/aiomagra/units_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/units.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/units.proto\x12\x08vemmiopb*\xa1\x02\n\x04Unit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07\x43\x45LSIUS\x10\x01\x12\x0e\n\nFAHRENHEIT\x10\x02\x12\x07\n\x03LUX\x10\x03\x12\x0e\n\nPERCENTAGE\x10\x04\x12\x08\n\x04WATT\x10\x05\x12\x0f\n\x0bPULSE_COUNT\x10\x06\x12\x07\n\x03KWH\x10\x07\x12\x08\n\x04KVAH\x10\x08\x12\x08\n\x04VOLT\x10\t\x12\n\n\x06\x41MPERE\x10\n\x12\x10\n\x0cPOWER_FACTOR\x10\x0b\x12\x10\n\x0c\x43UBIC_METERS\x10\x0c\x12\x0e\n\nCUBIC_FEET\x10\r\x12\x0e\n\nUS_GALLONS\x10\x0e\x12\x0b\n\x07\x44\x45GREES\x10\x0f\x12\x1c\n\x18METER_PER_SECOND_SQUARED\x10\x10\x12\x0c\n\x08MERCALLI\x10\x11\x12\x15\n\x11PARTS_PER_MILLION\x10\x12\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.units_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _UNIT._serialized_start=35
   _UNIT._serialized_end=324
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aiomagra-0.1.1/src/aiomagra/websocket_pb2.py` & `aiomagra-0.1.2/src/aiomagra/websocket_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/websocket.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import pubsub_pb2 as aiomagra_dot_pubsub__pb2
+from aiomagra import reports_pb2 as aiomagra_dot_reports__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61iomagra/websocket.proto\x12\x08vemmiopb\x1a\x15\x61iomagra/pubsub.proto\x1a\x16\x61iomagra/reports.proto\"\xa7\x01\n\x10WebsocketMessage\x12\x10\n\x08\x66rame_id\x18\x01 \x01(\x04\x12)\n\x07request\x18\x02 \x01(\x0b\x32\x18.vemmiopb.CommandRequest\x12%\n\x05reply\x18\x03 \x01(\x0b\x32\x16.vemmiopb.CommandReply\x12/\n\x0egateway_report\x18\x04 \x01(\x0b\x32\x17.vemmiopb.GatewayReportB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.websocket_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _WEBSOCKETMESSAGE._serialized_start=86
   _WEBSOCKETMESSAGE._serialized_end=253
 # @@protoc_insertion_point(module_scope)
```

### Comparing `aiomagra-0.1.1/src/aiomagra/wifi.proto` & `aiomagra-0.1.2/src/aiomagra/wifi.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/wifi_pb2.py` & `aiomagra-0.1.2/src/aiomagra/wifi_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/wifi.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61iomagra/wifi.proto\x12\x08vemmiopb\x1a\x1fgoogle/protobuf/timestamp.proto\"\x12\n\x10WiFiQueryRequest\"o\n\x11WiFiQueryResponse\x12+\n\ninterfaces\x18\x01 \x03(\x0b\x32\x17.vemmiopb.WiFiInterface\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x11\n\x0fWiFiScanRequest\"3\n\x10WiFiScanResponse\x12\x1f\n\x04\x62sss\x18\x01 \x03(\x0b\x32\x11.vemmiopb.WiFiBSS\"/\n\x12WiFiConnectRequest\x12\x0c\n\x04ssid\x18\x01 \x01(\t\x12\x0b\n\x03psk\x18\x02 \x01(\t\"\x15\n\x13WiFiConnectResponse\"}\n\rWiFiInterface\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rhardware_addr\x18\x02 \x01(\x0c\x12\x1e\n\x03\x62ss\x18\x03 \x01(\x0b\x32\x11.vemmiopb.WiFiBSS\x12\'\n\x08stations\x18\x04 \x03(\x0b\x32\x15.vemmiopb.WiFiStation\"=\n\x07WiFiBSS\x12\x0c\n\x04ssid\x18\x01 \x01(\t\x12\x11\n\tfrequency\x18\x02 \x01(\x05\x12\x11\n\tlast_seen\x18\x03 \x01(\x03\"Y\n\x0bWiFiStation\x12\x15\n\rhardware_addr\x18\x01 \x01(\x0c\x12\x0e\n\x06signal\x18\x02 \x01(\x05\x12\x11\n\tconnected\x18\x03 \x01(\x03\x12\x10\n\x08inactive\x18\x04 \x01(\x03\x32\xdb\x01\n\x04WiFi\x12\x44\n\tWiFiQuery\x12\x1a.vemmiopb.WiFiQueryRequest\x1a\x1b.vemmiopb.WiFiQueryResponse\x12\x41\n\x08WiFiScan\x12\x19.vemmiopb.WiFiScanRequest\x1a\x1a.vemmiopb.WiFiScanResponse\x12J\n\x0bWiFiConnect\x12\x1c.vemmiopb.WiFiConnectRequest\x1a\x1d.vemmiopb.WiFiConnectResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.wifi_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _WIFIQUERYREQUEST._serialized_start=66
   _WIFIQUERYREQUEST._serialized_end=84
   _WIFIQUERYRESPONSE._serialized_start=86
   _WIFIQUERYRESPONSE._serialized_end=197
```

### Comparing `aiomagra-0.1.1/src/aiomagra/zigbee.proto` & `aiomagra-0.1.2/src/aiomagra/zigbee.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/zigbee_pb2.py` & `aiomagra-0.1.2/src/aiomagra/zigbee_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/zigbee.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from aiomagra import devices_pb2 as aiomagra_dot_devices__pb2
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61iomagra/zigbee.proto\x12\x08vemmiopb\x1a\x16\x61iomagra/devices.proto\x1a\x17\x61iomagra/metadata.proto\"\x16\n\x14ZigbeeIncludeRequest\":\n\x15ZigbeeIncludeResponse\x12!\n\x07\x64\x65vices\x18\x01 \x03(\x0b\x32\x10.vemmiopb.Device\"B\n\x14ZigbeeExcludeRequest\x12*\n\x08metadata\x18\x01 \x01(\x0b\x32\x18.vemmiopb.ZigbeeMetadata\"\x17\n\x15ZigbeeExcludeResponse\"\x14\n\x12ZigbeeNodesRequest\":\n\x13ZigbeeNodesResponse\x12#\n\x05nodes\x18\x01 \x03(\x0b\x32\x14.vemmiopb.ZigbeeNode\"W\n\nZigbeeNode\x12\x11\n\tieee_addr\x18\x01 \x01(\x05\x12\x12\n\neui64_addr\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\x05\x12\x10\n\x08\x63lusters\x18\x04 \x03(\x05\x32\xfb\x01\n\x06Zigbee\x12P\n\rZigbeeInclude\x12\x1e.vemmiopb.ZigbeeIncludeRequest\x1a\x1f.vemmiopb.ZigbeeIncludeResponse\x12P\n\rZigbeeExclude\x12\x1e.vemmiopb.ZigbeeExcludeRequest\x1a\x1f.vemmiopb.ZigbeeExcludeResponse\x12M\n\x0eZigbeeGetNodes\x12\x1c.vemmiopb.ZigbeeNodesRequest\x1a\x1d.vemmiopb.ZigbeeNodesResponseB=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.zigbee_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ZIGBEEINCLUDEREQUEST._serialized_start=84
   _ZIGBEEINCLUDEREQUEST._serialized_end=106
   _ZIGBEEINCLUDERESPONSE._serialized_start=108
   _ZIGBEEINCLUDERESPONSE._serialized_end=166
```

### Comparing `aiomagra-0.1.1/src/aiomagra/zwave.proto` & `aiomagra-0.1.2/src/aiomagra/zwave.proto`

 * *Files identical despite different names*

### Comparing `aiomagra-0.1.1/src/aiomagra/zwave_pb2.py` & `aiomagra-0.1.2/src/aiomagra/zwave_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+# -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: aiomagra/zwave.proto
 """Generated protocol buffer code."""
-from google.protobuf import (
-  descriptor as _descriptor,
-  descriptor_pool as _descriptor_pool,
-  symbol_database as _symbol_database,
-)
 from google.protobuf.internal import builder as _builder
-
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+from aiomagra import devices_pb2 as aiomagra_dot_devices__pb2
+from aiomagra import metadata_pb2 as aiomagra_dot_metadata__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61iomagra/zwave.proto\x12\x08vemmiopb\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x16\x61iomagra/devices.proto\x1a\x17\x61iomagra/metadata.proto\"%\n\x13ZWaveIncludeRequest\x12\x0e\n\x06secure\x18\x01 \x01(\x08\"\xf6\x02\n\x12ZWaveIncludeStatus\x12\x39\n\x05\x66ound\x18\x01 \x01(\x0b\x32(.vemmiopb.ZWaveIncludeStatus.DeviceFoundH\x00\x12\x39\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x0b\x32(.vemmiopb.ZWaveIncludeStatus.DeviceAddedH\x00\x12:\n\x05ready\x18\x03 \x01(\x0b\x32).vemmiopb.ZWaveIncludeStatus.IncludeReadyH\x00\x12@\n\x08progress\x18\x04 \x01(\x0b\x32,.vemmiopb.ZWaveIncludeStatus.IncludeProgressH\x00\x1a\r\n\x0b\x44\x65viceFound\x1a\x30\n\x0b\x44\x65viceAdded\x12!\n\x07\x64\x65vices\x18\x01 \x03(\x0b\x32\x10.vemmiopb.Device\x1a\x0e\n\x0cIncludeReady\x1a\x11\n\x0fIncludeProgressB\x08\n\x06status\"\x15\n\x13ZWaveExcludeRequest\"\x8e\x03\n\x12ZWaveExcludeStatus\x12=\n\x07removed\x18\x01 \x01(\x0b\x32*.vemmiopb.ZWaveExcludeStatus.DeviceRemovedH\x00\x12:\n\x05ready\x18\x02 \x01(\x0b\x32).vemmiopb.ZWaveExcludeStatus.ExcludeReadyH\x00\x12@\n\x08progress\x18\x03 \x01(\x0b\x32,.vemmiopb.ZWaveExcludeStatus.ExcludeProgressH\x00\x12@\n\tnot_found\x18\x04 \x01(\x0b\x32+.vemmiopb.ZWaveExcludeStatus.DeviceNotFoundH\x00\x1a:\n\rDeviceRemoved\x12)\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.vemmiopb.ZWaveMetadata\x1a\x0e\n\x0c\x45xcludeReady\x1a\x11\n\x0f\x45xcludeProgress\x1a\x10\n\x0e\x44\x65viceNotFoundB\x08\n\x06status\"\x13\n\x11ZWaveAbortRequest\"\x14\n\x12ZWaveAbortResponse\"O\n\x10ZWaveTestRequest\x12,\n\x07node_id\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\"\x13\n\x11ZWaveTestResponse\"\\\n\x10ZWaveHealRequest\x12,\n\x07node_id\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x1a\n\x12init_return_routes\x18\x02 \x01(\x08\"\x13\n\x11ZWaveHealResponse\",\n\x19ZWaveReplaceFailedRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\"\x1c\n\x1aZWaveReplaceFailedResponse\"+\n\x18ZWaveRemoveFailedRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\"\x1b\n\x19ZWaveRemoveFailedResponse\"\x19\n\x17ZWaveHealthCheckRequest\"\xca\x01\n\x16ZWaveHealthCheckStatus\x12\x34\n\x07started\x18\x01 \x01(\x0b\x32!.vemmiopb.ZWaveHealthCheckStartedH\x00\x12\x36\n\x08progress\x18\x02 \x01(\x0b\x32\".vemmiopb.ZWaveHealthCheckProgressH\x00\x12\x38\n\tcompleted\x18\x03 \x01(\x0b\x32#.vemmiopb.ZWaveHealthCheckCompletedH\x00\x42\x08\n\x06status\"\x19\n\x17ZWaveHealthCheckStarted\"8\n\x18ZWaveHealthCheckProgress\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\r\n\x05total\x18\x02 \x01(\x05\"K\n\x19ZWaveHealthCheckCompleted\x12.\n\x05nodes\x18\x01 \x03(\x0b\x32\x1f.vemmiopb.ZWaveHealthStatusNode\"h\n\x15ZWaveHealthStatusNode\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12/\n\x08\x63\x61tegory\x18\x02 \x01(\x0e\x32\x1d.vemmiopb.ZWaveHealthCategory\x12\r\n\x05value\x18\x03 \x01(\x05\"\x13\n\x11ZWaveNodesRequest\"8\n\x12ZWaveNodesResponse\x12\"\n\x05nodes\x18\x01 \x03(\x0b\x32\x13.vemmiopb.ZWaveNode\"#\n\x10ZWaveNodeRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\"6\n\x11ZWaveNodeResponse\x12!\n\x04node\x18\x01 \x01(\x0b\x32\x13.vemmiopb.ZWaveNode\"\x14\n\x12ZWaveUpdateRequest\"\xde\x01\n\x11ZWaveUpdateStatus\x12?\n\x08topology\x18\x01 \x01(\x0b\x32+.vemmiopb.ZWaveNetworkTopologyUpdateStartedH\x00\x12<\n\x08neighbor\x18\x02 \x01(\x0b\x32(.vemmiopb.ZWaveNodeNeighborUpdateStartedH\x00\x12@\n\tnode_info\x18\x03 \x01(\x0b\x32+.vemmiopb.ZWaveNodeInformationUpdateStartedH\x00\x42\x08\n\x06status\"#\n!ZWaveNetworkTopologyUpdateStarted\" \n\x1eZWaveNodeNeighborUpdateStarted\"#\n!ZWaveNodeInformationUpdateStarted\")\n\x16ZWaveUpdateNodeRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\"\x19\n\x17ZWaveUpdateNodeResponse\"\x13\n\x11ZWaveResetRequest\"\x14\n\x12ZWaveResetResponse\"\xf4\x01\n\tZWaveNode\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x11\n\tvendor_id\x18\x02 \x01(\x05\x12\x14\n\x0cproduct_type\x18\x03 \x01(\x05\x12\x12\n\nproduct_id\x18\x04 \x01(\x05\x12*\n\tendpoints\x18\x05 \x03(\x0b\x32\x17.vemmiopb.ZWaveEndpoint\x12\x19\n\x11manufacturer_name\x18\x06 \x01(\t\x12\x14\n\x0cproduct_name\x18\x07 \x01(\t\x12\x11\n\tuser_name\x18\x08 \x01(\t\x12)\n\x06status\x18\t \x01(\x0e\x32\x19.vemmiopb.ZWaveNodeStatus\"{\n\rZWaveEndpoint\x12\r\n\x05\x65p_id\x18\x01 \x01(\x05\x12\x15\n\rgeneric_class\x18\x02 \x01(\x05\x12\x16\n\x0especific_class\x18\x03 \x01(\x05\x12,\n\ninterfaces\x18\x04 \x03(\x0b\x32\x18.vemmiopb.ZWaveInterface\"\x94\x01\n\x0eZWaveInterface\x12\x15\n\rcommand_class\x18\x01 \x01(\x05\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x14\n\x0creal_version\x18\x04 \x01(\x05\x12\r\n\x05label\x18\x05 \x01(\t\x12\x0c\n\x04help\x18\x06 \x01(\t\x12\'\n\x05items\x18\x07 \x03(\x0b\x32\x18.vemmiopb.ZWaveValueItem\".\n\x0eZWaveValueItem\x12\r\n\x05value\x18\x01 \x01(\x05\x12\r\n\x05label\x18\x02 \x01(\t\"\x19\n\x17ZWaveListEntriesRequest\"M\n\x18ZWaveListEntriesResponse\x12\x31\n\x07\x65ntries\x18\x01 \x03(\x0b\x32 .vemmiopb.ZWaveProvisioningEntry\"R\n\x14ZWaveAddEntryRequest\x12\x0b\n\x03\x64sk\x18\x01 \x01(\t\x12-\n\x04info\x18\x02 \x03(\x0b\x32\x1f.vemmiopb.ZWaveProvisioningInfo\"\x17\n\x15ZWaveAddEntryResponse\"&\n\x17ZWaveRemoveEntryRequest\x12\x0b\n\x03\x64sk\x18\x01 \x01(\t\"\x1a\n\x18ZWaveRemoveEntryResponse\"T\n\x16ZWaveProvisioningEntry\x12\x0b\n\x03\x64sk\x18\x01 \x01(\t\x12-\n\x04info\x18\x02 \x03(\x0b\x32\x1f.vemmiopb.ZWaveProvisioningInfo\"\x8f\x03\n\x15ZWaveProvisioningInfo\x12\x42\n\x0cproduct_type\x18\x01 \x01(\x0b\x32*.vemmiopb.ZWaveProvisioningInfoProductTypeH\x00\x12>\n\nproduct_id\x18\x02 \x01(\x0b\x32(.vemmiopb.ZWaveProvisioningInfoProductIDH\x00\x12\x1c\n\x12inclusion_interval\x18\x03 \x01(\x05H\x00\x12\x0e\n\x04uuid\x18\x04 \x01(\tH\x00\x12\x0e\n\x04name\x18\x05 \x01(\tH\x00\x12\x12\n\x08location\x18\x06 \x01(\tH\x00\x12\x1a\n\x10inclusion_status\x18\x07 \x01(\x05H\x00\x12\x16\n\x0cgranted_keys\x18\x08 \x01(\x05H\x00\x12\x1c\n\x12\x62ootstrapping_mode\x18\t \x01(\x05H\x00\x12\x46\n\x0enetwork_status\x18\n \x01(\x0b\x32,.vemmiopb.ZWaveProvisioningInfoNetworkStatusH\x00\x42\x06\n\x04info\"d\n ZWaveProvisioningInfoProductType\x12\x15\n\rgeneric_class\x18\x01 \x01(\x05\x12\x16\n\x0especific_class\x18\x02 \x01(\x05\x12\x11\n\ticon_type\x18\x03 \x01(\x05\"\xa1\x01\n\x1eZWaveProvisioningInfoProductID\x12\x17\n\x0fmanufacturer_id\x18\x01 \x01(\x05\x12\x14\n\x0cproduct_type\x18\x02 \x01(\x05\x12\x12\n\nproduct_id\x18\x03 \x01(\x05\x12\x1b\n\x13\x61pplication_version\x18\x04 \x01(\x05\x12\x1f\n\x17\x61pplication_sub_version\x18\x05 \x01(\x05\"E\n\"ZWaveProvisioningInfoNetworkStatus\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\x0e\n\x06status\x18\x02 \x01(\x05\"N\n\x1dZWaveNotificationItemsRequest\x12\x0f\n\x07node_id\x18\x01 \x01(\x05\x12\r\n\x05\x65p_id\x18\x02 \x01(\x05\x12\r\n\x05index\x18\x03 \x01(\x05\"/\n\x1eZWaveNotificationItemsResponse\x12\r\n\x05items\x18\x01 \x03(\x05*\x95\x01\n\x13ZWaveHealthCategory\x12\x1c\n\x18ZWAVE_HEALTH_UNSPECIFIED\x10\x00\x12\x16\n\x12ZWAVE_HEALTH_GREEN\x10\x01\x12\x17\n\x13ZWAVE_HEALTH_YELLOW\x10\x02\x12\x14\n\x10ZWAVE_HEALTH_RED\x10\x03\x12\x19\n\x15ZWAVE_HEALTH_CRITICAL\x10\x04*r\n\x0fZWaveNodeStatus\x12\x1b\n\x17NODE_STATUS_UNSPECIFIED\x10\x00\x12\x15\n\x11NODE_STATUS_ALIVE\x10\x01\x12\x14\n\x10NODE_STATUS_DOWN\x10\x02\x12\x15\n\x11NODE_STATUS_SLEEP\x10\x03\x32\x8d\x0b\n\x05ZWave\x12M\n\x0cZWaveInclude\x12\x1d.vemmiopb.ZWaveIncludeRequest\x1a\x1c.vemmiopb.ZWaveIncludeStatus0\x01\x12M\n\x0cZWaveExclude\x12\x1d.vemmiopb.ZWaveExcludeRequest\x1a\x1c.vemmiopb.ZWaveExcludeStatus0\x01\x12G\n\nZWaveAbort\x12\x1b.vemmiopb.ZWaveAbortRequest\x1a\x1c.vemmiopb.ZWaveAbortResponse\x12K\n\x0eZWaveReadNodes\x12\x1b.vemmiopb.ZWaveNodesRequest\x1a\x1c.vemmiopb.ZWaveNodesResponse\x12H\n\rZWaveReadNode\x12\x1a.vemmiopb.ZWaveNodeRequest\x1a\x1b.vemmiopb.ZWaveNodeResponse\x12J\n\x0bZWaveUpdate\x12\x1c.vemmiopb.ZWaveUpdateRequest\x1a\x1b.vemmiopb.ZWaveUpdateStatus0\x01\x12V\n\x0fZWaveUpdateNode\x12 .vemmiopb.ZWaveUpdateNodeRequest\x1a!.vemmiopb.ZWaveUpdateNodeResponse\x12G\n\nZWaveReset\x12\x1b.vemmiopb.ZWaveResetRequest\x1a\x1c.vemmiopb.ZWaveResetResponse\x12Y\n\x10ZWaveListEntries\x12!.vemmiopb.ZWaveListEntriesRequest\x1a\".vemmiopb.ZWaveListEntriesResponse\x12P\n\rZWaveAddEntry\x12\x1e.vemmiopb.ZWaveAddEntryRequest\x1a\x1f.vemmiopb.ZWaveAddEntryResponse\x12Y\n\x10ZWaveRemoveEntry\x12!.vemmiopb.ZWaveRemoveEntryRequest\x1a\".vemmiopb.ZWaveRemoveEntryResponse\x12k\n\x16ZWaveNotificationItems\x12\'.vemmiopb.ZWaveNotificationItemsRequest\x1a(.vemmiopb.ZWaveNotificationItemsResponse\x12\x44\n\tZWaveTest\x12\x1a.vemmiopb.ZWaveTestRequest\x1a\x1b.vemmiopb.ZWaveTestResponse\x12\x44\n\tZWaveHeal\x12\x1a.vemmiopb.ZWaveHealRequest\x1a\x1b.vemmiopb.ZWaveHealResponse\x12_\n\x12ZWaveReplaceFailed\x12#.vemmiopb.ZWaveReplaceFailedRequest\x1a$.vemmiopb.ZWaveReplaceFailedResponse\x12\\\n\x11ZWaveRemoveFailed\x12\".vemmiopb.ZWaveRemoveFailedRequest\x1a#.vemmiopb.ZWaveRemoveFailedResponse\x12Y\n\x10ZWaveHealthCheck\x12!.vemmiopb.ZWaveHealthCheckRequest\x1a .vemmiopb.ZWaveHealthCheckStatus0\x01\x42=\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\x01Z\n./vemmiopbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aiomagra.zwave_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS is False:
+if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n-com.vemmio.ha.integration.vemmio.rpc.vemmiopbP\001Z\n./vemmiopb'
   _ZWAVEHEALTHCATEGORY._serialized_start=4314
   _ZWAVEHEALTHCATEGORY._serialized_end=4463
   _ZWAVENODESTATUS._serialized_start=4465
   _ZWAVENODESTATUS._serialized_end=4579
```

