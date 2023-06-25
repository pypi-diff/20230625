# Comparing `tmp/pyjs8call-0.2.0.tar.gz` & `tmp/pyjs8call-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjs8call-0.2.0.tar", last modified: Wed Mar 22 20:03:51 2023, max compression
+gzip compressed data, was "pyjs8call-0.2.1.tar", last modified: Sun Jun 25 19:48:17 2023, max compression
```

## Comparing `pyjs8call-0.2.0.tar` & `pyjs8call-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-03-22 20:03:51.621863 pyjs8call-0.2.0/
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     1119 2022-12-28 23:29:29.000000 pyjs8call-0.2.0/LICENSE
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    12280 2023-03-22 20:03:51.621863 pyjs8call-0.2.0/PKG-INFO
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    11672 2023-03-22 19:47:19.000000 pyjs8call-0.2.0/README.md
-drwxrwxr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-03-22 20:03:51.621863 pyjs8call-0.2.0/pyjs8call/
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     1889 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/__init__.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     9406 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/appmonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    64162 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/client.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    16635 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/confighandler.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     6034 2023-02-17 15:42:31.000000 pyjs8call-0.2.0/pyjs8call/hbnetwork.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     2656 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/idlemonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    14588 2023-02-17 15:42:31.000000 pyjs8call-0.2.0/pyjs8call/inboxmonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    24706 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/js8call.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    27603 2023-02-17 15:42:31.000000 pyjs8call-0.2.0/pyjs8call/message.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    14658 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/offsetmonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     6204 2023-02-17 15:42:31.000000 pyjs8call-0.2.0/pyjs8call/outgoingmonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)     7727 2023-02-17 15:42:31.000000 pyjs8call-0.2.0/pyjs8call/spotmonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    20333 2023-02-17 15:42:31.000000 pyjs8call-0.2.0/pyjs8call/timemonitor.py
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    10533 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/pyjs8call/windowmonitor.py
-drwxrwxr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-03-22 20:03:51.621863 pyjs8call-0.2.0/pyjs8call.egg-info/
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)    12280 2023-03-22 20:03:51.000000 pyjs8call-0.2.0/pyjs8call.egg-info/PKG-INFO
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)      532 2023-03-22 20:03:51.000000 pyjs8call-0.2.0/pyjs8call.egg-info/SOURCES.txt
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)        1 2023-03-22 20:03:51.000000 pyjs8call-0.2.0/pyjs8call.egg-info/dependency_links.txt
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)       12 2023-03-22 20:03:51.000000 pyjs8call-0.2.0/pyjs8call.egg-info/requires.txt
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)       10 2023-03-22 20:03:51.000000 pyjs8call-0.2.0/pyjs8call.egg-info/top_level.txt
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)       38 2023-03-22 20:03:51.621863 pyjs8call-0.2.0/setup.cfg
--rw-rw-r--   0 otisbyron  (1000) otisbyron  (1000)      821 2023-03-17 21:10:35.000000 pyjs8call-0.2.0/setup.py
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-06-25 19:48:17.211603 pyjs8call-0.2.1/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1119 2022-12-26 14:28:50.000000 pyjs8call-0.2.1/LICENSE
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    13528 2023-06-25 19:48:17.211603 pyjs8call-0.2.1/PKG-INFO
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    12955 2023-06-09 16:36:37.000000 pyjs8call-0.2.1/README.md
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-06-25 19:48:17.201604 pyjs8call-0.2.1/pyjs8call/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1897 2023-06-04 23:57:51.000000 pyjs8call-0.2.1/pyjs8call/__init__.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    10801 2023-06-07 23:43:03.000000 pyjs8call-0.2.1/pyjs8call/appmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    78673 2023-06-21 16:43:09.000000 pyjs8call-0.2.1/pyjs8call/client.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    17875 2023-06-08 02:22:48.000000 pyjs8call-0.2.1/pyjs8call/confighandler.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     6242 2023-06-03 22:03:44.000000 pyjs8call-0.2.1/pyjs8call/hbnetwork.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    15042 2023-06-07 22:13:30.000000 pyjs8call-0.2.1/pyjs8call/inboxmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    25902 2023-06-23 23:15:14.000000 pyjs8call-0.2.1/pyjs8call/js8call.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    30064 2023-06-24 00:36:13.000000 pyjs8call-0.2.1/pyjs8call/message.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    15050 2023-06-04 17:37:40.000000 pyjs8call-0.2.1/pyjs8call/offsetmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     7382 2023-06-24 00:36:40.000000 pyjs8call-0.2.1/pyjs8call/outgoingmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    12420 2023-06-25 19:15:45.000000 pyjs8call-0.2.1/pyjs8call/schedulemonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     8487 2023-06-12 16:45:12.000000 pyjs8call-0.2.1/pyjs8call/spotmonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    21157 2023-06-03 22:03:44.000000 pyjs8call-0.2.1/pyjs8call/timemonitor.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    10696 2023-06-03 22:03:44.000000 pyjs8call-0.2.1/pyjs8call/windowmonitor.py
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-06-25 19:48:17.201604 pyjs8call-0.2.1/pyjs8call.egg-info/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)    13528 2023-06-25 19:48:16.000000 pyjs8call-0.2.1/pyjs8call.egg-info/PKG-INFO
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)      607 2023-06-25 19:48:17.000000 pyjs8call-0.2.1/pyjs8call.egg-info/SOURCES.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)        1 2023-06-25 19:48:16.000000 pyjs8call-0.2.1/pyjs8call.egg-info/dependency_links.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       12 2023-06-25 19:48:16.000000 pyjs8call-0.2.1/pyjs8call.egg-info/requires.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       10 2023-06-25 19:48:16.000000 pyjs8call-0.2.1/pyjs8call.egg-info/top_level.txt
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)       38 2023-06-25 19:48:17.211603 pyjs8call-0.2.1/setup.cfg
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)      823 2023-06-08 01:26:06.000000 pyjs8call-0.2.1/setup.py
+drwxr-xr-x   0 otisbyron  (1000) otisbyron  (1000)        0 2023-06-25 19:48:17.211603 pyjs8call-0.2.1/tests/
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     3971 2023-05-27 00:16:28.000000 pyjs8call-0.2.1/tests/test_cross_platform.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1672 2023-02-25 18:49:44.000000 pyjs8call-0.2.1/tests/test_helpers.py
+-rw-r--r--   0 otisbyron  (1000) otisbyron  (1000)     1222 2023-02-25 22:19:38.000000 pyjs8call-0.2.1/tests/test_start.py
```

### Comparing `pyjs8call-0.2.0/LICENSE` & `pyjs8call-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjs8call-0.2.0/PKG-INFO` & `pyjs8call-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyjs8call
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for interfacing with the JS8Call API
 Home-page: https://github.com/simplyequipped/pyjs8call
 Author: Simply Equipped LLC
 Author-email: howard@simplyequipped.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
+Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pypi version](https://img.shields.io/pypi/v/pyjs8call?color=blue&label=pypi%20version)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![pypi downloads](https://img.shields.io/pypi/dw/pyjs8call?color=blue&label=pypi%20downloads)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![github license](https://img.shields.io/github/license/simplyequipped/pyjs8call?color=blue)](https://github.com/simplyequipped/pyjs8call/blob/main/LICENSE)
 
@@ -135,17 +133,17 @@
 
 Time master functionality is also implemented which sends outgoing messages on a time interval that other stations can use to synchronize their time drift. Targets the @TIME group by default.
 
 **Inbox Monitor** (pyjs8call.inboxmonitor)
 
 Monitors the local inbox. Notification of new messages is handled via callback function.
 
-**Idle Monitor** (pyjs8call.idlemonitor)
+**Schedule Monitor** (pyjs8call.schedulemonitor)
 
-Monitors the JS8Call application process run time and restarts the application perodically (when there is no outgoing activity) to avoid the JS8Call idle timeout. This is useful when running the JS8Call application headless.
+Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile.
 
 &nbsp;  
 
 ### Examples
 
 Basic usage:
 ```
@@ -183,14 +181,32 @@
 js8call.spots.filter(distance = 1000)
 
 # get a list of spot messages in the last 15 minutes
 max_age = 15 * 60 # convert minutes to seconds
 js8call.spots.filter(age = max_age)
 ```
 
+Run multiple JS8Call instances:
+```
+import pyjs8call
+
+# Option A: use the standard network port and no rig name for the primary instance
+js8call = pyjs8call.Client()
+js8call.start()
+
+# Option B: specify a network port and rig name for the primary instance
+#js8call_ft857 = pyjs8call.Client(port=2443)
+#js8call_ft857.start(args=['--rig-name', 'FT857'])
+
+# specify a different network port for the secondary instance
+js8call_qdx = pyjs8call.Client(port=2444)
+# specify the rig name as a command line argument
+js8call_qdx.start(args=['--rig-name', 'QDX'])
+```
+
 Using the spot monitor:
 ```
 import pyjs8call
 
 # callback function for all new spots
 def new_spots(spots):
     for spot in spots:
@@ -235,15 +251,15 @@
 
 js8call = pyjs8call.Client()
 # set inbox monitor callback
 js8call.callback.inbox = new_inbox_msg
 js8call.start()
 
 # enable local inbox monitoring and periodic remote inbox message query
-js8call.inbox.enable_monitoring()
+js8call.inbox.enable()
 ```
 
 Using the outgoing message monitor:
 ```
 import pyjs8call
 
 # callback function for message status change
@@ -268,15 +284,42 @@
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
 js8call.start()
 
 # use default 10 minute interval
-js8call.heartbeat.enable_networking()
+js8call.heartbeat.enable()
+```
+
+Using the schedule monitor:
+```
+import pyjs8call
+
+# callback function for schedule entry activation
+def schedule_activation(schedule_entry):
+    print('Activating ' + repr(schedule_entry))
+
+js8call = pyjs8call.Client()
+# set schedule activation callback
+js8call.callbacks.schedule = schedule_activation
+js8call.start()
+
+# return to the current configuration later
+js8call.schedule.add('14:00')
+# change configuration profile and set frequency and modem speed
+js8call.schedule.add('8:00', 7078000, 'normal', 'QDX')
+# change frequency only
+js8call.schedule.add('9:00', 7074000)
+# remove schedule entry
+js8call.schedule.remove('9:00')
+
+# print formatted information for each schedule entry
+for entry in js8call.schedule.get_schedule():
+    print(str(entry))
 ```
 
 Set config file settings:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
@@ -315,9 +358,7 @@
 ### Acknowledgements
 
 Inspired by [js8net](https://github.com/jfrancis42/js8net) by N0GQ<br>
 [JS8Call](http://js8call.com) by KN4CRD
 
 &nbsp;
 
-
-
```

### Comparing `pyjs8call-0.2.0/README.md` & `pyjs8call-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -117,17 +117,17 @@
 
 Time master functionality is also implemented which sends outgoing messages on a time interval that other stations can use to synchronize their time drift. Targets the @TIME group by default.
 
 **Inbox Monitor** (pyjs8call.inboxmonitor)
 
 Monitors the local inbox. Notification of new messages is handled via callback function.
 
-**Idle Monitor** (pyjs8call.idlemonitor)
+**Schedule Monitor** (pyjs8call.schedulemonitor)
 
-Monitors the JS8Call application process run time and restarts the application perodically (when there is no outgoing activity) to avoid the JS8Call idle timeout. This is useful when running the JS8Call application headless.
+Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile.
 
 &nbsp;  
 
 ### Examples
 
 Basic usage:
 ```
@@ -165,14 +165,32 @@
 js8call.spots.filter(distance = 1000)
 
 # get a list of spot messages in the last 15 minutes
 max_age = 15 * 60 # convert minutes to seconds
 js8call.spots.filter(age = max_age)
 ```
 
+Run multiple JS8Call instances:
+```
+import pyjs8call
+
+# Option A: use the standard network port and no rig name for the primary instance
+js8call = pyjs8call.Client()
+js8call.start()
+
+# Option B: specify a network port and rig name for the primary instance
+#js8call_ft857 = pyjs8call.Client(port=2443)
+#js8call_ft857.start(args=['--rig-name', 'FT857'])
+
+# specify a different network port for the secondary instance
+js8call_qdx = pyjs8call.Client(port=2444)
+# specify the rig name as a command line argument
+js8call_qdx.start(args=['--rig-name', 'QDX'])
+```
+
 Using the spot monitor:
 ```
 import pyjs8call
 
 # callback function for all new spots
 def new_spots(spots):
     for spot in spots:
@@ -217,15 +235,15 @@
 
 js8call = pyjs8call.Client()
 # set inbox monitor callback
 js8call.callback.inbox = new_inbox_msg
 js8call.start()
 
 # enable local inbox monitoring and periodic remote inbox message query
-js8call.inbox.enable_monitoring()
+js8call.inbox.enable()
 ```
 
 Using the outgoing message monitor:
 ```
 import pyjs8call
 
 # callback function for message status change
@@ -250,15 +268,42 @@
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
 js8call.start()
 
 # use default 10 minute interval
-js8call.heartbeat.enable_networking()
+js8call.heartbeat.enable()
+```
+
+Using the schedule monitor:
+```
+import pyjs8call
+
+# callback function for schedule entry activation
+def schedule_activation(schedule_entry):
+    print('Activating ' + repr(schedule_entry))
+
+js8call = pyjs8call.Client()
+# set schedule activation callback
+js8call.callbacks.schedule = schedule_activation
+js8call.start()
+
+# return to the current configuration later
+js8call.schedule.add('14:00')
+# change configuration profile and set frequency and modem speed
+js8call.schedule.add('8:00', 7078000, 'normal', 'QDX')
+# change frequency only
+js8call.schedule.add('9:00', 7074000)
+# remove schedule entry
+js8call.schedule.remove('9:00')
+
+# print formatted information for each schedule entry
+for entry in js8call.schedule.get_schedule():
+    print(str(entry))
 ```
 
 Set config file settings:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
```

### Comparing `pyjs8call-0.2.0/pyjs8call/__init__.py` & `pyjs8call-0.2.1/pyjs8call/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 __docformat__ = 'google'
 
 
 from pyjs8call.offsetmonitor import OffsetMonitor
 from pyjs8call.confighandler import ConfigHandler
 from pyjs8call.hbnetwork import HeartbeatNetworking
-from pyjs8call.idlemonitor import IdleMonitor
+from pyjs8call.schedulemonitor import ScheduleMonitor
 from pyjs8call.spotmonitor import SpotMonitor
 from pyjs8call.appmonitor import AppMonitor
 from pyjs8call.message import Message
 # modules importing message module
 from pyjs8call.windowmonitor import WindowMonitor
 from pyjs8call.inboxmonitor import InboxMonitor
 from pyjs8call.timemonitor import DriftMonitor
```

### Comparing `pyjs8call-0.2.0/pyjs8call/appmonitor.py` & `pyjs8call-0.2.1/pyjs8call/appmonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,31 @@
 '''
 
 __docformat__ = 'google'
 
 
 import time
 import threading
-import signal
 import shutil
 import subprocess
 
 import psutil
 
 
 class AppMonitor:
     '''JS8Call application monitor.
 
+    If the JS8Call application is closed and *restart* is *False*, pyjs8call will exit. If *restart* is *True* pyjs8call will continue to run and JS8Call will be restarted.
+
+
+
     Attributes:
         headless (bool): Whether JS8Call is running headless using xvfb (see *start()*)
-        restart (bool): Whether to restart the JS8Call application if it stops, defaults to True
+        args (list): Sequence of command line arguments to be passed to JS8Call, defaults to empty list
+        restart (bool): Whether to restart the JS8Call application if it stops, defaults to False
     '''
 
     def __init__(self, parent):
         '''Initialize JS8Call application monitor.
 
         Args:
             parent (pyjs8call.js8call): The parent js8call object
@@ -54,31 +58,40 @@
         Returns:
             pyjs8call.appmonitor.AppMonitor: Constructed application monitor object
         '''
         self._parent = parent
         self._xvfb_proc = None
         self._js8call_proc = None
         self.headless = False
-        self.restart = True
+        self.args = []
+        self.restart = False
 
-    def start(self, headless=False):
+    def start(self, headless=False, args=None):
         ''' Start JS8Call application.
 
+        See the subprocess.Popen *args* parameter documentation for information on how to break command line arguments into a sequence. The *js8call* command does not need to be included, only additional arguments. For example, passing `['--rig-name', 'FT857']` as the *args* parameter results in `js8call --rig-name FT857` being called to start the JS8Call application. Note that *args* only applies if JS8Call is started by pyjs8call.
+
         Args:
             headless (bool): Run JS8Call headless using xvfb (Linux only, requires xvfb to be installed), defaults to False
+            args (list): Sequence of command line arguments to be passed to JS8Call, defaults to None
 
         Raises:
             RuntimeError: JS8Call is not installed
             RuntimeError: Cannot run headless on Windows, xvfb is not supported
             RuntimeError: Attempting to run application headless and xvfb not installed
             RuntimeError: JS8Call application failed to start
         '''
         if self.is_running():
             return
 
+        if args is None:
+            self.args = []
+        else:
+            self.args = args
+
         if headless:
             self._start_xvfb()
         else:
             self._start_js8call()
 
         time.sleep(1)
 
@@ -150,31 +163,36 @@
     def _start_xvfb(self):
         '''Start JS8Call application headless via xvfb.
         
         Raises:
             RuntimeError: Cannot run headless on Windows, xvfb is not supported
             RuntimeError: Attempting to run application headless and xvfb not installed
             RuntimeError: JS8Call application not installed
+            RuntimeError: JS8Call application failed to start
         '''
         xvfb_exec_path = shutil.which('xvfb-run')
         js8call_exec_path = shutil.which('js8call')
 
         if psutil.WINDOWS:
             raise RuntimeError('Cannot run headless on Windows, xvfb is not supported')
         if xvfb_exec_path is None:
             raise RuntimeError('Cannot run headless without xvfb installed, on Debian systems try: sudo apt install xvfb')
         if js8call_exec_path is None:
             raise RuntimeError('JS8Call application not installed')
 
-        # check if js8call already running via xvfb
-        self._find_running_xvfb_process()
+        if self.args == []:
+            # check if js8call already running via xvfb
+            self._find_running_xvfb_process()
 
         # proc not set if not already running
         if self._xvfb_proc is None:
-            self._xvfb_proc = psutil.Popen([xvfb_exec_path, '-a', js8call_exec_path], stderr = subprocess.DEVNULL)
+            exec_path = [xvfb_exec_path, '-a', js8call_exec_path]
+            exec_path.extend(self.args)
+
+            self._xvfb_proc = psutil.Popen(exec_path, stderr = subprocess.DEVNULL)
         
         # wait until socket connected or timeout
         if self._socket_connected():
             # find js8call child process under xvfb
             for child in self._xvfb_proc.children():
                 if child.name().lower() == 'js8call':
                     self._js8call_proc = child
@@ -196,49 +214,53 @@
             RuntimeError: JS8Call application failed to start
         '''
         js8call_exec_path = shutil.which('js8call')
 
         if js8call_exec_path is None:
             raise RuntimeError('JS8Call application not installed')
 
-        # check if js8call already running
-        self._find_running_js8call_process()
+        if self.args == []:
+            # check if js8call already running
+            self._find_running_js8call_process()
 
         # proc not set if not already running
         if self._js8call_proc is None:
-            self._js8call_proc = psutil.Popen([js8call_exec_path], stderr = subprocess.DEVNULL)
+            exec_path = [js8call_exec_path]
+            exec_path.extend(self.args)
+
+            self._js8call_proc = psutil.Popen(exec_path, stderr = subprocess.DEVNULL)
 
         # wait until socket connected or timeout
         if self._socket_connected():
             # start js8call monitoring thread
             thread = threading.Thread(target=self._monitor)
             thread.daemon = True
             thread.start()
         else:
             raise RuntimeError('JS8Call application failed to start')
 
-    def _socket_connected(self, timeout=60):
+    def _socket_connected(self, timeout=120):
         '''Wait for JS8Call socket connection after starting application.
         
         Args:
-            timeout (int): Number of seconds to wait for socket to connect, defaults to 60
+            timeout (int): Number of seconds to wait for connection, defaults to 120
             
         Returns:
             bool: True if socket connected, False otherwise
         '''
         if self._parent.connected:
             return True
 
         timeout += time.time()
 
         while True:
             try:
-                # error if unable to connect
+                # connection refused error if unable to connect
                 self._parent.connect()
-                # no errors, connected
+                # no errors, socket connected
                 return True
             except ConnectionRefusedError:
                 pass
 
             if time.time() > timeout:
                 break
 
@@ -272,12 +294,16 @@
                 
             self._js8call_proc = proc
             return
 
     def _monitor(self):
         '''Application monitoring thread.'''
         while self._parent.online:
-            if not self.is_running() and self.restart:
-                # restart the whole system and reconnect
-                self._parent._client.restart()
+            if not self.is_running() and not self._parent._client.restarting:
+                if self.restart:
+                    # restart the whole system and reconnect
+                    self._parent._client.restart()
+                
+                else:
+                    psutil.Process().terminate()
 
             time.sleep(1)
```

### Comparing `pyjs8call-0.2.0/pyjs8call/client.py` & `pyjs8call-0.2.1/pyjs8call/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,118 +36,191 @@
     ```
 '''
 
 __docformat__ = 'google'
 
 
 import time
+import shutil
 import atexit
 import threading
 from datetime import datetime, timezone
 from math import radians, sin, cos, acos, atan2, pi
 
 import pyjs8call
 from pyjs8call import Message
 
 
 class Client:
     '''JS8Call API client.
+    
+    
+    **Caution**: Custom processing of messages is an advanced feature that can break internal message handling if implemented incorrectly. Use this feature only if you understand what you are doing.
+    **Note**: Any delay in *process_incoming* and *process_outgoing* functions will cause delays in internal incoming and outgoing message processing loops. Custom processing should be kept to a minimum to avoid cumulative delays.
+    
+    Custom Incoming Message Processing:
+    
+    The *process_incoming* function is called after internal processing of an incoming message from the JS8Call application, but before adding the message to the incoming message queue.
+    
+    *process_incoming* should accept a pyjs8call.message object, and return a pyjs8call.message object. If an error occurs during processing, either:
+        - set the *msg.error* string before returning the message, which will cause the message to continue processing and be added to the incoming message queue
+        OR
+        - return None, which will cause the message to be dropped
+    
+    *process_incoming* function signatures:
+        `func(pyjs8call.Message) -> pyjs8call.Message`
+        `func(pyjs8call.Message) -> None`
+
+    Custom Outgoing Message Processing:
+    
+    The *process_outgoing* function is called just after message creation in the following functions:
+        - send_message
+        - send_directed_message
+        - send_directed_command_message
+    
+    *process_outgoing* should accept a pyjs8call.message object, and return a pyjs8call.message object. If an error occurs during processing:
+        - set the *msg.error* string, which will cause the message to be returned with a failed status (the message will not be sent)
+    
+    *process_outoing* function signature:
+        `func(pyjs8call.message) -> pyjs8call.message`
+    
 
     Attributes:
         js8call (pyjs8call.js8call): Manages JS8Call application and TCP socket communication
         spots (pyjs8call.spotmonitor): Monitors station activity and issues callbacks
         window (pyjs8call.windowmonitor): Monitors the JS8Call transmit window
         offset (pyjs8call.offsetmonitor): Manages JS8Call offset frequency
         outgoing (pyjs8call.outgoingmonitor): Monitors JS8Call outgoing message text
-        drift (pyjs8call.timemonitor): Monitors JS8Call time drift
+        drift_sync (pyjs8call.timemonitor): Monitors JS8Call time drift
         time_master (pyjs8call.timemonitor): Manages time master outgoing messages
         inbox (pyjs8call.inboxmonitor): Monitors JS8Call inbox messages
         config (pyjs8call.confighandler): Manages JS8Call configuration file
         heartbeat (pyjs8call.hbnetwork): Manages heartbeat outgoing messages
-        idle (pyjs8call.idlemonitor): Monitors the JS8Call idle timeout
+        schedule (pyjs8call.schedulemonitor): Monitors and activates schedule entries
         callback (pyjs8call.client.Callbacks): Callback function reference object
         settings (pyjs8call.client.Settings): Configuration setting function reference object
         clean_directed_text (bool): Remove JS8Call callsign structure from incoming messages, defaults to True
         monitor_outgoing (bool): Monitor outgoing message status (see pyjs8call.outgoingmonitor), defaults to True
         online (bool): Whether the JS8Call application and pyjs8call interface are online
         host (str): IP address matching JS8Call *TCP Server Hostname* setting
         port (int): Port number matching JS8Call *TCP Server Port* setting
+        process_incoming (func): Function to call for custom processing of incoming messages, defaults to None
+        process_outgoing (func): Function to call for custom processing of outgoing messages, defaults to None
     '''
 
     def __init__(self, host='127.0.0.1', port=2442, config_path=None):
         '''Initialize JS8Call API client.
 
         Registers the Client.stop function with the atexit module.
         
         Configures the following settings:
         - enable autoreply at startup
         - disable autoreply confirmation
         - enable transmit
 
+        Initializes the following for access prior to starting:
+        - js8call (pyjs8call.js8call)
+        - config (pyjs8call.confighandler)
+        - settings (pyjs8call.client.settings)
+        - callback (pyjs8call.client.callbacks)
+
         Args:
             host (str): JS8Call TCP address setting, defaults to '127.0.0.1'
             port (int): JS8Call TCP port setting, defaults to 2442
             config_path (str): Non-standard JS8Call.ini configuration file path, defaults to None
 
         Returns:
             pyjs8call.client: Constructed client object
+
+        Raises:
+            RuntimeError: JS8Call application not installed
         '''
         self.host = host
         self.port = port
+        self.online = False
+        self.restarting = False
+        self.process_incoming = None
+        self.process_outgoing = None
         self.clean_directed_text = True
         self.monitor_outgoing = True
-        self.online = False
 
         self.js8call = None
         self.spots = None
         self.window = None
         self.offset = None
         self.outgoing = None
-        self.drift = None
+        self.drift_sync = None
         self.time_master = None
         self.inbox = None
         self.heartbeat = None
-        self.idle = None
+        self.schedule = None
 
         # delay between setting value and getting updated value
         self._set_get_delay = 0.1 # seconds
 
+        # ensure js8call application is installed
+        if shutil.which('js8call') is None:
+            raise RuntimeError('JS8Call application not installed')
+
         self.config = pyjs8call.ConfigHandler(config_path = config_path)
         self.settings = Settings(self)
         self.callback = Callbacks()
+        self.js8call = pyjs8call.JS8Call(self, self.host, self.port)
 
         # stop application and client at exit
         atexit.register(self.stop)
         
-    def start(self, headless=False, debugging=False, logging=False):
+    def start(self, headless=False, args=None, debugging=False, logging=False):
         '''Start and connect to the the JS8Call application.
 
         Initializes sub-module objects:
         - Spot monitor (see pyjs8call.spotmonitor)
         - Window monitor (see pyjs8call.windowmonitor)
         - Offset monitor (see pyjs8call.offsetmonitor)
         - Outgoing monitor (see pyjs8call.outgoingmonitor)
         - Time drift monitor (see pyjs8call.timemonitor)
         - Time master (see pyjs8call.timemonitor)
         - Heartbeat networking (see pyjs8call.hbnetwork)
-        - Inbox master (see pyjs8call.inboxmonitor)
-        - Idle monitor (see pyjs8call.idlemonitor)
+        - Inbox monitor (see pyjs8call.inboxmonitor)
+        - Schedule monitor (see pyjs8call.schedulemonitor)
 
         Adds the @TIME group to JS8Call via the config file to enable drift monitor features.
 
         If logging is enabled the log file will be stored in the current user's *HOME* directory.
 
+        if *args* contains the rig name switch (-r or --rig-name) the rig name is used to instantiate the rig specific config file before launching. Changes to the config object prior to calling *start* are saved to the rig specifc file only, and are not written to the main config file.
+
         Args:
             headless (bool): Run JS8Call headless via xvfb (Linux only)
+            args (list): Command line arguments (see appmonitor.start()), defaults to None
             debugging (bool): Print message data to the console, defaults to False
             logging (bool): Print message data to ~/pyjs8call.log, defaults to False
 
         Raises:
             RuntimeError: JS8Call config file section does not exist (likely because JS8Call has not been run and configured after installation)
         '''
+        if args is None:
+            args = []
+        else:
+            rig_name = None
+
+            # try to find the rig name switch, and then the following rig name
+            try:
+                rig_name = args[args.index('-r') + 1]
+            except ValueError:
+                pass
+
+            try:
+                rig_name = args[args.index('--rig-name') + 1]
+            except ValueError:
+                pass
+
+            if rig_name is not None:
+                self.config.load_rig_config(rig_name)
+
         try:
             self.settings.enable_autoreply_startup()
             self.settings.disable_autoreply_confirmation()
             self.settings.enable_transmit()
             # enable JS8Call TCP connection
             self.config.set('Configuration', 'TCPEnabled', 'true')
             self.config.set('Configuration', 'TCPServer', self.host)
@@ -157,16 +230,15 @@
             self.config.add_group('@TIME')
             self.config.write()
         except RuntimeError as e:
             raise RuntimeError('Try launching JS8Call, configuring audio and CAT interfaces as needed, '
                                'and then exiting the application normally. When the application '
                                'exits normally the first time it will initialize the config file.') from e
 
-        self.js8call = pyjs8call.JS8Call(self, self.host, self.port)
-        self.js8call.start(headless = headless)
+        self.js8call.start(headless = headless, args = args)
         self.online = True
 
         if debugging:
             self.js8call.enable_debugging()
 
         if logging:
             self.js8call.enable_logging()
@@ -176,66 +248,90 @@
         rx_thread.start()
         time.sleep(1)
 
         self.window = pyjs8call.WindowMonitor(self)
         self.spots = pyjs8call.SpotMonitor(self)
         self.offset = pyjs8call.OffsetMonitor(self)
         self.outgoing = pyjs8call.OutgoingMonitor(self)
-        self.drift = pyjs8call.DriftMonitor(self)
+        self.drift_sync = pyjs8call.DriftMonitor(self)
         self.time_master = pyjs8call.TimeMaster(self)
         self.heartbeat = pyjs8call.HeartbeatNetworking(self)
         self.inbox = pyjs8call.InboxMonitor(self)
-        self.idle = pyjs8call.IdleMonitor(self)
+        self.schedule = pyjs8call.ScheduleMonitor(self)
         
-        self.window.enable_monitoring()
-        self.spots.enable_monitoring()
-        self.offset.enable_monitoring()
-        self.outgoing.enable_monitoring()
+        self.window.enable()
+        self.spots.enable()
+        self.offset.enable()
+        self.outgoing.enable()
+        self.schedule.enable()
 
     def stop(self):
         '''Stop all threads, close the TCP socket, and kill the JS8Call application.'''
         self.online = False
-        self.idle.disable_monitoring()
         
         try:
             return self.js8call.stop()
         except Exception:
             pass
 
     def restart(self):
         '''Stop and restart the JS8Call application and the associated TCP socket.
 
         pyjs8call.js8call settings are preserved.
         '''
+        self.restarting = True
+
+        # pause module loops to prevent errors
+        modules = [
+            self.outgoing,
+            self.offset,
+            self.inbox,
+            self.heartbeat,
+            self.drift_sync,
+            self.time_master,
+            self.spots,
+            self.schedule
+        ]
+
+        paused_modules = []
+
+        for module in modules:
+            if module.enabled() and not module.paused():
+                module.pause()
+                paused_modules.append(module)
+
         # write any pending config file changes, convience
         self.config.write()
+        # reeset window monitoring
+        self.window.reset()
         # save settings
-        settings = self.js8call.restart_settings()
         headless = self.js8call.app.headless
-        idle_monitoring_enabled = self.idle.enabled()
+        args = self.js8call.app.args
+        settings = self.js8call.restart_settings()
 
         # stop
         self.stop()
-        time.sleep(0.25)
 
         # start
         self.js8call = pyjs8call.JS8Call(self, self.host, self.port)
-        self.js8call.start(headless = headless)
+        # restore settings
+        self.js8call.reinitialize(settings)
+        self.js8call.start(headless = headless, args = args)
         self.online = True
 
         rx_thread = threading.Thread(target=self._rx)
         rx_thread.daemon = True
         rx_thread.start()
         time.sleep(0.5)
 
-        # restore settings
-        self.js8call.reinitialize(settings)
-        # re-enable idle timeout monitoring
-        if idle_monitoring_enabled:
-            self.idle.enable_monitoring()
+        # resume paused module loops
+        for module in paused_modules:
+            module.resume()
+
+        self.restarting = False
 
     def restart_when_inactive(self, age=0):
         '''Restart the JS8Call application once there is no outgoing activity.
         
         This function is non-blocking due to the use of *threading.Thread* internally.
         
         See *pyjs8call.js8call.activity()* for more details.
@@ -282,21 +378,27 @@
         '''Get the state of the connection to the JS8Call application.
 
         Returns:
             bool: State of connection to JS8Call application
         '''
         return self.js8call.connected
 
-    def identities(self):
+    def identities(self, hb = False):
         '''Get identities associated with local stations.
         
+        Args:
+            hb (bool): Whether to include the @HB group in identity list, defaults to False
         Returns:
             list: Configured callsign and custom groups
         '''
         ids = self.config.get_groups()
+        
+        if hb and '@HB' not in ids:
+            ids.append('@HB')
+            
         ids.append(self.settings.get_station_callsign())
         return ids
     
     def msg_is_to_me(self, msg):
         '''Determine if specified message is addressed to local station.
         
         Utilizes *msg.is_directed_to()* and *client.identities()* internally.
@@ -355,73 +457,103 @@
         msg.set('text', message)
         return msg
     
     def send_message(self, message):
         '''Send a raw JS8Call message.
         
         Message format: *MESSAGE*
+        
+        *process_outgoing* is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             message (str): Message text to send
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
         # msg.type = Message.TX_SEND_MESSAGE by default
         msg = Message(value = message)
+        
+        # custom processing of outgoing messages
+        if self.process_outgoing is not None:
+            msg = self.process_outgoing(msg)
+
+            if msg.error is not None:
+                msg.set('status', Message.STATUS_FAILED)
+                return msg
 
         if self.monitor_outgoing:
             self.outgoing.monitor(msg)
 
         self.js8call.send(msg)
         return msg
 
     def send_directed_command_message(self, destination, command, message=None):
         '''Send a directed JS8Call command message.
 
         Message format: *DESTINATION**COMMAND* *MESSAGE*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
+        
+        *process_outgoing* is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the message to
             command (str): Command to include in message (see *pyjs8call.message* static commands)
             message (str): Message text to send, defaults to None
         '''
         # msg.type = Message.TX_SEND_MESSAGE by default
         msg = Message(destination, command, message)
+        
+        # custom processing of outgoing messages
+        if self.process_outgoing is not None:
+            msg = self.process_outgoing(msg)
+
+            if msg.error is not None:
+                msg.set('status', Message.STATUS_FAILED)
+                return msg
 
         if self.monitor_outgoing:
             self.outgoing.monitor(msg)
-
+            
         self.js8call.send(msg)
         return msg
     
     def send_directed_message(self, destination, message):
         '''Send a directed JS8Call message.
         
         Message format: *DESTINATION* *MESSAGE*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
+        
+        *process_outgoing* is called just after message object creation, if set. If *msg.error* is set after custom processing, the message object is returned with a failed status and without being sent.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the message to
             message (str): Message text to send
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
         # msg.type = Message.TX_SEND_MESSAGE by default
         msg = Message(destination = destination, value = message)
+        
+        # custom processing of outgoing messages
+        if self.process_outgoing is not None:
+            msg = self.process_outgoing(msg)
+
+            if msg.error is not None:
+                msg.set('status', Message.STATUS_FAILED)
+                return msg
 
         if self.monitor_outgoing:
             self.outgoing.monitor(msg)
 
         self.js8call.send(msg)
         return msg
 
@@ -430,15 +562,15 @@
 
         Note that JS8Call will only transmit API messages at the selected offset. Heartbeat messages can still be sent, but will not be in the heartbeat sub-band.
 
         Message format: @HB HEARTBEAT *GRID*
 
         If no grid square is given the configured JS8Call grid square is used.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             grid (str): Grid square (truncated to 4 characters), defaults to None
 
         Returns:
             pyjs8call.message: Constructed messsage object
         '''
@@ -456,15 +588,15 @@
     def send_aprs_grid(self, grid=None):
         '''Send a JS8Call message with APRS grid square.
         
         Message format: @APRSIS GRID *GRID*
 
         If no grid square is given the configured JS8Call grid square is used.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             grid (str): Grid square (trucated to 4 characters), defaults to None
 
         Returns:
             pyjs8call.message: Constructed messsage object
 
@@ -481,15 +613,15 @@
         return self.send_directed_command_message('@APRSIS', Message.CMD_GRID, grid)
 
     def send_aprs_sms(self, phone, message):
         '''Send a JS8Call APRS message via a SMS gateway.
         
         Message format: @APRSIS CMD :SMSGATE&nbsp;&nbsp;&nbsp;:@1234567890 *MESSAGE*
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             phone (str): Phone number to send SMS message to
             message (str): Message to be sent via SMS message
 
         Returns:
             pyjs8call.message: Constructed message object
@@ -499,15 +631,15 @@
         return self.send_directed_command_message('@APRSIS', Message.CMD_CMD, message)
     
     def send_aprs_email(self, email, message):
         '''Send a JS8Call APRS message via an e-mail gateway.
         
         Message format: @APRSIS CMD :EMAIL-2&nbsp;&nbsp;&nbsp;:EMAIL@DOMAIN.COM *MESSAGE*
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             email (str): Email address to send message to
             message (str): Message to be sent via email
 
         Returns:
             pyjs8call.message: Constructed message object
@@ -518,15 +650,15 @@
     def send_aprs_pota_spot(self, park, freq, mode, message, callsign=None):
         '''Send JS8Call APRS POTA spot message.
         
         Message format: @APRSIS CMD :POTAGW&nbsp;&nbsp;&nbsp;:*CALLSIGN* *PARK* *FREQ* *MODE* *MESSAGE*
 
         JS8Call configured callsign is used if no callsign is given.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             park (str): Name of park being activated
             freq (int): Frequency (in kHz) being used for park activation
             mode (str): Radio operating mode used for park activation
             message (str): Message to be sent with POTA spot
             callsign (str): Callsign of operator activating the park, defaults to None
@@ -582,15 +714,15 @@
     def send_inbox_message(self, destination, message):
         '''Send JS8Call inbox message.
 
         Message format: *DESTINATION* MSG *MESSAGE*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the message to
             message (str): Message text to send
 
         Returns:
             pyjs8call.message: Constructed message object
@@ -599,16 +731,16 @@
 
     def store_remote_inbox_message(self, remote, destination, message):
         '''Send JS8Call inbox message to be forwarded.
 
         Message format: *REMOTE* MSG TO:*DESTINATION* *MESSAGE*
 
         If *remote* is a list of callsigns they will be joined in the specified order and sent as a relay.
-
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             remote (str, list): Callsign of intermediate station storing the message
             destination (str): Callsign of message recipient
             message (str): Message text to send
 
         Returns:
@@ -630,41 +762,41 @@
         msg = Message()
         msg.set('type', Message.INBOX_STORE_MESSAGE)
         msg.set('params', {'CALLSIGN': destination, 'TEXT': message})
         self.js8call.send(msg)
         time.sleep(self._set_get_delay)
         return self.get_inbox_messages()
 
-    def query_call(self, destination, callsign):
+    def query_call(self, callsign, destination='@ALLCALL'):
         '''Send JS8Call callsign query.
         
         Message format: *DESTINATION* QUERY CALL *CALLSIGN*?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
-            destination (str, list): Callsign(s) to direct the query to
             callsign (str): Callsign to query for
+            destination (str, list): Callsign(s) to direct the query to, defaults to @ALLCALL
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
         message = callsign + Message.CMD_Q
         return self.send_directed_command_message(destination, Message.CMD_QUERY_CALL, message)
 
     def query_messages(self, destination='@ALLCALL'):
         '''Send JS8Call stored message query.
         
         Message format: *DESTINATION* QUERY MSGS
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to, defaults to '@ALLCALL'
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
@@ -673,15 +805,15 @@
     def query_message_id(self, destination, msg_id):
         '''Send JS8Call stored message ID query.
         
         Message format: *DESTINATION* QUERY MSG *ID*
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
             msg_id (str): Message ID to query for
 
         Returns:
             pyjs8call.message: Constructed message object
@@ -692,15 +824,15 @@
     def query_hearing(self, destination):
         '''Send JS8Call hearing query.
         
         Message format: *DESTINATION* HEARING?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
@@ -709,15 +841,15 @@
     def query_snr(self, destination):
         '''Send JS8Call SNR query.
         
         Message format: *DESTINATION* SNR?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
@@ -726,15 +858,15 @@
     def query_grid(self, destination):
         '''Send JS8Call grid query.
         
         Message format: *DESTINATION* GRID?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
@@ -743,15 +875,15 @@
     def query_info(self, destination):
         '''Send JS8Call info query.
         
         Message format: *DESTINATION* INFO?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
 
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
@@ -759,85 +891,159 @@
 
     def query_status(self, destination):
         '''Send JS8Call status query.
         
         Message format: *DESTINATION* STATUS?
 
         If *destination* is a list of callsigns they will be joined in the specified order and sent as a relay.
-
-        The constructed message object is passed to pyjs8call.txmonitor internally if *Client.monitor_outgoing* is True (default).
+        
+        The constructed message object is passed to pyjs8call.outgoingmonitor internally if *monitor_outgoing* is True (default).
 
         Args:
             destination (str, list): Callsign(s) to direct the query to
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
         return self.send_directed_command_message(destination, Message.CMD_STATUS_Q)
 
-    def get_call_activity(self, age=60):
+    def get_call_activity(self, age=None):
         '''Get JS8Call call activity.
 
+        To get or set JS8Call callsign activity aging from the configuration file:
+        `client.config.get('Configuration', 'CallsignAging', int)`
+        `client.config.set('Configuration', 'CallsignAging', 120) # 120 minutes`
+
+        See *client.get_distance()* for more information on the value and format of *distance*.
+
         Each call activity item is a dictionary with the following keys:
 
         | Key | Value Type |
         | -------- | -------- |
         | origin | str |
         | grid | str |
         | snr | int |
         | time (UTC) | int |
+        | timestamp (local) | int |
+        | local_time_str | str |
+        | speed | str |
         | hearing | list |
+        | heard_by | list |
+        | distance | tuple |
 
         Args:
-            age (int): Maximum activity age in minutes, defaults to 60
+            age (int): Maximum activity age in minutes, defaults to JS8Call callsign activity aging
 
         Returns:
-            list: Call activity items
+            list: Call activity items, sorted decending by *time* (recent first)
+
+            If grid is not set, distance is *(None, None)*.
         '''
+        if age is None:
+            age = self.config.get('Configuration', 'CallsignAging', int)
+
+        age *= 60 # minutes to seconds
+
         msg = Message()
         msg.type = Message.RX_GET_CALL_ACTIVITY
         self.js8call.send(msg)
         call_activity = self.js8call.watch('call_activity')
 
-        hearing = self.hearing(age = age)
-        age *= 60 # minutes to seconds
-        now = datetime.now(timezone.utc).timestamp()
-
-        for i in range(len(call_activity)):
-            origin = call_activity[i]['origin']
-            item_age = now - call_activity[i]['time']
+        #TODO improve efficiency (heard_by calls hearing again)
+        hearing = self.hearing(age)
+        heard_by = self.heard_by(age , hearing)
+        now = time.time()
+
+        for i in call_activity.copy():
+            activity = call_activity.pop(0)
+            activity['origin'] = activity['origin'].strip()
+            activity['grid'] = activity['grid'].strip()
 
-            if item_age > age:
+            # remove aged activity
+            if age != 0 and (now - activity['timestamp']) > age:
                 continue
 
-            if origin in hearing:
-                call_activity[i]['hearing'] = hearing[origin]
+            if activity['origin'] in hearing:
+                activity['hearing'] = hearing[activity['origin']]
+            else:
+                activity['hearing'] = []
 
+            if activity['origin'] in heard_by:
+                activity['heard_by'] = heard_by[activity['origin']]
+            else:
+                activity['heard_by'] = []
+
+            if activity['grid'] not in (None, ''):
+                activity['distance'] = self.grid_distance(activity['grid'])
+            else:
+                activity['distance'] = (None, None, None)
+
+            spot = self.spots.filter(origin = activity['origin'], age = age, count = 1)
+            if len(spot) and isinstance(spot[0].get('speed'), int):
+                activity['speed'] = self.settings.submode_to_speed(spot[0].get('speed'))
+            else:
+                activity['speed'] = ''
+
+            call_activity.append(activity)
+
+        call_activity.sort(key = lambda activity: activity['timestamp'], reverse = True)
         return call_activity
 
-    def get_band_activity(self):
+    def get_band_activity(self, age=None):
         '''Get JS8Call band activity.
 
+        To get or set JS8Call callsign activity aging from the configuration file:
+        `client.config.get('Configuration', 'ActivityAging', int)`
+        `client.config.set('Configuration', 'ActivityAging', 5) # 5 minutes`
+
         Each band activity item is a dictionary with the following keys:
 
         | Key | Value Type |
         | -------- | -------- |
         | freq (Hz) | int |
         | offset (Hz) | int |
         | snr | int |
         | time (UTC) | int |
+        | timestamp (local) | int |
+        | local_time_str | str |
         | text | str |
 
+        Args:
+            age (int): Maximum activity age in minutes, defaults to JS8Call band activity aging
+
         Returns:
-            list: Band activity items
+            list: Band activity items, sorted ascending by offset
         '''
+        if age is None:
+            age = self.config.get('Configuration', 'ActivityAging', int)
+
+            if age == 0:
+                age = None
+
+        if age is not None:
+            age *= 60 # minutes to seconds
+
         msg = Message()
         msg.type = Message.RX_GET_BAND_ACTIVITY
         self.js8call.send(msg)
         band_activity = self.js8call.watch('band_activity')
+
+        now = time.time()
+
+        if age is not None:
+            # remove aged activity
+            for i in band_activity.copy():
+                activity = band_activity.pop(0)
+
+                if (now - activity['timestamp']) > age:
+                    continue
+
+                band_activity.append(activity)
+
+        band_activity.sort(key=lambda activity: activity['offset'])
         return band_activity
 
     def get_selected_call(self):
         '''Get JS8Call selected callsign.
 
         Returns:
             str: Callsign selected on the JS8Call user interface
@@ -896,55 +1102,86 @@
     def get_rx_messages(self, own=True):
         '''Get list of messages from the JS8Call rx text field.
 
         Each message is a dictionary object with the following keys:
         - time
         - offset
         - origin
+        - destination
         - text
 
+        Dictionary keys *origin* and *destination* may be *None*.
+
         Args:
             own (bool): Include outgoing messages listed in the rx text field, defaults to True
 
         Returns:
             list: Messages from the rx text field
         '''
+        #TODO is command handling required?
+
         rx_text = self.get_rx_text()
         callsign = self.settings.get_station_callsign()
-        msgs = rx_text.split('\n')
-        msgs = [m.strip() for m in msgs if len(m.strip()) > 0]
+        msgs = rx_text.split('\n\n')
+        msgs = [m.strip(' ' + Message.EOM) for m in msgs if len(m.strip()) > 0]
 
         rx_messages = []
         for msg in msgs:
+            if '-' not in msg:
+                continue
+
+            #TODO
+            print(msg)
+
             parts = msg.split('-')
-            data = {
-                #TODO convert time format
-                'time' : parts[0].strip(),
-                'offset' : int(parts[1].strip(' \n()')),
-                'origin' : parts[2].split(':')[0].strip(),
-                'text' : parts[2].split(':')[1].strip(' \n' + Message.EOM)
-            }
+            data = {}
+
+            data['time'] = parts[0].strip()
+            data['offset'] = int(parts[1].strip(' \n()'))
+
+            if ':' not in parts[2]:
+                data['origin'] = None
+                data['destination'] = None
+                data['text'] = parts[2].strip()
+            else:
+                if '  ' in parts[2]:
+                    callsigns = parts[2].split('  ')[0].split(':')
+                    data['origin'] = callsigns[0].strip()
+                    data['destination'] = callsigns[1].strip()
+                    data['text'] = parts[2].split('  ')[1].strip()
+                elif '@HB' in parts[2]:
+                    data['origin'] = parts[2].split(':')[0].strip()
+                    data['destination'] = '@HB'
+                    data['text'] = parts[2].split('@HB')[1].strip()
+                else:
+                    data['origin'] = parts[2].split(':')[0].strip()
+                    data['destination'] = None
+                    data['text'] = parts[2].split(':')[1].strip()
 
-            if not own and data['callsign'] == callsign:
+            if not own and data['origin'] == callsign:
                 continue
 
             rx_messages.append(data)
 
         return rx_messages
     
-    def hearing(self, age=60):
-        '''Get information on which stations other stations are hearing.
+    def hearing(self, age=None):
+        '''Which stations other stations are hearing.
 
         Args:
-            age (int): Maximum message age in minutes, defaults to 60
+            age (int): Maximum message age in minutes, defaults to JS8Call callsign activity aging
 
         Returns:
-            dict: Example format *{'station': ['station', ...], ...}*
+            dict: Example format `{'station': ['station', ...], ...}`
         '''
-        age *= 60
+        if age is None:
+            age = self.config.get('Configuration', 'CallsignAging', int)
+
+        age *= 60 # minutes to seconds
+            
         callsign = self.settings.get_station_callsign()
         hearing = {}
         
         for spot in self.spots.filter(age = age):
             # only process msgs with directed commands
             if spot.cmd is None:
                 continue
@@ -958,57 +1195,99 @@
             if spot.cmd == Message.CMD_HEARING and spot.hearing is not None:
                 if spot.origin not in hearing:
                     hearing[spot.origin] = spot.hearing
                 else:
                     spot_hearing = [station for station in spot.hearing if station not in hearing[spot.origin]]
                     hearing[spot.origin].extend(spot_hearing)
             
-            if spot.cmd in (Message.CMD_ACK, Message.CMD_HEARTBEAT_SNR):
+            if spot.cmd in Message.COMMAND_RESPONSES:
                 if spot.origin not in hearing:
                     hearing[spot.origin] = []
 
                 if isinstance(spot.path, list):
                     # handle relay path
                     #TODO review if path list should be reversed
                     relay_path = Message.CMD_RELAY.join(spot.path)
 
                     if relay_path not in hearing[spot.origin]:
                         hearing[spot.origin].append(relay_path)
 
                 elif spot.destination != '@ALLCALL' and spot.destination not in hearing[spot.origin]:
                     hearing[spot.origin].append(spot.destination)
 
+        #TODO track spot snr for sorting
+        #return {callsign:stations.sort(lambda station: station['snr'], decending) for callsign, stations in hearing.items()}
         return hearing
 
-#TODO
-#    def heard_by(self, age=60):
-#        '''Get information on which stations are heard other stations.
-#        
+    def heard_by(self, age=None, hearing=None):
+        '''Which stations are heard by other stations.
+
+        *client.heard_by()* is the inverse of *client.hearing()*.
+
+        If calling both *client.hearing()* and *client.heard_by*, it is more efficient to pass the result of *client.hearing()* to *client.heard_by()*. Otherwise, *client.heard_by()* will call *client.hearing()* again internally.
+
+        Args:
+            age (int): Maximum message age in minutes, defaults to JS8Call callsign activity aging
+            hearing (dict): Result of *client.hearing()*, defaults to result of *client.hearing()*
+
+        Returns:
+            dict: Example format `{'station': ['station', ...], ...}`
+        '''
+        if age is None:
+            age = self.config.get('Configuration', 'CallsignAging', int)
+        
+        age *= 60
+        heard_by = {}
+
+        if hearing is None:
+            hearing = self.hearing(age)
+
+        for key, value in hearing.items():
+            for callsign in value:
+                if callsign not in heard_by:
+                    heard_by[callsign] = [key]
+                elif key not in heard_by[callsign]:
+                    heard_by[callsign].append(key)
+
+        return heard_by
+
+#    def discover_path(self, destination, age=60):
 #        '''
+#        '''
+#        age *= 60
 #        callsign = self.settings.get_station_callsign()
-#        heard = {}
+#        heard_by = self.heard_by(age = age)
+#
+#        if destination in heard_by:
+#            if callsign in heard_by[destination]:
+#                return destination
+#
+#            else:
+#                '>'.join()
+            
         
-    def grid_distance(self, grid_a, grid_b=None, miles=True):
+    def grid_distance(self, grid_a, grid_b=None):
         '''Calculate great circle distance and bearing between grid squares.
 
         If *grid_b* is *None* the JS8Call grid square is used.
 
         Bearing is calculated from *grid_b* to *grid_a*.
 
         *grid* must be a 4 or 6 character Maidenhead grid square (ex. EM19 or EM19es). If *grid* is longer than 6 characters it will be truncated to 6 characters.
 
         Reference: https://www.movable-type.co.uk/scripts/latlong.html
 
         Args:
             grid_a (str): First grid square
-            grid_b (str): Second grid square, defaults to None
-            miles (bool): Calculate distance in miles if True, in km if False, defaults to True
+            grid_b (str): Second grid square, defaults to JS8Call grid square
 
         Returns:
-            tuple (int, int): Distance/bearing pair (ex. (1194, 312))
+            tuple (int, str, int): Distance, distance units, and bearing in degrees (ex. (1194, 'mi', 312)).
+            
+            Distance units match JS8Call distance units, see *client.settings.get_distance_units()*.
 
         Raises:
             ValueError: *grid_b* is *None* and JS8Call grid square is not set
         '''
         earth_radius_km = 6371
         earth_radius_mi = 3958.756
 
@@ -1022,27 +1301,29 @@
         lat_b, lon_b = self.grid_to_lat_lon(grid_b)
         # convert degrees to radians
         lat_a, lon_a, lat_b, lon_b = map(radians, [lat_a, lon_a, lat_b, lon_b])
 
         # calculate great circle distance
         gcd = acos(sin(lat_a) * sin(lat_b) + cos(lat_a) * cos(lat_b) * cos(lon_b - lon_a))
         
-        if miles:
+        if self.settings.get_distance_units_miles():
             distance = int(round(earth_radius_mi * gcd, 0))
+            units = 'mi'
         else:
             distance = int(round(earth_radius_km * gcd, 0))
+            units = 'km'
 
         # calculate bearing
         y = sin(lon_a - lon_b) * cos(lat_a)
         x = cos(lat_b) * sin(lat_a) - sin(lat_b) * cos(lat_a) * cos(lon_a - lon_b)
         angle = atan2(y, x)
         bearing = (angle * 180 / pi + 360) % 360
         bearing = int(round(bearing, 0))
 
-        return (distance, bearing)
+        return (distance, units, bearing)
 
     def grid_to_lat_lon(self, grid):
         '''Convert grid square to latitude/longitude.
 
         *grid* must be a 4 or 6 character Maidenhead grid square (ex. EM19 or EM19es). If *grid* is longer than 6 characters it will be truncated to 6 characters.
 
         Latitude and longitude are rounded to 3 decimal places.
@@ -1233,18 +1514,38 @@
     def disable_transmit(self):
         '''Disable transmitting via config file.
         
         It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
         '''
         self._client.config.set('Configuration', 'TransmitOFF', 'true')
 
+    def get_profile(self):
+        '''Get active JS8call configuration profile via config file.
+
+        This is a convenience function. See pyjs8call.confighandler for other configuration related functions.
+
+        Returns:
+            str: Name of the active configuration profile
+        '''
+        return self._client.config.get_active_profile()
+
+    def get_profile_list(self):
+        '''Get list of JS8Call configuration profiles via config file.
+
+        This is a convenience function. See pyjs8call.confighandler for other configuration related functions.
+
+        Returns:
+            list: List of configuration profile names
+        '''
+        return self._client.config.get_profile_list()
+
     def set_profile(self, profile):
         '''Set active JS8Call configuration profile via config file.
         
-        This is a convenience function. See pyjs8call.confighandler for other configuration profile related functions.
+        This is a convenience function. See pyjs8call.confighandler for other configuration related functions.
         
         It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
 
         Args:
             profile (str): Profile name
 
         Raises:
@@ -1459,34 +1760,86 @@
             int: Idle timeout in minutes
         '''
         return self._client.config.get('Configuration', 'TxIdleWatchdog', value_type=int)
 
     def set_idle_timeout(self, timeout):
         '''Set JS8Call idle timeout.
 
-        The JS8Call idle timeout must be between 5 and 1440 minutes.
+        If the JS8Call idle timeout is less than 5 minutes, JS8Call will force it to 5 minutes on the next application start or exit.
+
+        The maximum idle timeout is 1440 minutes (24 hours).
+
+        Disable the idle timeout by setting it to 0 (zero).
 
         It is recommended that this function be called before calling *client.start()*. If this function is called after *client.start()* then the application will have to be restarted to utilize the new config file settings. See *client.restart()*.
 
         Args:
-            timeout (int): Timeout to set in minutes
+            timeout (int): Idle timeout in minutes
 
         Returns:
             int: Current idle timeout in minutes
 
         Raises:
-            ValueError: Idle timeout must be between 5 and 1440 minutes
+            ValueError: Idle timeout must be between 0 and 1440 minutes
         '''
-        if timeout < 5 or timeout > 1440:
-            raise ValueError('Idle timeout must be between 5 and 1440 minutes')
+        if timeout < 0 or timeout > 1440:
+            raise ValueError('Idle timeout must be between 0 and 1440 minutes')
 
         self._client.config.set('Configuration', 'TxIdleWatchdog', timeout)
-
         return self.get_idle_timeout()
 
+    def get_distance_units_miles(self):
+        '''Get JS8Call distance unit setting.
+        
+        Returns:
+            bool: True if distance units are set to miles, False if km
+        '''
+        return self._client.config.get('Configuration', 'Miles', value_type=bool)
+        
+    def set_distance_units_miles(self, units_miles):
+        '''Set JS8Call distance unit setting.
+        
+        Args:
+            units_miles (bool): Set units to miles if True, set to km if False
+            
+        Returns:
+            bool: True if distance units are set to miles, False if km
+        '''
+        self._client.config.set('Configuration', 'Miles', str(units_miles).lower())
+        return self.get_distance_units_miles()
+        
+    def get_distance_units(self):
+        '''Get JS8Call distance units.
+        
+        Returns:
+            str: Configured distance units: 'mi' or 'km'
+        '''
+        if self.get_distance_units_miles():
+            return 'mi'
+        else:
+            return 'km'
+        
+    def set_distance_units(self, units):
+        ''' Set JS8Call distance units.
+        
+        Args:
+            units (str): Distance units: 'mi', 'miles', 'km', or 'kilometers'
+            
+        Returns:
+            str: Configured distance units: 'miles' or 'km'
+        '''
+        if units.lower() in ['mi', 'miles']:
+            self.set_distance_units_miles(True)
+            return self.get_distance_units()
+        elif units.lower() in ['km', 'kilometers']:
+            self.set_distance_units_miles(False)
+            return self.get_distance_units()
+        else:
+            raise ValueError('Distance units must be: mi, miles, km, or kilometers')
+    
     def get_station_grid(self, update=False):
         '''Get JS8Call grid square.
 
         Args:
             update (bool): Update if True or use local state if False, defaults to False
 
         Returns:
@@ -1621,15 +1974,17 @@
 
     Attributes:
         incoming (dict): Incoming message callback function lists organized by message type
         outgoing (func): Outgoing message status change callback function, defaults to None
         spots (func): New spots callback funtion, defaults to None
         station_spot (func): Watched station spot callback function, defaults to None
         group_spot (func): Watched group spot callback function, defaults to None
-        window (func): Transmit window transition callback function, defaults to None
+        window (func): rx/tx window transition callback function, defaults to None
+        inbox (func): New inbox message callback function, defaults to None
+        schedule (func): Schedule entry activation callback function, defaults to None
 
     *incoming* structure: *{type: [callback, ...], ...}*
     - *type* is an incoming  message type (see pyjs8call.message for information on message types)
     - *callback* function signature: *func(msg)* where *msg* is a pyjs8call.message object
 
     *outgoing* callback signature: *func(msg)* where *msg* is a pyjs8call.message object
     - Called by pyjs8call.txmonitor
@@ -1645,28 +2000,33 @@
 
     *window* callback signature: *func()*
     - Called by pyjs8call.windowmonitor
 
     *inbox* callback signature: *func(msgs)* where *msgs* is a list of *dict* message items
     - See *client.get_inbox_messages()* for message item *dict* key details
     - Called by pyjs8call.inboxmonitor
+
+    *schedule* callback signature: *func(sch)* where *sch* is a pyjs8call.schedule.Schedule object
+    - See *pyjs8call.schedule.Schedule* for object property details
+    - Called by pyjs8call.schedulemonitor
     '''
 
     def __init__(self):
         '''Initialize callback object.
 
         Returns:
             pyjs8call.client.Callbacks: Constructed callback object
         '''
         self.outgoing = None
         self.spots = None
         self.station_spot = None
         self.group_spot = None
         self.window = None
         self.inbox = None
+        self.schedule = None
         self.incoming = {
             Message.RX_DIRECTED: [],
         }
 
     def register_incoming(self, callback, message_type=Message.RX_DIRECTED):
         '''Register incoming message callback function.
```

### Comparing `pyjs8call-0.2.0/pyjs8call/confighandler.py` & `pyjs8call-0.2.1/pyjs8call/confighandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,41 +74,70 @@
 
         Args:
             config_path (str): Alternate config file path, defaults to None
 
         Raises:
             FileNotFoundError: Config file not found at specified path
         '''
+        self.file = 'JS8Call.ini'
+        self.rig = None
+
         if config_path is not None:
-            self.path = config_path
+            self.path, self.file = os.path.split(config_path)
         elif psutil.WINDOWS:
-            self.path = os.path.expandvars('C:\\Users\\$USERNAME\\AppData\\Local\\JS8Call\\JS8Call.ini')
+            self.path = os.path.expandvars('C:\\Users\\$USERNAME\\AppData\\Local\\JS8Call')
         elif psutil.MACOS:
-            self.path = os.path.join(os.path.expanduser('~'), 'Library/Preferences/JS8Call.ini')
+            self.path = os.path.join(os.path.expanduser('~'), 'Library/Preferences')
         else:
-            self.path = os.path.join(os.path.expanduser('~'), '.config/JS8Call.ini')
+            self.path = os.path.join(os.path.expanduser('~'), '.config')
+        
+        self.config_path = os.path.join(self.path, self.file)
+        self._main_config_path = os.path.join(self.path, self.file)
+
+        if not os.path.exists(self.config_path):
+            raise FileNotFoundError('JS8Call config file not found at ' + str(self.config_path))
+
+        self.config = configparser.ConfigParser(interpolation = None)
+        self.config.optionxform = lambda option: option
+        self.config.read(self.config_path)
 
-        if not os.path.exists(self.path):
-            raise FileNotFoundError('JS8Call config file not found at ' + str(self.path))
+    def load_rig_config(self, rig_name):
+        '''Load rig-specific config file.
+
+        This function is used internally by pyjs8call.Client.start().
+
+        Args:
+            rig_name (str): Rig name being passed to JS8Call at application launch
+        '''
+        self.rig = rig_name.strip()
+        file_parts = self.file.split('.')
+        self.file = file_parts[0] + ' - ' + self.rig + '.' + file_parts[1]
+        self.config_path = os.path.join(self.path, self.file)
+
+        if not os.path.exists(self.config_path):
+            with open(self.config_path, 'w') as fd:
+                # write main config object to the rig config file
+                self.config.write(fd, space_around_delimiters = False)
 
+        # replace main config object with rig config
         self.config = configparser.ConfigParser(interpolation = None)
         self.config.optionxform = lambda option: option
-        self.config.read(self.path)
+        self.config.read(self.config_path)
 
     def write(self):
         '''Write the config parser object to file.
 
-        A backup of the original JS8Call config file is saved as JS8Call.ini.original in the same directory as the JS8Call.ini file.
+        A backup of the original JS8Call config file is saved as JS8Call.ini.original in the same directory as the JS8Call.ini file. Rig specific config file backups are not saved.
         '''
-        if not os.path.exists(self.path + '.original'):
+        if self.rig is None and not os.path.exists(self.config_path + '.original'):
             # create a backup of the original config file before writing changes
-            with open(self.path + '.original', 'w') as fd:
+            with open(self.config_path + '.original', 'w') as fd:
                 self.config.write(fd, space_around_delimiters = False)
 
-        with open(self.path, 'w') as fd:
+        with open(self.config_path, 'w') as fd:
             # write current config object to the config file
             self.config.write(fd, space_around_delimiters = False)
 
     def set(self, section, option, value):
         '''Set an option value in a given section.
 
         Value can be of the following types:
```

### Comparing `pyjs8call-0.2.0/pyjs8call/hbnetwork.py` & `pyjs8call-0.2.1/pyjs8call/hbnetwork.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,15 +52,31 @@
         '''
         self._client = client
         self._enabled = False
         self._paused = False
         self._last_outgoing = 0
         self._offset = None
 
-    def enable_networking(self, interval=10):
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+
+        Returns:
+            bool: True if paused, False if running
+        '''
+        return self._paused
+
+    def enable(self, interval=10):
         '''Enable heartbeat networking.
 
         Args:
             interval (int): Number of minutes between outgoing messages, defaults to 10
         '''
         if self._enabled:
             return
@@ -69,31 +85,31 @@
 
         self._offset = OffsetMonitor(self._client)
         self._offset.min_offset = 500
         self._offset.max_offset = 1000
         self._offset.bandwidth_safety_factor = 1.1
         self._offset.activity_cycles = 4
         self._offset.before_transition = 0.5
-        self._offset.pause_monitoring()
-        self._offset.enable_monitoring()
+        self._offset.pause()
+        self._offset.enable()
 
         thread = threading.Thread(target=self._monitor, args=(interval,))
         thread.daemon = True
         thread.start()
 
-    def disable_networking(self):
+    def disable(self):
         '''Disable heartbeat monitoring.'''
         self._enabled = False
-        self._offset.disable_monitoring()
+        self._offset.disable()
 
-    def pause_networking(self):
+    def pause(self):
         '''Pause heartbeat monitoring.'''
         self._paused = True
 
-    def resume_networking(self):
+    def resume(self):
         '''Resume heartbeat monitoring.'''
         self._last_outgoing = time.time()
         self._paused = False
 
     def _monitor(self, interval):
         '''Heartbeat monitor thread.'''
         interval *= 60
@@ -124,30 +140,30 @@
 
             # allow pause as late as possible
             if self._paused:
                 continue
 
             # pause main offset monitor
             main_offset_is_paused = self._client.offset.paused()
-            self._client.offset.pause_monitoring()
+            self._client.offset.pause()
             last_offset = self._client.settings.get_offset()
 
             # if no free hb offset or no activity, use pre-set random offset
             max_offset = self._offset.max_offset - self._offset.bandwidth
             hb_offset = random.randrange(self._offset.min_offset, max_offset)
             self._client.settings.set_offset(hb_offset)
             # resume hb offset monitor
-            self._offset.resume_monitoring()
+            self._offset.resume()
 
             # send heartbeat on next cycle
             #TODO self._client.window.ignore_next_tx_frame()
             self._client.send_heartbeat()
             
             # wait until the end of the following cycle
             self._client.window.sleep_until_next_transition(within = 1, before = 1)
             self._last_outgoing = time.time()
-            self._offset.pause_monitoring()
+            self._offset.pause()
             self._client.settings.set_offset(last_offset)
                 
             if not main_offset_is_paused:
-                self._client.offset.resume_monitoring()
+                self._client.offset.resume()
```

### Comparing `pyjs8call-0.2.0/pyjs8call/inboxmonitor.py` & `pyjs8call-0.2.1/pyjs8call/inboxmonitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,63 @@
         '''
         self._client = client
         self._enabled = False
         self._paused = False
         self._rx_queue = []
         self._rx_queue_lock = threading.Lock()
 
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+
+        Returns
+            bool: True if paused, False if running
+        '''
+        return self._paused
+
+    def enable(self, query=True, destination='@ALLCALL', interval=60):
+        '''Enable inbox monitoring.
+
+        If *query* is True a message query will be sent to *destination* every *interval* minutes. Incoming directed messages are responded to whether *query* is True or not. See *process_incoming()* for more information on incoming directed message handling.
+
+        Args:
+            query (bool): Transmit message queries periodically if True, defaults to True
+            destination (str): Outgoing message query destination, defaults to '@ALLCALL'
+            interval (int): Minutes between message queries, defaults to 60
+        '''
+        if self._enabled:
+            return
+
+        self._enabled = True
+        self._client.callback.register_incoming(self.process_incoming, message_type = Message.RX_DIRECTED)
+
+        thread = threading.Thread(target=self._monitor, args=(query, destination, interval))
+        thread.daemon = True
+        thread.start()
+
+    def disable(self):
+        '''Disable inbox monitoring.'''
+        self._enabled = False
+        self._client.callback.remove_incoming(self.process_incoming)
+
+    def pause(self):
+        '''Pause inbox monitoring.'''
+        self._paused = True
+
+    def resume(self):
+        '''Resume inbox monitoring.'''
+        self._paused = False
+
     def message(self, msg_id):
         '''Get specified inbox message.
         
         An inbox message is a *dict* with the following keys:
         
         | Key | Value Type |
         | -------- | -------- |
@@ -285,47 +334,14 @@
         db_path = self._client.config.get('Configuration', 'AzElDir')
         db_file = os.path.join(db_path, 'inbox.db3')
         conn = sqlite3.connect(db_file)
         conn.cursor().execute('DELETE FROM inbox_v1;')
         conn.commit()
         conn.close()
         
-    def enable_monitoring(self, query=True, destination='@ALLCALL', interval=60):
-        '''Enable inbox monitoring.
-
-        If *query* is True a message query will be sent to *destination* every *interval* minutes. Incoming directed messages are responded to whether *query* is True or not. See *process_incoming()* for more information on incoming directed message handling.
-
-        Args:
-            query (bool): Transmit message queries periodically if True, defaults to True
-            destination (str): Outgoing message query destination, defaults to '@ALLCALL'
-            interval (int): Minutes between message queries, defaults to 60
-        '''
-        if self._enabled:
-            return
-
-        self._enabled = True
-        self._client.callback.register_incoming(self.process_incoming, message_type = Message.RX_DIRECTED)
-
-        thread = threading.Thread(target=self._monitor, args=(query, destination, interval))
-        thread.daemon = True
-        thread.start()
-
-    def disable_monitoring(self):
-        '''Disable inbox monitoring.'''
-        self._enabled = False
-        self._client.callback.remove_incoming(self.process_incoming)
-
-    def pause_monitoring(self):
-        '''Pause inbox monitoring.'''
-        self._paused = True
-
-    def resume_monitoring(self):
-        '''Resume inbox monitoring.'''
-        self._paused = False
-
     def process_incoming(self, msg):
         '''Process incoming directed messages.
 
         This function is used internally.
 
         Parses message ID and sends a query for the remote message (see *pyjs8call.client.query_message_id()*).
 
@@ -359,14 +375,20 @@
         last_query_timestamp = 0
         query_interval *= 60
 
         rx_processing = False
         last_tx_timestamp = 0
 
         while self._enabled:
+            # delay until next window transition
+            self._client.window.sleep_until_next_transition(within = 0.5)
+            
+            if self._paused:
+                continue
+            
             window_duration = self._client.settings.get_window_duration()
             response_delay = window_duration * 30
 
             if len(self._rx_queue) > 0:
                 rx_processing = True
                 msg = self._rx_queue.pop(0)
 
@@ -382,23 +404,21 @@
                     # cull old msg
                     rx_processing = False
                 else:
                     # wait for response
                     self._rx_queue.insert(0, msg)
 
             elif not rx_processing and query and (last_query_timestamp + query_interval) < time.time():
-                if not self._paused:
+                # ensure no last second state change before transmitting
+                if not self._paused and self._enabled:
                     self._client.query_messages(destination)
                     last_query_timestamp = time.time()
 
             # check local inbox for new unread msgs
             inbox = self.unread()
 
             if inbox is not None:
                 new_msgs = [msg for msg in inbox if msg not in last_inbox]
                 last_inbox = inbox
 
                 if len(new_msgs) > 0:
                     self._callback(new_msgs)
-
-            # delay until next window transition
-            self._client.window.sleep_until_next_transition(within = 0.5)
```

### Comparing `pyjs8call-0.2.0/pyjs8call/js8call.py` & `pyjs8call-0.2.1/pyjs8call/js8call.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 
 class JS8Call:
     '''Low-level JS8Call TCP socket and local state management.
 
     Receives and transmits pyjs8call.message objects, and generally manages the local state representation of the JS8Call application.
 
-    Initializes pyjs8call.appmonitor as well as rx, tx, logging, ping threads.
-
+    Initializes pyjs8call.appmonitor as well as rx, tx, logging, application ping threads.
+    
     Attributes:
         app (pyjs8call.appmonitor): Application monitor object
         connected (bool): Whether the JS8Call TCP socket is connected
         max_spots (int): Maximum number of spots to store before dropping old spots, defaults to 5000
         last_incoming (float): Timestamp of last incoming user message, defaults to 0 (zero)
         last_outgoing (float): Timestamp of last outgoing user message, defaults to 0 (zero)
     '''
@@ -68,39 +68,43 @@
         self._host = host
         self._port = port
         self._rx_queue = []
         self._rx_queue_lock = threading.Lock()
         self._tx_queue = []
         self._tx_queue_lock = threading.Lock()
         self._socket = None
-        self._socket_ping_delay = 60 * 5 # seconds
+        self._socket_ping_delay = 60 # seconds
         self._debug = False
         self._debug_all = False
         self._log = False
         self._log_all = False
         self._log_path = os.path.join(os.path.expanduser('~'), 'pyjs8call.log')
         self._log_queue = ''
         self._log_queue_lock = threading.Lock()
         self._debug_log_type_blacklist = [
             Message.TX_GET_TEXT,        # tx monitor every 1 second
             Message.TX_TEXT,            # tx monitor every 1 second
             Message.RIG_PTT,            # too frequent, not useful
             Message.TX_FRAME,           # start of outgoing message, not useful
             Message.INBOX_MESSAGES,     # inbox monitor every window transition
             Message.INBOX_GET_MESSAGES, # inbox monitor every window transition
-            Message.STATION_STATUS      # too frequent
+            Message.STATION_STATUS,     # too frequent
+            Message.RIG_GET_FREQ,       # offset monitor every window transition
+            Message.RIG_FREQ            # offset monitor every window transition
         ]
         self._watching = None
         self._watch_timeout = 3 # seconds
         self._spots = []
         self.max_spots = 5000
         self._recent_spots = []
+        self._spots_lock = threading.Lock()
         self.connected = False
         self.last_incoming = 0
         self.last_outgoing = 0
+        self._last_incoming_api_msg = 0
 
         self.state = {
             'ptt' : False,
             'dial': None,
             'freq' : None,
             'offset' : None,
             'callsign' : None,
@@ -113,25 +117,34 @@
             'call_activity' : None,
             'band_activity' : None,
             'selected_call' : None,
         }
 
         self.app = pyjs8call.AppMonitor(self)
 
-    def start(self, headless=False):
+    def start(self, headless=False, args = None):
         '''Start the JS8Call application.
 
-        Used internally by pyjs8call.client.Client.start().
+        This function is blocking until the JS8Call application responds to a network command which ensures that the application is operational before continuing. This handles slower computers such as Raspberry Pi.
+
+        Used internally by client.start().
 
         Args:
             headless (bool): Run JS8Call headless using xvfb (Linux only), defaults to False
+            args (list): Command line arguments (see appmonitor.start), defaults to empty list
+
+        Raises:
+            RuntimeError: JS8Call application failed to start
         '''
-        self.online = True
-        self.app.start(headless=headless)
+        if args is None:
+            args = []
         
+        self.online = True
+        self.app.start(headless=headless, args = args)
+
         tx_thread = threading.Thread(target=self._tx)
         tx_thread.daemon = True
         tx_thread.start()
 
         rx_thread = threading.Thread(target=self._rx)
         rx_thread.daemon = True
         rx_thread.start()
@@ -140,14 +153,30 @@
         hb_thread.daemon = True
         hb_thread.start()
 
         log_thread = threading.Thread(target=self._log_monitor)
         log_thread.daemon = True
         log_thread.start()
 
+        time.sleep(1)
+        timeout = time.time() + 60
+
+        # wait for application to respond
+        while True:
+            try:
+                # value error while application is still starting (i.e. raspberry pi)
+                self._client.settings.get_speed()
+                # no errors, application responded
+                break
+            except ValueError:
+                pass
+
+            if time.time() > timeout:
+                RuntimeError('JS8Call application failed to start')
+
     def reinitialize(self, settings):
         '''Re-initialize internal settings after restart.
 
         Used internally.
 
         Args:
             settings (dict): Settings to re-initialize
@@ -173,71 +202,14 @@
             '_debug_log_type_blacklist',
             '_log',
             '_log_all'
         ]
 
         return {setting: getattr(self, setting) for setting in settings}
 
-    def get_spots(self):
-        '''Get list of spot messages.
-        
-        Returns:
-            list: All spot message objects
-        '''
-        return self._spots
-
-    def get_state(self, state):
-        '''Get asynchronous state value.
-
-        Waits for state to stop being watched before returning.
-
-        Internal state settings:
-        - ptt
-        - dial 
-        - freq
-        - offset
-        - callsign
-        - speed
-        - grid
-        - info
-        - rx_text
-        - tx_text
-        - inbox 
-        - call_activity
-        - band_activity
-        - selected_call
-
-        Args:
-            state (str): State value to get
-
-        Returns:
-            Returned type varies depending on the specified state value.
-        '''
-        while self.watching(state):
-            time.sleep(0.1)
-
-        return self.state[state]
-
-    def watching(self, state=None):
-        '''Get internal asynchronous setting state.
-
-        See *get_state()* for a list of internal state settings.
-
-        Args:
-            state (str): State to check, defaults to None
-
-        Returns:
-            str: Name of internal setting waiting for async JS8Call response, if *state* is None
-            bool: Whether *state* is waiting for async JS8Call response, if *state* is specified
-        '''
-        if state is None:
-            return self._watching
-        else:
-            return bool(state == self._watching)
-
     def stop(self):
         '''Stop threads and JS8Call application.'''
         self.online = False
         self._socket.close()
         self.app.stop()
 
     def enable_debugging(self, debug_all=False):
@@ -307,14 +279,15 @@
 
         Sets the status of the message object to *queued* (see pyjs8call.message statuses).
 
         Args:
             msg (pyjs8call.message): Message object to be transmitted
         '''
         msg.status = Message.STATUS_QUEUED
+        msg.set('profile', self._client.settings.get_profile())
 
         with self._tx_queue_lock:
             self._tx_queue.append(msg)
         
     def append_to_rx_queue(self, msg):
         '''Queue received message from the JS8Call application for handling.
 
@@ -339,14 +312,63 @@
         if len(self._rx_queue) > 0:
             with self._rx_queue_lock:
                 msg = self._rx_queue.pop(0)
 
             msg.status = Message.STATUS_RECEIVED
             return msg
 
+    def get_state(self, state):
+        '''Get asynchronous state value.
+
+        Waits for state to stop being watched before returning.
+
+        Internal state settings:
+        - ptt
+        - dial 
+        - freq
+        - offset
+        - callsign
+        - speed
+        - grid
+        - info
+        - rx_text
+        - tx_text
+        - inbox 
+        - call_activity
+        - band_activity
+        - selected_call
+
+        Args:
+            state (str): State value to get
+
+        Returns:
+            Returned type varies depending on the specified state value.
+        '''
+        while self.watching(state):
+            time.sleep(0.1)
+
+        return self.state[state]
+
+    def watching(self, state=None):
+        '''Get internal asynchronous setting state.
+
+        See *get_state()* for a list of internal state settings.
+
+        Args:
+            state (str): State to check, defaults to None
+
+        Returns:
+            str: Name of internal setting waiting for async JS8Call response, if *state* is None
+            bool: Whether *state* is waiting for async JS8Call response, if *state* is specified
+        '''
+        if state is None:
+            return self._watching
+        else:
+            return bool(state == self._watching)
+
     def watch(self, item):
         '''Watch local state variable for updating based on a response from the JS8Call application.
 
         The JS8Call application responds to requests asynchronously, which means responses may not be received in the same order as the requests or in a reasonable timeframe following the request. To handle these asynchronous reponses, the responses set local state variables as they are received. The process is as follows:
         - Send a request to the JS8Call application
         - Set local state variable associated with anticipated response to a known value (None)
         - Wait for a response, timing out if a response is not received within 3 seconds
@@ -377,14 +399,22 @@
         # timeout occurred, revert to last state
         if self.state[item] is None:
             self.state[item] = last_state
         
         self._watching = None
         return self.state[item]
 
+    def get_spots(self):
+        '''Get list of spot messages.
+        
+        Returns:
+            list: All spot message objects
+        '''
+        return self._spots
+
     def _spot(self, msg):
         '''Store a message when a station is heard.
 
         The message is compared to a list of recent messages (heard within the last 10 seconds) to prevent duplicate spots from multiple JS8Call API messages associated with the same station event.
 
         The list of stored messages is culled once it exceeeds the maximum size set by *max_spots* by dropping the oldest message.
 
@@ -392,21 +422,22 @@
 
         Args:
             msg (pyjs8call.message): Message to spot
         '''
         # cull recent spots
         self._recent_spots = [spot for spot in self._recent_spots if spot.age() < 10]
 
-        if msg not in self._recent_spots:
-            self._recent_spots.append(msg)
-            self._spots.append(msg)
-
-        # cull spots
-        if len(self._spots) > self.max_spots:
-            self._spots.pop(0)
+        with self._spots_lock:
+            if msg not in self._recent_spots:
+                self._recent_spots.append(msg)
+                self._spots.append(msg)
+    
+            # cull spots
+            if len(self._spots) > self.max_spots:
+                self._spots.pop(0)
 
     def _log_msg(self, msg):
         '''Add message to log queue.'''
         if msg.type in Message.TX_TYPES:
             msg_type = 'TX'
         elif msg.type in Message.RX_TYPES:
             msg_type = 'RX'
@@ -425,19 +456,19 @@
                         fd.write(self._log_queue)
                     self._log_queue = ''
             time.sleep(1)
 
     def _ping(self):
         '''JS8Call application ping thread.
 
-        If no messages have been received from the JS8Call in the last 5 minutes, a request is issued to the application to make sure it is still connected and functioning as expected.
+        If no messages have been received from the JS8Call in the last minute, a request is issued to the application to make sure it is still connected and functioning as expected.
         '''
         while self.online:
-            # if no recent rx, check the connection by making a request
-            timeout = self.last_incoming + self._socket_ping_delay
+            # if no recent api msgs, check the connection by making a request
+            timeout = self._last_incoming_api_msg + self._socket_ping_delay
 
             if time.time() > timeout:
                 self.connected = False
                 msg = Message()
                 msg.type = Message.STATION_GET_CALLSIGN
                 self.send(msg)
                 
@@ -449,50 +480,46 @@
         The JS8Call tx text field is read every second by pyjs8call.txmonitor. This is utilized to reduce additional socket traffic by reading the local state variable directly without requesting additional updates from the application.
 
         When processing the transmit message queue, if a transmission is in process (i.e. there is text in the tx text field) then transmission of additional messages is prevented until the current transmission is complete.
 
         If debugging or logging is enabled then each message sent over the TCP socket is printed to the console or to file respectively. By default not all messages are printed or logged (see pyjs8call.js8call.JS8Call._debug_log_type_blacklist). Frequently sent and received messages used internal to pyjs8call are not printed or logged.
         '''
         tx_text = False
-        force_tx_text = False
+        active_tx_state = False
 
         while self.online:
             # TxMonitor updates tx_text every second
-            # do not attempt to update while value is being watched (i.e. updated)
-            if not self.watching('tx_text') and self.state['tx_text'] is not None:
-                if len(self.state['tx_text'].strip()) > 0:
-                    tx_text = True
-                    force_tx_text = False
-                else:
-                    tx_text = False
+            if self.state['tx_text'] == '':
+                tx_text = False
+            else:
+                tx_text = True
+                active_tx_state = False
 
             with self._tx_queue_lock:
                 for msg in self._tx_queue.copy():
                     # hold off on sending messages while there is something being sent (text in the tx text field)
-                    if msg.type == Message.TX_SEND_MESSAGE and (tx_text or force_tx_text):
+                    if msg.type in Message.USER_MSG_TYPES and (tx_text or active_tx_state):
                         continue
-
+            
                     packed = msg.pack()
-    
+                    
                     if self._debug and (self._debug_all or (msg.type not in self._debug_log_type_blacklist)):
                         print('TX: ' + packed.decode('utf-8').strip())
     
                     if self._log and (self._log_all or (msg.type not in self._debug_log_type_blacklist)):
                         self._log_msg(msg)
     
                     try:
                         self._socket.sendall(packed)
                         self._tx_queue.remove(msg)
-                    
+
                         if msg.type in Message.USER_MSG_TYPES:
                             self.last_outgoing = time.time()
-                        
-                        # make sure the next queued msg doesn't get sent before the tx text state updates
-                        if msg.type == Message.TX_SEND_MESSAGE:
-                            force_tx_text = True
+                            # make sure the next queued msg doesn't get sent before the tx text state updates
+                            active_tx_state = True
 
                     except (BrokenPipeError, ValueError, OSError):
                         # BrokenPipeError may happen when restarting due to closed socket
                         # ValueError may happen when restarting, tx_queue.remove fails (possibly due to PEP 475)
                         # OSError may happen when stopping during msg processing, socket.sendall fails
                         pass
 
@@ -518,15 +545,15 @@
         '''
         while self.online:
             data = b''
             data_str = ''
 
             try:
                 data += self._socket.recv(65535)
-            except (socket.timeout, OSError):
+            except socket.timeout:
                 # if rx from socket fails continue trying
                 continue
             except OSError:
                 # OSError occurs while app is restarting
                 self.connected = False
                 continue
 
@@ -556,20 +583,19 @@
                 except Exception as e:
                     if self._debug or self._debug_all:
                         raise e
                     else:
                         # if parsing message fails, stop processing
                         continue
 
-                # if error in message value, stop processing
-                if msg.value is not None and Message.ERR in msg.value:
-                    continue
-
                 if msg.type in Message.USER_MSG_TYPES:
                     self.last_incoming = time.time()
+
+                msg.status = Message.STATUS_RECEIVED
+                self._last_incoming_api_msg = time.time()
                 
                 # print msg in debug mode
                 if self._debug and (self._debug_all or (msg.type not in self._debug_log_type_blacklist)):
                     print('RX: ' + json.dumps(msg.dict()))
 
                 # log msg
                 if self._log and (self._log_all or (msg.type not in self._debug_log_type_blacklist)):
@@ -582,32 +608,32 @@
     def _process_message(self, msg):
         '''Process received message.
 
         Messages are processed based on their command and/or their type (see pyjs8call.message for commands and types). Messages are spotted when appropriate. Responses to JS8Call setting and state requests are handled to update the associated local state variables.
 
         Automatic cleaning of directed message text is handled if enabled (see pyjs8call.client).
 
-        Tx frame messages are passed to pyjs8call.windowmonitor.
-
         Args:
             msg (pyjs8call.message): Message to process
         '''
         # try to get distance and bearing
-        if msg.grid not in (None, ''):
-            miles = bool(self._client.config.get('Configuration', 'Miles') == 'true')
-
+        if msg.get('grid') not in (None, ''):
             try:
                 # raises ValueError for incorrect grid format
-                distance, bearing = self._client.grid_distance(msg.grid, miles = miles)
+                distance, units, bearing = self._client.grid_distance(msg.get('grid'))
                 msg.set('distance', distance)
+                msg.set('distance_units', units)
                 msg.set('bearing', bearing)
             except ValueError:
                 pass
 
-
+        # set active profile for spot filtering
+        msg.set('profile', self._client.settings.get_profile())
+        
+        
         ### command handling ###
 
         if msg.cmd in Message.COMMANDS:
             self._spot(msg)
 
 
         ### message type handling ###
@@ -615,14 +641,21 @@
         if msg.type == Message.INBOX_MESSAGES:
             self.state['inbox'] = msg.messages
 
         elif msg.type == Message.RX_SPOT:
             self._spot(msg)
 
         elif msg.type == Message.RX_DIRECTED:
+            # custom processing of incoming messages
+            if self._client.process_incoming is not None:
+                msg = self._client.process_incoming(msg)
+
+                if msg is None:
+                    return
+            
             # clean msg text to remove callsigns, etc
             if self._client.clean_directed_text:
                 msg = self._client.clean_rx_message_text(msg)
 
             self._spot(msg)
 
         elif msg.type == Message.RIG_FREQ:
@@ -666,15 +699,13 @@
         elif msg.type == Message.RX_CALL_ACTIVITY:
             self.state['call_activity'] = msg.call_activity
 
         elif msg.type == Message.RX_BAND_ACTIVITY:
             self.state['band_activity'] = msg.band_activity
 
         elif msg.type == Message.RX_ACTIVITY:
-            # utilized by activity monitor via callback
             pass
 
         elif msg.type == Message.TX_FRAME:
-            # utilized by tx monitor via callback
             pass
-
+            
         self.append_to_rx_queue(msg)
```

### Comparing `pyjs8call-0.2.0/pyjs8call/message.py` & `pyjs8call-0.2.1/pyjs8call/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     | CMD_RELAY | '>' |
     | CMD_Q | '?' |
     | CMD_FREETEXT | '&nbsp;' &nbsp;&nbsp;(space) |
     | CMD_FREETEXT_2 | '&nbsp;&nbsp;' &nbsp;(space x2) |
     | &nbsp; | &nbsp; |
     | **Commands** | **Value** |
     | AUTOREPLY_COMMANDS | *list* of autoreply commands |
+    | CHECKSUM_COMMANDS | *list* of checksumed commands |
     | COMMANDS | *list* of all commands |
 
     &nbsp;
 
     Statuses:
 
     | Status | Value |
@@ -173,20 +174,23 @@
     Most attributes with a default value of None are included so messages can be handled internally without worrying about the nuances of JS8Call API message attributes, which vary greatly.
 
     Attributes:
         id (str): Random url-safe text string, 16 bytes in length
         type (str): Message type (see static types), defaults to TX_SEND_MESSAGE
         destination (str): Destination callsign
         value (str): Message contents
-        time (str): UTC timestamp (see datetime.now(timezone.utc).timestamp)
-        timestamp (str): Local timestamp (see time.time)
+        time (float): UTC timestamp (see *datetime.now(timezone.utc).timestamp*)
+        timestamp (float): Local timestamp (see *time.time*)
+        local_time_str (str): Local time string (see *time.strftime('%X', time.localtime())*)
+        tdrift (float): Time drift specified by JS8call, defaults to None
         params (dict): Message parameters used by certain JS8Call API messages
         attributes (list): Attributes for internal use (see *Message.set*)
         status (str): Message status (see static statuses), defaults to STATUS_CREATED
         raw (str): Raw message string passed to *Message.parse*, defaults to None
+        packed (bytes): Byte string returned from *pack()*, defaults to None
         freq (str): Dial frequency plus offset frequency in Hz, defaults to None
         dial (str): Dial frequency in Hz, defaults to None
         offset (str): Passband offset frequency in Hz, defaults to None
         call (str): Callsign, used by certain JS8Call API messages, defaults to None
         grid (str): Grid square, default to None
         path (list): Parsed relay path, defaults to None
         snr (str): Signal-to-noise ratio, defaults to None
@@ -198,15 +202,18 @@
         speed (str): JS8Call modem speed of received signal
         extra (str): Used by certain JS8Call API messages, defaults to None
         hearing (list): Response to HEARING? query, defaults to None
         messages (list): Inbox messages, defaults to None
         band_activity (list): JS8Call band activity items, defaults to None
         call_activity (list): JS8Call call activity items, defaults to None
         distance (int): Distance from JS8Call grid square to message grid square, defaults to None
+        distance_units (str): Distance units (mi/km) of *distance*, defaults to None
         bearing (int): Bearing from JS8Call grid square to message grid square, defaults to None
+        profile (str): Active configuration profile when message was received, defaults to None
+        error (str): Error message, defaults to None
 
     *text* is also used to store 'cleaned' incoming message text, see *pyjs8call.client.clean_rx_message_text()*.
     '''
 
     # outgoing message types
     RX_GET_TEXT             = 'RX.GET_TEXT'
     RX_GET_CALL_ACTIVITY    = 'RX.GET_CALL_ACTIVITY'
@@ -301,14 +308,18 @@
     CMD_FREETEXT            = ' '
     CMD_FREETEXT_2          = '  '
 
     COMMANDS = [CMD_HB, CMD_HEARTBEAT, CMD_HEARTBEAT_SNR, CMD_CQ, CMD_SNR_Q, CMD_Q, CMD_GRID_Q, CMD_GRID, CMD_INFO_Q, CMD_INFO, CMD_STATUS_Q, CMD_STATUS, CMD_HEARING_Q, CMD_HEARING, CMD_HW_CPY_Q, CMD_MSG, CMD_MSG_TO, CMD_QUERY, CMD_QUERY_MSGS, CMD_QUERY_MSGS_Q, CMD_QUERY_CALL, CMD_NO, CMD_YES, CMD_AGN_Q, CMD_ACK, CMD_NACK, CMD_DIT_DIT, CMD_FB, CMD_SK, CMD_RR, CMD_QSL, CMD_QSL_Q, CMD_CMD, CMD_SNR, CMD_73, CMD_RELAY, CMD_FREETEXT, CMD_FREETEXT_2]
 
     AUTOREPLY_COMMANDS = [CMD_SNR_Q, CMD_Q, CMD_HEARING_Q, CMD_GRID, CMD_STATUS_Q, CMD_MSG, CMD_MSG_TO, CMD_QUERY, CMD_QUERY_MSGS, CMD_QUERY_MSGS_Q, CMD_QUERY_CALL, CMD_INFO_Q, CMD_AGN_Q, CMD_ACK, CMD_NACK]
 
+    COMMAND_RESPONSES = [CMD_HEARTBEAT_SNR, CMD_SNR, CMD_GRID, CMD_INFO, CMD_STATUS, CMD_HEARING, CMD_NO, CMD_YES, CMD_ACK, CMD_SNR]
+
+    CHECKSUM_COMMANDS = [CMD_RELAY, CMD_MSG, CMD_MSG_TO, CMD_QUERY, CMD_QUERY_MSGS, CMD_QUERY_MSGS_Q, CMD_QUERY_CALL, CMD_CMD]
+
     # status types
     STATUS_CREATED          = 'created'
     STATUS_QUEUED           = 'queued'
     STATUS_SENDING          = 'sending'
     STATUS_SENT             = 'sent'
     STATUS_FAILED           = 'failed'
     STATUS_RECEIVED         = 'received'
@@ -329,30 +340,23 @@
             value (str): Message text to send, defaults to None
 
         Returns:
             pyjs8call.message: Constructed message object
         '''
         self.attributes = []
         self.raw = None
+        self.packed = None
+        self.packed_dict = None
 
-        self.set('id', secrets.token_urlsafe(16))
-        self.set('type', Message.TX_SEND_MESSAGE)
-        self.set('destination', destination)
-        self.set('cmd', cmd)
-        self.set('value', value)
-        self.set('time', datetime.now(timezone.utc).timestamp())
-        self.set('timestamp', time.time())
-        self.set('params', {})
-        self.set('status', Message.STATUS_CREATED)
-        
         # initialize common msg fields
         common = [
             'freq',
             'dial',
             'offset',
+            'tdrift',
             'call',
             'grid',
             'snr',
             'from',
             'origin',
             'utc',
             'path',
@@ -360,19 +364,33 @@
             'speed',
             'extra',
             'hearing',
             'messages',
             'band_activity',
             'call_activity',
             'distance',
-            'bearing'
+            'distance_units',
+            'bearing',
+            'profile',
+            'error'
         ]
 
         for attribute in common:
             self.set(attribute, None)
+        
+        self.set('id', secrets.token_urlsafe(16))
+        self.set('type', Message.TX_SEND_MESSAGE)
+        self.set('destination', destination)
+        self.set('cmd', cmd)
+        self.set('value', value)
+        self.set('time', datetime.now(timezone.utc).timestamp())
+        self.set('timestamp', time.time())
+        self.set('local_time_str', '{}L'.format(time.strftime('%X', time.localtime(self.get('timestamp')))))
+        self.set('params', {})
+        self.set('status', Message.STATUS_CREATED)
 
     def set(self, attribute, value):
         '''Set message attribute value.
 
         Uses *setattr* internally to add attributes to the message object. Added attributes are tracked in the *attributes* attribute. Attributes are converted to lowercase for consistency.
 
         Special attribute handling for consistency:
@@ -471,17 +489,20 @@
                     if isinstance(self.destination, list):
                         # handle relay
                         destination = Message.CMD_RELAY.join(self.destination)
                     else:
                         destination = self.destination
                     
                     if self.cmd is None:
-                        value = destination + ' ' + value
+                        # directed message without command
+                        # note: double space!
+                        value = '{}  {}'.format(destination, value)
                     else:
-                        value = destination + self.cmd + ' ' + value
+                        # directed message with command
+                        value = '{}{} {}'.format(destination, self.cmd, value)
 
                 value = value.strip()
 
             # add to dict if value is set
             if value is not None:
                 data[attribute] = value
 
@@ -496,32 +517,35 @@
         - origin
         - cmd
         - from
         - time
         - timestamp
         - text
         - status
+        - profile
+        - error
 
         Args:
             exclude (list): Attribute names to exclude, defaults to None
             
         Returns:
             UTF-8 encoded byte string. A dictionary representation of the message attributes is converted to a string using *json.dumps* before encoding.
         '''
         if exclude is None:
             exclude = [] 
 
         #TODO make sure 'text' is not used since it is excluded by default
-        exclude.extend(['id', 'destination', 'cmd', 'time', 'timestamp', 'from', 'origin', 'text', 'status'])
+        exclude.extend(['id', 'destination', 'cmd', 'time', 'timestamp', 'from', 'origin', 'text', 'status', 'profile', 'error'])
 
-        data = self.dict(exclude = exclude)
+        self.packed_dict = self.dict(exclude = exclude)
         # convert dict to json string
-        packed = json.dumps(data) + '\r\n'
-        # return bytes
-        return packed.encode('utf-8')
+        packed = json.dumps(self.packed_dict) + '\r\n'
+        self.packed = packed.encode('utf-8')
+
+        return self.packed
 
     def parse(self, msg_str):
         '''Load message string into message object.
 
         *Message.parse* should be called inside a try/except block to handle parsing errors.
 
         Args:
@@ -558,15 +582,17 @@
             for message in msg['params']['MESSAGES']:
                 self.messages.append({
                     'cmd' : message['params']['CMD'],
                     'freq' : message['params']['DIAL'],
                     'offset' : message['params']['OFFSET'],
                     'snr' : message['params']['SNR'],
                     'speed' : message['params']['SUBMODE'],
-                    'time' : message['params']['UTC'],
+                    'time' : message['params']['UTC'] / 1000, # milliseconds to seconds
+                    'timestamp' : time.mktime(time.localtime(value['UTC'] / 1000)), # milliseconds to seconds
+                    'local_time_str' : '{}L'.format(time.strftime('%X', time.localtime(value['UTC'] / 1000))), # milliseconds to seconds
                     'origin' : message['params']['FROM'],
                     'destination' : message['params']['TO'],
                     'path' : message['params']['PATH'],
                     'text' : message['params']['TEXT'].strip(),
                     'value' : message['value'],
                     'status' : message['type'].lower(),
                     'unread': bool(message['type'].lower() == 'unread'),
@@ -577,34 +603,36 @@
             self.call_activity = []
             for key, value in msg['params'].items():
                 if key == '_ID' or value is None:
                     continue
 
                 self.call_activity.append({
                     'origin' : key,
-                    'grid' : value['GRID'],
+                    'grid' : value['GRID'].strip(),
                     'snr' : value['SNR'],
-                    'time' : value['UTC'],
-                    # hearing data added in client.get_call_activity
-                    'hearing': []
+                    'time' : value['UTC'] / 1000, # milliseconds to seconds
+                    'timestamp' : time.mktime(time.localtime(value['UTC'] / 1000)), # milliseconds to seconds
+                    'local_time_str' : '{}L'.format(time.strftime('%X', time.localtime(value['UTC'] / 1000))) # milliseconds to seconds
                 })
 
         #TODO can this replace activity monitor?
         elif self.type == Message.RX_BAND_ACTIVITY:
             self.band_activity = []
             for key, value in msg['params'].items():
                 try:
                     # skip if key is not a freq offset (int)
                     int(key)
 
                     self.band_activity.append({
                         'freq' : value['DIAL'],
                         'offset' : value['OFFSET'],
                         'snr' : value['SNR'],
-                        'time' : value['UTC'],
+                        'time' : value['UTC'] / 1000, # milliseconds to seconds
+                        'timestamp' : time.mktime(time.localtime(value['UTC'] / 1000)), # milliseconds to seconds
+                        'local_time_str' : '{}L'.format(time.strftime('%X', time.localtime(value['UTC'] / 1000))), # milliseconds to seconds
                         'text' : value['TEXT']
                     })
                 except ValueError:
                     continue
 
                 
         # command handling
@@ -684,32 +712,38 @@
         '''
         for attribute, value in json.loads(msg_str).items():
             self.set(attribute, value)
 
     def __eq__(self, msg):
         '''Whether another message is considered equal to self.
 
-        There are two cases where spots are considered equal:
-        - When both messages have the same timestamps (literally the same message)
-        - When both messages have the same origin, offset frequency, and snr (same station event reported by differnt JS8Call API messages at slightly differnt times) 
+        There are multiple cases where spots are considered equal:
+        - When both incoming messages have the same timestamps (literally the same message)
+        - When both incoming messages have the same origin, offset frequency, and snr (same station event reported by differnt JS8Call API messages at slightly differnt times) 
+        - When both outgoing messages have the same timestamp, type, and value
 
         Args:
             msg (pyjs8call.message): Message to compare
 
         Returns:
             bool: Whether the two messages are considered equal
         '''
         if not isinstance(msg, Message):
             return False
 
         # comparing origin, offset, and snr allows equating the same message sent more than once
         # from the js8call application (likely as different message types) at slightly different
         # times (likely milliseconds apart)
-        return bool( self.timestamp == msg.timestamp or
-            (msg.origin == self.origin and msg.offset == self.offset and msg.snr == self.snr) )
+        if msg.type in self.RX_TYPES:
+            return bool( self.timestamp == msg.timestamp or
+                (msg.origin == self.origin and msg.offset == self.offset and msg.snr == self.snr) )
+
+        else:
+            # tx types
+            return bool(msg.type == self.type and msg.value == msg.value and msg.timestamp == self.timestamp)
 
     def __lt__(self, msg):
         '''Whether another message is less than self.
 
         Timestamps are compared.
 
         Args:
@@ -729,7 +763,10 @@
             msg (pyjs8call.message): Message to compare
 
         Returns:
             bool: Whether self.timestamp is greater than the specified msg.timestamp
         '''
         return bool(self.timestamp > msg.timestamp)
 
+    def __repr__(self):
+        return '<Message {}>'.format(self.id)
+
```

### Comparing `pyjs8call-0.2.0/pyjs8call/offsetmonitor.py` & `pyjs8call-0.2.1/pyjs8call/offsetmonitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,40 +62,53 @@
         self.bandwidth_safety_factor = 1.25
         self.offset = self._client.settings.get_offset()
         self.before_transition = 1
         self.activity_cycles = 1.5
         self._enabled = False
         self._paused = False
 
-    def enable_monitoring(self):
+    def enabled(self):
+        '''Get enabled status.
+        
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+        
+        Returns:
+            bool: True if paused, False if running
+        '''
+        return self._paused
+
+    def enable(self):
         '''Enable offset monitoring.'''
         if self._enabled:
             return
 
         self._enabled = True
 
         thread = threading.Thread(target=self._monitor)
         thread.daemon = True
         thread.start()
 
-    def disable_monitoring(self):
+    def disable(self):
         '''Disable offset monitoring.'''
         self._enabled = False
 
-    def pause_monitoring(self):
+    def pause(self):
         '''Pause offset monitoring.'''
         self._paused = True
 
-    def resume_monitoring(self):
+    def resume(self):
         '''Resume offset monitoring.'''
         self._paused = False
 
-    def paused(self):
-        return self._paused
-
     def _min_signal_freq(self, offset, bandwidth):
         '''Get lower edge of signal.
 
         Args:
             offset (int): Signal offset frequency in Hz
             bandwidth (int): Signal bandwidth in Hz
 
@@ -264,29 +277,34 @@
 
         Returns:
             int or None: New offset frequency in Hz, or None if there are no available sections
         '''
         # calculate distance from the current offset to each unused section
         distance = []
 
+        # keep track of unused_spectrum position after distance sort
         i = 0
         for lower_limit, upper_limit in unused_spectrum:
             if upper_limit < self.offset:
                 # below the current offset
                 distance.append( (i, self.offset - upper_limit) )
             elif lower_limit > self.offset:
                 # above the current offset
                 distance.append( (i, lower_limit - self.offset) )
 
             i += 1
 
         # sort by distance from current offset
         distance.sort(key = lambda dist: dist[1])
-        # index of nearest unused section
-        nearest = distance[0][0]
+
+        try:
+            # index of nearest unused section
+            nearest = distance[0][0]
+        except IndexError:
+            return None
 
         # use nearest unused section
         lower_limit = unused_spectrum[nearest][0]
         upper_limit = unused_spectrum[nearest][1]
 
         safe_bandwidth = self.bandwidth * self.bandwidth_safety_factor
```

### Comparing `pyjs8call-0.2.0/pyjs8call/outgoingmonitor.py` & `pyjs8call-0.2.1/pyjs8call/outgoingmonitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
     A message changes to STATUS_QUEUED when monitoring begins.
 
     A message changes to STATUS_SENDING when the destination and value are seen in the JS8Call tx text field and the status of the message is STATUS_QUEUED.
 
     A message changes to STATUS_SENT when the destination and value are no longer seen in the JS8Call tx text field and the status of the message is STATUS_SENDING.
 
-    A message changes to STATUS_FAILED when the message is not sent within 30 tx cycles. Therefore the maximum age of a monitored message depends on the JS8Call modem speed setting:
-    - 3 minutes in turbo mode which has 6 second tx cycles
-    - 5 minutes in fast mode which has 10 second tx cycles
-    - 7.5 minutes in normal mode which has 15 second cycles
-    - 15 minutes in slow mode which has 30 second tx cycles
+    A message changes to STATUS_FAILED when the message is not sent within 600 tx cycles. Therefore the maximum age of a monitored message depends on the JS8Call modem speed setting:
+    - 6 minutes in turbo mode which has 6 second tx cycles
+    - 10 minutes in fast mode which has 10 second tx cycles
+    - 15 minutes in normal mode which has 15 second cycles
+    - 30 minutes in slow mode which has 30 second tx cycles
 
     A message is dropped from the monitoring queue once the status is set to STATUS_SENT or STATUS_FAILED.
     '''
 
     def __init__(self, client):
         '''Initialize outgoing message monitor.
 
@@ -67,32 +67,62 @@
             client (pyjs8call.client): Parent client object
 
         Returns:
             pyjs8call.outgoingmonitor: Constructed outgoing message monitor object
         '''
         self._client = client
         self._enabled = False
+        self._paused = False
         self._msg_queue = []
         self._msg_queue_lock = threading.Lock()
-        # initialize msg max age to 30 tx cycles in fast mode (10 sec cycles)
-        self._msg_max_age = 10 * 30 # 5 minutes
+        # initialize msg max age to 10 minutes
+        self._msg_max_age = 10 * 60 # 10 minutes
 
-    def enable_monitoring(self):
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+
+        Returns:
+            bool: True if paused, False if running
+        '''
+        return self._paused
+
+    def enable(self):
+        '''Enable outgoing message monitoring.'''
         if self._enabled:
             return
 
         self._enabled = True
 
         thread = threading.Thread(target=self._monitor)
         thread.daemon = True
         thread.start()
 
-    def disable_monitoring(self):
+    def disable(self):
+        '''Disable outgoing message monitoring.
+        
+        **Caution**: Internal processes rely on the transmit text field state updates performed by this module.
+        '''
         self._enabled = False
 
+    def pause(self):
+        '''Pause outgoing message monitoring.'''
+        self._paused = True
+
+    def resume(self):
+        '''Resume outgoing message monitoring.'''
+        self._paused = False
+
     def _callback(self, msg):
         '''Handle callback for monitored message status change.
 
         Calls the *pyjs8call.client.callback.outgoing* callback function.
 
         Args:
             msg (pyjs8call.message): Monitored message with changed status
@@ -110,54 +140,68 @@
         Args:
             msg (pyjs8call.message): Message to look for in the JS8Call tx text field
         '''
         msg.status = Message.STATUS_QUEUED
 
         with self._msg_queue_lock:
             self._msg_queue.append(msg)
-
+            
     def _monitor(self):
         '''Tx monitor thread.'''
         while self._enabled:
             time.sleep(0.5)
+
+            if self._paused:
+                continue
+
             # other modules rely on tx text updates from JS8Call
             tx_text = self._client.get_tx_text()
 
             if tx_text is None:
-                continue
+                tx_text = ''
 
             # drop the first callsign and strip spaces and end-of-message
             # original format: 'callsign: callsign  message'
             if ':' in tx_text:
                 tx_text = tx_text.split(':')[1].strip(' ' + Message.EOM)
             
-            # update msg max age based on speed setting (30 tx cycles)
-            self._msg_max_age = self._client.settings.get_window_duration() * 30
+            # update msg max age based on speed setting (60 tx cycles)
+            self._msg_max_age = self._client.settings.get_window_duration() * 60
             
             with self._msg_queue_lock:
                 self._process_queue(tx_text)
 
     def _process_queue(self, tx_text):
         '''Compare queued message to tx text.'''
+        tx_text_wo_checksum = ' '.join(tx_text.split()[:-1])
+
         for i in range(len(self._msg_queue)):
             msg = self._msg_queue.pop(0)
-            msg_value = msg.dict()['value'].strip()
 
-            if msg_value == tx_text and msg.status == Message.STATUS_QUEUED:
+            if msg.packed_dict is None:
+                msg.pack()
+
+            msg_value = msg.packed_dict['value'].strip()
+
+            if (
+                ( (msg.cmd in Message.CHECKSUM_COMMANDS and msg_value == tx_text_wo_checksum) or msg_value == tx_text ) and
+                msg.status == Message.STATUS_QUEUED
+            ):
                 # msg text was added to js8call tx field, sending
-                msg.status = Message.STATUS_SENDING
+                msg.set('status', Message.STATUS_SENDING)
                 self._callback(msg)
-            elif msg_value != tx_text and msg.status == Message.STATUS_SENDING:
+            elif msg_value != tx_text_wo_checksum and msg_value != tx_text and msg.status == Message.STATUS_SENDING:
                 # msg text was removed from js8call tx field, sent
-                msg.status = Message.STATUS_SENT
+                msg.set('status', Message.STATUS_SENT)
                 self._callback(msg)
                 # msg dropped from queue
                 return None
             elif time.time() > msg.timestamp + self._msg_max_age:
                 # msg too old, sending failed
-                msg.status = Message.STATUS_FAILED
+                msg.set('status', Message.STATUS_FAILED)
+                msg.error = 'failed to send'
                 self._callback(msg)
                 # msg dropped from queue
                 return None
 
             self._msg_queue.append(msg)
```

### Comparing `pyjs8call-0.2.0/pyjs8call/spotmonitor.py` & `pyjs8call-0.2.1/pyjs8call/spotmonitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,63 +49,89 @@
             client (pyjs8call.client): Parent client object
 
         Returns:
             pyjs8call.spotmonitor: Constructed spot monitor object
         '''
         self._client = client
         self._enabled = False
+        self._paused = False
         self._station_watch_list = []
         self._group_watch_list = []
-        self._spots_lock = threading.Lock()
 
-    def enable_monitoring(self):
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+
+        Returns:
+            bool: True if paused, False if running
+        '''
+        return self._paused
+
+    def enable(self):
         '''Enable spot monitoring.'''
         if self._enabled:
             return
 
         self._enabled = True
 
         thread = threading.Thread(target=self._monitor)
         thread.daemon = True
         thread.start()
 
-    def disable_monitoring(self):
+    def disable(self):
         '''Disable spot monitoring.'''
         self._enabled = False
 
+    def pause(self):
+        '''Pause spot monitoring.'''
+        self._paused = True
+
+    def resume(self):
+        '''Resume spot monitoring.'''
+        self._paused = False
+
     def all(self):
         '''Get all stored spot messages.'''
-        with self._spots_lock:
+        with self._client.js8call._spots_lock:
             return self._client.js8call.get_spots()
 
-    def filter(self, origin=None, destination=None, distance=0, age=0, count=0):
+    def filter(self, origin=None, destination=None, distance=0, age=0, count=0, profile=None):
         '''Get filtered spot messages.
 
         Spots are *pyjs8call.message* objects. Specified *origin* and *destination* strings are converted to uppercase.
 
         When *distance*, *age*, or *count* are 0 (zero) they are ignored.
 
         Args:
             origin (str): Message origin callsign to match
             destination (str): Message destination callsign or group designator to match
             distance (int): Maximum message grid square distance, defaults to 0 (zero)
             age (int): Maximum message age in seconds, defaults to 0 (zero)
             count (int): Number of most recent spot messages to return, defaults to 0 (zero)
+            profile (str): Configuration profile at the time spot was sent or received, defaults to None
 
         Returns:
             list: Spot messages matching specified filter criteria
         '''
         spots = []
-        with self._spots_lock:
+        with self._client.js8call._spots_lock:
             for spot in self._client.js8call.get_spots():
                 if (
                     (age == 0 or spot.age() <= age) and
                     (distance == 0 or (spot.distance is not None and spot.distance <= distance)) and
                     (origin is None or origin.upper() == spot.origin) and 
-                    (destination is None or destination.upper() == spot.destination)
+                    (destination is None or destination.upper() == spot.destination) and
+                    (profile is None or profile == spot.profile)
                 ):
                     spots.append(spot)
 
         if 0 < count < len(spots):
             count *= -1
             spots = spots[count:]
 
@@ -117,15 +143,15 @@
         Args:
             count (int): Number of spot messages to return
 
         Returns:
             list: Last *count* spot messages received
         '''
         count *= -1
-        with self._spots_lock:
+        with self._client.js8call._spots_lock:
             return self._client.js8call.get_spots()[count:]
 
     def add_station_watch(self, station):
         '''Add watched station.
 
         Args:
             station (str): Station callsign to watch for
@@ -218,14 +244,17 @@
         Uses *filter()* internally.
         '''
         last_spot_update_timestamp = 0
 
         while self._enabled:
             self._client.window.sleep_until_next_transition()
 
+            if self._paused:
+                continue
+
             # get new spots since last update
             time_since_last_update = time.time() - last_spot_update_timestamp
             new_spots = self.filter(age = time_since_last_update)
             last_spot_update_timestamp = time.time()
 
             if len(new_spots) > 0:
                 self._callback(new_spots)
```

### Comparing `pyjs8call-0.2.0/pyjs8call/timemonitor.py` & `pyjs8call-0.2.1/pyjs8call/timemonitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,67 @@
         self._client = client
         self._enabled = False
         self._paused = False
         self._searching = False
         self._search_activity = []
         self._drift = self._client.config.get('MainWindow', 'TimeDrift', value_type=int)
 
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+
+        Returns:
+            bool: True if paused, False if running
+        '''
+        return self._paused
+
+    def enable(self, station=None, group='@TIME', interval=60, threshold=0.5, age=15):
+        '''Enable automatic time drift monitoring.
+        
+        Uses *sync_to_group()* if *group* is specified (default).
+        
+        Uses *sync_to_station()* if *station* is specified.
+        
+        Uses *sync_to_activity()* if *group* and *station* are both None.
+        
+        Args:
+            station (str): Station callsign to sync time drift to, defaults to None
+            group (str): Group designator to sync time drift to, defaults to '@TIME'
+            interval (int): Number of minutes between sync attempts, defaults to 60
+            threshold (float): Time drift in seconds to exceed before syncing, defaults to 0.5
+            age (int): Maximum age of activity in minutes, defaults to 15
+        '''
+        if self._enabled:
+            return
+        
+        self._enabled = True
+        
+        thread = threading.Thread(target=self._monitor, args=(station, group, interval, threshold, age))
+        thread.daemon = True
+        thread.start()
+
+    def disable(self):
+        '''Disable automatic time drift monitoring.'''
+        self._enabled = False
+
+    def pause(self):
+        '''Pause automatic time drift monitoring.'''
+        self._paused = True
+        
+    def resume(self):
+        '''Resume automatic time drift monitoring.'''
+        self._paused = False
+        
     def get_drift(self):
         '''Get current time drift.
 
         Time drift changes are tracked internally when *set_drift()* is called.
 
         Note that if time drift is changed via the JS8Call user interface this function will return the incorrect time drift. Time drift information is only saved to the configuration file on exit and is not available via the JS8Call API while the application is running.
 
@@ -355,51 +408,14 @@
 
         Args:
             threshold (float): Median time drift in seconds to exceed before syncing, defaults to 0.5
             age (int): Maximum age of activity in minutes, defaults to 15
         '''
         return self.sync_to_group('@TIME', threshold = threshold, age = age)
 
-    def enable_auto_sync(self, station=None, group='@TIME', interval=60, threshold=0.5, age=15):
-        '''Enable automatic time drift monitoring.
-        
-        Uses *sync_to_group()* if *group* is specified (default).
-        
-        Uses *sync_to_station()* if *station* is specified.
-        
-        Uses *sync_to_activity()* if *group* and *station* are both None.
-        
-        Args:
-            station (str): Station callsign to sync time drift to, defaults to None
-            group (str): Group designator to sync time drift to, defaults to '@TIME'
-            interval (int): Number of minutes between sync attempts, defaults to 60
-            threshold (float): Time drift in seconds to exceed before syncing, defaults to 0.5
-            age (int): Maximum age of activity in minutes, defaults to 15
-        '''
-        if self._enabled:
-            return
-        
-        self._enabled = True
-        
-        thread = threading.Thread(target=self._monitor, args=(station, group, interval, threshold, age))
-        thread.daemon = True
-        thread.start()
-
-    def disable_auto_sync(self):
-        '''Disable automatic time drift monitoring.'''
-        self._enabled = False
-
-    def pause_auto_sync(self):
-        '''Pause automatic time drift monitoring.'''
-        self._paused = True
-        
-    def resume_auto_sync(self):
-        '''Resume automatic time drift monitoring.'''
-        self._paused = False
-        
     def _restart_client(self):
         '''Restart client when there is no activity.'''
         self._client.js8call.block_until_inactive()
         self._client.restart()
 
     def _monitor(self, station, group, interval, threshold, age):
         '''Auto time drift sync thread.'''
@@ -442,14 +458,31 @@
             client (pyjs8call.client): Parent client object
             
         Returns:
             pyjs8call.timemonitor.TimeMaster: Constructed time master object
         '''
         self._client = client
         self._enabled = False
+        self._paused = False
+
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def paused(self):
+        '''Get paused status.
+        
+        Returns:
+            bool: True if paused, False if running
+        '''
+        return self._paused
 
     def enable(self, destination='@TIME', message='SYNC', interval=10):
         '''Enable automatic time master messaging.
     
         Note that *destination* can technically be set to a specific callsign. However, this may prevent other stations from synchronizing with the master station.
         
         Note that receiving stations will recognize incoming messages as a directed message (which result in a spot) unless a message is included.
@@ -467,24 +500,31 @@
         thread = threading.Thread(target=self._monitor, args=(destination, message, interval))
         thread.daemon = True
         thread.start()
 
     def disable(self):
         '''Disable time master messaging.'''
         self._enabled = False
+
+    def pause(self):
+        '''Pause time master.'''
+        self._paused = True
+
+    def resume(self):
+        '''Resume time master.'''
+        self._paused = False
         
     def _monitor(self, destination, message, interval):
         '''Time master message transmit thread.
 
         See *TimeMaster.enable()* for argument details.
         '''
         interval *= 60
         last_outgoing_timestamp = 0
         
         while self._enabled:
-            if last_outgoing_timestamp + interval < time.time():
+            if last_outgoing_timestamp + interval < time.time() and not self._paused:
                 text = destination + ' ' + message
-                    
                 self._client.send_message(text.strip())
                 last_outgoing_timestamp = time.time()
 
             time.sleep(1)
```

### Comparing `pyjs8call-0.2.0/pyjs8call/windowmonitor.py` & `pyjs8call-0.2.1/pyjs8call/windowmonitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,76 +56,88 @@
             client (pyjs8call.client): Parent client object
 
         Returns:
             pyjs8call.windowmonitor: Constructed window monitor object
         '''
         self._client = client
         self._enabled = False
-        self._last_tx_frame_timestamp = 0
+        self._last_rig_ptt_timestamp = 0
         self._last_rx_msg_timestamp = 0
         self._next_window_timestamp = 0
         self._timestamp_lock = threading.Lock()
-        self._ignore_next_tx_frame = False
 
-    def enable_monitoring(self):
+    def enabled(self):
+        '''Get enabled status.
+
+        Returns:
+            bool: True if enabled, False if disabled
+        '''
+        return self._enabled
+
+    def enable(self):
         '''Enable rx/tx window monitoring.'''
         if self._enabled:
             return
 
         self._enabled = True
         
-        self._client.callback.register_incoming(self.process_tx_frame, message_type = Message.TX_FRAME)
+        self._client.callback.register_incoming(self.process_rig_ptt, message_type = Message.RIG_PTT)
         self._client.callback.register_incoming(self.process_rx_msg, message_type = Message.RX_DIRECTED)
         self._client.callback.register_incoming(self.process_rx_msg, message_type = Message.RX_ACTIVITY)
 
         thread = threading.Thread(target = self._monitor)
         thread.daemon = True
         thread.start()
 
-    def disable_monitoring(self):
-        '''Disable rx/tx window monitoring.'''
+    def disable(self):
+        '''Disable rx/tx window monitoring.
+
+        **Caution**: Many internal modules depend on the window monitor to function. Only disable this module if you understand what you are doing.
+        '''
         self._enabled = False
         self._client.callback.remove_incoming(self.process_rx_msg)
-        self._client.callback.remove_incoming(self.process_tx_frame)
+        self._client.callback.remove_incoming(self.process_rig_ptt)
+
+    def reset(self):
+        '''Reset rx/tx window monitoring timestamps.
+
+        This function is used internally during restart.
+        '''
+        self._next_window_timestamp = 0
+        self._last_rig_ptt_timestamp = 0
+        self._last_rx_msg_timestamp = 0
 
     def _callback(self):
         '''Window transition callback function handling.
 
         Calls the *pyjs8call.client.callback.window* callback function using *threading.Thread*.
         '''
         if self._client.callback.window is not None:
             thread = threading.Thread(target = self._client.callback.window)
             thread.daemon = True
             thread.start()
 
-    def ignore_next_tx_frame(self):
-        '''Ignore the next tx frame.
-
-        Used to ignore outgoing messages that may cause cumulative tx frame offset errors when there are no other outgoing messages (ex. pyjs8call heartbeat networking messages).
-        '''
-        self._ignore_next_tx_frame = True
-
-    def process_tx_frame(self, msg):
-        '''Process tx frame message.
+    def process_rig_ptt(self, msg):
+        '''Process rig ptt message.
 
         This function is for internal use only.
 
-        Use the timestamp of a tx frame API message to mark the beginning of a rx/tx window transition.
+        Use the timestamp of a PTT API message to mark the rx/tx window transition.
 
         Args:
-            msg (pyjs8call.message): Tx frame message object
+            msg (pyjs8call.message): Rig PTT message object
         '''
-        if self._ignore_next_tx_frame:
-            self._ignore_next_tx_frame = False
+        # ignore ptt off messages
+        if not msg.ptt:
             return
 
         window_duration = self._client.settings.get_window_duration()
 
         with self._timestamp_lock:
-            self._last_tx_frame_timestamp = msg.timestamp
+            self._last_rig_ptt_timestamp = msg.timestamp
             self._next_window_timestamp = msg.timestamp + window_duration
 
     def process_rx_msg(self, msg):
         '''Process incoming message.
 
         This function is for internal use only.
 
@@ -234,7 +246,8 @@
                     self._callback()
                     # update window duration in case speed setting changed
                     window_duration = self._client.settings.get_window_duration()
                     # increament the window timestamp
                     self._next_window_timestamp += window_duration
 
             time.sleep(0.01)
+
```

### Comparing `pyjs8call-0.2.0/pyjs8call.egg-info/PKG-INFO` & `pyjs8call-0.2.1/pyjs8call.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyjs8call
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package for interfacing with the JS8Call API
 Home-page: https://github.com/simplyequipped/pyjs8call
 Author: Simply Equipped LLC
 Author-email: howard@simplyequipped.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
+Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![pypi version](https://img.shields.io/pypi/v/pyjs8call?color=blue&label=pypi%20version)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![pypi downloads](https://img.shields.io/pypi/dw/pyjs8call?color=blue&label=pypi%20downloads)](https://pypi.org/project/pyjs8call) &nbsp;&nbsp;&nbsp;
 [![github license](https://img.shields.io/github/license/simplyequipped/pyjs8call?color=blue)](https://github.com/simplyequipped/pyjs8call/blob/main/LICENSE)
 
@@ -135,17 +133,17 @@
 
 Time master functionality is also implemented which sends outgoing messages on a time interval that other stations can use to synchronize their time drift. Targets the @TIME group by default.
 
 **Inbox Monitor** (pyjs8call.inboxmonitor)
 
 Monitors the local inbox. Notification of new messages is handled via callback function.
 
-**Idle Monitor** (pyjs8call.idlemonitor)
+**Schedule Monitor** (pyjs8call.schedulemonitor)
 
-Monitors the JS8Call application process run time and restarts the application perodically (when there is no outgoing activity) to avoid the JS8Call idle timeout. This is useful when running the JS8Call application headless.
+Monitors configured schedule entries and applies the necessary setting changes at the scheduled time. Settings that can be changed on a schedule include frequency, modem speed, and configuration profile.
 
 &nbsp;  
 
 ### Examples
 
 Basic usage:
 ```
@@ -183,14 +181,32 @@
 js8call.spots.filter(distance = 1000)
 
 # get a list of spot messages in the last 15 minutes
 max_age = 15 * 60 # convert minutes to seconds
 js8call.spots.filter(age = max_age)
 ```
 
+Run multiple JS8Call instances:
+```
+import pyjs8call
+
+# Option A: use the standard network port and no rig name for the primary instance
+js8call = pyjs8call.Client()
+js8call.start()
+
+# Option B: specify a network port and rig name for the primary instance
+#js8call_ft857 = pyjs8call.Client(port=2443)
+#js8call_ft857.start(args=['--rig-name', 'FT857'])
+
+# specify a different network port for the secondary instance
+js8call_qdx = pyjs8call.Client(port=2444)
+# specify the rig name as a command line argument
+js8call_qdx.start(args=['--rig-name', 'QDX'])
+```
+
 Using the spot monitor:
 ```
 import pyjs8call
 
 # callback function for all new spots
 def new_spots(spots):
     for spot in spots:
@@ -235,15 +251,15 @@
 
 js8call = pyjs8call.Client()
 # set inbox monitor callback
 js8call.callback.inbox = new_inbox_msg
 js8call.start()
 
 # enable local inbox monitoring and periodic remote inbox message query
-js8call.inbox.enable_monitoring()
+js8call.inbox.enable()
 ```
 
 Using the outgoing message monitor:
 ```
 import pyjs8call
 
 # callback function for message status change
@@ -268,15 +284,42 @@
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
 js8call.start()
 
 # use default 10 minute interval
-js8call.heartbeat.enable_networking()
+js8call.heartbeat.enable()
+```
+
+Using the schedule monitor:
+```
+import pyjs8call
+
+# callback function for schedule entry activation
+def schedule_activation(schedule_entry):
+    print('Activating ' + repr(schedule_entry))
+
+js8call = pyjs8call.Client()
+# set schedule activation callback
+js8call.callbacks.schedule = schedule_activation
+js8call.start()
+
+# return to the current configuration later
+js8call.schedule.add('14:00')
+# change configuration profile and set frequency and modem speed
+js8call.schedule.add('8:00', 7078000, 'normal', 'QDX')
+# change frequency only
+js8call.schedule.add('9:00', 7074000)
+# remove schedule entry
+js8call.schedule.remove('9:00')
+
+# print formatted information for each schedule entry
+for entry in js8call.schedule.get_schedule():
+    print(str(entry))
 ```
 
 Set config file settings:
 ```
 import pyjs8call
 
 js8call = pyjs8call.Client()
@@ -315,9 +358,7 @@
 ### Acknowledgements
 
 Inspired by [js8net](https://github.com/jfrancis42/js8net) by N0GQ<br>
 [JS8Call](http://js8call.com) by KN4CRD
 
 &nbsp;
 
-
-
```

### Comparing `pyjs8call-0.2.0/pyjs8call.egg-info/SOURCES.txt` & `pyjs8call-0.2.1/pyjs8call.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 README.md
 setup.py
 pyjs8call/__init__.py
 pyjs8call/appmonitor.py
 pyjs8call/client.py
 pyjs8call/confighandler.py
 pyjs8call/hbnetwork.py
-pyjs8call/idlemonitor.py
 pyjs8call/inboxmonitor.py
 pyjs8call/js8call.py
 pyjs8call/message.py
 pyjs8call/offsetmonitor.py
 pyjs8call/outgoingmonitor.py
+pyjs8call/schedulemonitor.py
 pyjs8call/spotmonitor.py
 pyjs8call/timemonitor.py
 pyjs8call/windowmonitor.py
 pyjs8call.egg-info/PKG-INFO
 pyjs8call.egg-info/SOURCES.txt
 pyjs8call.egg-info/dependency_links.txt
 pyjs8call.egg-info/requires.txt
-pyjs8call.egg-info/top_level.txt
+pyjs8call.egg-info/top_level.txt
+tests/test_cross_platform.py
+tests/test_helpers.py
+tests/test_start.py
```

### Comparing `pyjs8call-0.2.0/setup.py` & `pyjs8call-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyjs8call',
-    version='0.2.0',
+    version='0.2.1',
     author='Simply Equipped LLC',
     author_email='howard@simplyequipped.com',
     description='Python package for interfacing with the JS8Call API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/simplyequipped/pyjs8call',
     packages=setuptools.find_packages(),
@@ -17,9 +17,9 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows'
     ],
-    python_requires='>=3.6'
+    python_requires='>=3.6.1'
 )
```

