# Comparing `tmp/weather_command-6.1.1.tar.gz` & `tmp/weather_command-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-6.1.1.tar", max compression
+gzip compressed data, was "weather_command-6.1.2.tar", max compression
```

## Comparing `weather_command-6.1.1.tar` & `weather_command-6.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-06-02 02:22:00.480474 weather_command-6.1.1/LICENSE
--rw-r--r--   0        0        0     3393 2023-06-02 02:22:00.480474 weather_command-6.1.1/README.md
--rw-r--r--   0        0        0     1793 2023-06-02 02:22:00.484476 weather_command-6.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/__main__.py
--rw-r--r--   0        0        0    18650 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_builder.py
--rw-r--r--   0        0        0     5340 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_config.py
--rw-r--r--   0        0        0     2667 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_utils.py
--rw-r--r--   0        0        0     2849 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/errors.py
--rw-r--r--   0        0        0     9084 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-06-02 02:22:00.484476 weather_command-6.1.1/weather_command/settings_commands.py
--rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 weather_command-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 14:37:08.202663 weather_command-6.1.2/LICENSE
+-rw-r--r--   0        0        0     3393 2023-06-25 14:37:08.202663 weather_command-6.1.2/README.md
+-rw-r--r--   0        0        0     1793 2023-06-25 14:37:08.202663 weather_command-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/__main__.py
+-rw-r--r--   0        0        0    18650 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_builder.py
+-rw-r--r--   0        0        0     5340 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_config.py
+-rw-r--r--   0        0        0     2667 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_utils.py
+-rw-r--r--   0        0        0     2849 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/errors.py
+-rw-r--r--   0        0        0     9084 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/main.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/py.typed
+-rw-r--r--   0        0        0     2816 2023-06-25 14:37:08.206663 weather_command-6.1.2/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 weather_command-6.1.2/PKG-INFO
```

### Comparing `weather_command-6.1.1/LICENSE` & `weather_command-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/README.md` & `weather_command-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/pyproject.toml` & `weather_command-6.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "weather-command"
-version = "6.1.1"
+version = "6.1.2"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
 keywords = ["weather", "cli"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-rich = "13.4.1"
+python = "^3.8"
+rich = "13.4.2"
 httpx = "0.24.1"
-pydantic = "1.10.8"
+pydantic = "1.10.9"
 camel-converter = {version = "3.0.0", extras = ["pydantic"]}
 typer = "0.9.0"
 tenacity = "8.2.2"
 pyyaml = "6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
-mypy = "1.3.0"
+mypy = "1.4.0"
 pre-commit = "2.21.0"
-pytest = "7.3.1"
+pytest = "7.4.0"
 pytest-cov = "4.1.0"
-ruff = "0.0.270"
+ruff = "0.0.275"
 tomli = {version = "2.0.1", python = "<3.11"}
 types-pyyaml = "6.0.12.10"
 pytest-asyncio = "0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -79,9 +79,9 @@
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:", "pragma: no cover"]
 
 [tool.ruff]
 select = ["E", "F", "UP", "I001", "T201", "T203"]
 ignore = ["E501"]
 line-length = 100
-target-version = "py37"
+target-version = "py38"
 fix = true
```

### Comparing `weather_command-6.1.1/weather_command/_builder.py` & `weather_command-6.1.2/weather_command/_builder.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/weather_command/_cache.py` & `weather_command-6.1.2/weather_command/_cache.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/weather_command/_config.py` & `weather_command-6.1.2/weather_command/_config.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/weather_command/_location.py` & `weather_command-6.1.2/weather_command/_location.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/weather_command/_weather.py` & `weather_command-6.1.2/weather_command/_weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/weather_command/main.py` & `weather_command-6.1.2/weather_command/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
 from weather_command._location import build_location_url, get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "6.1.1"
+__version__ = "6.1.2"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
```

### Comparing `weather_command-6.1.1/weather_command/models/weather.py` & `weather_command-6.1.2/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/weather_command/settings_commands.py` & `weather_command-6.1.2/weather_command/settings_commands.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.1.1/PKG-INFO` & `weather_command-6.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 6.1.1
+Version: 6.1.2
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: camel-converter[pydantic] (==3.0.0)
 Requires-Dist: httpx (==0.24.1)
-Requires-Dist: pydantic (==1.10.8)
+Requires-Dist: pydantic (==1.10.9)
 Requires-Dist: pyyaml (==6.0)
-Requires-Dist: rich (==13.4.1)
+Requires-Dist: rich (==13.4.2)
 Requires-Dist: tenacity (==8.2.2)
 Requires-Dist: typer (==0.9.0)
 Project-URL: Documentation, https://github.com/sanders41/weather-command
 Project-URL: Repository, https://github.com/sanders41/weather-command
 Description-Content-Type: text/markdown
 
 # Weather Command
```

