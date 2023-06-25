# Comparing `tmp/delfino-1.3.0.tar.gz` & `tmp/delfino-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino-1.3.0.tar", max compression
+gzip compressed data, was "delfino-2.0.0.tar", max compression
```

## Comparing `delfino-1.3.0.tar` & `delfino-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1067 2023-05-13 10:12:13.093087 delfino-1.3.0/LICENSE
--rw-r--r--   0        0        0    18511 2023-05-13 10:12:13.093087 delfino-1.3.0/README.md
--rw-r--r--   0        0        0     3681 2023-05-13 10:12:13.093087 delfino-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/__init__.py
--rw-r--r--   0        0        0      273 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/backports.py
--rw-r--r--   0        0        0       76 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/click_utils/__init__.py
--rw-r--r--   0        0        0    10468 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/click_utils/command.py
--rwxr-xr-x   0        0        0     2238 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/click_utils/command_groups.py
--rw-r--r--   0        0        0     3378 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/click_utils/set_from_config.py
--rw-r--r--   0        0        0     1343 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/config.py
--rw-r--r--   0        0        0      270 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/constants.py
--rw-r--r--   0        0        0      182 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/decorators/__init__.py
--rw-r--r--   0        0        0      545 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/decorators/files_folders.py
--rw-r--r--   0        0        0     1754 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/decorators/pass_app_context.py
--rw-r--r--   0        0        0     1545 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/decorators/pass_args.py
--rw-r--r--   0        0        0     4220 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/execution.py
--rw-r--r--   0        0        0        0 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/internal_parameters/__init__.py
--rw-r--r--   0        0        0     5402 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/internal_parameters/completion.py
--rw-r--r--   0        0        0      506 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/internal_parameters/help.py
--rw-r--r--   0        0        0      892 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/internal_parameters/verbosity.py
--rw-r--r--   0        0        0     4278 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/main.py
--rw-r--r--   0        0        0      143 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/models/__init__.py
--rw-r--r--   0        0        0      522 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/models/app_context.py
--rw-r--r--   0        0        0     1686 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/models/pyproject_toml.py
--rw-r--r--   0        0        0     1090 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/terminal_output.py
--rw-r--r--   0        0        0      618 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/utils.py
--rw-r--r--   0        0        0     1350 2023-05-13 10:12:13.093087 delfino-1.3.0/src/delfino/validation.py
--rw-r--r--   0        0        0    20131 1970-01-01 00:00:00.000000 delfino-1.3.0/setup.py
--rw-r--r--   0        0        0    19981 1970-01-01 00:00:00.000000 delfino-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-25 13:39:39.738619 delfino-2.0.0/LICENSE
+-rw-r--r--   0        0        0    18511 2023-06-25 13:39:39.738619 delfino-2.0.0/README.md
+-rw-r--r--   0        0        0     3596 2023-06-25 13:39:39.742619 delfino-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/__init__.py
+-rw-r--r--   0        0        0      273 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/backports.py
+-rw-r--r--   0        0        0       76 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/click_utils/__init__.py
+-rw-r--r--   0        0        0    10468 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/click_utils/command.py
+-rwxr-xr-x   0        0        0     2215 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/click_utils/command_groups.py
+-rw-r--r--   0        0        0     3342 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/click_utils/set_from_config.py
+-rw-r--r--   0        0        0     1343 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/config.py
+-rw-r--r--   0        0        0      346 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/constants.py
+-rw-r--r--   0        0        0      182 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/decorators/__init__.py
+-rw-r--r--   0        0        0      578 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/decorators/files_folders.py
+-rw-r--r--   0        0        0     1754 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/decorators/pass_app_context.py
+-rw-r--r--   0        0        0     1564 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/decorators/pass_args.py
+-rw-r--r--   0        0        0     4263 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/execution.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/internal_parameters/__init__.py
+-rw-r--r--   0        0        0     5445 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/internal_parameters/completion.py
+-rw-r--r--   0        0        0      506 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/internal_parameters/help.py
+-rw-r--r--   0        0        0      892 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/internal_parameters/verbosity.py
+-rw-r--r--   0        0        0     4269 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/main.py
+-rw-r--r--   0        0        0      143 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/models/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/models/app_context.py
+-rw-r--r--   0        0        0     1380 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/models/pyproject_toml.py
+-rw-r--r--   0        0        0     1090 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/terminal_output.py
+-rw-r--r--   0        0        0      618 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/utils.py
+-rw-r--r--   0        0        0     1350 2023-06-25 13:39:39.742619 delfino-2.0.0/src/delfino/validation.py
+-rw-r--r--   0        0        0    19677 1970-01-01 00:00:00.000000 delfino-2.0.0/PKG-INFO
```

### Comparing `delfino-1.3.0/LICENSE` & `delfino-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/README.md` & `delfino-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/pyproject.toml` & `delfino-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 [tool.poetry]
 name = "delfino"
-version = "1.3.0"
+version = "2.0.0"
 description = "A collection of command line helper scripts wrapping tools used during Python development."
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.scripts]
 delfino = "delfino.main:main"
 mike = "delfino.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8"
 toml = "^0.10"
 click = "^8.0"
 pydantic = "^1.8"
 deprecation ="^2.1"
 importlib-metadata = {version = "*", python = "<3.10"}
 
 [tool.poetry.extras]
 completion = ["shellingham"]
 
 [tool.poetry.group.dev.dependencies]
 shellingham = "^1.4"
 types-toml = "*"
-delfino-core = {extras = ["verify-all", "dependencies-update"], version = "^3.9.0"}
+delfino-core = {extras = ["verify-all", "dependencies-update"], version = "^5.1"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 # Setting compatible with black. See https://black.readthedocs.io/en/stable/compatible_configs.html
@@ -119,15 +118,14 @@
     "D202",  # "No blank lines allowed after function docstring" is false positive caused by black formatter.
     "D204",  # "1 blank line required after class docstring"
     "D401",  # "First line should be in imperative mood"
     "D413",  # "Missing blank line after last section"
 ]
 
 [tool.delfino.plugins.delfino-core]
-disable_commands = ['build-docker']
 
 
 #[tool.delfino.dockerhub]
 #username = "radeklat"
 #build_for_platforms = [
 #    "linux/amd64",
 #    "linux/arm64",
```

### Comparing `delfino-1.3.0/src/delfino/click_utils/command.py` & `delfino-2.0.0/src/delfino/click_utils/command.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/click_utils/command_groups.py` & `delfino-2.0.0/src/delfino/click_utils/command_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 
 
 def get_command_groups(app_context: AppContext) -> Dict[str, List[str]]:
     return {**app_context.plugin_config.command_groups, **app_context.pyproject_toml.tool.delfino.command_groups}
 
 
 def _get_target_command_names(group_name: str, app_context: AppContext) -> List[str]:
-    target_command_names = get_command_groups(app_context).get(group_name, None)
-
-    if target_command_names is None:
+    if (target_command_names := get_command_groups(app_context).get(group_name, None)) is None:
         raise click.exceptions.Abort(f"Command group '{group_name}' does not exist.")
 
     if not target_command_names:
         _LOG.warning(f"Command group '{group_name}' contains no commands.")
         raise click.exceptions.Exit()
 
     return target_command_names
```

### Comparing `delfino-1.3.0/src/delfino/click_utils/set_from_config.py` & `delfino-2.0.0/src/delfino/click_utils/set_from_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,15 @@
         """Returns key-value pair to set in invoking another command.
 
         Similarly to ``__call__``, it takes the value from config if it exists. It also checks
         if the command has a ``click.Parameter`` of the matching name.
 
         This is useful for invoking commands indirectly, for example in a group command.
         """
-        app_context = ctx.find_object(AppContext)
-
-        if app_context is None:
+        if (app_context := ctx.find_object(AppContext)) is None:
             raise RuntimeError("AppContext was expected to be set but none found.")
 
         command_config = getattr(app_context.plugin_config, command.name or "", {})
 
         if isinstance(command_config, dict):
             value_from_config = command_config.get(self.config_option_name, None)
         else:
@@ -59,17 +57,15 @@
     def __call__(self, ctx: click.Context, param: click.Parameter, value: Any) -> Any:
         """Load passed arguments from config if none given on command line."""
         # Command line options have higher priority. Return them instead of options from the config file.
         if value:
             return value
 
         # No command line options provided, try to load them from config
-        app_context = ctx.find_object(AppContext)
-
-        if app_context is None:
+        if (app_context := ctx.find_object(AppContext)) is None:
             raise RuntimeError("AppContext was expected to be set but none found.")
 
         command_name: str = ctx.command.name or ""
         value_from_config: str = getattr(app_context.plugin_config, command_name, {}).get(self.config_option_name, None)
         if value_from_config:
             return self._type_cast_value(ctx, param, value_from_config)
```

### Comparing `delfino-1.3.0/src/delfino/config.py` & `delfino-2.0.0/src/delfino/config.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/decorators/files_folders.py` & `delfino-2.0.0/src/delfino/decorators/files_folders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Final
+
 import click
 
 from delfino.click_utils.set_from_config import SetOptionFromConfigCallback
 
-_ARGUMENT_NAME: str = "files_folders"
+_ARGUMENT_NAME: Final[str] = "files_folders"
 FILES_FOLDERS_OPTION_CALLBACK = SetOptionFromConfigCallback(_ARGUMENT_NAME)
 
 files_folders_option = click.option(
     "-f",
     "--file",
     "--folder",
     _ARGUMENT_NAME,
```

### Comparing `delfino-1.3.0/src/delfino/decorators/pass_app_context.py` & `delfino-2.0.0/src/delfino/decorators/pass_app_context.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/decorators/pass_args.py` & `delfino-2.0.0/src/delfino/decorators/pass_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import shlex
-from typing import Any
+from typing import Any, Final
 
 import click
 
 from delfino.click_utils.set_from_config import SetOptionFromConfigCallback
 
 
 class _SetPassArgsFromConfigCallback(SetOptionFromConfigCallback):
     def _type_cast_value(self, ctx: click.Context, param: click.Parameter, value_from_config: Any) -> Any:
         if isinstance(value_from_config, str):
             value_from_config = tuple(shlex.split(value_from_config))
 
         return super()._type_cast_value(ctx, param, value_from_config)
 
 
-_ARGUMENT_NAME = "passed_args"
+_ARGUMENT_NAME: Final[str] = "passed_args"
 PASS_ARGS_CALLBACK = _SetPassArgsFromConfigCallback(_ARGUMENT_NAME, "pass_args")
 
 
 pass_args = click.argument(
     _ARGUMENT_NAME,
     metavar=f"[-- {_ARGUMENT_NAME.upper()}]",
     nargs=-1,
```

### Comparing `delfino-1.3.0/src/delfino/execution.py` & `delfino-2.0.0/src/delfino/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 import shlex
 import subprocess
 from enum import Enum
 from logging import getLogger
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, Final, Optional, Tuple
 
 import click
 
 from delfino.backports import shlex_join
 from delfino.utils import ArgsType
 
 _LOG = getLogger(__name__)
 
 
 class OnError(Enum):
-    PASS = "pass"
+    PASS: Final[str] = "pass"
     """Same as ``check=False``. Use when you're handling the return code yourself."""
 
-    EXIT = "exit"
+    EXIT: Final[str] = "exit"
     """Same as ``check=True`` + red print of stdout/stderr + ``raise click.exception.Exit()``.
     Use when running commands where non-zero return code indicates an error, not a failed check."""
 
-    ABORT = "abort"
+    ABORT: Final[str] = "abort"
     """Same as ``check=True`` + print of stdout/stderr + ``raise click.Abort()``.
     Use when running commands where non-zero return code indicates a failed check, not an error."""
 
 
 def _normalize_args(args: ArgsType, shell: bool) -> Tuple[ArgsType, str]:
     if shell:  # when `shell`, `args` must be a string
         if isinstance(args, str):
```

### Comparing `delfino-1.3.0/src/delfino/internal_parameters/completion.py` & `delfino-2.0.0/src/delfino/internal_parameters/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Callable, Dict, List, Union
+from typing import Callable, Dict, Final, List, Union
 
 import click
 
 from delfino.constants import ENTRY_POINT
 from delfino.validation import assert_pip_package_installed
 
 try:
@@ -25,23 +25,27 @@
     install: Callable[[str], Path]
 
     @property
     def formatted_completion(self) -> str:
         return self.completion.format(entry_point=ENTRY_POINT, entry_point_upper=ENTRY_POINT.upper()).strip()
 
 
-_COMPLETION_BASH = """
+_COMPLETION_BASH: Final[
+    str
+] = """
 _complete_{entry_point}() {{
     [ -n "$(which {entry_point})" ] && \\
         eval "$(_{entry_point_upper}_COMPLETE=bash_source {entry_point})";
 }}
 complete -F _complete_{entry_point} -o default invoke {entry_point}
 """
 
-_COMPLETION_ZSH = """
+_COMPLETION_ZSH: Final[
+    str
+] = """
 _complete_{entry_point}() {{
     which {entry_point} >/dev/null && \\
         eval $(_{entry_point_upper}_COMPLETE=zsh_source {entry_point})
 }}
 compctl -K _complete_{entry_point} + -f invoke {entry_point}
 """
```

### Comparing `delfino-1.3.0/src/delfino/internal_parameters/verbosity.py` & `delfino-2.0.0/src/delfino/internal_parameters/verbosity.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/main.py` & `delfino-2.0.0/src/delfino/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     def list_commands(self, ctx: click.Context) -> List[str]:
         """Override as MultiCommand always returns []."""
         del ctx
         return sorted(command.name for command in self._command_registry.visible_commands)
 
     def get_command(self, ctx: click.Context, cmd_name: str) -> Optional[click.Command]:
         """Override to give all commands a common ``AppContext`` or fail if ``pyproject.toml`` is broken/missing."""
-        cmd = self._command_registry.get(cmd_name, None)
-        if cmd is None:
+        if (cmd := self._command_registry.get(cmd_name, None)) is None:
             return None  # command doesn't exist
 
         if ctx.resilient_parsing:  # do not fail on auto-completion
             return cmd.command
 
         if self._pyproject_toml_validation_error:
             click.secho(str(self._pyproject_toml_validation_error), fg="red", err=True)
```

### Comparing `delfino-1.3.0/src/delfino/models/app_context.py` & `delfino-2.0.0/src/delfino/models/app_context.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/models/pyproject_toml.py` & `delfino-2.0.0/src/delfino/models/pyproject_toml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Tuple
-from warnings import warn
 
 from pydantic import BaseModel, Extra, Field
 
 from delfino.constants import DEFAULT_LOCAL_COMMAND_FOLDERS
 
 
 class PluginConfig(BaseModel):
@@ -21,22 +20,14 @@
 
 
 class Delfino(BaseModel):
     local_command_folders: Tuple[Path, ...] = DEFAULT_LOCAL_COMMAND_FOLDERS
     plugins: Dict[str, PluginConfig] = Field(default_factory=dict)
     command_groups: Dict[str, List[str]] = Field(default_factory=dict)
 
-    @property
-    def local_commands_directory(self) -> Path:
-        warn(
-            "tool.delfino.local_commands_directory is deprecated. Use tool.delfino.local_command_folders instead.",
-            DeprecationWarning,
-        )
-        return self.local_command_folders[0]
-
     class Config:
         extra = Extra.allow
 
 
 class Poetry(BaseModel):
     name: str
     version: str
```

### Comparing `delfino-1.3.0/src/delfino/terminal_output.py` & `delfino-2.0.0/src/delfino/terminal_output.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/utils.py` & `delfino-2.0.0/src/delfino/utils.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/src/delfino/validation.py` & `delfino-2.0.0/src/delfino/validation.py`

 * *Files identical despite different names*

### Comparing `delfino-1.3.0/setup.py` & `delfino-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,1259 +1,1230 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 6465 6c66 696e 6f27 2c0a 2027 6465  ['delfino',. 'de
-00000070: 6c66 696e 6f2e 636c 6963 6b5f 7574 696c  lfino.click_util
-00000080: 7327 2c0a 2027 6465 6c66 696e 6f2e 6465  s',. 'delfino.de
-00000090: 636f 7261 746f 7273 272c 0a20 2764 656c  corators',. 'del
-000000a0: 6669 6e6f 2e69 6e74 6572 6e61 6c5f 7061  fino.internal_pa
-000000b0: 7261 6d65 7465 7273 272c 0a20 2764 656c  rameters',. 'del
-000000c0: 6669 6e6f 2e6d 6f64 656c 7327 5d0a 0a70  fino.models']..p
-000000d0: 6163 6b61 6765 5f64 6174 6120 3d20 5c0a  ackage_data = \.
-000000e0: 7b27 273a 205b 272a 275d 7d0a 0a69 6e73  {'': ['*']}..ins
-000000f0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000100: 5c0a 5b27 636c 6963 6b3e 3d38 2e30 2c3c  \.['click>=8.0,<
-00000110: 392e 3027 2c0a 2027 6465 7072 6563 6174  9.0',. 'deprecat
-00000120: 696f 6e3e 3d32 2e31 2c3c 332e 3027 2c0a  ion>=2.1,<3.0',.
-00000130: 2027 7079 6461 6e74 6963 3e3d 312e 382c   'pydantic>=1.8,
-00000140: 3c32 2e30 272c 0a20 2774 6f6d 6c3e 3d30  <2.0',. 'toml>=0
-00000150: 2e31 302c 3c30 2e31 3127 5d0a 0a65 7874  .10,<0.11']..ext
-00000160: 7261 735f 7265 7175 6972 6520 3d20 5c0a  ras_require = \.
-00000170: 7b27 3a70 7974 686f 6e5f 7665 7273 696f  {':python_versio
-00000180: 6e20 3c20 2233 2e31 3022 273a 205b 2769  n < "3.10"': ['i
-00000190: 6d70 6f72 746c 6962 2d6d 6574 6164 6174  mportlib-metadat
-000001a0: 6127 5d7d 0a0a 656e 7472 795f 706f 696e  a']}..entry_poin
-000001b0: 7473 203d 205c 0a7b 2763 6f6e 736f 6c65  ts = \.{'console
-000001c0: 5f73 6372 6970 7473 273a 205b 2764 656c  _scripts': ['del
-000001d0: 6669 6e6f 203d 2064 656c 6669 6e6f 2e6d  fino = delfino.m
-000001e0: 6169 6e3a 6d61 696e 272c 2027 6d69 6b65  ain:main', 'mike
-000001f0: 203d 2064 656c 6669 6e6f 2e6d 6169 6e3a   = delfino.main:
-00000200: 6d61 696e 275d 7d0a 0a73 6574 7570 5f6b  main']}..setup_k
-00000210: 7761 7267 7320 3d20 7b0a 2020 2020 276e  wargs = {.    'n
-00000220: 616d 6527 3a20 2764 656c 6669 6e6f 272c  ame': 'delfino',
-00000230: 0a20 2020 2027 7665 7273 696f 6e27 3a20  .    'version': 
-00000240: 2731 2e33 2e30 272c 0a20 2020 2027 6465  '1.3.0',.    'de
-00000250: 7363 7269 7074 696f 6e27 3a20 2741 2063  scription': 'A c
-00000260: 6f6c 6c65 6374 696f 6e20 6f66 2063 6f6d  ollection of com
-00000270: 6d61 6e64 206c 696e 6520 6865 6c70 6572  mand line helper
-00000280: 2073 6372 6970 7473 2077 7261 7070 696e   scripts wrappin
-00000290: 6720 746f 6f6c 7320 7573 6564 2064 7572  g tools used dur
-000002a0: 696e 6720 5079 7468 6f6e 2064 6576 656c  ing Python devel
-000002b0: 6f70 6d65 6e74 2e27 2c0a 2020 2020 276c  opment.',.    'l
-000002c0: 6f6e 675f 6465 7363 7269 7074 696f 6e27  ong_description'
-000002d0: 3a20 273c 6831 2061 6c69 676e 3d22 6365  : '<h1 align="ce
-000002e0: 6e74 6572 2220 7374 796c 653d 2262 6f72  nter" style="bor
-000002f0: 6465 722d 626f 7474 6f6d 3a20 6e6f 6e65  der-bottom: none
-00000300: 3b22 3ef0 9fa7 b026 6e62 7370 3b26 6e62  ;">....&nbsp;&nb
-00000310: 7370 3b44 656c 6669 6e6f 266e 6273 703b  sp;Delfino&nbsp;
-00000320: 266e 6273 703b f09f a7b0 3c2f 6831 3e5c  &nbsp;....</h1>\
-00000330: 6e3c 6833 2061 6c69 676e 3d22 6365 6e74  n<h3 align="cent
-00000340: 6572 223e 5468 6520 556c 7469 6d61 7465  er">The Ultimate
-00000350: 2043 6f6d 6d61 6e64 204c 696e 6520 436f   Command Line Co
-00000360: 6d70 616e 696f 6e20 666f 7220 596f 7572  mpanion for Your
-00000370: 2050 726f 6a65 6374 733c 2f68 333e 5c6e   Projects</h3>\n
-00000380: 5c6e 3c70 2061 6c69 676e 3d22 6365 6e74  \n<p align="cent
-00000390: 6572 223e 5c6e 2020 2020 3c61 2068 7265  er">\n    <a hre
-000003a0: 663d 2268 7474 7073 3a2f 2f61 7070 2e63  f="https://app.c
-000003b0: 6972 636c 6563 692e 636f 6d2f 7069 7065  ircleci.com/pipe
-000003c0: 6c69 6e65 732f 6769 7468 7562 2f72 6164  lines/github/rad
-000003d0: 656b 6c61 742f 6465 6c66 696e 6f3f 6272  eklat/delfino?br
-000003e0: 616e 6368 3d6d 6169 6e22 3e5c 6e20 2020  anch=main">\n   
-000003f0: 2020 2020 203c 696d 6720 616c 743d 2243       <img alt="C
-00000400: 6972 636c 6543 4922 2073 7263 3d22 6874  ircleCI" src="ht
-00000410: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000420: 732e 696f 2f63 6972 636c 6563 692f 6275  s.io/circleci/bu
-00000430: 696c 642f 6769 7468 7562 2f72 6164 656b  ild/github/radek
-00000440: 6c61 742f 6465 6c66 696e 6f22 3e5c 6e20  lat/delfino">\n 
-00000450: 2020 203c 2f61 3e5c 6e20 2020 203c 6120     </a>\n    <a 
-00000460: 6872 6566 3d22 6874 7470 733a 2f2f 6170  href="https://ap
-00000470: 702e 636f 6465 636f 762e 696f 2f67 682f  p.codecov.io/gh/
-00000480: 7261 6465 6b6c 6174 2f64 656c 6669 6e6f  radeklat/delfino
-00000490: 2f22 3e5c 6e20 2020 2020 2020 203c 696d  /">\n        <im
-000004a0: 6720 616c 743d 2243 6f64 6563 6f76 2220  g alt="Codecov" 
-000004b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000004c0: 2e73 6869 656c 6473 2e69 6f2f 636f 6465  .shields.io/code
-000004d0: 636f 762f 632f 6769 7468 7562 2f72 6164  cov/c/github/rad
-000004e0: 656b 6c61 742f 6465 6c66 696e 6f22 3e5c  eklat/delfino">\
-000004f0: 6e20 2020 203c 2f61 3e5c 6e20 2020 203c  n    </a>\n    <
-00000500: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000510: 6769 7468 7562 2e63 6f6d 2f72 6164 656b  github.com/radek
-00000520: 6c61 742f 6465 6c66 696e 6f2f 7461 6773  lat/delfino/tags
-00000530: 223e 5c6e 2020 2020 2020 2020 3c69 6d67  ">\n        <img
-00000540: 2061 6c74 3d22 4769 7448 7562 2074 6167   alt="GitHub tag
-00000550: 2028 6c61 7465 7374 2053 656d 5665 7229   (latest SemVer)
-00000560: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00000570: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00000580: 7468 7562 2f74 6167 2f72 6164 656b 6c61  thub/tag/radekla
-00000590: 742f 6465 6c66 696e 6f22 3e5c 6e20 2020  t/delfino">\n   
-000005a0: 203c 2f61 3e5c 6e20 2020 203c 696d 6720   </a>\n    <img 
-000005b0: 616c 743d 224d 6169 6e74 656e 616e 6365  alt="Maintenance
-000005c0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-000005d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6d61  mg.shields.io/ma
-000005e0: 696e 7465 6e61 6e63 652f 7965 732f 3230  intenance/yes/20
-000005f0: 3233 223e 5c6e 2020 2020 3c61 2068 7265  23">\n    <a hre
-00000600: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000610: 622e 636f 6d2f 7261 6465 6b6c 6174 2f64  b.com/radeklat/d
-00000620: 656c 6669 6e6f 2f63 6f6d 6d69 7473 2f6d  elfino/commits/m
-00000630: 6169 6e22 3e5c 6e20 2020 2020 2020 203c  ain">\n        <
-00000640: 696d 6720 616c 743d 2247 6974 4875 6220  img alt="GitHub 
-00000650: 6c61 7374 2063 6f6d 6d69 7422 2073 7263  last commit" src
-00000660: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000670: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000680: 6c61 7374 2d63 6f6d 6d69 742f 7261 6465  last-commit/rade
-00000690: 6b6c 6174 2f64 656c 6669 6e6f 223e 5c6e  klat/delfino">\n
-000006a0: 2020 2020 3c2f 613e 5c6e 2020 2020 3c61      </a>\n    <a
-000006b0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
-000006c0: 7777 2e70 7974 686f 6e2e 6f72 672f 646f  ww.python.org/do
-000006d0: 632f 7665 7273 696f 6e73 2f22 3e5c 6e20  c/versions/">\n 
-000006e0: 2020 2020 2020 203c 696d 6720 616c 743d         <img alt=
-000006f0: 2250 7950 4920 2d20 5079 7468 6f6e 2056  "PyPI - Python V
-00000700: 6572 7369 6f6e 2220 7372 633d 2268 7474  ersion" src="htt
-00000710: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000720: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000730: 6f6e 732f 6465 6c66 696e 6f22 3e5c 6e20  ons/delfino">\n 
-00000740: 2020 203c 2f61 3e5c 6e20 2020 203c 6120     </a>\n    <a 
-00000750: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000760: 7069 7374 6174 732e 6f72 672f 7061 636b  pistats.org/pack
-00000770: 6167 6573 2f64 656c 6669 6e6f 223e 5c6e  ages/delfino">\n
-00000780: 2020 2020 2020 2020 3c69 6d67 2061 6c74          <img alt
-00000790: 3d22 446f 776e 6c6f 6164 7322 2073 7263  ="Downloads" src
-000007a0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000007b0: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-000007c0: 2f64 656c 6669 6e6f 223e 5c6e 2020 2020  /delfino">\n    
-000007d0: 3c2f 613e 5c6e 3c2f 703e 5c6e 5c6e 5469  </a>\n</p>\n\nTi
-000007e0: 7265 6420 6f66 206d 616e 6167 696e 6720  red of managing 
-000007f0: 7363 6174 7465 7265 6420 7363 7269 7074  scattered script
-00000800: 733f 2053 6179 2067 6f6f 6462 7965 2074  s? Say goodbye t
-00000810: 6f20 636f 6d70 6c65 7869 7479 2077 6974  o complexity wit
-00000820: 6820 4465 6c66 696e 6f21 5c6e 5c6e 4465  h Delfino!\n\nDe
-00000830: 6c66 696e 6f20 6973 2061 2070 6f77 6572  lfino is a power
-00000840: 6675 6c20 7772 6170 7065 7220 6172 6f75  ful wrapper arou
-00000850: 6e64 2043 6c69 636b 2c20 7468 6520 706f  nd Click, the po
-00000860: 7075 6c61 7220 636f 6d6d 616e 6420 6c69  pular command li
-00000870: 6e65 2069 6e74 6572 6661 6365 2070 6163  ne interface pac
-00000880: 6b61 6765 2e20 4974 2061 7574 6f6d 6174  kage. It automat
-00000890: 6963 616c 6c79 2064 6973 636f 7665 7273  ically discovers
-000008a0: 2061 6e64 2065 7865 6375 7465 7320 436c   and executes Cl
-000008b0: 6963 6b20 636f 6d6d 616e 6473 2069 6e20  ick commands in 
-000008c0: 796f 7572 2070 726f 6a65 6374 2e20 4275  your project. Bu
-000008d0: 7420 4465 6c66 696e 6f20 646f 6573 6e5c  t Delfino doesn\
-000008e0: 2774 2073 746f 7020 7468 6572 6520 2d20  't stop there - 
-000008f0: 6974 2074 616b 6573 2069 7420 6120 7374  it takes it a st
-00000900: 6570 2066 7572 7468 6572 2062 7920 616c  ep further by al
-00000910: 6c6f 7769 6e67 2079 6f75 2074 6f20 6372  lowing you to cr
-00000920: 6561 7465 2070 6c75 6769 6e73 2c20 6d61  eate plugins, ma
-00000930: 6b69 6e67 2073 6372 6970 7420 6469 7374  king script dist
-00000940: 7269 6275 7469 6f6e 2061 6e64 2069 6e73  ribution and ins
-00000950: 7461 6c6c 6174 696f 6e20 6120 6272 6565  tallation a bree
-00000960: 7a65 2e5c 6e5c 6e23 2057 6879 2063 686f  ze.\n\n# Why cho
-00000970: 6f73 6520 4465 6c66 696e 6f3f 5c6e 5c6e  ose Delfino?\n\n
-00000980: 2d20 2a2a 5374 7265 616d 6c69 6e65 2053  - **Streamline S
-00000990: 6372 6970 7473 2a2a 3a20 436f 6e73 6f6c  cripts**: Consol
-000009a0: 6964 6174 6520 616c 6c20 796f 7572 2068  idate all your h
-000009b0: 656c 7065 7220 7363 7269 7074 7320 696e  elper scripts in
-000009c0: 746f 2061 2073 696e 676c 652c 2065 6173  to a single, eas
-000009d0: 792d 746f 2d75 7365 2065 6e74 7279 2070  y-to-use entry p
-000009e0: 6f69 6e74 2e20 4e6f 206d 6f72 6520 6875  oint. No more hu
-000009f0: 6e74 696e 6720 666f 7220 7363 7269 7074  nting for script
-00000a00: 7320 6f72 2064 6561 6c69 6e67 2077 6974  s or dealing wit
-00000a10: 6820 636f 6e76 6f6c 7574 6564 2061 6c69  h convoluted ali
-00000a20: 6173 6573 2e20 5369 6d70 6c79 2075 7365  ases. Simply use
-00000a30: 2064 656c 6669 6e6f 2066 6f6c 6c6f 7765   delfino followe
-00000a40: 6420 6279 2074 6865 2073 6372 6970 7420  d by the script 
-00000a50: 6e61 6d65 2061 6e64 206f 7074 696f 6e73  name and options
-00000a60: 2e5c 6e2d 202a 2a52 6575 7361 626c 6520  .\n- **Reusable 
-00000a70: 506c 7567 696e 732a 2a3a 2050 6163 6b61  Plugins**: Packa
-00000a80: 6765 2079 6f75 7220 6865 6c70 6572 2073  ge your helper s
-00000a90: 6372 6970 7473 2061 7320 706c 7567 696e  cripts as plugin
-00000aa0: 7320 616e 6420 696e 7374 616c 6c20 7468  s and install th
-00000ab0: 656d 2077 6974 6820 7069 702e 204d 6169  em with pip. Mai
-00000ac0: 6e74 6169 6e20 636f 6e73 6973 7465 6e63  ntain consistenc
-00000ad0: 7920 6163 726f 7373 2070 726f 6a65 6374  y across project
-00000ae0: 7320 616e 6420 6561 7369 6c79 2069 6e63  s and easily inc
-00000af0: 6f72 706f 7261 7465 2075 7064 6174 6573  orporate updates
-00000b00: 2074 6872 6f75 6768 2061 2066 6c65 7869   through a flexi
-00000b10: 626c 6520 636f 6e66 6967 7572 6174 696f  ble configuratio
-00000b20: 6e20 7379 7374 656d 2e5c 6e2d 202a 2a53  n system.\n- **S
-00000b30: 696d 706c 6966 7920 546f 6f6c 696e 672a  implify Tooling*
-00000b40: 2a3a 2044 656c 6669 6e6f 2065 7874 656e  *: Delfino exten
-00000b50: 6473 2043 6c69 636b 2077 6974 6820 6164  ds Click with ad
-00000b60: 7661 6e63 6564 2066 6561 7475 7265 7320  vanced features 
-00000b70: 6c69 6b65 2070 6173 732d 7468 726f 7567  like pass-throug
-00000b80: 6820 636f 6d6d 616e 642d 6c69 6e65 206f  h command-line o
-00000b90: 7074 696f 6e73 2061 6e64 2073 6561 6d6c  ptions and seaml
-00000ba0: 6573 7320 6861 6e64 6c69 6e67 206f 6620  ess handling of 
-00000bb0: 6669 6c65 206c 6973 7473 2e20 5361 7920  file lists. Say 
-00000bc0: 676f 6f64 6279 6520 746f 2076 6572 626f  goodbye to verbo
-00000bd0: 7369 7479 2061 6e64 2068 656c 6c6f 2074  sity and hello t
-00000be0: 6f20 6f70 7469 6d69 7a65 6420 776f 726b  o optimized work
-00000bf0: 666c 6f77 732e 5c6e 5c6e 446f 6e5c 2774  flows.\n\nDon\'t
-00000c00: 206c 6574 2073 6361 7474 6572 6564 2073   let scattered s
-00000c10: 6372 6970 7473 2061 6e64 2063 6f6d 706c  cripts and compl
-00000c20: 6578 2074 6f6f 6c69 6e67 2073 6c6f 7720  ex tooling slow 
-00000c30: 796f 7520 646f 776e 2e20 456d 6272 6163  you down. Embrac
-00000c40: 6520 4465 6c66 696e 6f20 616e 6420 7265  e Delfino and re
-00000c50: 766f 6c75 7469 6f6e 697a 6520 796f 7572  volutionize your
-00000c60: 2063 6f6d 6d61 6e64 206c 696e 6520 6578   command line ex
-00000c70: 7065 7269 656e 6365 2e20 5472 7920 4465  perience. Try De
-00000c80: 6c66 696e 6f20 746f 6461 7920 616e 6420  lfino today and 
-00000c90: 756e 6c6f 636b 2073 696d 706c 6963 6974  unlock simplicit
-00000ca0: 7920 696e 2079 6f75 7220 7072 6f6a 6563  y in your projec
-00000cb0: 7473 215c 6e5c 6e3c 212d 2d5c 6e20 2020  ts!\n\n<!--\n   
-00000cc0: 2048 6f77 2074 6f20 6765 6e65 7261 7465   How to generate
-00000cd0: 2054 4f43 2066 726f 6d20 5079 4368 6172   TOC from PyChar
-00000ce0: 6d3a 5c6e 2020 2020 6874 7470 733a 2f2f  m:\n    https://
-00000cf0: 6769 7468 7562 2e63 6f6d 2f76 7363 682f  github.com/vsch/
-00000d00: 6964 6561 2d6d 756c 7469 6d61 726b 646f  idea-multimarkdo
-00000d10: 776e 2f77 696b 692f 5461 626c 652d 6f66  wn/wiki/Table-of
-00000d20: 2d43 6f6e 7465 6e74 732d 4578 7465 6e73  -Contents-Extens
-00000d30: 696f 6e5c 6e2d 2d3e 5c6e 5b54 4f43 206c  ion\n-->\n[TOC l
-00000d40: 6576 656c 733d 312c 3220 6d61 726b 646f  evels=1,2 markdo
-00000d50: 776e 2066 6f72 6d61 7474 6564 2062 756c  wn formatted bul
-00000d60: 6c65 7420 6869 6572 6172 6368 795d 3a20  let hierarchy]: 
-00000d70: 2320 2254 6162 6c65 206f 6620 636f 6e74  # "Table of cont
-00000d80: 656e 7422 5c6e 5c6e 2320 5461 626c 6520  ent"\n\n# Table 
-00000d90: 6f66 2063 6f6e 7465 6e74 5c6e 2d20 5b49  of content\n- [I
-00000da0: 6e73 7461 6c6c 6174 696f 6e5d 2823 696e  nstallation](#in
-00000db0: 7374 616c 6c61 7469 6f6e 295c 6e2d 205b  stallation)\n- [
-00000dc0: 436f 6e66 6967 7572 6174 696f 6e5d 2823  Configuration](#
-00000dd0: 636f 6e66 6967 7572 6174 696f 6e29 5c6e  configuration)\n
-00000de0: 2d20 5b55 7361 6765 5d28 2375 7361 6765  - [Usage](#usage
-00000df0: 295c 6e2d 205b 4465 7665 6c6f 706d 656e  )\n- [Developmen
-00000e00: 745d 2823 6465 7665 6c6f 706d 656e 7429  t](#development)
-00000e10: 5c6e 2020 2d20 5b43 6f6d 6d61 6e64 7320  \n  - [Commands 
-00000e20: 6469 7363 6f76 6572 795d 2823 636f 6d6d  discovery](#comm
-00000e30: 616e 6473 2d64 6973 636f 7665 7279 295c  ands-discovery)\
-00000e40: 6e20 202d 205b 4d69 6e69 6d61 6c20 636f  n  - [Minimal co
-00000e50: 6d6d 616e 645d 2823 6d69 6e69 6d61 6c2d  mmand](#minimal-
-00000e60: 636f 6d6d 616e 6429 5c6e 2020 2d20 5b4d  command)\n  - [M
-00000e70: 696e 696d 616c 2070 6c75 6769 6e5d 2823  inimal plugin](#
-00000e80: 6d69 6e69 6d61 6c2d 706c 7567 696e 295c  minimal-plugin)\
-00000e90: 6e2d 205b 4578 6973 7469 6e67 2070 6c75  n- [Existing plu
-00000ea0: 6769 6e73 5d28 2365 7869 7374 696e 672d  gins](#existing-
-00000eb0: 706c 7567 696e 7329 5c6e 2020 2d20 5b45  plugins)\n  - [E
-00000ec0: 6e61 626c 696e 6720 6120 706c 7567 696e  nabling a plugin
-00000ed0: 5d28 2365 6e61 626c 696e 672d 612d 706c  ](#enabling-a-pl
-00000ee0: 7567 696e 295c 6e20 202d 205b 456e 6162  ugin)\n  - [Enab
-00000ef0: 6c69 6e67 2f64 6973 6162 6c69 6e67 2063  ling/disabling c
-00000f00: 6f6d 6d61 6e64 735d 2823 656e 6162 6c69  ommands](#enabli
-00000f10: 6e67 6469 7361 626c 696e 672d 636f 6d6d  ngdisabling-comm
-00000f20: 616e 6473 295c 6e2d 205b 4164 7661 6e63  ands)\n- [Advanc
-00000f30: 6564 2075 7361 6765 5d28 2361 6476 616e  ed usage](#advan
-00000f40: 6365 642d 7573 6167 6529 5c6e 2020 2d20  ced-usage)\n  - 
-00000f50: 5b41 7574 6f2d 636f 6d70 6c65 7469 6f6e  [Auto-completion
-00000f60: 5d28 2361 7574 6f2d 636f 6d70 6c65 7469  ](#auto-completi
-00000f70: 6f6e 295c 6e20 202d 205b 5275 6e6e 696e  on)\n  - [Runnin
-00000f80: 6720 6578 7465 726e 616c 2070 726f 6772  g external progr
-00000f90: 616d 735d 2823 7275 6e6e 696e 672d 6578  ams](#running-ex
-00000fa0: 7465 726e 616c 2d70 726f 6772 616d 7329  ternal-programs)
-00000fb0: 5c6e 2020 2d20 5b4f 7074 696f 6e61 6c20  \n  - [Optional 
-00000fc0: 6465 7065 6e64 656e 6369 6573 5d28 236f  dependencies](#o
-00000fd0: 7074 696f 6e61 6c2d 6465 7065 6e64 656e  ptional-dependen
-00000fe0: 6369 6573 295c 6e20 202d 205b 5072 6f6a  cies)\n  - [Proj
-00000ff0: 6563 7420 7365 7474 696e 6773 5d28 2370  ect settings](#p
-00001000: 726f 6a65 6374 2d73 6574 7469 6e67 7329  roject-settings)
-00001010: 5c6e 2020 2d20 5b50 6c75 6769 6e20 7365  \n  - [Plugin se
-00001020: 7474 696e 6773 5d28 2370 6c75 6769 6e2d  ttings](#plugin-
-00001030: 7365 7474 696e 6773 295c 6e20 202d 205b  settings)\n  - [
-00001040: 5072 6f6a 6563 7420 7370 6563 6966 6963  Project specific
-00001050: 206f 7665 7272 6964 6573 5d28 2370 726f   overrides](#pro
-00001060: 6a65 6374 2d73 7065 6369 6669 632d 6f76  ject-specific-ov
-00001070: 6572 7269 6465 7329 5c6e 2020 2d20 5b47  errides)\n  - [G
-00001080: 726f 7570 696e 6720 636f 6d6d 616e 6473  rouping commands
-00001090: 5d28 2367 726f 7570 696e 672d 636f 6d6d  ](#grouping-comm
-000010a0: 616e 6473 295c 6e5c 6e23 2049 6e73 7461  ands)\n\n# Insta
-000010b0: 6c6c 6174 696f 6e5c 6e5c 6e2d 2070 6970  llation\n\n- pip
-000010c0: 3a20 6070 6970 2069 6e73 7461 6c6c 2064  : `pip install d
-000010d0: 656c 6669 6e6f 605c 6e2d 2050 6f65 7472  elfino`\n- Poetr
-000010e0: 793a 2060 706f 6574 7279 2061 6464 202d  y: `poetry add -
-000010f0: 2d67 726f 7570 3d64 6576 2064 656c 6669  -group=dev delfi
-00001100: 6e6f 605c 6e2d 2050 6970 656e 763a 2060  no`\n- Pipenv: `
-00001110: 7069 7065 6e76 2069 6e73 7461 6c6c 202d  pipenv install -
-00001120: 6420 6465 6c66 696e 6f60 5c6e 5c6e 6f72  d delfino`\n\nor
-00001130: 205c 6e5c 6e2d 2070 6970 3a20 6070 6970   \n\n- pip: `pip
-00001140: 2069 6e73 7461 6c6c 2064 656c 6669 6e6f   install delfino
-00001150: 5b63 6f6d 706c 6574 696f 6e5d 605c 6e2d  [completion]`\n-
-00001160: 2050 6f65 7472 793a 2060 706f 6574 7279   Poetry: `poetry
-00001170: 2061 6464 202d 2d67 726f 7570 3d64 6576   add --group=dev
-00001180: 2064 656c 6669 6e6f 5b63 6f6d 706c 6574   delfino[complet
-00001190: 696f 6e5d 605c 6e2d 2050 6970 656e 763a  ion]`\n- Pipenv:
-000011a0: 2060 7069 7065 6e76 2069 6e73 7461 6c6c   `pipenv install
-000011b0: 202d 6420 6465 6c66 696e 6f5b 636f 6d70   -d delfino[comp
-000011c0: 6c65 7469 6f6e 5d60 5c6e 5c6e 746f 2065  letion]`\n\nto e
-000011d0: 6e61 626c 6520 5b61 7574 6f2d 636f 6d70  nable [auto-comp
-000011e0: 6c65 7469 6f6e 5d28 2361 7574 6f2d 636f  letion](#auto-co
-000011f0: 6d70 6c65 7469 6f6e 292e 5c6e 5c6e 2320  mpletion).\n\n# 
-00001200: 436f 6e66 6967 7572 6174 696f 6e5c 6e5c  Configuration\n\
-00001210: 6e41 6c6c 2063 6f6e 6669 6775 7261 7469  nAll configurati
-00001220: 6f6e 2069 7320 6578 7065 6374 6564 2074  on is expected t
-00001230: 6f20 6c69 7665 2069 6e20 6f6e 6520 6f66  o live in one of
-00001240: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-00001250: 696c 6573 3a5c 6e5c 6e2d 2060 7079 7072  iles:\n\n- `pypr
-00001260: 6f6a 6563 742e 746f 6d6c 6020 696e 2074  oject.toml` in t
-00001270: 6865 2070 726f 6a65 6374 2072 6f6f 745c  he project root\
-00001280: 6e2d 2060 2e64 656c 6669 6e6f 7263 6020  n- `.delfinorc` 
-00001290: 696e 2074 6865 2070 726f 6a65 6374 2072  in the project r
-000012a0: 6f6f 7420 2d20 746f 2061 6c6c 6f77 2064  oot - to allow d
-000012b0: 6576 2073 7065 6369 6669 6320 636f 6e66  ev specific conf
-000012c0: 6967 2c20 6e6f 7420 736f 7572 6365 2063  ig, not source c
-000012d0: 6f6e 7472 6f6c 6c65 6420 6f72 2066 6f72  ontrolled or for
-000012e0: 206e 6f6e 2d50 7974 686f 6e20 7072 6f6a   non-Python proj
-000012f0: 6563 7473 5c6e 2d20 602e 6465 6c66 696e  ects\n- `.delfin
-00001300: 6f72 6360 2069 6e20 7468 6520 7573 6572  orc` in the user
-00001310: 2068 6f6d 6520 6469 7265 6374 6f72 7920   home directory 
-00001320: 2d20 666f 7220 7573 6572 2074 6f6f 6c73  - for user tools
-00001330: 2061 7661 696c 6162 6c65 2069 6e20 7468   available in th
-00001340: 6520 7379 7374 656d 5c6e 5c6e 4966 206d  e system\n\nIf m
-00001350: 756c 7469 706c 6520 6669 6c65 7320 6172  ultiple files ar
-00001360: 6520 6469 7363 6f76 6572 6564 2c20 6f6e  e discovered, on
-00001370: 6c79 2074 6865 2068 6967 6865 7374 206f  ly the highest o
-00001380: 6e65 2069 6e20 7468 6520 6c69 7374 2077  ne in the list w
-00001390: 696c 6c20 6265 2075 7365 642e 5c6e 5c6e  ill be used.\n\n
-000013a0: 5468 6520 666f 726d 6174 2066 6f72 2060  The format for `
-000013b0: 2e64 656c 6669 6e6f 7263 6020 6973 2074  .delfinorc` is t
-000013c0: 6865 2073 616d 6520 6173 2066 6f72 2060  he same as for `
-000013d0: 7079 7072 6f6a 6563 742e 746f 6d6c 602e  pyproject.toml`.
-000013e0: 5c6e 5c6e 2320 5573 6167 655c 6e5c 6e52  \n\n# Usage\n\nR
-000013f0: 756e 2060 6465 6c66 696e 6f20 2d2d 6865  un `delfino --he
-00001400: 6c70 6020 746f 2073 6565 2061 6c6c 2061  lp` to see all a
-00001410: 7661 696c 6162 6c65 2063 6f6d 6d61 6e64  vailable command
-00001420: 7320 616e 6420 7468 6569 7220 7573 6167  s and their usag
-00001430: 652e 5c6e 5c6e 2320 4465 7665 6c6f 706d  e.\n\n# Developm
-00001440: 656e 745c 6e5c 6e44 656c 6669 6e6f 2069  ent\n\nDelfino i
-00001450: 7320 6120 7369 6d70 6c65 2077 7261 7070  s a simple wrapp
-00001460: 6572 2061 726f 756e 6420 5b43 6c69 636b  er around [Click
-00001470: 2063 6f6d 6d61 6e64 735d 2868 7474 7073   commands](https
-00001480: 3a2f 2f63 6c69 636b 2e70 616c 6c65 7473  ://click.pallets
-00001490: 7072 6f6a 6563 7473 2e63 6f6d 2f71 7569  projects.com/qui
-000014a0: 636b 7374 6172 742f 2362 6173 6963 2d63  ckstart/#basic-c
-000014b0: 6f6e 6365 7074 732d 6372 6561 7469 6e67  oncepts-creating
-000014c0: 2d61 2d63 6f6d 6d61 6e64 292e 2041 6e79  -a-command). Any
-000014d0: 2043 6c69 636b 2063 6f6d 6d61 6e64 2077   Click command w
-000014e0: 696c 6c20 6265 2061 6363 6570 7465 6420  ill be accepted 
-000014f0: 6279 2044 656c 6669 6e6f 2e5c 6e5c 6e23  by Delfino.\n\n#
-00001500: 2320 436f 6d6d 616e 6473 2064 6973 636f  # Commands disco
-00001510: 7665 7279 5c6e 5c6e 4465 6c66 696e 6f20  very\n\nDelfino 
-00001520: 6c6f 6f6b 7320 666f 7220 616e 7920 5b60  looks for any [`
-00001530: 636c 6963 6b2e 436f 6d6d 616e 6460 5d28  click.Command`](
-00001540: 6874 7470 733a 2f2f 636c 6963 6b2e 7061  https://click.pa
-00001550: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
-00001560: 6d2f 656e 2f38 2e30 2e78 2f61 7069 2f23  m/en/8.0.x/api/#
-00001570: 636c 6963 6b2e 436f 6d6d 616e 6429 2073  click.Command) s
-00001580: 7562 2d63 6c61 7373 2069 6e20 7468 6520  ub-class in the 
-00001590: 666f 6c6c 6f77 696e 6720 6c6f 6361 7469  following locati
-000015a0: 6f6e 733a 5c6e 5c6e 2d20 6063 6f6d 6d61  ons:\n\n- `comma
-000015b0: 6e64 7360 2066 6f6c 6465 7220 696e 2074  nds` folder in t
-000015c0: 6865 2072 6f6f 7420 6f66 2074 6865 2070  he root of the p
-000015d0: 726f 6a65 6374 2028 6e65 7874 2074 6f20  roject (next to 
-000015e0: 7468 6520 6070 7970 726f 6a65 6374 2e74  the `pyproject.t
-000015f0: 6f6d 6c60 2066 696c 6529 2e20 5468 6973  oml` file). This
-00001600: 206c 6f63 6174 696f 6e20 6973 2075 7365   location is use
-00001610: 6675 6c20 666f 7220 636f 6d6d 616e 6473  ful for commands
-00001620: 2074 6861 7420 646f 6e5c 2774 206e 6565   that don\'t nee
-00001630: 6420 746f 2062 6520 7265 706c 6963 6174  d to be replicat
-00001640: 6564 2069 6e20 6d75 6c74 6970 6c65 206c  ed in multiple l
-00001650: 6f63 6174 696f 6e73 2f70 726f 6a65 6374  ocations/project
-00001660: 732e 2054 6f20 6368 616e 6765 2074 6865  s. To change the
-00001670: 2064 6566 6175 6c74 206c 6f63 6174 696f   default locatio
-00001680: 6e2c 2075 7365 2074 6865 2060 746f 6f6c  n, use the `tool
-00001690: 2e64 656c 6669 6e6f 2e6c 6f63 616c 5f63  .delfino.local_c
-000016a0: 6f6d 6d61 6e64 5f66 6f6c 6465 7273 6020  ommand_folders` 
-000016b0: 636f 6e66 6967 206f 7074 696f 6e2e 2049  config option. I
-000016c0: 7420 616c 6c6f 7773 2073 7065 6369 6679  t allows specify
-000016d0: 696e 6720 6d6f 7265 2074 6861 6e20 6f6e  ing more than on
-000016e0: 6520 666f 6c64 6572 2e5c 6e2d 2070 7974  e folder.\n- pyt
-000016f0: 686f 6e20 6d6f 6475 6c65 2069 6d70 6f72  hon module impor
-00001700: 7420 7061 7468 2028 603c 494d 504f 5254  t path (`<IMPORT
-00001710: 5f50 4154 483e 6029 2073 7065 6369 6669  _PATH>`) specifi
-00001720: 6564 2062 7920 6065 6e74 7279 5f70 6f69  ed by `entry_poi
-00001730: 6e74 6020 6f66 205b 6120 706c 7567 696e  nt` of [a plugin
-00001740: 5d28 236d 696e 696d 616c 2d70 6c75 6769  ](#minimal-plugi
-00001750: 6e29 3a5c 6e20 2060 6060 746f 6d6c 5c6e  n):\n  ```toml\n
-00001760: 2020 5b74 6f6f 6c2e 706f 6574 7279 2e70    [tool.poetry.p
-00001770: 6c75 6769 6e73 5d20 2320 4f70 7469 6f6e  lugins] # Option
-00001780: 616c 2073 7570 6572 2074 6162 6c65 5c6e  al super table\n
-00001790: 5c6e 2020 5b74 6f6f 6c2e 706f 6574 7279  \n  [tool.poetry
-000017a0: 2e70 6c75 6769 6e73 2e22 6465 6c66 696e  .plugins."delfin
-000017b0: 6f2e 706c 7567 696e 225d 5c6e 2020 2264  o.plugin"]\n  "d
-000017c0: 656c 6669 6e6f 2d3c 504c 5547 494e 5f4e  elfino-<PLUGIN_N
-000017d0: 414d 453e 2220 3d20 223c 494d 504f 5254  AME>" = "<IMPORT
-000017e0: 5f50 4154 483e 225c 6e20 2060 6060 5c6e  _PATH>"\n  ```\n
-000017f0: 2d20 466f 6c64 6572 2073 7065 6369 6669  - Folder specifi
-00001800: 6564 2069 6e20 7468 6520 5b63 6f6e 6669  ed in the [confi
-00001810: 6720 6669 6c65 5d28 2363 6f6e 6669 6775  g file](#configu
-00001820: 7261 7469 6f6e 2920 756e 6465 7220 6074  ration) under `t
-00001830: 6f6f 6c2e 6465 6c66 696e 6f2e 6c6f 6361  ool.delfino.loca
-00001840: 6c5f 636f 6d6d 616e 6473 5f64 6972 6563  l_commands_direc
-00001850: 746f 7279 602e 5c6e 5c6e 416e 7920 6669  tory`.\n\nAny fi
-00001860: 6c65 7320 7374 6172 7469 6e67 2077 6974  les starting wit
-00001870: 6820 616e 2075 6e64 6572 7363 6f72 652c  h an underscore,
-00001880: 2065 7863 6570 7420 666f 7220 605f 5f69   except for `__i
-00001890: 6e69 745f 5f2e 7079 602c 2077 696c 6c20  nit__.py`, will 
-000018a0: 6265 2069 676e 6f72 6564 2e5c 6e5c 6e3e  be ignored.\n\n>
-000018b0: 202a 2a57 6172 6e69 6e67 2a2a 5c6e 3e20   **Warning**\n> 
-000018c0: 466f 6c64 6572 7320 6172 6520 4e4f 5420  Folders are NOT 
-000018d0: 696e 7370 6563 7465 6420 7265 6375 7273  inspected recurs
-000018e0: 6976 656c 792e 2049 6620 796f 7520 706c  ively. If you pl
-000018f0: 6163 6520 616e 7920 636f 6d6d 616e 6473  ace any commands
-00001900: 2069 6e74 6f20 6e65 7374 6564 2066 6f6c   into nested fol
-00001910: 6465 7273 2c20 7468 6579 2077 696c 6c20  ders, they will 
-00001920: 6e6f 7420 6265 206c 6f61 6465 6420 6279  not be loaded by
-00001930: 2044 656c 6669 6e6f 2e5c 6e5c 6e5c 6e23   Delfino.\n\n\n#
-00001940: 2320 4d69 6e69 6d61 6c20 636f 6d6d 616e  # Minimal comman
-00001950: 645c 6e5c 6e3c 212d 2d20 544f 444f 2852  d\n\n<!-- TODO(R
-00001960: 6164 656b 293a 2044 656c 6669 6e6f 2065  adek): Delfino e
-00001970: 7870 6563 7473 2060 7079 7072 6f6a 6563  xpects `pyprojec
-00001980: 742e 746f 6d6c 6020 636f 6e66 6967 7572  t.toml` configur
-00001990: 6564 2e20 2d2d 3e5c 6e3c 212d 2d20 544f  ed. -->\n<!-- TO
-000019a0: 444f 2852 6164 656b 293a 2044 656c 6669  DO(Radek): Delfi
-000019b0: 6e6f 2065 7870 6563 7473 2050 6f65 7472  no expects Poetr
-000019c0: 7920 6f72 2050 6970 656e 7620 746f 2062  y or Pipenv to b
-000019d0: 6520 6176 6169 6c61 626c 652e 202d 2d3e  e available. -->
-000019e0: 5c6e 5c6e 312e 2043 7265 6174 6520 6120  \n\n1. Create a 
-000019f0: 6063 6f6d 6d61 6e64 7360 2066 6f6c 6465  `commands` folde
-00001a00: 723a 5c6e 2020 2060 6060 7368 656c 6c20  r:\n   ```shell 
-00001a10: 7363 7269 7074 5c6e 2020 206d 6b64 6972  script\n   mkdir
-00001a20: 2063 6f6d 6d61 6e64 735c 6e20 2020 6060   commands\n   ``
-00001a30: 605c 6e32 2e20 4372 6561 7465 2061 2060  `\n2. Create a `
-00001a40: 636f 6d6d 616e 6473 2f5f 5f69 6e69 745f  commands/__init_
-00001a50: 5f2e 7079 6020 6669 6c65 2c20 7769 7468  _.py` file, with
-00001a60: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00001a70: 6f6e 7465 6e74 3a5c 6e20 2020 6060 6070  ontent:\n   ```p
-00001a80: 7974 686f 6e5c 6e20 2020 696d 706f 7274  ython\n   import
-00001a90: 2063 6c69 636b 5c6e 2020 205c 6e20 2020   click\n   \n   
-00001aa0: 4063 6c69 636b 2e63 6f6d 6d61 6e64 2829  @click.command()
-00001ab0: 5c6e 2020 2064 6566 2063 6f6d 6d61 6e64  \n   def command
-00001ac0: 5f74 6573 7428 293a 5c6e 2020 2020 2020  _test():\n      
-00001ad0: 2022 2222 5465 7374 7320 636f 6d6d 616e   """Tests comman
-00001ae0: 6473 2070 6c61 6365 6420 696e 2074 6865  ds placed in the
-00001af0: 2060 636f 6d6d 616e 6473 6020 666f 6c64   `commands` fold
-00001b00: 6572 2061 7265 206c 6f61 6465 642e 2222  er are loaded.""
-00001b10: 225c 6e20 2020 2020 2020 7072 696e 7428  "\n       print(
-00001b20: 22e2 9ca8 2054 6869 7320 636f 6d6d 616e  "... This comman
-00001b30: 6420 776f 726b 7321 20e2 9ca8 2229 5c6e  d works! ...")\n
-00001b40: 2020 2060 6060 5c6e 332e 2053 6565 2069     ```\n3. See i
-00001b50: 6620 4465 6c66 696e 6f20 6c6f 6164 7320  f Delfino loads 
-00001b60: 7468 6520 636f 6d6d 616e 642e 204f 7065  the command. Ope
-00001b70: 6e20 6120 7465 726d 696e 616c 2061 6e64  n a terminal and
-00001b80: 2069 6e20 7468 6520 726f 6f74 206f 6620   in the root of 
-00001b90: 7468 6520 7072 6f6a 6563 742c 2063 616c  the project, cal
-00001ba0: 6c3a 2060 6465 6c66 696e 6f20 2d2d 6865  l: `delfino --he
-00001bb0: 6c70 602e 2059 6f75 2073 686f 756c 6420  lp`. You should 
-00001bc0: 7365 6520 736f 6d65 7468 696e 6720 6c69  see something li
-00001bd0: 6b65 2074 6869 733a 5c6e 2020 2060 6060  ke this:\n   ```
-00001be0: 7465 7874 5c6e 2020 2055 7361 6765 3a20  text\n   Usage: 
-00001bf0: 6465 6c66 696e 6f20 5b4f 5054 494f 4e53  delfino [OPTIONS
-00001c00: 5d20 434f 4d4d 414e 4420 5b41 5247 535d  ] COMMAND [ARGS]
-00001c10: 2e2e 2e5c 6e20 2020 5c6e 2020 204f 7074  ...\n   \n   Opt
-00001c20: 696f 6e73 3a5c 6e20 2020 2020 2d2d 6865  ions:\n     --he
-00001c30: 6c70 2020 5368 6f77 2074 6869 7320 6d65  lp  Show this me
-00001c40: 7373 6167 6520 616e 6420 6578 6974 2e5c  ssage and exit.\
-00001c50: 6e20 2020 5c6e 2020 2043 6f6d 6d61 6e64  n   \n   Command
-00001c60: 733a 5c6e 2020 2020 202e 2e2e 5c6e 2020  s:\n     ...\n  
-00001c70: 2020 2063 6f6d 6d61 6e64 2d74 6573 7420     command-test 
-00001c80: 2020 2020 2020 2020 2020 2054 6573 7473             Tests
-00001c90: 2063 6f6d 6d61 6e64 7320 706c 6163 6564   commands placed
-00001ca0: 2069 6e20 7468 6520 6063 6f6d 6d61 6e64   in the `command
-00001cb0: 7360 2066 6f6c 6465 722e 2e2e 5c6e 2020  s` folder...\n  
-00001cc0: 2020 202e 2e2e 5c6e 2020 2060 6060 5c6e     ...\n   ```\n
-00001cd0: 342e 2052 756e 2074 6865 2063 6f6d 6d61  4. Run the comma
-00001ce0: 6e64 2077 6974 6820 6064 656c 6669 6e6f  nd with `delfino
-00001cf0: 2063 6f6d 6d61 6e64 2d74 6573 7460 5c6e   command-test`\n
-00001d00: 5c6e 2323 204d 696e 696d 616c 2070 6c75  \n## Minimal plu
-00001d10: 6769 6e5c 6e5c 6e49 6620 796f 755c 2764  gin\n\nIf you\'d
-00001d20: 206c 696b 6520 746f 2075 7365 206f 6e65   like to use one
-00001d30: 206f 7220 6d6f 7265 2063 6f6d 6d61 6e64   or more command
-00001d40: 7320 696e 206d 756c 7469 706c 6520 706c  s in multiple pl
-00001d50: 6163 6573 2c20 796f 7520 6361 6e20 6372  aces, you can cr
-00001d60: 6561 7465 2061 2070 6c75 6769 6e2e 2041  eate a plugin. A
-00001d70: 2070 6c75 6769 6e20 6973 206a 7573 7420   plugin is just 
-00001d80: 6120 7265 6775 6c61 7220 5079 7468 6f6e  a regular Python
-00001d90: 2070 6163 6b61 6765 2077 6974 6820 7370   package with sp
-00001da0: 6563 6966 6963 2065 6e74 7279 2070 6f69  ecific entry poi
-00001db0: 6e74 2074 656c 6c69 6e67 2044 656c 6669  nt telling Delfi
-00001dc0: 6e6f 2069 7420 7368 6f75 6c64 2075 7365  no it should use
-00001dd0: 2069 742e 2049 7420 6361 6e20 616c 736f   it. It can also
-00001de0: 2062 6520 6469 7374 7269 6275 7465 6420   be distributed 
-00001df0: 6173 2061 6e79 206f 7468 6572 2050 7974  as any other Pyt
-00001e00: 686f 6e20 7061 636b 6167 6573 2c20 666f  hon packages, fo
-00001e10: 7220 6578 616d 706c 6520 7669 6120 5079  r example via Py
-00001e20: 7069 2e5c 6e5c 6e54 6865 2071 7569 636b  pi.\n\nThe quick
-00001e30: 6573 7420 7761 7920 746f 2063 7265 6174  est way to creat
-00001e40: 6520 6f6e 6520 6973 2074 6f20 7573 6520  e one is to use 
-00001e50: 6120 5b44 656c 6669 6e6f 2070 6c75 6769  a [Delfino plugi
-00001e60: 6e20 636f 6f6b 6965 6375 7474 6572 2074  n cookiecutter t
-00001e70: 656d 706c 6174 655d 2868 7474 7073 3a2f  emplate](https:/
-00001e80: 2f67 6974 6875 622e 636f 6d2f 7261 6465  /github.com/rade
-00001e90: 6b6c 6174 2f64 656c 6669 6e6f 2d70 6c75  klat/delfino-plu
-00001ea0: 6769 6e2d 636f 6f6b 6965 6375 7474 6572  gin-cookiecutter
-00001eb0: 2d74 656d 706c 6174 6529 2c20 7768 6963  -template), whic
-00001ec0: 6820 6173 6b73 2079 6f75 2073 6576 6572  h asks you sever
-00001ed0: 616c 2071 7565 7374 696f 6e73 2061 6e64  al questions and
-00001ee0: 2073 6574 7320 7570 2074 6865 2077 686f   sets up the who
-00001ef0: 6c65 2070 726f 6a65 6374 2e5c 6e5c 6e41  le project.\n\nA
-00001f00: 6c74 6572 6e61 7469 7665 6c79 2c20 796f  lternatively, yo
-00001f10: 7520 6361 6e20 6765 7420 696e 7370 6972  u can get inspir
-00001f20: 6564 2062 7920 5b74 6865 2064 656d 6f20  ed by [the demo 
-00001f30: 706c 7567 696e 5d28 6874 7470 733a 2f2f  plugin](https://
-00001f40: 6769 7468 7562 2e63 6f6d 2f72 6164 656b  github.com/radek
-00001f50: 6c61 742f 6465 6c66 696e 6f2d 6465 6d6f  lat/delfino-demo
-00001f60: 2920 6f72 2061 6e79 206f 6620 7468 6520  ) or any of the 
-00001f70: 6f74 6865 7220 5b65 7869 7374 696e 6720  other [existing 
-00001f80: 706c 7567 696e 735d 2823 706c 7567 696e  plugins](#plugin
-00001f90: 7329 2e5c 6e5c 6e23 2045 7869 7374 696e  s).\n\n# Existin
-00001fa0: 6720 706c 7567 696e 735c 6e5c 6e50 6c75  g plugins\n\nPlu
-00001fb0: 6769 6e73 2063 616e 2067 7265 6174 6c79  gins can greatly
-00001fc0: 2072 6564 7563 6520 636f 6465 2064 7570   reduce code dup
-00001fd0: 6c69 6361 7469 6f6e 2061 6e64 2f6f 7220  lication and/or 
-00001fe0: 7072 6f6d 6f74 6520 796f 7572 206f 776e  promote your own
-00001ff0: 2073 7461 6e64 6172 6473 2069 6e20 6d75   standards in mu
-00002000: 6c74 6970 6c65 2070 6c61 6365 732e 2046  ltiple places. F
-00002010: 6f72 2065 7861 6d70 6c65 2c20 796f 7520  or example, you 
-00002020: 6361 6e20 6372 6561 7465 2061 2070 6c75  can create a plu
-00002030: 6769 6e20 7772 6170 7069 6e67 2063 6f6d  gin wrapping com
-00002040: 6d6f 6e20 6c69 6e74 696e 6720 746f 6f6c  mon linting tool
-00002050: 7320 7468 6174 2079 6f75 2075 7365 206f  s that you use o
-00002060: 6e20 796f 7572 2070 726f 6a65 6374 732c  n your projects,
-00002070: 2069 6e63 6c75 6469 6e67 2074 6865 6972   including their
-00002080: 2064 6566 6175 6c74 2063 6f6e 6669 6775   default configu
-00002090: 7261 7469 6f6e 2e20 4b65 6570 696e 6720  ration. Keeping 
-000020a0: 7468 6520 7275 6c65 7320 616e 6420 6372  the rules and cr
-000020b0: 6561 7469 6e67 206e 6577 2070 726f 6a65  eating new proje
-000020c0: 6374 7320 7769 7468 2074 6865 2073 616d  cts with the sam
-000020d0: 6520 7374 796c 6520 7375 6464 656e 6c79  e style suddenly
-000020e0: 2062 6563 6f6d 6573 2061 206d 6174 7465   becomes a matte
-000020f0: 7220 6f66 2069 6e73 7461 6c6c 696e 6720  r of installing 
-00002100: 6f6e 6520 5079 7468 6f6e 206c 6962 7261  one Python libra
-00002110: 7279 2e5c 6e5c 6e45 6163 6820 706c 7567  ry.\n\nEach plug
-00002120: 696e 2063 616e 2063 6f6e 7461 696e 206f  in can contain o
-00002130: 6e65 206f 7220 6d6f 7265 2043 6c69 636b  ne or more Click
-00002140: 2063 6f6d 6d61 6e64 7320 7468 6174 2061   commands that a
-00002150: 7265 2061 7574 6f6d 6174 6963 616c 6c79  re automatically
-00002160: 2064 6973 636f 7665 7265 6420 616e 6420   discovered and 
-00002170: 6578 706f 7365 6420 6279 2044 656c 6669  exposed by Delfi
-00002180: 6e6f 2e20 5365 6520 5b60 6465 6c66 696e  no. See [`delfin
-00002190: 6f2d 6465 6d6f 605d 2868 7474 7073 3a2f  o-demo`](https:/
-000021a0: 2f67 6974 6875 622e 636f 6d2f 7261 6465  /github.com/rade
-000021b0: 6b6c 6174 2f64 656c 6669 6e6f 2d64 656d  klat/delfino-dem
-000021c0: 6f29 2066 6f72 2061 206d 696e 696d 616c  o) for a minimal
-000021d0: 2070 6c75 6769 6e2c 2077 6869 6368 2070   plugin, which p
-000021e0: 726f 7669 6465 2061 2060 6465 6d6f 6020  rovide a `demo` 
-000021f0: 636f 6d6d 616e 6420 7072 696e 7469 6e67  command printing
-00002200: 206f 7574 2061 206d 6573 7361 6765 2e5c   out a message.\
-00002210: 6e5c 6e45 7869 7374 696e 6720 706c 7567  n\nExisting plug
-00002220: 696e 733a 5c6e 5c6e 7c20 506c 7567 696e  ins:\n\n| Plugin
-00002230: 206e 616d 6520 2020 2020 2020 2020 2020   name           
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002260: 2020 2020 2020 207c 2044 6573 6372 6970         | Descrip
-00002270: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022c0: 2020 2020 2020 2020 2020 2020 7c5c 6e7c              |\n|
-000022d0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000022e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000022f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a  --------------|:
-00002310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002370: 2d2d 2d7c 5c6e 7c20 5b64 656c 6669 6e6f  ---|\n| [delfino
-00002380: 2d64 656d 6f5d 2868 7474 7073 3a2f 2f67  -demo](https://g
-00002390: 6974 6875 622e 636f 6d2f 7261 6465 6b6c  ithub.com/radekl
-000023a0: 6174 2f64 656c 6669 6e6f 2d64 656d 6f29  at/delfino-demo)
-000023b0: 2020 2020 207c 2041 206d 696e 696d 616c       | A minimal
-000023c0: 2070 6c75 6769 6e20 6578 616d 706c 6520   plugin example 
-000023d0: 666f 7220 4465 6c66 696e 6f2e 2043 6f6e  for Delfino. Con
-000023e0: 7461 696e 7320 6f6e 6520 636f 6d6d 616e  tains one comman
-000023f0: 6420 7072 696e 7469 6e67 2061 206d 6573  d printing a mes
-00002400: 7361 6765 2e20 2020 2020 2020 2020 2020  sage.           
-00002410: 2020 2020 2020 2020 2020 7c5c 6e7c 205b            |\n| [
-00002420: 6465 6c66 696e 6f2d 636f 7265 5d28 6874  delfino-core](ht
-00002430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002440: 2f72 6164 656b 6c61 742f 6465 6c66 696e  /radeklat/delfin
-00002450: 6f2d 636f 7265 2920 2020 2020 7c20 436f  o-core)     | Co
-00002460: 6d6d 616e 6473 2077 7261 7070 696e 6720  mmands wrapping 
-00002470: 746f 6f6c 7320 7573 6564 2064 7572 696e  tools used durin
-00002480: 6720 6576 6572 7920 6461 7920 6465 7665  g every day deve
-00002490: 6c6f 706d 656e 7420 286c 696e 7469 6e67  lopment (linting
-000024a0: 2c20 7465 7374 696e 672c 2064 6570 656e  , testing, depen
-000024b0: 6465 6e63 6965 7320 7570 6461 7465 292e  dencies update).
-000024c0: 207c 5c6e 7c20 5b64 656c 6669 6e6f 2d64   |\n| [delfino-d
-000024d0: 6f63 6b65 725d 2868 7474 7073 3a2f 2f67  ocker](https://g
-000024e0: 6974 6875 622e 636f 6d2f 7261 6465 6b6c  ithub.com/radekl
-000024f0: 6174 2f64 656c 6669 6e6f 2d64 6f63 6b65  at/delfino-docke
-00002500: 7229 207c 2044 6f63 6b65 7220 6275 696c  r) | Docker buil
-00002510: 6420 6865 6c70 6572 2073 6372 6970 742e  d helper script.
-00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002560: 2020 2020 2020 2020 7c5c 6e5c 6e23 2320          |\n\n## 
-00002570: 456e 6162 6c69 6e67 2061 2070 6c75 6769  Enabling a plugi
-00002580: 6e5c 6e5c 6e46 6f72 2073 6563 7572 6974  n\n\nFor securit
-00002590: 7920 7265 6173 6f6e 732c 2070 6c75 6769  y reasons, plugi
-000025a0: 6e73 2061 7265 2064 6973 6162 6c65 6420  ns are disabled 
-000025b0: 6279 2064 6566 6175 6c74 2e20 546f 2065  by default. To e
-000025c0: 6e61 626c 6520 6120 706c 7567 696e 2c20  nable a plugin, 
-000025d0: 796f 7520 6861 7665 2074 6f20 696e 636c  you have to incl
-000025e0: 7564 6520 6974 2069 6e20 7468 6520 6070  ude it in the `p
-000025f0: 7970 726f 6a65 6374 2e74 6f6d 6c60 2066  yproject.toml` f
-00002600: 696c 653a 5c6e 5c6e 6060 6074 6f6d 6c5c  ile:\n\n```toml\
-00002610: 6e5b 746f 6f6c 2e64 656c 6669 6e6f 2e70  n[tool.delfino.p
-00002620: 6c75 6769 6e73 2e3c 504c 5547 494e 5f4e  lugins.<PLUGIN_N
-00002630: 414d 453e 5d5c 6e60 6060 5c6e 5c6e 2323  AME>]\n```\n\n##
-00002640: 2045 6e61 626c 696e 672f 6469 7361 626c   Enabling/disabl
-00002650: 696e 6720 636f 6d6d 616e 6473 5c6e 5c6e  ing commands\n\n
-00002660: 4279 2064 6566 6175 6c74 2c20 616c 6c20  By default, all 
-00002670: 636f 6d6d 616e 6473 2061 7265 2065 6e61  commands are ena
-00002680: 626c 6564 2e20 5573 6520 6065 6e61 626c  bled. Use `enabl
-00002690: 655f 636f 6d6d 616e 6473 6020 6f72 2060  e_commands` or `
-000026a0: 6469 7361 626c 655f 636f 6d6d 616e 6473  disable_commands
-000026b0: 6020 2074 6f20 7368 6f77 206f 6e6c 7920  `  to show only 
-000026c0: 6120 7375 6273 6574 206f 6620 636f 6d6d  a subset of comm
-000026d0: 616e 6473 2e20 4966 2062 6f74 6820 7573  ands. If both us
-000026e0: 6564 2c20 6469 7361 626c 6564 2063 6f6d  ed, disabled com
-000026f0: 6d61 6e64 7320 6172 6520 7375 6274 7261  mands are subtra
-00002700: 6374 6564 2066 726f 6d20 7468 6520 7365  cted from the se
-00002710: 7420 6f66 2065 6e61 626c 6564 2063 6f6d  t of enabled com
-00002720: 6d61 6e64 732e 5c6e 5c6e 6060 6074 6f6d  mands.\n\n```tom
-00002730: 6c5c 6e23 205b 746f 6f6c 2e64 656c 6669  l\n# [tool.delfi
-00002740: 6e6f 2e70 6c75 6769 6e73 2e3c 504c 5547  no.plugins.<PLUG
-00002750: 494e 5f4e 414d 455f 413e 5d5c 6e23 2065  IN_NAME_A>]\n# e
-00002760: 6e61 626c 655f 636f 6d6d 616e 6473 203d  nable_commands =
-00002770: 205b 3c43 4f4d 4d41 4e44 5f4e 414d 453e   [<COMMAND_NAME>
-00002780: 5d5c 6e23 2064 6973 6162 6c65 5f63 6f6d  ]\n# disable_com
-00002790: 6d61 6e64 7320 3d20 5b3c 434f 4d4d 414e  mands = [<COMMAN
-000027a0: 445f 4e41 4d45 3e5d 5c6e 5c6e 2320 5b74  D_NAME>]\n\n# [t
-000027b0: 6f6f 6c2e 6465 6c66 696e 6f2e 706c 7567  ool.delfino.plug
-000027c0: 696e 732e 3c50 4c55 4749 4e5f 4e41 4d45  ins.<PLUGIN_NAME
-000027d0: 5f42 3e5d 5c6e 2320 656e 6162 6c65 5f63  _B>]\n# enable_c
-000027e0: 6f6d 6d61 6e64 7320 3d20 5b3c 434f 4d4d  ommands = [<COMM
-000027f0: 414e 445f 4e41 4d45 3e5d 5c6e 2320 6469  AND_NAME>]\n# di
-00002800: 7361 626c 655f 636f 6d6d 616e 6473 203d  sable_commands =
-00002810: 205b 3c43 4f4d 4d41 4e44 5f4e 414d 453e   [<COMMAND_NAME>
-00002820: 5d5c 6e60 6060 5c6e 5c6e 2320 4164 7661  ]\n```\n\n# Adva
-00002830: 6e63 6564 2075 7361 6765 5c6e 5c6e 3c21  nced usage\n\n<!
-00002840: 2d2d 5c6e 2323 2041 6476 616e 6365 6420  --\n## Advanced 
-00002850: 436f 6d6d 616e 645c 6e5c 6e44 656c 6669  Command\n\nDelfi
-00002860: 6e6f 2061 6464 7320 6f70 7469 6f6e 616c  no adds optional
-00002870: 2062 6974 7320 6f66 2066 756e 6374 696f   bits of functio
-00002880: 6e61 6c69 7479 206f 6e20 746f 7020 6f66  nality on top of
-00002890: 2043 6c69 636b 2e20 5468 6520 666f 6c6c   Click. The foll
-000028a0: 6f77 696e 6720 6578 616d 706c 6520 6465  owing example de
-000028b0: 6d6f 6e73 7472 6174 6573 2073 6f6d 6520  monstrates some 
-000028c0: 6f66 2074 686f 7365 3a5c 6e5c 6e60 6060  of those:\n\n```
-000028d0: 7079 7468 6f6e 5c6e 2320 636f 6d6d 616e  python\n# comman
-000028e0: 6473 2f5f 5f69 6e69 745f 5f2e 7079 5c6e  ds/__init__.py\n
-000028f0: 5c6e 696d 706f 7274 2063 6c69 636b 5c6e  \nimport click\n
-00002900: 5c6e 6672 6f6d 2064 656c 6669 6e6f 2e63  \nfrom delfino.c
-00002910: 6f6e 7465 7874 7320 696d 706f 7274 2070  ontexts import p
-00002920: 6173 735f 6170 705f 636f 6e74 6578 742c  ass_app_context,
-00002930: 2041 7070 436f 6e74 6578 745c 6e66 726f   AppContext\nfro
-00002940: 6d20 6465 6c66 696e 6f2e 7661 6c69 6461  m delfino.valida
-00002950: 7469 6f6e 2069 6d70 6f72 7420 6173 7365  tion import asse
-00002960: 7274 5f70 6970 5f70 6163 6b61 6765 5f69  rt_pip_package_i
-00002970: 6e73 7461 6c6c 6564 2c20 7079 7072 6f6a  nstalled, pyproj
-00002980: 6563 745f 746f 6d6c 5f6b 6579 5f6d 6973  ect_toml_key_mis
-00002990: 7369 6e67 5c6e 5c6e 4063 6c69 636b 2e63  sing\n\n@click.c
-000029a0: 6f6d 6d61 6e64 2829 5c6e 2320 5468 6520  ommand()\n# The 
-000029b0: 6070 6173 735f 6170 705f 636f 6e74 6578  `pass_app_contex
-000029c0: 7460 2064 6563 6f72 6174 6f72 2061 6464  t` decorator add
-000029d0: 7320 6041 7070 436f 6e74 6578 7460 2061  s `AppContext` a
-000029e0: 7320 7468 6520 6669 7273 7420 7061 7261  s the first para
-000029f0: 6d65 7465 722e 5c6e 4070 6173 735f 6170  meter.\n@pass_ap
-00002a00: 705f 636f 6e74 6578 745c 6e64 6566 2063  p_context\ndef c
-00002a10: 6f6d 6d61 6e64 5f74 6573 7428 6170 705f  ommand_test(app_
-00002a20: 636f 6e74 6578 743a 2041 7070 436f 6e74  context: AppCont
-00002a30: 6578 7429 3a5c 6e20 2020 2222 2254 6573  ext):\n   """Tes
-00002a40: 7473 2063 6f6d 6d61 6e64 7320 706c 6163  ts commands plac
-00002a50: 6564 2069 6e20 7468 6520 6063 6f6d 6d61  ed in the `comma
-00002a60: 6e64 7360 2066 6f6c 6465 7220 6172 6520  nds` folder are 
-00002a70: 6c6f 6164 6564 2e22 2222 5c6e 2020 2023  loaded."""\n   #
-00002a80: 2054 6573 7420 6f70 7469 6f6e 616c 2064   Test optional d
-00002a90: 6570 656e 6465 6e63 6965 732e 2041 6e79  ependencies. Any
-00002aa0: 2066 6169 6c69 6e67 2061 7373 6572 7469   failing asserti
-00002ab0: 6f6e 2077 696c 6c20 6265 2070 7269 6e74  on will be print
-00002ac0: 6564 2061 733a 5c6e 2020 2023 2043 6f6d  ed as:\n   # Com
-00002ad0: 6d61 6e64 205c 273c 4e41 4d45 3e5c 2720  mand \'<NAME>\' 
-00002ae0: 6973 206d 6973 636f 6e66 6967 7572 6564  is misconfigured
-00002af0: 2e20 3c41 5353 4552 5449 4f4e 2045 5252  . <ASSERTION ERR
-00002b00: 4f52 204d 4553 5341 4745 3e5c 6e20 2020  OR MESSAGE>\n   
-00002b10: 6173 7365 7274 5f70 6970 5f70 6163 6b61  assert_pip_packa
-00002b20: 6765 5f69 6e73 7461 6c6c 6564 2822 6465  ge_installed("de
-00002b30: 6c66 696e 6f22 295c 6e5c 6e20 2020 2320  lfino")\n\n   # 
-00002b40: 4170 7043 6f6e 7465 7874 2063 6f6e 7461  AppContext conta
-00002b50: 696e 2061 2070 6172 7365 6420 6070 7970  in a parsed `pyp
-00002b60: 726f 6a65 6374 2e74 6f6d 6c60 2066 696c  roject.toml` fil
-00002b70: 652e 5c6e 2020 2023 2043 6f6d 6d61 6e64  e.\n   # Command
-00002b80: 7320 6361 6e20 6164 6420 7468 6569 7220  s can add their 
-00002b90: 636f 6e66 6967 2075 6e64 6572 2060 5b74  config under `[t
-00002ba0: 6f6f 6c2e 6465 6c66 696e 6f2e 636f 6d6d  ool.delfino.comm
-00002bb0: 616e 6473 2e3c 434f 4d4d 414e 445f 4e41  ands.<COMMAND_NA
-00002bc0: 4d45 3e5d 602e 5c6e 2020 2061 7373 6572  ME>]`.\n   asser
-00002bd0: 7420 2263 6f6d 6d61 6e64 5f74 6573 7422  t "command_test"
-00002be0: 2069 6e20 6170 705f 636f 6e74 6578 742e   in app_context.
-00002bf0: 7079 7072 6f6a 6563 745f 746f 6d6c 2e74  pyproject_toml.t
-00002c00: 6f6f 6c2e 6465 6c66 696e 6f2e 636f 6d6d  ool.delfino.comm
-00002c10: 616e 6473 2c20 5c5c 5c6e 2020 2020 2020  ands, \\\n      
-00002c20: 2070 7970 726f 6a65 6374 5f74 6f6d 6c5f   pyproject_toml_
-00002c30: 6b65 795f 6d69 7373 696e 6728 2274 6f6f  key_missing("too
-00002c40: 6c2e 6465 6c66 696e 6f2e 636f 6d6d 616e  l.delfino.comman
-00002c50: 6473 2e63 6f6d 6d61 6e64 5f74 6573 7422  ds.command_test"
-00002c60: 295c 6e5c 6e20 2020 7072 696e 7428 6170  )\n\n   print(ap
-00002c70: 705f 636f 6e74 6578 742e 7079 7072 6f6a  p_context.pyproj
-00002c80: 6563 745f 746f 6d6c 2e74 6f6f 6c2e 6465  ect_toml.tool.de
-00002c90: 6c66 696e 6f2e 636f 6d6d 616e 6473 5b22  lfino.commands["
-00002ca0: 636f 6d6d 616e 642d 7465 7374 225d 295c  command-test"])\
-00002cb0: 6e60 6060 5c6e 2d2d 3e5c 6e5c 6e23 2320  n```\n-->\n\n## 
-00002cc0: 4175 746f 2d63 6f6d 706c 6574 696f 6e5c  Auto-completion\
-00002cd0: 6e5c 6e59 6f75 2063 616e 2065 6974 6865  n\nYou can eithe
-00002ce0: 7220 6174 7465 6d70 7420 746f 2069 6e73  r attempt to ins
-00002cf0: 7461 6c6c 2063 6f6d 706c 6574 696f 6e73  tall completions
-00002d00: 2061 7574 6f6d 6174 6963 616c 6c79 2077   automatically w
-00002d10: 6974 683a 5c6e 5c6e 6060 6073 6865 6c6c  ith:\n\n```shell
-00002d20: 2073 6372 6970 745c 6e64 656c 6669 6e6f   script\ndelfino
-00002d30: 202d 2d69 6e73 7461 6c6c 2d63 6f6d 706c   --install-compl
-00002d40: 6574 696f 6e5c 6e60 6060 5c6e 5c6e 6f72  etion\n```\n\nor
-00002d50: 2067 656e 6572 6174 6520 6974 2077 6974   generate it wit
-00002d60: 683a 5c6e 5c6e 6060 6073 6865 6c6c 2073  h:\n\n```shell s
-00002d70: 6372 6970 745c 6e64 656c 6669 6e6f 202d  cript\ndelfino -
-00002d80: 2d73 686f 772d 636f 6d70 6c65 7469 6f6e  -show-completion
-00002d90: 5c6e 6060 605c 6e5c 6e61 6e64 206d 616e  \n```\n\nand man
-00002da0: 7561 6c6c 7920 7075 7420 6974 2069 6e20  ually put it in 
-00002db0: 7468 6520 7265 6c65 7661 6e74 2052 4320  the relevant RC 
-00002dc0: 6669 6c65 2e5c 6e5c 6e54 6865 2061 7574  file.\n\nThe aut
-00002dd0: 6f2d 636f 6d70 6c65 7469 6f6e 2069 6d70  o-completion imp
-00002de0: 6c65 6d65 6e74 6174 696f 6e20 6973 2064  lementation is d
-00002df0: 796e 616d 6963 2073 6f20 7468 6174 2065  ynamic so that e
-00002e00: 7665 7279 2074 696d 6520 6974 2069 7320  very time it is 
-00002e10: 696e 766f 6b65 642c 2069 7420 7573 6573  invoked, it uses
-00002e20: 2074 6865 2063 7572 7265 6e74 2070 726f   the current pro
-00002e30: 6a65 6374 2e20 4561 6368 2070 726f 6a65  ject. Each proje
-00002e40: 6374 2063 616e 2068 6176 6520 6469 6666  ct can have diff
-00002e50: 6572 656e 7420 636f 6d6d 616e 6473 206f  erent commands o
-00002e60: 7220 6469 7361 626c 6520 6365 7274 6169  r disable certai
-00002e70: 6e20 636f 6d6d 616e 6473 2069 7420 646f  n commands it do
-00002e80: 6573 6e5c 2774 2075 7365 2e20 416e 6420  esn\'t use. And 
-00002e90: 6479 6e61 6d69 6320 6175 746f 2d63 6f6d  dynamic auto-com
-00002ea0: 706c 6574 696f 6e20 6d61 6b65 7320 7375  pletion makes su
-00002eb0: 7265 206f 6e6c 7920 7468 6520 6375 7272  re only the curr
-00002ec0: 656e 746c 7920 6176 6169 6c61 626c 6520  ently available 
-00002ed0: 636f 6d6d 616e 6473 2077 696c 6c20 6265  commands will be
-00002ee0: 2073 7567 6765 7374 6564 2e5c 6e5c 6e54   suggested.\n\nT
-00002ef0: 6865 2064 6f77 6e73 6964 6520 6f66 2074  he downside of t
-00002f00: 6869 7320 6170 7072 6f61 6368 2069 7320  his approach is 
-00002f10: 7468 6174 2065 7661 6c75 6174 696e 6720  that evaluating 
-00002f20: 7768 6174 2069 7320 6176 6169 6c61 626c  what is availabl
-00002f30: 6520 6561 6368 2074 696d 6520 6973 2073  e each time is s
-00002f40: 6c6f 7765 7220 7468 616e 2061 2073 7461  lower than a sta
-00002f50: 7469 6320 6c69 7374 206f 6620 636f 6d6d  tic list of comm
-00002f60: 616e 6473 2e5c 6e5c 6e23 2320 5275 6e6e  ands.\n\n## Runn
-00002f70: 696e 6720 6578 7465 726e 616c 2070 726f  ing external pro
-00002f80: 6772 616d 735c 6e5c 6e49 7420 6973 2075  grams\n\nIt is u
-00002f90: 7020 746f 2079 6f75 2068 6f77 2079 6f75  p to you how you
-00002fa0: 2077 616e 7420 746f 2065 7865 6375 7465   want to execute
-00002fb0: 2065 7874 6572 6e61 6c20 7072 6f63 6573   external proces
-00002fc0: 7365 7320 6173 2070 6172 7420 6f66 2063  ses as part of c
-00002fd0: 6f6d 6d61 6e64 7320 2869 6620 796f 7520  ommands (if you 
-00002fe0: 6e65 6564 2074 6f20 6174 2061 6c6c 292e  need to at all).
-00002ff0: 2041 2063 6f6d 6d6f 6e20 7761 7920 696e   A common way in
-00003000: 2050 7974 686f 6e20 6973 2074 6f20 7573   Python is to us
-00003010: 6520 6073 7562 7072 6f63 6573 732e 7275  e `subprocess.ru
-00003020: 6e60 2e20 4465 6c66 696e 6f20 636f 6d65  n`. Delfino come
-00003030: 7320 7769 7468 2069 7473 206f 776e 205b  s with its own [
-00003040: 6072 756e 6020 696d 706c 656d 656e 7461  `run` implementa
-00003050: 7469 6f6e 5d28 6874 7470 733a 2f2f 6769  tion](https://gi
-00003060: 7468 7562 2e63 6f6d 2f72 6164 656b 6c61  thub.com/radekla
-00003070: 742f 6465 6c66 696e 6f2f 626c 6f62 2f6d  t/delfino/blob/m
-00003080: 6169 6e2f 7372 632f 6465 6c66 696e 6f2f  ain/src/delfino/
-00003090: 6578 6563 7574 696f 6e2e 7079 234c 3934  execution.py#L94
-000030a0: 292c 2077 6869 6368 2077 7261 7073 2061  ), which wraps a
-000030b0: 6e64 2073 696d 706c 6966 6965 7320 6073  nd simplifies `s
-000030c0: 7562 7072 6f63 6573 732e 7275 6e60 2066  ubprocess.run` f
-000030d0: 6f72 2074 6865 206d 6f73 7420 636f 6d6d  or the most comm
-000030e0: 6f6e 2075 7365 2063 6173 6573 3a5c 6e5c  on use cases:\n\
-000030f0: 6e2d 204e 6f72 6d61 6c69 7a69 6e67 2060  n- Normalizing `
-00003100: 7375 6270 726f 6365 7373 2e72 756e 6020  subprocess.run` 
-00003110: 6172 6775 6d65 6e74 7320 2d20 796f 7520  arguments - you 
-00003120: 6361 6e20 7061 7373 2069 6e20 6569 7468  can pass in eith
-00003130: 6572 2061 2073 7472 696e 6720 6f72 2061  er a string or a
-00003140: 206c 6973 742e 2045 6974 6865 7220 7761   list. Either wa
-00003150: 792c 2060 7375 6270 726f 6365 7373 2e72  y, `subprocess.r
-00003160: 756e 6020 7769 6c6c 2062 6520 6578 6563  un` will be exec
-00003170: 7574 6564 2063 6f72 7265 6374 6c79 2e5c  uted correctly.\
-00003180: 6e2d 2048 616e 646c 696e 6720 6572 726f  n- Handling erro
-00003190: 7273 2066 726f 6d20 7468 6520 6578 6563  rs from the exec
-000031a0: 7574 696f 6e20 7669 6120 7468 6520 606f  ution via the `o
-000031b0: 6e5f 6572 726f 7260 2061 7267 756d 656e  n_error` argumen
-000031c0: 742e 2047 6976 696e 6720 7468 6520 6f70  t. Giving the op
-000031d0: 7469 6f6e 2074 6f20 6569 7468 6572 2069  tion to either i
-000031e0: 676e 6f72 6520 7468 6520 6572 726f 7273  gnore the errors
-000031f0: 2061 6e64 2063 6f6e 7469 6e75 6520 2860   and continue (`
-00003200: 5041 5353 6029 2c20 6e6f 7420 636f 6e74  PASS`), not cont
-00003210: 696e 7565 2061 6e64 2063 6c65 616e 2065  inue and clean e
-00003220: 7869 7420 2860 4558 4954 6029 206f 7220  xit (`EXIT`) or 
-00003230: 6e6f 7420 636f 6e74 696e 7565 2061 6e64  not continue and
-00003240: 2061 626f 7274 2077 6974 6820 6572 726f   abort with erro
-00003250: 7220 636f 6465 2028 6041 424f 5254 6029  r code (`ABORT`)
-00003260: 2e5c 6e2d 2053 6574 7469 6e67 2065 6e76  .\n- Setting env
-00003270: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00003280: 6573 2e5c 6e2d 204c 6f67 6769 6e67 2077  es.\n- Logging w
-00003290: 6861 7420 6973 2062 6569 6e67 2065 7865  hat is being exe
-000032a0: 6375 7465 6420 696e 2074 6865 2064 6562  cuted in the deb
-000032b0: 7567 206c 6576 656c 2e5c 6e5c 6e45 7861  ug level.\n\nExa
-000032c0: 6d70 6c65 3a5c 6e5c 6e60 6060 7079 7468  mple:\n\n```pyth
-000032d0: 6f6e 5c6e 2320 636f 6d6d 616e 6473 2f5f  on\n# commands/_
-000032e0: 5f69 6e69 745f 5f2e 7079 5c6e 5c6e 696d  _init__.py\n\nim
-000032f0: 706f 7274 2063 6c69 636b 5c6e 6672 6f6d  port click\nfrom
-00003300: 2064 656c 6669 6e6f 2e65 7865 6375 7469   delfino.executi
-00003310: 6f6e 2069 6d70 6f72 7420 7275 6e2c 204f  on import run, O
-00003320: 6e45 7272 6f72 5c6e 5c6e 4063 6c69 636b  nError\n\n@click
-00003330: 2e63 6f6d 6d61 6e64 2829 5c6e 6465 6620  .command()\ndef 
-00003340: 7465 7374 2829 3a5c 6e20 2020 2072 756e  test():\n    run
-00003350: 2822 7079 7465 7374 2074 6573 7473 222c  ("pytest tests",
-00003360: 206f 6e5f 6572 726f 723d 4f6e 4572 726f   on_error=OnErro
-00003370: 722e 4142 4f52 5429 5c6e 6060 605c 6e5c  r.ABORT)\n```\n\
-00003380: 6e23 2320 4f70 7469 6f6e 616c 2064 6570  n## Optional dep
-00003390: 656e 6465 6e63 6965 735c 6e5c 6e49 6620  endencies\n\nIf 
-000033a0: 796f 7520 7075 7420 7365 7665 7261 6c20  you put several 
-000033b0: 636f 6d6d 616e 6473 2069 6e74 6f20 6f6e  commands into on
-000033c0: 6520 5b70 6c75 6769 6e5d 2823 706c 7567  e [plugin](#plug
-000033d0: 696e 7329 2c20 796f 7520 6361 6e20 6d61  ins), you can ma
-000033e0: 6b65 2073 6f6d 6520 6465 7065 6e64 656e  ke some dependen
-000033f0: 6369 6573 206f 6620 736f 6d65 2063 6f6d  cies of some com
-00003400: 6d61 6e64 7320 5b6f 7074 696f 6e61 6c5d  mands [optional]
-00003410: 2868 7474 7073 3a2f 2f70 7974 686f 6e2d  (https://python-
-00003420: 706f 6574 7279 2e6f 7267 2f64 6f63 732f  poetry.org/docs/
-00003430: 7079 7072 6f6a 6563 7423 6578 7472 6173  pyproject#extras
-00003440: 292e 2054 6869 7320 6973 2075 7365 6675  ). This is usefu
-00003450: 6c20 7768 656e 2061 2063 6f6d 6d61 6e64  l when a command
-00003460: 2069 7320 6e6f 7420 616c 7761 7973 2075   is not always u
-00003470: 7365 642c 2061 6e64 2079 6f75 2064 6f6e  sed, and you don
-00003480: 5c27 7420 7761 6e74 2074 6f20 696e 7374  \'t want to inst
-00003490: 616c 6c20 756e 6e65 6365 7373 6172 7920  all unnecessary 
-000034a0: 6465 7065 6e64 656e 6369 6573 2e20 496e  dependencies. In
-000034b0: 7374 6561 642c 2079 6f75 2063 616e 2063  stead, you can c
-000034c0: 6865 636b 2069 6620 6120 6465 7065 6e64  heck if a depend
-000034d0: 656e 6379 2069 7320 696e 7374 616c 6c65  ency is installe
-000034e0: 6420 6f6e 6c79 2077 6865 6e20 7468 6520  d only when the 
-000034f0: 636f 6d6d 616e 6420 6973 2065 7865 6375  command is execu
-00003500: 7465 6420 7769 7468 2060 6465 6c66 696e  ted with `delfin
-00003510: 6f2e 7661 6c69 6461 7469 6f6e 2e61 7373  o.validation.ass
-00003520: 6572 745f 7069 705f 7061 636b 6167 655f  ert_pip_package_
-00003530: 696e 7374 616c 6c65 6460 3a5c 6e5c 6e60  installed`:\n\n`
-00003540: 6060 7079 7468 6f6e 5c6e 2320 636f 6d6d  ``python\n# comm
-00003550: 616e 6473 2f5f 5f69 6e69 745f 5f2e 7079  ands/__init__.py
-00003560: 5c6e 5c6e 696d 706f 7274 2063 6c69 636b  \n\nimport click
-00003570: 5c6e 6672 6f6d 2064 656c 6669 6e6f 2e76  \nfrom delfino.v
-00003580: 616c 6964 6174 696f 6e20 696d 706f 7274  alidation import
-00003590: 2061 7373 6572 745f 7069 705f 7061 636b   assert_pip_pack
-000035a0: 6167 655f 696e 7374 616c 6c65 645c 6e5c  age_installed\n\
-000035b0: 6e74 7279 3a5c 6e20 2020 2066 726f 6d20  ntry:\n    from 
-000035c0: 6769 7420 696d 706f 7274 2052 6570 6f5c  git import Repo\
-000035d0: 6e65 7863 6570 7420 496d 706f 7274 4572  nexcept ImportEr
-000035e0: 726f 723a 5c6e 2020 2020 7061 7373 5c6e  ror:\n    pass\n
-000035f0: 5c6e 4063 6c69 636b 2e63 6f6d 6d61 6e64  \n@click.command
-00003600: 2829 5c6e 6465 6620 6769 745f 6163 7469  ()\ndef git_acti
-00003610: 7665 5f62 7261 6e63 6828 293a 5c6e 2020  ve_branch():\n  
-00003620: 2020 6173 7365 7274 5f70 6970 5f70 6163    assert_pip_pac
-00003630: 6b61 6765 5f69 6e73 7461 6c6c 6564 2822  kage_installed("
-00003640: 6769 7470 7974 686f 6e22 295c 6e20 2020  gitpython")\n   
-00003650: 2070 7269 6e74 2852 6570 6f28 222e 2229   print(Repo(".")
-00003660: 2e61 6374 6976 655f 6272 616e 6368 295c  .active_branch)\
-00003670: 6e60 6060 5c6e 5c6e 496e 2074 6865 2065  n```\n\nIn the e
-00003680: 7861 6d70 6c65 2061 626f 7665 2c20 6966  xample above, if
-00003690: 2060 6769 7470 7974 686f 6e60 2069 7320   `gitpython` is 
-000036a0: 6e6f 7420 696e 7374 616c 6c65 642c 2064  not installed, d
-000036b0: 656c 6669 6e6f 2077 696c 6c20 7368 6f77  elfino will show
-000036c0: 2074 6865 2063 6f6d 6d61 6e64 2062 7574   the command but
-000036d0: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
-000036e0: 7375 6767 6573 7469 6f6e 2074 6f20 696e  suggestion to in
-000036f0: 7374 616c 6c20 6067 6974 7079 7468 6f6e  stall `gitpython
-00003700: 6020 6f6e 6c79 2077 6865 6e20 7468 6520  ` only when the 
-00003710: 636f 6d6d 616e 6420 6973 2065 7865 6375  command is execu
-00003720: 7465 642e 2059 6f75 2063 616e 2061 6c73  ted. You can als
-00003730: 6f20 6164 6420 6067 6974 5f61 6374 6976  o add `git_activ
-00003740: 655f 6272 616e 6368 6020 696e 746f 205b  e_branch` into [
-00003750: 6064 6973 6162 6c65 5f63 6f6d 6d61 6e64  `disable_command
-00003760: 7360 2063 6f6e 6669 675d 2823 656e 6162  s` config](#enab
-00003770: 6c69 6e67 6469 7361 626c 696e 672d 636f  lingdisabling-co
-00003780: 6d6d 616e 6473 2920 696e 2070 6c61 6365  mmands) in place
-00003790: 7320 7768 6572 6520 796f 7520 646f 6e5c  s where you don\
-000037a0: 2774 2069 6e74 656e 6420 746f 2075 7365  't intend to use
-000037b0: 2069 742e 5c6e 5c6e 5468 6973 2077 6179   it.\n\nThis way
-000037c0: 2079 6f75 2063 616e 2067 7265 6174 6c79   you can greatly
-000037d0: 2072 6564 7563 6520 7468 6520 6e75 6d62   reduce the numb
-000037e0: 6572 206f 6620 6465 7065 6e64 656e 6369  er of dependenci
-000037f0: 6573 2061 2070 6c75 6769 6e20 6272 696e  es a plugin brin
-00003800: 6773 2069 6e74 6f20 6120 7072 6f6a 6563  gs into a projec
-00003810: 7420 7769 7468 6f75 7420 6120 6e65 6564  t without a need
-00003820: 2074 6f20 6861 7665 206d 616e 7920 736d   to have many sm
-00003830: 616c 6c20 706c 7567 696e 732e 5c6e 5c6e  all plugins.\n\n
-00003840: 2323 2050 726f 6a65 6374 2073 6574 7469  ## Project setti
-00003850: 6e67 735c 6e5c 6e59 6f75 2063 616e 2073  ngs\n\nYou can s
-00003860: 746f 7265 2061 6e20 6172 6269 7472 6172  tore an arbitrar
-00003870: 7920 6f62 6a65 6374 2069 6e20 7468 6520  y object in the 
-00003880: 436c 6963 6b20 636f 6e74 6578 7420 6173  Click context as
-00003890: 205b 6063 6c69 636b 2e43 6f6e 7465 7874   [`click.Context
-000038a0: 2e6f 626a 605d 2868 7474 7073 3a2f 2f63  .obj`](https://c
-000038b0: 6c69 636b 2e70 616c 6c65 7473 7072 6f6a  lick.palletsproj
-000038c0: 6563 7473 2e63 6f6d 2f61 7069 2f23 636c  ects.com/api/#cl
-000038d0: 6963 6b2e 436f 6e74 6578 742e 6f62 6a29  ick.Context.obj)
-000038e0: 2e20 4465 6c66 696e 6f20 7574 696c 697a  . Delfino utiliz
-000038f0: 6573 2074 6869 7320 6f62 6a65 6374 2074  es this object t
-00003900: 6f20 7374 6f72 6520 616e 2069 6e73 7461  o store an insta
-00003910: 6e63 6520 6f66 205b 6041 7070 436f 6e74  nce of [`AppCont
-00003920: 6578 7460 5d28 6874 7470 733a 2f2f 6769  ext`](https://gi
-00003930: 7468 7562 2e63 6f6d 2f72 6164 656b 6c61  thub.com/radekla
-00003940: 742f 6465 6c66 696e 6f2f 626c 6f62 2f6d  t/delfino/blob/m
-00003950: 6169 6e2f 7372 632f 6465 6c66 696e 6f2f  ain/src/delfino/
-00003960: 6d6f 6465 6c73 2f61 7070 5f63 6f6e 7465  models/app_conte
-00003970: 7874 2e70 7929 2c20 7768 6963 6820 7072  xt.py), which pr
-00003980: 6f76 6964 6573 2061 6363 6573 7320 746f  ovides access to
-00003990: 2070 726f 6a65 6374 2072 656c 6174 6564   project related
-000039a0: 2069 6e66 6f72 6d61 7469 6f6e 2e20 4966   information. If
-000039b0: 2079 6f75 206e 6565 6420 746f 2c20 796f   you need to, yo
-000039c0: 7520 6361 6e20 7374 696c 6c20 6174 7461  u can still atta
-000039d0: 6368 2061 7262 6974 7261 7279 2061 7474  ch arbitrary att
-000039e0: 7269 6275 7465 7320 746f 2074 6869 7320  ributes to this 
-000039f0: 6f62 6a65 6374 206c 6174 6572 2e5c 6e5c  object later.\n\
-00003a00: 6e59 6f75 2063 616e 2070 6173 7320 7468  nYou can pass th
-00003a10: 6973 206f 626a 6563 7420 746f 2079 6f75  is object to you
-00003a20: 7220 636f 6d6d 616e 6473 2062 7920 6465  r commands by de
-00003a30: 636f 7261 7469 6e67 2074 6865 6d20 7769  corating them wi
-00003a40: 7468 205b 6063 6c69 636b 2e70 6173 735f  th [`click.pass_
-00003a50: 6f62 6a60 5d28 6874 7470 733a 2f2f 636c  obj`](https://cl
-00003a60: 6963 6b2e 7061 6c6c 6574 7370 726f 6a65  ick.palletsproje
-00003a70: 6374 732e 636f 6d2f 6170 692f 2363 6c69  cts.com/api/#cli
-00003a80: 636b 2e70 6173 735f 6f62 6a29 3a5c 6e5c  ck.pass_obj):\n\
-00003a90: 6e60 6060 7079 7468 6f6e 5c6e 2320 636f  n```python\n# co
-00003aa0: 6d6d 616e 6473 2f5f 5f69 6e69 745f 5f2e  mmands/__init__.
-00003ab0: 7079 5c6e 5c6e 696d 706f 7274 2063 6c69  py\n\nimport cli
-00003ac0: 636b 5c6e 6672 6f6d 2064 656c 6669 6e6f  ck\nfrom delfino
-00003ad0: 2e6d 6f64 656c 732e 6170 705f 636f 6e74  .models.app_cont
-00003ae0: 6578 7420 696d 706f 7274 2041 7070 436f  ext import AppCo
-00003af0: 6e74 6578 745c 6e5c 6e40 636c 6963 6b2e  ntext\n\n@click.
-00003b00: 636f 6d6d 616e 6428 295c 6e40 636c 6963  command()\n@clic
-00003b10: 6b2e 7061 7373 5f6f 626a 5c6e 6465 6620  k.pass_obj\ndef 
-00003b20: 7072 696e 745f 6170 705f 7665 7273 696f  print_app_versio
-00003b30: 6e28 6f62 6a3a 2041 7070 436f 6e74 6578  n(obj: AppContex
-00003b40: 7429 3a5c 6e20 2020 2070 7269 6e74 286f  t):\n    print(o
-00003b50: 626a 2e70 7970 726f 6a65 6374 5f74 6f6d  bj.pyproject_tom
-00003b60: 6c2e 746f 6f6c 2e70 6f65 7472 792e 7665  l.tool.poetry.ve
-00003b70: 7273 696f 6e29 5c6e 6060 605c 6e5c 6e23  rsion)\n```\n\n#
-00003b80: 2320 506c 7567 696e 2073 6574 7469 6e67  # Plugin setting
-00003b90: 735c 6e5c 6e50 6c75 6769 6e20 7365 7474  s\n\nPlugin sett
-00003ba0: 696e 6773 2061 7265 2065 7870 6563 7465  ings are expecte
-00003bb0: 6420 746f 206c 6976 6520 696e 2074 6865  d to live in the
-00003bc0: 2060 7079 7072 6f6a 6563 742e 746f 6d6c   `pyproject.toml
-00003bd0: 6020 6669 6c65 2e20 546f 2070 7265 7665  ` file. To preve
-00003be0: 6e74 206e 616d 696e 6720 636f 6e66 6c69  nt naming confli
-00003bf0: 6374 732c 2065 6163 6820 706c 7567 696e  cts, each plugin
-00003c00: 206d 7573 7420 7075 7420 6974 7320 7365   must put its se
-00003c10: 7474 696e 6773 2075 6e64 6572 2060 746f  ttings under `to
-00003c20: 6f6c 2e64 656c 6669 6e6f 2e70 6c75 6769  ol.delfino.plugi
-00003c30: 6e73 2e3c 504c 5547 494e 5f4e 414d 453e  ns.<PLUGIN_NAME>
-00003c40: 602e 2049 7420 616c 736f 2061 6c6c 6f77  `. It also allow
-00003c50: 7320 4465 6c66 696e 6f20 746f 2070 6173  s Delfino to pas
-00003c60: 7320 7468 6573 6520 7365 7474 696e 6773  s these settings
-00003c70: 2064 6972 6563 746c 7920 746f 2063 6f6d   directly to com
-00003c80: 6d61 6e64 7320 6672 6f6d 2074 6865 7365  mands from these
-00003c90: 2070 6c75 6769 6e73 2e5c 6e5c 6e44 656c   plugins.\n\nDel
-00003ca0: 6669 6e6f 206c 6f61 6473 2c20 7061 7273  fino loads, pars
-00003cb0: 6573 2c20 7661 6c69 6461 7465 7320 616e  es, validates an
-00003cc0: 6420 7374 6f72 6573 2070 6c75 6769 6e20  d stores plugin 
-00003cd0: 7365 7474 696e 6773 2069 6e20 5b60 4170  settings in [`Ap
-00003ce0: 7043 6f6e 7465 7874 2e70 6c75 6769 6e5f  pContext.plugin_
-00003cf0: 636f 6e66 6967 605d 2868 7474 7073 3a2f  config`](https:/
-00003d00: 2f67 6974 6875 622e 636f 6d2f 7261 6465  /github.com/rade
-00003d10: 6b6c 6174 2f64 656c 6669 6e6f 2f62 6c6f  klat/delfino/blo
-00003d20: 622f 6d61 696e 2f73 7263 2f64 656c 6669  b/main/src/delfi
-00003d30: 6e6f 2f6d 6f64 656c 732f 6170 705f 636f  no/models/app_co
-00003d40: 6e74 6578 742e 7079 292e 2049 6620 6e6f  ntext.py). If no
-00003d50: 7420 7370 6563 6966 6965 6420 6f74 6865  t specified othe
-00003d60: 7277 6973 6520 2873 6565 2062 656c 6f77  rwise (see below
-00003d70: 292c 2069 7420 7769 6c6c 2062 6520 616e  ), it will be an
-00003d80: 2069 6e73 7461 6e63 6520 6f66 205b 6050   instance of [`P
-00003d90: 6c75 6769 6e43 6f6e 6669 6760 5d28 6874  luginConfig`](ht
-00003da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003db0: 2f72 6164 656b 6c61 742f 6465 6c66 696e  /radeklat/delfin
-00003dc0: 6f2f 626c 6f62 2f6d 6169 6e2f 7372 632f  o/blob/main/src/
-00003dd0: 6465 6c66 696e 6f2f 6d6f 6465 6c73 2f70  delfino/models/p
-00003de0: 7970 726f 6a65 6374 5f74 6f6d 6c2e 7079  yproject_toml.py
-00003df0: 292c 2077 6974 6820 616e 7920 6578 7472  ), with any extr
-00003e00: 6120 6b65 7973 2075 6e76 616c 6964 6174  a keys unvalidat
-00003e10: 6564 2061 6e64 2069 6e20 4a53 4f4e 2d6c  ed and in JSON-l
-00003e20: 696b 6520 5079 7468 6f6e 206f 626a 6563  ike Python objec
-00003e30: 7473 2e5c 6e5c 6e59 6f75 2063 616e 2061  ts.\n\nYou can a
-00003e40: 6464 2061 6464 6974 696f 6e61 6c20 7661  dd additional va
-00003e50: 6c69 6461 7469 6f6e 2074 6f20 796f 7572  lidation to your
-00003e60: 2070 6c75 6769 6e20 7365 7474 696e 6773   plugin settings
-00003e70: 2062 7920 7375 622d 636c 6173 7369 6e67   by sub-classing
-00003e80: 2074 6865 2060 506c 7567 696e 436f 6e66   the `PluginConf
-00003e90: 6967 6020 2c20 6465 6669 6e69 6e67 2065  ig` , defining e
-00003ea0: 7870 6563 7465 6420 6b65 7973 2c20 6465  xpected keys, de
-00003eb0: 6661 756c 7420 7661 6c75 6573 2061 6e64  fault values and
-00003ec0: 2f6f 7220 7661 6c69 6461 7469 6f6e 2e20  /or validation. 
-00003ed0: 4465 6c66 696e 6f20 7574 696c 697a 6573  Delfino utilizes
-00003ee0: 205b 6070 7964 616e 7469 6360 5d28 6874   [`pydantic`](ht
-00003ef0: 7470 733a 2f2f 646f 6373 2e70 7964 616e  tps://docs.pydan
-00003f00: 7469 632e 6465 762f 2920 746f 2063 7265  tic.dev/) to cre
-00003f10: 6174 6520 6461 7461 2063 6c61 7373 6573  ate data classes
-00003f20: 2e5c 6e5c 6e44 656c 6669 6e6f 2061 6c73  .\n\nDelfino als
-00003f30: 6f20 6e65 6564 7320 746f 206b 6e6f 772c  o needs to know,
-00003f40: 2077 6869 6368 2063 6c61 7373 2074 6f20   which class to 
-00003f50: 7573 6520 666f 7220 7468 6520 7661 6c69  use for the vali
-00003f60: 6461 7469 6f6e 2e20 546f 2064 6f20 7468  dation. To do th
-00003f70: 6174 2c20 7377 6974 6368 2074 6f20 6064  at, switch to `d
-00003f80: 656c 6669 6e6f 2e64 6563 6f72 6174 6f72  elfino.decorator
-00003f90: 732e 7061 7373 5f61 7070 5f63 6f6e 7465  s.pass_app_conte
-00003fa0: 7874 6020 696e 7374 6561 6420 6f66 205b  xt` instead of [
-00003fb0: 6063 6c69 636b 2e70 6173 735f 6f62 6a60  `click.pass_obj`
-00003fc0: 5d28 6874 7470 733a 2f2f 636c 6963 6b2e  ](https://click.
-00003fd0: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
-00003fe0: 636f 6d2f 6170 692f 2363 6c69 636b 2e70  com/api/#click.p
-00003ff0: 6173 735f 6f62 6a29 3a5c 6e5c 6e60 6060  ass_obj):\n\n```
-00004000: 746f 6d6c 5c6e 2320 7079 7072 6f6a 6563  toml\n# pyprojec
-00004010: 742e 746f 6d6c 5c6e 5c6e 5b74 6f6f 6c2e  t.toml\n\n[tool.
-00004020: 6465 6c66 696e 6f2e 706c 7567 696e 732e  delfino.plugins.
-00004030: 6465 6c66 696e 6f5f 6c6f 6769 6e5f 706c  delfino_login_pl
-00004040: 7567 696e 5d5c 6e75 7365 726e 616d 6520  ugin]\nusername 
-00004050: 3d20 2275 7365 7222 5c6e 6060 605c 6e5c  = "user"\n```\n\
-00004060: 6e60 6060 7079 7468 6f6e 5c6e 2320 636f  n```python\n# co
-00004070: 6d6d 616e 6473 2f5f 5f69 6e69 745f 5f2e  mmands/__init__.
-00004080: 7079 5c6e 5c6e 696d 706f 7274 2063 6c69  py\n\nimport cli
-00004090: 636b 5c6e 6672 6f6d 2064 656c 6669 6e6f  ck\nfrom delfino
-000040a0: 2e6d 6f64 656c 732e 7079 7072 6f6a 6563  .models.pyprojec
-000040b0: 745f 746f 6d6c 2069 6d70 6f72 7420 506c  t_toml import Pl
-000040c0: 7567 696e 436f 6e66 6967 5c6e 6672 6f6d  uginConfig\nfrom
-000040d0: 2064 656c 6669 6e6f 2e6d 6f64 656c 732e   delfino.models.
-000040e0: 6170 705f 636f 6e74 6578 7420 696d 706f  app_context impo
-000040f0: 7274 2041 7070 436f 6e74 6578 745c 6e66  rt AppContext\nf
-00004100: 726f 6d20 6465 6c66 696e 6f2e 6465 636f  rom delfino.deco
-00004110: 7261 746f 7273 2069 6d70 6f72 7420 7061  rators import pa
-00004120: 7373 5f61 7070 5f63 6f6e 7465 7874 5c6e  ss_app_context\n
-00004130: 5c6e 5c6e 636c 6173 7320 4c6f 6769 6e50  \n\nclass LoginP
-00004140: 6c75 6769 6e43 6f6e 6669 6728 506c 7567  luginConfig(Plug
-00004150: 696e 436f 6e66 6967 293a 5c6e 2020 2020  inConfig):\n    
-00004160: 6c6f 6769 6e3a 2073 7472 5c6e 5c6e 5c6e  login: str\n\n\n
-00004170: 4063 6c69 636b 2e63 6f6d 6d61 6e64 2829  @click.command()
-00004180: 5c6e 4070 6173 735f 6170 705f 636f 6e74  \n@pass_app_cont
-00004190: 6578 7428 4c6f 6769 6e50 6c75 6769 6e43  ext(LoginPluginC
-000041a0: 6f6e 6669 6729 5c6e 6465 6620 6c6f 6769  onfig)\ndef logi
-000041b0: 6e28 6170 705f 636f 6e74 6578 743a 2041  n(app_context: A
-000041c0: 7070 436f 6e74 6578 745b 4c6f 6769 6e50  ppContext[LoginP
-000041d0: 6c75 6769 6e43 6f6e 6669 675d 293a 5c6e  luginConfig]):\n
-000041e0: 2020 2020 7072 696e 7428 6170 705f 636f      print(app_co
-000041f0: 6e74 6578 742e 706c 7567 696e 5f63 6f6e  ntext.plugin_con
-00004200: 6669 672e 6c6f 6769 6e29 5c6e 6060 605c  fig.login)\n```\
-00004210: 6e5c 6e54 6865 2060 4170 7043 6f6e 7465  n\nThe `AppConte
-00004220: 7874 6020 636c 6173 7320 6973 2067 656e  xt` class is gen
-00004230: 6572 6963 2e20 4465 6669 6e69 6e67 2074  eric. Defining t
-00004240: 6865 2060 506c 7567 696e 436f 6e66 6967  he `PluginConfig
-00004250: 5479 7065 6020 2873 7563 6820 6173 2060  Type` (such as `
-00004260: 4170 7043 6f6e 7465 7874 5b4c 6f67 696e  AppContext[Login
-00004270: 506c 7567 696e 436f 6e66 6967 5d60 2069  PluginConfig]` i
-00004280: 6e20 7468 6520 6578 616d 706c 6520 6162  n the example ab
-00004290: 6f76 6529 2065 6e61 626c 6573 2069 6e74  ove) enables int
-000042a0: 726f 7370 6563 7469 6f6e 2061 6e64 2074  rospection and t
-000042b0: 7970 6520 6368 6563 6b73 2e5c 6e5c 6e23  ype checks.\n\n#
-000042c0: 2320 5072 6f6a 6563 7420 7370 6563 6966  # Project specif
-000042d0: 6963 206f 7665 7272 6964 6573 5c6e 5c6e  ic overrides\n\n
-000042e0: 4974 2069 7320 6c69 6b65 6c79 2079 6f75  It is likely you
-000042f0: 7220 7072 6f6a 6563 7473 2077 696c 6c20  r projects will 
-00004300: 7265 7175 6972 6520 736c 6967 6874 2064  require slight d
-00004310: 6976 6572 6765 6e63 6520 746f 2074 6865  ivergence to the
-00004320: 2064 6566 6175 6c74 7320 796f 7520 656e   defaults you en
-00004330: 636f 6465 2069 6e20 796f 7572 2073 6372  code in your scr
-00004340: 6970 7473 2e20 5468 6520 666f 6c6c 6f77  ipts. The follow
-00004350: 696e 6720 7365 6374 696f 6e73 2063 6f76  ing sections cov
-00004360: 6572 2074 6865 206d 6f73 7420 636f 6d6d  er the most comm
-00004370: 6f6e 2075 7365 2063 6173 6573 2e5c 6e5c  on use cases.\n\
-00004380: 6e23 2323 2050 6173 732d 7468 726f 7567  n### Pass-throug
-00004390: 6820 6172 6775 6d65 6e74 735c 6e5c 6e59  h arguments\n\nY
-000043a0: 6f75 2063 616e 2070 6173 7320 6164 6469  ou can pass addi
-000043b0: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
-000043c0: 2074 6f20 646f 776e 7374 7265 616d 2074   to downstream t
-000043d0: 6f6f 6c73 2062 7920 6465 636f 7261 7469  ools by decorati
-000043e0: 6e67 2063 6f6d 6d61 6e64 7320 7769 7468  ng commands with
-000043f0: 2074 6865 205b 6064 6563 6f72 6174 6f72   the [`decorator
-00004400: 732e 7061 7373 5f61 7267 7360 5d28 6874  s.pass_args`](ht
-00004410: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004420: 2f72 6164 656b 6c61 742f 6465 6c66 696e  /radeklat/delfin
-00004430: 6f2f 626c 6f62 2f6d 6169 6e2f 7372 632f  o/blob/main/src/
-00004440: 6465 6c66 696e 6f2f 6465 636f 7261 746f  delfino/decorato
-00004450: 7273 2f70 6173 735f 6172 6773 2e70 7929  rs/pass_args.py)
-00004460: 2064 6563 6f72 6174 6f72 3a5c 6e5c 6e60   decorator:\n\n`
-00004470: 6060 7079 7468 6f6e 5c6e 2320 636f 6d6d  ``python\n# comm
-00004480: 616e 6473 2f5f 5f69 6e69 745f 5f2e 7079  ands/__init__.py
-00004490: 5c6e 5c6e 6672 6f6d 2074 7970 696e 6720  \n\nfrom typing 
-000044a0: 696d 706f 7274 2054 7570 6c65 5c6e 5c6e  import Tuple\n\n
-000044b0: 696d 706f 7274 2063 6c69 636b 5c6e 6672  import click\nfr
-000044c0: 6f6d 2064 656c 6669 6e6f 2e64 6563 6f72  om delfino.decor
-000044d0: 6174 6f72 7320 696d 706f 7274 2070 6173  ators import pas
-000044e0: 735f 6172 6773 5c6e 6672 6f6d 2064 656c  s_args\nfrom del
-000044f0: 6669 6e6f 2e65 7865 6375 7469 6f6e 2069  fino.execution i
-00004500: 6d70 6f72 7420 7275 6e2c 204f 6e45 7272  mport run, OnErr
-00004510: 6f72 5c6e 5c6e 4063 6c69 636b 2e63 6f6d  or\n\n@click.com
-00004520: 6d61 6e64 2829 5c6e 4070 6173 735f 6172  mand()\n@pass_ar
-00004530: 6773 5c6e 6465 6620 7465 7374 2870 6173  gs\ndef test(pas
-00004540: 7365 645f 6172 6773 3a20 5475 706c 655b  sed_args: Tuple[
-00004550: 7374 722c 202e 2e2e 5d29 3a5c 6e20 2020  str, ...]):\n   
-00004560: 2072 756e 285b 2270 7974 6573 7422 2c20   run(["pytest", 
-00004570: 2274 6573 7473 222c 202a 7061 7373 6564  "tests", *passed
-00004580: 5f61 7267 735d 2c20 6f6e 5f65 7272 6f72  _args], on_error
-00004590: 3d4f 6e45 7272 6f72 2e41 424f 5254 295c  =OnError.ABORT)\
-000045a0: 6e60 6060 5c6e 5c6e 5468 656e 2061 6464  n```\n\nThen add
-000045b0: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
-000045c0: 7320 6361 6e20 6265 2070 6173 7365 6420  s can be passed 
-000045d0: 6569 7468 6572 2076 6961 2063 6f6d 6d61  either via comma
-000045e0: 6e64 206c 696e 6520 6166 7465 7220 602d  nd line after `-
-000045f0: 2d60 3a5c 6e5c 6e60 6060 7368 656c 6c20  -`:\n\n```shell 
-00004600: 7363 7269 7074 5c6e 6465 6c66 696e 6f20  script\ndelfino 
-00004610: 7465 7374 202d 2d20 2d2d 6361 7074 7572  test -- --captur
-00004620: 653d 6e6f 5c6e 6060 605c 6e5c 6e4f 7220  e=no\n```\n\nOr 
-00004630: 7669 6120 636f 6e66 6967 7572 6174 696f  via configuratio
-00004640: 6e20 696e 2074 6865 2060 7079 7072 6f6a  n in the `pyproj
-00004650: 6563 742e 746f 6d6c 6020 6669 6c65 3a5c  ect.toml` file:\
-00004660: 6e5c 6e60 6060 746f 6d6c 5c6e 5b74 6f6f  n\n```toml\n[too
-00004670: 6c2e 6465 6c66 696e 6f2e 706c 7567 696e  l.delfino.plugin
-00004680: 732e 3c50 4c55 4749 4e3e 2e74 6573 745d  s.<PLUGIN>.test]
-00004690: 5c6e 7061 7373 5f61 7267 7320 3d20 5b5c  \npass_args = [\
-000046a0: 272d 2d63 6170 7475 7265 3d6e 6f5c 275d  '--capture=no\']
-000046b0: 5c6e 6060 605c 6e5c 6e45 6974 6865 7220  \n```\n\nEither 
-000046c0: 7761 792c 2062 6f74 6820 7769 6c6c 2072  way, both will r
-000046d0: 6573 756c 7420 696e 2065 7865 6375 7469  esult in executi
-000046e0: 6e67 2060 7079 7465 7374 2074 6573 7473  ng `pytest tests
-000046f0: 202d 2d63 6170 7475 7265 3d6e 6f60 2e5c   --capture=no`.\
-00004700: 6e5c 6e23 2323 2046 696c 6573 206f 7665  n\n### Files ove
-00004710: 7272 6964 655c 6e5c 6e59 6f75 2063 616e  rride\n\nYou can
-00004720: 206f 7665 7272 6964 6520 6669 6c65 7320   override files 
-00004730: 7061 7373 6564 2074 6f20 646f 776e 7374  passed to downst
-00004740: 7265 616d 2074 6f6f 6c73 2062 7920 6465  ream tools by de
-00004750: 636f 7261 7469 6e67 2063 6f6d 6d61 6e64  corating command
-00004760: 7320 7769 7468 2074 6865 205b 6064 6563  s with the [`dec
-00004770: 6f72 6174 6f72 732e 6669 6c65 735f 666f  orators.files_fo
-00004780: 6c64 6572 735f 6f70 7469 6f6e 605d 2868  lders_option`](h
-00004790: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000047a0: 6d2f 7261 6465 6b6c 6174 2f64 656c 6669  m/radeklat/delfi
-000047b0: 6e6f 2f62 6c6f 622f 6d61 696e 2f73 7263  no/blob/main/src
-000047c0: 2f64 656c 6669 6e6f 2f64 6563 6f72 6174  /delfino/decorat
-000047d0: 6f72 732f 6669 6c65 735f 666f 6c64 6572  ors/files_folder
-000047e0: 732e 7079 2920 6465 636f 7261 746f 723a  s.py) decorator:
-000047f0: 5c6e 5c6e 6060 6070 7974 686f 6e5c 6e23  \n\n```python\n#
-00004800: 2063 6f6d 6d61 6e64 732f 5f5f 696e 6974   commands/__init
-00004810: 5f5f 2e70 795c 6e5c 6e66 726f 6d20 7479  __.py\n\nfrom ty
-00004820: 7069 6e67 2069 6d70 6f72 7420 5475 706c  ping import Tupl
-00004830: 655c 6e5c 6e69 6d70 6f72 7420 636c 6963  e\n\nimport clic
-00004840: 6b5c 6e66 726f 6d20 6465 6c66 696e 6f2e  k\nfrom delfino.
-00004850: 6465 636f 7261 746f 7273 2069 6d70 6f72  decorators impor
-00004860: 7420 6669 6c65 735f 666f 6c64 6572 735f  t files_folders_
-00004870: 6f70 7469 6f6e 5c6e 6672 6f6d 2064 656c  option\nfrom del
-00004880: 6669 6e6f 2e65 7865 6375 7469 6f6e 2069  fino.execution i
-00004890: 6d70 6f72 7420 7275 6e2c 204f 6e45 7272  mport run, OnErr
-000048a0: 6f72 5c6e 5c6e 4063 6c69 636b 2e63 6f6d  or\n\n@click.com
-000048b0: 6d61 6e64 2829 5c6e 4066 696c 6573 5f66  mand()\n@files_f
-000048c0: 6f6c 6465 7273 5f6f 7074 696f 6e5c 6e64  olders_option\nd
-000048d0: 6566 2074 6573 7428 6669 6c65 735f 666f  ef test(files_fo
-000048e0: 6c64 6572 733a 2054 7570 6c65 5b73 7472  lders: Tuple[str
-000048f0: 2c20 2e2e 2e5d 293a 5c6e 2020 2020 6966  , ...]):\n    if
-00004900: 206e 6f74 2066 696c 6573 5f66 6f6c 6465   not files_folde
-00004910: 7273 3a5c 6e20 2020 2020 2020 2066 696c  rs:\n        fil
-00004920: 6573 5f66 6f6c 6465 7273 203d 2028 2274  es_folders = ("t
-00004930: 6573 7473 2f75 6e69 7422 2c20 2274 6573  ests/unit", "tes
-00004940: 7473 2f69 6e74 6567 7261 7469 6f6e 2229  ts/integration")
-00004950: 5c6e 2020 2020 7275 6e28 5b22 7079 7465  \n    run(["pyte
-00004960: 7374 222c 202a 6669 6c65 735f 666f 6c64  st", *files_fold
-00004970: 6572 735d 2c20 6f6e 5f65 7272 6f72 3d4f  ers], on_error=O
-00004980: 6e45 7272 6f72 2e41 424f 5254 295c 6e60  nError.ABORT)\n`
-00004990: 6060 5c6e 5c6e 5468 656e 2074 6865 2064  ``\n\nThen the d
-000049a0: 6566 6175 6c74 2060 2274 6573 7473 2f75  efault `"tests/u
-000049b0: 6e69 7422 2c20 2274 6573 7473 2f69 6e74  nit", "tests/int
-000049c0: 6567 7261 7469 6f6e 2260 2066 6f6c 6465  egration"` folde
-000049d0: 7273 2063 616e 2062 6520 6f76 6572 7269  rs can be overri
-000049e0: 6464 656e 2065 6974 6865 7220 7669 6120  dden either via 
-000049f0: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
-00004a00: 696f 6e73 2060 2d66 602f 602d 2d66 696c  ions `-f`/`--fil
-00004a10: 6560 2f60 2d2d 666f 6c64 6572 603a 5c6e  e`/`--folder`:\n
-00004a20: 5c6e 6060 6073 6865 6c6c 2073 6372 6970  \n```shell scrip
-00004a30: 745c 6e64 656c 6669 6e6f 2074 6573 7420  t\ndelfino test 
-00004a40: 2d66 2074 6573 7473 2f6f 7468 6572 5c6e  -f tests/other\n
-00004a50: 6060 605c 6e5c 6e4f 7220 7669 6120 636f  ```\n\nOr via co
-00004a60: 6e66 6967 7572 6174 696f 6e20 696e 2074  nfiguration in t
-00004a70: 6865 2060 7079 7072 6f6a 6563 742e 746f  he `pyproject.to
-00004a80: 6d6c 6020 6669 6c65 3a5c 6e5c 6e60 6060  ml` file:\n\n```
-00004a90: 746f 6d6c 5c6e 5b74 6f6f 6c2e 6465 6c66  toml\n[tool.delf
-00004aa0: 696e 6f2e 706c 7567 696e 732e 3c50 4c55  ino.plugins.<PLU
-00004ab0: 4749 4e3e 2e74 6573 745d 5c6e 6669 6c65  GIN>.test]\nfile
-00004ac0: 735f 666f 6c64 6572 7320 3d20 5b5c 2774  s_folders = [\'t
-00004ad0: 6573 7473 2f6f 7468 6572 5c27 5d5c 6e60  ests/other\']\n`
-00004ae0: 6060 5c6e 5c6e 4569 7468 6572 2077 6179  ``\n\nEither way
-00004af0: 2c20 626f 7468 2077 696c 6c20 7265 7375  , both will resu
-00004b00: 6c74 2069 6e20 6578 6563 7574 696e 6720  lt in executing 
-00004b10: 6070 7974 6573 7420 7465 7374 732f 6f74  `pytest tests/ot
-00004b20: 6865 7260 2e5c 6e5c 6e23 2320 4772 6f75  her`.\n\n## Grou
-00004b30: 7069 6e67 2063 6f6d 6d61 6e64 735c 6e5c  ping commands\n\
-00004b40: 6e4f 6674 656e 2069 7420 6973 2075 7365  nOften it is use
-00004b50: 6675 6c20 746f 2072 756e 2073 6576 6572  ful to run sever
-00004b60: 616c 2063 6f6d 6d61 6e64 7320 6173 2061  al commands as a
-00004b70: 2067 726f 7570 2077 6974 6820 6120 6469   group with a di
-00004b80: 6666 6572 656e 7420 636f 6d6d 616e 6420  fferent command 
-00004b90: 6e61 6d65 2e20 436c 6963 6b20 7375 7070  name. Click supp
-00004ba0: 6f72 7473 2063 616c 6c69 6e67 206f 7468  orts calling oth
-00004bb0: 6572 2063 6f6d 6d61 6e64 7320 7769 7468  er commands with
-00004bc0: 205b 6063 6c69 636b 2e43 6f6e 7465 7874   [`click.Context
-00004bd0: 2e66 6f72 7761 7264 605d 2868 7474 7073  .forward`](https
-00004be0: 3a2f 2f63 6c69 636b 2e70 616c 6c65 7473  ://click.pallets
-00004bf0: 7072 6f6a 6563 7473 2e63 6f6d 2f61 7069  projects.com/api
-00004c00: 2f23 636c 6963 6b2e 436f 6e74 6578 742e  /#click.Context.
-00004c10: 666f 7277 6172 6429 206f 7220 5b60 636c  forward) or [`cl
-00004c20: 6963 6b2e 436f 6e74 6578 742e 696e 766f  ick.Context.invo
-00004c30: 6b65 605d 2868 7474 7073 3a2f 2f63 6c69  ke`](https://cli
-00004c40: 636b 2e70 616c 6c65 7473 7072 6f6a 6563  ck.palletsprojec
-00004c50: 7473 2e63 6f6d 2f61 7069 2f23 636c 6963  ts.com/api/#clic
-00004c60: 6b2e 436f 6e74 6578 742e 696e 766f 6b65  k.Context.invoke
-00004c70: 292e 5c6e 5c6e 3c21 2d2d 2054 4f44 4f28  ).\n\n<!-- TODO(
-00004c80: 5261 6465 6b29 3a20 4164 6420 6465 7363  Radek): Add desc
-00004c90: 7269 7074 696f 6e20 6f66 2060 6578 6563  ription of `exec
-00004ca0: 7574 655f 636f 6d6d 616e 6473 5f67 726f  ute_commands_gro
-00004cb0: 7570 6020 6f6e 6365 206d 6967 7261 7465  up` once migrate
-00004cc0: 6420 6672 6f6d 2060 6465 6c66 696e 6f2d  d from `delfino-
-00004cd0: 636f 7265 602e 202d 2d3e 5c6e 272c 0a20  core`. -->\n',. 
-00004ce0: 2020 2027 6175 7468 6f72 273a 2027 5261     'author': 'Ra
-00004cf0: 6465 6b20 4cc3 a174 272c 0a20 2020 2027  dek L..t',.    '
-00004d00: 6175 7468 6f72 5f65 6d61 696c 273a 2027  author_email': '
-00004d10: 7261 6465 6b2e 6c61 7440 676d 6169 6c2e  radek.lat@gmail.
-00004d20: 636f 6d27 2c0a 2020 2020 276d 6169 6e74  com',.    'maint
-00004d30: 6169 6e65 7227 3a20 274e 6f6e 6527 2c0a  ainer': 'None',.
-00004d40: 2020 2020 276d 6169 6e74 6169 6e65 725f      'maintainer_
-00004d50: 656d 6169 6c27 3a20 274e 6f6e 6527 2c0a  email': 'None',.
-00004d60: 2020 2020 2775 726c 273a 2027 6874 7470      'url': 'http
-00004d70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00004d80: 6164 656b 6c61 742f 6465 6c66 696e 6f27  adeklat/delfino'
-00004d90: 2c0a 2020 2020 2770 6163 6b61 6765 5f64  ,.    'package_d
-00004da0: 6972 273a 2070 6163 6b61 6765 5f64 6972  ir': package_dir
-00004db0: 2c0a 2020 2020 2770 6163 6b61 6765 7327  ,.    'packages'
-00004dc0: 3a20 7061 636b 6167 6573 2c0a 2020 2020  : packages,.    
-00004dd0: 2770 6163 6b61 6765 5f64 6174 6127 3a20  'package_data': 
-00004de0: 7061 636b 6167 655f 6461 7461 2c0a 2020  package_data,.  
-00004df0: 2020 2769 6e73 7461 6c6c 5f72 6571 7569    'install_requi
-00004e00: 7265 7327 3a20 696e 7374 616c 6c5f 7265  res': install_re
-00004e10: 7175 6972 6573 2c0a 2020 2020 2765 7874  quires,.    'ext
-00004e20: 7261 735f 7265 7175 6972 6527 3a20 6578  ras_require': ex
-00004e30: 7472 6173 5f72 6571 7569 7265 2c0a 2020  tras_require,.  
-00004e40: 2020 2765 6e74 7279 5f70 6f69 6e74 7327    'entry_points'
-00004e50: 3a20 656e 7472 795f 706f 696e 7473 2c0a  : entry_points,.
-00004e60: 2020 2020 2770 7974 686f 6e5f 7265 7175      'python_requ
-00004e70: 6972 6573 273a 2027 3e3d 332e 372e 322c  ires': '>=3.7.2,
-00004e80: 3c34 2e30 2e30 272c 0a7d 0a0a 0a73 6574  <4.0.0',.}...set
-00004e90: 7570 282a 2a73 6574 7570 5f6b 7761 7267  up(**setup_kwarg
-00004ea0: 7329 0a                                  s).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6465 6c66  : 2.1.Name: delf
+00000020: 696e 6f0a 5665 7273 696f 6e3a 2032 2e30  ino.Version: 2.0
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4120 636f  .0.Summary: A co
+00000040: 6c6c 6563 7469 6f6e 206f 6620 636f 6d6d  llection of comm
+00000050: 616e 6420 6c69 6e65 2068 656c 7065 7220  and line helper 
+00000060: 7363 7269 7074 7320 7772 6170 7069 6e67  scripts wrapping
+00000070: 2074 6f6f 6c73 2075 7365 6420 6475 7269   tools used duri
+00000080: 6e67 2050 7974 686f 6e20 6465 7665 6c6f  ng Python develo
+00000090: 706d 656e 742e 0a48 6f6d 652d 7061 6765  pment..Home-page
+000000a0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000b0: 2e63 6f6d 2f72 6164 656b 6c61 742f 6465  .com/radeklat/de
+000000c0: 6c66 696e 6f0a 4c69 6365 6e73 653a 204d  lfino.License: M
+000000d0: 4954 0a41 7574 686f 723a 2052 6164 656b  IT.Author: Radek
+000000e0: 204c c3a1 740a 4175 7468 6f72 2d65 6d61   L..t.Author-ema
+000000f0: 696c 3a20 7261 6465 6b2e 6c61 7440 676d  il: radek.lat@gm
+00000100: 6169 6c2e 636f 6d0a 5265 7175 6972 6573  ail.com.Requires
+00000110: 2d50 7974 686f 6e3a 203e 3d33 2e38 2c3c  -Python: >=3.8,<
+00000120: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
+00000130: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000140: 7573 203a 3a20 3420 2d20 4265 7461 0a43  us :: 4 - Beta.C
+00000150: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
+00000160: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
+00000170: 650a 436c 6173 7369 6669 6572 3a20 496e  e.Classifier: In
+00000180: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000190: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+000001a0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+000001b0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001c0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000001d0: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+000001e0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000001f0: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000200: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000210: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000220: 203a 3a20 5079 7468 6f6e 203a 3a20 330a   :: Python :: 3.
+00000230: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000260: 380a 436c 6173 7369 6669 6572 3a20 5072  8.Classifier: Pr
+00000270: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000280: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000290: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+000002a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002c0: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
+000002d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000002e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000002f0: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
+00000300: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000310: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000320: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
+00000330: 790a 436c 6173 7369 6669 6572 3a20 546f  y.Classifier: To
+00000340: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000350: 4465 7665 6c6f 706d 656e 740a 436c 6173  Development.Clas
+00000360: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000370: 2055 7469 6c69 7469 6573 0a50 726f 7669   Utilities.Provi
+00000380: 6465 732d 4578 7472 613a 2063 6f6d 706c  des-Extra: compl
+00000390: 6574 696f 6e0a 5265 7175 6972 6573 2d44  etion.Requires-D
+000003a0: 6973 743a 2063 6c69 636b 2028 3e3d 382e  ist: click (>=8.
+000003b0: 302c 3c39 2e30 290a 5265 7175 6972 6573  0,<9.0).Requires
+000003c0: 2d44 6973 743a 2064 6570 7265 6361 7469  -Dist: deprecati
+000003d0: 6f6e 2028 3e3d 322e 312c 3c33 2e30 290a  on (>=2.1,<3.0).
+000003e0: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
+000003f0: 6d70 6f72 746c 6962 2d6d 6574 6164 6174  mportlib-metadat
+00000400: 6120 3b20 7079 7468 6f6e 5f76 6572 7369  a ; python_versi
+00000410: 6f6e 203c 2022 332e 3130 220a 5265 7175  on < "3.10".Requ
+00000420: 6972 6573 2d44 6973 743a 2070 7964 616e  ires-Dist: pydan
+00000430: 7469 6320 283e 3d31 2e38 2c3c 322e 3029  tic (>=1.8,<2.0)
+00000440: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000450: 746f 6d6c 2028 3e3d 302e 3130 2c3c 302e  toml (>=0.10,<0.
+00000460: 3131 290a 4465 7363 7269 7074 696f 6e2d  11).Description-
+00000470: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000480: 7874 2f6d 6172 6b64 6f77 6e0a 0a3c 6831  xt/markdown..<h1
+00000490: 2061 6c69 676e 3d22 6365 6e74 6572 2220   align="center" 
+000004a0: 7374 796c 653d 2262 6f72 6465 722d 626f  style="border-bo
+000004b0: 7474 6f6d 3a20 6e6f 6e65 3b22 3ef0 9fa7  ttom: none;">...
+000004c0: b026 6e62 7370 3b26 6e62 7370 3b44 656c  .&nbsp;&nbsp;Del
+000004d0: 6669 6e6f 266e 6273 703b 266e 6273 703b  fino&nbsp;&nbsp;
+000004e0: f09f a7b0 3c2f 6831 3e0a 3c68 3320 616c  ....</h1>.<h3 al
+000004f0: 6967 6e3d 2263 656e 7465 7222 3e54 6865  ign="center">The
+00000500: 2055 6c74 696d 6174 6520 436f 6d6d 616e   Ultimate Comman
+00000510: 6420 4c69 6e65 2043 6f6d 7061 6e69 6f6e  d Line Companion
+00000520: 2066 6f72 2059 6f75 7220 5072 6f6a 6563   for Your Projec
+00000530: 7473 3c2f 6833 3e0a 0a3c 7020 616c 6967  ts</h3>..<p alig
+00000540: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+00000550: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000560: 2f61 7070 2e63 6972 636c 6563 692e 636f  /app.circleci.co
+00000570: 6d2f 7069 7065 6c69 6e65 732f 6769 7468  m/pipelines/gith
+00000580: 7562 2f72 6164 656b 6c61 742f 6465 6c66  ub/radeklat/delf
+00000590: 696e 6f3f 6272 616e 6368 3d6d 6169 6e22  ino?branch=main"
+000005a0: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
+000005b0: 6c74 3d22 4369 7263 6c65 4349 2220 7372  lt="CircleCI" sr
+000005c0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000005d0: 6869 656c 6473 2e69 6f2f 6369 7263 6c65  hields.io/circle
+000005e0: 6369 2f62 7569 6c64 2f67 6974 6875 622f  ci/build/github/
+000005f0: 7261 6465 6b6c 6174 2f64 656c 6669 6e6f  radeklat/delfino
+00000600: 223e 0a20 2020 203c 2f61 3e0a 2020 2020  ">.    </a>.    
+00000610: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000620: 2f61 7070 2e63 6f64 6563 6f76 2e69 6f2f  /app.codecov.io/
+00000630: 6768 2f72 6164 656b 6c61 742f 6465 6c66  gh/radeklat/delf
+00000640: 696e 6f2f 223e 0a20 2020 2020 2020 203c  ino/">.        <
+00000650: 696d 6720 616c 743d 2243 6f64 6563 6f76  img alt="Codecov
+00000660: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000670: 6d67 2e73 6869 656c 6473 2e69 6f2f 636f  mg.shields.io/co
+00000680: 6465 636f 762f 632f 6769 7468 7562 2f72  decov/c/github/r
+00000690: 6164 656b 6c61 742f 6465 6c66 696e 6f22  adeklat/delfino"
+000006a0: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
+000006b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000006c0: 6769 7468 7562 2e63 6f6d 2f72 6164 656b  github.com/radek
+000006d0: 6c61 742f 6465 6c66 696e 6f2f 7461 6773  lat/delfino/tags
+000006e0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+000006f0: 616c 743d 2247 6974 4875 6220 7461 6720  alt="GitHub tag 
+00000700: 286c 6174 6573 7420 5365 6d56 6572 2922  (latest SemVer)"
+00000710: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000720: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000730: 6875 622f 7461 672f 7261 6465 6b6c 6174  hub/tag/radeklat
+00000740: 2f64 656c 6669 6e6f 223e 0a20 2020 203c  /delfino">.    <
+00000750: 2f61 3e0a 2020 2020 3c69 6d67 2061 6c74  /a>.    <img alt
+00000760: 3d22 4d61 696e 7465 6e61 6e63 6522 2073  ="Maintenance" s
+00000770: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000780: 7368 6965 6c64 732e 696f 2f6d 6169 6e74  shields.io/maint
+00000790: 656e 616e 6365 2f79 6573 2f32 3032 3322  enance/yes/2023"
+000007a0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+000007b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000007c0: 6d2f 7261 6465 6b6c 6174 2f64 656c 6669  m/radeklat/delfi
+000007d0: 6e6f 2f63 6f6d 6d69 7473 2f6d 6169 6e22  no/commits/main"
+000007e0: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
+000007f0: 6c74 3d22 4769 7448 7562 206c 6173 7420  lt="GitHub last 
+00000800: 636f 6d6d 6974 2220 7372 633d 2268 7474  commit" src="htt
+00000810: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000820: 2e69 6f2f 6769 7468 7562 2f6c 6173 742d  .io/github/last-
+00000830: 636f 6d6d 6974 2f72 6164 656b 6c61 742f  commit/radeklat/
+00000840: 6465 6c66 696e 6f22 3e0a 2020 2020 3c2f  delfino">.    </
+00000850: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000860: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
+00000870: 6f6e 2e6f 7267 2f64 6f63 2f76 6572 7369  on.org/doc/versi
+00000880: 6f6e 732f 223e 0a20 2020 2020 2020 203c  ons/">.        <
+00000890: 696d 6720 616c 743d 2250 7950 4920 2d20  img alt="PyPI - 
+000008a0: 5079 7468 6f6e 2056 6572 7369 6f6e 2220  Python Version" 
+000008b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000008c0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+000008d0: 2f70 7976 6572 7369 6f6e 732f 6465 6c66  /pyversions/delf
+000008e0: 696e 6f22 3e0a 2020 2020 3c2f 613e 0a20  ino">.    </a>. 
+000008f0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000900: 733a 2f2f 7079 7069 7374 6174 732e 6f72  s://pypistats.or
+00000910: 672f 7061 636b 6167 6573 2f64 656c 6669  g/packages/delfi
+00000920: 6e6f 223e 0a20 2020 2020 2020 203c 696d  no">.        <im
+00000930: 6720 616c 743d 2244 6f77 6e6c 6f61 6473  g alt="Downloads
+00000940: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+00000950: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000960: 7069 2f64 6d2f 6465 6c66 696e 6f22 3e0a  pi/dm/delfino">.
+00000970: 2020 2020 3c2f 613e 0a3c 2f70 3e0a 0a54      </a>.</p>..T
+00000980: 6972 6564 206f 6620 6d61 6e61 6769 6e67  ired of managing
+00000990: 2073 6361 7474 6572 6564 2073 6372 6970   scattered scrip
+000009a0: 7473 3f20 5361 7920 676f 6f64 6279 6520  ts? Say goodbye 
+000009b0: 746f 2063 6f6d 706c 6578 6974 7920 7769  to complexity wi
+000009c0: 7468 2044 656c 6669 6e6f 210a 0a44 656c  th Delfino!..Del
+000009d0: 6669 6e6f 2069 7320 6120 706f 7765 7266  fino is a powerf
+000009e0: 756c 2077 7261 7070 6572 2061 726f 756e  ul wrapper aroun
+000009f0: 6420 436c 6963 6b2c 2074 6865 2070 6f70  d Click, the pop
+00000a00: 756c 6172 2063 6f6d 6d61 6e64 206c 696e  ular command lin
+00000a10: 6520 696e 7465 7266 6163 6520 7061 636b  e interface pack
+00000a20: 6167 652e 2049 7420 6175 746f 6d61 7469  age. It automati
+00000a30: 6361 6c6c 7920 6469 7363 6f76 6572 7320  cally discovers 
+00000a40: 616e 6420 6578 6563 7574 6573 2043 6c69  and executes Cli
+00000a50: 636b 2063 6f6d 6d61 6e64 7320 696e 2079  ck commands in y
+00000a60: 6f75 7220 7072 6f6a 6563 742e 2042 7574  our project. But
+00000a70: 2044 656c 6669 6e6f 2064 6f65 736e 2774   Delfino doesn't
+00000a80: 2073 746f 7020 7468 6572 6520 2d20 6974   stop there - it
+00000a90: 2074 616b 6573 2069 7420 6120 7374 6570   takes it a step
+00000aa0: 2066 7572 7468 6572 2062 7920 616c 6c6f   further by allo
+00000ab0: 7769 6e67 2079 6f75 2074 6f20 6372 6561  wing you to crea
+00000ac0: 7465 2070 6c75 6769 6e73 2c20 6d61 6b69  te plugins, maki
+00000ad0: 6e67 2073 6372 6970 7420 6469 7374 7269  ng script distri
+00000ae0: 6275 7469 6f6e 2061 6e64 2069 6e73 7461  bution and insta
+00000af0: 6c6c 6174 696f 6e20 6120 6272 6565 7a65  llation a breeze
+00000b00: 2e0a 0a23 2057 6879 2063 686f 6f73 6520  ...# Why choose 
+00000b10: 4465 6c66 696e 6f3f 0a0a 2d20 2a2a 5374  Delfino?..- **St
+00000b20: 7265 616d 6c69 6e65 2053 6372 6970 7473  reamline Scripts
+00000b30: 2a2a 3a20 436f 6e73 6f6c 6964 6174 6520  **: Consolidate 
+00000b40: 616c 6c20 796f 7572 2068 656c 7065 7220  all your helper 
+00000b50: 7363 7269 7074 7320 696e 746f 2061 2073  scripts into a s
+00000b60: 696e 676c 652c 2065 6173 792d 746f 2d75  ingle, easy-to-u
+00000b70: 7365 2065 6e74 7279 2070 6f69 6e74 2e20  se entry point. 
+00000b80: 4e6f 206d 6f72 6520 6875 6e74 696e 6720  No more hunting 
+00000b90: 666f 7220 7363 7269 7074 7320 6f72 2064  for scripts or d
+00000ba0: 6561 6c69 6e67 2077 6974 6820 636f 6e76  ealing with conv
+00000bb0: 6f6c 7574 6564 2061 6c69 6173 6573 2e20  oluted aliases. 
+00000bc0: 5369 6d70 6c79 2075 7365 2064 656c 6669  Simply use delfi
+00000bd0: 6e6f 2066 6f6c 6c6f 7765 6420 6279 2074  no followed by t
+00000be0: 6865 2073 6372 6970 7420 6e61 6d65 2061  he script name a
+00000bf0: 6e64 206f 7074 696f 6e73 2e0a 2d20 2a2a  nd options..- **
+00000c00: 5265 7573 6162 6c65 2050 6c75 6769 6e73  Reusable Plugins
+00000c10: 2a2a 3a20 5061 636b 6167 6520 796f 7572  **: Package your
+00000c20: 2068 656c 7065 7220 7363 7269 7074 7320   helper scripts 
+00000c30: 6173 2070 6c75 6769 6e73 2061 6e64 2069  as plugins and i
+00000c40: 6e73 7461 6c6c 2074 6865 6d20 7769 7468  nstall them with
+00000c50: 2070 6970 2e20 4d61 696e 7461 696e 2063   pip. Maintain c
+00000c60: 6f6e 7369 7374 656e 6379 2061 6372 6f73  onsistency acros
+00000c70: 7320 7072 6f6a 6563 7473 2061 6e64 2065  s projects and e
+00000c80: 6173 696c 7920 696e 636f 7270 6f72 6174  asily incorporat
+00000c90: 6520 7570 6461 7465 7320 7468 726f 7567  e updates throug
+00000ca0: 6820 6120 666c 6578 6962 6c65 2063 6f6e  h a flexible con
+00000cb0: 6669 6775 7261 7469 6f6e 2073 7973 7465  figuration syste
+00000cc0: 6d2e 0a2d 202a 2a53 696d 706c 6966 7920  m..- **Simplify 
+00000cd0: 546f 6f6c 696e 672a 2a3a 2044 656c 6669  Tooling**: Delfi
+00000ce0: 6e6f 2065 7874 656e 6473 2043 6c69 636b  no extends Click
+00000cf0: 2077 6974 6820 6164 7661 6e63 6564 2066   with advanced f
+00000d00: 6561 7475 7265 7320 6c69 6b65 2070 6173  eatures like pas
+00000d10: 732d 7468 726f 7567 6820 636f 6d6d 616e  s-through comman
+00000d20: 642d 6c69 6e65 206f 7074 696f 6e73 2061  d-line options a
+00000d30: 6e64 2073 6561 6d6c 6573 7320 6861 6e64  nd seamless hand
+00000d40: 6c69 6e67 206f 6620 6669 6c65 206c 6973  ling of file lis
+00000d50: 7473 2e20 5361 7920 676f 6f64 6279 6520  ts. Say goodbye 
+00000d60: 746f 2076 6572 626f 7369 7479 2061 6e64  to verbosity and
+00000d70: 2068 656c 6c6f 2074 6f20 6f70 7469 6d69   hello to optimi
+00000d80: 7a65 6420 776f 726b 666c 6f77 732e 0a0a  zed workflows...
+00000d90: 446f 6e27 7420 6c65 7420 7363 6174 7465  Don't let scatte
+00000da0: 7265 6420 7363 7269 7074 7320 616e 6420  red scripts and 
+00000db0: 636f 6d70 6c65 7820 746f 6f6c 696e 6720  complex tooling 
+00000dc0: 736c 6f77 2079 6f75 2064 6f77 6e2e 2045  slow you down. E
+00000dd0: 6d62 7261 6365 2044 656c 6669 6e6f 2061  mbrace Delfino a
+00000de0: 6e64 2072 6576 6f6c 7574 696f 6e69 7a65  nd revolutionize
+00000df0: 2079 6f75 7220 636f 6d6d 616e 6420 6c69   your command li
+00000e00: 6e65 2065 7870 6572 6965 6e63 652e 2054  ne experience. T
+00000e10: 7279 2044 656c 6669 6e6f 2074 6f64 6179  ry Delfino today
+00000e20: 2061 6e64 2075 6e6c 6f63 6b20 7369 6d70   and unlock simp
+00000e30: 6c69 6369 7479 2069 6e20 796f 7572 2070  licity in your p
+00000e40: 726f 6a65 6374 7321 0a0a 3c21 2d2d 0a20  rojects!..<!--. 
+00000e50: 2020 2048 6f77 2074 6f20 6765 6e65 7261     How to genera
+00000e60: 7465 2054 4f43 2066 726f 6d20 5079 4368  te TOC from PyCh
+00000e70: 6172 6d3a 0a20 2020 2068 7474 7073 3a2f  arm:.    https:/
+00000e80: 2f67 6974 6875 622e 636f 6d2f 7673 6368  /github.com/vsch
+00000e90: 2f69 6465 612d 6d75 6c74 696d 6172 6b64  /idea-multimarkd
+00000ea0: 6f77 6e2f 7769 6b69 2f54 6162 6c65 2d6f  own/wiki/Table-o
+00000eb0: 662d 436f 6e74 656e 7473 2d45 7874 656e  f-Contents-Exten
+00000ec0: 7369 6f6e 0a2d 2d3e 0a5b 544f 4320 6c65  sion.-->.[TOC le
+00000ed0: 7665 6c73 3d31 2c32 206d 6172 6b64 6f77  vels=1,2 markdow
+00000ee0: 6e20 666f 726d 6174 7465 6420 6275 6c6c  n formatted bull
+00000ef0: 6574 2068 6965 7261 7263 6879 5d3a 2023  et hierarchy]: #
+00000f00: 2022 5461 626c 6520 6f66 2063 6f6e 7465   "Table of conte
+00000f10: 6e74 220a 0a23 2054 6162 6c65 206f 6620  nt"..# Table of 
+00000f20: 636f 6e74 656e 740a 2d20 5b49 6e73 7461  content.- [Insta
+00000f30: 6c6c 6174 696f 6e5d 2823 696e 7374 616c  llation](#instal
+00000f40: 6c61 7469 6f6e 290a 2d20 5b43 6f6e 6669  lation).- [Confi
+00000f50: 6775 7261 7469 6f6e 5d28 2363 6f6e 6669  guration](#confi
+00000f60: 6775 7261 7469 6f6e 290a 2d20 5b55 7361  guration).- [Usa
+00000f70: 6765 5d28 2375 7361 6765 290a 2d20 5b44  ge](#usage).- [D
+00000f80: 6576 656c 6f70 6d65 6e74 5d28 2364 6576  evelopment](#dev
+00000f90: 656c 6f70 6d65 6e74 290a 2020 2d20 5b43  elopment).  - [C
+00000fa0: 6f6d 6d61 6e64 7320 6469 7363 6f76 6572  ommands discover
+00000fb0: 795d 2823 636f 6d6d 616e 6473 2d64 6973  y](#commands-dis
+00000fc0: 636f 7665 7279 290a 2020 2d20 5b4d 696e  covery).  - [Min
+00000fd0: 696d 616c 2063 6f6d 6d61 6e64 5d28 236d  imal command](#m
+00000fe0: 696e 696d 616c 2d63 6f6d 6d61 6e64 290a  inimal-command).
+00000ff0: 2020 2d20 5b4d 696e 696d 616c 2070 6c75    - [Minimal plu
+00001000: 6769 6e5d 2823 6d69 6e69 6d61 6c2d 706c  gin](#minimal-pl
+00001010: 7567 696e 290a 2d20 5b45 7869 7374 696e  ugin).- [Existin
+00001020: 6720 706c 7567 696e 735d 2823 6578 6973  g plugins](#exis
+00001030: 7469 6e67 2d70 6c75 6769 6e73 290a 2020  ting-plugins).  
+00001040: 2d20 5b45 6e61 626c 696e 6720 6120 706c  - [Enabling a pl
+00001050: 7567 696e 5d28 2365 6e61 626c 696e 672d  ugin](#enabling-
+00001060: 612d 706c 7567 696e 290a 2020 2d20 5b45  a-plugin).  - [E
+00001070: 6e61 626c 696e 672f 6469 7361 626c 696e  nabling/disablin
+00001080: 6720 636f 6d6d 616e 6473 5d28 2365 6e61  g commands](#ena
+00001090: 626c 696e 6764 6973 6162 6c69 6e67 2d63  blingdisabling-c
+000010a0: 6f6d 6d61 6e64 7329 0a2d 205b 4164 7661  ommands).- [Adva
+000010b0: 6e63 6564 2075 7361 6765 5d28 2361 6476  nced usage](#adv
+000010c0: 616e 6365 642d 7573 6167 6529 0a20 202d  anced-usage).  -
+000010d0: 205b 4175 746f 2d63 6f6d 706c 6574 696f   [Auto-completio
+000010e0: 6e5d 2823 6175 746f 2d63 6f6d 706c 6574  n](#auto-complet
+000010f0: 696f 6e29 0a20 202d 205b 5275 6e6e 696e  ion).  - [Runnin
+00001100: 6720 6578 7465 726e 616c 2070 726f 6772  g external progr
+00001110: 616d 735d 2823 7275 6e6e 696e 672d 6578  ams](#running-ex
+00001120: 7465 726e 616c 2d70 726f 6772 616d 7329  ternal-programs)
+00001130: 0a20 202d 205b 4f70 7469 6f6e 616c 2064  .  - [Optional d
+00001140: 6570 656e 6465 6e63 6965 735d 2823 6f70  ependencies](#op
+00001150: 7469 6f6e 616c 2d64 6570 656e 6465 6e63  tional-dependenc
+00001160: 6965 7329 0a20 202d 205b 5072 6f6a 6563  ies).  - [Projec
+00001170: 7420 7365 7474 696e 6773 5d28 2370 726f  t settings](#pro
+00001180: 6a65 6374 2d73 6574 7469 6e67 7329 0a20  ject-settings). 
+00001190: 202d 205b 506c 7567 696e 2073 6574 7469   - [Plugin setti
+000011a0: 6e67 735d 2823 706c 7567 696e 2d73 6574  ngs](#plugin-set
+000011b0: 7469 6e67 7329 0a20 202d 205b 5072 6f6a  tings).  - [Proj
+000011c0: 6563 7420 7370 6563 6966 6963 206f 7665  ect specific ove
+000011d0: 7272 6964 6573 5d28 2370 726f 6a65 6374  rrides](#project
+000011e0: 2d73 7065 6369 6669 632d 6f76 6572 7269  -specific-overri
+000011f0: 6465 7329 0a20 202d 205b 4772 6f75 7069  des).  - [Groupi
+00001200: 6e67 2063 6f6d 6d61 6e64 735d 2823 6772  ng commands](#gr
+00001210: 6f75 7069 6e67 2d63 6f6d 6d61 6e64 7329  ouping-commands)
+00001220: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
+00001230: 0a0a 2d20 7069 703a 2060 7069 7020 696e  ..- pip: `pip in
+00001240: 7374 616c 6c20 6465 6c66 696e 6f60 0a2d  stall delfino`.-
+00001250: 2050 6f65 7472 793a 2060 706f 6574 7279   Poetry: `poetry
+00001260: 2061 6464 202d 2d67 726f 7570 3d64 6576   add --group=dev
+00001270: 2064 656c 6669 6e6f 600a 2d20 5069 7065   delfino`.- Pipe
+00001280: 6e76 3a20 6070 6970 656e 7620 696e 7374  nv: `pipenv inst
+00001290: 616c 6c20 2d64 2064 656c 6669 6e6f 600a  all -d delfino`.
+000012a0: 0a6f 7220 0a0a 2d20 7069 703a 2060 7069  .or ..- pip: `pi
+000012b0: 7020 696e 7374 616c 6c20 6465 6c66 696e  p install delfin
+000012c0: 6f5b 636f 6d70 6c65 7469 6f6e 5d60 0a2d  o[completion]`.-
+000012d0: 2050 6f65 7472 793a 2060 706f 6574 7279   Poetry: `poetry
+000012e0: 2061 6464 202d 2d67 726f 7570 3d64 6576   add --group=dev
+000012f0: 2064 656c 6669 6e6f 5b63 6f6d 706c 6574   delfino[complet
+00001300: 696f 6e5d 600a 2d20 5069 7065 6e76 3a20  ion]`.- Pipenv: 
+00001310: 6070 6970 656e 7620 696e 7374 616c 6c20  `pipenv install 
+00001320: 2d64 2064 656c 6669 6e6f 5b63 6f6d 706c  -d delfino[compl
+00001330: 6574 696f 6e5d 600a 0a74 6f20 656e 6162  etion]`..to enab
+00001340: 6c65 205b 6175 746f 2d63 6f6d 706c 6574  le [auto-complet
+00001350: 696f 6e5d 2823 6175 746f 2d63 6f6d 706c  ion](#auto-compl
+00001360: 6574 696f 6e29 2e0a 0a23 2043 6f6e 6669  etion)...# Confi
+00001370: 6775 7261 7469 6f6e 0a0a 416c 6c20 636f  guration..All co
+00001380: 6e66 6967 7572 6174 696f 6e20 6973 2065  nfiguration is e
+00001390: 7870 6563 7465 6420 746f 206c 6976 6520  xpected to live 
+000013a0: 696e 206f 6e65 206f 6620 7468 6520 666f  in one of the fo
+000013b0: 6c6c 6f77 696e 6720 6669 6c65 733a 0a0a  llowing files:..
+000013c0: 2d20 6070 7970 726f 6a65 6374 2e74 6f6d  - `pyproject.tom
+000013d0: 6c60 2069 6e20 7468 6520 7072 6f6a 6563  l` in the projec
+000013e0: 7420 726f 6f74 0a2d 2060 2e64 656c 6669  t root.- `.delfi
+000013f0: 6e6f 7263 6020 696e 2074 6865 2070 726f  norc` in the pro
+00001400: 6a65 6374 2072 6f6f 7420 2d20 746f 2061  ject root - to a
+00001410: 6c6c 6f77 2064 6576 2073 7065 6369 6669  llow dev specifi
+00001420: 6320 636f 6e66 6967 2c20 6e6f 7420 736f  c config, not so
+00001430: 7572 6365 2063 6f6e 7472 6f6c 6c65 6420  urce controlled 
+00001440: 6f72 2066 6f72 206e 6f6e 2d50 7974 686f  or for non-Pytho
+00001450: 6e20 7072 6f6a 6563 7473 0a2d 2060 2e64  n projects.- `.d
+00001460: 656c 6669 6e6f 7263 6020 696e 2074 6865  elfinorc` in the
+00001470: 2075 7365 7220 686f 6d65 2064 6972 6563   user home direc
+00001480: 746f 7279 202d 2066 6f72 2075 7365 7220  tory - for user 
+00001490: 746f 6f6c 7320 6176 6169 6c61 626c 6520  tools available 
+000014a0: 696e 2074 6865 2073 7973 7465 6d0a 0a49  in the system..I
+000014b0: 6620 6d75 6c74 6970 6c65 2066 696c 6573  f multiple files
+000014c0: 2061 7265 2064 6973 636f 7665 7265 642c   are discovered,
+000014d0: 206f 6e6c 7920 7468 6520 6869 6768 6573   only the highes
+000014e0: 7420 6f6e 6520 696e 2074 6865 206c 6973  t one in the lis
+000014f0: 7420 7769 6c6c 2062 6520 7573 6564 2e0a  t will be used..
+00001500: 0a54 6865 2066 6f72 6d61 7420 666f 7220  .The format for 
+00001510: 602e 6465 6c66 696e 6f72 6360 2069 7320  `.delfinorc` is 
+00001520: 7468 6520 7361 6d65 2061 7320 666f 7220  the same as for 
+00001530: 6070 7970 726f 6a65 6374 2e74 6f6d 6c60  `pyproject.toml`
+00001540: 2e0a 0a23 2055 7361 6765 0a0a 5275 6e20  ...# Usage..Run 
+00001550: 6064 656c 6669 6e6f 202d 2d68 656c 7060  `delfino --help`
+00001560: 2074 6f20 7365 6520 616c 6c20 6176 6169   to see all avai
+00001570: 6c61 626c 6520 636f 6d6d 616e 6473 2061  lable commands a
+00001580: 6e64 2074 6865 6972 2075 7361 6765 2e0a  nd their usage..
+00001590: 0a23 2044 6576 656c 6f70 6d65 6e74 0a0a  .# Development..
+000015a0: 4465 6c66 696e 6f20 6973 2061 2073 696d  Delfino is a sim
+000015b0: 706c 6520 7772 6170 7065 7220 6172 6f75  ple wrapper arou
+000015c0: 6e64 205b 436c 6963 6b20 636f 6d6d 616e  nd [Click comman
+000015d0: 6473 5d28 6874 7470 733a 2f2f 636c 6963  ds](https://clic
+000015e0: 6b2e 7061 6c6c 6574 7370 726f 6a65 6374  k.palletsproject
+000015f0: 732e 636f 6d2f 7175 6963 6b73 7461 7274  s.com/quickstart
+00001600: 2f23 6261 7369 632d 636f 6e63 6570 7473  /#basic-concepts
+00001610: 2d63 7265 6174 696e 672d 612d 636f 6d6d  -creating-a-comm
+00001620: 616e 6429 2e20 416e 7920 436c 6963 6b20  and). Any Click 
+00001630: 636f 6d6d 616e 6420 7769 6c6c 2062 6520  command will be 
+00001640: 6163 6365 7074 6564 2062 7920 4465 6c66  accepted by Delf
+00001650: 696e 6f2e 0a0a 2323 2043 6f6d 6d61 6e64  ino...## Command
+00001660: 7320 6469 7363 6f76 6572 790a 0a44 656c  s discovery..Del
+00001670: 6669 6e6f 206c 6f6f 6b73 2066 6f72 2061  fino looks for a
+00001680: 6e79 205b 6063 6c69 636b 2e43 6f6d 6d61  ny [`click.Comma
+00001690: 6e64 605d 2868 7474 7073 3a2f 2f63 6c69  nd`](https://cli
+000016a0: 636b 2e70 616c 6c65 7473 7072 6f6a 6563  ck.palletsprojec
+000016b0: 7473 2e63 6f6d 2f65 6e2f 382e 302e 782f  ts.com/en/8.0.x/
+000016c0: 6170 692f 2363 6c69 636b 2e43 6f6d 6d61  api/#click.Comma
+000016d0: 6e64 2920 7375 622d 636c 6173 7320 696e  nd) sub-class in
+000016e0: 2074 6865 2066 6f6c 6c6f 7769 6e67 206c   the following l
+000016f0: 6f63 6174 696f 6e73 3a0a 0a2d 2060 636f  ocations:..- `co
+00001700: 6d6d 616e 6473 6020 666f 6c64 6572 2069  mmands` folder i
+00001710: 6e20 7468 6520 726f 6f74 206f 6620 7468  n the root of th
+00001720: 6520 7072 6f6a 6563 7420 286e 6578 7420  e project (next 
+00001730: 746f 2074 6865 2060 7079 7072 6f6a 6563  to the `pyprojec
+00001740: 742e 746f 6d6c 6020 6669 6c65 292e 2054  t.toml` file). T
+00001750: 6869 7320 6c6f 6361 7469 6f6e 2069 7320  his location is 
+00001760: 7573 6566 756c 2066 6f72 2063 6f6d 6d61  useful for comma
+00001770: 6e64 7320 7468 6174 2064 6f6e 2774 206e  nds that don't n
+00001780: 6565 6420 746f 2062 6520 7265 706c 6963  eed to be replic
+00001790: 6174 6564 2069 6e20 6d75 6c74 6970 6c65  ated in multiple
+000017a0: 206c 6f63 6174 696f 6e73 2f70 726f 6a65   locations/proje
+000017b0: 6374 732e 2054 6f20 6368 616e 6765 2074  cts. To change t
+000017c0: 6865 2064 6566 6175 6c74 206c 6f63 6174  he default locat
+000017d0: 696f 6e2c 2075 7365 2074 6865 2060 746f  ion, use the `to
+000017e0: 6f6c 2e64 656c 6669 6e6f 2e6c 6f63 616c  ol.delfino.local
+000017f0: 5f63 6f6d 6d61 6e64 5f66 6f6c 6465 7273  _command_folders
+00001800: 6020 636f 6e66 6967 206f 7074 696f 6e2e  ` config option.
+00001810: 2049 7420 616c 6c6f 7773 2073 7065 6369   It allows speci
+00001820: 6679 696e 6720 6d6f 7265 2074 6861 6e20  fying more than 
+00001830: 6f6e 6520 666f 6c64 6572 2e0a 2d20 7079  one folder..- py
+00001840: 7468 6f6e 206d 6f64 756c 6520 696d 706f  thon module impo
+00001850: 7274 2070 6174 6820 2860 3c49 4d50 4f52  rt path (`<IMPOR
+00001860: 545f 5041 5448 3e60 2920 7370 6563 6966  T_PATH>`) specif
+00001870: 6965 6420 6279 2060 656e 7472 795f 706f  ied by `entry_po
+00001880: 696e 7460 206f 6620 5b61 2070 6c75 6769  int` of [a plugi
+00001890: 6e5d 2823 6d69 6e69 6d61 6c2d 706c 7567  n](#minimal-plug
+000018a0: 696e 293a 0a20 2060 6060 746f 6d6c 0a20  in):.  ```toml. 
+000018b0: 205b 746f 6f6c 2e70 6f65 7472 792e 706c   [tool.poetry.pl
+000018c0: 7567 696e 735d 2023 204f 7074 696f 6e61  ugins] # Optiona
+000018d0: 6c20 7375 7065 7220 7461 626c 650a 0a20  l super table.. 
+000018e0: 205b 746f 6f6c 2e70 6f65 7472 792e 706c   [tool.poetry.pl
+000018f0: 7567 696e 732e 2264 656c 6669 6e6f 2e70  ugins."delfino.p
+00001900: 6c75 6769 6e22 5d0a 2020 2264 656c 6669  lugin"].  "delfi
+00001910: 6e6f 2d3c 504c 5547 494e 5f4e 414d 453e  no-<PLUGIN_NAME>
+00001920: 2220 3d20 223c 494d 504f 5254 5f50 4154  " = "<IMPORT_PAT
+00001930: 483e 220a 2020 6060 600a 2d20 466f 6c64  H>".  ```.- Fold
+00001940: 6572 2073 7065 6369 6669 6564 2069 6e20  er specified in 
+00001950: 7468 6520 5b63 6f6e 6669 6720 6669 6c65  the [config file
+00001960: 5d28 2363 6f6e 6669 6775 7261 7469 6f6e  ](#configuration
+00001970: 2920 756e 6465 7220 6074 6f6f 6c2e 6465  ) under `tool.de
+00001980: 6c66 696e 6f2e 6c6f 6361 6c5f 636f 6d6d  lfino.local_comm
+00001990: 616e 6473 5f64 6972 6563 746f 7279 602e  ands_directory`.
+000019a0: 0a0a 416e 7920 6669 6c65 7320 7374 6172  ..Any files star
+000019b0: 7469 6e67 2077 6974 6820 616e 2075 6e64  ting with an und
+000019c0: 6572 7363 6f72 652c 2065 7863 6570 7420  erscore, except 
+000019d0: 666f 7220 605f 5f69 6e69 745f 5f2e 7079  for `__init__.py
+000019e0: 602c 2077 696c 6c20 6265 2069 676e 6f72  `, will be ignor
+000019f0: 6564 2e0a 0a3e 202a 2a57 6172 6e69 6e67  ed...> **Warning
+00001a00: 2a2a 0a3e 2046 6f6c 6465 7273 2061 7265  **.> Folders are
+00001a10: 204e 4f54 2069 6e73 7065 6374 6564 2072   NOT inspected r
+00001a20: 6563 7572 7369 7665 6c79 2e20 4966 2079  ecursively. If y
+00001a30: 6f75 2070 6c61 6365 2061 6e79 2063 6f6d  ou place any com
+00001a40: 6d61 6e64 7320 696e 746f 206e 6573 7465  mands into neste
+00001a50: 6420 666f 6c64 6572 732c 2074 6865 7920  d folders, they 
+00001a60: 7769 6c6c 206e 6f74 2062 6520 6c6f 6164  will not be load
+00001a70: 6564 2062 7920 4465 6c66 696e 6f2e 0a0a  ed by Delfino...
+00001a80: 0a23 2320 4d69 6e69 6d61 6c20 636f 6d6d  .## Minimal comm
+00001a90: 616e 640a 0a3c 212d 2d20 544f 444f 2852  and..<!-- TODO(R
+00001aa0: 6164 656b 293a 2044 656c 6669 6e6f 2065  adek): Delfino e
+00001ab0: 7870 6563 7473 2060 7079 7072 6f6a 6563  xpects `pyprojec
+00001ac0: 742e 746f 6d6c 6020 636f 6e66 6967 7572  t.toml` configur
+00001ad0: 6564 2e20 2d2d 3e0a 3c21 2d2d 2054 4f44  ed. -->.<!-- TOD
+00001ae0: 4f28 5261 6465 6b29 3a20 4465 6c66 696e  O(Radek): Delfin
+00001af0: 6f20 6578 7065 6374 7320 506f 6574 7279  o expects Poetry
+00001b00: 206f 7220 5069 7065 6e76 2074 6f20 6265   or Pipenv to be
+00001b10: 2061 7661 696c 6162 6c65 2e20 2d2d 3e0a   available. -->.
+00001b20: 0a31 2e20 4372 6561 7465 2061 2060 636f  .1. Create a `co
+00001b30: 6d6d 616e 6473 6020 666f 6c64 6572 3a0a  mmands` folder:.
+00001b40: 2020 2060 6060 7368 656c 6c20 7363 7269     ```shell scri
+00001b50: 7074 0a20 2020 6d6b 6469 7220 636f 6d6d  pt.   mkdir comm
+00001b60: 616e 6473 0a20 2020 6060 600a 322e 2043  ands.   ```.2. C
+00001b70: 7265 6174 6520 6120 6063 6f6d 6d61 6e64  reate a `command
+00001b80: 732f 5f5f 696e 6974 5f5f 2e70 7960 2066  s/__init__.py` f
+00001b90: 696c 652c 2077 6974 6820 7468 6520 666f  ile, with the fo
+00001ba0: 6c6c 6f77 696e 6720 636f 6e74 656e 743a  llowing content:
+00001bb0: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
+00001bc0: 2069 6d70 6f72 7420 636c 6963 6b0a 2020   import click.  
+00001bd0: 200a 2020 2040 636c 6963 6b2e 636f 6d6d   .   @click.comm
+00001be0: 616e 6428 290a 2020 2064 6566 2063 6f6d  and().   def com
+00001bf0: 6d61 6e64 5f74 6573 7428 293a 0a20 2020  mand_test():.   
+00001c00: 2020 2020 2222 2254 6573 7473 2063 6f6d      """Tests com
+00001c10: 6d61 6e64 7320 706c 6163 6564 2069 6e20  mands placed in 
+00001c20: 7468 6520 6063 6f6d 6d61 6e64 7360 2066  the `commands` f
+00001c30: 6f6c 6465 7220 6172 6520 6c6f 6164 6564  older are loaded
+00001c40: 2e22 2222 0a20 2020 2020 2020 7072 696e  .""".       prin
+00001c50: 7428 22e2 9ca8 2054 6869 7320 636f 6d6d  t("... This comm
+00001c60: 616e 6420 776f 726b 7321 20e2 9ca8 2229  and works! ...")
+00001c70: 0a20 2020 6060 600a 332e 2053 6565 2069  .   ```.3. See i
+00001c80: 6620 4465 6c66 696e 6f20 6c6f 6164 7320  f Delfino loads 
+00001c90: 7468 6520 636f 6d6d 616e 642e 204f 7065  the command. Ope
+00001ca0: 6e20 6120 7465 726d 696e 616c 2061 6e64  n a terminal and
+00001cb0: 2069 6e20 7468 6520 726f 6f74 206f 6620   in the root of 
+00001cc0: 7468 6520 7072 6f6a 6563 742c 2063 616c  the project, cal
+00001cd0: 6c3a 2060 6465 6c66 696e 6f20 2d2d 6865  l: `delfino --he
+00001ce0: 6c70 602e 2059 6f75 2073 686f 756c 6420  lp`. You should 
+00001cf0: 7365 6520 736f 6d65 7468 696e 6720 6c69  see something li
+00001d00: 6b65 2074 6869 733a 0a20 2020 6060 6074  ke this:.   ```t
+00001d10: 6578 740a 2020 2055 7361 6765 3a20 6465  ext.   Usage: de
+00001d20: 6c66 696e 6f20 5b4f 5054 494f 4e53 5d20  lfino [OPTIONS] 
+00001d30: 434f 4d4d 414e 4420 5b41 5247 535d 2e2e  COMMAND [ARGS]..
+00001d40: 2e0a 2020 200a 2020 204f 7074 696f 6e73  ..   .   Options
+00001d50: 3a0a 2020 2020 202d 2d68 656c 7020 2053  :.     --help  S
+00001d60: 686f 7720 7468 6973 206d 6573 7361 6765  how this message
+00001d70: 2061 6e64 2065 7869 742e 0a20 2020 0a20   and exit..   . 
+00001d80: 2020 436f 6d6d 616e 6473 3a0a 2020 2020    Commands:.    
+00001d90: 202e 2e2e 0a20 2020 2020 636f 6d6d 616e   ....     comman
+00001da0: 642d 7465 7374 2020 2020 2020 2020 2020  d-test          
+00001db0: 2020 5465 7374 7320 636f 6d6d 616e 6473    Tests commands
+00001dc0: 2070 6c61 6365 6420 696e 2074 6865 2060   placed in the `
+00001dd0: 636f 6d6d 616e 6473 6020 666f 6c64 6572  commands` folder
+00001de0: 2e2e 2e0a 2020 2020 202e 2e2e 0a20 2020  ....     ....   
+00001df0: 6060 600a 342e 2052 756e 2074 6865 2063  ```.4. Run the c
+00001e00: 6f6d 6d61 6e64 2077 6974 6820 6064 656c  ommand with `del
+00001e10: 6669 6e6f 2063 6f6d 6d61 6e64 2d74 6573  fino command-tes
+00001e20: 7460 0a0a 2323 204d 696e 696d 616c 2070  t`..## Minimal p
+00001e30: 6c75 6769 6e0a 0a49 6620 796f 7527 6420  lugin..If you'd 
+00001e40: 6c69 6b65 2074 6f20 7573 6520 6f6e 6520  like to use one 
+00001e50: 6f72 206d 6f72 6520 636f 6d6d 616e 6473  or more commands
+00001e60: 2069 6e20 6d75 6c74 6970 6c65 2070 6c61   in multiple pla
+00001e70: 6365 732c 2079 6f75 2063 616e 2063 7265  ces, you can cre
+00001e80: 6174 6520 6120 706c 7567 696e 2e20 4120  ate a plugin. A 
+00001e90: 706c 7567 696e 2069 7320 6a75 7374 2061  plugin is just a
+00001ea0: 2072 6567 756c 6172 2050 7974 686f 6e20   regular Python 
+00001eb0: 7061 636b 6167 6520 7769 7468 2073 7065  package with spe
+00001ec0: 6369 6669 6320 656e 7472 7920 706f 696e  cific entry poin
+00001ed0: 7420 7465 6c6c 696e 6720 4465 6c66 696e  t telling Delfin
+00001ee0: 6f20 6974 2073 686f 756c 6420 7573 6520  o it should use 
+00001ef0: 6974 2e20 4974 2063 616e 2061 6c73 6f20  it. It can also 
+00001f00: 6265 2064 6973 7472 6962 7574 6564 2061  be distributed a
+00001f10: 7320 616e 7920 6f74 6865 7220 5079 7468  s any other Pyth
+00001f20: 6f6e 2070 6163 6b61 6765 732c 2066 6f72  on packages, for
+00001f30: 2065 7861 6d70 6c65 2076 6961 2050 7970   example via Pyp
+00001f40: 692e 0a0a 5468 6520 7175 6963 6b65 7374  i...The quickest
+00001f50: 2077 6179 2074 6f20 6372 6561 7465 206f   way to create o
+00001f60: 6e65 2069 7320 746f 2075 7365 2061 205b  ne is to use a [
+00001f70: 4465 6c66 696e 6f20 706c 7567 696e 2063  Delfino plugin c
+00001f80: 6f6f 6b69 6563 7574 7465 7220 7465 6d70  ookiecutter temp
+00001f90: 6c61 7465 5d28 6874 7470 733a 2f2f 6769  late](https://gi
+00001fa0: 7468 7562 2e63 6f6d 2f72 6164 656b 6c61  thub.com/radekla
+00001fb0: 742f 6465 6c66 696e 6f2d 706c 7567 696e  t/delfino-plugin
+00001fc0: 2d63 6f6f 6b69 6563 7574 7465 722d 7465  -cookiecutter-te
+00001fd0: 6d70 6c61 7465 292c 2077 6869 6368 2061  mplate), which a
+00001fe0: 736b 7320 796f 7520 7365 7665 7261 6c20  sks you several 
+00001ff0: 7175 6573 7469 6f6e 7320 616e 6420 7365  questions and se
+00002000: 7473 2075 7020 7468 6520 7768 6f6c 6520  ts up the whole 
+00002010: 7072 6f6a 6563 742e 0a0a 416c 7465 726e  project...Altern
+00002020: 6174 6976 656c 792c 2079 6f75 2063 616e  atively, you can
+00002030: 2067 6574 2069 6e73 7069 7265 6420 6279   get inspired by
+00002040: 205b 7468 6520 6465 6d6f 2070 6c75 6769   [the demo plugi
+00002050: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
+00002060: 622e 636f 6d2f 7261 6465 6b6c 6174 2f64  b.com/radeklat/d
+00002070: 656c 6669 6e6f 2d64 656d 6f29 206f 7220  elfino-demo) or 
+00002080: 616e 7920 6f66 2074 6865 206f 7468 6572  any of the other
+00002090: 205b 6578 6973 7469 6e67 2070 6c75 6769   [existing plugi
+000020a0: 6e73 5d28 2370 6c75 6769 6e73 292e 0a0a  ns](#plugins)...
+000020b0: 2320 4578 6973 7469 6e67 2070 6c75 6769  # Existing plugi
+000020c0: 6e73 0a0a 506c 7567 696e 7320 6361 6e20  ns..Plugins can 
+000020d0: 6772 6561 746c 7920 7265 6475 6365 2063  greatly reduce c
+000020e0: 6f64 6520 6475 706c 6963 6174 696f 6e20  ode duplication 
+000020f0: 616e 642f 6f72 2070 726f 6d6f 7465 2079  and/or promote y
+00002100: 6f75 7220 6f77 6e20 7374 616e 6461 7264  our own standard
+00002110: 7320 696e 206d 756c 7469 706c 6520 706c  s in multiple pl
+00002120: 6163 6573 2e20 466f 7220 6578 616d 706c  aces. For exampl
+00002130: 652c 2079 6f75 2063 616e 2063 7265 6174  e, you can creat
+00002140: 6520 6120 706c 7567 696e 2077 7261 7070  e a plugin wrapp
+00002150: 696e 6720 636f 6d6d 6f6e 206c 696e 7469  ing common linti
+00002160: 6e67 2074 6f6f 6c73 2074 6861 7420 796f  ng tools that yo
+00002170: 7520 7573 6520 6f6e 2079 6f75 7220 7072  u use on your pr
+00002180: 6f6a 6563 7473 2c20 696e 636c 7564 696e  ojects, includin
+00002190: 6720 7468 6569 7220 6465 6661 756c 7420  g their default 
+000021a0: 636f 6e66 6967 7572 6174 696f 6e2e 204b  configuration. K
+000021b0: 6565 7069 6e67 2074 6865 2072 756c 6573  eeping the rules
+000021c0: 2061 6e64 2063 7265 6174 696e 6720 6e65   and creating ne
+000021d0: 7720 7072 6f6a 6563 7473 2077 6974 6820  w projects with 
+000021e0: 7468 6520 7361 6d65 2073 7479 6c65 2073  the same style s
+000021f0: 7564 6465 6e6c 7920 6265 636f 6d65 7320  uddenly becomes 
+00002200: 6120 6d61 7474 6572 206f 6620 696e 7374  a matter of inst
+00002210: 616c 6c69 6e67 206f 6e65 2050 7974 686f  alling one Pytho
+00002220: 6e20 6c69 6272 6172 792e 0a0a 4561 6368  n library...Each
+00002230: 2070 6c75 6769 6e20 6361 6e20 636f 6e74   plugin can cont
+00002240: 6169 6e20 6f6e 6520 6f72 206d 6f72 6520  ain one or more 
+00002250: 436c 6963 6b20 636f 6d6d 616e 6473 2074  Click commands t
+00002260: 6861 7420 6172 6520 6175 746f 6d61 7469  hat are automati
+00002270: 6361 6c6c 7920 6469 7363 6f76 6572 6564  cally discovered
+00002280: 2061 6e64 2065 7870 6f73 6564 2062 7920   and exposed by 
+00002290: 4465 6c66 696e 6f2e 2053 6565 205b 6064  Delfino. See [`d
+000022a0: 656c 6669 6e6f 2d64 656d 6f60 5d28 6874  elfino-demo`](ht
+000022b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000022c0: 2f72 6164 656b 6c61 742f 6465 6c66 696e  /radeklat/delfin
+000022d0: 6f2d 6465 6d6f 2920 666f 7220 6120 6d69  o-demo) for a mi
+000022e0: 6e69 6d61 6c20 706c 7567 696e 2c20 7768  nimal plugin, wh
+000022f0: 6963 6820 7072 6f76 6964 6520 6120 6064  ich provide a `d
+00002300: 656d 6f60 2063 6f6d 6d61 6e64 2070 7269  emo` command pri
+00002310: 6e74 696e 6720 6f75 7420 6120 6d65 7373  nting out a mess
+00002320: 6167 652e 0a0a 4578 6973 7469 6e67 2070  age...Existing p
+00002330: 6c75 6769 6e73 3a0a 0a7c 2050 6c75 6769  lugins:..| Plugi
+00002340: 6e20 6e61 6d65 2020 2020 2020 2020 2020  n name          
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002370: 2020 2020 2020 2020 7c20 4465 7363 7269          | Descri
+00002380: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000023e0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+000023f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a  --------------|:
+00002420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002480: 2d2d 2d7c 0a7c 205b 6465 6c66 696e 6f2d  ---|.| [delfino-
+00002490: 6465 6d6f 5d28 6874 7470 733a 2f2f 6769  demo](https://gi
+000024a0: 7468 7562 2e63 6f6d 2f72 6164 656b 6c61  thub.com/radekla
+000024b0: 742f 6465 6c66 696e 6f2d 6465 6d6f 2920  t/delfino-demo) 
+000024c0: 2020 2020 7c20 4120 6d69 6e69 6d61 6c20      | A minimal 
+000024d0: 706c 7567 696e 2065 7861 6d70 6c65 2066  plugin example f
+000024e0: 6f72 2044 656c 6669 6e6f 2e20 436f 6e74  or Delfino. Cont
+000024f0: 6169 6e73 206f 6e65 2063 6f6d 6d61 6e64  ains one command
+00002500: 2070 7269 6e74 696e 6720 6120 6d65 7373   printing a mess
+00002510: 6167 652e 2020 2020 2020 2020 2020 2020  age.            
+00002520: 2020 2020 2020 2020 207c 0a7c 205b 6465           |.| [de
+00002530: 6c66 696e 6f2d 636f 7265 5d28 6874 7470  lfino-core](http
+00002540: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
+00002550: 6164 656b 6c61 742f 6465 6c66 696e 6f2d  adeklat/delfino-
+00002560: 636f 7265 2920 2020 2020 7c20 436f 6d6d  core)     | Comm
+00002570: 616e 6473 2077 7261 7070 696e 6720 746f  ands wrapping to
+00002580: 6f6c 7320 7573 6564 2064 7572 696e 6720  ols used during 
+00002590: 6576 6572 7920 6461 7920 6465 7665 6c6f  every day develo
+000025a0: 706d 656e 7420 286c 696e 7469 6e67 2c20  pment (linting, 
+000025b0: 7465 7374 696e 672c 2064 6570 656e 6465  testing, depende
+000025c0: 6e63 6965 7320 7570 6461 7465 292e 207c  ncies update). |
+000025d0: 0a7c 205b 6465 6c66 696e 6f2d 646f 636b  .| [delfino-dock
+000025e0: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
+000025f0: 7562 2e63 6f6d 2f72 6164 656b 6c61 742f  ub.com/radeklat/
+00002600: 6465 6c66 696e 6f2d 646f 636b 6572 2920  delfino-docker) 
+00002610: 7c20 446f 636b 6572 2062 7569 6c64 2068  | Docker build h
+00002620: 656c 7065 7220 7363 7269 7074 2e20 2020  elper script.   
+00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002670: 2020 2020 207c 0a0a 2323 2045 6e61 626c       |..## Enabl
+00002680: 696e 6720 6120 706c 7567 696e 0a0a 466f  ing a plugin..Fo
+00002690: 7220 7365 6375 7269 7479 2072 6561 736f  r security reaso
+000026a0: 6e73 2c20 706c 7567 696e 7320 6172 6520  ns, plugins are 
+000026b0: 6469 7361 626c 6564 2062 7920 6465 6661  disabled by defa
+000026c0: 756c 742e 2054 6f20 656e 6162 6c65 2061  ult. To enable a
+000026d0: 2070 6c75 6769 6e2c 2079 6f75 2068 6176   plugin, you hav
+000026e0: 6520 746f 2069 6e63 6c75 6465 2069 7420  e to include it 
+000026f0: 696e 2074 6865 2060 7079 7072 6f6a 6563  in the `pyprojec
+00002700: 742e 746f 6d6c 6020 6669 6c65 3a0a 0a60  t.toml` file:..`
+00002710: 6060 746f 6d6c 0a5b 746f 6f6c 2e64 656c  ``toml.[tool.del
+00002720: 6669 6e6f 2e70 6c75 6769 6e73 2e3c 504c  fino.plugins.<PL
+00002730: 5547 494e 5f4e 414d 453e 5d0a 6060 600a  UGIN_NAME>].```.
+00002740: 0a23 2320 456e 6162 6c69 6e67 2f64 6973  .## Enabling/dis
+00002750: 6162 6c69 6e67 2063 6f6d 6d61 6e64 730a  abling commands.
+00002760: 0a42 7920 6465 6661 756c 742c 2061 6c6c  .By default, all
+00002770: 2063 6f6d 6d61 6e64 7320 6172 6520 656e   commands are en
+00002780: 6162 6c65 642e 2055 7365 2060 656e 6162  abled. Use `enab
+00002790: 6c65 5f63 6f6d 6d61 6e64 7360 206f 7220  le_commands` or 
+000027a0: 6064 6973 6162 6c65 5f63 6f6d 6d61 6e64  `disable_command
+000027b0: 7360 2020 746f 2073 686f 7720 6f6e 6c79  s`  to show only
+000027c0: 2061 2073 7562 7365 7420 6f66 2063 6f6d   a subset of com
+000027d0: 6d61 6e64 732e 2049 6620 626f 7468 2075  mands. If both u
+000027e0: 7365 642c 2064 6973 6162 6c65 6420 636f  sed, disabled co
+000027f0: 6d6d 616e 6473 2061 7265 2073 7562 7472  mmands are subtr
+00002800: 6163 7465 6420 6672 6f6d 2074 6865 2073  acted from the s
+00002810: 6574 206f 6620 656e 6162 6c65 6420 636f  et of enabled co
+00002820: 6d6d 616e 6473 2e0a 0a60 6060 746f 6d6c  mmands...```toml
+00002830: 0a23 205b 746f 6f6c 2e64 656c 6669 6e6f  .# [tool.delfino
+00002840: 2e70 6c75 6769 6e73 2e3c 504c 5547 494e  .plugins.<PLUGIN
+00002850: 5f4e 414d 455f 413e 5d0a 2320 656e 6162  _NAME_A>].# enab
+00002860: 6c65 5f63 6f6d 6d61 6e64 7320 3d20 5b3c  le_commands = [<
+00002870: 434f 4d4d 414e 445f 4e41 4d45 3e5d 0a23  COMMAND_NAME>].#
+00002880: 2064 6973 6162 6c65 5f63 6f6d 6d61 6e64   disable_command
+00002890: 7320 3d20 5b3c 434f 4d4d 414e 445f 4e41  s = [<COMMAND_NA
+000028a0: 4d45 3e5d 0a0a 2320 5b74 6f6f 6c2e 6465  ME>]..# [tool.de
+000028b0: 6c66 696e 6f2e 706c 7567 696e 732e 3c50  lfino.plugins.<P
+000028c0: 4c55 4749 4e5f 4e41 4d45 5f42 3e5d 0a23  LUGIN_NAME_B>].#
+000028d0: 2065 6e61 626c 655f 636f 6d6d 616e 6473   enable_commands
+000028e0: 203d 205b 3c43 4f4d 4d41 4e44 5f4e 414d   = [<COMMAND_NAM
+000028f0: 453e 5d0a 2320 6469 7361 626c 655f 636f  E>].# disable_co
+00002900: 6d6d 616e 6473 203d 205b 3c43 4f4d 4d41  mmands = [<COMMA
+00002910: 4e44 5f4e 414d 453e 5d0a 6060 600a 0a23  ND_NAME>].```..#
+00002920: 2041 6476 616e 6365 6420 7573 6167 650a   Advanced usage.
+00002930: 0a3c 212d 2d0a 2323 2041 6476 616e 6365  .<!--.## Advance
+00002940: 6420 436f 6d6d 616e 640a 0a44 656c 6669  d Command..Delfi
+00002950: 6e6f 2061 6464 7320 6f70 7469 6f6e 616c  no adds optional
+00002960: 2062 6974 7320 6f66 2066 756e 6374 696f   bits of functio
+00002970: 6e61 6c69 7479 206f 6e20 746f 7020 6f66  nality on top of
+00002980: 2043 6c69 636b 2e20 5468 6520 666f 6c6c   Click. The foll
+00002990: 6f77 696e 6720 6578 616d 706c 6520 6465  owing example de
+000029a0: 6d6f 6e73 7472 6174 6573 2073 6f6d 6520  monstrates some 
+000029b0: 6f66 2074 686f 7365 3a0a 0a60 6060 7079  of those:..```py
+000029c0: 7468 6f6e 0a23 2063 6f6d 6d61 6e64 732f  thon.# commands/
+000029d0: 5f5f 696e 6974 5f5f 2e70 790a 0a69 6d70  __init__.py..imp
+000029e0: 6f72 7420 636c 6963 6b0a 0a66 726f 6d20  ort click..from 
+000029f0: 6465 6c66 696e 6f2e 636f 6e74 6578 7473  delfino.contexts
+00002a00: 2069 6d70 6f72 7420 7061 7373 5f61 7070   import pass_app
+00002a10: 5f63 6f6e 7465 7874 2c20 4170 7043 6f6e  _context, AppCon
+00002a20: 7465 7874 0a66 726f 6d20 6465 6c66 696e  text.from delfin
+00002a30: 6f2e 7661 6c69 6461 7469 6f6e 2069 6d70  o.validation imp
+00002a40: 6f72 7420 6173 7365 7274 5f70 6970 5f70  ort assert_pip_p
+00002a50: 6163 6b61 6765 5f69 6e73 7461 6c6c 6564  ackage_installed
+00002a60: 2c20 7079 7072 6f6a 6563 745f 746f 6d6c  , pyproject_toml
+00002a70: 5f6b 6579 5f6d 6973 7369 6e67 0a0a 4063  _key_missing..@c
+00002a80: 6c69 636b 2e63 6f6d 6d61 6e64 2829 0a23  lick.command().#
+00002a90: 2054 6865 2060 7061 7373 5f61 7070 5f63   The `pass_app_c
+00002aa0: 6f6e 7465 7874 6020 6465 636f 7261 746f  ontext` decorato
+00002ab0: 7220 6164 6473 2060 4170 7043 6f6e 7465  r adds `AppConte
+00002ac0: 7874 6020 6173 2074 6865 2066 6972 7374  xt` as the first
+00002ad0: 2070 6172 616d 6574 6572 2e0a 4070 6173   parameter..@pas
+00002ae0: 735f 6170 705f 636f 6e74 6578 740a 6465  s_app_context.de
+00002af0: 6620 636f 6d6d 616e 645f 7465 7374 2861  f command_test(a
+00002b00: 7070 5f63 6f6e 7465 7874 3a20 4170 7043  pp_context: AppC
+00002b10: 6f6e 7465 7874 293a 0a20 2020 2222 2254  ontext):.   """T
+00002b20: 6573 7473 2063 6f6d 6d61 6e64 7320 706c  ests commands pl
+00002b30: 6163 6564 2069 6e20 7468 6520 6063 6f6d  aced in the `com
+00002b40: 6d61 6e64 7360 2066 6f6c 6465 7220 6172  mands` folder ar
+00002b50: 6520 6c6f 6164 6564 2e22 2222 0a20 2020  e loaded.""".   
+00002b60: 2320 5465 7374 206f 7074 696f 6e61 6c20  # Test optional 
+00002b70: 6465 7065 6e64 656e 6369 6573 2e20 416e  dependencies. An
+00002b80: 7920 6661 696c 696e 6720 6173 7365 7274  y failing assert
+00002b90: 696f 6e20 7769 6c6c 2062 6520 7072 696e  ion will be prin
+00002ba0: 7465 6420 6173 3a0a 2020 2023 2043 6f6d  ted as:.   # Com
+00002bb0: 6d61 6e64 2027 3c4e 414d 453e 2720 6973  mand '<NAME>' is
+00002bc0: 206d 6973 636f 6e66 6967 7572 6564 2e20   misconfigured. 
+00002bd0: 3c41 5353 4552 5449 4f4e 2045 5252 4f52  <ASSERTION ERROR
+00002be0: 204d 4553 5341 4745 3e0a 2020 2061 7373   MESSAGE>.   ass
+00002bf0: 6572 745f 7069 705f 7061 636b 6167 655f  ert_pip_package_
+00002c00: 696e 7374 616c 6c65 6428 2264 656c 6669  installed("delfi
+00002c10: 6e6f 2229 0a0a 2020 2023 2041 7070 436f  no")..   # AppCo
+00002c20: 6e74 6578 7420 636f 6e74 6169 6e20 6120  ntext contain a 
+00002c30: 7061 7273 6564 2060 7079 7072 6f6a 6563  parsed `pyprojec
+00002c40: 742e 746f 6d6c 6020 6669 6c65 2e0a 2020  t.toml` file..  
+00002c50: 2023 2043 6f6d 6d61 6e64 7320 6361 6e20   # Commands can 
+00002c60: 6164 6420 7468 6569 7220 636f 6e66 6967  add their config
+00002c70: 2075 6e64 6572 2060 5b74 6f6f 6c2e 6465   under `[tool.de
+00002c80: 6c66 696e 6f2e 636f 6d6d 616e 6473 2e3c  lfino.commands.<
+00002c90: 434f 4d4d 414e 445f 4e41 4d45 3e5d 602e  COMMAND_NAME>]`.
+00002ca0: 0a20 2020 6173 7365 7274 2022 636f 6d6d  .   assert "comm
+00002cb0: 616e 645f 7465 7374 2220 696e 2061 7070  and_test" in app
+00002cc0: 5f63 6f6e 7465 7874 2e70 7970 726f 6a65  _context.pyproje
+00002cd0: 6374 5f74 6f6d 6c2e 746f 6f6c 2e64 656c  ct_toml.tool.del
+00002ce0: 6669 6e6f 2e63 6f6d 6d61 6e64 732c 205c  fino.commands, \
+00002cf0: 0a20 2020 2020 2020 7079 7072 6f6a 6563  .       pyprojec
+00002d00: 745f 746f 6d6c 5f6b 6579 5f6d 6973 7369  t_toml_key_missi
+00002d10: 6e67 2822 746f 6f6c 2e64 656c 6669 6e6f  ng("tool.delfino
+00002d20: 2e63 6f6d 6d61 6e64 732e 636f 6d6d 616e  .commands.comman
+00002d30: 645f 7465 7374 2229 0a0a 2020 2070 7269  d_test")..   pri
+00002d40: 6e74 2861 7070 5f63 6f6e 7465 7874 2e70  nt(app_context.p
+00002d50: 7970 726f 6a65 6374 5f74 6f6d 6c2e 746f  yproject_toml.to
+00002d60: 6f6c 2e64 656c 6669 6e6f 2e63 6f6d 6d61  ol.delfino.comma
+00002d70: 6e64 735b 2263 6f6d 6d61 6e64 2d74 6573  nds["command-tes
+00002d80: 7422 5d29 0a60 6060 0a2d 2d3e 0a0a 2323  t"]).```.-->..##
+00002d90: 2041 7574 6f2d 636f 6d70 6c65 7469 6f6e   Auto-completion
+00002da0: 0a0a 596f 7520 6361 6e20 6569 7468 6572  ..You can either
+00002db0: 2061 7474 656d 7074 2074 6f20 696e 7374   attempt to inst
+00002dc0: 616c 6c20 636f 6d70 6c65 7469 6f6e 7320  all completions 
+00002dd0: 6175 746f 6d61 7469 6361 6c6c 7920 7769  automatically wi
+00002de0: 7468 3a0a 0a60 6060 7368 656c 6c20 7363  th:..```shell sc
+00002df0: 7269 7074 0a64 656c 6669 6e6f 202d 2d69  ript.delfino --i
+00002e00: 6e73 7461 6c6c 2d63 6f6d 706c 6574 696f  nstall-completio
+00002e10: 6e0a 6060 600a 0a6f 7220 6765 6e65 7261  n.```..or genera
+00002e20: 7465 2069 7420 7769 7468 3a0a 0a60 6060  te it with:..```
+00002e30: 7368 656c 6c20 7363 7269 7074 0a64 656c  shell script.del
+00002e40: 6669 6e6f 202d 2d73 686f 772d 636f 6d70  fino --show-comp
+00002e50: 6c65 7469 6f6e 0a60 6060 0a0a 616e 6420  letion.```..and 
+00002e60: 6d61 6e75 616c 6c79 2070 7574 2069 7420  manually put it 
+00002e70: 696e 2074 6865 2072 656c 6576 616e 7420  in the relevant 
+00002e80: 5243 2066 696c 652e 0a0a 5468 6520 6175  RC file...The au
+00002e90: 746f 2d63 6f6d 706c 6574 696f 6e20 696d  to-completion im
+00002ea0: 706c 656d 656e 7461 7469 6f6e 2069 7320  plementation is 
+00002eb0: 6479 6e61 6d69 6320 736f 2074 6861 7420  dynamic so that 
+00002ec0: 6576 6572 7920 7469 6d65 2069 7420 6973  every time it is
+00002ed0: 2069 6e76 6f6b 6564 2c20 6974 2075 7365   invoked, it use
+00002ee0: 7320 7468 6520 6375 7272 656e 7420 7072  s the current pr
+00002ef0: 6f6a 6563 742e 2045 6163 6820 7072 6f6a  oject. Each proj
+00002f00: 6563 7420 6361 6e20 6861 7665 2064 6966  ect can have dif
+00002f10: 6665 7265 6e74 2063 6f6d 6d61 6e64 7320  ferent commands 
+00002f20: 6f72 2064 6973 6162 6c65 2063 6572 7461  or disable certa
+00002f30: 696e 2063 6f6d 6d61 6e64 7320 6974 2064  in commands it d
+00002f40: 6f65 736e 2774 2075 7365 2e20 416e 6420  oesn't use. And 
+00002f50: 6479 6e61 6d69 6320 6175 746f 2d63 6f6d  dynamic auto-com
+00002f60: 706c 6574 696f 6e20 6d61 6b65 7320 7375  pletion makes su
+00002f70: 7265 206f 6e6c 7920 7468 6520 6375 7272  re only the curr
+00002f80: 656e 746c 7920 6176 6169 6c61 626c 6520  ently available 
+00002f90: 636f 6d6d 616e 6473 2077 696c 6c20 6265  commands will be
+00002fa0: 2073 7567 6765 7374 6564 2e0a 0a54 6865   suggested...The
+00002fb0: 2064 6f77 6e73 6964 6520 6f66 2074 6869   downside of thi
+00002fc0: 7320 6170 7072 6f61 6368 2069 7320 7468  s approach is th
+00002fd0: 6174 2065 7661 6c75 6174 696e 6720 7768  at evaluating wh
+00002fe0: 6174 2069 7320 6176 6169 6c61 626c 6520  at is available 
+00002ff0: 6561 6368 2074 696d 6520 6973 2073 6c6f  each time is slo
+00003000: 7765 7220 7468 616e 2061 2073 7461 7469  wer than a stati
+00003010: 6320 6c69 7374 206f 6620 636f 6d6d 616e  c list of comman
+00003020: 6473 2e0a 0a23 2320 5275 6e6e 696e 6720  ds...## Running 
+00003030: 6578 7465 726e 616c 2070 726f 6772 616d  external program
+00003040: 730a 0a49 7420 6973 2075 7020 746f 2079  s..It is up to y
+00003050: 6f75 2068 6f77 2079 6f75 2077 616e 7420  ou how you want 
+00003060: 746f 2065 7865 6375 7465 2065 7874 6572  to execute exter
+00003070: 6e61 6c20 7072 6f63 6573 7365 7320 6173  nal processes as
+00003080: 2070 6172 7420 6f66 2063 6f6d 6d61 6e64   part of command
+00003090: 7320 2869 6620 796f 7520 6e65 6564 2074  s (if you need t
+000030a0: 6f20 6174 2061 6c6c 292e 2041 2063 6f6d  o at all). A com
+000030b0: 6d6f 6e20 7761 7920 696e 2050 7974 686f  mon way in Pytho
+000030c0: 6e20 6973 2074 6f20 7573 6520 6073 7562  n is to use `sub
+000030d0: 7072 6f63 6573 732e 7275 6e60 2e20 4465  process.run`. De
+000030e0: 6c66 696e 6f20 636f 6d65 7320 7769 7468  lfino comes with
+000030f0: 2069 7473 206f 776e 205b 6072 756e 6020   its own [`run` 
+00003100: 696d 706c 656d 656e 7461 7469 6f6e 5d28  implementation](
+00003110: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003120: 6f6d 2f72 6164 656b 6c61 742f 6465 6c66  om/radeklat/delf
+00003130: 696e 6f2f 626c 6f62 2f6d 6169 6e2f 7372  ino/blob/main/sr
+00003140: 632f 6465 6c66 696e 6f2f 6578 6563 7574  c/delfino/execut
+00003150: 696f 6e2e 7079 234c 3934 292c 2077 6869  ion.py#L94), whi
+00003160: 6368 2077 7261 7073 2061 6e64 2073 696d  ch wraps and sim
+00003170: 706c 6966 6965 7320 6073 7562 7072 6f63  plifies `subproc
+00003180: 6573 732e 7275 6e60 2066 6f72 2074 6865  ess.run` for the
+00003190: 206d 6f73 7420 636f 6d6d 6f6e 2075 7365   most common use
+000031a0: 2063 6173 6573 3a0a 0a2d 204e 6f72 6d61   cases:..- Norma
+000031b0: 6c69 7a69 6e67 2060 7375 6270 726f 6365  lizing `subproce
+000031c0: 7373 2e72 756e 6020 6172 6775 6d65 6e74  ss.run` argument
+000031d0: 7320 2d20 796f 7520 6361 6e20 7061 7373  s - you can pass
+000031e0: 2069 6e20 6569 7468 6572 2061 2073 7472   in either a str
+000031f0: 696e 6720 6f72 2061 206c 6973 742e 2045  ing or a list. E
+00003200: 6974 6865 7220 7761 792c 2060 7375 6270  ither way, `subp
+00003210: 726f 6365 7373 2e72 756e 6020 7769 6c6c  rocess.run` will
+00003220: 2062 6520 6578 6563 7574 6564 2063 6f72   be executed cor
+00003230: 7265 6374 6c79 2e0a 2d20 4861 6e64 6c69  rectly..- Handli
+00003240: 6e67 2065 7272 6f72 7320 6672 6f6d 2074  ng errors from t
+00003250: 6865 2065 7865 6375 7469 6f6e 2076 6961  he execution via
+00003260: 2074 6865 2060 6f6e 5f65 7272 6f72 6020   the `on_error` 
+00003270: 6172 6775 6d65 6e74 2e20 4769 7669 6e67  argument. Giving
+00003280: 2074 6865 206f 7074 696f 6e20 746f 2065   the option to e
+00003290: 6974 6865 7220 6967 6e6f 7265 2074 6865  ither ignore the
+000032a0: 2065 7272 6f72 7320 616e 6420 636f 6e74   errors and cont
+000032b0: 696e 7565 2028 6050 4153 5360 292c 206e  inue (`PASS`), n
+000032c0: 6f74 2063 6f6e 7469 6e75 6520 616e 6420  ot continue and 
+000032d0: 636c 6561 6e20 6578 6974 2028 6045 5849  clean exit (`EXI
+000032e0: 5460 2920 6f72 206e 6f74 2063 6f6e 7469  T`) or not conti
+000032f0: 6e75 6520 616e 6420 6162 6f72 7420 7769  nue and abort wi
+00003300: 7468 2065 7272 6f72 2063 6f64 6520 2860  th error code (`
+00003310: 4142 4f52 5460 292e 0a2d 2053 6574 7469  ABORT`)..- Setti
+00003320: 6e67 2065 6e76 6972 6f6e 6d65 6e74 2076  ng environment v
+00003330: 6172 6961 626c 6573 2e0a 2d20 4c6f 6767  ariables..- Logg
+00003340: 696e 6720 7768 6174 2069 7320 6265 696e  ing what is bein
+00003350: 6720 6578 6563 7574 6564 2069 6e20 7468  g executed in th
+00003360: 6520 6465 6275 6720 6c65 7665 6c2e 0a0a  e debug level...
+00003370: 4578 616d 706c 653a 0a0a 6060 6070 7974  Example:..```pyt
+00003380: 686f 6e0a 2320 636f 6d6d 616e 6473 2f5f  hon.# commands/_
+00003390: 5f69 6e69 745f 5f2e 7079 0a0a 696d 706f  _init__.py..impo
+000033a0: 7274 2063 6c69 636b 0a66 726f 6d20 6465  rt click.from de
+000033b0: 6c66 696e 6f2e 6578 6563 7574 696f 6e20  lfino.execution 
+000033c0: 696d 706f 7274 2072 756e 2c20 4f6e 4572  import run, OnEr
+000033d0: 726f 720a 0a40 636c 6963 6b2e 636f 6d6d  ror..@click.comm
+000033e0: 616e 6428 290a 6465 6620 7465 7374 2829  and().def test()
+000033f0: 3a0a 2020 2020 7275 6e28 2270 7974 6573  :.    run("pytes
+00003400: 7420 7465 7374 7322 2c20 6f6e 5f65 7272  t tests", on_err
+00003410: 6f72 3d4f 6e45 7272 6f72 2e41 424f 5254  or=OnError.ABORT
+00003420: 290a 6060 600a 0a23 2320 4f70 7469 6f6e  ).```..## Option
+00003430: 616c 2064 6570 656e 6465 6e63 6965 730a  al dependencies.
+00003440: 0a49 6620 796f 7520 7075 7420 7365 7665  .If you put seve
+00003450: 7261 6c20 636f 6d6d 616e 6473 2069 6e74  ral commands int
+00003460: 6f20 6f6e 6520 5b70 6c75 6769 6e5d 2823  o one [plugin](#
+00003470: 706c 7567 696e 7329 2c20 796f 7520 6361  plugins), you ca
+00003480: 6e20 6d61 6b65 2073 6f6d 6520 6465 7065  n make some depe
+00003490: 6e64 656e 6369 6573 206f 6620 736f 6d65  ndencies of some
+000034a0: 2063 6f6d 6d61 6e64 7320 5b6f 7074 696f   commands [optio
+000034b0: 6e61 6c5d 2868 7474 7073 3a2f 2f70 7974  nal](https://pyt
+000034c0: 686f 6e2d 706f 6574 7279 2e6f 7267 2f64  hon-poetry.org/d
+000034d0: 6f63 732f 7079 7072 6f6a 6563 7423 6578  ocs/pyproject#ex
+000034e0: 7472 6173 292e 2054 6869 7320 6973 2075  tras). This is u
+000034f0: 7365 6675 6c20 7768 656e 2061 2063 6f6d  seful when a com
+00003500: 6d61 6e64 2069 7320 6e6f 7420 616c 7761  mand is not alwa
+00003510: 7973 2075 7365 642c 2061 6e64 2079 6f75  ys used, and you
+00003520: 2064 6f6e 2774 2077 616e 7420 746f 2069   don't want to i
+00003530: 6e73 7461 6c6c 2075 6e6e 6563 6573 7361  nstall unnecessa
+00003540: 7279 2064 6570 656e 6465 6e63 6965 732e  ry dependencies.
+00003550: 2049 6e73 7465 6164 2c20 796f 7520 6361   Instead, you ca
+00003560: 6e20 6368 6563 6b20 6966 2061 2064 6570  n check if a dep
+00003570: 656e 6465 6e63 7920 6973 2069 6e73 7461  endency is insta
+00003580: 6c6c 6564 206f 6e6c 7920 7768 656e 2074  lled only when t
+00003590: 6865 2063 6f6d 6d61 6e64 2069 7320 6578  he command is ex
+000035a0: 6563 7574 6564 2077 6974 6820 6064 656c  ecuted with `del
+000035b0: 6669 6e6f 2e76 616c 6964 6174 696f 6e2e  fino.validation.
+000035c0: 6173 7365 7274 5f70 6970 5f70 6163 6b61  assert_pip_packa
+000035d0: 6765 5f69 6e73 7461 6c6c 6564 603a 0a0a  ge_installed`:..
+000035e0: 6060 6070 7974 686f 6e0a 2320 636f 6d6d  ```python.# comm
+000035f0: 616e 6473 2f5f 5f69 6e69 745f 5f2e 7079  ands/__init__.py
+00003600: 0a0a 696d 706f 7274 2063 6c69 636b 0a66  ..import click.f
+00003610: 726f 6d20 6465 6c66 696e 6f2e 7661 6c69  rom delfino.vali
+00003620: 6461 7469 6f6e 2069 6d70 6f72 7420 6173  dation import as
+00003630: 7365 7274 5f70 6970 5f70 6163 6b61 6765  sert_pip_package
+00003640: 5f69 6e73 7461 6c6c 6564 0a0a 7472 793a  _installed..try:
+00003650: 0a20 2020 2066 726f 6d20 6769 7420 696d  .    from git im
+00003660: 706f 7274 2052 6570 6f0a 6578 6365 7074  port Repo.except
+00003670: 2049 6d70 6f72 7445 7272 6f72 3a0a 2020   ImportError:.  
+00003680: 2020 7061 7373 0a0a 4063 6c69 636b 2e63    pass..@click.c
+00003690: 6f6d 6d61 6e64 2829 0a64 6566 2067 6974  ommand().def git
+000036a0: 5f61 6374 6976 655f 6272 616e 6368 2829  _active_branch()
+000036b0: 3a0a 2020 2020 6173 7365 7274 5f70 6970  :.    assert_pip
+000036c0: 5f70 6163 6b61 6765 5f69 6e73 7461 6c6c  _package_install
+000036d0: 6564 2822 6769 7470 7974 686f 6e22 290a  ed("gitpython").
+000036e0: 2020 2020 7072 696e 7428 5265 706f 2822      print(Repo("
+000036f0: 2e22 292e 6163 7469 7665 5f62 7261 6e63  .").active_branc
+00003700: 6829 0a60 6060 0a0a 496e 2074 6865 2065  h).```..In the e
+00003710: 7861 6d70 6c65 2061 626f 7665 2c20 6966  xample above, if
+00003720: 2060 6769 7470 7974 686f 6e60 2069 7320   `gitpython` is 
+00003730: 6e6f 7420 696e 7374 616c 6c65 642c 2064  not installed, d
+00003740: 656c 6669 6e6f 2077 696c 6c20 7368 6f77  elfino will show
+00003750: 2074 6865 2063 6f6d 6d61 6e64 2062 7574   the command but
+00003760: 2077 696c 6c20 6661 696c 2077 6974 6820   will fail with 
+00003770: 7375 6767 6573 7469 6f6e 2074 6f20 696e  suggestion to in
+00003780: 7374 616c 6c20 6067 6974 7079 7468 6f6e  stall `gitpython
+00003790: 6020 6f6e 6c79 2077 6865 6e20 7468 6520  ` only when the 
+000037a0: 636f 6d6d 616e 6420 6973 2065 7865 6375  command is execu
+000037b0: 7465 642e 2059 6f75 2063 616e 2061 6c73  ted. You can als
+000037c0: 6f20 6164 6420 6067 6974 5f61 6374 6976  o add `git_activ
+000037d0: 655f 6272 616e 6368 6020 696e 746f 205b  e_branch` into [
+000037e0: 6064 6973 6162 6c65 5f63 6f6d 6d61 6e64  `disable_command
+000037f0: 7360 2063 6f6e 6669 675d 2823 656e 6162  s` config](#enab
+00003800: 6c69 6e67 6469 7361 626c 696e 672d 636f  lingdisabling-co
+00003810: 6d6d 616e 6473 2920 696e 2070 6c61 6365  mmands) in place
+00003820: 7320 7768 6572 6520 796f 7520 646f 6e27  s where you don'
+00003830: 7420 696e 7465 6e64 2074 6f20 7573 6520  t intend to use 
+00003840: 6974 2e0a 0a54 6869 7320 7761 7920 796f  it...This way yo
+00003850: 7520 6361 6e20 6772 6561 746c 7920 7265  u can greatly re
+00003860: 6475 6365 2074 6865 206e 756d 6265 7220  duce the number 
+00003870: 6f66 2064 6570 656e 6465 6e63 6965 7320  of dependencies 
+00003880: 6120 706c 7567 696e 2062 7269 6e67 7320  a plugin brings 
+00003890: 696e 746f 2061 2070 726f 6a65 6374 2077  into a project w
+000038a0: 6974 686f 7574 2061 206e 6565 6420 746f  ithout a need to
+000038b0: 2068 6176 6520 6d61 6e79 2073 6d61 6c6c   have many small
+000038c0: 2070 6c75 6769 6e73 2e0a 0a23 2320 5072   plugins...## Pr
+000038d0: 6f6a 6563 7420 7365 7474 696e 6773 0a0a  oject settings..
+000038e0: 596f 7520 6361 6e20 7374 6f72 6520 616e  You can store an
+000038f0: 2061 7262 6974 7261 7279 206f 626a 6563   arbitrary objec
+00003900: 7420 696e 2074 6865 2043 6c69 636b 2063  t in the Click c
+00003910: 6f6e 7465 7874 2061 7320 5b60 636c 6963  ontext as [`clic
+00003920: 6b2e 436f 6e74 6578 742e 6f62 6a60 5d28  k.Context.obj`](
+00003930: 6874 7470 733a 2f2f 636c 6963 6b2e 7061  https://click.pa
+00003940: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
+00003950: 6d2f 6170 692f 2363 6c69 636b 2e43 6f6e  m/api/#click.Con
+00003960: 7465 7874 2e6f 626a 292e 2044 656c 6669  text.obj). Delfi
+00003970: 6e6f 2075 7469 6c69 7a65 7320 7468 6973  no utilizes this
+00003980: 206f 626a 6563 7420 746f 2073 746f 7265   object to store
+00003990: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
+000039a0: 5b60 4170 7043 6f6e 7465 7874 605d 2868  [`AppContext`](h
+000039b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000039c0: 6d2f 7261 6465 6b6c 6174 2f64 656c 6669  m/radeklat/delfi
+000039d0: 6e6f 2f62 6c6f 622f 6d61 696e 2f73 7263  no/blob/main/src
+000039e0: 2f64 656c 6669 6e6f 2f6d 6f64 656c 732f  /delfino/models/
+000039f0: 6170 705f 636f 6e74 6578 742e 7079 292c  app_context.py),
+00003a00: 2077 6869 6368 2070 726f 7669 6465 7320   which provides 
+00003a10: 6163 6365 7373 2074 6f20 7072 6f6a 6563  access to projec
+00003a20: 7420 7265 6c61 7465 6420 696e 666f 726d  t related inform
+00003a30: 6174 696f 6e2e 2049 6620 796f 7520 6e65  ation. If you ne
+00003a40: 6564 2074 6f2c 2079 6f75 2063 616e 2073  ed to, you can s
+00003a50: 7469 6c6c 2061 7474 6163 6820 6172 6269  till attach arbi
+00003a60: 7472 6172 7920 6174 7472 6962 7574 6573  trary attributes
+00003a70: 2074 6f20 7468 6973 206f 626a 6563 7420   to this object 
+00003a80: 6c61 7465 722e 0a0a 596f 7520 6361 6e20  later...You can 
+00003a90: 7061 7373 2074 6869 7320 6f62 6a65 6374  pass this object
+00003aa0: 2074 6f20 796f 7572 2063 6f6d 6d61 6e64   to your command
+00003ab0: 7320 6279 2064 6563 6f72 6174 696e 6720  s by decorating 
+00003ac0: 7468 656d 2077 6974 6820 5b60 636c 6963  them with [`clic
+00003ad0: 6b2e 7061 7373 5f6f 626a 605d 2868 7474  k.pass_obj`](htt
+00003ae0: 7073 3a2f 2f63 6c69 636b 2e70 616c 6c65  ps://click.palle
+00003af0: 7473 7072 6f6a 6563 7473 2e63 6f6d 2f61  tsprojects.com/a
+00003b00: 7069 2f23 636c 6963 6b2e 7061 7373 5f6f  pi/#click.pass_o
+00003b10: 626a 293a 0a0a 6060 6070 7974 686f 6e0a  bj):..```python.
+00003b20: 2320 636f 6d6d 616e 6473 2f5f 5f69 6e69  # commands/__ini
+00003b30: 745f 5f2e 7079 0a0a 696d 706f 7274 2063  t__.py..import c
+00003b40: 6c69 636b 0a66 726f 6d20 6465 6c66 696e  lick.from delfin
+00003b50: 6f2e 6d6f 6465 6c73 2e61 7070 5f63 6f6e  o.models.app_con
+00003b60: 7465 7874 2069 6d70 6f72 7420 4170 7043  text import AppC
+00003b70: 6f6e 7465 7874 0a0a 4063 6c69 636b 2e63  ontext..@click.c
+00003b80: 6f6d 6d61 6e64 2829 0a40 636c 6963 6b2e  ommand().@click.
+00003b90: 7061 7373 5f6f 626a 0a64 6566 2070 7269  pass_obj.def pri
+00003ba0: 6e74 5f61 7070 5f76 6572 7369 6f6e 286f  nt_app_version(o
+00003bb0: 626a 3a20 4170 7043 6f6e 7465 7874 293a  bj: AppContext):
+00003bc0: 0a20 2020 2070 7269 6e74 286f 626a 2e70  .    print(obj.p
+00003bd0: 7970 726f 6a65 6374 5f74 6f6d 6c2e 746f  yproject_toml.to
+00003be0: 6f6c 2e70 6f65 7472 792e 7665 7273 696f  ol.poetry.versio
+00003bf0: 6e29 0a60 6060 0a0a 2323 2050 6c75 6769  n).```..## Plugi
+00003c00: 6e20 7365 7474 696e 6773 0a0a 506c 7567  n settings..Plug
+00003c10: 696e 2073 6574 7469 6e67 7320 6172 6520  in settings are 
+00003c20: 6578 7065 6374 6564 2074 6f20 6c69 7665  expected to live
+00003c30: 2069 6e20 7468 6520 6070 7970 726f 6a65   in the `pyproje
+00003c40: 6374 2e74 6f6d 6c60 2066 696c 652e 2054  ct.toml` file. T
+00003c50: 6f20 7072 6576 656e 7420 6e61 6d69 6e67  o prevent naming
+00003c60: 2063 6f6e 666c 6963 7473 2c20 6561 6368   conflicts, each
+00003c70: 2070 6c75 6769 6e20 6d75 7374 2070 7574   plugin must put
+00003c80: 2069 7473 2073 6574 7469 6e67 7320 756e   its settings un
+00003c90: 6465 7220 6074 6f6f 6c2e 6465 6c66 696e  der `tool.delfin
+00003ca0: 6f2e 706c 7567 696e 732e 3c50 4c55 4749  o.plugins.<PLUGI
+00003cb0: 4e5f 4e41 4d45 3e60 2e20 4974 2061 6c73  N_NAME>`. It als
+00003cc0: 6f20 616c 6c6f 7773 2044 656c 6669 6e6f  o allows Delfino
+00003cd0: 2074 6f20 7061 7373 2074 6865 7365 2073   to pass these s
+00003ce0: 6574 7469 6e67 7320 6469 7265 6374 6c79  ettings directly
+00003cf0: 2074 6f20 636f 6d6d 616e 6473 2066 726f   to commands fro
+00003d00: 6d20 7468 6573 6520 706c 7567 696e 732e  m these plugins.
+00003d10: 0a0a 4465 6c66 696e 6f20 6c6f 6164 732c  ..Delfino loads,
+00003d20: 2070 6172 7365 732c 2076 616c 6964 6174   parses, validat
+00003d30: 6573 2061 6e64 2073 746f 7265 7320 706c  es and stores pl
+00003d40: 7567 696e 2073 6574 7469 6e67 7320 696e  ugin settings in
+00003d50: 205b 6041 7070 436f 6e74 6578 742e 706c   [`AppContext.pl
+00003d60: 7567 696e 5f63 6f6e 6669 6760 5d28 6874  ugin_config`](ht
+00003d70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003d80: 2f72 6164 656b 6c61 742f 6465 6c66 696e  /radeklat/delfin
+00003d90: 6f2f 626c 6f62 2f6d 6169 6e2f 7372 632f  o/blob/main/src/
+00003da0: 6465 6c66 696e 6f2f 6d6f 6465 6c73 2f61  delfino/models/a
+00003db0: 7070 5f63 6f6e 7465 7874 2e70 7929 2e20  pp_context.py). 
+00003dc0: 4966 206e 6f74 2073 7065 6369 6669 6564  If not specified
+00003dd0: 206f 7468 6572 7769 7365 2028 7365 6520   otherwise (see 
+00003de0: 6265 6c6f 7729 2c20 6974 2077 696c 6c20  below), it will 
+00003df0: 6265 2061 6e20 696e 7374 616e 6365 206f  be an instance o
+00003e00: 6620 5b60 506c 7567 696e 436f 6e66 6967  f [`PluginConfig
+00003e10: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+00003e20: 622e 636f 6d2f 7261 6465 6b6c 6174 2f64  b.com/radeklat/d
+00003e30: 656c 6669 6e6f 2f62 6c6f 622f 6d61 696e  elfino/blob/main
+00003e40: 2f73 7263 2f64 656c 6669 6e6f 2f6d 6f64  /src/delfino/mod
+00003e50: 656c 732f 7079 7072 6f6a 6563 745f 746f  els/pyproject_to
+00003e60: 6d6c 2e70 7929 2c20 7769 7468 2061 6e79  ml.py), with any
+00003e70: 2065 7874 7261 206b 6579 7320 756e 7661   extra keys unva
+00003e80: 6c69 6461 7465 6420 616e 6420 696e 204a  lidated and in J
+00003e90: 534f 4e2d 6c69 6b65 2050 7974 686f 6e20  SON-like Python 
+00003ea0: 6f62 6a65 6374 732e 0a0a 596f 7520 6361  objects...You ca
+00003eb0: 6e20 6164 6420 6164 6469 7469 6f6e 616c  n add additional
+00003ec0: 2076 616c 6964 6174 696f 6e20 746f 2079   validation to y
+00003ed0: 6f75 7220 706c 7567 696e 2073 6574 7469  our plugin setti
+00003ee0: 6e67 7320 6279 2073 7562 2d63 6c61 7373  ngs by sub-class
+00003ef0: 696e 6720 7468 6520 6050 6c75 6769 6e43  ing the `PluginC
+00003f00: 6f6e 6669 6760 202c 2064 6566 696e 696e  onfig` , definin
+00003f10: 6720 6578 7065 6374 6564 206b 6579 732c  g expected keys,
+00003f20: 2064 6566 6175 6c74 2076 616c 7565 7320   default values 
+00003f30: 616e 642f 6f72 2076 616c 6964 6174 696f  and/or validatio
+00003f40: 6e2e 2044 656c 6669 6e6f 2075 7469 6c69  n. Delfino utili
+00003f50: 7a65 7320 5b60 7079 6461 6e74 6963 605d  zes [`pydantic`]
+00003f60: 2868 7474 7073 3a2f 2f64 6f63 732e 7079  (https://docs.py
+00003f70: 6461 6e74 6963 2e64 6576 2f29 2074 6f20  dantic.dev/) to 
+00003f80: 6372 6561 7465 2064 6174 6120 636c 6173  create data clas
+00003f90: 7365 732e 0a0a 4465 6c66 696e 6f20 616c  ses...Delfino al
+00003fa0: 736f 206e 6565 6473 2074 6f20 6b6e 6f77  so needs to know
+00003fb0: 2c20 7768 6963 6820 636c 6173 7320 746f  , which class to
+00003fc0: 2075 7365 2066 6f72 2074 6865 2076 616c   use for the val
+00003fd0: 6964 6174 696f 6e2e 2054 6f20 646f 2074  idation. To do t
+00003fe0: 6861 742c 2073 7769 7463 6820 746f 2060  hat, switch to `
+00003ff0: 6465 6c66 696e 6f2e 6465 636f 7261 746f  delfino.decorato
+00004000: 7273 2e70 6173 735f 6170 705f 636f 6e74  rs.pass_app_cont
+00004010: 6578 7460 2069 6e73 7465 6164 206f 6620  ext` instead of 
+00004020: 5b60 636c 6963 6b2e 7061 7373 5f6f 626a  [`click.pass_obj
+00004030: 605d 2868 7474 7073 3a2f 2f63 6c69 636b  `](https://click
+00004040: 2e70 616c 6c65 7473 7072 6f6a 6563 7473  .palletsprojects
+00004050: 2e63 6f6d 2f61 7069 2f23 636c 6963 6b2e  .com/api/#click.
+00004060: 7061 7373 5f6f 626a 293a 0a0a 6060 6074  pass_obj):..```t
+00004070: 6f6d 6c0a 2320 7079 7072 6f6a 6563 742e  oml.# pyproject.
+00004080: 746f 6d6c 0a0a 5b74 6f6f 6c2e 6465 6c66  toml..[tool.delf
+00004090: 696e 6f2e 706c 7567 696e 732e 6465 6c66  ino.plugins.delf
+000040a0: 696e 6f5f 6c6f 6769 6e5f 706c 7567 696e  ino_login_plugin
+000040b0: 5d0a 7573 6572 6e61 6d65 203d 2022 7573  ].username = "us
+000040c0: 6572 220a 6060 600a 0a60 6060 7079 7468  er".```..```pyth
+000040d0: 6f6e 0a23 2063 6f6d 6d61 6e64 732f 5f5f  on.# commands/__
+000040e0: 696e 6974 5f5f 2e70 790a 0a69 6d70 6f72  init__.py..impor
+000040f0: 7420 636c 6963 6b0a 6672 6f6d 2064 656c  t click.from del
+00004100: 6669 6e6f 2e6d 6f64 656c 732e 7079 7072  fino.models.pypr
+00004110: 6f6a 6563 745f 746f 6d6c 2069 6d70 6f72  oject_toml impor
+00004120: 7420 506c 7567 696e 436f 6e66 6967 0a66  t PluginConfig.f
+00004130: 726f 6d20 6465 6c66 696e 6f2e 6d6f 6465  rom delfino.mode
+00004140: 6c73 2e61 7070 5f63 6f6e 7465 7874 2069  ls.app_context i
+00004150: 6d70 6f72 7420 4170 7043 6f6e 7465 7874  mport AppContext
+00004160: 0a66 726f 6d20 6465 6c66 696e 6f2e 6465  .from delfino.de
+00004170: 636f 7261 746f 7273 2069 6d70 6f72 7420  corators import 
+00004180: 7061 7373 5f61 7070 5f63 6f6e 7465 7874  pass_app_context
+00004190: 0a0a 0a63 6c61 7373 204c 6f67 696e 506c  ...class LoginPl
+000041a0: 7567 696e 436f 6e66 6967 2850 6c75 6769  uginConfig(Plugi
+000041b0: 6e43 6f6e 6669 6729 3a0a 2020 2020 6c6f  nConfig):.    lo
+000041c0: 6769 6e3a 2073 7472 0a0a 0a40 636c 6963  gin: str...@clic
+000041d0: 6b2e 636f 6d6d 616e 6428 290a 4070 6173  k.command().@pas
+000041e0: 735f 6170 705f 636f 6e74 6578 7428 4c6f  s_app_context(Lo
+000041f0: 6769 6e50 6c75 6769 6e43 6f6e 6669 6729  ginPluginConfig)
+00004200: 0a64 6566 206c 6f67 696e 2861 7070 5f63  .def login(app_c
+00004210: 6f6e 7465 7874 3a20 4170 7043 6f6e 7465  ontext: AppConte
+00004220: 7874 5b4c 6f67 696e 506c 7567 696e 436f  xt[LoginPluginCo
+00004230: 6e66 6967 5d29 3a0a 2020 2020 7072 696e  nfig]):.    prin
+00004240: 7428 6170 705f 636f 6e74 6578 742e 706c  t(app_context.pl
+00004250: 7567 696e 5f63 6f6e 6669 672e 6c6f 6769  ugin_config.logi
+00004260: 6e29 0a60 6060 0a0a 5468 6520 6041 7070  n).```..The `App
+00004270: 436f 6e74 6578 7460 2063 6c61 7373 2069  Context` class i
+00004280: 7320 6765 6e65 7269 632e 2044 6566 696e  s generic. Defin
+00004290: 696e 6720 7468 6520 6050 6c75 6769 6e43  ing the `PluginC
+000042a0: 6f6e 6669 6754 7970 6560 2028 7375 6368  onfigType` (such
+000042b0: 2061 7320 6041 7070 436f 6e74 6578 745b   as `AppContext[
+000042c0: 4c6f 6769 6e50 6c75 6769 6e43 6f6e 6669  LoginPluginConfi
+000042d0: 675d 6020 696e 2074 6865 2065 7861 6d70  g]` in the examp
+000042e0: 6c65 2061 626f 7665 2920 656e 6162 6c65  le above) enable
+000042f0: 7320 696e 7472 6f73 7065 6374 696f 6e20  s introspection 
+00004300: 616e 6420 7479 7065 2063 6865 636b 732e  and type checks.
+00004310: 0a0a 2323 2050 726f 6a65 6374 2073 7065  ..## Project spe
+00004320: 6369 6669 6320 6f76 6572 7269 6465 730a  cific overrides.
+00004330: 0a49 7420 6973 206c 696b 656c 7920 796f  .It is likely yo
+00004340: 7572 2070 726f 6a65 6374 7320 7769 6c6c  ur projects will
+00004350: 2072 6571 7569 7265 2073 6c69 6768 7420   require slight 
+00004360: 6469 7665 7267 656e 6365 2074 6f20 7468  divergence to th
+00004370: 6520 6465 6661 756c 7473 2079 6f75 2065  e defaults you e
+00004380: 6e63 6f64 6520 696e 2079 6f75 7220 7363  ncode in your sc
+00004390: 7269 7074 732e 2054 6865 2066 6f6c 6c6f  ripts. The follo
+000043a0: 7769 6e67 2073 6563 7469 6f6e 7320 636f  wing sections co
+000043b0: 7665 7220 7468 6520 6d6f 7374 2063 6f6d  ver the most com
+000043c0: 6d6f 6e20 7573 6520 6361 7365 732e 0a0a  mon use cases...
+000043d0: 2323 2320 5061 7373 2d74 6872 6f75 6768  ### Pass-through
+000043e0: 2061 7267 756d 656e 7473 0a0a 596f 7520   arguments..You 
+000043f0: 6361 6e20 7061 7373 2061 6464 6974 696f  can pass additio
+00004400: 6e61 6c20 6172 6775 6d65 6e74 7320 746f  nal arguments to
+00004410: 2064 6f77 6e73 7472 6561 6d20 746f 6f6c   downstream tool
+00004420: 7320 6279 2064 6563 6f72 6174 696e 6720  s by decorating 
+00004430: 636f 6d6d 616e 6473 2077 6974 6820 7468  commands with th
+00004440: 6520 5b60 6465 636f 7261 746f 7273 2e70  e [`decorators.p
+00004450: 6173 735f 6172 6773 605d 2868 7474 7073  ass_args`](https
+00004460: 3a2f 2f67 6974 6875 622e 636f 6d2f 7261  ://github.com/ra
+00004470: 6465 6b6c 6174 2f64 656c 6669 6e6f 2f62  deklat/delfino/b
+00004480: 6c6f 622f 6d61 696e 2f73 7263 2f64 656c  lob/main/src/del
+00004490: 6669 6e6f 2f64 6563 6f72 6174 6f72 732f  fino/decorators/
+000044a0: 7061 7373 5f61 7267 732e 7079 2920 6465  pass_args.py) de
+000044b0: 636f 7261 746f 723a 0a0a 6060 6070 7974  corator:..```pyt
+000044c0: 686f 6e0a 2320 636f 6d6d 616e 6473 2f5f  hon.# commands/_
+000044d0: 5f69 6e69 745f 5f2e 7079 0a0a 6672 6f6d  _init__.py..from
+000044e0: 2074 7970 696e 6720 696d 706f 7274 2054   typing import T
+000044f0: 7570 6c65 0a0a 696d 706f 7274 2063 6c69  uple..import cli
+00004500: 636b 0a66 726f 6d20 6465 6c66 696e 6f2e  ck.from delfino.
+00004510: 6465 636f 7261 746f 7273 2069 6d70 6f72  decorators impor
+00004520: 7420 7061 7373 5f61 7267 730a 6672 6f6d  t pass_args.from
+00004530: 2064 656c 6669 6e6f 2e65 7865 6375 7469   delfino.executi
+00004540: 6f6e 2069 6d70 6f72 7420 7275 6e2c 204f  on import run, O
+00004550: 6e45 7272 6f72 0a0a 4063 6c69 636b 2e63  nError..@click.c
+00004560: 6f6d 6d61 6e64 2829 0a40 7061 7373 5f61  ommand().@pass_a
+00004570: 7267 730a 6465 6620 7465 7374 2870 6173  rgs.def test(pas
+00004580: 7365 645f 6172 6773 3a20 5475 706c 655b  sed_args: Tuple[
+00004590: 7374 722c 202e 2e2e 5d29 3a0a 2020 2020  str, ...]):.    
+000045a0: 7275 6e28 5b22 7079 7465 7374 222c 2022  run(["pytest", "
+000045b0: 7465 7374 7322 2c20 2a70 6173 7365 645f  tests", *passed_
+000045c0: 6172 6773 5d2c 206f 6e5f 6572 726f 723d  args], on_error=
+000045d0: 4f6e 4572 726f 722e 4142 4f52 5429 0a60  OnError.ABORT).`
+000045e0: 6060 0a0a 5468 656e 2061 6464 6974 696f  ``..Then additio
+000045f0: 6e61 6c20 6172 6775 6d65 6e74 7320 6361  nal arguments ca
+00004600: 6e20 6265 2070 6173 7365 6420 6569 7468  n be passed eith
+00004610: 6572 2076 6961 2063 6f6d 6d61 6e64 206c  er via command l
+00004620: 696e 6520 6166 7465 7220 602d 2d60 3a0a  ine after `--`:.
+00004630: 0a60 6060 7368 656c 6c20 7363 7269 7074  .```shell script
+00004640: 0a64 656c 6669 6e6f 2074 6573 7420 2d2d  .delfino test --
+00004650: 202d 2d63 6170 7475 7265 3d6e 6f0a 6060   --capture=no.``
+00004660: 600a 0a4f 7220 7669 6120 636f 6e66 6967  `..Or via config
+00004670: 7572 6174 696f 6e20 696e 2074 6865 2060  uration in the `
+00004680: 7079 7072 6f6a 6563 742e 746f 6d6c 6020  pyproject.toml` 
+00004690: 6669 6c65 3a0a 0a60 6060 746f 6d6c 0a5b  file:..```toml.[
+000046a0: 746f 6f6c 2e64 656c 6669 6e6f 2e70 6c75  tool.delfino.plu
+000046b0: 6769 6e73 2e3c 504c 5547 494e 3e2e 7465  gins.<PLUGIN>.te
+000046c0: 7374 5d0a 7061 7373 5f61 7267 7320 3d20  st].pass_args = 
+000046d0: 5b27 2d2d 6361 7074 7572 653d 6e6f 275d  ['--capture=no']
+000046e0: 0a60 6060 0a0a 4569 7468 6572 2077 6179  .```..Either way
+000046f0: 2c20 626f 7468 2077 696c 6c20 7265 7375  , both will resu
+00004700: 6c74 2069 6e20 6578 6563 7574 696e 6720  lt in executing 
+00004710: 6070 7974 6573 7420 7465 7374 7320 2d2d  `pytest tests --
+00004720: 6361 7074 7572 653d 6e6f 602e 0a0a 2323  capture=no`...##
+00004730: 2320 4669 6c65 7320 6f76 6572 7269 6465  # Files override
+00004740: 0a0a 596f 7520 6361 6e20 6f76 6572 7269  ..You can overri
+00004750: 6465 2066 696c 6573 2070 6173 7365 6420  de files passed 
+00004760: 746f 2064 6f77 6e73 7472 6561 6d20 746f  to downstream to
+00004770: 6f6c 7320 6279 2064 6563 6f72 6174 696e  ols by decoratin
+00004780: 6720 636f 6d6d 616e 6473 2077 6974 6820  g commands with 
+00004790: 7468 6520 5b60 6465 636f 7261 746f 7273  the [`decorators
+000047a0: 2e66 696c 6573 5f66 6f6c 6465 7273 5f6f  .files_folders_o
+000047b0: 7074 696f 6e60 5d28 6874 7470 733a 2f2f  ption`](https://
+000047c0: 6769 7468 7562 2e63 6f6d 2f72 6164 656b  github.com/radek
+000047d0: 6c61 742f 6465 6c66 696e 6f2f 626c 6f62  lat/delfino/blob
+000047e0: 2f6d 6169 6e2f 7372 632f 6465 6c66 696e  /main/src/delfin
+000047f0: 6f2f 6465 636f 7261 746f 7273 2f66 696c  o/decorators/fil
+00004800: 6573 5f66 6f6c 6465 7273 2e70 7929 2064  es_folders.py) d
+00004810: 6563 6f72 6174 6f72 3a0a 0a60 6060 7079  ecorator:..```py
+00004820: 7468 6f6e 0a23 2063 6f6d 6d61 6e64 732f  thon.# commands/
+00004830: 5f5f 696e 6974 5f5f 2e70 790a 0a66 726f  __init__.py..fro
+00004840: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
+00004850: 5475 706c 650a 0a69 6d70 6f72 7420 636c  Tuple..import cl
+00004860: 6963 6b0a 6672 6f6d 2064 656c 6669 6e6f  ick.from delfino
+00004870: 2e64 6563 6f72 6174 6f72 7320 696d 706f  .decorators impo
+00004880: 7274 2066 696c 6573 5f66 6f6c 6465 7273  rt files_folders
+00004890: 5f6f 7074 696f 6e0a 6672 6f6d 2064 656c  _option.from del
+000048a0: 6669 6e6f 2e65 7865 6375 7469 6f6e 2069  fino.execution i
+000048b0: 6d70 6f72 7420 7275 6e2c 204f 6e45 7272  mport run, OnErr
+000048c0: 6f72 0a0a 4063 6c69 636b 2e63 6f6d 6d61  or..@click.comma
+000048d0: 6e64 2829 0a40 6669 6c65 735f 666f 6c64  nd().@files_fold
+000048e0: 6572 735f 6f70 7469 6f6e 0a64 6566 2074  ers_option.def t
+000048f0: 6573 7428 6669 6c65 735f 666f 6c64 6572  est(files_folder
+00004900: 733a 2054 7570 6c65 5b73 7472 2c20 2e2e  s: Tuple[str, ..
+00004910: 2e5d 293a 0a20 2020 2069 6620 6e6f 7420  .]):.    if not 
+00004920: 6669 6c65 735f 666f 6c64 6572 733a 0a20  files_folders:. 
+00004930: 2020 2020 2020 2066 696c 6573 5f66 6f6c         files_fol
+00004940: 6465 7273 203d 2028 2274 6573 7473 2f75  ders = ("tests/u
+00004950: 6e69 7422 2c20 2274 6573 7473 2f69 6e74  nit", "tests/int
+00004960: 6567 7261 7469 6f6e 2229 0a20 2020 2072  egration").    r
+00004970: 756e 285b 2270 7974 6573 7422 2c20 2a66  un(["pytest", *f
+00004980: 696c 6573 5f66 6f6c 6465 7273 5d2c 206f  iles_folders], o
+00004990: 6e5f 6572 726f 723d 4f6e 4572 726f 722e  n_error=OnError.
+000049a0: 4142 4f52 5429 0a60 6060 0a0a 5468 656e  ABORT).```..Then
+000049b0: 2074 6865 2064 6566 6175 6c74 2060 2274   the default `"t
+000049c0: 6573 7473 2f75 6e69 7422 2c20 2274 6573  ests/unit", "tes
+000049d0: 7473 2f69 6e74 6567 7261 7469 6f6e 2260  ts/integration"`
+000049e0: 2066 6f6c 6465 7273 2063 616e 2062 6520   folders can be 
+000049f0: 6f76 6572 7269 6464 656e 2065 6974 6865  overridden eithe
+00004a00: 7220 7669 6120 636f 6d6d 616e 6420 6c69  r via command li
+00004a10: 6e65 206f 7074 696f 6e73 2060 2d66 602f  ne options `-f`/
+00004a20: 602d 2d66 696c 6560 2f60 2d2d 666f 6c64  `--file`/`--fold
+00004a30: 6572 603a 0a0a 6060 6073 6865 6c6c 2073  er`:..```shell s
+00004a40: 6372 6970 740a 6465 6c66 696e 6f20 7465  cript.delfino te
+00004a50: 7374 202d 6620 7465 7374 732f 6f74 6865  st -f tests/othe
+00004a60: 720a 6060 600a 0a4f 7220 7669 6120 636f  r.```..Or via co
+00004a70: 6e66 6967 7572 6174 696f 6e20 696e 2074  nfiguration in t
+00004a80: 6865 2060 7079 7072 6f6a 6563 742e 746f  he `pyproject.to
+00004a90: 6d6c 6020 6669 6c65 3a0a 0a60 6060 746f  ml` file:..```to
+00004aa0: 6d6c 0a5b 746f 6f6c 2e64 656c 6669 6e6f  ml.[tool.delfino
+00004ab0: 2e70 6c75 6769 6e73 2e3c 504c 5547 494e  .plugins.<PLUGIN
+00004ac0: 3e2e 7465 7374 5d0a 6669 6c65 735f 666f  >.test].files_fo
+00004ad0: 6c64 6572 7320 3d20 5b27 7465 7374 732f  lders = ['tests/
+00004ae0: 6f74 6865 7227 5d0a 6060 600a 0a45 6974  other'].```..Eit
+00004af0: 6865 7220 7761 792c 2062 6f74 6820 7769  her way, both wi
+00004b00: 6c6c 2072 6573 756c 7420 696e 2065 7865  ll result in exe
+00004b10: 6375 7469 6e67 2060 7079 7465 7374 2074  cuting `pytest t
+00004b20: 6573 7473 2f6f 7468 6572 602e 0a0a 2323  ests/other`...##
+00004b30: 2047 726f 7570 696e 6720 636f 6d6d 616e   Grouping comman
+00004b40: 6473 0a0a 4f66 7465 6e20 6974 2069 7320  ds..Often it is 
+00004b50: 7573 6566 756c 2074 6f20 7275 6e20 7365  useful to run se
+00004b60: 7665 7261 6c20 636f 6d6d 616e 6473 2061  veral commands a
+00004b70: 7320 6120 6772 6f75 7020 7769 7468 2061  s a group with a
+00004b80: 2064 6966 6665 7265 6e74 2063 6f6d 6d61   different comma
+00004b90: 6e64 206e 616d 652e 2043 6c69 636b 2073  nd name. Click s
+00004ba0: 7570 706f 7274 7320 6361 6c6c 696e 6720  upports calling 
+00004bb0: 6f74 6865 7220 636f 6d6d 616e 6473 2077  other commands w
+00004bc0: 6974 6820 5b60 636c 6963 6b2e 436f 6e74  ith [`click.Cont
+00004bd0: 6578 742e 666f 7277 6172 6460 5d28 6874  ext.forward`](ht
+00004be0: 7470 733a 2f2f 636c 6963 6b2e 7061 6c6c  tps://click.pall
+00004bf0: 6574 7370 726f 6a65 6374 732e 636f 6d2f  etsprojects.com/
+00004c00: 6170 692f 2363 6c69 636b 2e43 6f6e 7465  api/#click.Conte
+00004c10: 7874 2e66 6f72 7761 7264 2920 6f72 205b  xt.forward) or [
+00004c20: 6063 6c69 636b 2e43 6f6e 7465 7874 2e69  `click.Context.i
+00004c30: 6e76 6f6b 6560 5d28 6874 7470 733a 2f2f  nvoke`](https://
+00004c40: 636c 6963 6b2e 7061 6c6c 6574 7370 726f  click.palletspro
+00004c50: 6a65 6374 732e 636f 6d2f 6170 692f 2363  jects.com/api/#c
+00004c60: 6c69 636b 2e43 6f6e 7465 7874 2e69 6e76  lick.Context.inv
+00004c70: 6f6b 6529 2e0a 0a3c 212d 2d20 544f 444f  oke)...<!-- TODO
+00004c80: 2852 6164 656b 293a 2041 6464 2064 6573  (Radek): Add des
+00004c90: 6372 6970 7469 6f6e 206f 6620 6065 7865  cription of `exe
+00004ca0: 6375 7465 5f63 6f6d 6d61 6e64 735f 6772  cute_commands_gr
+00004cb0: 6f75 7060 206f 6e63 6520 6d69 6772 6174  oup` once migrat
+00004cc0: 6564 2066 726f 6d20 6064 656c 6669 6e6f  ed from `delfino
+00004cd0: 2d63 6f72 6560 2e20 2d2d 3e0a 0a         -core`. -->..
```

