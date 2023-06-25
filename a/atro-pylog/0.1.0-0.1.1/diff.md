# Comparing `tmp/atro-pylog-0.1.0.tar.gz` & `tmp/atro-pylog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.1.0.tar", last modified: Sun Jun 25 09:29:57 2023, max compression
+gzip compressed data, was "atro-pylog-0.1.1.tar", last modified: Sun Jun 25 10:17:29 2023, max compression
```

## Comparing `atro-pylog-0.1.0.tar` & `atro-pylog-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.1.0/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)      103 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1776 2023-06-25 09:25:57.000000 atro-pylog-0.1.0/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1050 2023-06-24 13:08:30.000000 atro-pylog-0.1.0/pylog/level.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      363 2023-06-24 13:08:30.000000 atro-pylog-0.1.0/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1182 2023-06-25 09:14:57.000000 atro-pylog-0.1.0/pylog/opentelemetry_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      127 2023-06-25 09:16:13.000000 atro-pylog-0.1.0/pylog/rich_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      660 2023-06-25 09:22:59.000000 atro-pylog-0.1.0/pylog/settings.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1086 2023-06-25 09:29:53.000000 atro-pylog-0.1.0/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.1.1/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      103 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1763 2023-06-25 09:30:27.000000 atro-pylog-0.1.1/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1050 2023-06-24 13:08:30.000000 atro-pylog-0.1.1/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      363 2023-06-24 13:08:30.000000 atro-pylog-0.1.1/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1106 2023-06-25 09:30:29.000000 atro-pylog-0.1.1/pylog/opentelemetry_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      127 2023-06-25 09:16:13.000000 atro-pylog-0.1.1/pylog/rich_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      766 2023-06-25 10:09:27.000000 atro-pylog-0.1.1/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1086 2023-06-25 10:17:11.000000 atro-pylog-0.1.1/setup.py
```

### Comparing `atro-pylog-0.1.0/PKG-INFO` & `atro-pylog-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.1.0/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.1.1/atro_pylog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.1.0/pylog/__init__.py` & `atro-pylog-0.1.1/pylog/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import logging
 import sys
 import traceback
 from pathlib import Path
 
 sys.path.append(Path(__file__).resolve().parent.parent.as_posix())
 
+from pylog.level import level_to_str, str_to_level  # noqa E402
 from pylog.logger_type import LoggerType  # noqa E402
+from pylog.logger_type import str_to_logger_type  # noqa E402
 from pylog.opentelemetry_setup import open_telemetry_logger_setup  # noqa E402
 from pylog.rich_setup import rich_handler  # noqa E402
 from pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings  # noqa E402
-from pylog.level import level_to_str, str_to_level # noqa E402
-from pylog.logger_type import str_to_logger_type # noqa E402
+
 logger = logging.getLogger(__name__)
 
 
 def exception_handler(exc_type, exc_value, exc_traceback):
     logger.critical(f"Exception: \n {str(exc_value)} \n {''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))}")
 
 
 def set_logger(base_settings: BaseLoggerSettings = BaseLoggerSettings(), open_telemetry_settings: OpenTelemetryLoggerSettings = OpenTelemetryLoggerSettings()):
     sys.excepthook = exception_handler
     handlers = []
-    
+
     types = [str_to_logger_type(type.strip()) for type in base_settings.type.split(";")]
     for tp in types:
         match tp:
             case LoggerType.RICH:
                 handlers.append(rich_handler(str_to_level(base_settings.level)))
             case LoggerType.OPENTELEMETRY:
                 handlers.append(open_telemetry_logger_setup(str_to_level(base_settings.level), open_telemetry_settings))
             case _:
                 raise Exception(f"Unknown logger type: {tp}")
     logger = logging.getLogger(base_settings.name)
     if logger.hasHandlers():
         logger.handlers.clear()
-        
+
     logging.basicConfig(level=level_to_str(base_settings.level), format=base_settings.msg_format, datefmt=base_settings.date_format, handlers=handlers)
-    
+
     return logger
```

### Comparing `atro-pylog-0.1.0/pylog/level.py` & `atro-pylog-0.1.1/pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.1.0/pylog/opentelemetry_setup.py` & `atro-pylog-0.1.1/pylog/opentelemetry_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-import logging
-
 from opentelemetry import trace
 from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.grpc._log_exporter import OTLPLogExporter
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 
-from pylog.level import level_to_str
-from pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings
+from pylog.settings import OpenTelemetryLoggerSettings
 
 
 def open_telemetry_logger_setup(level: int, settings: OpenTelemetryLoggerSettings):
     trace.set_tracer_provider(TracerProvider())
-    logger_provider = LoggerProvider( # type: ignore
+    logger_provider = LoggerProvider(  # type: ignore
         resource=Resource.create(
             {
                 "service.name": settings.service_name,
                 "service.instance.id": settings.instance_id,
             },
         ),
     )
     set_logger_provider(logger_provider)
     exporter = OTLPLogExporter(insecure=True, endpoint=settings.endpoint)
     logger_provider.add_log_record_processor(BatchLogRecordProcessor(exporter))
     return LoggingHandler(level=level, logger_provider=logger_provider)
-
```

### Comparing `atro-pylog-0.1.0/pylog/settings.py` & `atro-pylog-0.1.1/pylog/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import logging
 
 from pydantic import BaseSettings
-
-from pylog.logger_type import LoggerType
-
+from pathlib import Path
 
 class BaseLoggerSettings(BaseSettings):
     name: str = "pylog"
     type: str = "rich"
     level: int | str = logging.DEBUG
     msg_format: str = "%(message)s"
     date_format: str = "%X"
 
     class Config:
         env_prefix = "ATRO_PYLOG_"
-        env_file = ".env"
+        env_file = (Path.home() / ".config" / "atro" / "pylog.env").as_posix(), ".env"
         env_file_encoding = "utf-8"
 
 
 class OpenTelemetryLoggerSettings(BaseSettings):
     service_name: str = "pylog"
     instance_id: str = "pylog"
     endpoint: str | None = None
 
     class Config:
         env_prefix = "ATRO_PYLOG_"
-        env_file = ".env"
+        env_file = (Path.home() / ".config" / "atro" / "pylog.env").as_posix(), ".env", 
         env_file_encoding = "utf-8"
```

### Comparing `atro-pylog-0.1.0/setup.py` & `atro-pylog-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
```

