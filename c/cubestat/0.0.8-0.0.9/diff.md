# Comparing `tmp/cubestat-0.0.8.tar.gz` & `tmp/cubestat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubestat-0.0.8.tar", last modified: Wed Jun 21 01:52:58 2023, max compression
+gzip compressed data, was "cubestat-0.0.9.tar", last modified: Thu Jun 22 15:22:52 2023, max compression
```

## Comparing `cubestat-0.0.8.tar` & `cubestat-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:58.134715 cubestat-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 01:52:47.000000 cubestat-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 01:52:58.134715 cubestat-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-21 01:52:47.000000 cubestat-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:58.134715 cubestat-0.0.8/cubestat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:47.000000 cubestat-0.0.8/cubestat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16390 2023-06-21 01:52:47.000000 cubestat-0.0.8/cubestat/cubestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:52:58.134715 cubestat-0.0.8/cubestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 01:52:58.000000 cubestat-0.0.8/cubestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:52:58.134715 cubestat-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-21 01:52:47.000000 cubestat-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:22:52.295114 cubestat-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-22 15:22:42.000000 cubestat-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-22 15:22:52.295114 cubestat-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-22 15:22:42.000000 cubestat-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:22:52.291114 cubestat-0.0.9/cubestat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:22:42.000000 cubestat-0.0.9/cubestat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16795 2023-06-22 15:22:42.000000 cubestat-0.0.9/cubestat/cubestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:22:52.295114 cubestat-0.0.9/cubestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-22 15:22:52.000000 cubestat-0.0.9/cubestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-22 15:22:52.000000 cubestat-0.0.9/cubestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:22:52.000000 cubestat-0.0.9/cubestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 15:22:52.000000 cubestat-0.0.9/cubestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 15:22:52.000000 cubestat-0.0.9/cubestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 15:22:52.000000 cubestat-0.0.9/cubestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:22:52.295114 cubestat-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-22 15:22:42.000000 cubestat-0.0.9/setup.py
```

### Comparing `cubestat-0.0.8/LICENSE` & `cubestat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cubestat-0.0.8/README.md` & `cubestat-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -48,20 +48,31 @@
 * UP/DOWN - scroll the lines in case there are more cores.
 
 Running on Apple devices will require sudo access, as `powermetrics` has this limitation. Running on Linux doesn't require it.
 
 Multi-gpu example - training [nano GPT](https://github.com/karpathy/nanoGPT) on 4 nVidia GPU instance:
 ![multigpu](static/multigpu.png)
 
+## Neural Engine utilization
+
+A few notes on 'what does this even represent?'. Utilization we report is essentially power consumption reported by powermetrics.
+To convert it to % we divide it by some 'maximum' value observed in experimentation. There are many drawbacks to this:
+* The concept of 'utilization' overall it pretty ambiguous, e.g. for a x86 CPU - when CPU is wasting cycles on a cache miss, is it 'utilized' or not? If CPU is doing scalar instructions on 1 execution port rather than vectorized instructions on several ports, is it 'utilized' or not?
+* It is unclear if power consumption is a decent proxy for utilization;
+* The upper bound must be different for different models (M1, M1 Max, M2, etc.). Need to identify the model and do tests for them.
+* It is unclear if my tests are actually hitting upperbound. The highest I could achieve was multiple layers of convolutions with no non-linearities between them (which makes model pretty useless)
+
+
 ## Dependencies
 * Python 3.?+
 * psutil 5.9.5
 * pynvml for nVidia cards monitoring
 
 ## TODO
+* Apple Neural Engine correct scale.
 * GPU aggregation
 * CPU by socket/NUMA/SMT
 * status line (why though?)
 * better colors (especially for dark background)
 * multi-column layout for large instances (e.g. with 100+ cores)
 * try on Windows and BSD
 * Google TPU load?
```

### Comparing `cubestat-0.0.8/cubestat/cubestat.py` & `cubestat-0.0.9/cubestat/cubestat.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import curses
 import itertools
 import plistlib
 import subprocess
 import time
 import sys
 import psutil
+import logging
 
 from importlib.util import find_spec
 from enum import Enum
 from math import floor
 from threading import Thread, Lock
 
 class EnumLoop(Enum):
@@ -57,15 +58,15 @@
         'cpu': {},
         'ram': {'RAM used %': psutil.virtual_memory().percent},
         'accelerators': {},
         'disk': {},
         'network': {},
     }
 
-# psutil + nvsmi for nVidia GPU
+# psutil + nvsmi for nVidia GPU if available
 class LinuxReader:
     def __init__(self, interval_ms):
         self.has_nvidia = False
         self.first = True
         self.interval_ms = interval_ms
         try:
             subprocess.check_output('nvidia-smi')
@@ -87,15 +88,15 @@
         nw_load = psutil.net_io_counters()
         nw_read_kb = nw_load.bytes_recv / 2 ** 10
         nw_written_kb = nw_load.bytes_sent / 2 ** 10
         d = self.interval_ms / 1000.0
 
         cpu_clusters = []
 
-        cluster_title = 'Total CPU util %'
+        cluster_title = 'Total CPU Util, %'
         cpu_clusters.append(cluster_title)
         total_load = 0.0
         res['cpu'][cluster_title] = 0.0
 
         cpu_load = psutil.cpu_percent(percpu=True)
         for i, v in enumerate(cpu_load):
             title = f'CPU {i} util %'
@@ -123,19 +124,26 @@
         res['network']['network i KB/s'] = ((nw_read_kb - self.network_read_last) / d)
         res['network']['network w KB/s'] = ((nw_written_kb - self.network_written_last) / d)
         self.network_read_last = nw_read_kb
         self.network_written_last = nw_written_kb
         return res.items(), cpu_clusters
 
 class AppleReader:
-    def __init__(self, interval_ms) -> None:
-        self.interval_ms = interval_ms
+    # these scalers are based on running mock convnet from scripts/apple_loadgen.py
+    ane_power_scalers_mw = {
+        'Mac14,2': 15000.0, # M2 MacBook Air
+        'Macmini9,1': 13000.0, # M1 Mac Mini
+    }
+
+    def __init__(self) -> None:
+        pass
 
     def read(self, snapshot):
         res = snapshot_base()
+        hw_model = snapshot["hw_model"]
 
         cpu_clusters = []
         for cluster in snapshot['processor']['clusters']:
             idle_cluster, total_cluster = 0.0, 0.0
             cluster_title = f'{cluster["name"]} total CPU util %'
             cpu_clusters.append(cluster_title)
             res['cpu'][cluster_title] = 0.0
@@ -143,15 +151,18 @@
                 title = f'{cluster["name"]} CPU {cpu["cpu"]} util %'
                 res['cpu'][title] = 100.0 - 100.0 * cpu['idle_ratio']
                 idle_cluster += cpu['idle_ratio']
                 total_cluster += 1.0
             res['cpu'][cluster_title] = 100.0 - 100.0 * idle_cluster / total_cluster
 
         res['accelerators']['GPU util %'] = 100.0 - 100.0 * snapshot['gpu']['idle_ratio']
-        ane_scaling = 8.0 * self.interval_ms
+        
+        # TODO: this is likely different for different models. Need to run some tests.
+        # Scaler 15000.0 is based on testing on M2
+        ane_scaling = AppleReader.ane_power_scalers_mw.get(hw_model, 15000.0)
         res['accelerators']['ANE util %'] = 100.0 * snapshot['processor']['ane_energy'] / ane_scaling
 
         res['disk']['disk read'] = snapshot['disk']['rbytes_per_s']
         res['disk']['disk write'] = snapshot['disk']['wbytes_per_s']
         res['network']['network rx'] = snapshot['network']['ibyte_rate']
         res['network']['network tx'] = snapshot['network']['obyte_rate']
         return res.items(), cpu_clusters
@@ -378,15 +389,15 @@
 
     def loop(self, reader, *args):
         reader_thread = Thread(target=reader, daemon=True, args=args)
         reader_thread.start()
         self.render_loop()
 
 def start_apple(stdscr, powermetrics, firstline):
-    h = Horizon(stdscr, AppleReader(args.refresh_ms))
+    h = Horizon(stdscr, AppleReader())
     h.loop(h.reader_loop_apple, powermetrics, firstline)
 
 def start_linux(stdscr):
     h = Horizon(stdscr, LinuxReader(args.refresh_ms))
     h.loop(h.reader_loop_linux)
 
 def main():
```

### Comparing `cubestat-0.0.8/setup.py` & `cubestat-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cubestat',
-    version='0.0.8',
+    version='0.0.9',
     author='Oleksandr Kuvshynov',
     author_email='okuvshynov@gmail.com',
     description='Horizon chart in terminal for system monitoring',
     long_description='Horizon chart in terminal. Supports CPU/GPU/ANE/RAM/IO monitoring for Apple M1/M2, nVidia GPUs',
     packages=find_packages(),
     install_requires=[
         'psutil>=5.9.5',
```

