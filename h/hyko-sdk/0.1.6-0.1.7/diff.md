# Comparing `tmp/hyko_sdk-0.1.6.tar.gz` & `tmp/hyko_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.1.6.tar", last modified: Wed Jun 21 11:40:16 2023, max compression
+gzip compressed data, was "hyko_sdk-0.1.7.tar", last modified: Sun Jun 25 10:43:50 2023, max compression
```

## Comparing `hyko_sdk-0.1.6.tar` & `hyko_sdk-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/PKG-INFO
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      411 2023-05-17 08:56:51.000000 hyko_sdk-0.1.6/README.md
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/hyko_sdk/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       40 2023-06-21 11:17:29.000000 hyko_sdk-0.1.6/hyko_sdk/__init__.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)     2995 2023-06-21 11:24:07.000000 hyko_sdk-0.1.6/hyko_sdk/io.py
--rw-rw-r--   0 crptx     (1000) crptx     (1000)     2772 2023-06-21 11:24:49.000000 hyko_sdk-0.1.6/hyko_sdk/metadata.py
-drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/hyko_sdk.egg-info/
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      250 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        1 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/requires.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-21 11:40:16.000000 hyko_sdk-0.1.6/hyko_sdk.egg-info/top_level.txt
--rw-rw-r--   0 crptx     (1000) crptx     (1000)       80 2023-06-21 11:17:29.000000 hyko_sdk-0.1.6/pyproject.toml
--rw-rw-r--   0 crptx     (1000) crptx     (1000)      327 2023-06-21 11:40:16.723916 hyko_sdk-0.1.6/setup.cfg
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/PKG-INFO
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      411 2023-05-17 08:56:51.000000 hyko_sdk-0.1.7/README.md
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/hyko_sdk/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       40 2023-06-21 11:17:29.000000 hyko_sdk-0.1.7/hyko_sdk/__init__.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)     2915 2023-06-25 10:41:00.000000 hyko_sdk-0.1.7/hyko_sdk/io.py
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)     2798 2023-06-25 10:39:49.000000 hyko_sdk-0.1.7/hyko_sdk/metadata.py
+drwxrwxr-x   0 crptx     (1000) crptx     (1000)        0 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/hyko_sdk.egg-info/
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      192 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      250 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        1 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/requires.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)        9 2023-06-25 10:43:50.000000 hyko_sdk-0.1.7/hyko_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)       80 2023-06-21 11:17:29.000000 hyko_sdk-0.1.7/pyproject.toml
+-rw-rw-r--   0 crptx     (1000) crptx     (1000)      327 2023-06-25 10:43:50.756125 hyko_sdk-0.1.7/setup.cfg
```

### Comparing `hyko_sdk-0.1.6/hyko_sdk/io.py` & `hyko_sdk-0.1.7/hyko_sdk/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from enum import Enum
-from typing import Optional
-from pydantic import BaseModel
-
-from typing import Any, Callable, Dict, Generator, Optional
+from typing import Any, Union, Optional, Callable, Dict, Generator
 
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 
-from pydantic import BaseModel
-
 
 class Number(float):
 
     @classmethod
     def __get_validators__(cls) -> Generator[Callable, None, None]:
         yield cls.validate
 
@@ -124,8 +119,8 @@
     ARRAY_AUDIO = "array[audio]"
 
 class IOPort(BaseModel):
     name: str
     description: Optional[str]
     type: IOPortType
     required: bool
-    default: Optional[float | int | str]
+    default: Optional[Union[float, int, str]]
```

### Comparing `hyko_sdk-0.1.6/hyko_sdk/metadata.py` & `hyko_sdk-0.1.7/hyko_sdk/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pydantic import BaseModel
-from typing import Any
+from typing import Any, List, Union, Optional
 from .io import IOPortType, IOPort
 
 
-def pmodel_to_ports(pmodel: BaseModel) -> list[IOPort]:
+def pmodel_to_ports(pmodel: BaseModel) -> List[IOPort]:
     
     schema = pmodel.schema()
 
     fields_properties: dict[str, dict[str, Any]] = schema["properties"]
-    required_fields: list[str] | None = schema.get("required")
+    required_fields: Optional[List[str]] = schema.get("required")
 
     ports = []
     
     for field_name, field_props in fields_properties.items():
         field_type = field_props.get("type")
 
         if field_type is None:
@@ -83,10 +83,10 @@
 
 
 class MetaData(BaseModel):
     name: str
     description: str
     version: str
     category: str
-    inputs: list[IOPort]
-    outputs: list[IOPort]
-    params: list[IOPort]
+    inputs: List[IOPort]
+    outputs: List[IOPort]
+    params: List[IOPort]
```

