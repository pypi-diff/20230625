# Comparing `tmp/gridworks_protocol-0.5.4.tar.gz` & `tmp/gridworks_protocol-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.5.4.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.5.5.tar", max compression
```

## Comparing `gridworks_protocol-0.5.4.tar` & `gridworks_protocol-0.5.5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     1070 2023-06-07 18:24:01.001160 gridworks_protocol-0.5.4/LICENSE
--rw-r--r--   0        0        0     2552 2023-06-07 18:24:01.001160 gridworks_protocol-0.5.4/README.md
--rw-r--r--   0        0        0     2308 2023-06-07 18:24:22.457406 gridworks_protocol-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1439 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/__init__.py
--rw-r--r--   0        0        0     1339 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0     1488 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      995 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1112 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/relay_cac.py
--rw-r--r--   0        0        0     1118 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0     1580 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1094 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1659 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0     1479 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1357 2023-06-07 18:24:01.005159 gridworks_protocol-0.5.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1267 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/components/relay_component.py
--rw-r--r--   0        0        0     1465 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0     1308 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    14718 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0     1957 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    12051 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/decoders.py
--rw-r--r--   0        0        0      451 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     3486 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     1119 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0     2657 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     3480 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     1823 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     1148 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0      160 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      460 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      442 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3058 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0       40 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/topic.py
--rw-r--r--   0        0        0     6632 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     5464 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0     6107 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0    10172 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     3876 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     3583 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    21173 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    13387 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     7175 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_boolean_actuator_component.py
--rw-r--r--   0        0        0     8431 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     5782 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     4959 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     5570 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     5313 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    12770 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11864 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    13625 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    12328 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8369 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0     9449 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0    21533 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0     9915 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    11254 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0     7606 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     2751 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0    11076 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/relay_cac_gt.py
--rw-r--r--   0        0        0     7602 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/relay_component_gt.py
--rw-r--r--   0        0        0    11686 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0     8084 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0    20734 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0     7268 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     5991 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    18195 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    14031 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    12205 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2556 2023-06-07 18:24:01.009159 gridworks_protocol-0.5.4/src/gwproto/utils.py
--rw-r--r--   0        0        0     3619 1970-01-01 00:00:00.000000 gridworks_protocol-0.5.4/setup.py
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 gridworks_protocol-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-25 19:45:07.053018 gridworks_protocol-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2552 2023-06-25 19:45:07.053018 gridworks_protocol-0.5.5/README.md
+-rw-r--r--   0        0        0     2308 2023-06-25 19:45:19.753082 gridworks_protocol-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1439 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     1339 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0     1488 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      995 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1112 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1118 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0     1580 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0     1388 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1094 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1659 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0     1479 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1357 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1267 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1465 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0     1308 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      165 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    14718 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0     1957 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    12051 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/decoders.py
+-rw-r--r--   0        0        0      451 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     3486 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     1119 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0     2657 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     3480 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     1823 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     1148 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0      160 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      442 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3168 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3058 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0       40 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/topic.py
+-rw-r--r--   0        0        0     6632 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     5464 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0     6107 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0    10172 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     3876 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     3583 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    21173 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    13387 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     7175 2023-06-25 19:45:07.057018 gridworks_protocol-0.5.5/src/gwproto/types/gt_boolean_actuator_component.py
+-rw-r--r--   0        0        0     8431 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     5782 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     4959 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     5570 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     5313 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    12770 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11864 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    13625 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    12328 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8369 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0     9449 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0    21533 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0     9915 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    11254 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7606 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     2751 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0    11076 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0     7602 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11686 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0     8084 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0    20734 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7268 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     5991 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    18195 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    14031 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    12205 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     2556 2023-06-25 19:45:07.061018 gridworks_protocol-0.5.5/src/gwproto/utils.py
+-rw-r--r--   0        0        0     3619 1970-01-01 00:00:00.000000 gridworks_protocol-0.5.5/setup.py
+-rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 gridworks_protocol-0.5.5/PKG-INFO
```

### Comparing `gridworks_protocol-0.5.4/LICENSE` & `gridworks_protocol-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/README.md` & `gridworks_protocol-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/pyproject.toml` & `gridworks_protocol-0.5.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.5.4"
+version = "0.5.5"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
@@ -19,15 +19,15 @@
 Changelog = "https://github.com/thegridelectric/gridworks-protocol/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4.0"
 pydantic = "^1.10.2"
 pendulum = "^2.1.2"
 fastapi-utils = "^0.2.1"
-gridworks = "^0.2.6"
+gridworks = "^0.2.7"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gridworks_protocol-0.5.4/src/gwproto/__init__.py` & `gridworks_protocol-0.5.5/src/gwproto/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/relay_cac.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/components/relay_component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/components/relay_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/hardware_layout.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.5.5/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/decoders.py` & `gridworks_protocol-0.5.5/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.5.5/src/gwproto/enums/actor_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.5.5/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.5.5/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/enums/role.py` & `gridworks_protocol-0.5.5/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.5.5/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/enums/unit.py` & `gridworks_protocol-0.5.5/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.5.5/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.5.5/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.5.5/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.5.5/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/message.py` & `gridworks_protocol-0.5.5/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.5.5/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/messages/event.py` & `gridworks_protocol-0.5.5/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/messages/misc.py` & `gridworks_protocol-0.5.5/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/topic.py` & `gridworks_protocol-0.5.5/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/__init__.py` & `gridworks_protocol-0.5.5/src/gwproto/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/component_attribute_class_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.5.5/src/gwproto/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.5.5/src/gwproto/types/egauge_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.5.5/src/gwproto/types/egauge_register_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/electric_meter_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_boolean_actuator_component.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_boolean_actuator_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_status.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.5.5/src/gwproto/types/gt_telemetry.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.5.5/src/gwproto/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.5.5/src/gwproto/types/power_watts.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/relay_cac_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/relay_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/relay_component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/relay_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.5.5/src/gwproto/types/snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.5.5/src/gwproto/types/spaceheat_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.5.5/src/gwproto/types/telemetry_reporting_config.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.5.5/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/src/gwproto/utils.py` & `gridworks_protocol-0.5.5/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.5.4/setup.py` & `gridworks_protocol-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,21 @@
  'gwproto.types']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['fastapi-utils>=0.2.1,<0.3.0',
- 'gridworks>=0.2.6,<0.3.0',
+ 'gridworks>=0.2.7,<0.3.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'gridworks-protocol',
-    'version': '0.5.4',
+    'version': '0.5.5',
     'description': 'Gridworks Protocol',
     'long_description': "# Gridworks Protocol\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-protocol.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/gridworks-protocol.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-protocol)][python version]\n[![License](https://img.shields.io/pypi/l/gridworks-protocol)][license]\n\n[![Read the documentation at https://gridworks-protocol.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-protocol/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-protocol/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-protocol/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/gridworks-protocol/\n[status]: https://pypi.org/project/gridworks-protocol/\n[python version]: https://pypi.org/project/gridworks-protocol\n[read the docs]: https://gridworks-protocol.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-protocol/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-protocol\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Protocol_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-protocol\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Protocol_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-protocol/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-protocol/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-protocol/blob/main/CONTRIBUTING.md\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-protocol',
```

### Comparing `gridworks_protocol-0.5.4/PKG-INFO` & `gridworks_protocol-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.5.4
+Version: 0.5.5
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
-Requires-Dist: gridworks (>=0.2.6,<0.3.0)
+Requires-Dist: gridworks (>=0.2.7,<0.3.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-protocol/releases
 Project-URL: Documentation, https://gridworks-protocol.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-protocol
 Description-Content-Type: text/markdown
```

