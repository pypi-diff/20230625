# Comparing `tmp/atro-pylog-0.0.9.tar.gz` & `tmp/atro-pylog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.0.9.tar", last modified: Sat Jun 24 13:16:14 2023, max compression
+gzip compressed data, was "atro-pylog-0.1.0.tar", last modified: Sun Jun 25 09:29:57 2023, max compression
```

## Comparing `atro-pylog-0.0.9.tar` & `atro-pylog-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 13:16:14.271514 atro-pylog-0.0.9/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-24 13:16:14.271514 atro-pylog-0.0.9/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.0.9/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 13:16:14.271514 atro-pylog-0.0.9/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-24 13:16:14.000000 atro-pylog-0.0.9/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-24 13:16:14.000000 atro-pylog-0.0.9/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-24 13:16:14.000000 atro-pylog-0.0.9/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)      105 2023-06-24 13:16:14.000000 atro-pylog-0.0.9/atro_pylog.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-24 13:16:14.000000 atro-pylog-0.0.9/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-24 13:16:14.271514 atro-pylog-0.0.9/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1221 2023-06-24 13:16:01.000000 atro-pylog-0.0.9/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1050 2023-06-24 13:08:30.000000 atro-pylog-0.0.9/pylog/level.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      363 2023-06-24 13:08:30.000000 atro-pylog-0.0.9/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1351 2023-06-24 13:08:30.000000 atro-pylog-0.0.9/pylog/opentelemetry_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      376 2023-06-24 13:08:30.000000 atro-pylog-0.0.9/pylog/rich_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      676 2023-06-24 13:08:30.000000 atro-pylog-0.0.9/pylog/settings.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-24 13:16:14.271514 atro-pylog-0.0.9/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1088 2023-06-24 13:15:31.000000 atro-pylog-0.0.9/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.1.0/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      103 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-25 09:29:57.000000 atro-pylog-0.1.0/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1776 2023-06-25 09:25:57.000000 atro-pylog-0.1.0/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1050 2023-06-24 13:08:30.000000 atro-pylog-0.1.0/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      363 2023-06-24 13:08:30.000000 atro-pylog-0.1.0/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1182 2023-06-25 09:14:57.000000 atro-pylog-0.1.0/pylog/opentelemetry_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      127 2023-06-25 09:16:13.000000 atro-pylog-0.1.0/pylog/rich_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      660 2023-06-25 09:22:59.000000 atro-pylog-0.1.0/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 09:29:57.649602 atro-pylog-0.1.0/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1086 2023-06-25 09:29:53.000000 atro-pylog-0.1.0/setup.py
```

### Comparing `atro-pylog-0.0.9/PKG-INFO` & `atro-pylog-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.9/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.1.0/atro_pylog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.0.9/pylog/level.py` & `atro-pylog-0.1.0/pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.0.9/pylog/opentelemetry_setup.py` & `atro-pylog-0.1.0/pylog/opentelemetry_setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 
 from pylog.level import level_to_str
 from pylog.settings import BaseLoggerSettings, OpenTelemetryLoggerSettings
 
 
-def open_telemetry_logger_setup(base_settings: BaseLoggerSettings, settings: OpenTelemetryLoggerSettings):
+def open_telemetry_logger_setup(level: int, settings: OpenTelemetryLoggerSettings):
     trace.set_tracer_provider(TracerProvider())
-    logger_provider = LoggerProvider(
+    logger_provider = LoggerProvider( # type: ignore
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
-    handler = LoggingHandler(level=logging.NOTSET, logger_provider=logger_provider)
-    logging.basicConfig(level=level_to_str(base_settings.level), format=base_settings.msg_format, datefmt=base_settings.date_format, handlers=[handler])
+    return LoggingHandler(level=level, logger_provider=logger_provider)
+
```

### Comparing `atro-pylog-0.0.9/pylog/settings.py` & `atro-pylog-0.1.0/pylog/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic import BaseSettings
 
 from pylog.logger_type import LoggerType
 
 
 class BaseLoggerSettings(BaseSettings):
     name: str = "pylog"
-    type: LoggerType = LoggerType.RICH
+    type: str = "rich"
     level: int | str = logging.DEBUG
     msg_format: str = "%(message)s"
     date_format: str = "%X"
 
     class Config:
         env_prefix = "ATRO_PYLOG_"
         env_file = ".env"
```

### Comparing `atro-pylog-0.0.9/setup.py` & `atro-pylog-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.0.9",
+    version="0.1.0",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
-    install_requires=["loguru", "opentelemetry-api", "opentelemetry-exporter-otlp-proto-grpc", "opentelemetry-sdk", "pydantic", "python-dotenv"],
+    install_requires=["rich", "opentelemetry-api", "opentelemetry-exporter-otlp-proto-grpc", "opentelemetry-sdk", "pydantic", "python-dotenv"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

