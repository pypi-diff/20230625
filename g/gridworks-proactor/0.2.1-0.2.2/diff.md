# Comparing `tmp/gridworks_proactor-0.2.1.tar.gz` & `tmp/gridworks_proactor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.2.1.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.2.2.tar", max compression
```

## Comparing `gridworks_proactor-0.2.1.tar` & `gridworks_proactor-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1070 2023-05-15 19:10:11.078098 gridworks_proactor-0.2.1/LICENSE
--rw-r--r--   0        0        0     4286 2023-05-15 19:10:11.078098 gridworks_proactor-0.2.1/README.md
--rw-r--r--   0        0        0     2390 2023-05-15 19:10:27.823119 gridworks_proactor-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2304 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4109 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0      373 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     3107 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0      677 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0     1775 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/__init__.py
--rw-r--r--   0        0        0     2932 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/acks.py
--rw-r--r--   0        0        0      514 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/asyncio_timer_manager.py
--rw-r--r--   0        0        0    16554 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/link_manager.py
--rw-r--r--   0        0        0    16232 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/link_state.py
--rw-r--r--   0        0        0     2220 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/message_times.py
--rw-r--r--   0        0        0    11137 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/mqtt.py
--rw-r--r--   0        0        0     1487 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/links/timer_interface.py
--rw-r--r--   0        0        0     5557 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/logger.py
--rw-r--r--   0        0        0     4184 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7718 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/message.py
--rw-r--r--   0        0        0    13287 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/persister.py
--rw-r--r--   0        0        0    23176 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     3448 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/stats.py
--rw-r--r--   0        0        0     9207 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     6070 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     1491 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     6602 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     6895 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20076 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      401 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2565 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      195 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2197 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     2388 2023-05-15 19:10:11.082098 gridworks_proactor-0.2.1/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0     9334 2023-05-15 19:10:11.086098 gridworks_proactor-0.2.1/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    47306 2023-05-15 19:10:11.086098 gridworks_proactor-0.2.1/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     2936 2023-05-15 19:10:11.086098 gridworks_proactor-0.2.1/src/gwproactor_test/wait.py
--rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 gridworks_proactor-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-25 19:59:33.144424 gridworks_proactor-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4286 2023-06-25 19:59:33.144424 gridworks_proactor-0.2.2/README.md
+-rw-r--r--   0        0        0     2390 2023-06-25 19:59:50.624567 gridworks_proactor-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2304 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0     1610 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4109 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0      373 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     3107 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0      677 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0     1775 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/__init__.py
+-rw-r--r--   0        0        0     2932 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/acks.py
+-rw-r--r--   0        0        0      514 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/asyncio_timer_manager.py
+-rw-r--r--   0        0        0    16554 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/link_manager.py
+-rw-r--r--   0        0        0    16232 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/link_state.py
+-rw-r--r--   0        0        0     2220 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/message_times.py
+-rw-r--r--   0        0        0    11137 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/mqtt.py
+-rw-r--r--   0        0        0     1487 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/links/timer_interface.py
+-rw-r--r--   0        0        0     5557 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     4184 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7718 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/message.py
+-rw-r--r--   0        0        0    13287 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    23176 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     3448 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     3714 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     9207 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     6070 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     1487 2023-06-25 19:59:50.624567 gridworks_proactor-0.2.2/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     6602 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     6895 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20073 2023-06-25 19:59:50.624567 gridworks_proactor-0.2.2/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      401 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2565 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      195 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2197 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     2388 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0     9334 2023-06-25 19:59:33.148424 gridworks_proactor-0.2.2/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    47301 2023-06-25 19:59:50.624567 gridworks_proactor-0.2.2/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 gridworks_proactor-0.2.2/PKG-INFO
```

### Comparing `gridworks_proactor-0.2.1/LICENSE` & `gridworks_proactor-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/README.md` & `gridworks_proactor-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/pyproject.toml` & `gridworks_proactor-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.2.1"
+version = "0.2.2"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
@@ -25,15 +25,15 @@
 python-dotenv = "^1.0.0"
 pendulum = "^2.1.2"
 xdg = "^6.0.0"
 paho-mqtt = "^1.6.1"
 result = "^0.9.0"
 pytest = {version = "^7.2.0", optional = true}
 pytest-asyncio = {version = "^0.20.3", optional = true}
-gridworks-protocol = ">=0.3.6"
+gridworks-protocol = ">=0.5.5"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
```

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/__init__.py` & `gridworks_proactor-0.2.2/src/gwproactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.2.2/src/gwproactor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/config/logging.py` & `gridworks_proactor-0.2.2/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/config/paths.py` & `gridworks_proactor-0.2.2/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.2.2/src/gwproactor/config/proactor_settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/__init__.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/acks.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/acks.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/asyncio_timer_manager.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/asyncio_timer_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/link_manager.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/link_manager.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/link_state.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/link_state.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/message_times.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/message_times.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/mqtt.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/links/timer_interface.py` & `gridworks_proactor-0.2.2/src/gwproactor/links/timer_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/logger.py` & `gridworks_proactor-0.2.2/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.2.2/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/message.py` & `gridworks_proactor-0.2.2/src/gwproactor/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/persister.py` & `gridworks_proactor-0.2.2/src/gwproactor/persister.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/proactor_implementation.py` & `gridworks_proactor-0.2.2/src/gwproactor/proactor_implementation.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.2.2/src/gwproactor/proactor_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/problems.py` & `gridworks_proactor-0.2.2/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/stats.py` & `gridworks_proactor-0.2.2/src/gwproactor/stats.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.2.2/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor/watchdog.py` & `gridworks_proactor-0.2.2/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/__init__.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+from gridworks_test.wait import AwaitablePredicate
+from gridworks_test.wait import ErrorStringFunction
+from gridworks_test.wait import Predicate
+from gridworks_test.wait import StopWatch
+from gridworks_test.wait import await_for
+
 from gwproactor_test.clean import DefaultTestEnv
 from gwproactor_test.clean import clean_test_env
 from gwproactor_test.clean import default_test_env
 from gwproactor_test.comm_test_helper import CommTestHelper
 from gwproactor_test.comm_test_helper import ProactorTestHelper
 from gwproactor_test.logger_guard import LoggerGuard
 from gwproactor_test.logger_guard import LoggerGuards
 from gwproactor_test.logger_guard import restore_loggers
 from gwproactor_test.proactor_recorder import ProactorT
 from gwproactor_test.proactor_recorder import RecorderInterface
 from gwproactor_test.proactor_recorder import RecorderLinkStats
 from gwproactor_test.proactor_recorder import RecorderStats
 from gwproactor_test.proactor_recorder import make_recorder_class
 from gwproactor_test.proactor_test_collections import ProactorCommTests
-from gwproactor_test.wait import AwaitablePredicate
-from gwproactor_test.wait import ErrorStringFunction
-from gwproactor_test.wait import Predicate
-from gwproactor_test.wait import StopWatch
-from gwproactor_test.wait import await_for
 
 
 __all__ = [
     "DefaultTestEnv",
     "clean_test_env",
     "default_test_env",
     "CommTestHelper",
```

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/clean.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/clean.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/comm_test_helper.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.2.2/src/gwproactor_test/config/hardware-layout.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921052631578948%*

 * *Differences: {"'MyAtomicTNodeGNode'": "{'Alias': 'd1.isone.ct.newhaven.orange1'}",*

 * * "'MyScadaGNode'": "{'Alias': 'd1.isone.ct.newhaven.orange1.ta.scada'}",*

 * * "'MyTerminalAssetGNode'": "{'Alias': 'd1.isone.ct.newhaven.orange1.ta'}"}*

```diff
@@ -51,29 +51,29 @@
             "HwUid": "1001ab",
             "TypeAlias": "gt.electric.meter.component.100"
         }
     ],
     "MultipurposeSensorCacs": [],
     "MultipurposeSensorComponents": [],
     "MyAtomicTNodeGNode": {
-        "Alias": "dw1.isone.ct.newhaven.orange1",
+        "Alias": "d1.isone.ct.newhaven.orange1",
         "DisplayName": "Little Orange House Garage Heating System AtomicTNode",
         "GNodeId": "c4c9a280-453f-4c36-a081-970a3774b3ed",
         "GNodeStatusValue": "Active",
         "PrimaryGNodeRoleAlias": "AtomicTNode"
     },
     "MyScadaGNode": {
-        "Alias": "dw1.isone.ct.newhaven.orange1.ta.scada",
+        "Alias": "d1.isone.ct.newhaven.orange1.ta.scada",
         "DisplayName": "Little Orange House Garage Heating System SCADA",
         "GNodeId": "c9794c6d-e013-4d74-9570-f9ba4b0f0b0d",
         "GNodeStatusValue": "Active",
         "PrimaryGNodeRoleAlias": "Scada"
     },
     "MyTerminalAssetGNode": {
-        "Alias": "dw1.isone.ct.newhaven.orange1.ta",
+        "Alias": "d1.isone.ct.newhaven.orange1.ta",
         "DisplayName": "Little Orange House Garage Heating System TerminalAsset",
         "GNodeId": "e250a99c-7b7f-469a-8f54-96ea83e95112",
         "GNodeStatusValue": "Active",
         "PrimaryGNodeRoleAlias": "TerminalAsset"
     },
     "OtherCacs": [
         {
```

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/dummies/child/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/proactor_recorder.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.2.1/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.2.2/src/gwproactor_test/proactor_test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import pytest
 from gwproto import MQTTTopic
 from paho.mqtt.client import MQTT_ERR_CONN_LOST
 
 from gwproactor.links import StateName
 from gwproactor.message import DBGPayload
+from gwproactor_test import await_for
 from gwproactor_test.comm_test_helper import CommTestHelper
-from gwproactor_test.wait import await_for
 
 
 @pytest.mark.asyncio
 class ProactorCommTests:
     CTH: Type[CommTestHelper]
 
     async def test_no_parent(self):
```

### Comparing `gridworks_proactor-0.2.1/PKG-INFO` & `gridworks_proactor-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gridworks-proactor
-Version: 0.2.1
+Version: 0.2.2
 Summary: Gridworks Proactor
 Home-page: https://github.com/thegridelectric/gridworks-proactor
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: tests
-Requires-Dist: gridworks-protocol (>=0.3.6)
+Requires-Dist: gridworks-protocol (>=0.5.5)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "tests"
 Requires-Dist: pytest-asyncio (>=0.20.3,<0.21.0) ; extra == "tests"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: result (>=0.9.0,<0.10.0)
```

