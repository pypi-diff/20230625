# Comparing `tmp/networklab-1.5.4.tar.gz` & `tmp/networklab-1.5.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.4.tar", last modified: Sat Jun 10 16:47:15 2023, max compression
+gzip compressed data, was "networklab-1.5.4.post1.tar", last modified: Sun Jun 25 16:16:30 2023, max compression
```

## Comparing `networklab-1.5.4.tar` & `networklab-1.5.4.post1.tar`

### file list

```diff
@@ -1,621 +1,624 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-10 16:47:05.000000 networklab-1.5.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-10 16:47:05.000000 networklab-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 16:47:15.521443 networklab-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-10 16:47:05.000000 networklab-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.421442 networklab-1.5.4/netsim/
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/addressing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.425442 networklab-1.5.4/netsim/ansible/
--rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)     2714 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)     1269 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/create-config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 runner    (1001) docker     (123)     3424 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/initial-config.ansible
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/missing.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.425442 networklab-1.5.4/netsim/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/frr/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/frr/mpls-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/linux/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/nxos/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/tasks/vmx/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/templates/bfd/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/bgp/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/eigrp/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/evpn/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.445442 networklab-1.5.4/netsim/ansible/templates/initial/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.449442 networklab-1.5.4/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.449442 networklab-1.5.4/netsim/ansible/templates/isis/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.457442 networklab-1.5.4/netsim/ansible/templates/mpls/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.465443 networklab-1.5.4/netsim/ansible/templates/ospf/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.465443 networklab-1.5.4/netsim/ansible/templates/sr/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.465443 networklab-1.5.4/netsim/ansible/templates/srv6/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.469443 networklab-1.5.4/netsim/ansible/templates/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.477443 networklab-1.5.4/netsim/ansible/templates/vrf/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.477443 networklab-1.5.4/netsim/ansible/templates/vxlan/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.481443 networklab-1.5.4/netsim/augment/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    40808 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.481443 networklab-1.5.4/netsim/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9700 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/alias.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/clab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/down.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/empty.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/external_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/up.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/usage.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.485443 networklab-1.5.4/netsim/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/filemaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.485443 networklab-1.5.4/netsim/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/addressing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/attributes.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/automation.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/hints.yml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/multilab.yml
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/ports.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/arubacx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/asav.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/asav.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/csr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/eos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/eos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/fortios.yml
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/frr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/iosv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/iosv.yml
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/junos.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/none.yml
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/sros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/unknown.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vmx.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vmx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vsrx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vsrx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.417442 networklab-1.5.4/netsim/extra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/ebgp.utils/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/multilab/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/none/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/none/none.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/proxy-arp/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.497443 networklab-1.5.4/netsim/install/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/ansible.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/containerlab.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/grpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.497443 networklab-1.5.4/netsim/install/libvirt/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.497443 networklab-1.5.4/netsim/install/libvirt/asav/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/asav.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/csr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/eos.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/iosv.xml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.501443 networklab-1.5.4/netsim/install/libvirt/vptx/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.501443 networklab-1.5.4/netsim/install/libvirt/vsrx/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3185 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.505443 networklab-1.5.4/netsim/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    23624 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/_dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bfd.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bfd.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bgp.yml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/eigrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/eigrp.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/evpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/evpn.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/gateway.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/isis.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/isis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/mpls.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/mpls.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/ospf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/ospf.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/sr.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/sr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/srv6.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/srv6.yml
--rw-r--r--   0 runner    (1001) docker     (123)    58619 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vlan.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20435 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vrf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vxlan.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/d2.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/d2.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/graph.yml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/clab.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/external.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/virtualbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/virtualbox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/read_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.421442 networklab-1.5.4/netsim/templates/provider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/clab/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/clab/frr/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/clab/linux/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/templates/provider/libvirt/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/templates/provider/virtualbox/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/tests/clab.yml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/graphite.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/tools/suzieq/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/suzieq.yml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/topology-defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/netsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/networklab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-10 16:47:06.000000 networklab-1.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:47:15.521443 networklab-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-10 16:47:06.000000 networklab-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-06-10 16:47:06.000000 networklab-1.5.4/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.365451 networklab-1.5.4.post1/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/addressing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.365451 networklab-1.5.4.post1/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2899 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1269 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3460 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/missing.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.369451 networklab-1.5.4.post1/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/frr/mpls-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.373452 networklab-1.5.4.post1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.377452 networklab-1.5.4.post1/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.377452 networklab-1.5.4.post1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.381452 networklab-1.5.4.post1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.389452 networklab-1.5.4.post1/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.389452 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.389452 networklab-1.5.4.post1/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.393452 networklab-1.5.4.post1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.397452 networklab-1.5.4.post1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.401452 networklab-1.5.4.post1/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.401452 networklab-1.5.4.post1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.401452 networklab-1.5.4.post1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.405452 networklab-1.5.4.post1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.409452 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.409452 networklab-1.5.4.post1/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40803 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.413452 networklab-1.5.4.post1/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9700 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/clab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.413452 networklab-1.5.4.post1/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.413452 networklab-1.5.4.post1/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.357451 networklab-1.5.4.post1/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.417452 networklab-1.5.4.post1/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.421453 networklab-1.5.4.post1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3185 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.425453 networklab-1.5.4.post1/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    23624 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    58909 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22607 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/providers/virtualbox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/read_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.361451 networklab-1.5.4.post1/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.429453 networklab-1.5.4.post1/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.433453 networklab-1.5.4.post1/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/netsim/utils/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 16:16:30.000000 networklab-1.5.4.post1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 16:16:30.437453 networklab-1.5.4.post1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-06-25 16:16:20.000000 networklab-1.5.4.post1/tests/test_transformation.py
```

### Comparing `networklab-1.5.4/LICENSE.md` & `networklab-1.5.4.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/PKG-INFO` & `networklab-1.5.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.4
+Version: 1.5.4.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.5.4/README.md` & `networklab-1.5.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/addressing.py` & `networklab-1.5.4.post1/netsim/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/collect-configs.ansible` & `networklab-1.5.4.post1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/config.ansible` & `networklab-1.5.4.post1/netsim/ansible/config.ansible`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env ansible-playbook
 #
 ---
 - name: Deploy device configuration
   hosts: all:!unprovisioned
   gather_facts: false
+  vars:
+    node_provider: "{{ provider|default(netlab_provider) }}"
   tasks:
   - block:
     - set_fact:
         netlab_device_type: "{{ netlab_device_type|default(ansible_network_os) }}"
 
     - fail: msg="Specify configuration template name with an external variable"
       when: config is not defined
@@ -17,20 +19,20 @@
         config_template: "{{ lookup('first_found',params,errors='ignore') }}"
       vars:
         params:
           paths:
           - "{{ lookup('env','PWD') }}"
           - "."
           files:
-          - "{{ config + '/' + inventory_hostname + '.' + netlab_device_type + '-' + netlab_provider + '.j2' }}"
+          - "{{ config + '/' + inventory_hostname + '.' + netlab_device_type + '-' + node_provider + '.j2' }}"
           - "{{ config + '/' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
           - "{{ config + '/' + inventory_hostname + '.j2' }}"
-          - "{{ config + '/' + netlab_device_type + '-' + netlab_provider + '.j2' }}"
+          - "{{ config + '/' + netlab_device_type + '-' + node_provider + '.j2' }}"
           - "{{ config + '/' + netlab_device_type + '.j2' }}"
-          - "{{ config + '/' + ansible_network_os + '-' + netlab_provider + '.j2' }}"
+          - "{{ config + '/' + ansible_network_os + '-' + node_provider + '.j2' }}"
           - "{{ config + '/' + ansible_network_os + '.j2' }}"
           - "{{ config + '.' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
           - "{{ config + '.' + inventory_hostname + '.' + ansible_network_os + '.j2' }}"
           - "{{ config + '.' + inventory_hostname + '.j2' }}"
           - "{{ config + '.' + netlab_device_type + '.j2' }}"
           - "{{ config + '.' + ansible_network_os + '.j2' }}"
           - "{{ config }}"
@@ -48,15 +50,20 @@
         verbosity: 1
 
     tags: [ always ]
 
   - include_tasks: "{{ item }}"
     with_first_found:
     - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy-{{ inventory_hostname }}.yml"
-    - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ netlab_provider }}.yml"
+    - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ node_provider }}.yml"
     - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}.yml"
-    - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ netlab_provider }}.yml"
+    - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ node_provider }}.yml"
     - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}.yml"
     - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.yml"
-    - "tasks/deploy-config/{{netlab_device_type}}-{{netlab_provider}}.yml"
+    - "tasks/deploy-config/{{netlab_device_type}}-{{node_provider}}.yml"
     - "tasks/deploy-config/{{netlab_device_type}}.yml"
     - "tasks/deploy-config/{{ansible_network_os}}.yml"
+    args:
+      apply:
+        vars:
+          netsim_action: "{{ config }}"
+          config_template: "{{ config_template }}"
```

### Comparing `networklab-1.5.4/netsim/ansible/create-config.ansible` & `networklab-1.5.4.post1/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/initial-config.ansible` & `networklab-1.5.4.post1/netsim/ansible/initial-config.ansible`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     - set_fact:
         ready_script: "{{ lookup('first_found',params,errors='ignore') }}"
       vars:
         params:
           paths:
           - "tasks/readiness-check"
           files:
-          - "{{netlab_device_type}}-{{netlab_provider}}.yml"
+          - "{{netlab_device_type}}-{{provider|default(netlab_provider)}}.yml"
           - "{{netlab_device_type}}.yml"
-          - "{{ansible_network_os}}-{{netlab_provider}}.yml"
+          - "{{ansible_network_os}}-{{provider|default(netlab_provider)}}.yml"
           - "{{ansible_network_os}}.yml"
 
     - name: Waiting for device to become ready
       include_tasks: "{{ ready_script }}"
       when: ready_script|default('')
       args:
         apply:
```

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files 19% similar despite different names*

```diff
@@ -3,11 +3,13 @@
     dest: /tmp/config.sh
 
 - set_fact: deployed_config={{ lookup('template',config_template) }}
 
 - name: "run /tmp/config.sh to deploy {{netsim_action}} config from {{ config_template }}"
   command: bash /tmp/config.sh
   when: not ansible_check_mode and ("#!/bin/bash" in deployed_config)
+  become: true
 
 - name: "run vtysh to import {{netsim_action}} config from {{ config_template }}"
   command: vtysh -f /tmp/config.sh
   when: not ansible_check_mode and not ("#!/bin/bash" in deployed_config)
+  become: true
```

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #
 # Deploy module-specific configuration (specified in "item") to a device
 #
 - set_fact:
     config_template: "{{ lookup('first_found',params,errors='ignore') }}"
   tags: [ always ]
   vars:
+    node_provider: "{{ provider|default(netlab_provider) }}"
     params:
       paths:
       - "{{ lookup('env','PWD') }}"
       - "../../extra"
       files:
-      - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '-' + netlab_provider + '.j2' }}"
+      - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '-' + node_provider + '.j2' }}"
       - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
       - "{{ custom_config + '/' + inventory_hostname + '.j2' }}"
-      - "{{ custom_config + '/' + netlab_device_type + '-' + netlab_provider + '.j2' }}"
+      - "{{ custom_config + '/' + netlab_device_type + '-' + node_provider + '.j2' }}"
       - "{{ custom_config + '/' + netlab_device_type + '.j2' }}"
-      - "{{ custom_config + '/' + ansible_network_os + '-' + netlab_provider + '.j2' }}"
+      - "{{ custom_config + '/' + ansible_network_os + '-' + node_provider + '.j2' }}"
       - "{{ custom_config + '/' + ansible_network_os + '.j2' }}"
       - "{{ custom_config + '.' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
       - "{{ custom_config + '.' + inventory_hostname + '.' + ansible_network_os + '.j2' }}"
       - "{{ custom_config + '.' + inventory_hostname + '.j2' }}"
       - "{{ custom_config + '.' + netlab_device_type + '.j2' }}"
       - "{{ custom_config + '.' + ansible_network_os + '.j2' }}"
       - "{{ custom_config }}"
@@ -36,28 +37,30 @@
       =========================================
       {{ lookup('template',config_template) }}
     verbosity: 1
   tags: [ test,custom ]
 
 - include_tasks: "{{ item }}"
   tags: [ custom ]
+  vars:
+    node_provider: "{{ provider|default(netlab_provider) }}"
   with_first_found:
   - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy-{{ inventory_hostname }}.yml"
-  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ netlab_provider }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ node_provider }}.yml"
   - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}.yml"
-  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ netlab_provider }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ node_provider }}.yml"
   - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}.yml"
   - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.yml"
-  - "../../extra/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ netlab_provider }}.yml"
+  - "../../extra/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ node_provider }}.yml"
   - "../../extra/{{ custom_config }}/deploy.{{ netlab_device_type }}.yml"
-  - "deploy-config/{{netlab_device_type}}-{{ netlab_provider }}.yml"
+  - "deploy-config/{{netlab_device_type}}-{{ node_provider }}.yml"
   - "deploy-config/{{netlab_device_type}}.yml"
-  - "../../extra/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ netlab_provider }}.yml"
+  - "../../extra/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ node_provider }}.yml"
   - "../../extra/{{ custom_config }}/deploy.{{ ansible_network_os }}.yml"
-  - "deploy-config/{{ansible_network_os}}-{{ netlab_provider }}.yml"
+  - "deploy-config/{{ansible_network_os}}-{{ node_provider }}.yml"
   - "deploy-config/{{ansible_network_os}}.yml"
   - "../missing.yml"
   args:
     apply:
       vars:
         netsim_action: "{{ custom_config }}"
       tags: [ always ]
```

### Comparing `networklab-1.5.4/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/deploy-module.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,35 +19,35 @@
 - block:
   - set_fact:
       config_template: "{{ lookup('first_found',params,errors='ignore') }}"
     vars:
       params:
         paths: "{{ paths }}"
         files:
-        - "{{ config_module }}/{{netlab_device_type}}-{{netlab_provider}}.j2"
+        - "{{ config_module }}/{{netlab_device_type}}-{{provider|default(netlab_provider)}}.j2"
         - "{{ config_module }}/{{netlab_device_type}}.j2"
-        - "{{ config_module }}/{{ansible_network_os}}-{{netlab_provider}}.j2"
+        - "{{ config_module }}/{{ansible_network_os}}-{{provider|default(netlab_provider)}}.j2"
         - "{{ config_module }}/{{ansible_network_os}}.j2"
 
   - debug:
       msg: |
         {{ config_module }} configuration for {{ inventory_hostname }}
         =========================================
         {{ lookup('template',config_template or paths[0]+'/missing.j2') }}
       verbosity: 1  
   
   - include_tasks: "{{ item }}"
     with_first_found:
-    - "{{netlab_device_type}}/{{ config_module }}-{{ netlab_provider }}.yml"
+    - "{{netlab_device_type}}/{{ config_module }}-{{ provider|default(netlab_provider) }}.yml"
     - "{{netlab_device_type}}/{{ config_module }}.yml"
-    - "deploy-config/{{netlab_device_type}}-{{ netlab_provider }}.yml"
+    - "deploy-config/{{netlab_device_type}}-{{ provider|default(netlab_provider) }}.yml"
     - "deploy-config/{{netlab_device_type}}.yml"
-    - "{{ansible_network_os}}/{{ config_module }}-{{ netlab_provider }}.yml"
+    - "{{ansible_network_os}}/{{ config_module }}-{{ provider|default(netlab_provider) }}.yml"
     - "{{ansible_network_os}}/{{ config_module }}.yml"
-    - "deploy-config/{{ansible_network_os}}-{{ netlab_provider }}.yml"
+    - "deploy-config/{{ansible_network_os}}-{{ provider|default(netlab_provider) }}.yml"
     - "deploy-config/{{ansible_network_os}}.yml"
     - "../missing.yml"
     args:
       apply:
         vars:
           config_template: "{{ config_template }}"
           netsim_action: "{{ config_module }}"
```

### Comparing `networklab-1.5.4/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -3,11 +3,13 @@
     dest: /tmp/config.sh
 
 - set_fact: deployed_config={{ lookup('template',config_template) }}
 
 - name: "run /tmp/config.sh to deploy {{netsim_action}} config from {{ config_template }}"
   command: bash /tmp/config.sh
   when: not ansible_check_mode and ("#!/bin/bash" in deployed_config)
+  become: true
 
 - name: "run vtysh to import {{netsim_action}} config from {{ config_template }}"
   command: vtysh -f /tmp/config.sh
   when: not ansible_check_mode and not ("#!/bin/bash" in deployed_config)
+  become: true
```

### Comparing `networklab-1.5.4/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.5.4.post1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files 2% similar despite different names*

```diff
@@ -138,21 +138,23 @@
    export-policy: accept_all
    peer-as: {{ neighbor.as }}
    transport:
     local-address: {{ transport_ip }}
 {%  if vrf_bgp.rr|default(0) %}
     passive-mode: True
     _annotate_passive-mode: "Improve robustness during startup"
-   route-reflector:
-    cluster-id: {{ vrf_bgp.rr_cluster_id|default(False) or router_id }}
-    client: True
 {%  else %}
    next-hop-self: {{ vrf_bgp.next_hop_self|default(False) }}
 {%  endif %}
 {% endif %}
+{% if vrf_bgp.rr|default(0) %}
+   route-reflector:
+    cluster-id: {{ vrf_bgp.rr_cluster_id|default(False) or router_id }}
+    client: True
+{% endif %}
 {% endmacro %}
 
 {#
   Define IPv4 and IPv6 BGP neighbors
 #}
 {% for n in vrf_bgp.neighbors %}
 {% for af in ['ipv4','ipv6'] if n[af] is defined %}
```

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   exit-vni
 {% endfor %}
 
 {% for n in bgp.neighbors if n.evpn|default(False) %}
 {%  for af in ['ipv4','ipv6'] if af in n %}
 {%   set peer = n[af] if n[af] is string else n.local_if|default('?') %}
   neighbor {{ peer }} activate
+  neighbor {{ peer }} soft-reconfiguration inbound
 {%   if bgp.rr|default('') and not n.rr|default('') %}
   neighbor {{ peer }} route-reflector-client
 {%   endif %}
 {%  endfor %}
 {% endfor %}
 
  exit-address-family
```

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 
 updates:
 {% for type in evpn.session %}
 - path: network-instance[name=default]/protocols/bgp
   val:
    group:
    - group-name: {{ 'ibgp-ipv4' if type=='ibgp' else 'ebgp' }} # Could create a dedicated group for EVPN only?
+{%  if type=='ebgp' %}
+     export-policy: "accept_all"
+{%  endif %}
      afi-safi:
      - afi-safi-name: evpn
        admin-state: enable
-{% if bgp.rr|default(0) %}
+{%  if bgp.rr|default(0) %}
      next-hop-self: False
-{% endif %}
+{%  endif %}
    route-advertisement:
     rapid-withdrawal: True
    afi-safi:
    - afi-safi-name: evpn
      evpn:
       rapid-update: True
 {% endfor %}
```

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/asa.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/frr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/vyos.j2`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,97 @@
-#!/bin/bash
-#
-set -e
-#
-# Create bash profile script
-#
-cat <<SCRIPT >/root/.bash_profile
-#!/bin/bash
-#
-export PS1="\h(bash)#"
-echo "Use vtysh to connect to FRR daemon"
-echo
-SCRIPT
-#
-# Build hosts file
-#
-{% for k,v in hostvars.items() if k != inventory_hostname and v.af.ipv4|default(False) %}
-echo "{%- if v.loopback.ipv4 is defined %}{{ v.loopback.ipv4|ipaddr('address') }} {% endif %}
-{%- for l in v.interfaces|default([]) if 'ipv4' in l and l.ipv4 != True and l.ipv4|ipv4 %}{{ l.ipv4|ipaddr('address') }} {% endfor %}{{ k }}" >>/tmp/hosts
-{% endfor %}
-sort /tmp/hosts|uniq >>/etc/hosts
+#!/bin/vbash
+source /opt/vyatta/etc/functions/script-template
 
-#
-# Enable FRR modules (if not using containerlab bind-mounted /etc/frr/daemons)
-#
-{% if clab is not defined or clab.binds|default({})=={} %}
-{% set modlist = {'bgp':'bgpd','ospf':['ospfd','ospf6d'],'isis':'isisd','vrf':'bgpd','mpls':'ldpd'} %}
-{% for m in module|default([]) if modlist[m] is defined %}
-{%   for frr_m in [modlist[m]]|flatten %}
-echo "{{ frr_m }}=yes" >>/etc/frr/daemons
-{%   endfor %}
-{% endfor %}
+if [ "$(id -g -n)" != 'vyattacfg' ] ; then
+    exec sg vyattacfg -c "/bin/vbash $(readlink -f $0) $@"
+fi
+
+# Configuration items start here
 
-/usr/lib/frr/frrinit.sh restart
+configure
+{#
+It seems VyOS has some problems in handling hostnames with only one letter in it.
+#}
+{% if inventory_hostname|length > 1 %}
+set system host-name '{{ inventory_hostname }}'
+{% else %}
+set system host-name 'vyos-{{ inventory_hostname }}'
 {% endif %}
 
-#
-# Create loopbacks and stub devices
-#
-{% for i in (interfaces+[{ 'type': 'loopback', 'ifname': 'lo0'}]) if i.type in ['loopback','stub'] %}
-if [ ! -e /sys/devices/virtual/net/{{ i.ifname }} ]; then
-  ip link add {{ i.ifname }} type dummy
-  ip link set dev {{ i.ifname }} up
-fi
-{% endfor %}
+{% if vrfs is defined %}
+{% include 'vyos.vrf.j2' %}
+{% endif %}
+{% if vlans is defined %}
+{% include 'vyos.vlan.j2' %}
+{% endif %}
 
-#
-# Add vtysh.conf file
-echo "service integrated-vtysh-config" >/etc/frr/vtysh.conf
-#
-# Set Ethernet interface MTU
-{% for l in interfaces|default([]) if l.mtu is defined %}
-ip link set {{ l.ifname }} mtu {{ l.mtu }}
-{% endfor %}
-#
-# Rest of initial configuration done through VTYSH
-#
-cat >/tmp/config <<CONFIG
-hostname {{ inventory_hostname }}
-!
-{% if 'ipv6' in af %}
-ipv6 forwarding
-{% endif %}
-!
-{% if loopback is defined %}
-interface lo0
- no shutdown
-{%  if loopback.ipv4 is defined %}
- ip address {{ loopback.ipv4 }}
-{%  endif %}
-{%  if loopback.ipv6 is defined %}
- ipv6 address {{ loopback.ipv6 }}
-{%  endif %}
-!
+{% if 'ipv4' in loopback %}
+set interfaces dummy dum0 address {{ loopback.ipv4 }}
 {% endif %}
+{% if 'ipv6' in loopback %}
+set interfaces dummy dum0 address {{ loopback.ipv6 }}
+{% endif %}
+
 {% for l in interfaces|default([]) %}
-interface {{ l.ifname }}
-! no shutdown
+
+{#
+# - Define interface hierarchy/tree level (i.e. ethernet, bridge, ...)
+# - Set proper interface name to be used below
+# While right now the ifname, when a bridge, is always brX.Y,
+#  this code is ready for future "plain" bridges (i.e., br1)
+#}
+{%   set ns = namespace(iface_level="ethernet", ifname=l.ifname) %}
+{%   if l.ifname.startswith('br') %}
+{%     set ns.iface_level = "bridge" %}
+{%   elif l.ifname.startswith('dum') %}
+{%     set ns.iface_level = "dummy" %}
+{%   endif %}
+{#
+# Split interface name with vif, if needed
+#}
+{%   set ifnamedata = l.ifname.split('.') %}
+{%   if ifnamedata|length > 1 %}
+{%     set ns.ifname = ifnamedata[0] + ' vif ' + ifnamedata[1] %}
+{%   endif %}
+
 {% if l.name is defined %}
- description {{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} description '{{ l.name }}{{ " ["+l.role+"]" if l.role is defined else "" }}'
 {% elif l.type|default("") == "stub" %}
- description Stub interface
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} description 'Stub interface'
 {% endif %}
-{% if l.ipv4 is defined and (l.ipv4 is string or loopback.ipv4 is defined) %}
- ip address {{ l.ipv4 if l.ipv4 is string else loopback.ipv4 }}
-{% else %}
- ! no ip address
+
+{% if l.mtu is defined %}
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} mtu {{ l.mtu }}
 {% endif %}
-{% if l.ipv6 is defined %}
-{%  if l.ipv6 is string and l.ipv6|ipv6 %}
- ipv6 address {{ l.ipv6 }}
-{%  endif %}
- ipv6 nd ra-interval 5
- no ipv6 nd suppress-ra
-{% else %}
- ! Note, currently does not take for OS configured interfaces; known issue
- ipv6 nd suppress-ra
+
+{% if 'ipv4' in l %}
+{%   if l.ipv4 == True and 'ipv4' in loopback %}
+# Need to set the same address as loopback (dum0) to make it behave as unnumbered
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} address {{ loopback.ipv4 }}
+{%   elif l.ipv4|ipv4 %}
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} address {{ l.ipv4 }}
+{%   endif %}
 {% endif %}
-{% if l.bandwidth is defined %}
- bandwidth {{ l.bandwidth  }}
+
+{% if 'ipv6' in l %}
+{%   if l.ipv6 == True %}
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} ipv6
+{%   elif l.ipv6|ipv6 %}
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} address {{ l.ipv6 }};
+{%   endif %}
 {% endif %}
-!
-{% endfor %}
-do write
-CONFIG
-vtysh -f /tmp/config
-
-# Workaround for FRR issue with disabling ipv6 (https://github.com/FRRouting/frr/issues/7738)
-{% for l in interfaces if l.type in ['lan','p2p','stub'] and l.ipv6 is not defined %}
-sysctl -qw net.ipv6.conf.{{ l.ifname }}.disable_ipv6=1
+
+{% if l.vrf is defined %}
+set interfaces {{ ns.iface_level }} {{ ns.ifname }} vrf {{ l.vrf }}
+{% endif %}
+
 {% endfor %}
 
-exit 0
+set service lldp interface all
+set service lldp interface {{ mgmt.ifname|default('eth0') }} disable
+
+# Commit, save and exit from subshell
+
+commit
+save
+exit
+
```

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/ios.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/junos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files 16% similar despite different names*

```diff
@@ -28,31 +28,55 @@
 SCRIPT
 
 systemctl restart systemd-resolved
 
 # Set persistent hostname
 hostnamectl set-hostname {{ inventory_hostname }}
 
+NEED_APT_UPDATE=YES
+{% if netlab_net_tools|default(False) %}
+#
+# Install net-tools (arp, route...)
+#
+if which arp; then
+  echo "net-tools already installed"
+else
+  apt-get update -qq
+  apt-get install -qq net-tools
+  NEED_APT_UPDATE=
+fi
+{% endif %}
+{% if netlab_lldp_enable|default(False) %}
 #
 # Enable LLDP
 #
-apt-get update -qq
-apt-get install -qq lldpd net-tools
+if systemctl is-active --quiet lldpd.service; then
+  echo "LLDP already installed"
+else
+  if "$NEED_APT_UPDATE"; then
+    apt-get update -qq
+  fi
+  apt-get install -qq lldpd
+fi
+
 cat <<CONFIG >/etc/lldpd.d/system.conf
 configure lldp tx-interval 30
 configure lldp tx-hold 3
 configure system interface pattern *,!eth0,eth*
 CONFIG
 systemctl enable lldpd
 systemctl restart lldpd
+{% endif %}
 
-# Sysctl
+# Sysctl settings: IPv4/IPv6 forwarding, IPv6 LLA
+#
+{% set pkt_fwd = "1" if role|default("host") == "router" else "0" %}
 cat <<SCRIPT > /etc/sysctl.d/10-netsim.conf
-net.ipv4.ip_forward=0
-net.ipv6.conf.all.forwarding=0
+net.ipv4.ip_forward={{ pkt_fwd }}
+net.ipv6.conf.all.forwarding={{ pkt_fwd }}
 
 {%   if loopback.ipv6 is defined %}
 net.ipv6.conf.lo.disable_ipv6=0
 {%   endif %}
 {% for l in interfaces|default([]) %}
 {%   if l.ipv6 is defined %}
 net.ipv6.conf.{{ l.ifname }}.disable_ipv6=0
```

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ### One-Shot configuration (non-Ubuntu VM or container)
 #
 # Disable IPv4 and IPv6 forwarding
 #
-sysctl -w net.ipv4.ip_forward=0
-sysctl -w net.ipv6.conf.all.forwarding=0
+{% set pkt_fwd = "1" if role|default("host") == "router" else "0" %}
+sysctl -w net.ipv4.ip_forward={{ pkt_fwd }}
+sysctl -w net.ipv6.conf.all.forwarding={{ pkt_fwd }}
 {% if loopback is defined %}
 #
 # Loopback addressing
 #
 {%   if 'ipv4' in loopback %}
 set +e
 ip addr del {{ loopback.ipv4 }} dev lo 2>/dev/null
```

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/asa.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/frr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/ios.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/junos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/sr/junos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/sr/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.5.4.post1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/api.py` & `networklab-1.5.4.post1/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/augment/components.py` & `networklab-1.5.4.post1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/augment/config.py` & `networklab-1.5.4.post1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/augment/devices.py` & `networklab-1.5.4.post1/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/augment/groups.py` & `networklab-1.5.4.post1/netsim/augment/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,29 +289,31 @@
       unique_keys: typing.List[str] = []) -> None:
 
   if not unique_keys:
     unique_keys = copy_keys
   for gname,gdata in topology.groups.items():
     #
     # Find groups with node_data dictionaries
+    # and check that the key within node_data dictionary we're interested in is also a dictionary
+    #
     if must_be_dict(gdata,f'node_data.{key}',f'groups.{gname}',module=module,create_empty=False):
-      for obj_name in list(gdata.node_data[key].keys()):
-        if gdata.node_data[key][obj_name] is None:
-          gdata.node_data[key][obj_name] = {}
-        obj_data =  gdata.node_data[key][obj_name]
+      for obj_name in list(gdata.node_data[key].keys()):              # Iterate over VLANs/VRFs within the group
+        if gdata.node_data[key][obj_name] is None:                    # ... replace None values with
+          gdata.node_data[key][obj_name] = {}                         # ... empty dictionaries
+        obj_data =  gdata.node_data[key][obj_name]                    # Now get the data to work with
         if not obj_name in topology[key] or topology[key][obj_name] is None:
-          topology[key][obj_name] = {}
-        for attr in unique_keys:
+          topology[key][obj_name] = {}                                # Make sure global object is also a dictionary
+        for attr in unique_keys:                                      # Check whether we have an overlap in unique keys
           if attr in topology[key][obj_name] and attr in obj_data and \
-             topology[key][obj_name][attr] != obj_data[attr]:                          # Unique key present on both ends and not equal
+             topology[key][obj_name][attr] != obj_data[attr]:         # Unique key present on both ends and not equal
             common.error(
               f'Cannot redefine {key} attribute {attr} for {key}.{obj_name} from node_data in group {gname}',
               common.IncorrectValue,
               module)
-        for attr in copy_keys:
+        for attr in copy_keys:                                        # Finally, copy missing values from group to global object
           if attr in obj_data and attr not in topology[key][obj_name]:
             topology[key][obj_name][attr] = obj_data[attr]
 
 #
 # create_bgp_autogroups -- create BGP AS groups
 #
```

### Comparing `networklab-1.5.4/netsim/augment/links.py` & `networklab-1.5.4.post1/netsim/augment/links.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,15 +891,15 @@
 Link index utility functions:
 
 * get_next_linkindex: get last linkindex+1 or default value
 * get_link_by_index: given a link index, return the link
 '''
 
 def get_next_linkindex(topology: Box) -> int:
-  if not 'links' in topology:
+  if not topology.links:
     topology.links = []
     return topology.defaults.get('link_index',1)
 
   return topology.links[-1].linkindex + 1
 
 def get_link_by_index(topology: Box, idx: int) -> typing.Optional[Box]:
   for link in topology.links:
```

### Comparing `networklab-1.5.4/netsim/augment/main.py` & `networklab-1.5.4.post1/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/augment/nodes.py` & `networklab-1.5.4.post1/netsim/augment/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
       data=n_data,                                    # Validate node data
       topology=topology,
       data_path=f'nodes.{n_name}',                    # Topology path to node name
       data_name=f'node',
       attr_list=['node'],                             # We're checking node attributes
       modules=n_data.get('module',[]),                # ... against node modules
       module='nodes',                                 # Function is called from 'nodes' module
+      ignored=['_','netlab_'],                        # Ignore attributes starting with _ or netlab_
       extra_attributes=extra)                         # Allow provider- and tool-specific settings
 
 def augment_mgmt_if(node: Box, defaults: Box, addrs: typing.Optional[Box]) -> None:
   if 'ifname' not in node.mgmt:
     mgmt_if = devices.get_device_attribute(node,'mgmt_if',defaults)
     if not mgmt_if:
       ifname_format = devices.get_device_attribute(node,'interface_name',defaults)
```

### Comparing `networklab-1.5.4/netsim/augment/plugin.py` & `networklab-1.5.4.post1/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/augment/topology.py` & `networklab-1.5.4.post1/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/callback.py` & `networklab-1.5.4.post1/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/__init__.py` & `networklab-1.5.4.post1/netsim/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/ansible.py` & `networklab-1.5.4.post1/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/clab.py` & `networklab-1.5.4.post1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/collect.py` & `networklab-1.5.4.post1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/config.py` & `networklab-1.5.4.post1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/connect.py` & `networklab-1.5.4.post1/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/create.py` & `networklab-1.5.4.post1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/down.py` & `networklab-1.5.4.post1/netsim/cli/down.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/external_commands.py` & `networklab-1.5.4.post1/netsim/cli/external_commands.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/initial.py` & `networklab-1.5.4.post1/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/install.py` & `networklab-1.5.4.post1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/libvirt.py` & `networklab-1.5.4.post1/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/read.py` & `networklab-1.5.4.post1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/restart.py` & `networklab-1.5.4.post1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/show.py` & `networklab-1.5.4.post1/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/status.py` & `networklab-1.5.4.post1/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/test.py` & `networklab-1.5.4.post1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/up.py` & `networklab-1.5.4.post1/netsim/cli/up.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/cli/usage.txt` & `networklab-1.5.4.post1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/common.py` & `networklab-1.5.4.post1/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/data/__init__.py` & `networklab-1.5.4.post1/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/data/filemaps.py` & `networklab-1.5.4.post1/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/data/global_vars.py` & `networklab-1.5.4.post1/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/data/types.py` & `networklab-1.5.4.post1/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/data/validate.py` & `networklab-1.5.4.post1/netsim/data/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,28 +308,32 @@
       data_path: str,                                   # Path to the data object (needed in error messages)
       data_name: str,                                   # Name of the object (needed in error messages, example: 'node')
       attr_list: typing.List[str],                      # List of valid attributes (example: ['node'] or ['link','interface'])
       modules: typing.Optional[list] = [],              # List of relevant modules
       module: str = 'attributes',                       # Module generating the error message (default: 'attributes')
       module_source: typing.Optional[str] = None,       # Where did we get the list of modules?
       attributes: typing.Optional[Box] = None,          # Where to get valid attributes from
-      extra_attributes: typing.Optional[Box] = None     # Dynamic attributes (needed to validate provider and tool settings)
+      extra_attributes: typing.Optional[Box] = None,    # Dynamic attributes (needed to validate provider and tool settings)
+      ignored: typing.Optional[list] = ['_']            # Ignored prefixes
         ) -> typing.Any: 
 
   #
   # Part 1: set up default values
   #
   global list_of_modules
 
   if attributes is None:
     attributes = topology.defaults.attributes
 
   if extra_attributes:
     attributes = attributes + extra_attributes
 
+  if not ignored:
+    ignored = ['_']
+
   if not isinstance(attributes,Box):
     common.fatal('Internal error in validate_attributes: attributes is not a Box')
     return None
 
   if not 'extra' in topology.defaults.attributes:
     build_module_extra_attributes(topology)
 
@@ -379,15 +383,15 @@
     common.error(
       f'Cannot validate attributes in {data_path} -- that should have been a dictionary, found {type(data).__name__}',
       common.IncorrectType,
       'validate')
     return
 
   for k in data.keys():
-    if k.startswith('_'):                               # Skip internal attributes
+    if any(k.startswith(i) for i in ignored):           # Skip internal attributes
       continue
 
     if k in valid:
       validate_item(
         parent=data,
         key=k,
         data_type=valid[k],
```

### Comparing `networklab-1.5.4/netsim/defaults/attributes.yml` & `networklab-1.5.4.post1/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/__init__.py` & `networklab-1.5.4.post1/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/arubacx.py` & `networklab-1.5.4.post1/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/arubacx.yml` & `networklab-1.5.4.post1/netsim/devices/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/asav.py` & `networklab-1.5.4.post1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/asav.yml` & `networklab-1.5.4.post1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/csr.yml` & `networklab-1.5.4.post1/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/cumulus.yml` & `networklab-1.5.4.post1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/cumulus_nvue.yml` & `networklab-1.5.4.post1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/dellos10.yml` & `networklab-1.5.4.post1/netsim/devices/dellos10.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/eos.py` & `networklab-1.5.4.post1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/eos.yml` & `networklab-1.5.4.post1/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/frr.yml` & `networklab-1.5.4.post1/netsim/devices/none.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,56 @@
-description: FRR container
+description: Dummy device used to test topology transformation
+#
+# Most features are enabled on the dummy device -- this file is a pretty
+# good template if you want to figure out what device features there are.
+#
 interface_name: eth{ifindex}
-mgmt_if: eth0
-loopback_interface_name: "lo{ifindex}"
-group_vars:
-  ansible_connection: docker
-  ansible_network_os: frr
-  ansible_python_interpreter: auto_silent
+loopback_interface_name: Loopback{ifindex}
+tunnel_interface_name: Tunnel{ifindex}
+virtualbox:
+  image: none
+libvirt:
+  image: none
 clab:
-  # image: frrouting/frr:v7.5.0
-  image: frrouting/frr:v8.4.0
-  mtu: 1500
-  node:
-    kind: linux
-    config_templates:
-      daemons: /etc/frr/daemons
+  image: none
 external:
   image: none
+group_vars:
+  ansible_connection: paramiko_ssh
+  ansible_network_os: none
 features:
+  bgp:
+    local_as: True
+    vrf_local_as: True
+    local_as_ibgp: True
+    activate_af: True
+    ipv6_lla: True
+    rfc8950: True
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
+  ospf:
+    unnumbered: True
+  isis:
+    unnumbered:
+      ipv4: True
+      ipv6: True
+      network: True
+  mpls:
+    ldp: True
+    bgp: True
+    vpn: True
+    6pe: True
+  evpn:
+    irb: True
+    asymmetrical_irb: True
+    bundle: [ vlan_aware ]
+  gateway:
+    protocol: [ anycast, vrrp ]
   vlan:
-    model: router
-    svi_interface_name: "vlan{vlan}"
+    model: l3-switch
+    svi_interface_name: Vlan{vlan}
     subif_name: "{ifname}.{vlan.access_id}"
     mixed_trunk: True
     native_routed: True
-  evpn:
-    irb: True
-  vrf:
-    keep_module: True # Don't remove vrf module even if no interfaces are associated with any vrfs
-  bgp:
-    activate_af: True
-    ipv6_lla: True
-    rfc8950: True
-    local_as: True
-    vrf_local_as: True
-  mpls:
-    ldp: True
-    vpn: True
-graphite.icon: router
```

### Comparing `networklab-1.5.4/netsim/devices/iosv.py` & `networklab-1.5.4.post1/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/iosv.yml` & `networklab-1.5.4.post1/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/iosxr.yml` & `networklab-1.5.4.post1/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/junos.py` & `networklab-1.5.4.post1/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/linux.yml` & `networklab-1.5.4.post1/netsim/devices/linux.yml`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 group_vars:
   ansible_network_os: linux
   ansible_connection: paramiko
   ansible_user: vagrant
   ansible_ssh_pass: vagrant
   docker_shell: sh -il
   ansible_python_interpreter: auto_silent
+  netlab_lldp_enable: True
+  netlab_net_tools: True
 clab:
   image: python:3.9-alpine
   mtu: 1500
   node:
     kind: linux
     config_templates:
       hosts: /etc/hosts
```

### Comparing `networklab-1.5.4/netsim/devices/none.yml` & `networklab-1.5.4.post1/netsim/devices/vmx.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,42 @@
-description: Dummy device used to test topology transformation
-#
-# Most features are enabled on the dummy device -- this file is a pretty
-# good template if you want to figure out what device features there are.
-#
-interface_name: eth{ifindex}
-loopback_interface_name: Loopback{ifindex}
-tunnel_interface_name: Tunnel{ifindex}
-virtualbox:
-  image: none
-libvirt:
-  image: none
-clab:
-  image: none
-external:
-  image: none
+description: Juniper vMX container
+interface_name: ge-0/0/{ifindex}
+loopback_interface_name: "lo0.{ifindex}"
+ifindex_offset: 0
+mgmt_if: fxp0
 group_vars:
-  ansible_connection: paramiko_ssh
-  ansible_network_os: none
+  ansible_user: admin
+  ansible_ssh_pass: "admin@123"
+  ansible_network_os: junos
+  ansible_connection: netconf
+  netlab_console_connection: ssh
+  netlab_device_type: vmx
 features:
-  bgp:
-    local_as: True
-    vrf_local_as: True
-    local_as_ibgp: True
-    activate_af: True
-    ipv6_lla: True
-    rfc8950: True
   initial:
     ipv4:
       unnumbered: True
     ipv6:
       lla: True
   ospf:
     unnumbered: True
   isis:
     unnumbered:
       ipv4: True
       ipv6: True
-      network: True
-  mpls:
-    ldp: True
-    bgp: True
-    vpn: True
-    6pe: True
-  evpn:
-    irb: True
-    asymmetrical_irb: True
-    bundle: [ vlan_aware ]
-  gateway:
-    protocol: [ anycast, vrrp ]
   vlan:
-    model: l3-switch
-    svi_interface_name: Vlan{vlan}
+    model: router
+    svi_interface_name: irb.{vlan}
     subif_name: "{ifname}.{vlan.access_id}"
     mixed_trunk: True
     native_routed: True
+  mpls:
+    ldp: True
+    vpn: True
+clab:
+  image: vrnetlab/vr-vmx:18.2R1.9
+  node:
+    kind: vr-vmx
+  interface:
+    name: eth{ifindex+1}
+external:
+  image: none
+graphite.icon: router
```

### Comparing `networklab-1.5.4/netsim/devices/nxos.yml` & `networklab-1.5.4.post1/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/routeros7.yml` & `networklab-1.5.4.post1/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/srlinux.yml` & `networklab-1.5.4.post1/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/sros.yml` & `networklab-1.5.4.post1/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/unknown.py` & `networklab-1.5.4.post1/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/vmx.py` & `networklab-1.5.4.post1/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/vptx.py` & `networklab-1.5.4.post1/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/vptx.yml` & `networklab-1.5.4.post1/netsim/devices/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/vsrx.py` & `networklab-1.5.4.post1/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/vsrx.yml` & `networklab-1.5.4.post1/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/devices/vyos.yml` & `networklab-1.5.4.post1/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.5.4.post1/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/multilab/plugin.py` & `networklab-1.5.4.post1/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/proxy-arp/plugin.py` & `networklab-1.5.4.post1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.5.4.post1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/extra/proxy-arp/sros.j2` & `networklab-1.5.4.post1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/ansible.sh` & `networklab-1.5.4.post1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/containerlab.sh` & `networklab-1.5.4.post1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/grpc.sh` & `networklab-1.5.4.post1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/arubacx.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/asav/day0-config` & `networklab-1.5.4.post1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/csr.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/dellos10.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/eos.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/eos.xml.j2` & `networklab-1.5.4.post1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/iosv.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.5.4.post1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/iosxr.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/nxos.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.5.4.post1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/routeros7.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.5.4.post1/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.5.4.post1/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vptx/run.sh` & `networklab-1.5.4.post1/netsim/install/libvirt/vptx/run.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vptx.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.5.4.post1/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.5.4.post1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt/vsrx.txt` & `networklab-1.5.4.post1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/libvirt.sh` & `networklab-1.5.4.post1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/install/ubuntu.sh` & `networklab-1.5.4.post1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/__init__.py` & `networklab-1.5.4.post1/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/_dataplane.py` & `networklab-1.5.4.post1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/_routing.py` & `networklab-1.5.4.post1/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/bfd.py` & `networklab-1.5.4.post1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/bfd.yml` & `networklab-1.5.4.post1/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/bgp.py` & `networklab-1.5.4.post1/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/bgp.yml` & `networklab-1.5.4.post1/netsim/modules/bgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/evpn.py` & `networklab-1.5.4.post1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/evpn.yml` & `networklab-1.5.4.post1/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/gateway.py` & `networklab-1.5.4.post1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/gateway.yml` & `networklab-1.5.4.post1/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/isis.py` & `networklab-1.5.4.post1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/isis.yml` & `networklab-1.5.4.post1/netsim/modules/isis.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/mpls.py` & `networklab-1.5.4.post1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/mpls.yml` & `networklab-1.5.4.post1/netsim/modules/mpls.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/ospf.py` & `networklab-1.5.4.post1/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/ospf.yml` & `networklab-1.5.4.post1/netsim/modules/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/srv6.py` & `networklab-1.5.4.post1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/vlan.py` & `networklab-1.5.4.post1/netsim/modules/vlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,15 +416,15 @@
 """
 create_vlan_link_data: Create initial link data for a VLAN member link
 
 Used by create_vlan_links and create_loopback_vlan_links
 """
 def create_vlan_link_data(init: typing.Union[Box,dict],vname: str, parent: typing.Any, topology: Box) -> Box:
   link_data = data.get_box(init)
-  link_data.linkindex = topology.links[-1].linkindex + 1
+  link_data.linkindex = links.get_next_linkindex(topology)
   link_data.parentindex = parent
   link_data.vlan.access = vname
   link_data.vlan_name = vname
   link_data.type = 'vlan_member'
   link_data.interfaces = []
   fix_vlan_mode_attribute(link_data)
 
@@ -1081,14 +1081,17 @@
           path='topology',
           create_empty=False,
           abort=True,
           module='vlan')      # Check that we're dealing with a VLAN dictionary and return if there's an error
       except:
         return
 
+      if not 'links' in topology:                 # Make sure there's a 'links' element in topology
+        topology.links = []                       # ... so the various link-related hooks are called and we get 
+                                                  # ... VLAN subinterfaces
     if 'groups' in topology:
       groups.export_group_node_data(topology,'vlans','vlan',copy_keys=['id','vni'])
 
     if topology.get('vlan.mode',None):
       if topology.vlan.mode not in vlan_mode_kwd:     # pragma: no cover
         common.error(
           f'Invalid global vlan.mode value {topology.vlan.mode}',
```

### Comparing `networklab-1.5.4/netsim/modules/vlan.yml` & `networklab-1.5.4.post1/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/vrf.py` & `networklab-1.5.4.post1/netsim/modules/vrf.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,36 @@
 from .. import data
 from ..data import global_vars
 from ..data.validate import validate_attributes
 from ..data.types import must_be_list,must_be_dict,must_be_id
 from ..augment import devices,groups,links
 from .. import addressing
 
+#
+# get_node_vrf_data: an abstraction layer that returns node-level VRF data structure
+# as it would appear after the node_post_transform hook
+#
+# You have to use this function instead of 'node or global data' logic whenever you need
+# node VRF data before VRF node_post_transform hook is executed
+#
+
+def get_node_vrf_data(vname: str, node: Box, topology: Box) -> typing.Optional[Box]:
+  topo_data = topology.get('vrfs').get(vname,None)    # Get global VRF data (or none if there's no global data)
+  if not vname in node.get('vrfs',{}):                # If there's no node VRF data
+    return topo_data                                  # ... return global value whatever it is
+  else:
+    node_data = node.vrfs[vname]                      # We have some node VRF data, and we assume it's a Box
+    topo_data = topo_data or {}                       # Global data must be a dict/Box or the merge will fail
+    return topo_data + node_data                      # Now merge global+node data
+                                                      # ... note that the result will always be a Box
+
+#
+# Build the global data structures needed for ID/RD allocation and populate
+# them with preconfigured global- and node VRF data
+#
 def populate_vrf_static_ids(topology: Box) -> None:
   for k in ('id','rd'):
     _dataplane.create_id_set(f'vrf_{k}')
     _dataplane.extend_id_set(f'vrf_{k}',_dataplane.build_id_set(topology,'vrfs',k,'topology'))
 
   _dataplane.set_id_counter('vrf_id',1,4095)
 
@@ -165,41 +187,54 @@
 # Set RD values for all VRFs that have no RD attribute or RD value set to None (= auto-generate)
 #
 def set_vrf_ids(obj: Box, topology: Box) -> None:
   if not 'vrfs' in obj:
     return
 
   asn = None
-  obj_name = 'global VRFs' if obj is topology else obj.name
+  is_global = obj is topology
+  obj_name = 'global VRFs' if is_global else obj.name
 
-  for vname,vdata in obj.vrfs.items():
-    if vrf_needs_id(vdata):
-      asn = asn or get_rd_as_number(obj,topology)
-      if not asn:
-        common.error('Need a usable vrf.as or bgp.as to create auto-generated VRF RD for {vname} in {obj_name}',
-          common.MissingValue,
-          'vrf')
-        return
-      set_vrf_auto_id(vdata,get_next_vrf_id(asn))
+  for vname,vdata in obj.vrfs.items():                      # Iterate over object VRFs
+    if not vrf_needs_id(vdata):                             # Skip if the ID/RD is set
+      continue
+
+    if not is_global and vname in topology.get('vrfs',{}):  # Can we copy the global values?
+      vdata.id = topology.vrfs[vname].id                    # ... we have to copy individual values because
+      vdata.rd = topology.vrfs[vname].rd                    # ... we cannot simply merge global into node data
+      continue                                              # ... before post-transform
+
+    asn = asn or get_rd_as_number(obj,topology)
+    if not asn:
+      common.error('Need a usable vrf.as or bgp.as to create auto-generated VRF RD for {vname} in {obj_name}',
+        common.MissingValue,
+        'vrf')
+      return
+    set_vrf_auto_id(vdata,get_next_vrf_id(asn))
 
 #
 # Set import/export route targets
 #
 def set_import_export_rt(obj : Box, topology: Box) -> None:
   if not 'vrfs' in obj:
     return None
 
-  obj_name = 'global VRFs' if obj is topology else obj.name
+  is_global = obj is topology
+  obj_name = 'global VRFs' if is_global else obj.name
   obj_id   = 'vrfs' if obj is topology else f'nodes.{obj.name}.vrfs'
   asn      = None
 
   for vname,vdata in obj.vrfs.items():
     for rtname in ['import','export']:
       if not rtname in vdata:
-        vdata[rtname] = [ vdata.rd ]
+        if not is_global and vname in topology.get('vrfs',{}):        # Copy global RT into node RT if available
+          vdata[rtname] = topology.vrfs[vname][rtname]                # ... see set_vrf_ids for detailed description
+          continue                                                    # ... of this hack
+
+        vdata[rtname] = [ vdata.rd ]                                  # No usable parent RT, set RT to RD
         continue
 
       must_be_list(vdata,rtname,f'{obj_id}.{vname}')
 
       rtlist = []     # The final parsed and looked-up list of RT values
       for rtvalue in vdata[rtname]:
         if isinstance(rtvalue,int):         # RT can be specified as an integer, in which case ASN is prepended to it
@@ -415,20 +450,20 @@
     # Check if any global vrfs need to be pulled in due to being referenced by a vlan
     vlan_vrfs = [ vdata.vrf for vname,vdata in node.get('vlans',{}).items() if 'vrf' in vdata ]
     if not 'vrfs' in node:
       if not vlan_vrfs:  # No local vrfs and no vlan references -> exit
         return
       node.vrfs = {}     # Prepare to pull in global vrfs
 
-    if not must_be_dict(
+    if must_be_dict(
         parent=node,
         key='vrfs',
         path=f'nodes.{node.name}',
         create_empty=False,
-        module='vrf'):                                # Check that we're dealing with a VRF dictionary and return if there's none
+        module='vrf') is False:                            # Check that we're dealing with a VRF dictionary and return if there's none
       return
 
     for vname in set(list(node.vrfs.keys()) + vlan_vrfs):  # Filter out duplicates
       if node.vrfs[vname] is None:
         node.vrfs[vname] = {}
 
       validate_attributes(
@@ -437,16 +472,16 @@
         data_path=f'nodes.{node.name}.vrfs.{vname}',  # Path to node VRF definition
         data_name=f'VRF',
         attr_list=['vrf','link'],                     # We're checking VLAN and link attributes
         modules=node.get('module',[]),                # ... against node modules
         module_source=f'nodes.{node.name}',
         module='vrf')                                 # Function is called from 'vrf' module
 
-      if 'vrfs' in topology and vname in topology.vrfs:
-        node.vrfs[vname] = topology.vrfs[vname] + node.vrfs[vname]
+#      if 'vrfs' in topology and vname in topology.vrfs:
+#        node.vrfs[vname] = topology.vrfs[vname] + node.vrfs[vname]
 
     set_vrf_ids(node,topology)
     set_import_export_rt(node,topology)
 
   def link_pre_transform(self, link: Box, topology: Box) -> None:
     pass
```

### Comparing `networklab-1.5.4/netsim/modules/vxlan.py` & `networklab-1.5.4.post1/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/modules/vxlan.yml` & `networklab-1.5.4.post1/netsim/modules/vxlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/__init__.py` & `networklab-1.5.4.post1/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/ansible.py` & `networklab-1.5.4.post1/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/common.py` & `networklab-1.5.4.post1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/d2.py` & `networklab-1.5.4.post1/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/d2.yml` & `networklab-1.5.4.post1/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/devices.py` & `networklab-1.5.4.post1/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/format.py` & `networklab-1.5.4.post1/netsim/outputs/format.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/graph.py` & `networklab-1.5.4.post1/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/graphite.py` & `networklab-1.5.4.post1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/provider.py` & `networklab-1.5.4.post1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/tools.py` & `networklab-1.5.4.post1/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/outputs/yaml.py` & `networklab-1.5.4.post1/netsim/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/providers/__init__.py` & `networklab-1.5.4.post1/netsim/providers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Provider class and replacing or augmenting its methods (most commonly, transform)
 #
 
 import platform
 import subprocess
 import os
 import typing
+import pathlib
 
 # Related modules
 from box import Box
 
 from .. import common
 from ..callback import Callback
 from ..augment import devices,links
@@ -103,15 +104,15 @@
         common.error(
           f"Cannot find template {file}.j2 for extra file {self.provider}.{inkey}.{file} on node {node.name}",
           common.IncorrectValue,
           self.provider)
         continue
 
       out_folder = f"{self.provider}_files/{node.name}"
-      bind_dict[f"{out_folder}/{file}"] = mapping
+      bind_dict[f"{out_folder}/{file}"] = mapping         # note: node_files directory is flat
 
     node[self.provider][outkey] = filemaps.dict_to_mapping(bind_dict)
 
   def create_extra_files(
       self,
       node: Box,
       topology: Box,
@@ -129,20 +130,24 @@
     for file,mapping in bind_dict.items():
       if not out_folder in file:                  # Skip files that are not mapped into the temporary provider folder
         continue
       file_name = file.replace(out_folder+"/","")
       template_name = self.find_extra_template(node,file_name)
       if template_name:
         node_data = node + { 'hostvars': topology.nodes }
+        if '/' in file_name:                      # Create subdirectory in out_folder if needed
+          pathlib.Path(f"{out_folder}/{os.path.dirname(file_name)}").mkdir(parents=True,exist_ok=True)
         common.write_template(
           in_folder=os.path.dirname(template_name),
           j2=os.path.basename(template_name),
           data=node_data.to_dict(),
           out_folder=out_folder, filename=file_name)
         print( f"Created {out_folder}/{file_name} from {template_name.replace(sys_folder,'')}, mapped to {node.name}:{mapping}" )
+      else:
+        common.error(f"Cannot find template for {file_name} on node {node.name}",common.MissingValue,'provider')
 
   def create(self, topology: Box, fname: typing.Optional[str]) -> None:
     self.transform(topology)
     fname = self.get_output_name(fname,topology)
     output = common.open_output_file(fname)
     output.write(common.template(self.get_root_template(),topology.to_dict(),self.get_template_path(),self.provider))
     if fname != '-':
@@ -234,11 +239,12 @@
 """
 Select a subset of the topology -- links and nodes relevant to the current provider
 """
 def select_topology(topology: Box, provider: str) -> Box:
   topology = get_box(topology)                      # Create a copy of the topology
   for n in list(topology.nodes.keys()):             # Remove all nodes not belonging to the current provider
     if topology.nodes[n].provider != provider:
-      topology.nodes.pop(n,None)
+      topology.nodes[n].unmanaged = True
+#      topology.nodes.pop(n,None)
 
   topology.links = [ l for l in topology.links if provider in l.provider ]      # Retain only the links used by current provider
   return topology
```

### Comparing `networklab-1.5.4/netsim/providers/clab.py` & `networklab-1.5.4.post1/netsim/providers/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/providers/clab.yml` & `networklab-1.5.4.post1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/providers/external.py` & `networklab-1.5.4.post1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/providers/libvirt.py` & `networklab-1.5.4.post1/netsim/providers/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/providers/libvirt.yml` & `networklab-1.5.4.post1/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/read_topology.py` & `networklab-1.5.4.post1/netsim/read_topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/clab/clab.j2` & `networklab-1.5.4.post1/netsim/templates/provider/clab/clab.j2`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   ipv6-subnet: {{ defaults.addressing.mgmt.ipv6 }}
 {% endif %}
 {% if addressing.mgmt._bridge|default('') %}
   bridge: {{ addressing.mgmt._bridge }}
 {% endif %}
 topology:
   nodes:
-{% for name,n in nodes.items() %}
+{% for name,n in nodes.items() if not (n.unmanaged|default(False)) %}
 {%   set clab = n.clab|default({}) %}
     {{ name }}:
 {%   if n.mgmt.ipv4 is defined %}
       mgmt-ipv4: {{ n.mgmt.ipv4 }}
 {%   endif %}
 {%   if n.mgmt.ipv6 is defined %}
       mgmt-ipv6: {{ n.mgmt.ipv6 }}
@@ -63,22 +63,22 @@
       kind: {{ bridge_type }}
 {% endfor %}
 
   links:
 {% for l in links %}
 {% if (l.bridge is not defined) or l.node_count==2 %}
   - endpoints:
-{%   for n in nodes.values() %}
+{%   for n in nodes.values() if not (n.unmanaged|default(False)) %}
 {%     for nl in n.interfaces|default([]) if nl.linkindex|default(0) == l.linkindex %}
 {%       set clab = nl.clab|default({}) %}
     - "{{ n.name }}:{{ clab.name|default(nl.ifname) }}"
 {%     endfor %}
 {%   endfor %}
 {% else %}
-{%   for n in nodes.values() %}
+{%   for n in nodes.values() if not (n.unmanaged|default(False)) %}
 {%     for nl in n.interfaces|default([]) if nl.linkindex|default(0) == l.linkindex %}
 {%       set clab = nl.clab|default({}) %}
   - endpoints:
     - "{{ n.name }}:{{ clab.name|default(nl.ifname) }}"
 {# Use node_intf name for bridge veth interface in standard setup and more cryptic (but unique) name in multilab deployment #}
 {%       if defaults.multilab.id|default(False) %}
     - "{{ l.bridge }}:{{ name[:6] }}_{{ n.id }}_{{ nl.ifindex }}"
```

### Comparing `networklab-1.5.4/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.5.4.post1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.5.4.post1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/external/external.j2` & `networklab-1.5.4.post1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,14 @@
   config.vm.provider :libvirt do |libvirt|
 {% if addressing.mgmt._network|default(False) %}
     libvirt.management_network_name = "{{ addressing.mgmt._network }}"
 {% endif %}
     libvirt.management_network_address = "{{ addressing.mgmt.ipv4 }}"
     libvirt.default_prefix = "{{ defaults.name }}_"
   end
-{% for name,n in nodes.items() %}
+{% for name,n in nodes.items() if not (n.unmanaged|default(False)) %}
 {%   set name = name.split('.')[0] %}
 {%   set box  = n.box %}
 {%   include [ n.device ~ "-raw.j2","define-domain.j2" ] +%}
 {% endfor %}
 end
```

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.5.4.post1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.5.4.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # VirtualBox vagrantfile template
 #
 Vagrant.configure("2") do |config|
-{% for name,n in nodes.items() %}
+{% for name,n in nodes.items() if not (n.unmanaged|default(False)) %}
 {%   set name = name.split('.')[0] %}
 {%   set box  = n.box %}
   config.vm.define "{{ name }}" do |{{name}}|
     {{ name }}.vm.box = "{{ box }}"
 {% if 'box_version' in n  %}
     {{ name }}.vm.box_version = "{{ n.box_version }}"
 {% endif %}
```

### Comparing `networklab-1.5.4/netsim/tools/__init__.py` & `networklab-1.5.4.post1/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/tools/graphite.py` & `networklab-1.5.4.post1/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/tools/graphite.yml` & `networklab-1.5.4.post1/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/tools/suzieq.yml` & `networklab-1.5.4.post1/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/topology-defaults.yml` & `networklab-1.5.4.post1/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/utils/log.py` & `networklab-1.5.4.post1/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/utils/status.py` & `networklab-1.5.4.post1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/utils/strings.py` & `networklab-1.5.4.post1/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/netsim/utils/templates.py` & `networklab-1.5.4.post1/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/networklab.egg-info/PKG-INFO` & `networklab-1.5.4.post1/networklab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.4
+Version: 1.5.4.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `networklab-1.5.4/networklab.egg-info/SOURCES.txt` & `networklab-1.5.4.post1/networklab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -405,14 +405,15 @@
 netsim/devices/vptx.py
 netsim/devices/vptx.yml
 netsim/devices/vsrx.py
 netsim/devices/vsrx.yml
 netsim/devices/vyos.yml
 netsim/extra/ebgp.utils/default-originate.yml
 netsim/extra/ebgp.utils/eos.j2
+netsim/extra/ebgp.utils/frr.j2
 netsim/extra/ebgp.utils/ios.j2
 netsim/extra/ebgp.utils/junos.j2
 netsim/extra/ebgp.utils/plugin.py
 netsim/extra/ebgp.utils/routeros7.j2
 netsim/extra/ebgp.utils/srlinux.j2
 netsim/extra/ebgp.utils/topology.yml
 netsim/extra/ebgp.utils/vyos.j2
@@ -511,14 +512,15 @@
 netsim/templates/provider/libvirt/csr-domain.j2
 netsim/templates/provider/libvirt/cumulus-domain.j2
 netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
 netsim/templates/provider/libvirt/define-domain.j2
 netsim/templates/provider/libvirt/dellos10-domain.j2
 netsim/templates/provider/libvirt/eos-domain.j2
 netsim/templates/provider/libvirt/fortios-domain.j2
+netsim/templates/provider/libvirt/frr-domain.j2
 netsim/templates/provider/libvirt/iosv-domain.j2
 netsim/templates/provider/libvirt/iosxr-domain.j2
 netsim/templates/provider/libvirt/libvirt-bridge.j2
 netsim/templates/provider/libvirt/libvirt-tunnel.j2
 netsim/templates/provider/libvirt/linux-domain.j2
 netsim/templates/provider/libvirt/none-domain.j2
 netsim/templates/provider/libvirt/nxos-domain.j2
@@ -528,14 +530,15 @@
 netsim/templates/provider/libvirt/vptx-domain.j2
 netsim/templates/provider/libvirt/vsrx-domain.j2
 netsim/templates/provider/libvirt/vyos-domain.j2
 netsim/templates/provider/virtualbox/Vagrantfile.j2
 netsim/templates/provider/virtualbox/arcos-domain.j2
 netsim/templates/provider/virtualbox/cumulus-domain.j2
 netsim/templates/provider/virtualbox/eos-domain.j2
+netsim/templates/provider/virtualbox/frr-domain.j2
 netsim/templates/provider/virtualbox/linux-domain.j2
 netsim/templates/provider/virtualbox/nxos-domain.j2
 netsim/templates/provider/virtualbox/virtualbox-network.j2
 netsim/templates/provider/virtualbox/virtualbox-ports.j2
 netsim/templates/tests/clab.yml
 netsim/templates/tests/libvirt.yml
 netsim/templates/tests/virtualbox.yml
```

### Comparing `networklab-1.5.4/setup.py` & `networklab-1.5.4.post1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.4/tests/test_transformation.py` & `networklab-1.5.4.post1/tests/test_transformation.py`

 * *Files identical despite different names*

