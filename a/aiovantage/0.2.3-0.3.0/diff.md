# Comparing `tmp/aiovantage-0.2.3.tar.gz` & `tmp/aiovantage-0.3.0.tar.gz`

## Comparing `aiovantage-0.2.3.tar` & `aiovantage-0.3.0.tar`

### file list

```diff
@@ -1,136 +1,149 @@
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aiovantage-0.2.3/TODO
--rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 aiovantage-0.2.3/clienttest.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.github/dependabot.yml
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.github/workflows/lint.yml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/dump_system.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/monitor_all.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/control_load.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.2.3/examples/tasks/run_task.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/query.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0    18922 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/client.py
--rw-r--r--   0        0        0    10260 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/connection.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/errors.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/response.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/client.py
--rw-r--r--   0        0        0     7546 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/connection.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/errors.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/config_client/objects/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 aiovantage-0.2.3/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 aiovantage-0.2.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.2.3/LICENSE
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 aiovantage-0.2.3/README.md
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 aiovantage-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 aiovantage-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.3.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     6308 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    13502 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aiovantage-0.3.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 aiovantage-0.3.0/README.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 aiovantage-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 aiovantage-0.3.0/PKG-INFO
```

### Comparing `aiovantage-0.2.3/examples/dump_system.py` & `aiovantage-0.3.0/examples/dump_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,12 +101,12 @@
 
     # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Preload all the objects we want to dump
         await vantage.initialize()
 
         # Recursively print the root area and all its children
-        print_area(vantage, vantage.areas.root)
+        print_area(vantage, vantage.areas.get(area_id=0))
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/monitor_all.py` & `aiovantage-0.3.0/examples/monitor_all.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to updates for all objects
         vantage.subscribe(callback)
 
         # Fetch all known objects from the controller
         await vantage.initialize()
```

### Comparing `aiovantage-0.2.3/examples/areas/dump_areas.py` & `aiovantage-0.3.0/examples/blinds/dump_blinds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Prints out the id and name of each area in the Vantage controller."""
+"""Prints out the id and name of each blind in the Vantage controller."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage import Vantage
@@ -17,15 +17,16 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for area in vantage.areas:
-            print(f"[{area.id}] '{area.name}'")
+        # Print out the id and name of each blind
+        async for blind in vantage.blinds:
+            print(f"[{blind.id}] '{blind.name}'")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.3.0/examples/blind_groups/dump_blind_groups.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out details of each blind group
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Print out details of each blind group
         async for blind_group in vantage.blind_groups:
             print(f"[{blind_group.id}] '{blind_group.name}'")
             async for blind in vantage.blind_groups.blinds(blind_group.id):
                 print(f"    [{blind.id}] '{blind.name}'")
 
 
 with contextlib.suppress(KeyboardInterrupt):
```

### Comparing `aiovantage-0.2.3/examples/blinds/dump_blinds.py` & `aiovantage-0.3.0/examples/gmem/dump_gmem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Prints out the id and name of each blind in the Vantage controller."""
+"""Prints out the id, name, and value of each variable in the Vantage controller."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage import Vantage
@@ -17,15 +17,16 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for blind in vantage.blinds:
-            print(f"[{blind.id}] '{blind.name}'")
+        # Print out the id, name, and value of each variable
+        async for gmem in vantage.gmem:
+            print(f"[{gmem.id}] '{gmem.name}' = {repr(gmem.value)}")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/blinds/monitor_blinds.py` & `aiovantage-0.3.0/examples/blinds/monitor_blinds.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,20 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all loads
+        # Subscribe to updates for all blinds
         vantage.blinds.subscribe(callback)
 
-        # Fetch all known loads from the controller
+        # Fetch all known blinds from the controller
         await vantage.blinds.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
```

### Comparing `aiovantage-0.2.3/examples/buttons/dump_buttons.py` & `aiovantage-0.3.0/examples/buttons/dump_buttons.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Print out the id, name, and labels of each button
         async for button in vantage.buttons:
             print(
                 f"[{button.id}] name='{button.name}' "
                 f"text1='{button.text1}' text2='{button.text2}'"
             )
```

### Comparing `aiovantage-0.2.3/examples/buttons/monitor_buttons.py` & `aiovantage-0.3.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""Fetch all buttons from the Vantage controller, and print out any state changes."""
+"""Fetch all omni sensors from the Vantage controller, and print any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import Button
+from aiovantage.config_client.objects import OmniSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: Button, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: OmniSensor, data: Dict[str, Any]) -> None:
     """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[Button added] '{obj.name}' ({obj.id})")
+        print(f"[Sensor added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[Button updated] '{obj.name}' ({obj.id})")
+        print(f"[Sensor updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all buttons
-        vantage.buttons.subscribe(callback)
+        # Subscribe to updates for all sensors
+        vantage.omni_sensors.subscribe(callback)
 
-        # Fetch all known loads from the controller
-        await vantage.buttons.initialize()
+        # Fetch all known sensors from the controller
+        await vantage.omni_sensors.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/command_client/event_log.py` & `aiovantage-0.3.0/examples/command_client/status_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,52 @@
-"""Example of using the CommandClient to subscribe to system log events."""
+"""Use a CommandClient to subscribe to status updates for LOAD objects."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
-from aiovantage.command_client import CommandClient, Event, EventType
+from aiovantage.command_client import Event, EventStream, EventType
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
 def command_client_callback(event: Event) -> None:
-    """Print out the log message for each event."""
-    if event["tag"] == EventType.EVENT_LOG:
-        print(event["log"])
-    elif event["tag"] == EventType.CONNECTED:
-        print("Connected and monitoring for log events...")
+    """Print out the status update for each event."""
+    if event["type"] == EventType.STATUS:
+        print(f"[{event['status_type']}] id: {event['id']}, args: {event['args']}")
+    elif event["type"] == EventType.CONNECTED:
+        print("Connected and monitoring for status updates...")
+    elif event["type"] == EventType.DISCONNECTED:
+        print("Disconnected")
+    elif event["type"] == EventType.RECONNECTED:
+        print("Reconnected")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Create a Host Command client
-    async with CommandClient(args.host, args.username, args.password) as client:
+    # Create an EventStream client
+    async with EventStream(args.host, args.username, args.password) as events:
         # Subscribe to connection events
-        client.subscribe(command_client_callback, EventType.CONNECTED)
+        events.subscribe(
+            command_client_callback,
+            (EventType.CONNECTED, EventType.DISCONNECTED, EventType.RECONNECTED),
+        )
 
-        # Subscribe to system log events
-        await client.subscribe_event_log(command_client_callback, "SYSTEM")
+        # Subscribe to status updates for LOAD objects (STATUS LOAD)
+        events.subscribe_status(command_client_callback, "LOAD")
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/command_client/status_load.py` & `aiovantage-0.3.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-"""Use a CommandClient to subscribe to status updates for LOAD objects."""
+"""Fetch all anemo sensors from the Vantage controller, and print any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
+from typing import Any, Dict
 
-from aiovantage.command_client import CommandClient, Event, EventType
+from aiovantage import Vantage, VantageEvent
+from aiovantage.config_client.objects import AnemoSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def command_client_callback(event: Event) -> None:
-    """Print out the status update for each event."""
-    if event["tag"] == EventType.STATUS:
-        print(f"[{event['status_type']}] id: {event['id']}, args: {event['args']}")
-    elif event["tag"] == EventType.CONNECTED:
-        print("Connected and monitoring for status updates...")
-    elif event["tag"] == EventType.DISCONNECTED:
-        print("Disconnected")
-    elif event["tag"] == EventType.RECONNECTED:
-        print("Reconnected")
+def callback(event: VantageEvent, obj: AnemoSensor, data: Dict[str, Any]) -> None:
+    """Print out any state changes."""
+    if event == VantageEvent.OBJECT_ADDED:
+        print(f"[Sensor added] '{obj.name}' ({obj.id})")
+
+    elif event == VantageEvent.OBJECT_UPDATED:
+        print(f"[Sensor updated] '{obj.name}' ({obj.id})")
+        for attr in data.get("attrs_changed", []):
+            print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Create a Host Command client
-    async with CommandClient(args.host, args.username, args.password) as client:
-        # Subscribe to connection events
-        client.subscribe(
-            command_client_callback,
-            (EventType.CONNECTED, EventType.DISCONNECTED, EventType.RECONNECTED),
-        )
+    # Connect to the Vantage controller
+    async with Vantage(args.host, args.username, args.password) as vantage:
+        # Subscribe to updates for all sensors
+        vantage.anemo_sensors.subscribe(callback)
 
-        # Subscribe to status updates for LOAD objects (STATUS LOAD)
-        await client.subscribe_status(command_client_callback, "LOAD")
+        # Fetch all known sensors from the controller
+        await vantage.anemo_sensors.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/config_client/dump_objects.py` & `aiovantage-0.3.0/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/examples/config_client/get_version.py` & `aiovantage-0.3.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.3.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Print some details about each dry contact
+        # Print out the id and name of each dry contact
         async for dry_contact in vantage.dry_contacts:
             print(f"[{dry_contact.id}] name='{dry_contact.name}' ")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.3.0/examples/buttons/monitor_buttons.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""Fetch all dry contacts from the Vantage controller, and print any state changes."""
+"""Fetch all buttons from the Vantage controller, and print out any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import DryContact
+from aiovantage.config_client.objects import Button
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: DryContact, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: Button, data: Dict[str, Any]) -> None:
     """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
-        print(f"[DryContact added] '{obj.name}' ({obj.id})")
+        print(f"[Button added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
-        print(f"[DryContact updated] '{obj.name}' ({obj.id})")
+        print(f"[Button updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
             print(f"    {attr} = {getattr(obj, attr)}")
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to updates for all buttons
-        vantage.dry_contacts.subscribe(callback)
+        vantage.buttons.subscribe(callback)
 
-        # Fetch all known loads from the controller
-        await vantage.dry_contacts.initialize()
+        # Fetch all known buttons from the controller
+        await vantage.buttons.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/gmem/dump_gmem.py` & `aiovantage-0.3.0/examples/loads/dump_loads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Prints out the id, name, and value of each variable in the Vantage controller."""
+"""Prints out the id, name, and level of each load in the Vantage controller."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage import Vantage
@@ -17,15 +17,16 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and value of each GMem
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for gmem in vantage.gmem:
-            print(f"[{gmem.id}] '{gmem.name}' = {repr(gmem.value)}")
+        # Print out the id, name, and level of each load
+        async for load in vantage.loads:
+            print(f"[{load.id}] '{load.name}' level={load.level}%")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/gmem/monitor_gmem.py` & `aiovantage-0.3.0/examples/gmem/monitor_gmem.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,19 +30,20 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        # Subscribe to updates for all GMem objects
+        # Subscribe to updates for all variables
         vantage.gmem.subscribe(callback)
 
-        # Fetch all known GMem objects from the controller
+        # Fetch all known variables from the controller
         await vantage.gmem.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
```

### Comparing `aiovantage-0.2.3/examples/gmem/set_gmem.py` & `aiovantage-0.3.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/examples/load_groups/dump_load_groups.py` & `aiovantage-0.3.0/examples/load_groups/dump_load_groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Print out the id, name, and members of each load group
         async for load_group in vantage.load_groups:
             print(load_group)
             print(f"[{load_group.id}] '{load_group.name}' {load_group.load_ids}")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/loads/control_load.py` & `aiovantage-0.3.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/examples/loads/dump_loads.py` & `aiovantage-0.3.0/examples/stations/dump_stations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Prints out the id, name, and level of each load in the Vantage controller."""
+"""Prints out the id and name of each station in the Vantage controller."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage import Vantage
@@ -17,15 +17,16 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for load in vantage.loads:
-            print(f"[{load.id}] '{load.name}' level={load.level}%")
+        # Print out the id and name of each station
+        async for station in vantage.stations:
+            print(f"[{station.id}] '{station.name}'")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/loads/monitor_loads.py` & `aiovantage-0.3.0/examples/loads/monitor_loads.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to updates for all loads
         vantage.loads.subscribe(callback)
 
         # Fetch all known loads from the controller
         await vantage.loads.initialize()
```

### Comparing `aiovantage-0.2.3/examples/loads/poll_on_loads.py` & `aiovantage-0.3.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/examples/loads/toggle_load.py` & `aiovantage-0.3.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.3.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Print out the id, name, and level of each omni sensor
         async for omni_sensor in vantage.omni_sensors:
             level = f"{omni_sensor.level}" if omni_sensor.level is not None else "?"
             print(f"[{omni_sensor.id}] '{omni_sensor.name}' = {level}")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.3.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-"""Fetch all omni sensors from the Vantage controller, and print any state changes."""
+"""Fetch all light sensors from the Vantage controller, and print any state changes."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import Any, Dict
 
 from aiovantage import Vantage, VantageEvent
-from aiovantage.config_client.objects import OmniSensor
+from aiovantage.config_client.objects import LightSensor
 
 # Grab connection info from command line arguments
 parser = argparse.ArgumentParser(description="aiovantage example")
 parser.add_argument("host", help="hostname of Vantage controller")
 parser.add_argument("--username", help="username for Vantage controller")
 parser.add_argument("--password", help="password for Vantage controller")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-def callback(event: VantageEvent, obj: OmniSensor, data: Dict[str, Any]) -> None:
+def callback(event: VantageEvent, obj: LightSensor, data: Dict[str, Any]) -> None:
     """Print out any state changes."""
     if event == VantageEvent.OBJECT_ADDED:
         print(f"[Sensor added] '{obj.name}' ({obj.id})")
 
     elif event == VantageEvent.OBJECT_UPDATED:
         print(f"[Sensor updated] '{obj.name}' ({obj.id})")
         for attr in data.get("attrs_changed", []):
@@ -32,18 +32,18 @@
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to updates for all sensors
-        vantage.omni_sensors.subscribe(callback)
+        vantage.light_sensors.subscribe(callback)
 
         # Fetch all known sensors from the controller
-        await vantage.omni_sensors.initialize()
+        await vantage.light_sensors.initialize()
 
         # Keep running for a while
         await asyncio.sleep(3600)
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.3.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and level of each load
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
+        # Print out the id, name, and state of each RGB load
         async for rgb_load in vantage.rgb_loads:
             print(
                 f"[{rgb_load.id}] '{rgb_load.name}' "
                 f"is {'ON' if rgb_load.is_on else 'OFF'}"
             )
```

### Comparing `aiovantage-0.2.3/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.3.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Subscribe to RGB load updates
         vantage.rgb_loads.subscribe(callback)
 
         # Fetch all known RGB loads from the controller
         await vantage.rgb_loads.initialize()
```

### Comparing `aiovantage-0.2.3/examples/stations/dump_stations.py` & `aiovantage-0.3.0/examples/tasks/dump_tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Prints out the id and name of each station in the Vantage controller."""
+"""Prints out the id, name, and state of each task in the Vantage controller."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage import Vantage
@@ -17,14 +17,16 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for station in vantage.stations:
-            print(f"[{station.id}] '{station.name}'")
+        # Print out the id, name, and state of each task
+        async for task in vantage.tasks:
+            print(f"[{task.id}] '{task.name}' is_running={task.is_running}")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/tasks/dump_tasks.py` & `aiovantage-0.3.0/examples/light_sensors/dump_light_sensors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Prints out the id, name, and running state of each task in the Vantage controller."""
+"""Prints out the id, name, and level of each light sensor in the Vantage controller."""
 
 import argparse
 import asyncio
 import contextlib
 import logging
 
 from aiovantage import Vantage
@@ -17,15 +17,16 @@
 
 
 async def main() -> None:
     """Run code example."""
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
-    # Connect to the Vantage controller and print out the name and value of each GMem
+    # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
-        async for task in vantage.tasks:
-            print(f"[{task.id}] '{task.name}' is_running={task.is_running}")
+        # Print out the id, name, and level of each light sensor
+        async for sensor in vantage.light_sensors:
+            print(f"[{sensor.id}] '{sensor.name}' = {sensor.level}")
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.2.3/examples/tasks/run_task.py` & `aiovantage-0.3.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/__init__.py` & `aiovantage-0.3.0/src/aiovantage/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 
 import asyncio
 from types import TracebackType
 from typing import Callable, Optional, Type
 
 from typing_extensions import Self
 
-from aiovantage.command_client import CommandClient
+from aiovantage.command_client import CommandClient, EventStream
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.objects import SystemObject
+from aiovantage.controllers.anemo_sensors import AnemoSensorsController
 from aiovantage.controllers.areas import AreasController
 from aiovantage.controllers.base import EventCallback
 from aiovantage.controllers.blind_groups import BlindGroupsController
 from aiovantage.controllers.blinds import BlindsController
 from aiovantage.controllers.buttons import ButtonsController
 from aiovantage.controllers.dry_contacts import DryContactsController
 from aiovantage.controllers.gmem import GMemController
+from aiovantage.controllers.light_sensors import LightSensorsController
 from aiovantage.controllers.load_groups import LoadGroupsController
 from aiovantage.controllers.loads import LoadsController
 from aiovantage.controllers.masters import MastersController
 from aiovantage.controllers.omni_sensors import OmniSensorsController
 from aiovantage.controllers.rgb_loads import RGBLoadsController
 from aiovantage.controllers.stations import StationsController
 from aiovantage.controllers.tasks import TasksController
+from aiovantage.controllers.temperature_sensors import TemperatureSensorsController
 
 from .events import VantageEvent
 
 
 class Vantage:
     """Control a Vantage InFusion controller."""
 
@@ -40,40 +43,48 @@
         *,
         use_ssl: bool = True,
         config_port: Optional[int] = None,
         command_port: Optional[int] = None,
     ) -> None:
         """Initialize the Vantage instance."""
 
-        # Set up config and command clients
+        # Set up clients
         self._config_client = ConfigClient(
             host, username, password, ssl=use_ssl, port=config_port
         )
 
         self._command_client = CommandClient(
             host, username, password, ssl=use_ssl, port=command_port
         )
 
+        self._event_stream = EventStream(
+            host, username, password, ssl=use_ssl, port=command_port
+        )
+
         # Set up controllers
+        self._anemo_sensors = AnemoSensorsController(self)
         self._areas = AreasController(self)
         self._blinds = BlindsController(self)
         self._blind_groups = BlindGroupsController(self)
         self._buttons = ButtonsController(self)
         self._dry_contacts = DryContactsController(self)
         self._gmem = GMemController(self)
+        self._light_sensors = LightSensorsController(self)
         self._loads = LoadsController(self)
         self._load_groups = LoadGroupsController(self)
         self._masters = MastersController(self)
         self._rgb_loads = RGBLoadsController(self)
         self._omni_sensors = OmniSensorsController(self)
         self._stations = StationsController(self)
         self._tasks = TasksController(self)
+        self._temperature_sensors = TemperatureSensorsController(self)
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
+        await self.event_stream.start()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
@@ -90,14 +101,24 @@
 
     @property
     def command_client(self) -> CommandClient:
         """Return the command client."""
         return self._command_client
 
     @property
+    def event_stream(self) -> EventStream:
+        """Return the event stream."""
+        return self._event_stream
+
+    @property
+    def anemo_sensors(self) -> AnemoSensorsController:
+        """Return the AnemoSensors controller for managing anemo sensors."""
+        return self._anemo_sensors
+
+    @property
     def areas(self) -> AreasController:
         """Return the Areas controller for managing areas."""
         return self._areas
 
     @property
     def blinds(self) -> BlindsController:
         """Return the Blinds controller for managing blinds."""
@@ -115,14 +136,19 @@
 
     @property
     def dry_contacts(self) -> DryContactsController:
         """Return the DryContacts controller for managing dry contacts."""
         return self._dry_contacts
 
     @property
+    def light_sensors(self) -> LightSensorsController:
+        """Return the LightSensors controller for managing light sensors."""
+        return self._light_sensors
+
+    @property
     def loads(self) -> LoadsController:
         """Return the Load controller for managing loads (lights, fans, etc)."""
         return self._loads
 
     @property
     def load_groups(self) -> LoadGroupsController:
         """Return the LoadGroup controller for managing groups of loads."""
@@ -154,58 +180,70 @@
         return self._stations
 
     @property
     def tasks(self) -> TasksController:
         """Return the Tasks controller for managing tasks."""
         return self._tasks
 
+    @property
+    def temperature_sensors(self) -> TemperatureSensorsController:
+        """Return the TemperatureSensors controller for managing temperature sensors."""
+        return self._temperature_sensors
+
     async def close(self) -> None:
         """Close the clients."""
 
         self.config_client.close()
-        await self.command_client.close()
+        self.command_client.close()
+        await self.event_stream.stop()
 
     async def initialize(self) -> None:
         """Fetch all objects from the controllers."""
 
         await asyncio.gather(
+            self._anemo_sensors.initialize(),
             self._areas.initialize(),
             self._blinds.initialize(),
             self._blind_groups.initialize(),
             self._buttons.initialize(),
             self._dry_contacts.initialize(),
             self._gmem.initialize(),
+            self._light_sensors.initialize(),
             self._loads.initialize(),
             self._masters.initialize(),
             self._rgb_loads.initialize(),
             self._omni_sensors.initialize(),
             self._stations.initialize(),
             self._tasks.initialize(),
+            self._temperature_sensors.initialize(),
         )
 
     def subscribe(self, callback: EventCallback[SystemObject]) -> Callable[[], None]:
         """Subscribe to state changes for all objects.
 
         Returns:
             A function to unsubscribe.
         """
 
         unsubscribes = [
+            self.anemo_sensors.subscribe(callback),
             self.areas.subscribe(callback),
             self.blinds.subscribe(callback),
             self.blind_groups.subscribe(callback),
             self.buttons.subscribe(callback),
             self.dry_contacts.subscribe(callback),
             self.gmem.subscribe(callback),
+            self.light_sensors.subscribe(callback),
             self.loads.subscribe(callback),
             self.masters.subscribe(callback),
             self.rgb_loads.subscribe(callback),
             self.omni_sensors.subscribe(callback),
             self.stations.subscribe(callback),
             self.tasks.subscribe(callback),
+            self.temperature_sensors.subscribe(callback),
         ]
 
         def unsubscribe() -> None:
             for unsub in unsubscribes:
                 unsub()
 
         return unsubscribe
```

### Comparing `aiovantage-0.2.3/src/aiovantage/query.py` & `aiovantage-0.3.0/src/aiovantage/query.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/README.md` & `aiovantage-0.3.0/src/aiovantage/command_client/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     await client.command("LOAD", 118, 100)
 ```
 
 
 ### Subscribe to load events
 
 ```python
-from aiovantage.command_client import CommandClient, Event, EventType
+from aiovantage.command_client import Event, EventStream, EventType
 
 def callback(event: Event) -> None:
-    assert event["tag"] == EventType.STATUS
+    assert event["type"] == EventType.STATUS
     print(f"Load {event['id']} changed state")
 
-client = CommandClient("10.2.0.103")
-await client.subscribe_status(callback, "LOAD")
+events = EventStream("10.2.0.103")
+await events.subscribe_status(callback, "LOAD")
 ```
```

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/client.py` & `aiovantage-0.3.0/src/aiovantage/command_client/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,517 +1,390 @@
-"""Client to communicate with the Host Command service."""
+"""Subscribe to events from the Vantage Host Command service."""
 
 import asyncio
 import logging
 from collections import defaultdict
 from contextlib import suppress
-from decimal import Decimal
+from enum import Enum
 from inspect import iscoroutinefunction
 from ssl import SSLContext
 from types import TracebackType
 from typing import (
-    Awaitable,
     Callable,
     Coroutine,
     Dict,
     Iterable,
     List,
+    Literal,
     Optional,
+    Sequence,
     Tuple,
     Type,
+    TypedDict,
     Union,
 )
 
 from typing_extensions import Self
 
-from .connection import CommandConnection
-from .errors import ClientConnectionError, ClientError, ClientTimeoutError
-from .events import Event, EventType
-from .response import CommandResponse
+from aiovantage.errors import ClientConnectionError, ClientError
+
+from .commands import CommandConnection
 from .utils import tokenize_response
 
-# Constants
 KEEPALIVE_INTERVAL = 60
 
+
+# Typing for events
+class EventType(Enum):
+    """Enumeration of event types."""
+
+    CONNECTED = "connect"
+    DISCONNECTED = "disconnect"
+    RECONNECTED = "reconnect"
+    STATUS = "status"
+    ENHANCED_LOG = "enhanced_log"
+
+
+# Typed dictionaries for events
+class ConnectEvent(TypedDict):
+    type: Literal[EventType.CONNECTED]
+
+
+class DisconnectEvent(TypedDict):
+    type: Literal[EventType.DISCONNECTED]
+
+
+class ReconnectEvent(TypedDict):
+    type: Literal[EventType.RECONNECTED]
+
+
+class StatusEvent(TypedDict):
+    type: Literal[EventType.STATUS]
+    id: int
+    status_type: str
+    args: Sequence[str]
+
+
+class EnhancedLogEvent(TypedDict):
+    type: Literal[EventType.ENHANCED_LOG]
+    log: str
+
+
+Event = Union[
+    ConnectEvent, DisconnectEvent, ReconnectEvent, StatusEvent, EnhancedLogEvent
+]
+
 # Type aliases for callbacks for event subscriptions
 EventCallback = Callable[[Event], Union[None, Coroutine]]
 EventFilter = Callable[[Event], bool]
 EventSubscription = Tuple[EventCallback, Optional[EventFilter]]
 
 
-class CommandClient:
-    """Client to communicate with the Host Command service.
-
-    This class handles connecting to the Host Command service, sending commands, and
-    receiving events. It also provides helper methods for subscribing to various types
-    of events, such as "STATUS" and "ELLOG".
-
-    Connections are created lazily when needed, and closed when the client is closed,
-    and will automatically reconnect if the connection is lost.
-    """
+class EventStream:
+    """Client to subscribe to events from the Vantage Host Command service."""
 
     def __init__(
         self,
         host: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         *,
         ssl: Union[SSLContext, bool] = True,
         port: Optional[int] = None,
-        conn_timeout: Optional[float] = 5,
-        read_timeout: Optional[float] = 10,
+        conn_timeout: float = 30,
     ) -> None:
-        """Initialize the CommandClient instance.
-
-        Args:
-            host: The hostname or IP address of the Host Command service.
-            username: The username to use to authenticate, if required.
-            password: The password to use to authenticate, if required.
-            ssl: Whether to use SSL when connecting. If True, a default SSL context will
-                be created. If False, SSL will not be used. If a SSLContext is provided,
-                it will be used.
-            port: The port to use when connecting. Defaults to 3010 if SSL is enabled,
-                otherwise 3001.
-            conn_timeout: The timeout to use when connecting, in seconds.
-            read_timeout: The timeout to use when reading, in seconds.
-        """
-
-        self._host = host
+        """Initialize the client."""
+        self._connection = CommandConnection(host, port, ssl, conn_timeout)
         self._username = username
         self._password = password
-        self._ssl = ssl
-        self._port = port
-        self._conn_timeout = conn_timeout
-        self._read_timeout = read_timeout
-
-        self._connection: Optional[CommandConnection] = None
-        self._event_handler_task: Optional[asyncio.Task[None]] = None
-        self._event_handler_ready: asyncio.Event = asyncio.Event()
-        self._keepalive_task: Optional[asyncio.Task[None]] = None
+        self._tasks: List[asyncio.Task[None]] = []
         self._subscriptions: List[EventSubscription] = []
-        self._subscribed_statuses: Dict[str, int] = defaultdict(int)
-        self._subscribed_objects: Dict[int, int] = defaultdict(int)
-        self._subscribed_event_logs: Dict[str, int] = defaultdict(int)
+        self._status_subscribers: Dict[str, int] = defaultdict(int)
+        self._enhanced_log_subscribers: Dict[str, int] = defaultdict(int)
+        self._connection_lock = asyncio.Lock()
+        self._command_queue: asyncio.Queue[str] = asyncio.Queue()
         self._logger = logging.getLogger(__name__)
-        self._lock = asyncio.Lock()
 
     async def __aenter__(self) -> Self:
         """Return context manager."""
+        await self.start()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         """Exit context manager."""
-        await self.close()
+        await self.stop()
         if exc_val:
             raise exc_val
 
-    async def connection(self, retry: bool = False) -> CommandConnection:
-        """Get a connection to the Host Command service, creating one if necessary.
-
-        Args:
-            retry: Whether to retry if the connection attempt fails.
-        """
-
-        try:
-            # Note: Getting a connection can potentially block for a long time even if
-            # retry is False, if someone else is already trying to get a connection.
-            await asyncio.wait_for(
-                self._lock.acquire(), timeout=(None if retry else self._conn_timeout)
-            )
-        except asyncio.TimeoutError as exc:
-            raise ClientTimeoutError("Timeout waiting for connection") from exc
+    async def start(self) -> None:
+        """Initialize the event stream."""
+        await self.get_connection()
+        self._tasks.append(asyncio.create_task(self._message_handler()))
+        self._tasks.append(asyncio.create_task(self._command_handler()))
+        self._tasks.append(asyncio.create_task(self._keepalive()))
+
+    async def stop(self) -> None:
+        """Stop the event stream."""
+        for task in self._tasks:
+            task.cancel()
+        self._tasks.clear()
+        self._connection.close()
+
+    async def get_connection(self) -> CommandConnection:
+        """Get a connection to the Host Command service."""
+        async with self._connection_lock:
+            if self._connection.closed:
+                # Open a new connection
+                await self._connection.open()
 
-        try:
-            if self._connection is None or self._connection.closed:
-                self._connection = await self._create_connection(retry=retry)
+                # Authenticate the new connection if we have credentials
+                if self._username is not None and self._password is not None:
+                    await self._send(f"LOGIN {self._username} {self._password}")
 
             return self._connection
-        finally:
-            self._lock.release()
-
-    async def close(self) -> None:
-        """Close the connections to the Host Command service and cancel any running tasks."""
-
-        # Cancel the keepalive task
-        if self._keepalive_task is not None:
-            self._keepalive_task.cancel()
-            self._keepalive_task = None
-
-        # Cancel the event handler task
-        if self._event_handler_task is not None:
-            self._event_handler_task.cancel()
-            self._event_handler_task = None
-
-        # Close the connections
-        if self._connection is not None:
-            self._connection.close()
-
-    async def command(
-        self,
-        command: str,
-        *params: Union[str, int, float, Decimal, bool],
-        force_quotes: bool = False,
-    ) -> CommandResponse:
-        """Send a command to the Host Command service and wait for a response.
-
-        Handles encoding the parameters correctly, and raises an exception if the
-        response line is R:ERROR.
-
-        Args:
-            command: The command to send, should be a single word string.
-            params: The parameters to send with the command.
-            force_quotes: Whether to force string params to be wrapped in double quotes.
-
-        Returns:
-            A CommandResponse instance.
-        """
-
-        conn = await self.connection()
-        return await conn.command(command, *params, force_quotes=force_quotes)
 
     def subscribe(
         self,
         callback: EventCallback,
         event_filter: Union[EventType, Iterable[EventType], EventFilter, None] = None,
     ) -> Callable[[], None]:
-        """Subscribe to Host Command events, optionally filtering by event type.
+        """Subscribe to events from the Host Command service.
 
         Args:
-            callback: The callback to call when an event is received.
-            event_filter: The event type(s) to filter by, or None to receive all events.
+            callback: The callback to invoke when an event is received.
+            event_filter: A filter to apply to events before invoking the callback.
 
         Returns:
-            A callback that can be called to unsubscribe.
+            A function that can be used to unsubscribe from events.
         """
 
         # Support filtering by event type, a list of event types, or a predicate
-        filter_fn: Optional[EventFilter]
+        subscription: EventSubscription
         if isinstance(event_filter, EventType):
-
-            def filter_fn(event: Event) -> bool:
-                return event["tag"] == event_filter
-
+            subscription = (callback, lambda event: event["type"] == event_filter)
         elif isinstance(event_filter, Iterable):
-
-            def filter_fn(event: Event) -> bool:
-                return event["tag"] in event_filter
-
+            subscription = (callback, lambda event: event["type"] in event_filter)  # type: ignore[operator]
         else:
-            filter_fn = event_filter
+            subscription = (callback, event_filter)
 
-        # Add the subscription
-        subscription: EventSubscription = (callback, filter_fn)
         self._subscriptions.append(subscription)
 
         # Return an unsubscribe callback to remove the subscription
         def unsubscribe() -> None:
             self._subscriptions.remove(subscription)
 
         return unsubscribe
 
-    async def subscribe_status(
-        self, callback: EventCallback, status_types: Union[str, Iterable[str]]
-    ) -> Callable[[], Awaitable[None]]:
-        """Subscribe to status events for the given status types, using "STATUS {type}".
+    def subscribe_status(
+        self, callback: EventCallback, status_type: str
+    ) -> Callable[[], None]:
+        """Subscribe to "Status" events from the Host Command service.
 
         Args:
-            callback: The callback to call when a status event is received.
-            status_types: The status types to subscribe to status events for.
+            callback: The callback to invoke when an event is received.
+            status_type: The type of status to subscribe to.
 
         Returns:
-            A coroutine to unsubscribe from status events.
+            A coroutine that can be used to unsubscribe from status events.
         """
 
-        # Start the event handler if it's not already running
-        await self._start_event_handler()
-
-        # Support both a single status type and a list of status types
-        if isinstance(status_types, str):
-            status_types = (status_types,)
-
-        # Filter received status events by type
-        def event_filter(event: Event) -> bool:
-            return (
-                event["tag"] == EventType.STATUS
-                and event["status_type"] in status_types
-            )
-
-        # Add the subscription to the list
-        remove_subscription = self.subscribe(callback, event_filter)
-
-        # Ask the Host Command service to start sending status events
-        conn = await self.connection()
-        for status_type in status_types:
-            self._subscribed_statuses[status_type] += 1
-            if self._subscribed_statuses[status_type] == 1:
-                await conn.command("STATUS", status_type)
-
-        # Return an unsubscribe callback
-        async def unsubscribe() -> None:
-            for status_type in status_types:
-                # Note: there's no nice way to ask the Host Command service to stop
-                # sending status events of a particular type.
-                self._subscribed_statuses[status_type] -= 1
+        # Enable this status type if it's not already enabled
+        self._status_subscribers[status_type] += 1
+        if self._status_subscribers[status_type] == 1:
+            self._enable_status(status_type)
+
+        # Subscribe, and return an unsubscribe callback
+        remove_subscription = self.subscribe(
+            callback,
+            lambda event: (
+                event["type"] == EventType.STATUS
+                and event["status_type"] == status_type
+            ),
+        )
 
+        def unsubscribe() -> None:
+            self._status_subscribers[status_type] -= 1
+            if self._status_subscribers[status_type] == 0:
+                self._disable_status(status_type)
             remove_subscription()
 
         return unsubscribe
 
-    async def subscribe_objects(
-        self, callback: EventCallback, object_ids: Union[int, Iterable[int]]
-    ) -> Callable[[], Awaitable[None]]:
-        """Subscribe to status events for the given object ids, using "ADDSTATUS {id}".
+    def subscribe_enhanced_log(
+        self, callback: EventCallback, log_type: str
+    ) -> Callable[[], None]:
+        """Subscribe to "Enhanced Log" events from the Host Command service.
 
         Args:
-            callback: The callback to call when a status event is received.
-            object_ids: The ids to subscribe to status events for.
+            callback: The callback to invoke when an event is received.
+            log_type: The type of log to subscribe to.
 
         Returns:
-            A coroutine to unsubscribe from status events.
+            A coroutine that can be used to unsubscribe from log events.
         """
 
-        # Start the event handler if it's not already running
-        await self._start_event_handler()
+        # Enable this log type if it's not already enabled
+        self._enhanced_log_subscribers[log_type] += 1
+        if self._enhanced_log_subscribers[log_type] == 1:
+            self._enable_enhanced_log(log_type)
 
-        # Support both a single object id and a list of object ids
-        if isinstance(object_ids, int):
-            object_ids = (object_ids,)
-
-        # Filter recived status events by id
-        def event_filter(event: Event) -> bool:
-            return event["tag"] == EventType.STATUS and event["id"] in object_ids
-
-        # Add the subscription to the list
-        remove_subscription = self.subscribe(callback, event_filter)
-
-        # Ask the controller to start sending status events for these objects
-        conn = await self.connection()
-        for object_id in object_ids:
-            self._subscribed_objects[object_id] += 1
-            if self._subscribed_objects[object_id] == 1:
-                await conn.command("ADDSTATUS", object_id)
-
-        # Return an unsubscribe callback
-        async def unsubscribe() -> None:
-            with suppress(ClientConnectionError):
-                for object_id in object_ids:
-                    self._subscribed_objects[object_id] -= 1
-                    if self._subscribed_objects[object_id] == 0:
-                        await conn.command("DELSTATUS", object_id)
+        # Subscribe, and return an unsubscribe callback
+        remove_subscription = self.subscribe(callback, EventType.ENHANCED_LOG)
 
+        def unsubscribe() -> None:
+            self._enhanced_log_subscribers[log_type] -= 1
+            if self._enhanced_log_subscribers[log_type] == 0:
+                self._disable_enhanced_log(log_type)
             remove_subscription()
 
         return unsubscribe
 
-    async def subscribe_event_log(
-        self, callback: EventCallback, log_types: Union[str, Iterable[str]]
-    ) -> Callable[[], Awaitable[None]]:
-        """Subscribe to event log events, using "ELLOG {type} ON".
+    def emit(self, event: Event) -> None:
+        """Emit an event to subscribers.
 
         Args:
-            callback: The callback to call when an event log event is received.
-            log_types: The event log types to subscribe to.
-
-        Returns:
-            A coroutine to unsubscribe from event log events.
+            event: The event to emit.
         """
-
-        # Start the event handler if it's not already running
-        await self._start_event_handler()
-
-        # Support both a single log type and a list of log types
-        if isinstance(log_types, str):
-            log_types = (log_types,)
-
-        # Add the subscription to the list
-        remove_subscription = self.subscribe(callback, EventType.EVENT_LOG)
-
-        # Get the connection
-        conn = await self.connection()
-
-        # Enable the event log
-        await conn.command("ELAGG ON")
-
-        # Ask the controller to start sending event logs for these types
-        for log_type in log_types:
-            self._subscribed_event_logs[log_type] += 1
-            if self._subscribed_event_logs[log_type] == 1:
-                await conn.command("ELENABLE", log_type, "ON")
-                await conn.command("ELLOG", log_type, "ON")
-
-        # Return an unsubscribe callback
-        async def unsubscribe() -> None:
-            with suppress(ClientConnectionError):
-                for log_type in log_types:
-                    self._subscribed_event_logs[log_type] -= 1
-                    if self._subscribed_event_logs[log_type] == 0:
-                        await conn.command("ELLOG", log_type, "OFF")
-
-            remove_subscription()
-
-        return unsubscribe
-
-    def _emit(self, event: Event) -> None:
-        # Emit an event to any subscribers that are interested in it
-
         for callback, event_filter in self._subscriptions:
             if event_filter is None or event_filter(event):
                 if iscoroutinefunction(callback):
-                    asyncio.create_task(callback(event))  # noqa: RUF006
+                    asyncio.create_task(callback(event))
                 else:
                     callback(event)
 
-    async def _start_event_handler(self) -> None:
-        # Start the event handler if it's not already running
-
-        if self._event_handler_task is None or self._event_handler_task.done():
-            self._event_handler_task = asyncio.create_task(self._event_handler())
-            await self._event_handler_ready.wait()
-
-    async def _create_connection(self, retry: bool = False) -> CommandConnection:
-        # Get a new connection to the Host Command service, authenticating if necessary
-
+    async def _message_handler(self) -> None:
+        # Handle incoming messages from the Host Command service.
         connect_attempts = 0
         while True:
             connect_attempts += 1
-
             try:
-                conn = CommandConnection(
-                    self._host,
-                    self._port,
-                    ssl=self._ssl,
-                    conn_timeout=self._conn_timeout,
-                    read_timeout=self._read_timeout,
-                )
-                await conn.open()
+                # Get the connection to the Host Command service
+                conn = await self.get_connection()
 
-                # Log in if we have credentials
-                if self._username is not None and self._password is not None:
-                    await conn.command("LOGIN", self._username, self._password)
+                # Notify that we're connected
+                self._logger.debug("Connected to EventStream")
+                if connect_attempts == 1:
+                    self.emit({"type": EventType.CONNECTED})
+                else:
+                    self.emit({"type": EventType.RECONNECTED})
+                    self._resubscribe()
+                connect_attempts = 1
+
+                # Wait for new messages
+                while True:
+                    message = await conn.readuntil(b"\r\n")
+                    message = message.rstrip()
+                    self._logger.debug("Received message: %s", message)
+                    self._parse_message(message)
 
-                return conn
             except ClientConnectionError:
-                if not retry:
-                    raise
+                pass  # Pass through to retry logic below
+
+            # If we get here, the connection was lost
+            self.emit({"type": EventType.DISCONNECTED})
+
+            # Clear the command queue
+            with suppress(asyncio.QueueEmpty):
+                while not self._command_queue.empty():
+                    self._command_queue.get_nowait()
+                    self._command_queue.task_done()
 
             # Attempt to reconnect, with backoff
             reconnect_wait = min(2 * connect_attempts, 600)
-
             self._logger.debug(
-                "Connection to controller failed - retrying in %d seconds",
+                "Disconnected from EventStream - retrying in %d seconds",
                 reconnect_wait,
             )
 
+            # Log a warning every 10 attempts
             if connect_attempts % 10 == 0:
                 self._logger.warning(
                     "%d attempts to (re)connect to controller failed"
                     " - This might be an indication of connection issues.",
                     connect_attempts,
                 )
 
             await asyncio.sleep(reconnect_wait)
 
-    async def _resubscribe(self, conn: CommandConnection) -> None:
-        # Re-subscribe to events after a reconnection
-
-        # Re-subscribe to status events
-        for status_type, count in self._subscribed_statuses.items():
-            if count > 0:
-                await conn.command("STATUS", status_type)
-
-        # Re-subscribe to object events
-        for object_id, count in self._subscribed_objects.items():
-            if count > 0:
-                await conn.command("ADDSTATUS", object_id)
-
-        # Re-subscribe to event log events
-        for log_type, count in self._subscribed_event_logs.items():
-            if count > 0:
-                await conn.command("ELENABLE", log_type, "ON")
-                await conn.command("ELLOG", log_type, "ON")
-
-    async def _event_handler(self) -> None:
-        # The event handler task
-
+    async def _command_handler(self) -> None:
+        # Handle outgoing commands to the Host Command service.
         while True:
             try:
-                # Get a connection, retrying if necessary
-                conn = await self.connection(retry=True)
-
-                # Signal that we're connected
-                if self._event_handler_ready.is_set():
-                    await self._resubscribe(conn)
-                    self._emit({"tag": EventType.RECONNECTED})
-                else:
-                    self._event_handler_ready.set()
-                    self._emit({"tag": EventType.CONNECTED})
-
-                self._logger.info("Event handler connected and listening for events")
-
-                # Start the keepalive task
-                self._keepalive_task = asyncio.create_task(self._keepalive())
-
-                # Start processing events
-                async for event in conn.events():
-                    self._logger.debug("Received event: %s", event)
-
-                    if event.startswith("S:"):
-                        # Parse a status message
-                        status_type, id_str, *args = tokenize_response(event)
-                        status_type = status_type[2:]
-
-                        # Notify subscribers
-                        self._emit(
-                            {
-                                "tag": EventType.STATUS,
-                                "status_type": status_type,
-                                "id": int(id_str),
-                                "args": args,
-                            },
-                        )
-                    elif event.startswith("EL:"):
-                        # Parse an event log message
-                        message = event[4:]
-
-                        # Notify subscribers
-                        self._emit(
-                            {
-                                "tag": EventType.EVENT_LOG,
-                                "log": message,
-                            },
-                        )
-                    else:
-                        self._logger.warning("Received unexpected event: %s", event)
-
-            except ClientConnectionError:
-                pass
-
-            except Exception:
-                # Unexpected error, log for debugging
-                self._logger.exception("Unexpected error in event handler")
-                raise
-
-            # If we get here, the connection was lost
-            self._logger.debug("Event handler lost connection")
-            self._emit({"tag": EventType.DISCONNECTED})
-
-            # Cancel the keepalive task
-            if self._keepalive_task is not None:
-                self._keepalive_task.cancel()
-                self._keepalive_task = None
+                command = await self._command_queue.get()
+                await self._send(command)
+                self._command_queue.task_done()
+            except ClientError as err:
+                self._logger.debug("Error while sending command: %s", str(err))
 
     async def _keepalive(self) -> None:
-        # Send an "ECHO" command periodically to keep the connection alive,
-        # and detect dropped connections.
-
+        # Send a periodic "ECHO" keepalive command.
         while True:
             await asyncio.sleep(KEEPALIVE_INTERVAL)
 
             try:
-                await self.command("ECHO")
+                await self._send("ECHO")
             except ClientError as err:
                 self._logger.debug("Error while sending keepalive: %s", str(err))
+
+    async def _send(self, message: str) -> None:
+        # Send a plaintext message to the Host Command service."""
+        self._logger.debug("Sending message: %s", message)
+        await self._connection.write(f"{message}\n")
+
+    def _parse_message(self, message: str) -> None:
+        # Parse a message from the Host Command service.
+        if message.startswith("S:"):
+            # Parse a "Status" message
+            status_type, id_str, *args = tokenize_response(message)
+            self.emit(
+                {
+                    "type": EventType.STATUS,
+                    "status_type": status_type[2:],
+                    "id": int(id_str),
+                    "args": args,
+                }
+            )
+        elif message.startswith("EL:"):
+            # Parse an "Enhanced Log" message
+            self.emit({"type": EventType.ENHANCED_LOG, "log": message[4:]})
+        elif message.startswith("R:ERROR"):
+            self._logger.error("Error message from EventStream: %s", message)
+
+    def _queue_command(self, command: str) -> None:
+        # Queue a command to be sent to the Host Command service.
+        self._command_queue.put_nowait(command)
+
+    def _enable_status(self, status_type: str) -> None:
+        # Enable status updates on the controller for a particular status type.
+        self._queue_command(f"STATUS {status_type}")
+
+    def _disable_status(self, status_type: str) -> None:
+        # Disable status updates on the controller for a particular status type.
+        self._queue_command("STATUS NONE")
+        for status_type, count in self._status_subscribers.items():
+            if count > 0:
+                self._queue_command(f"STATUS {status_type}")
+
+    def _enable_enhanced_log(self, log_type: str) -> None:
+        # Enable enhanced logging on the controller for a particular log type.
+        self._queue_command("ELAGG 1 ON")
+        self._queue_command(f"ELENABLE {log_type} ON")
+        self._queue_command(f"ELLOG {log_type} ON")
+
+    def _disable_enhanced_log(self, log_type: str) -> None:
+        # Disable enhanced logging on the controller for a particular log type.
+        self._queue_command(f"ELLOG {log_type} OFF")
+
+    def _resubscribe(self) -> None:
+        # Re-subscribe to events after a reconnection.
+        for status_type, count in self._status_subscribers.items():
+            if count > 0:
+                self._enable_status(status_type)
+
+        for log_type, count in self._enhanced_log_subscribers.items():
+            if count > 0:
+                self._enable_enhanced_log(log_type)
```

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/utils.py` & `aiovantage-0.3.0/src/aiovantage/command_client/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,16 @@
 """Utility functions for the Host Command service client."""
 
 import re
 from decimal import Decimal
-from ssl import CERT_NONE, PROTOCOL_TLS_CLIENT, SSLContext
 from typing import Sequence, Union
 
 TOKEN_PATTERN = re.compile(r'"([^""]*(?:""[^""]*)*)"|(\{.*?\})|(\S+)')
 
 
-def create_ssl_context() -> SSLContext:
-    """SSL context that doesn't verify hostname or certificate.
-
-    We don't have a local issuer certificate to check against, and we'll most likely be
-    connecting to an IP address, so we can't check the hostname.
-    """
-
-    context = SSLContext(PROTOCOL_TLS_CLIENT)
-    context.check_hostname = False
-    context.verify_mode = CERT_NONE
-    return context
-
-
 def tokenize_response(string: str) -> Sequence[str]:
     """Tokenize a response from the Host Command service.
 
     Handles quoted strings and byte arrays (in curly braces) as single tokens.
 
     Args:
         string: The response string to tokenize.
@@ -43,15 +29,15 @@
 
         tokens.append(token)
 
     return tokens
 
 
 def encode_params(
-    *params: Union[str, int, float, Decimal, bool], force_quotes: bool = False
+    *params: Union[str, int, float, Decimal], force_quotes: bool = False
 ) -> str:
     """Encode a list of parameters for sending to the Host Command service.
 
     Converts all params to strings, wraps strings in double quotes, and escapes
     double quotes.
 
     Args:
@@ -67,15 +53,13 @@
     for value in params:
         if isinstance(value, str):
             if '"' in value or " " in value or force_quotes:
                 value = value.replace('"', '""')
                 encoded_params.append(f'"{value}"')
             else:
                 encoded_params.append(value)
-        elif isinstance(value, bool):
-            encoded_params.append(str(int(value)))
         elif isinstance(value, (int, float, Decimal)):
             encoded_params.append(str(value))
         else:
             raise TypeError(f"Invalid value type: {type(value)}")
 
     return " ".join(encoded_params)
```

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-"""Comand client object interfaces."""
+"""Command client object interfaces."""
 
+from .anemo_sensor import AnemoSensorInterface
 from .blind import BlindInterface
 from .button import ButtonInterface
 from .color_temperature import ColorTemperatureInterface
 from .gmem import GMemInterface
 from .introspection import IntrospectionInterface
+from .light_sensor import LightSensorInterface
 from .load import LoadInterface
 from .object import ObjectInterface
 from .rgb_load import RGBLoadInterface
 from .sensor import SensorInterface
+from .sounder import SounderInterface
 from .task import TaskInterface
+from .temperature import TemperatureInterface
 
 __all__ = [
+    "AnemoSensorInterface",
     "BlindInterface",
     "ButtonInterface",
     "ColorTemperatureInterface",
     "GMemInterface",
     "IntrospectionInterface",
+    "LightSensorInterface",
     "LoadInterface",
     "ObjectInterface",
     "RGBLoadInterface",
     "SensorInterface",
+    "SounderInterface",
     "TaskInterface",
+    "TemperatureInterface",
 ]
```

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/object.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.3.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/README.md` & `aiovantage-0.3.0/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/helpers.py` & `aiovantage-0.3.0/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.3.0/src/aiovantage/config_client/xml_dataclass.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.3.0/src/aiovantage/config_client/methods/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.3.0/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @dataclass
 class OpenFilter:
     """IConfiguration.OpenFilter method definition."""
 
     interface: ClassVar[str] = "IConfiguration"
-    call: Optional["Params"] = xml_element("call", default=None)
+    call: Optional["OpenFilter.Params"] = xml_element("call", default=None)
     return_value: Optional[int] = xml_element("return", default=None)
 
     # @dataclass
     # class Filter:
     #     # TODO: Try using a wrapper
     #     object_type: List[str] = xml_element("ObjectType")
```

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.3.0/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.3.0/src/aiovantage/config_client/methods/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,23 @@
 from .pwm_power_profile import PWMPowerProfile
 from .qis_blind import QISBlind
 from .qube_blind import QubeBlind
 from .relay_blind import RelayBlind
 from .rgb_load import RGBLoad
 from .scene_point_relay import ScenePointRelay
 from .sensor import Sensor
+from .somfy.rs485_group import RS485Group
+from .somfy.rs485_shade import RS485Shade
+from .somfy.urtsi_2_group import URTSI2Group
+from .somfy.urtsi_2_shade import URTSI2Shade
 from .station_bus import StationBus
 from .station_object import StationObject
 from .system_object import SystemObject
 from .task import Task
 from .temperature import Temperature
-from .urtsi_2_group import URTSI2Group
-from .urtsi_2_shade import URTSI2Shade
 
 __all__ = [
     "AnemoSensor",
     "Area",
     "Blind",
     "BlindGroup",
     "Button",
@@ -61,14 +63,16 @@
     "OmniSensor",
     "PowerProfile",
     "PWMPowerProfile",
     "QISBlind",
     "QubeBlind",
     "RelayBlind",
     "RGBLoad",
+    "RS485Group",
+    "RS485Shade",
     "ScenePointRelay",
     "Sensor",
     "StationBus",
     "StationObject",
     "SystemObject",
     "Task",
     "Temperature",
```

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """OmniSensor object."""
 
 from dataclasses import dataclass
+from decimal import Decimal
+from typing import Union
 
 from aiovantage.config_client.xml_dataclass import xml_attribute, xml_element
 
 from .sensor import Sensor
 
 
 @dataclass
@@ -25,14 +27,18 @@
         formula: Formula = xml_element("Formula")
         method: str = xml_element("Method")
         method_hw: str = xml_element("MethodHW")
 
     get: GetMethodType = xml_element("Get")
     parent_id: int = xml_element("Parent")
 
+    def __post_init__(self) -> None:
+        """Post init."""
+        self.level: Union[int, Decimal, None] = None
+
     @property
     def is_current_sensor(self) -> bool:
         """Return True if the sensor is a current sensor."""
         return self.model == "Current"
 
     @property
     def is_power_sensor(self) -> bool:
```

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.3.0/src/aiovantage/config_client/objects/system_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/base.py` & `aiovantage-0.3.0/src/aiovantage/controllers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Sequence,
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 
-from aiovantage.command_client import CommandClient, Event, EventType
+from aiovantage.command_client import CommandClient, Event, EventStream, EventType
 from aiovantage.command_client.utils import tokenize_response
 from aiovantage.config_client import ConfigClient
 from aiovantage.config_client.helpers import get_objects
 from aiovantage.config_client.objects import SystemObject
 from aiovantage.events import VantageEvent
 from aiovantage.query import QuerySet
 
@@ -37,16 +37,16 @@
 EventCallback = Callable[[VantageEvent, T, Dict[str, Any]], None]
 EventSubscription = Tuple[EventCallback[T], Optional[Iterable[VantageEvent]]]
 
 
 class BaseController(QuerySet[T]):
     """Base controller for Vantage objects."""
 
-    # The Vantage object types that this controller handles
     vantage_types: Tuple[str, ...]
+    """The Vantage object types that this controller handles."""
 
     def __init__(self, vantage: "Vantage") -> None:
         """Initialize instance."""
         self._vantage = vantage
         self._items: Dict[int, T] = {}
         self._logger = logging.getLogger(__package__)
         self._subscriptions: List[EventSubscription[T]] = []
@@ -74,14 +74,19 @@
         return self._vantage.config_client
 
     @property
     def command_client(self) -> CommandClient:
         """Return the command client instance."""
         return self._vantage.command_client
 
+    @property
+    def event_stream(self) -> EventStream:
+        """Return the event stream instance."""
+        return self._vantage.event_stream
+
     async def initialize(self) -> None:
         """Initialize a stateless controller by populating the objects it manages."""
 
         if self._initialized:
             return
 
         await self.fetch_objects()
@@ -174,22 +179,22 @@
             else:
                 callback(event_type, obj, data)
 
 
 class StatefulController(BaseController[T]):
     """Base controller for Vantage objects that have state."""
 
-    # Which Vantage status types this controller handles, if any
     status_types: Optional[Tuple[str, ...]] = None
+    """Which Vantage status types this controller handles, if any."""
 
-    # Should we subscribe to status updates from the event log?
-    event_log_status: bool = False
+    enhanced_log_status: bool = False
+    """Should this controller subscribe to updates from the Enhanced Log."""
 
-    # Which status methods this controller handles from the event log
-    event_log_status_methods: Optional[Tuple[str, ...]] = None
+    enhanced_log_status_methods: Optional[Tuple[str, ...]] = None
+    """Which status methods this controller handles from the Enhanced Log."""
 
     @abstractmethod
     async def fetch_object_state(self, vid: int) -> None:
         """Fetch the initial state of an object."""
 
     @abstractmethod
     def handle_object_update(self, vid: int, status: str, args: Sequence[str]) -> None:
@@ -203,48 +208,44 @@
         """
 
         if self._initialized:
             return
 
         await self.fetch_objects()
         await self.fetch_full_state()
-        await self.subscribe_to_updates()
+        self.subscribe_to_updates()
 
-        self.command_client.subscribe(
-            self._handle_command_client_event, EventType.RECONNECTED
-        )
+        self.event_stream.subscribe(self._handle_event, EventType.RECONNECTED)
 
         self._initialized = True
 
     async def fetch_full_state(self) -> None:
         """Fetch the full state of all objects managed by this controller."""
 
         await asyncio.gather(
             *[self.fetch_object_state(obj.id) for obj in self._items.values()]
         )
 
         self._logger.info("%s fetched full state", self.__class__.__name__)
 
-    async def subscribe_to_updates(self) -> None:
+    def subscribe_to_updates(self) -> None:
         """Subscribe to state updates for objects managed by this controller."""
 
         if not self._items:
             return
 
-        # Subscribe to object state updates from the event log
-        if self.event_log_status:
-            await self.command_client.subscribe_event_log(
-                self._handle_command_client_event, ("STATUS", "STATUSEX")
-            )
-
         # Subscribe to "STATUS {type}" updates, if this controller cares about them
         if self.status_types:
-            await self.command_client.subscribe_status(
-                self._handle_command_client_event, self.status_types
-            )
+            for status_type in self.status_types:
+                self.event_stream.subscribe_status(self._handle_event, status_type)
+
+        # Subscribe to object status events from the "Enhanced Log"
+        if self.enhanced_log_status:
+            self.event_stream.subscribe_enhanced_log(self._handle_event, "STATUS")
+            self.event_stream.subscribe_enhanced_log(self._handle_event, "STATUSEX")
 
         self._logger.info("%s subscribed to updates", self.__class__.__name__)
 
     def update_state(self, vid: int, state: Dict[str, Any]) -> None:
         """Update the state of an object and notify subscribers if it changed.
 
         Args:
@@ -271,41 +272,39 @@
         if len(attrs_changed) > 0:
             self.emit(
                 VantageEvent.OBJECT_UPDATED,
                 obj,
                 {"attrs_changed": attrs_changed},
             )
 
-    async def _handle_command_client_event(self, event: Event) -> None:
-        # Handle status update events from the command client
-
-        if event["tag"] == EventType.STATUS:
-            # Handle "STATUS {type}" events
-
+    async def _handle_event(self, event: Event) -> None:
+        # Handle events from the event stream
+        if event["type"] == EventType.STATUS:
+            # Ignore events for objects that this controller doesn't manage
             if event["id"] not in self._items:
                 return
 
+            # Pass the event to the controller
             self.handle_object_update(event["id"], event["status_type"], event["args"])
 
-        elif event["tag"] == EventType.EVENT_LOG:
-            # Handle event log events
-
-            # Filter out events that this controller doesn't care about
+        elif event["type"] == EventType.ENHANCED_LOG:
+            # STATUS/STATUSEX logs can be tokenized the same as command responses
             id_str, method, *args = tokenize_response(event["log"])
+
+            # Ignore events with methods that this controller doesn't care about
             if (
-                self.event_log_status_methods
-                and method not in self.event_log_status_methods
+                self.enhanced_log_status_methods
+                and method not in self.enhanced_log_status_methods
             ):
                 return
 
+            # Ignore events for objects that this controller doesn't manage
             vid = int(id_str)
             if vid not in self._items:
                 return
 
             # Pass the event to the controller
             self.handle_object_update(vid, method, args)
 
-        elif event["tag"] == EventType.RECONNECTED:
-            # Handle reconnect events
-
-            # Fetch the full state
+        elif event["type"] == EventType.RECONNECTED:
+            # Fetch the full state of all objects after reconnecting
             await self.fetch_full_state()
```

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.3.0/src/aiovantage/controllers/blind_groups.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from .base import BaseController
 
 
 class BlindGroupsController(BaseController[BlindGroup], BlindInterface):
     """Controller holding and managing Vantage blind groups."""
 
     # Fetch the following object types from Vantage
-    vantage_types = ("BlindGroup", "Somfy.URTSI_2_Group_CHILD")
+    vantage_types = (
+        "BlindGroup",
+        "Somfy.RS-485_Group_CHILD",
+        "Somfy.URTSI_2_Group_CHILD",
+    )
 
     def blinds(self, vid: int) -> QuerySet[Blind]:
         """Return a queryset of all blinds in this blind group."""
 
         blind_group = self[vid]
         if blind_group.blind_ids is not None:
             # Some blind groups have a list of blind ids, use that to filter
```

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/blinds.py` & `aiovantage-0.3.0/src/aiovantage/controllers/blinds.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,25 @@
 from .base import StatefulController
 
 
 class BlindsController(StatefulController[Blind], BlindInterface):
     """Controller holding and managing Vantage blinds."""
 
     # Fetch the following object types from Vantage
-    vantage_types = ("QISBlind", "QubeBlind", "RelayBlind", "Somfy.URTSI_2_Shade_CHILD")
-
-    # Subscribe to status updates from the event log for the following methods
-    event_log_status = True
-    event_log_status_methods = ("Blind.GetPosition",)
+    vantage_types = (
+        "QISBlind",
+        "QubeBlind",
+        "RelayBlind",
+        "Somfy.RS-485_Shade_CHILD",
+        "Somfy.URTSI_2_Shade_CHILD",
+    )
+
+    # Subscribe to status updates from the Enhanced Log for the following methods
+    enhanced_log_status = True
+    enhanced_log_status_methods = ("Blind.GetPosition",)
 
     @override
     async def fetch_object_state(self, vid: int) -> None:
         """Fetch the initial state of a blind."""
 
         state: Dict[str, Any] = {
             "position": await BlindInterface.get_position(self, vid)
```

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/buttons.py` & `aiovantage-0.3.0/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.3.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/gmem.py` & `aiovantage-0.3.0/src/aiovantage/controllers/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/load_groups.py` & `aiovantage-0.3.0/src/aiovantage/controllers/load_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/loads.py` & `aiovantage-0.3.0/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.3.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 class OmniSensorsController(StatefulController[OmniSensor]):
     """Controller holding and managing Vantage omni sensors."""
 
     # Fetch the following object types from Vantage
     vantage_types = ("OmniSensor",)
 
-    # Subscribe to status updates from the event log
-    event_log_status = True
+    # Subscribe to status updates from the Enhanced Log
+    enhanced_log_status = True
 
     @override
     async def fetch_object_state(self, vid: int) -> None:
         """Fetch the initial state of an omni sensor."""
 
         state: Dict[str, Any] = {
             "level": await self.get_level(vid),
```

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.3.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     ColorTemperatureInterface,
 ):
     """Controller holding and managing Vantage RGB loads."""
 
     # Fetch the following object types from Vantage
     vantage_types = ("Vantage.DGColorLoad", "Vantage.DDGColorLoad")
 
-    # Subscribe to status updates from the event log for the following methods
-    event_log_status = True
-    event_log_status_methods = (
+    # Subscribe to status updates from the Enhanced Log for the following methods
+    enhanced_log_status = True
+    enhanced_log_status_methods = (
         "RGBLoad.GetHSL",
         "RGBLoad.GetRGB",
         "RGBLoad.GetRGBW",
         "ColorTemperature.Get",
         "Load.GetLevel",
     )
```

### Comparing `aiovantage-0.2.3/src/aiovantage/controllers/tasks.py` & `aiovantage-0.3.0/src/aiovantage/controllers/tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 class TasksController(StatefulController[Task], TaskInterface):
     """Controller holding and managing Vantage tasks."""
 
     # Fetch the following object types from Vantage
     vantage_types = ("Task",)
 
-    # Subscribe to status updates from the event log for the following methods
-    event_log_status = True
-    event_log_status_methods = ("Task.IsRunning", "Task.GetState")
+    # Subscribe to status updates from the Enhanced Log for the following methods
+    enhanced_log_status = True
+    enhanced_log_status_methods = ("Task.IsRunning", "Task.GetState")
 
     @override
     async def fetch_object_state(self, vid: int) -> None:
         """Fetch the initial state of a task."""
 
         state: Dict[str, Any] = {
             "is_running": await TaskInterface.is_running(self, vid),
```

### Comparing `aiovantage-0.2.3/LICENSE` & `aiovantage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.2.3/README.md` & `aiovantage-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 - Alternatively, eager-fetch objects with `controller.initialize`.
 
 
 ## Supported objects types
 
 The following interfaces/controllers are currently supported.
 
-| Type          | Description           | Controller                | Examples                          |
-| ------------- | --------------------- | ------------------------- | --------------------------------- |
-| Area          | Rooms, etc            | `vantage.areas`           | [Examples](examples/areas)        |
-| Blind         | Shades, blinds        | `vantage.blinds`          | [Examples](examples/blinds)       |
-| BlindGroups   | Groups of blinds      | `vantage.blind_groups`    | [Examples](examples/blind_groups) |
-| Buttons       | Keypad buttons        | `vantage.buttons`         | [Examples](examples/buttons)      |
-| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`    | [Examples](examples/dry_contacts) |
-| GMem          | Vantage variables     | `vantage.gmem`            | [Examples](examples/gmem)         |
-| Load          | Lights, relays, etc   | `vantage.loads`           | [Examples](examples/loads)        |
-| LoadGroup     | Groups of loads       | `vantage.load_groups`     | [Examples](examples/load_groups)  |
-| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`    | [Examples](examples/omni_sensors) |
-| RGBLoad       | RGB lights            | `vantage.rgb_loads`       | [Examples](examples/rgb_loads)    |
-| Stations      | Keypads, etc          | `vantage.stations`        | [Examples](examples/stations)     |
-| Tasks         | Vantage tasks         | `vantage.tasks`           | [Examples](examples/tasks)        |
+| Type          | Description           | Controller                    | Examples                                  |
+| ------------- | --------------------- | ----------------------------- | ----------------------------------------- |
+| AnemoSensor   | Wind speed sensors    | `vantage.anemo_sensors`       | [Examples](examples/anemo_sensors)        |
+| Area          | Rooms, etc            | `vantage.areas`               | [Examples](examples/areas)                |
+| Blind         | Shades, blinds        | `vantage.blinds`              | [Examples](examples/blinds)               |
+| BlindGroups   | Groups of blinds      | `vantage.blind_groups`        | [Examples](examples/blind_groups)         |
+| Buttons       | Keypad buttons        | `vantage.buttons`             | [Examples](examples/buttons)              |
+| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`        | [Examples](examples/dry_contacts)         |
+| GMem          | Vantage variables     | `vantage.gmem`                | [Examples](examples/gmem)                 |
+| LightSensor   | Light sensors         | `vantage.light_sensors`       | [Examples](examples/light_sensors)        |
+| Load          | Lights, relays, etc   | `vantage.loads`               | [Examples](examples/loads)                |
+| LoadGroup     | Groups of loads       | `vantage.load_groups`         | [Examples](examples/load_groups)          |
+| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`        | [Examples](examples/omni_sensors)         |
+| RGBLoad       | RGB lights            | `vantage.rgb_loads`           | [Examples](examples/rgb_loads)            |
+| Stations      | Keypads, etc          | `vantage.stations`            | [Examples](examples/stations)             |
+| Tasks         | Vantage tasks         | `vantage.tasks`               | [Examples](examples/tasks)                |
+| Temperature   | Temperature sensors   | `vantage.temperature_sensors` | [Examples](examples/temperature_sensors)  |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
 
 
 ## Installation
 
 ```shell
```

### Comparing `aiovantage-0.2.3/pyproject.toml` & `aiovantage-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 Documentation = "https://github.com/loopj/aiovantage#readme"
 Issues = "https://github.com/loopj/aiovantage/issues"
 Source = "https://github.com/loopj/aiovantage"
 
 [tool.hatch.version]
 path = "src/aiovantage/__about__.py"
 
+[[tool.hatch.envs.all.matrix]]
+python = ["3.8", "3.9", "3.10", "3.11"]
+
 [tool.hatch.envs.lint]
 dependencies = [
   "black==23.3.0",
   "mypy==1.4.0",
   "ruff==0.0.272",
 ]
 
@@ -61,20 +64,23 @@
 [tool.black]
 target-version = ["py38"]
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py38"
 select = [
-    "E",  # pycodestyle errors
-    "W",  # pycodestyle warnings
-    "F",  # pyflakes
-    "I",  # isort
-    "C",  # flake8-comprehensions
-    "B",  # flake8-bugbear
+    "E",    # pycodestyle errors
+    "W",    # pycodestyle warnings
+    "F",    # pyflakes
+    "I",    # isort
+    "C",    # flake8-comprehensions
+    "B",    # flake8-bugbear
+    "Q",    # flake8-quotes
+    "UP",   # pyupgrade
+    "C90",  # mccabe
 ]
 ignore = [
     "E501",  # line too long, handled by black
 ]
 
 [tool.ruff.isort]
 known-first-party = ["aiovantage"]
```

### Comparing `aiovantage-0.2.3/PKG-INFO` & `aiovantage-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.2.3
+Version: 0.3.0
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -48,28 +48,31 @@
 - Alternatively, eager-fetch objects with `controller.initialize`.
 
 
 ## Supported objects types
 
 The following interfaces/controllers are currently supported.
 
-| Type          | Description           | Controller                | Examples                          |
-| ------------- | --------------------- | ------------------------- | --------------------------------- |
-| Area          | Rooms, etc            | `vantage.areas`           | [Examples](examples/areas)        |
-| Blind         | Shades, blinds        | `vantage.blinds`          | [Examples](examples/blinds)       |
-| BlindGroups   | Groups of blinds      | `vantage.blind_groups`    | [Examples](examples/blind_groups) |
-| Buttons       | Keypad buttons        | `vantage.buttons`         | [Examples](examples/buttons)      |
-| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`    | [Examples](examples/dry_contacts) |
-| GMem          | Vantage variables     | `vantage.gmem`            | [Examples](examples/gmem)         |
-| Load          | Lights, relays, etc   | `vantage.loads`           | [Examples](examples/loads)        |
-| LoadGroup     | Groups of loads       | `vantage.load_groups`     | [Examples](examples/load_groups)  |
-| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`    | [Examples](examples/omni_sensors) |
-| RGBLoad       | RGB lights            | `vantage.rgb_loads`       | [Examples](examples/rgb_loads)    |
-| Stations      | Keypads, etc          | `vantage.stations`        | [Examples](examples/stations)     |
-| Tasks         | Vantage tasks         | `vantage.tasks`           | [Examples](examples/tasks)        |
+| Type          | Description           | Controller                    | Examples                                  |
+| ------------- | --------------------- | ----------------------------- | ----------------------------------------- |
+| AnemoSensor   | Wind speed sensors    | `vantage.anemo_sensors`       | [Examples](examples/anemo_sensors)        |
+| Area          | Rooms, etc            | `vantage.areas`               | [Examples](examples/areas)                |
+| Blind         | Shades, blinds        | `vantage.blinds`              | [Examples](examples/blinds)               |
+| BlindGroups   | Groups of blinds      | `vantage.blind_groups`        | [Examples](examples/blind_groups)         |
+| Buttons       | Keypad buttons        | `vantage.buttons`             | [Examples](examples/buttons)              |
+| DryContacts   | Motion sensors, etc   | `vantage.dry_contacts`        | [Examples](examples/dry_contacts)         |
+| GMem          | Vantage variables     | `vantage.gmem`                | [Examples](examples/gmem)                 |
+| LightSensor   | Light sensors         | `vantage.light_sensors`       | [Examples](examples/light_sensors)        |
+| Load          | Lights, relays, etc   | `vantage.loads`               | [Examples](examples/loads)                |
+| LoadGroup     | Groups of loads       | `vantage.load_groups`         | [Examples](examples/load_groups)          |
+| OmniSensor    | Power, current, etc   | `vantage.omni_sensors`        | [Examples](examples/omni_sensors)         |
+| RGBLoad       | RGB lights            | `vantage.rgb_loads`           | [Examples](examples/rgb_loads)            |
+| Stations      | Keypads, etc          | `vantage.stations`            | [Examples](examples/stations)             |
+| Tasks         | Vantage tasks         | `vantage.tasks`               | [Examples](examples/tasks)                |
+| Temperature   | Temperature sensors   | `vantage.temperature_sensors` | [Examples](examples/temperature_sensors)  |
 
 If you have an object that you expect to show up in one of these controllers, but it is missing, please let me know in an issue.
 
 
 ## Installation
 
 ```shell
```

