# Comparing `tmp/fluxoperator-0.0.29.tar.gz` & `tmp/fluxoperator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.29.tar", last modified: Fri Jun 23 19:56:51 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.3.tar", last modified: Sun Jun 25 05:43:07 2023, max compression
```

## Comparing `fluxoperator-0.0.29.tar` & `fluxoperator-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.193840 fluxoperator-0.0.29/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-23 19:56:51.193840 fluxoperator-0.0.29/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.185840 fluxoperator-0.0.29/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2005 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.185840 fluxoperator-0.0.29/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13678 2023-06-23 19:56:45.000000 fluxoperator-0.0.29/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.189840 fluxoperator-0.0.29/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1529 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8265 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8718 2023-06-23 19:56:45.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.189840 fluxoperator-0.0.29/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6151 2023-06-21 05:22:14.000000 fluxoperator-0.0.29/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.185840 fluxoperator-0.0.29/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2719 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1975 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.29/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-23 19:56:51.000000 fluxoperator-0.0.29/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-23 19:56:51.197841 fluxoperator-0.0.29/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:56:51.193840 fluxoperator-0.0.29/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-23 19:39:55.000000 fluxoperator-0.0.29/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1266 2023-06-14 19:07:03.000000 fluxoperator-0.0.29/test/test_network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.29/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2816 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2173 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13767 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1697 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4552 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/bursted_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4674 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/bursting.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6193 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/flux_broker.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13103 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-06-25 05:13:07.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8150 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16961 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8718 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3714 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6890 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.065711 fluxoperator-0.0.3/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2816 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2157 2023-06-25 05:43:07.000000 fluxoperator-0.0.3/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.3/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-06-25 05:43:06.000000 fluxoperator-0.0.3/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2152 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:43:07.069711 fluxoperator-0.0.3/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:13:08.000000 fluxoperator-0.0.3/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1352 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_bursted_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1831 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_bursting.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1341 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_flux_broker.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1234 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7553 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3352 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16512 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11270 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1773 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-06-25 05:43:00.000000 fluxoperator-0.0.3/test/test_network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.3/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.29/PKG-INFO` & `fluxoperator-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.29
+Version: 0.0.3
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -74,17 +74,20 @@
 import time
 import fluxoperator
 from pprint import pprint
 ```
 
 ## Documentation For Models
 
+ - [BurstedCluster](BurstedCluster.md)
+ - [Bursting](Bursting.md)
  - [Commands](Commands.md)
  - [ContainerResources](dContainerResources.md)
  - [ContainerVolume](ContainerVolume.md)
+ - [FluxBroker](FluxBrokerl.md)
  - [FluxRestful](FluxRestful.md)
  - [FluxSpec](FluxSpec.md)
  - [FluxUser](FluxUser.md)
  - [LifeCycle](LifeCycle.md)
  - [LoggingSpec](LoggingSpec.md)
  - [MiniCluster](MiniCluster.md)
  - [MiniClusterArchive](MiniClusterArchive.md)
```

### Comparing `fluxoperator-0.0.29/fluxoperator/__init__.py` & `fluxoperator-0.0.3/fluxoperator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 from fluxoperator.exceptions import OpenApiException
 from fluxoperator.exceptions import ApiTypeError
 from fluxoperator.exceptions import ApiValueError
 from fluxoperator.exceptions import ApiKeyError
 from fluxoperator.exceptions import ApiAttributeError
 from fluxoperator.exceptions import ApiException
 # import models into sdk package
+from fluxoperator.models.bursted_cluster import BurstedCluster
+from fluxoperator.models.bursting import Bursting
 from fluxoperator.models.commands import Commands
 from fluxoperator.models.container_resources import ContainerResources
 from fluxoperator.models.container_volume import ContainerVolume
+from fluxoperator.models.flux_broker import FluxBroker
 from fluxoperator.models.flux_restful import FluxRestful
 from fluxoperator.models.flux_spec import FluxSpec
 from fluxoperator.models.flux_user import FluxUser
 from fluxoperator.models.life_cycle import LifeCycle
 from fluxoperator.models.logging_spec import LoggingSpec
 from fluxoperator.models.mini_cluster import MiniCluster
 from fluxoperator.models.mini_cluster_archive import MiniClusterArchive
```

### Comparing `fluxoperator-0.0.29/fluxoperator/api_client.py` & `fluxoperator-0.0.3/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/client.py` & `fluxoperator-0.0.3/fluxoperator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,16 @@
 
     @property
     def core_v1(self):
         """
         Instantiate a core_v1 api (if not done yet)
 
         We have this here because we typically need to create the MiniCluster
-        first.
+        first. For a custom core_v1_api, provide core_c1_api to the FluxOperator
+        init function.
         """
         if self._core_v1 is not None:
             return self._core_v1
 
         self.c = client.Configuration.get_default_copy()
         self.c.assert_hostname = False
         client.Configuration.set_default(self.c)
```

### Comparing `fluxoperator-0.0.29/fluxoperator/configuration.py` & `fluxoperator-0.0.3/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/decorator.py` & `fluxoperator-0.0.3/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/exceptions.py` & `fluxoperator-0.0.3/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/__init__.py` & `fluxoperator-0.0.3/fluxoperator/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,17 +10,20 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
+from fluxoperator.models.bursted_cluster import BurstedCluster
+from fluxoperator.models.bursting import Bursting
 from fluxoperator.models.commands import Commands
 from fluxoperator.models.container_resources import ContainerResources
 from fluxoperator.models.container_volume import ContainerVolume
+from fluxoperator.models.flux_broker import FluxBroker
 from fluxoperator.models.flux_restful import FluxRestful
 from fluxoperator.models.flux_spec import FluxSpec
 from fluxoperator.models.flux_user import FluxUser
 from fluxoperator.models.life_cycle import LifeCycle
 from fluxoperator.models.logging_spec import LoggingSpec
 from fluxoperator.models.mini_cluster import MiniCluster
 from fluxoperator.models.mini_cluster_archive import MiniClusterArchive
```

### Comparing `fluxoperator-0.0.29/fluxoperator/models/commands.py` & `fluxoperator-0.0.3/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.3/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.3/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.3/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_status.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,210 +14,212 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from fluxoperator.configuration import Configuration
 
 
-class FluxSpec(object):
+class MiniClusterStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'connect_timeout': 'str',
-        'install_root': 'str',
-        'log_level': 'int',
-        'minimal_service': 'bool',
-        'option_flags': 'str',
-        'wrap': 'str'
+        'completed': 'bool',
+        'conditions': 'list[V1Condition]',
+        'jobid': 'str',
+        'maximum_size': 'int',
+        'selector': 'str',
+        'size': 'int'
     }
 
     attribute_map = {
-        'connect_timeout': 'connectTimeout',
-        'install_root': 'installRoot',
-        'log_level': 'logLevel',
-        'minimal_service': 'minimalService',
-        'option_flags': 'optionFlags',
-        'wrap': 'wrap'
+        'completed': 'completed',
+        'conditions': 'conditions',
+        'jobid': 'jobid',
+        'maximum_size': 'maximumSize',
+        'selector': 'selector',
+        'size': 'size'
     }
 
-    def __init__(self, connect_timeout='5s', install_root='/usr', log_level=6, minimal_service=False, option_flags='', wrap=None, local_vars_configuration=None):  # noqa: E501
-        """FluxSpec - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, completed=False, conditions=None, jobid='', maximum_size=0, selector='', size=0, local_vars_configuration=None):  # noqa: E501
+        """MiniClusterStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._connect_timeout = None
-        self._install_root = None
-        self._log_level = None
-        self._minimal_service = None
-        self._option_flags = None
-        self._wrap = None
+        self._completed = None
+        self._conditions = None
+        self._jobid = None
+        self._maximum_size = None
+        self._selector = None
+        self._size = None
         self.discriminator = None
 
-        if connect_timeout is not None:
-            self.connect_timeout = connect_timeout
-        if install_root is not None:
-            self.install_root = install_root
-        if log_level is not None:
-            self.log_level = log_level
-        if minimal_service is not None:
-            self.minimal_service = minimal_service
-        if option_flags is not None:
-            self.option_flags = option_flags
-        if wrap is not None:
-            self.wrap = wrap
+        if completed is not None:
+            self.completed = completed
+        if conditions is not None:
+            self.conditions = conditions
+        self.jobid = jobid
+        self.maximum_size = maximum_size
+        self.selector = selector
+        self.size = size
 
     @property
-    def connect_timeout(self):
-        """Gets the connect_timeout of this FluxSpec.  # noqa: E501
+    def completed(self):
+        """Gets the completed of this MiniClusterStatus.  # noqa: E501
 
-        Single user executable to provide to flux start  # noqa: E501
+        Label to indicate that job is completed, comes from Job.Completed The user can also look at conditions -> JobFinished  # noqa: E501
 
-        :return: The connect_timeout of this FluxSpec.  # noqa: E501
-        :rtype: str
+        :return: The completed of this MiniClusterStatus.  # noqa: E501
+        :rtype: bool
         """
-        return self._connect_timeout
+        return self._completed
 
-    @connect_timeout.setter
-    def connect_timeout(self, connect_timeout):
-        """Sets the connect_timeout of this FluxSpec.
+    @completed.setter
+    def completed(self, completed):
+        """Sets the completed of this MiniClusterStatus.
 
-        Single user executable to provide to flux start  # noqa: E501
+        Label to indicate that job is completed, comes from Job.Completed The user can also look at conditions -> JobFinished  # noqa: E501
 
-        :param connect_timeout: The connect_timeout of this FluxSpec.  # noqa: E501
-        :type connect_timeout: str
+        :param completed: The completed of this MiniClusterStatus.  # noqa: E501
+        :type completed: bool
         """
 
-        self._connect_timeout = connect_timeout
+        self._completed = completed
 
     @property
-    def install_root(self):
-        """Gets the install_root of this FluxSpec.  # noqa: E501
+    def conditions(self):
+        """Gets the conditions of this MiniClusterStatus.  # noqa: E501
 
-        Install root location  # noqa: E501
+        conditions hold the latest Flux Job and MiniCluster states  # noqa: E501
 
-        :return: The install_root of this FluxSpec.  # noqa: E501
-        :rtype: str
+        :return: The conditions of this MiniClusterStatus.  # noqa: E501
+        :rtype: list[V1Condition]
         """
-        return self._install_root
+        return self._conditions
 
-    @install_root.setter
-    def install_root(self, install_root):
-        """Sets the install_root of this FluxSpec.
+    @conditions.setter
+    def conditions(self, conditions):
+        """Sets the conditions of this MiniClusterStatus.
 
-        Install root location  # noqa: E501
+        conditions hold the latest Flux Job and MiniCluster states  # noqa: E501
 
-        :param install_root: The install_root of this FluxSpec.  # noqa: E501
-        :type install_root: str
+        :param conditions: The conditions of this MiniClusterStatus.  # noqa: E501
+        :type conditions: list[V1Condition]
         """
 
-        self._install_root = install_root
+        self._conditions = conditions
 
     @property
-    def log_level(self):
-        """Gets the log_level of this FluxSpec.  # noqa: E501
+    def jobid(self):
+        """Gets the jobid of this MiniClusterStatus.  # noqa: E501
 
-        Log level to use for flux logging (only in non TestMode)  # noqa: E501
+        The Jobid is set internally to associate to a miniCluster This isn't currently in use, we only have one!  # noqa: E501
 
-        :return: The log_level of this FluxSpec.  # noqa: E501
-        :rtype: int
+        :return: The jobid of this MiniClusterStatus.  # noqa: E501
+        :rtype: str
         """
-        return self._log_level
+        return self._jobid
 
-    @log_level.setter
-    def log_level(self, log_level):
-        """Sets the log_level of this FluxSpec.
+    @jobid.setter
+    def jobid(self, jobid):
+        """Sets the jobid of this MiniClusterStatus.
 
-        Log level to use for flux logging (only in non TestMode)  # noqa: E501
+        The Jobid is set internally to associate to a miniCluster This isn't currently in use, we only have one!  # noqa: E501
 
-        :param log_level: The log_level of this FluxSpec.  # noqa: E501
-        :type log_level: int
+        :param jobid: The jobid of this MiniClusterStatus.  # noqa: E501
+        :type jobid: str
         """
+        if self.local_vars_configuration.client_side_validation and jobid is None:  # noqa: E501
+            raise ValueError("Invalid value for `jobid`, must not be `None`")  # noqa: E501
 
-        self._log_level = log_level
+        self._jobid = jobid
 
     @property
-    def minimal_service(self):
-        """Gets the minimal_service of this FluxSpec.  # noqa: E501
+    def maximum_size(self):
+        """Gets the maximum_size of this MiniClusterStatus.  # noqa: E501
 
-        Only expose the broker service (to reduce load on DNS)  # noqa: E501
+        We keep the original size of the MiniCluster request as this is the absolute maximum  # noqa: E501
 
-        :return: The minimal_service of this FluxSpec.  # noqa: E501
-        :rtype: bool
+        :return: The maximum_size of this MiniClusterStatus.  # noqa: E501
+        :rtype: int
         """
-        return self._minimal_service
+        return self._maximum_size
 
-    @minimal_service.setter
-    def minimal_service(self, minimal_service):
-        """Sets the minimal_service of this FluxSpec.
+    @maximum_size.setter
+    def maximum_size(self, maximum_size):
+        """Sets the maximum_size of this MiniClusterStatus.
 
-        Only expose the broker service (to reduce load on DNS)  # noqa: E501
+        We keep the original size of the MiniCluster request as this is the absolute maximum  # noqa: E501
 
-        :param minimal_service: The minimal_service of this FluxSpec.  # noqa: E501
-        :type minimal_service: bool
+        :param maximum_size: The maximum_size of this MiniClusterStatus.  # noqa: E501
+        :type maximum_size: int
         """
+        if self.local_vars_configuration.client_side_validation and maximum_size is None:  # noqa: E501
+            raise ValueError("Invalid value for `maximum_size`, must not be `None`")  # noqa: E501
 
-        self._minimal_service = minimal_service
+        self._maximum_size = maximum_size
 
     @property
-    def option_flags(self):
-        """Gets the option_flags of this FluxSpec.  # noqa: E501
+    def selector(self):
+        """Gets the selector of this MiniClusterStatus.  # noqa: E501
 
-        Flux option flags, usually provided with -o optional - if needed, default option flags for the server These can also be set in the user interface to override here. This is only valid for a FluxRunner \"runFlux\" true  # noqa: E501
 
-        :return: The option_flags of this FluxSpec.  # noqa: E501
+        :return: The selector of this MiniClusterStatus.  # noqa: E501
         :rtype: str
         """
-        return self._option_flags
+        return self._selector
 
-    @option_flags.setter
-    def option_flags(self, option_flags):
-        """Sets the option_flags of this FluxSpec.
+    @selector.setter
+    def selector(self, selector):
+        """Sets the selector of this MiniClusterStatus.
 
-        Flux option flags, usually provided with -o optional - if needed, default option flags for the server These can also be set in the user interface to override here. This is only valid for a FluxRunner \"runFlux\" true  # noqa: E501
 
-        :param option_flags: The option_flags of this FluxSpec.  # noqa: E501
-        :type option_flags: str
+        :param selector: The selector of this MiniClusterStatus.  # noqa: E501
+        :type selector: str
         """
+        if self.local_vars_configuration.client_side_validation and selector is None:  # noqa: E501
+            raise ValueError("Invalid value for `selector`, must not be `None`")  # noqa: E501
 
-        self._option_flags = option_flags
+        self._selector = selector
 
     @property
-    def wrap(self):
-        """Gets the wrap of this FluxSpec.  # noqa: E501
+    def size(self):
+        """Gets the size of this MiniClusterStatus.  # noqa: E501
 
-        Commands for flux start --wrap  # noqa: E501
+        These are for the sub-resource scale functionality  # noqa: E501
 
-        :return: The wrap of this FluxSpec.  # noqa: E501
-        :rtype: str
+        :return: The size of this MiniClusterStatus.  # noqa: E501
+        :rtype: int
         """
-        return self._wrap
+        return self._size
 
-    @wrap.setter
-    def wrap(self, wrap):
-        """Sets the wrap of this FluxSpec.
+    @size.setter
+    def size(self, size):
+        """Sets the size of this MiniClusterStatus.
 
-        Commands for flux start --wrap  # noqa: E501
+        These are for the sub-resource scale functionality  # noqa: E501
 
-        :param wrap: The wrap of this FluxSpec.  # noqa: E501
-        :type wrap: str
+        :param size: The size of this MiniClusterStatus.  # noqa: E501
+        :type size: int
         """
+        if self.local_vars_configuration.client_side_validation and size is None:  # noqa: E501
+            raise ValueError("Invalid value for `size`, must not be `None`")  # noqa: E501
 
-        self._wrap = wrap
+        self._size = size
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -253,18 +255,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FluxSpec):
+        if not isinstance(other, MiniClusterStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, FluxSpec):
+        if not isinstance(other, MiniClusterStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fluxoperator-0.0.29/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.3/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.3/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.3/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.3/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/network.py` & `fluxoperator-0.0.3/fluxoperator/models/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.3/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/models/security_context.py` & `fluxoperator-0.0.3/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/resource/network.py` & `fluxoperator-0.0.3/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator/resource/pods.py` & `fluxoperator-0.0.3/fluxoperator/resource/pods.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 from kubernetes import client, config
 import fluxoperator.models as models
 
 import fluxoperator.defaults as defaults
 import sys
 
 # These are known objects we will parse
-_objects = ["logging", "volumes", "resources", "flux_restful", "container", "resources", "flux"]
+_objects = [
+    "logging",
+    "volumes",
+    "resources",
+    "flux_restful",
+    "container",
+    "resources",
+    "flux",
+]
 
 
 def _get_logging_spec(logging):
     """
     Return models.Logging
     """
     logging_defaults = {
@@ -37,25 +45,49 @@
         volume_spec = {}
         for attr in models.ContainerVolume.attribute_map:
             if attr in volume:
                 volume_spec[attr] = volume[attr]
         volumeset[name] = models.ContainerVolume(**volume_spec)
     return volumeset
 
+def _get_bursting_spec(bursting):
+    """
+    Get the bursting spec
+    """
+    burstspec = {}
+    for k in models.Bursting.attribute_map:
+        if k in bursting and k == "lead_broker":
+            burstspec[k] = _get_lead_broker_spec(bursting[k])
+        elif k in bursting:
+            burstspec[k] = bursting[k]
+    return models.Bursting(**burstspec)
+
+def _get_lead_broker_spec(broker):
+    """
+    Get the lead broker spec
+    """
+    brokerspec = {}
+    for k in models.FluxBroker.attribute_map:
+        if k in broker:
+            brokerspec[k] = broker[k]
+    return models.FluxBroker(**brokerspec)
 
 def _get_flux_spec(flux):
     """
     Get flux spec
     """
     fluxspec = {}
     for k in models.FluxSpec.attribute_map:
-        if k in flux:
+        if k in flux and k == "bursting":
+            fluxspec[k] = _get_bursting_spec(flux[k])
+        elif k in flux:
             fluxspec[k] = flux[k]
     return models.FluxSpec(**fluxspec)
 
+
 def _get_container_spec(container):
     """
     Get the container spec.
     """
     # For now only one container support, it must run Flux
     container_kwargs = {"run_flux": True}
     for k in models.MiniClusterContainer.attribute_map:
```

### Comparing `fluxoperator-0.0.29/fluxoperator/rest.py` & `fluxoperator-0.0.3/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.3/fluxoperator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.29
+Version: 0.0.3
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -74,17 +74,20 @@
 import time
 import fluxoperator
 from pprint import pprint
 ```
 
 ## Documentation For Models
 
+ - [BurstedCluster](BurstedCluster.md)
+ - [Bursting](Bursting.md)
  - [Commands](Commands.md)
  - [ContainerResources](dContainerResources.md)
  - [ContainerVolume](ContainerVolume.md)
+ - [FluxBroker](FluxBrokerl.md)
  - [FluxRestful](FluxRestful.md)
  - [FluxSpec](FluxSpec.md)
  - [FluxUser](FluxUser.md)
  - [LifeCycle](LifeCycle.md)
  - [LoggingSpec](LoggingSpec.md)
  - [MiniCluster](MiniCluster.md)
  - [MiniClusterArchive](MiniClusterArchive.md)
```

### Comparing `fluxoperator-0.0.29/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.3/fluxoperator.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 fluxoperator.egg-info/SOURCES.txt
 fluxoperator.egg-info/dependency_links.txt
 fluxoperator.egg-info/not-zip-safe
 fluxoperator.egg-info/requires.txt
 fluxoperator.egg-info/top_level.txt
 fluxoperator/api/__init__.py
 fluxoperator/models/__init__.py
+fluxoperator/models/bursted_cluster.py
+fluxoperator/models/bursting.py
 fluxoperator/models/commands.py
 fluxoperator/models/container_resources.py
 fluxoperator/models/container_volume.py
+fluxoperator/models/flux_broker.py
 fluxoperator/models/flux_restful.py
 fluxoperator/models/flux_spec.py
 fluxoperator/models/flux_user.py
 fluxoperator/models/life_cycle.py
 fluxoperator/models/logging_spec.py
 fluxoperator/models/mini_cluster.py
 fluxoperator/models/mini_cluster_archive.py
@@ -37,17 +40,20 @@
 fluxoperator/models/network.py
 fluxoperator/models/pod_spec.py
 fluxoperator/models/security_context.py
 fluxoperator/resource/__init__.py
 fluxoperator/resource/network.py
 fluxoperator/resource/pods.py
 test/__init__.py
+test/test_bursted_cluster.py
+test/test_bursting.py
 test/test_commands.py
 test/test_container_resources.py
 test/test_container_volume.py
+test/test_flux_broker.py
 test/test_flux_restful.py
 test/test_flux_spec.py
 test/test_flux_user.py
 test/test_life_cycle.py
 test/test_logging_spec.py
 test/test_mini_cluster.py
 test/test_mini_cluster_archive.py
```

### Comparing `fluxoperator-0.0.29/setup.py` & `fluxoperator-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.29",
+        version="0.0.3",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.29/test/test_commands.py` & `fluxoperator-0.0.3/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_container_resources.py` & `fluxoperator-0.0.3/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_container_volume.py` & `fluxoperator-0.0.3/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_flux_restful.py` & `fluxoperator-0.0.3/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_flux_spec.py` & `fluxoperator-0.0.3/test/test_flux_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,38 +15,36 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.flux_spec import FluxSpec  # noqa: E501
 from fluxoperator.rest import ApiException
 
+
 class TestFluxSpec(unittest.TestCase):
     """FluxSpec unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test FluxSpec
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
         # model = fluxoperator.models.flux_spec.FluxSpec()  # noqa: E501
-        if include_optional :
-            return FluxSpec(
-                connect_timeout = '5s', 
-                option_flags = ''
-            )
-        else :
-            return FluxSpec(
-        )
+        if include_optional:
+            return FluxSpec(connect_timeout="5s", option_flags="")
+        else:
+            return FluxSpec()
 
     def testFluxSpec(self):
         """Test FluxSpec"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_flux_user.py` & `fluxoperator-0.0.3/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_life_cycle.py` & `fluxoperator-0.0.3/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_logging_spec.py` & `fluxoperator-0.0.3/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.3/test/test_bursted_cluster.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,40 +12,41 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import fluxoperator
-from fluxoperator.models.mini_cluster_archive import MiniClusterArchive  # noqa: E501
+from fluxoperator.models.bursted_cluster import BurstedCluster  # noqa: E501
 from fluxoperator.rest import ApiException
 
-class TestMiniClusterArchive(unittest.TestCase):
-    """MiniClusterArchive unit test stubs"""
+class TestBurstedCluster(unittest.TestCase):
+    """BurstedCluster unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test MiniClusterArchive
+        """Test BurstedCluster
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = fluxoperator.models.mini_cluster_archive.MiniClusterArchive()  # noqa: E501
+        # model = fluxoperator.models.bursted_cluster.BurstedCluster()  # noqa: E501
         if include_optional :
-            return MiniClusterArchive(
-                path = ''
+            return BurstedCluster(
+                name = '', 
+                size = 56
             )
         else :
-            return MiniClusterArchive(
+            return BurstedCluster(
         )
 
-    def testMiniClusterArchive(self):
-        """Test MiniClusterArchive"""
+    def testBurstedCluster(self):
+        """Test BurstedCluster"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.3/test/test_mini_cluster_existing_volume.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import fluxoperator
-from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume  # noqa: E501
+from fluxoperator.models.mini_cluster_existing_volume import (
+    MiniClusterExistingVolume,
+)  # noqa: E501
 from fluxoperator.rest import ApiException
 
+
 class TestMiniClusterExistingVolume(unittest.TestCase):
     """MiniClusterExistingVolume unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterExistingVolume
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
         # model = fluxoperator.models.mini_cluster_existing_volume.MiniClusterExistingVolume()  # noqa: E501
-        if include_optional :
+        if include_optional:
+            return MiniClusterExistingVolume(claim_name="", path="", read_only=True)
+        else:
             return MiniClusterExistingVolume(
-                claim_name = '', 
-                path = '', 
-                read_only = True
+                claim_name="",
+                path="",
             )
-        else :
-            return MiniClusterExistingVolume(
-                claim_name = '',
-                path = '',
-        )
 
     def testMiniClusterExistingVolume(self):
         """Test MiniClusterExistingVolume"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_mini_cluster_status.py` & `fluxoperator-0.0.3/test/test_mini_cluster_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,43 +15,39 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus  # noqa: E501
 from fluxoperator.rest import ApiException
 
+
 class TestMiniClusterStatus(unittest.TestCase):
     """MiniClusterStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterStatus
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
         # model = fluxoperator.models.mini_cluster_status.MiniClusterStatus()  # noqa: E501
-        if include_optional :
+        if include_optional:
+            return MiniClusterStatus(conditions=[None], jobid="", maximum_size=56)
+        else:
             return MiniClusterStatus(
-                conditions = [
-                    None
-                    ], 
-                jobid = '', 
-                maximum_size = 56
+                jobid="",
+                maximum_size=56,
             )
-        else :
-            return MiniClusterStatus(
-                jobid = '',
-                maximum_size = 56,
-        )
 
     def testMiniClusterStatus(self):
         """Test MiniClusterStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_mini_cluster_user.py` & `fluxoperator-0.0.3/test/test_mini_cluster_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,39 +15,38 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.mini_cluster_user import MiniClusterUser  # noqa: E501
 from fluxoperator.rest import ApiException
 
+
 class TestMiniClusterUser(unittest.TestCase):
     """MiniClusterUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterUser
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
         # model = fluxoperator.models.mini_cluster_user.MiniClusterUser()  # noqa: E501
-        if include_optional :
+        if include_optional:
+            return MiniClusterUser(name="", password="")
+        else:
             return MiniClusterUser(
-                name = '', 
-                password = ''
+                name="",
             )
-        else :
-            return MiniClusterUser(
-                name = '',
-        )
 
     def testMiniClusterUser(self):
         """Test MiniClusterUser"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.3/test/test_mini_cluster_volume.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,57 +15,51 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.mini_cluster_volume import MiniClusterVolume  # noqa: E501
 from fluxoperator.rest import ApiException
 
+
 class TestMiniClusterVolume(unittest.TestCase):
     """MiniClusterVolume unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterVolume
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
         # model = fluxoperator.models.mini_cluster_volume.MiniClusterVolume()  # noqa: E501
-        if include_optional :
+        if include_optional:
             return MiniClusterVolume(
-                annotations = {
-                    'key' : ''
-                    }, 
-                attributes = {
-                    'key' : ''
-                    }, 
-                capacity = '5Gi', 
-                claim_annotations = {
-                    'key' : ''
-                    }, 
-                delete = True, 
-                driver = '', 
-                labels = {
-                    'key' : ''
-                    }, 
-                path = '', 
-                secret = '', 
-                secret_namespace = 'default', 
-                storage_class = 'hostpath', 
-                volume_handle = ''
+                annotations={"key": ""},
+                attributes={"key": ""},
+                capacity="5Gi",
+                claim_annotations={"key": ""},
+                delete=True,
+                driver="",
+                labels={"key": ""},
+                path="",
+                secret="",
+                secret_namespace="default",
+                storage_class="hostpath",
+                volume_handle="",
             )
-        else :
+        else:
             return MiniClusterVolume(
-                path = '',
-        )
+                path="",
+            )
 
     def testMiniClusterVolume(self):
         """Test MiniClusterVolume"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_network.py` & `fluxoperator-0.0.3/test/test_network.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,37 +15,36 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.network import Network  # noqa: E501
 from fluxoperator.rest import ApiException
 
+
 class TestNetwork(unittest.TestCase):
     """Network unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test Network
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
+        include_option is a boolean, when False only required
+        params are included, when True both required and
+        optional params are included"""
         # model = fluxoperator.models.network.Network()  # noqa: E501
-        if include_optional :
-            return Network(
-                headless_name = 'flux-service'
-            )
-        else :
-            return Network(
-        )
+        if include_optional:
+            return Network(headless_name="flux-service")
+        else:
+            return Network()
 
     def testNetwork(self):
         """Test Network"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `fluxoperator-0.0.29/test/test_pod_spec.py` & `fluxoperator-0.0.3/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.29/test/test_security_context.py` & `fluxoperator-0.0.3/test/test_security_context.py`

 * *Files identical despite different names*

