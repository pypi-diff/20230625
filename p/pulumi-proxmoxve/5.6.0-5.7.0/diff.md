# Comparing `tmp/pulumi_proxmoxve-5.6.0.tar.gz` & `tmp/pulumi_proxmoxve-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-5.6.0.tar", last modified: Thu Jun 15 14:21:32 2023, max compression
+gzip compressed data, was "pulumi_proxmoxve-5.7.0.tar", last modified: Sun Jun 25 17:20:26 2023, max compression
```

## Comparing `pulumi_proxmoxve-5.6.0.tar` & `pulumi_proxmoxve-5.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10392 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/get_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34450 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28465 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83149 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:21:32.181571 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 14:21:32.000000 pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:21:32.185571 pulumi_proxmoxve-5.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-15 14:21:31.000000 pulumi_proxmoxve-5.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/get_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37407 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29546 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34964 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28878 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83149 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:26.661079 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:20:26.665079 pulumi_proxmoxve-5.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-25 17:20:26.000000 pulumi_proxmoxve-5.7.0/setup.py
```

### Comparing `pulumi_proxmoxve-5.6.0/PKG-INFO` & `pulumi_proxmoxve-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 5.6.0
+Version: 5.7.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_proxmoxve-5.6.0/README.md` & `pulumi_proxmoxve-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,318 +3,443 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
+from .. import _utilities
 
 __all__ = [
-    'HostsEntryArgs',
-    'ProviderSshArgs',
-    'ProviderSshNodeArgs',
-    'ProviderVirtualEnvironmentArgs',
-    'ProviderVirtualEnvironmentSshArgs',
-    'ProviderVirtualEnvironmentSshNodeArgs',
+    'FirewallIPSetCidrArgs',
+    'FirewallLogRatelimitArgs',
+    'FirewallRulesRuleArgs',
+    'FirewallSecurityGroupRuleArgs',
 ]
 
 @pulumi.input_type
-class HostsEntryArgs:
+class FirewallIPSetCidrArgs:
     def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 hostnames: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "hostnames", hostnames)
+                 name: pulumi.Input[str],
+                 comment: Optional[pulumi.Input[str]] = None,
+                 nomatch: Optional[pulumi.Input[bool]] = None):
+        pulumi.set(__self__, "name", name)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if nomatch is not None:
+            pulumi.set(__self__, "nomatch", nomatch)
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "address")
+    def name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "name")
 
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def hostnames(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        return pulumi.get(self, "hostnames")
+    def comment(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "comment")
+
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
-    @hostnames.setter
-    def hostnames(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "hostnames", value)
+    @property
+    @pulumi.getter
+    def nomatch(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "nomatch")
+
+    @nomatch.setter
+    def nomatch(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "nomatch", value)
 
 
 @pulumi.input_type
-class ProviderSshArgs:
+class FirewallLogRatelimitArgs:
     def __init__(__self__, *,
-                 agent: Optional[pulumi.Input[bool]] = None,
-                 agent_socket: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        if agent is not None:
-            pulumi.set(__self__, "agent", agent)
-        if agent_socket is not None:
-            pulumi.set(__self__, "agent_socket", agent_socket)
-        if nodes is not None:
-            pulumi.set(__self__, "nodes", nodes)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+                 burst: Optional[pulumi.Input[int]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 rate: Optional[pulumi.Input[str]] = None):
+        if burst is not None:
+            pulumi.set(__self__, "burst", burst)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if rate is not None:
+            pulumi.set(__self__, "rate", rate)
 
     @property
     @pulumi.getter
-    def agent(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "agent")
+    def burst(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "burst")
 
-    @agent.setter
-    def agent(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "agent", value)
+    @burst.setter
+    def burst(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "burst", value)
 
     @property
-    @pulumi.getter(name="agentSocket")
-    def agent_socket(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "agent_socket")
+    @pulumi.getter
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "enabled")
 
-    @agent_socket.setter
-    def agent_socket(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "agent_socket", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
-    def nodes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]]:
-        return pulumi.get(self, "nodes")
+    def rate(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "rate")
+
+    @rate.setter
+    def rate(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "rate", value)
+
 
-    @nodes.setter
-    def nodes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]]):
-        pulumi.set(self, "nodes", value)
+@pulumi.input_type
+class FirewallRulesRuleArgs:
+    def __init__(__self__, *,
+                 action: Optional[pulumi.Input[str]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 dest: Optional[pulumi.Input[str]] = None,
+                 dport: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 iface: Optional[pulumi.Input[str]] = None,
+                 log: Optional[pulumi.Input[str]] = None,
+                 macro: Optional[pulumi.Input[str]] = None,
+                 pos: Optional[pulumi.Input[int]] = None,
+                 proto: Optional[pulumi.Input[str]] = None,
+                 security_group: Optional[pulumi.Input[str]] = None,
+                 source: Optional[pulumi.Input[str]] = None,
+                 sport: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        if action is not None:
+            pulumi.set(__self__, "action", action)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if dest is not None:
+            pulumi.set(__self__, "dest", dest)
+        if dport is not None:
+            pulumi.set(__self__, "dport", dport)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if iface is not None:
+            pulumi.set(__self__, "iface", iface)
+        if log is not None:
+            pulumi.set(__self__, "log", log)
+        if macro is not None:
+            pulumi.set(__self__, "macro", macro)
+        if pos is not None:
+            pulumi.set(__self__, "pos", pos)
+        if proto is not None:
+            pulumi.set(__self__, "proto", proto)
+        if security_group is not None:
+            pulumi.set(__self__, "security_group", security_group)
+        if source is not None:
+            pulumi.set(__self__, "source", source)
+        if sport is not None:
+            pulumi.set(__self__, "sport", sport)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
+    def action(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "action")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @action.setter
+    def action(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username")
+    def comment(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "comment")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
+    @property
+    @pulumi.getter
+    def dest(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "dest")
 
-@pulumi.input_type
-class ProviderSshNodeArgs:
-    def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 name: pulumi.Input[str]):
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "name", name)
+    @dest.setter
+    def dest(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dest", value)
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "address")
+    def dport(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "dport")
 
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
+    @dport.setter
+    def dport(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dport", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "name")
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "enabled")
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
+    @property
+    @pulumi.getter
+    def iface(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "iface")
 
-@pulumi.input_type
-class ProviderVirtualEnvironmentArgs:
-    def __init__(__self__, *,
-                 api_token: Optional[pulumi.Input[str]] = None,
-                 endpoint: Optional[pulumi.Input[str]] = None,
-                 insecure: Optional[pulumi.Input[bool]] = None,
-                 otp: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 ssh: Optional[pulumi.Input['ProviderVirtualEnvironmentSshArgs']] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        if api_token is not None:
-            pulumi.set(__self__, "api_token", api_token)
-        if endpoint is not None:
-            pulumi.set(__self__, "endpoint", endpoint)
-        if insecure is not None:
-            pulumi.set(__self__, "insecure", insecure)
-        if otp is not None:
-            pulumi.set(__self__, "otp", otp)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if ssh is not None:
-            pulumi.set(__self__, "ssh", ssh)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+    @iface.setter
+    def iface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "iface", value)
 
     @property
-    @pulumi.getter(name="apiToken")
-    def api_token(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "api_token")
+    @pulumi.getter
+    def log(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "log")
 
-    @api_token.setter
-    def api_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "api_token", value)
+    @log.setter
+    def log(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "log", value)
 
     @property
     @pulumi.getter
-    def endpoint(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "endpoint")
+    def macro(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "macro")
 
-    @endpoint.setter
-    def endpoint(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "endpoint", value)
+    @macro.setter
+    def macro(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "macro", value)
 
     @property
     @pulumi.getter
-    def insecure(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "insecure")
+    def pos(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "pos")
 
-    @insecure.setter
-    def insecure(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "insecure", value)
+    @pos.setter
+    def pos(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "pos", value)
 
     @property
     @pulumi.getter
-    def otp(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "otp")
+    def proto(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "proto")
 
-    @otp.setter
-    def otp(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "otp", value)
+    @proto.setter
+    def proto(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proto", value)
+
+    @property
+    @pulumi.getter(name="securityGroup")
+    def security_group(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "security_group")
+
+    @security_group.setter
+    def security_group(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "security_group", value)
 
     @property
     @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
+    def source(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "source")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @source.setter
+    def source(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
-    def ssh(self) -> Optional[pulumi.Input['ProviderVirtualEnvironmentSshArgs']]:
-        return pulumi.get(self, "ssh")
+    def sport(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "sport")
 
-    @ssh.setter
-    def ssh(self, value: Optional[pulumi.Input['ProviderVirtualEnvironmentSshArgs']]):
-        pulumi.set(self, "ssh", value)
+    @sport.setter
+    def sport(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "sport", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username")
+    def type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "type")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
-class ProviderVirtualEnvironmentSshArgs:
+class FirewallSecurityGroupRuleArgs:
     def __init__(__self__, *,
-                 agent: Optional[pulumi.Input[bool]] = None,
-                 agent_socket: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderVirtualEnvironmentSshNodeArgs']]]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        if agent is not None:
-            pulumi.set(__self__, "agent", agent)
-        if agent_socket is not None:
-            pulumi.set(__self__, "agent_socket", agent_socket)
-        if nodes is not None:
-            pulumi.set(__self__, "nodes", nodes)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+                 action: Optional[pulumi.Input[str]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 dest: Optional[pulumi.Input[str]] = None,
+                 dport: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 iface: Optional[pulumi.Input[str]] = None,
+                 log: Optional[pulumi.Input[str]] = None,
+                 macro: Optional[pulumi.Input[str]] = None,
+                 pos: Optional[pulumi.Input[int]] = None,
+                 proto: Optional[pulumi.Input[str]] = None,
+                 security_group: Optional[pulumi.Input[str]] = None,
+                 source: Optional[pulumi.Input[str]] = None,
+                 sport: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        if action is not None:
+            pulumi.set(__self__, "action", action)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if dest is not None:
+            pulumi.set(__self__, "dest", dest)
+        if dport is not None:
+            pulumi.set(__self__, "dport", dport)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if iface is not None:
+            pulumi.set(__self__, "iface", iface)
+        if log is not None:
+            pulumi.set(__self__, "log", log)
+        if macro is not None:
+            pulumi.set(__self__, "macro", macro)
+        if pos is not None:
+            pulumi.set(__self__, "pos", pos)
+        if proto is not None:
+            pulumi.set(__self__, "proto", proto)
+        if security_group is not None:
+            pulumi.set(__self__, "security_group", security_group)
+        if source is not None:
+            pulumi.set(__self__, "source", source)
+        if sport is not None:
+            pulumi.set(__self__, "sport", sport)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
-    def agent(self) -> Optional[pulumi.Input[bool]]:
-        return pulumi.get(self, "agent")
+    def action(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "action")
 
-    @agent.setter
-    def agent(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "agent", value)
+    @action.setter
+    def action(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "action", value)
 
     @property
-    @pulumi.getter(name="agentSocket")
-    def agent_socket(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "agent_socket")
+    @pulumi.getter
+    def comment(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "comment")
 
-    @agent_socket.setter
-    def agent_socket(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "agent_socket", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
     @pulumi.getter
-    def nodes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderVirtualEnvironmentSshNodeArgs']]]]:
-        return pulumi.get(self, "nodes")
+    def dest(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "dest")
 
-    @nodes.setter
-    def nodes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderVirtualEnvironmentSshNodeArgs']]]]):
-        pulumi.set(self, "nodes", value)
+    @dest.setter
+    def dest(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dest", value)
 
     @property
     @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password")
+    def dport(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "dport")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @dport.setter
+    def dport(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dport", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username")
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "enabled")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
+    @property
+    @pulumi.getter
+    def iface(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "iface")
 
-@pulumi.input_type
-class ProviderVirtualEnvironmentSshNodeArgs:
-    def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 name: pulumi.Input[str]):
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "name", name)
+    @iface.setter
+    def iface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "iface", value)
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "address")
+    def log(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "log")
 
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
+    @log.setter
+    def log(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "log", value)
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        return pulumi.get(self, "name")
+    def macro(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "macro")
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+    @macro.setter
+    def macro(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "macro", value)
+
+    @property
+    @pulumi.getter
+    def pos(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "pos")
+
+    @pos.setter
+    def pos(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "pos", value)
+
+    @property
+    @pulumi.getter
+    def proto(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "proto")
+
+    @proto.setter
+    def proto(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "proto", value)
+
+    @property
+    @pulumi.getter(name="securityGroup")
+    def security_group(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "security_group")
+
+    @security_group.setter
+    def security_group(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "security_group", value)
+
+    @property
+    @pulumi.getter
+    def source(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "source")
+
+    @source.setter
+    def source(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "source", value)
+
+    @property
+    @pulumi.getter
+    def sport(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "sport")
+
+    @sport.setter
+    def sport(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "sport", value)
+
+    @property
+    @pulumi.getter
+    def type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,17 +129,17 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Cluster/getNodes:getNodes', __args__, opts=opts, typ=GetNodesResult).value
 
     return AwaitableGetNodesResult(
-        cpu_counts=__ret__.cpu_counts,
-        cpu_utilizations=__ret__.cpu_utilizations,
-        id=__ret__.id,
-        memory_availables=__ret__.memory_availables,
-        memory_useds=__ret__.memory_useds,
-        names=__ret__.names,
-        onlines=__ret__.onlines,
-        ssl_fingerprints=__ret__.ssl_fingerprints,
-        support_levels=__ret__.support_levels,
-        uptimes=__ret__.uptimes)
+        cpu_counts=pulumi.get(__ret__, 'cpu_counts'),
+        cpu_utilizations=pulumi.get(__ret__, 'cpu_utilizations'),
+        id=pulumi.get(__ret__, 'id'),
+        memory_availables=pulumi.get(__ret__, 'memory_availables'),
+        memory_useds=pulumi.get(__ret__, 'memory_useds'),
+        names=pulumi.get(__ret__, 'names'),
+        onlines=pulumi.get(__ret__, 'onlines'),
+        ssl_fingerprints=pulumi.get(__ret__, 'ssl_fingerprints'),
+        support_levels=pulumi.get(__ret__, 'support_levels'),
+        uptimes=pulumi.get(__ret__, 'uptimes'))
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_dns.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_dns.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:index/getDNS:getDNS', __args__, opts=opts, typ=GetDNSResult).value
 
     return AwaitableGetDNSResult(
-        domain=__ret__.domain,
-        id=__ret__.id,
-        node_name=__ret__.node_name,
-        servers=__ret__.servers)
+        domain=pulumi.get(__ret__, 'domain'),
+        id=pulumi.get(__ret__, 'id'),
+        node_name=pulumi.get(__ret__, 'node_name'),
+        servers=pulumi.get(__ret__, 'servers'))
 
 
 @_utilities.lift_output_func(get_dns)
 def get_dns_output(node_name: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDNSResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_hosts.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_hosts.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,20 +97,20 @@
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:index/getHosts:getHosts', __args__, opts=opts, typ=GetHostsResult).value
 
     return AwaitableGetHostsResult(
-        addresses=__ret__.addresses,
-        digest=__ret__.digest,
-        entries=__ret__.entries,
-        hostnames=__ret__.hostnames,
-        id=__ret__.id,
-        node_name=__ret__.node_name)
+        addresses=pulumi.get(__ret__, 'addresses'),
+        digest=pulumi.get(__ret__, 'digest'),
+        entries=pulumi.get(__ret__, 'entries'),
+        hostnames=pulumi.get(__ret__, 'hostnames'),
+        id=pulumi.get(__ret__, 'id'),
+        node_name=pulumi.get(__ret__, 'node_name'))
 
 
 @_utilities.lift_output_func(get_hosts)
 def get_hosts_output(node_name: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHostsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_time.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,19 +87,19 @@
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:index/getTime:getTime', __args__, opts=opts, typ=GetTimeResult).value
 
     return AwaitableGetTimeResult(
-        id=__ret__.id,
-        local_time=__ret__.local_time,
-        node_name=__ret__.node_name,
-        time_zone=__ret__.time_zone,
-        utc_time=__ret__.utc_time)
+        id=pulumi.get(__ret__, 'id'),
+        local_time=pulumi.get(__ret__, 'local_time'),
+        node_name=pulumi.get(__ret__, 'node_name'),
+        time_zone=pulumi.get(__ret__, 'time_zone'),
+        utc_time=pulumi.get(__ret__, 'utc_time'))
 
 
 @_utilities.lift_output_func(get_time)
 def get_time_output(node_name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTimeResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/get_version.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/get_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,12 +84,12 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:index/getVersion:getVersion', __args__, opts=opts, typ=GetVersionResult).value
 
     return AwaitableGetVersionResult(
-        id=__ret__.id,
-        keyboard_layout=__ret__.keyboard_layout,
-        release=__ret__.release,
-        repository_id=__ret__.repository_id,
-        version=__ret__.version)
+        id=pulumi.get(__ret__, 'id'),
+        keyboard_layout=pulumi.get(__ret__, 'keyboard_layout'),
+        release=pulumi.get(__ret__, 'release'),
+        repository_id=pulumi.get(__ret__, 'repository_id'),
+        version=pulumi.get(__ret__, 'version'))
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,19 +88,19 @@
     """
     __args__ = dict()
     __args__['groupId'] = group_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
 
     return AwaitableGetGroupResult(
-        acls=__ret__.acls,
-        comment=__ret__.comment,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        members=__ret__.members)
+        acls=pulumi.get(__ret__, 'acls'),
+        comment=pulumi.get(__ret__, 'comment'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        members=pulumi.get(__ret__, 'members'))
 
 
 @_utilities.lift_output_func(get_group)
 def get_group_output(group_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
     return AwaitableGetGroupsResult(
-        comments=__ret__.comments,
-        group_ids=__ret__.group_ids,
-        id=__ret__.id)
+        comments=pulumi.get(__ret__, 'comments'),
+        group_ids=pulumi.get(__ret__, 'group_ids'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,18 +79,18 @@
     """
     __args__ = dict()
     __args__['poolId'] = pool_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPool:getPool', __args__, opts=opts, typ=GetPoolResult).value
 
     return AwaitableGetPoolResult(
-        comment=__ret__.comment,
-        id=__ret__.id,
-        members=__ret__.members,
-        pool_id=__ret__.pool_id)
+        comment=pulumi.get(__ret__, 'comment'),
+        id=pulumi.get(__ret__, 'id'),
+        members=pulumi.get(__ret__, 'members'),
+        pool_id=pulumi.get(__ret__, 'pool_id'))
 
 
 @_utilities.lift_output_func(get_pool)
 def get_pool_output(pool_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPoolResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,9 +57,9 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getPools:getPools', __args__, opts=opts, typ=GetPoolsResult).value
 
     return AwaitableGetPoolsResult(
-        id=__ret__.id,
-        pool_ids=__ret__.pool_ids)
+        id=pulumi.get(__ret__, 'id'),
+        pool_ids=pulumi.get(__ret__, 'pool_ids'))
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,17 @@
     """
     __args__ = dict()
     __args__['roleId'] = role_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getRole:getRole', __args__, opts=opts, typ=GetRoleResult).value
 
     return AwaitableGetRoleResult(
-        id=__ret__.id,
-        privileges=__ret__.privileges,
-        role_id=__ret__.role_id)
+        id=pulumi.get(__ret__, 'id'),
+        privileges=pulumi.get(__ret__, 'privileges'),
+        role_id=pulumi.get(__ret__, 'role_id'))
 
 
 @_utilities.lift_output_func(get_role)
 def get_role_output(role_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,11 +75,11 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getRoles:getRoles', __args__, opts=opts, typ=GetRolesResult).value
 
     return AwaitableGetRolesResult(
-        id=__ret__.id,
-        privileges=__ret__.privileges,
-        role_ids=__ret__.role_ids,
-        specials=__ret__.specials)
+        id=pulumi.get(__ret__, 'id'),
+        privileges=pulumi.get(__ret__, 'privileges'),
+        role_ids=pulumi.get(__ret__, 'role_ids'),
+        specials=pulumi.get(__ret__, 'specials'))
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,25 +142,25 @@
     """
     __args__ = dict()
     __args__['userId'] = user_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        acls=__ret__.acls,
-        comment=__ret__.comment,
-        email=__ret__.email,
-        enabled=__ret__.enabled,
-        expiration_date=__ret__.expiration_date,
-        first_name=__ret__.first_name,
-        groups=__ret__.groups,
-        id=__ret__.id,
-        keys=__ret__.keys,
-        last_name=__ret__.last_name,
-        user_id=__ret__.user_id)
+        acls=pulumi.get(__ret__, 'acls'),
+        comment=pulumi.get(__ret__, 'comment'),
+        email=pulumi.get(__ret__, 'email'),
+        enabled=pulumi.get(__ret__, 'enabled'),
+        expiration_date=pulumi.get(__ret__, 'expiration_date'),
+        first_name=pulumi.get(__ret__, 'first_name'),
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'),
+        keys=pulumi.get(__ret__, 'keys'),
+        last_name=pulumi.get(__ret__, 'last_name'),
+        user_id=pulumi.get(__ret__, 'user_id'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(user_id: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files 17% similar despite different names*

```diff
@@ -129,17 +129,17 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Permission/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
 
     return AwaitableGetUsersResult(
-        comments=__ret__.comments,
-        emails=__ret__.emails,
-        enableds=__ret__.enableds,
-        expiration_dates=__ret__.expiration_dates,
-        first_names=__ret__.first_names,
-        groups=__ret__.groups,
-        id=__ret__.id,
-        keys=__ret__.keys,
-        last_names=__ret__.last_names,
-        user_ids=__ret__.user_ids)
+        comments=pulumi.get(__ret__, 'comments'),
+        emails=pulumi.get(__ret__, 'emails'),
+        enableds=pulumi.get(__ret__, 'enableds'),
+        expiration_dates=pulumi.get(__ret__, 'expiration_dates'),
+        first_names=pulumi.get(__ret__, 'first_names'),
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'),
+        keys=pulumi.get(__ret__, 'keys'),
+        last_names=pulumi.get(__ret__, 'last_names'),
+        user_ids=pulumi.get(__ret__, 'user_ids'))
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,169 +17,159 @@
     def __init__(__self__, *,
                  api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input['ProviderSshArgs']] = None,
-                 username: Optional[pulumi.Input[str]] = None,
-                 virtual_environment: Optional[pulumi.Input['ProviderVirtualEnvironmentArgs']] = None):
+                 username: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] api_token: The API token for the Proxmox Virtual Environment API
-        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox Virtual Environment API
-        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step
-        :param pulumi.Input[str] otp: The one-time password for the Proxmox Virtual Environment API
-        :param pulumi.Input[str] password: The password for the Proxmox Virtual Environment API
-        :param pulumi.Input['ProviderSshArgs'] ssh: The SSH connection configuration to a Proxmox node
-        :param pulumi.Input[str] username: The username for the Proxmox Virtual Environment API
+        :param pulumi.Input[str] api_token: The API token for the Proxmox VE API.
+        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox VE API.
+        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step.
+        :param pulumi.Input[str] otp: The one-time password for the Proxmox VE API.
+        :param pulumi.Input[str] password: The password for the Proxmox VE API.
+        :param pulumi.Input['ProviderSshArgs'] ssh: The SSH configuration for the Proxmox nodes.
+        :param pulumi.Input[str] username: The username for the Proxmox VE API.
         """
         if api_token is not None:
             pulumi.set(__self__, "api_token", api_token)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
         if otp is not None:
+            warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+            pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
+        if otp is not None:
             pulumi.set(__self__, "otp", otp)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if ssh is not None:
             pulumi.set(__self__, "ssh", ssh)
         if username is not None:
             pulumi.set(__self__, "username", username)
-        if virtual_environment is not None:
-            warnings.warn("""Move attributes out of virtual_environment block""", DeprecationWarning)
-            pulumi.log.warn("""virtual_environment is deprecated: Move attributes out of virtual_environment block""")
-        if virtual_environment is not None:
-            pulumi.set(__self__, "virtual_environment", virtual_environment)
 
     @property
     @pulumi.getter(name="apiToken")
     def api_token(self) -> Optional[pulumi.Input[str]]:
         """
-        The API token for the Proxmox Virtual Environment API
+        The API token for the Proxmox VE API.
         """
         return pulumi.get(self, "api_token")
 
     @api_token.setter
     def api_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_token", value)
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
         """
-        The endpoint for the Proxmox Virtual Environment API
+        The endpoint for the Proxmox VE API.
         """
         return pulumi.get(self, "endpoint")
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter
     def insecure(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to skip the TLS verification step
+        Whether to skip the TLS verification step.
         """
         return pulumi.get(self, "insecure")
 
     @insecure.setter
     def insecure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "insecure", value)
 
     @property
     @pulumi.getter
     def otp(self) -> Optional[pulumi.Input[str]]:
         """
-        The one-time password for the Proxmox Virtual Environment API
+        The one-time password for the Proxmox VE API.
         """
+        warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
+
         return pulumi.get(self, "otp")
 
     @otp.setter
     def otp(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "otp", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The password for the Proxmox Virtual Environment API
+        The password for the Proxmox VE API.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def ssh(self) -> Optional[pulumi.Input['ProviderSshArgs']]:
         """
-        The SSH connection configuration to a Proxmox node
+        The SSH configuration for the Proxmox nodes.
         """
         return pulumi.get(self, "ssh")
 
     @ssh.setter
     def ssh(self, value: Optional[pulumi.Input['ProviderSshArgs']]):
         pulumi.set(self, "ssh", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The username for the Proxmox Virtual Environment API
+        The username for the Proxmox VE API.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
-    @property
-    @pulumi.getter(name="virtualEnvironment")
-    def virtual_environment(self) -> Optional[pulumi.Input['ProviderVirtualEnvironmentArgs']]:
-        return pulumi.get(self, "virtual_environment")
-
-    @virtual_environment.setter
-    def virtual_environment(self, value: Optional[pulumi.Input['ProviderVirtualEnvironmentArgs']]):
-        pulumi.set(self, "virtual_environment", value)
-
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
                  username: Optional[pulumi.Input[str]] = None,
-                 virtual_environment: Optional[pulumi.Input[pulumi.InputType['ProviderVirtualEnvironmentArgs']]] = None,
                  __props__=None):
         """
         The provider type for the proxmoxve package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] api_token: The API token for the Proxmox Virtual Environment API
-        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox Virtual Environment API
-        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step
-        :param pulumi.Input[str] otp: The one-time password for the Proxmox Virtual Environment API
-        :param pulumi.Input[str] password: The password for the Proxmox Virtual Environment API
-        :param pulumi.Input[pulumi.InputType['ProviderSshArgs']] ssh: The SSH connection configuration to a Proxmox node
-        :param pulumi.Input[str] username: The username for the Proxmox Virtual Environment API
+        :param pulumi.Input[str] api_token: The API token for the Proxmox VE API.
+        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox VE API.
+        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step.
+        :param pulumi.Input[str] otp: The one-time password for the Proxmox VE API.
+        :param pulumi.Input[str] password: The password for the Proxmox VE API.
+        :param pulumi.Input[pulumi.InputType['ProviderSshArgs']] ssh: The SSH configuration for the Proxmox nodes.
+        :param pulumi.Input[str] username: The username for the Proxmox VE API.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -207,76 +197,77 @@
                  api_token: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  insecure: Optional[pulumi.Input[bool]] = None,
                  otp: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
                  username: Optional[pulumi.Input[str]] = None,
-                 virtual_environment: Optional[pulumi.Input[pulumi.InputType['ProviderVirtualEnvironmentArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["api_token"] = None if api_token is None else pulumi.Output.secret(api_token)
             __props__.__dict__["endpoint"] = endpoint
             __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
+            if otp is not None and not opts.urn:
+                warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+                pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
             __props__.__dict__["otp"] = otp
             __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
             __props__.__dict__["ssh"] = pulumi.Output.from_input(ssh).apply(pulumi.runtime.to_json) if ssh is not None else None
             __props__.__dict__["username"] = username
-            if virtual_environment is not None and not opts.urn:
-                warnings.warn("""Move attributes out of virtual_environment block""", DeprecationWarning)
-                pulumi.log.warn("""virtual_environment is deprecated: Move attributes out of virtual_environment block""")
-            __props__.__dict__["virtual_environment"] = pulumi.Output.from_input(virtual_environment).apply(pulumi.runtime.to_json) if virtual_environment is not None else None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiToken", "password"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'proxmoxve',
             resource_name,
             __props__,
             opts)
 
     @property
     @pulumi.getter(name="apiToken")
     def api_token(self) -> pulumi.Output[Optional[str]]:
         """
-        The API token for the Proxmox Virtual Environment API
+        The API token for the Proxmox VE API.
         """
         return pulumi.get(self, "api_token")
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Output[Optional[str]]:
         """
-        The endpoint for the Proxmox Virtual Environment API
+        The endpoint for the Proxmox VE API.
         """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def otp(self) -> pulumi.Output[Optional[str]]:
         """
-        The one-time password for the Proxmox Virtual Environment API
+        The one-time password for the Proxmox VE API.
         """
+        warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
+
         return pulumi.get(self, "otp")
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Output[Optional[str]]:
         """
-        The password for the Proxmox Virtual Environment API
+        The password for the Proxmox VE API.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Output[Optional[str]]:
         """
-        The username for the Proxmox Virtual Environment API
+        The username for the Proxmox VE API.
         """
         return pulumi.get(self, "username")
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files 12% similar despite different names*

```diff
@@ -141,25 +141,25 @@
     """
     __args__ = dict()
     __args__['nodeName'] = node_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:Storage/getDatastores:getDatastores', __args__, opts=opts, typ=GetDatastoresResult).value
 
     return AwaitableGetDatastoresResult(
-        actives=__ret__.actives,
-        content_types=__ret__.content_types,
-        datastore_ids=__ret__.datastore_ids,
-        enableds=__ret__.enableds,
-        id=__ret__.id,
-        node_name=__ret__.node_name,
-        shareds=__ret__.shareds,
-        space_availables=__ret__.space_availables,
-        space_totals=__ret__.space_totals,
-        space_useds=__ret__.space_useds,
-        types=__ret__.types)
+        actives=pulumi.get(__ret__, 'actives'),
+        content_types=pulumi.get(__ret__, 'content_types'),
+        datastore_ids=pulumi.get(__ret__, 'datastore_ids'),
+        enableds=pulumi.get(__ret__, 'enableds'),
+        id=pulumi.get(__ret__, 'id'),
+        node_name=pulumi.get(__ret__, 'node_name'),
+        shareds=pulumi.get(__ret__, 'shareds'),
+        space_availables=pulumi.get(__ret__, 'space_availables'),
+        space_totals=pulumi.get(__ret__, 'space_totals'),
+        space_useds=pulumi.get(__ret__, 'space_useds'),
+        types=pulumi.get(__ret__, 'types'))
 
 
 @_utilities.lift_output_func(get_datastores)
 def get_datastores_output(node_name: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatastoresResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,25 +561,28 @@
 
 @pulumi.input_type
 class VirtualMachineInitializationArgs:
     def __init__(__self__, *,
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  dns: Optional[pulumi.Input['VirtualMachineInitializationDnsArgs']] = None,
                  ip_configs: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineInitializationIpConfigArgs']]]] = None,
+                 meta_data_file_id: Optional[pulumi.Input[str]] = None,
                  network_data_file_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user_account: Optional[pulumi.Input['VirtualMachineInitializationUserAccountArgs']] = None,
                  user_data_file_id: Optional[pulumi.Input[str]] = None,
                  vendor_data_file_id: Optional[pulumi.Input[str]] = None):
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if dns is not None:
             pulumi.set(__self__, "dns", dns)
         if ip_configs is not None:
             pulumi.set(__self__, "ip_configs", ip_configs)
+        if meta_data_file_id is not None:
+            pulumi.set(__self__, "meta_data_file_id", meta_data_file_id)
         if network_data_file_id is not None:
             pulumi.set(__self__, "network_data_file_id", network_data_file_id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if user_account is not None:
             pulumi.set(__self__, "user_account", user_account)
         if user_data_file_id is not None:
@@ -611,14 +614,23 @@
         return pulumi.get(self, "ip_configs")
 
     @ip_configs.setter
     def ip_configs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineInitializationIpConfigArgs']]]]):
         pulumi.set(self, "ip_configs", value)
 
     @property
+    @pulumi.getter(name="metaDataFileId")
+    def meta_data_file_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "meta_data_file_id")
+
+    @meta_data_file_id.setter
+    def meta_data_file_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "meta_data_file_id", value)
+
+    @property
     @pulumi.getter(name="networkDataFileId")
     def network_data_file_id(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "network_data_file_id")
 
     @network_data_file_id.setter
     def network_data_file_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_data_file_id", value)
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,19 +89,19 @@
     __args__ = dict()
     __args__['nodeName'] = node_name
     __args__['vmId'] = vm_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:VM/getVirtualMachine:getVirtualMachine', __args__, opts=opts, typ=GetVirtualMachineResult).value
 
     return AwaitableGetVirtualMachineResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        node_name=__ret__.node_name,
-        tags=__ret__.tags,
-        vm_id=__ret__.vm_id)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        node_name=pulumi.get(__ret__, 'node_name'),
+        tags=pulumi.get(__ret__, 'tags'),
+        vm_id=pulumi.get(__ret__, 'vm_id'))
 
 
 @_utilities.lift_output_func(get_virtual_machine)
 def get_virtual_machine_output(node_name: Optional[pulumi.Input[str]] = None,
                                vm_id: Optional[pulumi.Input[int]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachineResult]:
     """
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     __args__ = dict()
     __args__['nodeName'] = node_name
     __args__['tags'] = tags
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('proxmoxve:VM/getVirtualMachines:getVirtualMachines', __args__, opts=opts, typ=GetVirtualMachinesResult).value
 
     return AwaitableGetVirtualMachinesResult(
-        id=__ret__.id,
-        node_name=__ret__.node_name,
-        tags=__ret__.tags,
-        vms=__ret__.vms)
+        id=pulumi.get(__ret__, 'id'),
+        node_name=pulumi.get(__ret__, 'node_name'),
+        tags=pulumi.get(__ret__, 'tags'),
+        vms=pulumi.get(__ret__, 'vms'))
 
 
 @_utilities.lift_output_func(get_virtual_machines)
 def get_virtual_machines_output(node_name: Optional[pulumi.Input[Optional[str]]] = None,
                                 tags: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualMachinesResult]:
     """
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,14 +497,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "datastoreId":
             suggest = "datastore_id"
         elif key == "ipConfigs":
             suggest = "ip_configs"
+        elif key == "metaDataFileId":
+            suggest = "meta_data_file_id"
         elif key == "networkDataFileId":
             suggest = "network_data_file_id"
         elif key == "userAccount":
             suggest = "user_account"
         elif key == "userDataFileId":
             suggest = "user_data_file_id"
         elif key == "vendorDataFileId":
@@ -521,25 +523,28 @@
         VirtualMachineInitialization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  datastore_id: Optional[str] = None,
                  dns: Optional['outputs.VirtualMachineInitializationDns'] = None,
                  ip_configs: Optional[Sequence['outputs.VirtualMachineInitializationIpConfig']] = None,
+                 meta_data_file_id: Optional[str] = None,
                  network_data_file_id: Optional[str] = None,
                  type: Optional[str] = None,
                  user_account: Optional['outputs.VirtualMachineInitializationUserAccount'] = None,
                  user_data_file_id: Optional[str] = None,
                  vendor_data_file_id: Optional[str] = None):
         if datastore_id is not None:
             pulumi.set(__self__, "datastore_id", datastore_id)
         if dns is not None:
             pulumi.set(__self__, "dns", dns)
         if ip_configs is not None:
             pulumi.set(__self__, "ip_configs", ip_configs)
+        if meta_data_file_id is not None:
+            pulumi.set(__self__, "meta_data_file_id", meta_data_file_id)
         if network_data_file_id is not None:
             pulumi.set(__self__, "network_data_file_id", network_data_file_id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if user_account is not None:
             pulumi.set(__self__, "user_account", user_account)
         if user_data_file_id is not None:
@@ -559,14 +564,19 @@
 
     @property
     @pulumi.getter(name="ipConfigs")
     def ip_configs(self) -> Optional[Sequence['outputs.VirtualMachineInitializationIpConfig']]:
         return pulumi.get(self, "ip_configs")
 
     @property
+    @pulumi.getter(name="metaDataFileId")
+    def meta_data_file_id(self) -> Optional[str]:
+        return pulumi.get(self, "meta_data_file_id")
+
+    @property
     @pulumi.getter(name="networkDataFileId")
     def network_data_file_id(self) -> Optional[str]:
         return pulumi.get(self, "network_data_file_id")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 5.6.0
+Version: 5.7.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_proxmoxve-5.6.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-5.7.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-5.6.0/setup.py` & `pulumi_proxmoxve-5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.6.0"
-PLUGIN_VERSION = "5.6.0"
+VERSION = "5.7.0"
+PLUGIN_VERSION = "5.7.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'proxmoxve', PLUGIN_VERSION, '--server', 'github://api.github.com/muhlba91/pulumi-proxmoxve'])
         except OSError as error:
```

