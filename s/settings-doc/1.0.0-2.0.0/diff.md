# Comparing `tmp/settings_doc-1.0.0.tar.gz` & `tmp/settings_doc-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "settings_doc-1.0.0.tar", max compression
+gzip compressed data, was "settings_doc-2.0.0.tar", max compression
```

## Comparing `settings_doc-1.0.0.tar` & `settings_doc-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1067 2022-12-29 21:18:57.937564 settings_doc-1.0.0/LICENSE
--rw-r--r--   0        0        0     9982 2022-12-29 21:18:57.937564 settings_doc-1.0.0/README.md
--rw-r--r--   0        0        0     3750 2022-12-29 21:18:57.937564 settings_doc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-29 21:18:57.937564 settings_doc-1.0.0/src/settings_doc/__init__.py
--rw-r--r--   0        0        0     2902 2022-12-29 21:18:57.937564 settings_doc-1.0.0/src/settings_doc/importing.py
--rw-r--r--   0        0        0     6239 2022-12-29 21:18:57.937564 settings_doc-1.0.0/src/settings_doc/main.py
--rw-r--r--   0        0        0      759 2022-12-29 21:18:57.937564 settings_doc-1.0.0/src/settings_doc/templates/debug.jinja
--rw-r--r--   0        0        0     1700 2022-12-29 21:18:57.937564 settings_doc-1.0.0/src/settings_doc/templates/dotenv.jinja
--rw-r--r--   0        0        0     2123 2022-12-29 21:18:57.937564 settings_doc-1.0.0/src/settings_doc/templates/markdown.jinja
--rw-r--r--   0        0        0    11273 1970-01-01 00:00:00.000000 settings_doc-1.0.0/setup.py
--rw-r--r--   0        0        0    11742 1970-01-01 00:00:00.000000 settings_doc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-25 14:05:32.466293 settings_doc-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9982 2023-06-25 14:05:32.466293 settings_doc-2.0.0/README.md
+-rw-r--r--   0        0        0     3736 2023-06-25 14:05:32.466293 settings_doc-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 14:05:32.466293 settings_doc-2.0.0/src/settings_doc/__init__.py
+-rw-r--r--   0        0        0     2898 2023-06-25 14:05:32.466293 settings_doc-2.0.0/src/settings_doc/importing.py
+-rw-r--r--   0        0        0     6248 2023-06-25 14:05:32.466293 settings_doc-2.0.0/src/settings_doc/main.py
+-rw-r--r--   0        0        0      759 2023-06-25 14:05:32.466293 settings_doc-2.0.0/src/settings_doc/templates/debug.jinja
+-rw-r--r--   0        0        0     1700 2023-06-25 14:05:32.466293 settings_doc-2.0.0/src/settings_doc/templates/dotenv.jinja
+-rw-r--r--   0        0        0     2123 2023-06-25 14:05:32.466293 settings_doc-2.0.0/src/settings_doc/templates/markdown.jinja
+-rw-r--r--   0        0        0    11483 1970-01-01 00:00:00.000000 settings_doc-2.0.0/PKG-INFO
```

### Comparing `settings_doc-1.0.0/LICENSE` & `settings_doc-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `settings_doc-1.0.0/README.md` & `settings_doc-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     </a>
     <a href="https://app.codecov.io/gh/radeklat/settings-doc/">
         <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/settings-doc">
     </a>
     <a href="https://github.com/radeklat/settings-doc/tags">
         <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/settings-doc">
     </a>
-    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2022">
+    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2023">
     <a href="https://github.com/radeklat/settings-doc/commits/main">
         <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/settings-doc">
     </a>
     <a href="https://pypistats.org/packages/settings-doc">
         <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dm/settings-doc">
     </a>
     <a href="https://github.com/radeklat/settings-doc/blob/main/LICENSE">
```

### Comparing `settings_doc-1.0.0/pyproject.toml` & `settings_doc-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "settings-doc"
-version = "1.0.0"
+version = "2.0.0"
 description = "A command line tool for generating Markdown documentation and .env files from pydantic BaseSettings."
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 # https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -17,37 +17,36 @@
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Software Distribution",
     "Topic :: System :: Systems Administration",
     "Topic :: Text Processing :: Markup :: Markdown",
     "Topic :: Utilities",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 keywords = ["documentation", "environment variables", "generated", "markdown", "BaseSettings"]
 homepage = "https://github.com/radeklat/settings-doc"
 
 [tool.poetry.scripts]
 settings-doc = "settings_doc.main:app"
 
 [tool.poetry.dependencies]
-python = ">=3.7.2,<=3.11"
+python = "^3.8"
 Jinja2 = "^3.0.2"
 pydantic = "^1.8.2"
-typer = {version = "^0.4.0", extras = ["all"]}
+typer = {version = "^0.9", extras = ["all"]}  # https://typer.tiangolo.com/release-notes/
 
 [tool.poetry.dev-dependencies]
 click = "^8.0.3"
 types-toml = "*"
-delfino-core = {extras = ["verify_all", "dependencies-update"], version = "^4.0.1"}
+delfino-core = {extras = ["verify_all", "dependencies-update"], version = "^5.0"}
 pytest-mock = "^3.6.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `settings_doc-1.0.0/src/settings_doc/importing.py` & `settings_doc-2.0.0/src/settings_doc/importing.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pydantic import BaseSettings
 from typer import colors
 
 _MODULE_ERROR_MSG = "No `pydantic.BaseSettings` subclasses found in module '{module_path}'."
 _RELATIVE_IMPORT_ERROR_MSG = "Relative imports are not supported."
 
 
-@lru_cache()
+@lru_cache
 def import_module_path(module_paths: Tuple[str, ...]) -> Set[Type[BaseSettings]]:
     if not module_paths:
         return set()
 
     settings: Set[Type[BaseSettings]] = set()
 
     for module_path in module_paths:
@@ -45,15 +45,15 @@
             if len(module_paths) == 1
             else "No `pydantic.BaseSettings` subclasses found in any of the modules."
         )
 
     return settings
 
 
-@lru_cache()
+@lru_cache
 def import_class_path(class_paths: Tuple[str, ...]) -> Set[Type[BaseSettings]]:
     settings: Set[Type[BaseSettings]] = set()
 
     for class_path in class_paths:
         module, class_name = class_path.rsplit(".", maxsplit=1)
         try:
             new_class = getattr(importlib.import_module(module), class_name)
```

### Comparing `settings_doc-1.0.0/src/settings_doc/main.py` & `settings_doc-2.0.0/src/settings_doc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import re
 import shutil
 from collections.abc import Iterable as IterableCollection
 from enum import Enum, auto
 from itertools import chain
 from os import listdir
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple, Type
+from typing import Any, Dict, Final, List, Optional, Set, Tuple, Type
 
 from click import Abort, secho
 from jinja2 import Environment, FileSystemLoader, Template, select_autoescape
 from pydantic import BaseSettings
 from pydantic.fields import ModelField
 from typer import Option, Typer, colors
 
 from settings_doc import importing
 
 app = Typer()
 
 
-TEMPLATES_FOLDER: Path = Path(__file__).parent / "templates"
+TEMPLATES_FOLDER: Final[Path] = Path(__file__).parent / "templates"
 
 
 class OutputFormat(Enum):
     # noinspection PyMethodParameters
     def _generate_next_value_(name, start, count, last_values):  # pylint: disable=no-self-argument
         del start, count, last_values
         return name.lower()  # pylint: disable=no-member
@@ -124,15 +124,15 @@
     env.globals["is_values_with_descriptions"] = is_values_with_descriptions
     render = get_template(env, output_format).render(**render_kwargs)
 
     if update_file is None:
         print(render)
         return
 
-    with open(update_file, "r", encoding="utf-8") as file:
+    with open(update_file, encoding="utf-8") as file:
         content = file.read()
 
     with open(update_file, "w", encoding="utf-8") as file:
         if all(update_between):
             pattern = re.compile(f"({re.escape(update_between[0])}\n?).*(\n?{re.escape(update_between[1])})", re.DOTALL)
 
             if pattern.search(content) is None:
```

### Comparing `settings_doc-1.0.0/src/settings_doc/templates/debug.jinja` & `settings_doc-2.0.0/src/settings_doc/templates/debug.jinja`

 * *Files identical despite different names*

### Comparing `settings_doc-1.0.0/src/settings_doc/templates/dotenv.jinja` & `settings_doc-2.0.0/src/settings_doc/templates/dotenv.jinja`

 * *Files identical despite different names*

### Comparing `settings_doc-1.0.0/src/settings_doc/templates/markdown.jinja` & `settings_doc-2.0.0/src/settings_doc/templates/markdown.jinja`

 * *Files identical despite different names*

### Comparing `settings_doc-1.0.0/setup.py` & `settings_doc-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,705 +1,718 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 7365 7474 696e 6773 5f64 6f63 275d  ['settings_doc']
-00000070: 0a0a 7061 636b 6167 655f 6461 7461 203d  ..package_data =
-00000080: 205c 0a7b 2727 3a20 5b27 2a27 5d2c 2027   \.{'': ['*'], '
-00000090: 7365 7474 696e 6773 5f64 6f63 273a 205b  settings_doc': [
-000000a0: 2774 656d 706c 6174 6573 2f2a 275d 7d0a  'templates/*']}.
-000000b0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000000c0: 7320 3d20 5c0a 5b27 4a69 6e6a 6132 3e3d  s = \.['Jinja2>=
-000000d0: 332e 302e 322c 3c34 2e30 2e30 272c 2027  3.0.2,<4.0.0', '
-000000e0: 7079 6461 6e74 6963 3e3d 312e 382e 322c  pydantic>=1.8.2,
-000000f0: 3c32 2e30 2e30 272c 2027 7479 7065 725b  <2.0.0', 'typer[
-00000100: 616c 6c5d 3e3d 302e 342e 302c 3c30 2e35  all]>=0.4.0,<0.5
-00000110: 2e30 275d 0a0a 656e 7472 795f 706f 696e  .0']..entry_poin
-00000120: 7473 203d 205c 0a7b 2763 6f6e 736f 6c65  ts = \.{'console
-00000130: 5f73 6372 6970 7473 273a 205b 2773 6574  _scripts': ['set
-00000140: 7469 6e67 732d 646f 6320 3d20 7365 7474  tings-doc = sett
-00000150: 696e 6773 5f64 6f63 2e6d 6169 6e3a 6170  ings_doc.main:ap
-00000160: 7027 5d7d 0a0a 7365 7475 705f 6b77 6172  p']}..setup_kwar
-00000170: 6773 203d 207b 0a20 2020 2027 6e61 6d65  gs = {.    'name
-00000180: 273a 2027 7365 7474 696e 6773 2d64 6f63  ': 'settings-doc
-00000190: 272c 0a20 2020 2027 7665 7273 696f 6e27  ',.    'version'
-000001a0: 3a20 2731 2e30 2e30 272c 0a20 2020 2027  : '1.0.0',.    '
-000001b0: 6465 7363 7269 7074 696f 6e27 3a20 2741  description': 'A
-000001c0: 2063 6f6d 6d61 6e64 206c 696e 6520 746f   command line to
-000001d0: 6f6c 2066 6f72 2067 656e 6572 6174 696e  ol for generatin
-000001e0: 6720 4d61 726b 646f 776e 2064 6f63 756d  g Markdown docum
-000001f0: 656e 7461 7469 6f6e 2061 6e64 202e 656e  entation and .en
-00000200: 7620 6669 6c65 7320 6672 6f6d 2070 7964  v files from pyd
-00000210: 616e 7469 6320 4261 7365 5365 7474 696e  antic BaseSettin
-00000220: 6773 2e27 2c0a 2020 2020 276c 6f6e 675f  gs.',.    'long_
-00000230: 6465 7363 7269 7074 696f 6e27 3a20 273c  description': '<
-00000240: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
-00000250: 2220 7374 796c 653d 2262 6f72 6465 722d  " style="border-
-00000260: 626f 7474 6f6d 3a20 6e6f 6e65 3b22 3ee2  bottom: none;">.
-00000270: 9a99 266e 6273 703b f09f 939d 266e 6273  ..&nbsp;....&nbs
-00000280: 703b 266e 6273 703b 5365 7474 696e 6773  p;&nbsp;Settings
-00000290: 266e 6273 703b 446f 6347 656e 266e 6273  &nbsp;DocGen&nbs
-000002a0: 703b 266e 6273 703b f09f 939d 266e 6273  p;&nbsp;....&nbs
-000002b0: 703b e29a 993c 2f68 313e 5c6e 3c68 3320  p;...</h1>\n<h3 
-000002c0: 616c 6967 6e3d 2263 656e 7465 7222 3e41  align="center">A
-000002d0: 2063 6f6d 6d61 6e64 206c 696e 6520 746f   command line to
-000002e0: 6f6c 2066 6f72 2067 656e 6572 6174 696e  ol for generatin
-000002f0: 6720 4d61 726b 646f 776e 2064 6f63 756d  g Markdown docum
-00000300: 656e 7461 7469 6f6e 2061 6e64 202e 656e  entation and .en
-00000310: 7620 6669 6c65 7320 6672 6f6d 203c 6120  v files from <a 
-00000320: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000330: 6461 6e74 6963 2d64 6f63 732e 6865 6c70  dantic-docs.help
-00000340: 6d61 6e75 616c 2e69 6f2f 7573 6167 652f  manual.io/usage/
-00000350: 7365 7474 696e 6773 223e 7079 6461 6e74  settings">pydant
-00000360: 6963 2e42 6173 6553 6574 7469 6e67 733c  ic.BaseSettings<
-00000370: 2f61 3e2e 3c2f 6833 3e5c 6e5c 6e3c 7020  /a>.</h3>\n\n<p 
-00000380: 616c 6967 6e3d 2263 656e 7465 7222 3e5c  align="center">\
-00000390: 6e20 2020 203c 6120 6872 6566 3d22 6874  n    <a href="ht
-000003a0: 7470 733a 2f2f 6170 702e 6369 7263 6c65  tps://app.circle
-000003b0: 6369 2e63 6f6d 2f70 6970 656c 696e 6573  ci.com/pipelines
-000003c0: 2f67 6974 6875 622f 7261 6465 6b6c 6174  /github/radeklat
-000003d0: 2f73 6574 7469 6e67 732d 646f 633f 6272  /settings-doc?br
-000003e0: 616e 6368 3d6d 6169 6e22 3e5c 6e20 2020  anch=main">\n   
-000003f0: 2020 2020 203c 696d 6720 616c 743d 2243       <img alt="C
-00000400: 6972 636c 6543 4922 2073 7263 3d22 6874  ircleCI" src="ht
-00000410: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000420: 732e 696f 2f63 6972 636c 6563 692f 6275  s.io/circleci/bu
-00000430: 696c 642f 6769 7468 7562 2f72 6164 656b  ild/github/radek
-00000440: 6c61 742f 7365 7474 696e 6773 2d64 6f63  lat/settings-doc
-00000450: 223e 5c6e 2020 2020 3c2f 613e 5c6e 2020  ">\n    </a>\n  
-00000460: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000470: 3a2f 2f61 7070 2e63 6f64 6563 6f76 2e69  ://app.codecov.i
-00000480: 6f2f 6768 2f72 6164 656b 6c61 742f 7365  o/gh/radeklat/se
-00000490: 7474 696e 6773 2d64 6f63 2f22 3e5c 6e20  ttings-doc/">\n 
-000004a0: 2020 2020 2020 203c 696d 6720 616c 743d         <img alt=
-000004b0: 2243 6f64 6563 6f76 2220 7372 633d 2268  "Codecov" src="h
-000004c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000004d0: 6473 2e69 6f2f 636f 6465 636f 762f 632f  ds.io/codecov/c/
-000004e0: 6769 7468 7562 2f72 6164 656b 6c61 742f  github/radeklat/
-000004f0: 7365 7474 696e 6773 2d64 6f63 223e 5c6e  settings-doc">\n
-00000500: 2020 2020 3c2f 613e 5c6e 2020 2020 3c61      </a>\n    <a
-00000510: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000520: 6974 6875 622e 636f 6d2f 7261 6465 6b6c  ithub.com/radekl
-00000530: 6174 2f73 6574 7469 6e67 732d 646f 632f  at/settings-doc/
-00000540: 7461 6773 223e 5c6e 2020 2020 2020 2020  tags">\n        
-00000550: 3c69 6d67 2061 6c74 3d22 4769 7448 7562  <img alt="GitHub
-00000560: 2074 6167 2028 6c61 7465 7374 2053 656d   tag (latest Sem
-00000570: 5665 7229 2220 7372 633d 2268 7474 7073  Ver)" src="https
-00000580: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000590: 6f2f 6769 7468 7562 2f74 6167 2f72 6164  o/github/tag/rad
-000005a0: 656b 6c61 742f 7365 7474 696e 6773 2d64  eklat/settings-d
-000005b0: 6f63 223e 5c6e 2020 2020 3c2f 613e 5c6e  oc">\n    </a>\n
-000005c0: 2020 2020 3c69 6d67 2061 6c74 3d22 4d61      <img alt="Ma
-000005d0: 696e 7465 6e61 6e63 6522 2073 7263 3d22  intenance" src="
-000005e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005f0: 6c64 732e 696f 2f6d 6169 6e74 656e 616e  lds.io/maintenan
-00000600: 6365 2f79 6573 2f32 3032 3222 3e5c 6e20  ce/yes/2022">\n 
-00000610: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00000620: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00000630: 6164 656b 6c61 742f 7365 7474 696e 6773  adeklat/settings
-00000640: 2d64 6f63 2f63 6f6d 6d69 7473 2f6d 6169  -doc/commits/mai
-00000650: 6e22 3e5c 6e20 2020 2020 2020 203c 696d  n">\n        <im
-00000660: 6720 616c 743d 2247 6974 4875 6220 6c61  g alt="GitHub la
-00000670: 7374 2063 6f6d 6d69 7422 2073 7263 3d22  st commit" src="
-00000680: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000690: 6c64 732e 696f 2f67 6974 6875 622f 6c61  lds.io/github/la
-000006a0: 7374 2d63 6f6d 6d69 742f 7261 6465 6b6c  st-commit/radekl
-000006b0: 6174 2f73 6574 7469 6e67 732d 646f 6322  at/settings-doc"
-000006c0: 3e5c 6e20 2020 203c 2f61 3e5c 6e20 2020  >\n    </a>\n   
-000006d0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000006e0: 2f2f 7079 7069 7374 6174 732e 6f72 672f  //pypistats.org/
-000006f0: 7061 636b 6167 6573 2f73 6574 7469 6e67  packages/setting
-00000700: 732d 646f 6322 3e5c 6e20 2020 2020 2020  s-doc">\n       
-00000710: 203c 696d 6720 616c 743d 2250 7950 4920   <img alt="PyPI 
-00000720: 2d20 446f 776e 6c6f 6164 7322 2073 7263  - Downloads" src
-00000730: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000740: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-00000750: 2f73 6574 7469 6e67 732d 646f 6322 3e5c  /settings-doc">\
-00000760: 6e20 2020 203c 2f61 3e5c 6e20 2020 203c  n    </a>\n    <
-00000770: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000780: 6769 7468 7562 2e63 6f6d 2f72 6164 656b  github.com/radek
-00000790: 6c61 742f 7365 7474 696e 6773 2d64 6f63  lat/settings-doc
-000007a0: 2f62 6c6f 622f 6d61 696e 2f4c 4943 454e  /blob/main/LICEN
-000007b0: 5345 223e 5c6e 2020 2020 2020 2020 3c69  SE">\n        <i
-000007c0: 6d67 2061 6c74 3d22 5079 5049 202d 204c  mg alt="PyPI - L
-000007d0: 6963 656e 7365 2220 7372 633d 2268 7474  icense" src="htt
-000007e0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000007f0: 2e69 6f2f 7079 7069 2f6c 2f73 6574 7469  .io/pypi/l/setti
-00000800: 6e67 732d 646f 6322 3e5c 6e20 2020 203c  ngs-doc">\n    <
-00000810: 2f61 3e5c 6e20 2020 203c 6120 6872 6566  /a>\n    <a href
-00000820: 3d22 6874 7470 733a 2f2f 7777 772e 7079  ="https://www.py
-00000830: 7468 6f6e 2e6f 7267 2f64 6f63 2f76 6572  thon.org/doc/ver
-00000840: 7369 6f6e 732f 223e 5c6e 2020 2020 2020  sions/">\n      
-00000850: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
-00000860: 202d 2050 7974 686f 6e20 5665 7273 696f   - Python Versio
-00000870: 6e22 2073 7263 3d22 6874 7470 733a 2f2f  n" src="https://
-00000880: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000890: 7970 692f 7079 7665 7273 696f 6e73 2f73  ypi/pyversions/s
-000008a0: 6574 7469 6e67 732d 646f 6322 3e5c 6e20  ettings-doc">\n 
-000008b0: 2020 203c 2f61 3e5c 6e3c 2f70 3e5c 6e5c     </a>\n</p>\n\
-000008c0: 6e54 6865 2073 616d 6520 7761 7920 796f  nThe same way yo
-000008d0: 7520 6172 6520 6162 6c65 2074 6f20 6765  u are able to ge
-000008e0: 6e65 7261 7465 204f 7065 6e41 5049 2064  nerate OpenAPI d
-000008f0: 6f63 756d 656e 7461 7469 6f6e 2066 726f  ocumentation fro
-00000900: 6d20 5b60 7079 6461 6e74 6963 2e42 6173  m [`pydantic.Bas
-00000910: 654d 6f64 656c 605d 2868 7474 7073 3a2f  eModel`](https:/
-00000920: 2f70 7964 616e 7469 632d 646f 6373 2e68  /pydantic-docs.h
-00000930: 656c 706d 616e 7561 6c2e 696f 2f75 7361  elpmanual.io/usa
-00000940: 6765 2f6d 6f64 656c 732f 292c 2060 7365  ge/models/), `se
-00000950: 7474 696e 6773 2d64 6f63 6020 616c 6c6f  ttings-doc` allo
-00000960: 7773 2079 6f75 2074 6f20 6765 6e65 7261  ws you to genera
-00000970: 7465 2064 6f63 756d 656e 7461 7469 6f6e  te documentation
-00000980: 2066 726f 6d20 5b60 7079 6461 6e74 6963   from [`pydantic
-00000990: 2e42 6173 6553 6574 7469 6e67 7360 5d28  .BaseSettings`](
-000009a0: 6874 7470 733a 2f2f 7079 6461 6e74 6963  https://pydantic
-000009b0: 2d64 6f63 732e 6865 6c70 6d61 6e75 616c  -docs.helpmanual
-000009c0: 2e69 6f2f 7573 6167 652f 7365 7474 696e  .io/usage/settin
-000009d0: 6773 292e 5c6e 5c6e 4974 2069 7320 706f  gs).\n\nIt is po
-000009e0: 7765 7265 6420 6279 2074 6865 205b 4a69  wered by the [Ji
-000009f0: 6e6a 6132 5d28 6874 7470 733a 2f2f 6a69  nja2](https://ji
-00000a00: 6e6a 612e 7061 6c6c 6574 7370 726f 6a65  nja.palletsproje
-00000a10: 6374 732e 636f 6d2f 656e 2f6c 6174 6573  cts.com/en/lates
-00000a20: 742f 2920 7465 6d70 6c61 7469 6e67 2065  t/) templating e
-00000a30: 6e67 696e 6520 616e 6420 5b54 7970 6572  ngine and [Typer
-00000a40: 5d28 6874 7470 733a 2f2f 7479 7065 722e  ](https://typer.
-00000a50: 7469 616e 676f 6c6f 2e63 6f6d 2f29 2066  tiangolo.com/) f
-00000a60: 7261 6d65 776f 726b 2e20 4966 2079 6f75  ramework. If you
-00000a70: 2064 6f6e 5c27 7420 6c69 6b65 2074 6865   don\'t like the
-00000a80: 2062 7569 6c74 2d69 6e20 7465 6d70 6c61   built-in templa
-00000a90: 7465 732c 2079 6f75 2063 616e 2065 6173  tes, you can eas
-00000aa0: 696c 7920 6d6f 6469 6679 2074 6865 6d20  ily modify them 
-00000ab0: 6f72 2077 7269 7465 2063 6f6d 706c 6574  or write complet
-00000ac0: 656c 7920 6375 7374 6f6d 206f 6e65 732e  ely custom ones.
-00000ad0: 2041 6c6c 2061 7474 7269 6275 7465 7320   All attributes 
-00000ae0: 6f66 2074 6865 205b 6042 6173 6553 6574  of the [`BaseSet
-00000af0: 7469 6e67 7360 5d28 6874 7470 733a 2f2f  tings`](https://
-00000b00: 7079 6461 6e74 6963 2d64 6f63 732e 6865  pydantic-docs.he
-00000b10: 6c70 6d61 6e75 616c 2e69 6f2f 7573 6167  lpmanual.io/usag
-00000b20: 652f 7365 7474 696e 6773 2920 6d6f 6465  e/settings) mode
-00000b30: 6c73 2061 7265 2065 7870 6f73 6564 2074  ls are exposed t
-00000b40: 6f20 7468 6520 7465 6d70 6c61 7465 732e  o the templates.
-00000b50: 5c6e 5c6e 3c21 2d2d 5c6e 2020 2020 486f  \n\n<!--\n    Ho
-00000b60: 7720 746f 2067 656e 6572 6174 6520 544f  w to generate TO
-00000b70: 4320 6672 6f6d 2050 7943 6861 726d 3a5c  C from PyCharm:\
-00000b80: 6e20 2020 2068 7474 7073 3a2f 2f67 6974  n    https://git
-00000b90: 6875 622e 636f 6d2f 7673 6368 2f69 6465  hub.com/vsch/ide
-00000ba0: 612d 6d75 6c74 696d 6172 6b64 6f77 6e2f  a-multimarkdown/
-00000bb0: 7769 6b69 2f54 6162 6c65 2d6f 662d 436f  wiki/Table-of-Co
-00000bc0: 6e74 656e 7473 2d45 7874 656e 7369 6f6e  ntents-Extension
-00000bd0: 5c6e 2d2d 3e5c 6e5b 544f 4320 6c65 7665  \n-->\n[TOC leve
-00000be0: 6c73 3d31 2c32 206d 6172 6b64 6f77 6e20  ls=1,2 markdown 
-00000bf0: 666f 726d 6174 7465 6420 6275 6c6c 6574  formatted bullet
-00000c00: 2068 6965 7261 7263 6879 5d3a 2023 2022   hierarchy]: # "
-00000c10: 5461 626c 6520 6f66 2063 6f6e 7465 6e74  Table of content
-00000c20: 225c 6e5c 6e23 2054 6162 6c65 206f 6620  "\n\n# Table of 
-00000c30: 636f 6e74 656e 745c 6e2d 205b 496e 7374  content\n- [Inst
-00000c40: 616c 6c61 7469 6f6e 5d28 2369 6e73 7461  allation](#insta
-00000c50: 6c6c 6174 696f 6e29 5c6e 2d20 5b55 7361  llation)\n- [Usa
-00000c60: 6765 5d28 2375 7361 6765 295c 6e20 202d  ge](#usage)\n  -
-00000c70: 205b 4d69 6e69 6d61 6c20 6578 616d 706c   [Minimal exampl
-00000c80: 655d 2823 6d69 6e69 6d61 6c2d 6578 616d  e](#minimal-exam
-00000c90: 706c 6529 5c6e 2020 2d20 5b43 6c61 7373  ple)\n  - [Class
-00000ca0: 2061 7574 6f2d 6469 7363 6f76 6572 795d   auto-discovery]
-00000cb0: 2823 636c 6173 732d 6175 746f 2d64 6973  (#class-auto-dis
-00000cc0: 636f 7665 7279 295c 6e20 202d 205b 4164  covery)\n  - [Ad
-00000cd0: 6469 6e67 206d 6f72 6520 696e 666f 726d  ding more inform
-00000ce0: 6174 696f 6e5d 2823 6164 6469 6e67 2d6d  ation](#adding-m
-00000cf0: 6f72 652d 696e 666f 726d 6174 696f 6e29  ore-information)
-00000d00: 5c6e 2020 2d20 5b55 7064 6174 696e 6720  \n  - [Updating 
-00000d10: 6578 6973 7469 6e67 2064 6f63 756d 656e  existing documen
-00000d20: 7461 7469 6f6e 5d28 2375 7064 6174 696e  tation](#updatin
-00000d30: 672d 6578 6973 7469 6e67 2d64 6f63 756d  g-existing-docum
-00000d40: 656e 7461 7469 6f6e 295c 6e2d 205b 4164  entation)\n- [Ad
-00000d50: 7661 6e63 6564 2075 7361 6765 5d28 2361  vanced usage](#a
-00000d60: 6476 616e 6365 642d 7573 6167 6529 5c6e  dvanced-usage)\n
-00000d70: 2020 2d20 5b43 7573 746f 6d20 7465 6d70    - [Custom temp
-00000d80: 6c61 7465 735d 2823 6375 7374 6f6d 2d74  lates](#custom-t
-00000d90: 656d 706c 6174 6573 295c 6e20 202d 205b  emplates)\n  - [
-00000da0: 4375 7374 6f6d 2073 6574 7469 6e67 7320  Custom settings 
-00000db0: 6174 7472 6962 7574 6573 2069 6e20 7465  attributes in te
-00000dc0: 6d70 6c61 7465 735d 2823 6375 7374 6f6d  mplates](#custom
-00000dd0: 2d73 6574 7469 6e67 732d 6174 7472 6962  -settings-attrib
-00000de0: 7574 6573 2d69 6e2d 7465 6d70 6c61 7465  utes-in-template
-00000df0: 7329 5c6e 2d20 5b46 6561 7475 7265 7320  s)\n- [Features 
-00000e00: 6f76 6572 7669 6577 5d28 2366 6561 7475  overview](#featu
-00000e10: 7265 732d 6f76 6572 7669 6577 295c 6e20  res-overview)\n 
-00000e20: 202d 205b 4d61 726b 646f 776e 5d28 236d   - [Markdown](#m
-00000e30: 6172 6b64 6f77 6e29 5c6e 2020 2d20 5b2e  arkdown)\n  - [.
-00000e40: 656e 765d 2823 656e 7629 5c6e 5c6e 2320  env](#env)\n\n# 
-00000e50: 496e 7374 616c 6c61 7469 6f6e 5c6e 5c6e  Installation\n\n
-00000e60: 6060 605c 6e70 6970 2069 6e73 7461 6c6c  ```\npip install
-00000e70: 2073 6574 7469 6e67 732d 646f 635c 6e60   settings-doc\n`
-00000e80: 6060 5c6e 5c6e 2320 5573 6167 655c 6e5c  ``\n\n# Usage\n\
-00000e90: 6e53 6565 2060 7365 7474 696e 6773 2d64  nSee `settings-d
-00000ea0: 6f63 202d 2d68 656c 7060 2066 6f72 2061  oc --help` for a
-00000eb0: 6c6c 206f 7074 696f 6e73 2e5c 6e5c 6e23  ll options.\n\n#
-00000ec0: 2320 4d69 6e69 6d61 6c20 6578 616d 706c  # Minimal exampl
-00000ed0: 655c 6e5c 6e4c 6574 5c27 7320 6173 7375  e\n\nLet\'s assu
-00000ee0: 6d65 2074 6865 2066 6f6c 6c6f 7769 6e67  me the following
-00000ef0: 205b 6042 6173 6553 6574 7469 6e67 7360   [`BaseSettings`
-00000f00: 5d28 6874 7470 733a 2f2f 7079 6461 6e74  ](https://pydant
-00000f10: 6963 2d64 6f63 732e 6865 6c70 6d61 6e75  ic-docs.helpmanu
-00000f20: 616c 2e69 6f2f 7573 6167 652f 7365 7474  al.io/usage/sett
-00000f30: 696e 6773 2920 696e 2060 7372 632f 7365  ings) in `src/se
-00000f40: 7474 696e 6773 2e70 7960 206f 6620 6120  ttings.py` of a 
-00000f50: 7072 6f6a 6563 743a 5c6e 5c6e 6060 6070  project:\n\n```p
-00000f60: 7974 686f 6e5c 6e66 726f 6d20 7079 6461  ython\nfrom pyda
-00000f70: 6e74 6963 2069 6d70 6f72 7420 4261 7365  ntic import Base
-00000f80: 5365 7474 696e 6773 5c6e 5c6e 636c 6173  Settings\n\nclas
-00000f90: 7320 4170 7053 6574 7469 6e67 7328 4261  s AppSettings(Ba
-00000fa0: 7365 5365 7474 696e 6773 293a 5c6e 2020  seSettings):\n  
-00000fb0: 2020 6c6f 6767 696e 675f 6c65 7665 6c3a    logging_level:
-00000fc0: 2073 7472 5c6e 6060 605c 6e5c 6e59 6f75   str\n```\n\nYou
-00000fd0: 2063 616e 2067 656e 6572 6174 6520 6120   can generate a 
-00000fe0: 4d61 726b 646f 776e 2064 6f63 756d 656e  Markdown documen
-00000ff0: 7461 7469 6f6e 2069 6e74 6f20 7374 646f  tation into stdo
-00001000: 7574 2077 6974 683a 5c6e 5c6e 6060 6073  ut with:\n\n```s
-00001010: 6865 6c6c 2073 6372 6970 745c 6e73 6574  hell script\nset
-00001020: 7469 6e67 732d 646f 6320 6765 6e65 7261  tings-doc genera
-00001030: 7465 202d 2d63 6c61 7373 2073 7263 2e73  te --class src.s
-00001040: 6574 7469 6e67 732e 4170 7053 6574 7469  ettings.AppSetti
-00001050: 6e67 7320 2d2d 6f75 7470 7574 2d66 6f72  ngs --output-for
-00001060: 6d61 7420 6d61 726b 646f 776e 5c6e 6060  mat markdown\n``
-00001070: 605c 6e5c 6e57 6869 6368 2077 696c 6c20  `\n\nWhich will 
-00001080: 6f75 7470 7574 3a5c 6e5c 6e60 6060 6d61  output:\n\n```ma
-00001090: 726b 646f 776e 5c6e 2320 604c 4f47 4749  rkdown\n# `LOGGI
-000010a0: 4e47 5f4c 4556 454c 605c 6e5c 6e2a 2a52  NG_LEVEL`\n\n**R
-000010b0: 6571 7569 7265 642a 2a5c 6e60 6060 5c6e  equired**\n```\n
-000010c0: 5c6e 5369 6d69 6c61 726c 792c 2079 6f75  \nSimilarly, you
-000010d0: 2063 616e 2067 656e 6572 6174 6520 6120   can generate a 
-000010e0: 602e 656e 7660 2066 696c 6520 666f 7220  `.env` file for 
-000010f0: 6c6f 6361 6c20 6465 7665 6c6f 706d 656e  local developmen
-00001100: 7420 7769 7468 3a5c 6e5c 6e60 6060 7368  t with:\n\n```sh
-00001110: 656c 6c20 7363 7269 7074 5c6e 7365 7474  ell script\nsett
-00001120: 696e 6773 2d64 6f63 2067 656e 6572 6174  ings-doc generat
-00001130: 6520 2d2d 636c 6173 7320 7372 632e 7365  e --class src.se
-00001140: 7474 696e 6773 2e41 7070 5365 7474 696e  ttings.AppSettin
-00001150: 6773 202d 2d6f 7574 7075 742d 666f 726d  gs --output-form
-00001160: 6174 2064 6f74 656e 765c 6e60 6060 5c6e  at dotenv\n```\n
-00001170: 5c6e 5768 6963 6820 7769 6c6c 206f 7574  \nWhich will out
-00001180: 7075 743a 5c6e 5c6e 6060 6064 6f74 656e  put:\n\n```doten
-00001190: 765c 6e4c 4f47 4749 4e47 5f4c 4556 454c  v\nLOGGING_LEVEL
-000011a0: 3d5c 6e5c 6e60 6060 5c6e 5c6e 2323 2043  =\n\n```\n\n## C
-000011b0: 6c61 7373 2061 7574 6f2d 6469 7363 6f76  lass auto-discov
-000011c0: 6572 795c 6e5c 6e49 6620 796f 7520 6861  ery\n\nIf you ha
-000011d0: 7665 2061 206d 6f64 756c 6520 7769 7468  ve a module with
-000011e0: 2061 2073 696e 676c 6520 7365 7474 696e   a single settin
-000011f0: 6773 2063 6c61 7373 206f 7220 7761 6e74  gs class or want
-00001200: 2074 6f20 6c6f 6164 206d 756c 7469 706c   to load multipl
-00001210: 6520 636c 6173 7365 7320 6174 206f 6e63  e classes at onc
-00001220: 6520 6173 2061 2073 6f75 7263 652c 2079  e as a source, y
-00001230: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
-00001240: 7468 6520 602d 2d6d 6f64 756c 6560 206f  the `--module` o
-00001250: 7074 696f 6e2e 2054 6865 2066 6f6c 6c6f  ption. The follo
-00001260: 7769 6e67 2065 7861 6d70 6c65 2077 6f72  wing example wor
-00001270: 6b73 2065 7861 6374 6c79 206c 696b 6520  ks exactly like 
-00001280: 7468 6520 6f6e 6520 6162 6f76 6520 616e  the one above an
-00001290: 6420 7769 6c6c 2075 7365 2074 6865 2060  d will use the `
-000012a0: 4170 7053 6574 7469 6e67 7360 2063 6c61  AppSettings` cla
-000012b0: 7373 2061 7574 6f6d 6174 6963 616c 6c79  ss automatically
-000012c0: 2e5c 6e5c 6e60 6060 7368 656c 6c20 7363  .\n\n```shell sc
-000012d0: 7269 7074 5c6e 7365 7474 696e 6773 2d64  ript\nsettings-d
-000012e0: 6f63 2067 656e 6572 6174 6520 2d2d 6d6f  oc generate --mo
-000012f0: 6475 6c65 2073 7263 2e73 6574 7469 6e67  dule src.setting
-00001300: 7320 2d2d 6f75 7470 7574 2d66 6f72 6d61  s --output-forma
-00001310: 7420 646f 7465 6e76 5c6e 6060 605c 6e5c  t dotenv\n```\n\
-00001320: 6e49 6620 6d75 6c74 6970 6c65 2063 6c61  nIf multiple cla
-00001330: 7373 6573 2063 6f6e 7461 696e 2061 2066  sses contain a f
-00001340: 6965 6c64 2077 6974 6820 7468 6520 7361  ield with the sa
-00001350: 6d65 206e 616d 652c 2061 6c6c 2069 6e73  me name, all ins
-00001360: 7461 6e63 6573 2077 696c 6c20 6170 7065  tances will appe
-00001370: 6172 2069 6e20 7468 6520 6f75 7470 7574  ar in the output
-00001380: 2e5c 6e5c 6e23 2320 4164 6469 6e67 206d  .\n\n## Adding m
-00001390: 6f72 6520 696e 666f 726d 6174 696f 6e5c  ore information\
-000013a0: 6e5c 6e59 6f75 2063 616e 2061 6464 2061  n\nYou can add a
-000013b0: 6e79 2065 7874 7261 2066 6965 6c64 2070  ny extra field p
-000013c0: 6172 616d 6574 6572 7320 746f 2074 6865  arameters to the
-000013d0: 2073 6574 7469 6e67 732e 2042 7920 6465   settings. By de
-000013e0: 6661 756c 742c 2060 7365 7474 696e 6773  fault, `settings
-000013f0: 2d64 6f63 6020 7769 6c6c 2075 7469 6c69  -doc` will utili
-00001400: 7365 2074 6865 2064 6566 6175 6c74 2076  se the default v
-00001410: 616c 7565 2c20 7768 6574 6865 7220 7468  alue, whether th
-00001420: 6520 7061 7261 6d65 7465 7220 6973 2072  e parameter is r
-00001430: 6571 7569 7265 6420 6f72 206f 7074 696f  equired or optio
-00001440: 6e61 6c2c 2064 6573 6372 6970 7469 6f6e  nal, description
-00001450: 2c20 6578 616d 706c 6520 7661 6c75 652c  , example value,
-00001460: 2061 6e64 206c 6973 7420 6f66 2070 6f73   and list of pos
-00001470: 7369 626c 6520 7661 6c75 6573 3a5c 6e5c  sible values:\n\
-00001480: 6e60 6060 7079 7468 6f6e 5c6e 6672 6f6d  n```python\nfrom
-00001490: 2070 7964 616e 7469 6320 696d 706f 7274   pydantic import
-000014a0: 2042 6173 6553 6574 7469 6e67 732c 2046   BaseSettings, F
-000014b0: 6965 6c64 5c6e 5c6e 636c 6173 7320 4170  ield\n\nclass Ap
-000014c0: 7053 6574 7469 6e67 7328 4261 7365 5365  pSettings(BaseSe
-000014d0: 7474 696e 6773 293a 5c6e 2020 2020 6c6f  ttings):\n    lo
-000014e0: 6767 696e 675f 6c65 7665 6c3a 2073 7472  gging_level: str
-000014f0: 203d 2046 6965 6c64 285c 6e20 2020 2020   = Field(\n     
-00001500: 2020 2022 5741 524e 494e 4722 2c5c 6e20     "WARNING",\n 
-00001510: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00001520: 6f6e 3d22 4c6f 6720 6c65 7665 6c2e 222c  on="Log level.",
-00001530: 5c6e 2020 2020 2020 2020 6578 616d 706c  \n        exampl
-00001540: 653d 2260 5741 524e 494e 4760 222c 5c6e  e="`WARNING`",\n
-00001550: 2020 2020 2020 2020 706f 7373 6962 6c65          possible
-00001560: 5f76 616c 7565 733d 5b22 4445 4255 4722  _values=["DEBUG"
-00001570: 2c20 2249 4e46 4f22 2c20 2257 4152 4e49  , "INFO", "WARNI
-00001580: 4e47 222c 2022 4552 524f 5222 2c20 2243  NG", "ERROR", "C
-00001590: 5249 5449 4341 4c22 5d2c 5c6e 2020 2020  RITICAL"],\n    
-000015a0: 295c 6e60 6060 5c6e 5c6e 5768 6963 6820  )\n```\n\nWhich 
-000015b0: 7769 6c6c 2067 656e 6572 6174 6520 7468  will generate th
-000015c0: 6520 666f 6c6c 6f77 696e 6720 6d61 726b  e following mark
-000015d0: 646f 776e 3a5c 6e5c 6e60 6060 6d61 726b  down:\n\n```mark
-000015e0: 646f 776e 5c6e 2320 604c 4f47 4749 4e47  down\n# `LOGGING
-000015f0: 5f4c 4556 454c 605c 6e5c 6e2a 4f70 7469  _LEVEL`\n\n*Opti
-00001600: 6f6e 616c 2a2c 2064 6566 6175 6c74 2076  onal*, default v
-00001610: 616c 7565 3a20 6057 4152 4e49 4e47 605c  alue: `WARNING`\
-00001620: 6e5c 6e4c 6f67 206c 6576 656c 2e5c 6e5c  n\nLog level.\n\
-00001630: 6e23 2320 4578 616d 706c 6573 5c6e 5c6e  n## Examples\n\n
-00001640: 6057 4152 4e49 4e47 605c 6e5c 6e23 2320  `WARNING`\n\n## 
-00001650: 506f 7373 6962 6c65 2076 616c 7565 735c  Possible values\
-00001660: 6e5c 6e60 4445 4255 4760 2c20 6049 4e46  n\n`DEBUG`, `INF
-00001670: 4f60 2c20 6057 4152 4e49 4e47 602c 2060  O`, `WARNING`, `
-00001680: 4552 524f 5260 2c20 6043 5249 5449 4341  ERROR`, `CRITICA
-00001690: 4c60 5c6e 6060 605c 6e5c 6e6f 7220 602e  L`\n```\n\nor `.
-000016a0: 656e 7660 2066 696c 653a 5c6e 5c6e 6060  env` file:\n\n``
-000016b0: 6064 6f74 656e 765c 6e23 204c 6f67 206c  `dotenv\n# Log l
-000016c0: 6576 656c 2e5c 6e23 2050 6f73 7369 626c  evel.\n# Possibl
-000016d0: 6520 7661 6c75 6573 3a5c 6e23 2020 2060  e values:\n#   `
-000016e0: 4445 4255 4760 2c20 6049 4e46 4f60 2c20  DEBUG`, `INFO`, 
-000016f0: 6057 4152 4e49 4e47 602c 2060 4552 524f  `WARNING`, `ERRO
-00001700: 5260 2c20 6043 5249 5449 4341 4c60 5c6e  R`, `CRITICAL`\n
-00001710: 2320 4c4f 4747 494e 475f 4c45 5645 4c3d  # LOGGING_LEVEL=
-00001720: 5741 524e 494e 475c 6e60 6060 5c6e 5c6e  WARNING\n```\n\n
-00001730: 596f 7520 6361 6e20 6669 6e64 2065 7665  You can find eve
-00001740: 6e20 6d6f 7265 2063 6f6d 706c 6578 2075  n more complex u
-00001750: 7361 6765 206f 6620 6073 6574 7469 6e67  sage of `setting
-00001760: 732d 646f 6360 2069 6e20 5b6f 6e65 206f  s-doc` in [one o
-00001770: 6620 6d79 206f 7468 6572 2070 726f 6a65  f my other proje
-00001780: 6374 735d 2868 7474 7073 3a2f 2f67 6974  cts](https://git
-00001790: 6875 622e 636f 6d2f 7261 6465 6b6c 6174  hub.com/radeklat
-000017a0: 2f6d 7174 742d 696e 666c 7578 6462 2d67  /mqtt-influxdb-g
-000017b0: 6174 6577 6179 2f62 6c6f 622f 6d61 696e  ateway/blob/main
-000017c0: 2f52 4541 444d 452e 6d64 2365 6e76 6972  /README.md#envir
-000017d0: 6f6e 6d65 6e74 2d76 6172 6961 626c 6573  onment-variables
-000017e0: 292e 5c6e 5c6e 2323 2055 7064 6174 696e  ).\n\n## Updatin
-000017f0: 6720 6578 6973 7469 6e67 2064 6f63 756d  g existing docum
-00001800: 656e 7461 7469 6f6e 5c6e 5c6e 4974 2069  entation\n\nIt i
-00001810: 7320 706f 7373 6962 6c65 2074 6f20 6765  s possible to ge
-00001820: 6e65 7261 7465 2064 6f63 756d 656e 7461  nerate documenta
-00001830: 7469 6f6e 2069 6e74 6f20 616e 2065 7869  tion into an exi
-00001840: 7374 696e 6720 646f 6375 6d65 6e74 2e20  sting document. 
-00001850: 546f 2066 6974 2077 6974 6820 7468 6520  To fit with the 
-00001860: 6865 6164 696e 6720 7374 7275 6374 7572  heading structur
-00001870: 652c 2079 6f75 2063 616e 2061 646a 7573  e, you can adjus
-00001880: 7420 7468 6520 6865 6164 696e 6720 6c65  t the heading le
-00001890: 7665 6c73 2077 6974 6820 602d 2d68 6561  vels with `--hea
-000018a0: 6469 6e67 2d6f 6666 7365 7460 2e20 4164  ding-offset`. Ad
-000018b0: 6469 7469 6f6e 616c 6c79 2c20 796f 7520  ditionally, you 
-000018c0: 6361 6e20 7370 6563 6966 7920 7468 6520  can specify the 
-000018d0: 6c6f 6361 7469 6f6e 2077 6865 7265 2074  location where t
-000018e0: 6f20 6765 6e65 7261 7465 2074 6865 2064  o generate the d
-000018f0: 6f63 756d 656e 7461 7469 6f6e 2077 6974  ocumentation wit
-00001900: 6820 7477 6f20 6d61 726b 7320 7365 7420  h two marks set 
-00001910: 6279 2060 2d2d 6265 7477 6565 6e20 3c53  by `--between <S
-00001920: 5441 5254 204d 4152 4b3e 203c 454e 4420  TART MARK> <END 
-00001930: 4d41 524b 3e60 2e5c 6e5c 6e4c 6574 5c27  MARK>`.\n\nLet\'
-00001940: 7320 6173 7375 6d65 2079 6f75 7220 6052  s assume your `R
-00001950: 4541 444d 452e 6d64 6020 6c6f 6f6b 7320  EADME.md` looks 
-00001960: 6c69 6b65 2074 6869 733a 5c6e 5c6e 6060  like this:\n\n``
-00001970: 606d 6172 6b64 6f77 6e5c 6e23 204d 7920  `markdown\n# My 
-00001980: 6170 705c 6e5c 6e54 6869 7320 6170 7020  app\n\nThis app 
-00001990: 6973 2064 6973 7472 6962 7574 6573 2061  is distributes a
-000019a0: 7320 6120 646f 636b 6572 2069 6d61 6765  s a docker image
-000019b0: 2061 6e64 2063 6f6e 6669 6775 7261 626c   and configurabl
-000019c0: 6520 7669 6120 656e 7669 726f 6e6d 656e  e via environmen
-000019d0: 7420 7661 7269 6162 6c65 732e 2053 6565  t variables. See
-000019e0: 2074 6865 206c 6973 7420 6265 6c6f 772e   the list below.
-000019f0: 5c6e 5c6e 2320 456e 7669 726f 6e6d 656e  \n\n# Environmen
-00001a00: 7420 7661 7269 6162 6c65 735c 6e3c 212d  t variables\n<!-
-00001a10: 2d20 6765 6e65 7261 7465 6420 656e 762e  - generated env.
-00001a20: 2076 6172 732e 2073 7461 7274 202d 2d3e   vars. start -->
-00001a30: 5c6e 3c21 2d2d 2067 656e 6572 6174 6564  \n<!-- generated
-00001a40: 2065 6e76 2e20 7661 7273 2e20 656e 6420   env. vars. end 
-00001a50: 2d2d 3e5c 6e60 6060 5c6e 5c6e 5768 656e  -->\n```\n\nWhen
-00001a60: 2079 6f75 2072 756e 3a5c 6e5c 6e60 6060   you run:\n\n```
-00001a70: 7368 656c 6c20 7363 7269 7074 5c6e 7365  shell script\nse
-00001a80: 7474 696e 6773 2d64 6f63 2067 656e 6572  ttings-doc gener
-00001a90: 6174 6520 5c5c 5c6e 2020 2d2d 636c 6173  ate \\\n  --clas
-00001aa0: 7320 7372 632e 7365 7474 696e 6773 2e41  s src.settings.A
-00001ab0: 7070 5365 7474 696e 6773 205c 5c5c 6e20  ppSettings \\\n 
-00001ac0: 202d 2d6f 7574 7075 742d 666f 726d 6174   --output-format
-00001ad0: 206d 6172 6b64 6f77 6e20 5c5c 205c 6e20   markdown \\ \n 
-00001ae0: 202d 2d75 7064 6174 6520 5245 4144 4d45   --update README
-00001af0: 2e6d 6420 5c5c 5c6e 2020 2d2d 6265 7477  .md \\\n  --betw
-00001b00: 6565 6e20 223c 212d 2d20 6765 6e65 7261  een "<!-- genera
-00001b10: 7465 6420 656e 762e 2076 6172 732e 2073  ted env. vars. s
-00001b20: 7461 7274 202d 2d3e 2220 223c 212d 2d20  tart -->" "<!-- 
-00001b30: 6765 6e65 7261 7465 6420 656e 762e 2076  generated env. v
-00001b40: 6172 732e 2065 6e64 202d 2d3e 2220 5c5c  ars. end -->" \\
-00001b50: 5c6e 2020 2d2d 6865 6164 696e 672d 6f66  \n  --heading-of
-00001b60: 6673 6574 2031 5c6e 6060 605c 6e5c 6e74  fset 1\n```\n\nt
-00001b70: 6865 2075 7064 6174 6564 2060 5245 4144  he updated `READ
-00001b80: 4d45 2e6d 6460 2077 696c 6c20 6765 7420  ME.md` will get 
-00001b90: 6f6e 6c79 2074 6865 2073 7065 6369 6669  only the specifi
-00001ba0: 6564 206c 6f63 6174 696f 6e20 6f76 6572  ed location over
-00001bb0: 7772 6974 7465 6e3a 5c6e 5c6e 6060 606d  written:\n\n```m
-00001bc0: 6172 6b64 6f77 6e5c 6e23 204d 7920 6170  arkdown\n# My ap
-00001bd0: 705c 6e5c 6e54 6869 7320 6170 7020 6973  p\n\nThis app is
-00001be0: 2064 6973 7472 6962 7574 6573 2061 7320   distributes as 
-00001bf0: 6120 646f 636b 6572 2069 6d61 6765 2061  a docker image a
-00001c00: 6e64 2063 6f6e 6669 6775 7261 626c 6520  nd configurable 
-00001c10: 7669 6120 656e 7669 726f 6e6d 656e 7420  via environment 
-00001c20: 7661 7269 6162 6c65 732e 2053 6565 2074  variables. See t
-00001c30: 6865 206c 6973 7420 6265 6c6f 772e 5c6e  he list below.\n
-00001c40: 5c6e 2320 456e 7669 726f 6e6d 656e 7420  \n# Environment 
-00001c50: 7661 7269 6162 6c65 735c 6e3c 212d 2d20  variables\n<!-- 
-00001c60: 6765 6e65 7261 7465 6420 656e 762e 2076  generated env. v
-00001c70: 6172 732e 2073 7461 7274 202d 2d3e 5c6e  ars. start -->\n
-00001c80: 2323 2060 4c4f 4747 494e 475f 4c45 5645  ## `LOGGING_LEVE
-00001c90: 4c60 5c6e 5c6e 2a4f 7074 696f 6e61 6c2a  L`\n\n*Optional*
-00001ca0: 2c20 6465 6661 756c 7420 7661 6c75 653a  , default value:
-00001cb0: 2060 5741 524e 494e 4760 5c6e 5c6e 4c6f   `WARNING`\n\nLo
-00001cc0: 6720 6c65 7665 6c2e 5c6e 5c6e 2323 2320  g level.\n\n### 
-00001cd0: 4578 616d 706c 6573 5c6e 5c6e 6057 4152  Examples\n\n`WAR
-00001ce0: 4e49 4e47 605c 6e5c 6e23 2323 2050 6f73  NING`\n\n### Pos
-00001cf0: 7369 626c 6520 7661 6c75 6573 5c6e 5c6e  sible values\n\n
-00001d00: 6044 4542 5547 602c 2060 494e 464f 602c  `DEBUG`, `INFO`,
-00001d10: 2060 5741 524e 494e 4760 2c20 6045 5252   `WARNING`, `ERR
-00001d20: 4f52 602c 2060 4352 4954 4943 414c 605c  OR`, `CRITICAL`\
-00001d30: 6e3c 212d 2d20 6765 6e65 7261 7465 6420  n<!-- generated 
-00001d40: 656e 762e 2076 6172 732e 2065 6e64 202d  env. vars. end -
-00001d50: 2d3e 5c6e 6060 605c 6e5c 6e23 2041 6476  ->\n```\n\n# Adv
-00001d60: 616e 6365 6420 7573 6167 655c 6e5c 6e23  anced usage\n\n#
-00001d70: 2320 4375 7374 6f6d 2074 656d 706c 6174  # Custom templat
-00001d80: 6573 5c6e 5c6e 6073 6574 7469 6e67 732d  es\n\n`settings-
-00001d90: 646f 6360 2063 6f6d 6573 2077 6974 6820  doc` comes with 
-00001da0: 6120 6665 7720 6275 696c 742d 696e 2074  a few built-in t
-00001db0: 656d 706c 6174 6573 2e20 596f 7520 6361  emplates. You ca
-00001dc0: 6e20 6f76 6572 7269 6465 2074 6865 6d20  n override them 
-00001dd0: 6f72 2077 7269 7465 2063 6f6d 706c 6574  or write complet
-00001de0: 656c 7920 6e65 7720 6f6e 6573 2e5c 6e5c  ely new ones.\n\
-00001df0: 6e54 6f20 6a75 7374 206d 6f64 6966 7920  nTo just modify 
-00001e00: 7468 6520 6578 6973 7469 6e67 206f 6e65  the existing one
-00001e10: 733a 5c6e 312e 2043 6f70 7920 7468 6520  s:\n1. Copy the 
-00001e20: 6275 696c 742d 696e 2074 656d 706c 6174  built-in templat
-00001e30: 6573 2069 6e74 6f20 6120 6e65 7720 6469  es into a new di
-00001e40: 7265 6374 6f72 793a 5c6e 2020 2060 6060  rectory:\n   ```
-00001e50: 7368 656c 6c20 7363 7269 7074 5c6e 2020  shell script\n  
-00001e60: 206d 6b64 6972 2063 7573 746f 6d5f 7465   mkdir custom_te
-00001e70: 6d70 6c61 7465 735c 6e20 2020 7365 7474  mplates\n   sett
-00001e80: 696e 6773 2d64 6f63 2074 656d 706c 6174  ings-doc templat
-00001e90: 6573 202d 2d63 6f70 792d 746f 2063 7573  es --copy-to cus
-00001ea0: 746f 6d5f 7465 6d70 6c61 7465 735c 6e20  tom_templates\n 
-00001eb0: 2020 6060 605c 6e32 2e20 4d6f 6469 6679    ```\n2. Modify
-00001ec0: 2074 6865 2074 656d 706c 6174 6520 636f   the template co
-00001ed0: 7069 6573 2069 6e20 6063 7573 746f 6d5f  pies in `custom_
-00001ee0: 7465 6d70 6c61 7465 7360 2074 6f20 7375  templates` to su
-00001ef0: 6974 2079 6f75 7220 6e65 6564 732e 2059  it your needs. Y
-00001f00: 6f75 2063 616e 206b 6565 7020 6f6e 6c79  ou can keep only
-00001f10: 2074 6865 206d 6f64 6966 6965 6420 6f6e   the modified on
-00001f20: 6573 2061 7320 6073 6574 7469 6e67 732d  es as `settings-
-00001f30: 646f 6360 2061 6c77 6179 7320 6661 6c6c  doc` always fall
-00001f40: 7320 6261 636b 2074 6f20 7468 6520 6275  s back to the bu
-00001f50: 696c 742d 696e 206f 6e65 732e 5c6e 332e  ilt-in ones.\n3.
-00001f60: 2055 7365 2074 6865 6d20 7768 656e 2067   Use them when g
-00001f70: 656e 6572 6174 696e 6720 7468 6520 646f  enerating the do
-00001f80: 6375 6d65 6e74 6174 696f 6e3a 5c6e 2020  cumentation:\n  
-00001f90: 2060 6060 7368 656c 6c20 7363 7269 7074   ```shell script
-00001fa0: 5c6e 2020 2073 6574 7469 6e67 732d 646f  \n   settings-do
-00001fb0: 6320 6765 6e65 7261 7465 205c 5c5c 6e20  c generate \\\n 
-00001fc0: 2020 2020 2d2d 636c 6173 7320 7372 632e      --class src.
-00001fd0: 7365 7474 696e 6773 2e41 7070 5365 7474  settings.AppSett
-00001fe0: 696e 6773 205c 5c5c 6e20 2020 2020 2d2d  ings \\\n     --
-00001ff0: 6f75 7470 7574 2d66 6f72 6d61 7420 646f  output-format do
-00002000: 7465 6e76 205c 5c5c 6e20 2020 2020 2d2d  tenv \\\n     --
-00002010: 7465 6d70 6c61 7465 7320 6375 7374 6f6d  templates custom
-00002020: 5f74 656d 706c 6174 6573 5c6e 2020 2060  _templates\n   `
-00002030: 6060 5c6e 5c6e 546f 2063 7265 6174 6520  ``\n\nTo create 
-00002040: 6e65 7720 6f6e 6573 2c20 6372 6561 7465  new ones, create
-00002050: 2061 2066 6f6c 6465 7220 616e 6420 7468   a folder and th
-00002060: 656e 2061 204a 696e 6a61 3220 7465 6d70  en a Jinja2 temp
-00002070: 6c61 7465 2077 6974 6820 6120 6669 6c65  late with a file
-00002080: 206e 616d 6573 2060 3c4f 5554 5055 545f   names `<OUTPUT_
-00002090: 464f 524d 4154 3e2e 6a69 6e6a 6160 2e20  FORMAT>.jinja`. 
-000020a0: 5468 656e 2073 696d 706c 7920 7265 6665  Then simply refe
-000020b0: 7265 6e63 6520 626f 7468 2069 6e20 7468  rence both in th
-000020c0: 6520 636f 6d6d 616e 6420 6c69 6e65 206f  e command line o
-000020d0: 7074 696f 6e73 3a5c 6e5c 6e60 6060 7368  ptions:\n\n```sh
-000020e0: 656c 6c20 7363 7269 7074 5c6e 6d6b 6469  ell script\nmkdi
-000020f0: 7220 6375 7374 6f6d 5f74 656d 706c 6174  r custom_templat
-00002100: 6573 5c6e 5c6e 6563 686f 2022 7b7b 2066  es\n\necho "{{ f
-00002110: 6965 6c64 2e74 6974 6c65 207d 7d22 203e  ield.title }}" >
-00002120: 2063 7573 746f 6d5f 7465 6d70 6c61 7465   custom_template
-00002130: 732f 6f6e 6c79 5f74 6974 6c65 732e 6a69  s/only_titles.ji
-00002140: 6e6a 615c 6e5c 6e73 6574 7469 6e67 732d  nja\n\nsettings-
-00002150: 646f 6320 6765 6e65 7261 7465 205c 5c5c  doc generate \\\
-00002160: 6e20 2d2d 636c 6173 7320 7372 632e 7365  n --class src.se
-00002170: 7474 696e 6773 2e41 7070 5365 7474 696e  ttings.AppSettin
-00002180: 6773 205c 5c5c 6e20 2d2d 6f75 7470 7574  gs \\\n --output
-00002190: 2d66 6f72 6d61 7420 6f6e 6c79 5f74 6974  -format only_tit
-000021a0: 6c65 7320 5c5c 5c6e 202d 2d74 656d 706c  les \\\n --templ
-000021b0: 6174 6573 2063 7573 746f 6d5f 7465 6d70  ates custom_temp
-000021c0: 6c61 7465 735c 6e60 6060 5c6e 5c6e 2323  lates\n```\n\n##
-000021d0: 2043 7573 746f 6d20 7365 7474 696e 6773   Custom settings
-000021e0: 2061 7474 7269 6275 7465 7320 696e 2074   attributes in t
-000021f0: 656d 706c 6174 6573 5c6e 5c6e 4279 2064  emplates\n\nBy d
-00002200: 6566 6175 6c74 2c20 7468 6572 6520 6172  efault, there ar
-00002210: 6520 7365 7665 7261 6c20 7661 7269 6162  e several variab
-00002220: 6c65 7320 6176 6169 6c61 626c 6520 696e  les available in
-00002230: 2061 6c6c 2074 656d 706c 6174 6573 3a5c   all templates:\
-00002240: 6e2d 2060 6865 6164 696e 675f 6f66 6673  n- `heading_offs
-00002250: 6574 6020 2d20 7468 6520 7661 6c75 6520  et` - the value 
-00002260: 6f66 2074 6865 2060 2d2d 6865 6164 696e  of the `--headin
-00002270: 672d 6f66 6673 6574 6020 6f70 7469 6f6e  g-offset` option
-00002280: 2e20 4465 6661 756c 7473 2074 6f20 6030  . Defaults to `0
-00002290: 602e 5c6e 2d20 6066 6965 6c64 7360 2074  `.\n- `fields` t
-000022a0: 6865 2076 616c 7565 206f 6620 6042 6173  he value of `Bas
-000022b0: 6553 6574 7469 6e67 732e 5f5f 6669 656c  eSettings.__fiel
-000022c0: 6473 5f5f 2e76 616c 7565 7328 2960 2e20  ds__.values()`. 
-000022d0: 496e 206f 7468 6572 2077 6f72 6473 2c20  In other words, 
-000022e0: 6120 6c69 7374 206f 6620 696e 6469 7669  a list of indivi
-000022f0: 6475 616c 2073 6574 7469 6e67 7320 6669  dual settings fi
-00002300: 656c 6473 2e20 4561 6368 2066 6965 6c64  elds. Each field
-00002310: 2069 7320 7468 656e 2061 6e20 696e 7374   is then an inst
-00002320: 616e 6365 206f 6620 5b60 4d6f 6465 6c46  ance of [`ModelF
-00002330: 6965 6c64 605d 2868 7474 7073 3a2f 2f67  ield`](https://g
-00002340: 6974 6875 622e 636f 6d2f 7361 6d75 656c  ithub.com/samuel
-00002350: 636f 6c76 696e 2f70 7964 616e 7469 632f  colvin/pydantic/
-00002360: 626c 6f62 2f6d 6173 7465 722f 7079 6461  blob/master/pyda
-00002370: 6e74 6963 2f66 6965 6c64 732e 7079 292e  ntic/fields.py).
-00002380: 2049 6620 6d75 6c74 6970 6c65 2063 6c61   If multiple cla
-00002390: 7373 6573 2061 7265 2075 7365 6420 746f  sses are used to
-000023a0: 2067 656e 6572 6174 6520 7468 6520 646f   generate the do
-000023b0: 6375 6d65 6e74 6174 696f 6e2c 2060 4d6f  cumentation, `Mo
-000023c0: 6465 6c46 6965 6c64 6073 2066 726f 6d20  delField`s from 
-000023d0: 616c 6c20 636c 6173 7365 7320 6172 6520  all classes are 
-000023e0: 636f 6c6c 6563 7465 6420 696e 746f 2060  collected into `
-000023f0: 6669 656c 6473 602e 2054 6865 2069 6e66  fields`. The inf
-00002400: 6f72 6d61 7469 6f6e 2061 626f 7574 206f  ormation about o
-00002410: 7269 6769 6e61 6c20 636c 6173 7365 7320  riginal classes 
-00002420: 6973 206e 6f74 2072 6574 6169 6e65 642e  is not retained.
-00002430: 5c6e 2d20 6063 6c61 7373 6573 6020 2d20  \n- `classes` - 
-00002440: 6120 6469 6374 696f 6e61 7279 2c20 7768  a dictionary, wh
-00002450: 6572 6520 6b65 7973 2061 7265 2074 6865  ere keys are the
-00002460: 2060 4261 7365 5365 7474 696e 6773 6020   `BaseSettings` 
-00002470: 7375 622d 636c 6173 7365 7320 616e 6420  sub-classes and 
-00002480: 7661 6c75 6573 2061 7265 206c 6973 7473  values are lists
-00002490: 206f 6620 6578 7472 6163 7465 6420 604d   of extracted `M
-000024a0: 6f64 656c 4669 656c 6460 7320 6f66 2074  odelField`s of t
-000024b0: 6861 7420 636c 6173 732e 2054 6869 7320  hat class. This 
-000024c0: 6361 6e20 6265 2075 7365 6420 666f 7220  can be used for 
-000024d0: 6578 616d 706c 6520 746f 2073 706c 6974  example to split
-000024e0: 2069 6e64 6976 6964 7561 6c20 636c 6173   individual clas
-000024f0: 7365 7320 696e 746f 2073 6563 7469 6f6e  ses into section
-00002500: 732e 5c6e 5c6e 4578 7472 6120 7061 7261  s.\n\nExtra para
-00002510: 6d65 7465 7273 2075 6e6b 6e6f 776e 2074  meters unknown t
-00002520: 6f20 7079 6461 6e74 6963 2061 7265 2073  o pydantic are s
-00002530: 746f 7265 6420 696e 2060 6669 656c 642e  tored in `field.
-00002540: 6669 656c 645f 696e 666f 2e65 7874 7261  field_info.extra
-00002550: 602e 2045 7861 6d70 6c65 7320 6f66 2073  `. Examples of s
-00002560: 7563 6820 7061 7261 6d65 7465 7273 2061  uch parameters a
-00002570: 7265 2060 6578 616d 706c 6560 2061 6e64  re `example` and
-00002580: 2060 706f 7373 6962 6c65 5f76 616c 7565   `possible_value
-00002590: 7360 2e5c 6e5c 6e45 7665 6e20 7468 6520  s`.\n\nEven the 
-000025a0: 6261 7265 2060 4d6f 6465 6c46 6965 6c64  bare `ModelField
-000025b0: 6020 7769 7468 6f75 7420 616e 7920 6578  ` without any ex
-000025c0: 7472 6120 7061 7261 6d65 7465 7273 2068  tra parameters h
-000025d0: 6173 2061 206c 6172 6765 206e 756d 6265  as a large numbe
-000025e0: 7220 6f66 2061 7474 7269 6275 7465 732e  r of attributes.
-000025f0: 2054 6f20 7365 6520 7468 656d 2061 6c6c   To see them all
-00002600: 2c20 7275 6e20 7468 6973 2060 7365 7474  , run this `sett
-00002610: 696e 6773 2d64 6f63 6020 7769 7468 2060  ings-doc` with `
-00002620: 2d2d 666f 726d 6174 2064 6562 7567 602e  --format debug`.
-00002630: 5c6e 5c6e 546f 2061 6363 6573 7320 696e  \n\nTo access in
-00002640: 666f 726d 6174 696f 6e20 6672 6f6d 2074  formation from t
-00002650: 6865 2060 4261 7365 5365 7474 696e 6773  he `BaseSettings
-00002660: 6020 636c 6173 7365 732c 2075 7365 2074  ` classes, use t
-00002670: 6865 2060 636c 6173 7365 7360 2076 6172  he `classes` var
-00002680: 6961 626c 6520 696e 2074 6865 2074 656d  iable in the tem
-00002690: 706c 6174 6573 3a5c 6e5c 6e60 6060 6a69  plates:\n\n```ji
-000026a0: 6e6a 6132 5c6e 7b25 2066 6f72 2063 6c73  nja2\n{% for cls
-000026b0: 2c20 6669 656c 6473 2069 6e20 636c 6173  , fields in clas
-000026c0: 7365 732e 6974 656d 7328 2920 257d 5c6e  ses.items() %}\n
-000026d0: 2320 7b7b 2063 6c73 2e5f 5f6e 616d 655f  # {{ cls.__name_
-000026e0: 5f20 7d7d 5c6e 7b25 2065 6e64 666f 7220  _ }}\n{% endfor 
-000026f0: 257d 5c6e 6060 605c 6e5c 6e23 2046 6561  %}\n```\n\n# Fea
-00002700: 7475 7265 7320 6f76 6572 7669 6577 5c6e  tures overview\n
-00002710: 5c6e 2d20 4f75 7470 7574 2069 6e74 6f20  \n- Output into 
-00002720: 7365 7665 7261 6c20 666f 726d 6174 7320  several formats 
-00002730: 7769 7468 2060 2d2d 6f75 7470 7574 2d66  with `--output-f
-00002740: 6f72 6d61 7460 3a20 6d61 726b 646f 776e  ormat`: markdown
-00002750: 2c20 646f 7465 6e76 5c6e 2d20 5772 6974  , dotenv\n- Writ
-00002760: 6573 2069 6e74 6f20 7374 646f 7574 2062  es into stdout b
-00002770: 7920 6465 6661 756c 742c 2077 6869 6368  y default, which
-00002780: 2061 6c6c 6f77 7320 7069 7069 6e67 2074   allows piping t
-00002790: 6f20 6f74 6865 7220 746f 6f6c 7320 666f  o other tools fo
-000027a0: 7220 6675 7274 6865 7220 7072 6f63 6573  r further proces
-000027b0: 7369 6e67 2e5c 6e2d 2041 626c 6520 746f  sing.\n- Able to
-000027c0: 2075 7064 6174 6520 7370 6563 6966 6965   update specifie
-000027d0: 6420 6669 6c65 2077 6974 6820 602d 2d75  d file with `--u
-000027e0: 7064 6174 6560 2c20 6f70 7469 6f6e 616c  pdate`, optional
-000027f0: 6c79 2062 6574 7765 656e 2074 776f 2067  ly between two g
-00002800: 6976 656e 2073 7472 696e 6720 6d61 726b  iven string mark
-00002810: 7320 7769 7468 2060 2d2d 6265 7477 6565  s with `--betwee
-00002820: 6e60 2e20 5573 6566 756c 2066 6f72 206b  n`. Useful for k
-00002830: 6565 7069 6e67 2064 6f63 756d 656e 7461  eeping documenta
-00002840: 7469 6f6e 2075 7020 746f 2064 6174 652e  tion up to date.
-00002850: 5c6e 2d20 4164 6469 7469 6f6e 616c 2074  \n- Additional t
-00002860: 656d 706c 6174 6573 2061 6e64 2064 6566  emplates and def
-00002870: 6175 6c74 2074 656d 706c 6174 6520 6f76  ault template ov
-00002880: 6572 7269 6465 7320 7669 6120 602d 2d74  errides via `--t
-00002890: 656d 706c 6174 6573 602e 5c6e 5c6e 2323  emplates`.\n\n##
-000028a0: 204d 6172 6b64 6f77 6e5c 6e5c 6e2d 2041   Markdown\n\n- A
-000028b0: 6c6c 6f77 7320 7365 7474 696e 6720 6120  llows setting a 
-000028c0: 602d 2d68 6561 6469 6e67 2d6f 6666 7365  `--heading-offse
-000028d0: 7460 2074 6f20 6669 7420 696e 746f 2065  t` to fit into e
-000028e0: 7869 7374 696e 6720 646f 6375 6d65 6e74  xisting document
-000028f0: 6174 696f 6e2e 5c6e 2d20 496e 7465 6c6c  ation.\n- Intell
-00002900: 6967 656e 746c 7920 666f 726d 6174 7320  igently formats 
-00002910: 6578 616d 706c 6520 7661 6c75 6573 2061  example values a
-00002920: 733a 5c6e 2020 2d20 5369 6e67 6c65 206c  s:\n  - Single l
-00002930: 696e 6520 6966 2061 6c6c 2076 616c 7565  ine if all value
-00002940: 7320 6669 7420 7769 7468 696e 2037 3520  s fit within 75 
-00002950: 6368 6172 6163 7465 7273 2e5c 6e20 202d  characters.\n  -
-00002960: 204c 6973 7420 6f66 2076 616c 7565 7320   List of values 
-00002970: 6966 2061 6c6c 2076 616c 7565 7320 776f  if all values wo
-00002980: 6e5c 2774 2066 6974 206f 6e20 6120 7369  n\'t fit on a si
-00002990: 6e67 6c65 206c 696e 652e 5c6e 2020 2d20  ngle line.\n  - 
-000029a0: 4c69 7374 206f 6620 603c 5641 4c55 453e  List of `<VALUE>
-000029b0: 3a20 3c44 4553 4352 4950 5449 4f4e 3e60  : <DESCRIPTION>`
-000029c0: 2069 6620 6578 616d 706c 6520 7661 6c75   if example valu
-000029d0: 6573 2061 7265 2074 7570 6c65 7320 6f66  es are tuples of
-000029e0: 2031 2d32 2069 7465 6d73 2e5c 6e5c 6e23   1-2 items.\n\n#
-000029f0: 2320 2e65 6e76 5c6e 5c6e 2d20 4c65 6176  # .env\n\n- Leav
-00002a00: 6573 2065 6e76 6972 6f6e 6d65 6e74 2076  es environment v
-00002a10: 6172 6961 626c 6573 2063 6f6d 6d65 6e74  ariables comment
-00002a20: 6564 2069 6620 7468 6579 2068 6176 6520  ed if they have 
-00002a30: 6120 6465 6661 756c 7420 7661 6c75 6520  a default value 
-00002a40: 6173 2074 6865 2061 7070 2064 6f65 736e  as the app doesn
-00002a50: 5c27 7420 7265 7175 6972 6520 7468 656d  \'t require them
-00002a60: 2e5c 6e27 2c0a 2020 2020 2761 7574 686f  .\n',.    'autho
-00002a70: 7227 3a20 2752 6164 656b 204c c3a1 7427  r': 'Radek L..t'
-00002a80: 2c0a 2020 2020 2761 7574 686f 725f 656d  ,.    'author_em
-00002a90: 6169 6c27 3a20 2772 6164 656b 2e6c 6174  ail': 'radek.lat
-00002aa0: 4067 6d61 696c 2e63 6f6d 272c 0a20 2020  @gmail.com',.   
-00002ab0: 2027 6d61 696e 7461 696e 6572 273a 2027   'maintainer': '
-00002ac0: 4e6f 6e65 272c 0a20 2020 2027 6d61 696e  None',.    'main
-00002ad0: 7461 696e 6572 5f65 6d61 696c 273a 2027  tainer_email': '
-00002ae0: 4e6f 6e65 272c 0a20 2020 2027 7572 6c27  None',.    'url'
-00002af0: 3a20 2768 7474 7073 3a2f 2f67 6974 6875  : 'https://githu
-00002b00: 622e 636f 6d2f 7261 6465 6b6c 6174 2f73  b.com/radeklat/s
-00002b10: 6574 7469 6e67 732d 646f 6327 2c0a 2020  ettings-doc',.  
-00002b20: 2020 2770 6163 6b61 6765 5f64 6972 273a    'package_dir':
-00002b30: 2070 6163 6b61 6765 5f64 6972 2c0a 2020   package_dir,.  
-00002b40: 2020 2770 6163 6b61 6765 7327 3a20 7061    'packages': pa
-00002b50: 636b 6167 6573 2c0a 2020 2020 2770 6163  ckages,.    'pac
-00002b60: 6b61 6765 5f64 6174 6127 3a20 7061 636b  kage_data': pack
-00002b70: 6167 655f 6461 7461 2c0a 2020 2020 2769  age_data,.    'i
-00002b80: 6e73 7461 6c6c 5f72 6571 7569 7265 7327  nstall_requires'
-00002b90: 3a20 696e 7374 616c 6c5f 7265 7175 6972  : install_requir
-00002ba0: 6573 2c0a 2020 2020 2765 6e74 7279 5f70  es,.    'entry_p
-00002bb0: 6f69 6e74 7327 3a20 656e 7472 795f 706f  oints': entry_po
-00002bc0: 696e 7473 2c0a 2020 2020 2770 7974 686f  ints,.    'pytho
-00002bd0: 6e5f 7265 7175 6972 6573 273a 2027 3e3d  n_requires': '>=
-00002be0: 332e 372e 322c 3c3d 332e 3131 272c 0a7d  3.7.2,<=3.11',.}
-00002bf0: 0a0a 0a73 6574 7570 282a 2a73 6574 7570  ...setup(**setup
-00002c00: 5f6b 7761 7267 7329 0a                   _kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7365 7474  : 2.1.Name: sett
+00000020: 696e 6773 2d64 6f63 0a56 6572 7369 6f6e  ings-doc.Version
+00000030: 3a20 322e 302e 300a 5375 6d6d 6172 793a  : 2.0.0.Summary:
+00000040: 2041 2063 6f6d 6d61 6e64 206c 696e 6520   A command line 
+00000050: 746f 6f6c 2066 6f72 2067 656e 6572 6174  tool for generat
+00000060: 696e 6720 4d61 726b 646f 776e 2064 6f63  ing Markdown doc
+00000070: 756d 656e 7461 7469 6f6e 2061 6e64 202e  umentation and .
+00000080: 656e 7620 6669 6c65 7320 6672 6f6d 2070  env files from p
+00000090: 7964 616e 7469 6320 4261 7365 5365 7474  ydantic BaseSett
+000000a0: 696e 6773 2e0a 486f 6d65 2d70 6167 653a  ings..Home-page:
+000000b0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000000c0: 636f 6d2f 7261 6465 6b6c 6174 2f73 6574  com/radeklat/set
+000000d0: 7469 6e67 732d 646f 630a 4c69 6365 6e73  tings-doc.Licens
+000000e0: 653a 204d 4954 0a4b 6579 776f 7264 733a  e: MIT.Keywords:
+000000f0: 2064 6f63 756d 656e 7461 7469 6f6e 2c65   documentation,e
+00000100: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00000110: 626c 6573 2c67 656e 6572 6174 6564 2c6d  bles,generated,m
+00000120: 6172 6b64 6f77 6e2c 4261 7365 5365 7474  arkdown,BaseSett
+00000130: 696e 6773 0a41 7574 686f 723a 2052 6164  ings.Author: Rad
+00000140: 656b 204c c3a1 740a 4175 7468 6f72 2d65  ek L..t.Author-e
+00000150: 6d61 696c 3a20 7261 6465 6b2e 6c61 7440  mail: radek.lat@
+00000160: 676d 6169 6c2e 636f 6d0a 5265 7175 6972  gmail.com.Requir
+00000170: 6573 2d50 7974 686f 6e3a 203e 3d33 2e38  es-Python: >=3.8
+00000180: 2c3c 342e 300a 436c 6173 7369 6669 6572  ,<4.0.Classifier
+00000190: 3a20 4465 7665 6c6f 706d 656e 7420 5374  : Development St
+000001a0: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
+000001b0: 7563 7469 6f6e 2f53 7461 626c 650a 436c  uction/Stable.Cl
+000001c0: 6173 7369 6669 6572 3a20 456e 7669 726f  assifier: Enviro
+000001d0: 6e6d 656e 7420 3a3a 2043 6f6e 736f 6c65  nment :: Console
+000001e0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+000001f0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000200: 3a20 4465 7665 6c6f 7065 7273 0a43 6c61  : Developers.Cla
+00000210: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000220: 6420 4175 6469 656e 6365 203a 3a20 5379  d Audience :: Sy
+00000230: 7374 656d 2041 646d 696e 6973 7472 6174  stem Administrat
+00000240: 6f72 730a 436c 6173 7369 6669 6572 3a20  ors.Classifier: 
+00000250: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000260: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000270: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+00000280: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+00000290: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000002a0: 6e64 656e 740a 436c 6173 7369 6669 6572  ndent.Classifier
+000002b0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000002c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000002d0: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
+000002e0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000300: 203a 3a20 332e 380a 436c 6173 7369 6669   :: 3.8.Classifi
+00000310: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000330: 6f6e 203a 3a20 332e 390a 436c 6173 7369  on :: 3.9.Classi
+00000340: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000350: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000360: 7468 6f6e 203a 3a20 332e 3130 0a43 6c61  thon :: 3.10.Cla
+00000370: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000380: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000390: 2050 7974 686f 6e20 3a3a 2033 2e31 310a   Python :: 3.11.
+000003a0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000003b0: 6320 3a3a 2044 6f63 756d 656e 7461 7469  c :: Documentati
+000003c0: 6f6e 0a43 6c61 7373 6966 6965 723a 2054  on.Classifier: T
+000003d0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+000003e0: 2044 6576 656c 6f70 6d65 6e74 0a43 6c61   Development.Cla
+000003f0: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+00000400: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000410: 6f70 6d65 6e74 203a 3a20 446f 6375 6d65  opment :: Docume
+00000420: 6e74 6174 696f 6e0a 436c 6173 7369 6669  ntation.Classifi
+00000430: 6572 3a20 546f 7069 6320 3a3a 2053 7973  er: Topic :: Sys
+00000440: 7465 6d20 3a3a 2049 6e73 7461 6c6c 6174  tem :: Installat
+00000450: 696f 6e2f 5365 7475 700a 436c 6173 7369  ion/Setup.Classi
+00000460: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+00000470: 7973 7465 6d20 3a3a 2053 6f66 7477 6172  ystem :: Softwar
+00000480: 6520 4469 7374 7269 6275 7469 6f6e 0a43  e Distribution.C
+00000490: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+000004a0: 203a 3a20 5379 7374 656d 203a 3a20 5379   :: System :: Sy
+000004b0: 7374 656d 7320 4164 6d69 6e69 7374 7261  stems Administra
+000004c0: 7469 6f6e 0a43 6c61 7373 6966 6965 723a  tion.Classifier:
+000004d0: 2054 6f70 6963 203a 3a20 5465 7874 2050   Topic :: Text P
+000004e0: 726f 6365 7373 696e 6720 3a3a 204d 6172  rocessing :: Mar
+000004f0: 6b75 7020 3a3a 204d 6172 6b64 6f77 6e0a  kup :: Markdown.
+00000500: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000510: 6320 3a3a 2055 7469 6c69 7469 6573 0a43  c :: Utilities.C
+00000520: 6c61 7373 6966 6965 723a 2054 7970 696e  lassifier: Typin
+00000530: 6720 3a3a 2054 7970 6564 0a52 6571 7569  g :: Typed.Requi
+00000540: 7265 732d 4469 7374 3a20 4a69 6e6a 6132  res-Dist: Jinja2
+00000550: 2028 3e3d 332e 302e 322c 3c34 2e30 2e30   (>=3.0.2,<4.0.0
+00000560: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000570: 2070 7964 616e 7469 6320 283e 3d31 2e38   pydantic (>=1.8
+00000580: 2e32 2c3c 322e 302e 3029 0a52 6571 7569  .2,<2.0.0).Requi
+00000590: 7265 732d 4469 7374 3a20 7479 7065 725b  res-Dist: typer[
+000005a0: 616c 6c5d 2028 3e3d 302e 392c 3c30 2e31  all] (>=0.9,<0.1
+000005b0: 3029 0a44 6573 6372 6970 7469 6f6e 2d43  0).Description-C
+000005c0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+000005d0: 742f 6d61 726b 646f 776e 0a0a 3c68 3120  t/markdown..<h1 
+000005e0: 616c 6967 6e3d 2263 656e 7465 7222 2073  align="center" s
+000005f0: 7479 6c65 3d22 626f 7264 6572 2d62 6f74  tyle="border-bot
+00000600: 746f 6d3a 206e 6f6e 653b 223e e29a 9926  tom: none;">...&
+00000610: 6e62 7370 3bf0 9f93 9d26 6e62 7370 3b26  nbsp;....&nbsp;&
+00000620: 6e62 7370 3b53 6574 7469 6e67 7326 6e62  nbsp;Settings&nb
+00000630: 7370 3b44 6f63 4765 6e26 6e62 7370 3b26  sp;DocGen&nbsp;&
+00000640: 6e62 7370 3bf0 9f93 9d26 6e62 7370 3be2  nbsp;....&nbsp;.
+00000650: 9a99 3c2f 6831 3e0a 3c68 3320 616c 6967  ..</h1>.<h3 alig
+00000660: 6e3d 2263 656e 7465 7222 3e41 2063 6f6d  n="center">A com
+00000670: 6d61 6e64 206c 696e 6520 746f 6f6c 2066  mand line tool f
+00000680: 6f72 2067 656e 6572 6174 696e 6720 4d61  or generating Ma
+00000690: 726b 646f 776e 2064 6f63 756d 656e 7461  rkdown documenta
+000006a0: 7469 6f6e 2061 6e64 202e 656e 7620 6669  tion and .env fi
+000006b0: 6c65 7320 6672 6f6d 203c 6120 6872 6566  les from <a href
+000006c0: 3d22 6874 7470 733a 2f2f 7079 6461 6e74  ="https://pydant
+000006d0: 6963 2d64 6f63 732e 6865 6c70 6d61 6e75  ic-docs.helpmanu
+000006e0: 616c 2e69 6f2f 7573 6167 652f 7365 7474  al.io/usage/sett
+000006f0: 696e 6773 223e 7079 6461 6e74 6963 2e42  ings">pydantic.B
+00000700: 6173 6553 6574 7469 6e67 733c 2f61 3e2e  aseSettings</a>.
+00000710: 3c2f 6833 3e0a 0a3c 7020 616c 6967 6e3d  </h3>..<p align=
+00000720: 2263 656e 7465 7222 3e0a 2020 2020 3c61  "center">.    <a
+00000730: 2068 7265 663d 2268 7474 7073 3a2f 2f61   href="https://a
+00000740: 7070 2e63 6972 636c 6563 692e 636f 6d2f  pp.circleci.com/
+00000750: 7069 7065 6c69 6e65 732f 6769 7468 7562  pipelines/github
+00000760: 2f72 6164 656b 6c61 742f 7365 7474 696e  /radeklat/settin
+00000770: 6773 2d64 6f63 3f62 7261 6e63 683d 6d61  gs-doc?branch=ma
+00000780: 696e 223e 0a20 2020 2020 2020 203c 696d  in">.        <im
+00000790: 6720 616c 743d 2243 6972 636c 6543 4922  g alt="CircleCI"
+000007a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+000007b0: 672e 7368 6965 6c64 732e 696f 2f63 6972  g.shields.io/cir
+000007c0: 636c 6563 692f 6275 696c 642f 6769 7468  cleci/build/gith
+000007d0: 7562 2f72 6164 656b 6c61 742f 7365 7474  ub/radeklat/sett
+000007e0: 696e 6773 2d64 6f63 223e 0a20 2020 203c  ings-doc">.    <
+000007f0: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00000800: 2268 7474 7073 3a2f 2f61 7070 2e63 6f64  "https://app.cod
+00000810: 6563 6f76 2e69 6f2f 6768 2f72 6164 656b  ecov.io/gh/radek
+00000820: 6c61 742f 7365 7474 696e 6773 2d64 6f63  lat/settings-doc
+00000830: 2f22 3e0a 2020 2020 2020 2020 3c69 6d67  /">.        <img
+00000840: 2061 6c74 3d22 436f 6465 636f 7622 2073   alt="Codecov" s
+00000850: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000860: 7368 6965 6c64 732e 696f 2f63 6f64 6563  shields.io/codec
+00000870: 6f76 2f63 2f67 6974 6875 622f 7261 6465  ov/c/github/rade
+00000880: 6b6c 6174 2f73 6574 7469 6e67 732d 646f  klat/settings-do
+00000890: 6322 3e0a 2020 2020 3c2f 613e 0a20 2020  c">.    </a>.   
+000008a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000008b0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6164  //github.com/rad
+000008c0: 656b 6c61 742f 7365 7474 696e 6773 2d64  eklat/settings-d
+000008d0: 6f63 2f74 6167 7322 3e0a 2020 2020 2020  oc/tags">.      
+000008e0: 2020 3c69 6d67 2061 6c74 3d22 4769 7448    <img alt="GitH
+000008f0: 7562 2074 6167 2028 6c61 7465 7374 2053  ub tag (latest S
+00000900: 656d 5665 7229 2220 7372 633d 2268 7474  emVer)" src="htt
+00000910: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000920: 2e69 6f2f 6769 7468 7562 2f74 6167 2f72  .io/github/tag/r
+00000930: 6164 656b 6c61 742f 7365 7474 696e 6773  adeklat/settings
+00000940: 2d64 6f63 223e 0a20 2020 203c 2f61 3e0a  -doc">.    </a>.
+00000950: 2020 2020 3c69 6d67 2061 6c74 3d22 4d61      <img alt="Ma
+00000960: 696e 7465 6e61 6e63 6522 2073 7263 3d22  intenance" src="
+00000970: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000980: 6c64 732e 696f 2f6d 6169 6e74 656e 616e  lds.io/maintenan
+00000990: 6365 2f79 6573 2f32 3032 3322 3e0a 2020  ce/yes/2023">.  
+000009a0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000009b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7261  ://github.com/ra
+000009c0: 6465 6b6c 6174 2f73 6574 7469 6e67 732d  deklat/settings-
+000009d0: 646f 632f 636f 6d6d 6974 732f 6d61 696e  doc/commits/main
+000009e0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+000009f0: 616c 743d 2247 6974 4875 6220 6c61 7374  alt="GitHub last
+00000a00: 2063 6f6d 6d69 7422 2073 7263 3d22 6874   commit" src="ht
+00000a10: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000a20: 732e 696f 2f67 6974 6875 622f 6c61 7374  s.io/github/last
+00000a30: 2d63 6f6d 6d69 742f 7261 6465 6b6c 6174  -commit/radeklat
+00000a40: 2f73 6574 7469 6e67 732d 646f 6322 3e0a  /settings-doc">.
+00000a50: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+00000a60: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000a70: 7069 7374 6174 732e 6f72 672f 7061 636b  pistats.org/pack
+00000a80: 6167 6573 2f73 6574 7469 6e67 732d 646f  ages/settings-do
+00000a90: 6322 3e0a 2020 2020 2020 2020 3c69 6d67  c">.        <img
+00000aa0: 2061 6c74 3d22 5079 5049 202d 2044 6f77   alt="PyPI - Dow
+00000ab0: 6e6c 6f61 6473 2220 7372 633d 2268 7474  nloads" src="htt
+00000ac0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000ad0: 2e69 6f2f 7079 7069 2f64 6d2f 7365 7474  .io/pypi/dm/sett
+00000ae0: 696e 6773 2d64 6f63 223e 0a20 2020 203c  ings-doc">.    <
+00000af0: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00000b00: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000b10: 636f 6d2f 7261 6465 6b6c 6174 2f73 6574  com/radeklat/set
+00000b20: 7469 6e67 732d 646f 632f 626c 6f62 2f6d  tings-doc/blob/m
+00000b30: 6169 6e2f 4c49 4345 4e53 4522 3e0a 2020  ain/LICENSE">.  
+00000b40: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
+00000b50: 5079 5049 202d 204c 6963 656e 7365 2220  PyPI - License" 
+00000b60: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000b70: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000b80: 2f6c 2f73 6574 7469 6e67 732d 646f 6322  /l/settings-doc"
+00000b90: 3e0a 2020 2020 3c2f 613e 0a20 2020 203c  >.    </a>.    <
+00000ba0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000bb0: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
+00000bc0: 6f63 2f76 6572 7369 6f6e 732f 223e 0a20  oc/versions/">. 
+00000bd0: 2020 2020 2020 203c 696d 6720 616c 743d         <img alt=
+00000be0: 2250 7950 4920 2d20 5079 7468 6f6e 2056  "PyPI - Python V
+00000bf0: 6572 7369 6f6e 2220 7372 633d 2268 7474  ersion" src="htt
+00000c00: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000c10: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
+00000c20: 6f6e 732f 7365 7474 696e 6773 2d64 6f63  ons/settings-doc
+00000c30: 223e 0a20 2020 203c 2f61 3e0a 3c2f 703e  ">.    </a>.</p>
+00000c40: 0a0a 5468 6520 7361 6d65 2077 6179 2079  ..The same way y
+00000c50: 6f75 2061 7265 2061 626c 6520 746f 2067  ou are able to g
+00000c60: 656e 6572 6174 6520 4f70 656e 4150 4920  enerate OpenAPI 
+00000c70: 646f 6375 6d65 6e74 6174 696f 6e20 6672  documentation fr
+00000c80: 6f6d 205b 6070 7964 616e 7469 632e 4261  om [`pydantic.Ba
+00000c90: 7365 4d6f 6465 6c60 5d28 6874 7470 733a  seModel`](https:
+00000ca0: 2f2f 7079 6461 6e74 6963 2d64 6f63 732e  //pydantic-docs.
+00000cb0: 6865 6c70 6d61 6e75 616c 2e69 6f2f 7573  helpmanual.io/us
+00000cc0: 6167 652f 6d6f 6465 6c73 2f29 2c20 6073  age/models/), `s
+00000cd0: 6574 7469 6e67 732d 646f 6360 2061 6c6c  ettings-doc` all
+00000ce0: 6f77 7320 796f 7520 746f 2067 656e 6572  ows you to gener
+00000cf0: 6174 6520 646f 6375 6d65 6e74 6174 696f  ate documentatio
+00000d00: 6e20 6672 6f6d 205b 6070 7964 616e 7469  n from [`pydanti
+00000d10: 632e 4261 7365 5365 7474 696e 6773 605d  c.BaseSettings`]
+00000d20: 2868 7474 7073 3a2f 2f70 7964 616e 7469  (https://pydanti
+00000d30: 632d 646f 6373 2e68 656c 706d 616e 7561  c-docs.helpmanua
+00000d40: 6c2e 696f 2f75 7361 6765 2f73 6574 7469  l.io/usage/setti
+00000d50: 6e67 7329 2e0a 0a49 7420 6973 2070 6f77  ngs)...It is pow
+00000d60: 6572 6564 2062 7920 7468 6520 5b4a 696e  ered by the [Jin
+00000d70: 6a61 325d 2868 7474 7073 3a2f 2f6a 696e  ja2](https://jin
+00000d80: 6a61 2e70 616c 6c65 7473 7072 6f6a 6563  ja.palletsprojec
+00000d90: 7473 2e63 6f6d 2f65 6e2f 6c61 7465 7374  ts.com/en/latest
+00000da0: 2f29 2074 656d 706c 6174 696e 6720 656e  /) templating en
+00000db0: 6769 6e65 2061 6e64 205b 5479 7065 725d  gine and [Typer]
+00000dc0: 2868 7474 7073 3a2f 2f74 7970 6572 2e74  (https://typer.t
+00000dd0: 6961 6e67 6f6c 6f2e 636f 6d2f 2920 6672  iangolo.com/) fr
+00000de0: 616d 6577 6f72 6b2e 2049 6620 796f 7520  amework. If you 
+00000df0: 646f 6e27 7420 6c69 6b65 2074 6865 2062  don't like the b
+00000e00: 7569 6c74 2d69 6e20 7465 6d70 6c61 7465  uilt-in template
+00000e10: 732c 2079 6f75 2063 616e 2065 6173 696c  s, you can easil
+00000e20: 7920 6d6f 6469 6679 2074 6865 6d20 6f72  y modify them or
+00000e30: 2077 7269 7465 2063 6f6d 706c 6574 656c   write completel
+00000e40: 7920 6375 7374 6f6d 206f 6e65 732e 2041  y custom ones. A
+00000e50: 6c6c 2061 7474 7269 6275 7465 7320 6f66  ll attributes of
+00000e60: 2074 6865 205b 6042 6173 6553 6574 7469   the [`BaseSetti
+00000e70: 6e67 7360 5d28 6874 7470 733a 2f2f 7079  ngs`](https://py
+00000e80: 6461 6e74 6963 2d64 6f63 732e 6865 6c70  dantic-docs.help
+00000e90: 6d61 6e75 616c 2e69 6f2f 7573 6167 652f  manual.io/usage/
+00000ea0: 7365 7474 696e 6773 2920 6d6f 6465 6c73  settings) models
+00000eb0: 2061 7265 2065 7870 6f73 6564 2074 6f20   are exposed to 
+00000ec0: 7468 6520 7465 6d70 6c61 7465 732e 0a0a  the templates...
+00000ed0: 3c21 2d2d 0a20 2020 2048 6f77 2074 6f20  <!--.    How to 
+00000ee0: 6765 6e65 7261 7465 2054 4f43 2066 726f  generate TOC fro
+00000ef0: 6d20 5079 4368 6172 6d3a 0a20 2020 2068  m PyCharm:.    h
+00000f00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000f10: 6d2f 7673 6368 2f69 6465 612d 6d75 6c74  m/vsch/idea-mult
+00000f20: 696d 6172 6b64 6f77 6e2f 7769 6b69 2f54  imarkdown/wiki/T
+00000f30: 6162 6c65 2d6f 662d 436f 6e74 656e 7473  able-of-Contents
+00000f40: 2d45 7874 656e 7369 6f6e 0a2d 2d3e 0a5b  -Extension.-->.[
+00000f50: 544f 4320 6c65 7665 6c73 3d31 2c32 206d  TOC levels=1,2 m
+00000f60: 6172 6b64 6f77 6e20 666f 726d 6174 7465  arkdown formatte
+00000f70: 6420 6275 6c6c 6574 2068 6965 7261 7263  d bullet hierarc
+00000f80: 6879 5d3a 2023 2022 5461 626c 6520 6f66  hy]: # "Table of
+00000f90: 2063 6f6e 7465 6e74 220a 0a23 2054 6162   content"..# Tab
+00000fa0: 6c65 206f 6620 636f 6e74 656e 740a 2d20  le of content.- 
+00000fb0: 5b49 6e73 7461 6c6c 6174 696f 6e5d 2823  [Installation](#
+00000fc0: 696e 7374 616c 6c61 7469 6f6e 290a 2d20  installation).- 
+00000fd0: 5b55 7361 6765 5d28 2375 7361 6765 290a  [Usage](#usage).
+00000fe0: 2020 2d20 5b4d 696e 696d 616c 2065 7861    - [Minimal exa
+00000ff0: 6d70 6c65 5d28 236d 696e 696d 616c 2d65  mple](#minimal-e
+00001000: 7861 6d70 6c65 290a 2020 2d20 5b43 6c61  xample).  - [Cla
+00001010: 7373 2061 7574 6f2d 6469 7363 6f76 6572  ss auto-discover
+00001020: 795d 2823 636c 6173 732d 6175 746f 2d64  y](#class-auto-d
+00001030: 6973 636f 7665 7279 290a 2020 2d20 5b41  iscovery).  - [A
+00001040: 6464 696e 6720 6d6f 7265 2069 6e66 6f72  dding more infor
+00001050: 6d61 7469 6f6e 5d28 2361 6464 696e 672d  mation](#adding-
+00001060: 6d6f 7265 2d69 6e66 6f72 6d61 7469 6f6e  more-information
+00001070: 290a 2020 2d20 5b55 7064 6174 696e 6720  ).  - [Updating 
+00001080: 6578 6973 7469 6e67 2064 6f63 756d 656e  existing documen
+00001090: 7461 7469 6f6e 5d28 2375 7064 6174 696e  tation](#updatin
+000010a0: 672d 6578 6973 7469 6e67 2d64 6f63 756d  g-existing-docum
+000010b0: 656e 7461 7469 6f6e 290a 2d20 5b41 6476  entation).- [Adv
+000010c0: 616e 6365 6420 7573 6167 655d 2823 6164  anced usage](#ad
+000010d0: 7661 6e63 6564 2d75 7361 6765 290a 2020  vanced-usage).  
+000010e0: 2d20 5b43 7573 746f 6d20 7465 6d70 6c61  - [Custom templa
+000010f0: 7465 735d 2823 6375 7374 6f6d 2d74 656d  tes](#custom-tem
+00001100: 706c 6174 6573 290a 2020 2d20 5b43 7573  plates).  - [Cus
+00001110: 746f 6d20 7365 7474 696e 6773 2061 7474  tom settings att
+00001120: 7269 6275 7465 7320 696e 2074 656d 706c  ributes in templ
+00001130: 6174 6573 5d28 2363 7573 746f 6d2d 7365  ates](#custom-se
+00001140: 7474 696e 6773 2d61 7474 7269 6275 7465  ttings-attribute
+00001150: 732d 696e 2d74 656d 706c 6174 6573 290a  s-in-templates).
+00001160: 2d20 5b46 6561 7475 7265 7320 6f76 6572  - [Features over
+00001170: 7669 6577 5d28 2366 6561 7475 7265 732d  view](#features-
+00001180: 6f76 6572 7669 6577 290a 2020 2d20 5b4d  overview).  - [M
+00001190: 6172 6b64 6f77 6e5d 2823 6d61 726b 646f  arkdown](#markdo
+000011a0: 776e 290a 2020 2d20 5b2e 656e 765d 2823  wn).  - [.env](#
+000011b0: 656e 7629 0a0a 2320 496e 7374 616c 6c61  env)..# Installa
+000011c0: 7469 6f6e 0a0a 6060 600a 7069 7020 696e  tion..```.pip in
+000011d0: 7374 616c 6c20 7365 7474 696e 6773 2d64  stall settings-d
+000011e0: 6f63 0a60 6060 0a0a 2320 5573 6167 650a  oc.```..# Usage.
+000011f0: 0a53 6565 2060 7365 7474 696e 6773 2d64  .See `settings-d
+00001200: 6f63 202d 2d68 656c 7060 2066 6f72 2061  oc --help` for a
+00001210: 6c6c 206f 7074 696f 6e73 2e0a 0a23 2320  ll options...## 
+00001220: 4d69 6e69 6d61 6c20 6578 616d 706c 650a  Minimal example.
+00001230: 0a4c 6574 2773 2061 7373 756d 6520 7468  .Let's assume th
+00001240: 6520 666f 6c6c 6f77 696e 6720 5b60 4261  e following [`Ba
+00001250: 7365 5365 7474 696e 6773 605d 2868 7474  seSettings`](htt
+00001260: 7073 3a2f 2f70 7964 616e 7469 632d 646f  ps://pydantic-do
+00001270: 6373 2e68 656c 706d 616e 7561 6c2e 696f  cs.helpmanual.io
+00001280: 2f75 7361 6765 2f73 6574 7469 6e67 7329  /usage/settings)
+00001290: 2069 6e20 6073 7263 2f73 6574 7469 6e67   in `src/setting
+000012a0: 732e 7079 6020 6f66 2061 2070 726f 6a65  s.py` of a proje
+000012b0: 6374 3a0a 0a60 6060 7079 7468 6f6e 0a66  ct:..```python.f
+000012c0: 726f 6d20 7079 6461 6e74 6963 2069 6d70  rom pydantic imp
+000012d0: 6f72 7420 4261 7365 5365 7474 696e 6773  ort BaseSettings
+000012e0: 0a0a 636c 6173 7320 4170 7053 6574 7469  ..class AppSetti
+000012f0: 6e67 7328 4261 7365 5365 7474 696e 6773  ngs(BaseSettings
+00001300: 293a 0a20 2020 206c 6f67 6769 6e67 5f6c  ):.    logging_l
+00001310: 6576 656c 3a20 7374 720a 6060 600a 0a59  evel: str.```..Y
+00001320: 6f75 2063 616e 2067 656e 6572 6174 6520  ou can generate 
+00001330: 6120 4d61 726b 646f 776e 2064 6f63 756d  a Markdown docum
+00001340: 656e 7461 7469 6f6e 2069 6e74 6f20 7374  entation into st
+00001350: 646f 7574 2077 6974 683a 0a0a 6060 6073  dout with:..```s
+00001360: 6865 6c6c 2073 6372 6970 740a 7365 7474  hell script.sett
+00001370: 696e 6773 2d64 6f63 2067 656e 6572 6174  ings-doc generat
+00001380: 6520 2d2d 636c 6173 7320 7372 632e 7365  e --class src.se
+00001390: 7474 696e 6773 2e41 7070 5365 7474 696e  ttings.AppSettin
+000013a0: 6773 202d 2d6f 7574 7075 742d 666f 726d  gs --output-form
+000013b0: 6174 206d 6172 6b64 6f77 6e0a 6060 600a  at markdown.```.
+000013c0: 0a57 6869 6368 2077 696c 6c20 6f75 7470  .Which will outp
+000013d0: 7574 3a0a 0a60 6060 6d61 726b 646f 776e  ut:..```markdown
+000013e0: 0a23 2060 4c4f 4747 494e 475f 4c45 5645  .# `LOGGING_LEVE
+000013f0: 4c60 0a0a 2a2a 5265 7175 6972 6564 2a2a  L`..**Required**
+00001400: 0a60 6060 0a0a 5369 6d69 6c61 726c 792c  .```..Similarly,
+00001410: 2079 6f75 2063 616e 2067 656e 6572 6174   you can generat
+00001420: 6520 6120 602e 656e 7660 2066 696c 6520  e a `.env` file 
+00001430: 666f 7220 6c6f 6361 6c20 6465 7665 6c6f  for local develo
+00001440: 706d 656e 7420 7769 7468 3a0a 0a60 6060  pment with:..```
+00001450: 7368 656c 6c20 7363 7269 7074 0a73 6574  shell script.set
+00001460: 7469 6e67 732d 646f 6320 6765 6e65 7261  tings-doc genera
+00001470: 7465 202d 2d63 6c61 7373 2073 7263 2e73  te --class src.s
+00001480: 6574 7469 6e67 732e 4170 7053 6574 7469  ettings.AppSetti
+00001490: 6e67 7320 2d2d 6f75 7470 7574 2d66 6f72  ngs --output-for
+000014a0: 6d61 7420 646f 7465 6e76 0a60 6060 0a0a  mat dotenv.```..
+000014b0: 5768 6963 6820 7769 6c6c 206f 7574 7075  Which will outpu
+000014c0: 743a 0a0a 6060 6064 6f74 656e 760a 4c4f  t:..```dotenv.LO
+000014d0: 4747 494e 475f 4c45 5645 4c3d 0a0a 6060  GGING_LEVEL=..``
+000014e0: 600a 0a23 2320 436c 6173 7320 6175 746f  `..## Class auto
+000014f0: 2d64 6973 636f 7665 7279 0a0a 4966 2079  -discovery..If y
+00001500: 6f75 2068 6176 6520 6120 6d6f 6475 6c65  ou have a module
+00001510: 2077 6974 6820 6120 7369 6e67 6c65 2073   with a single s
+00001520: 6574 7469 6e67 7320 636c 6173 7320 6f72  ettings class or
+00001530: 2077 616e 7420 746f 206c 6f61 6420 6d75   want to load mu
+00001540: 6c74 6970 6c65 2063 6c61 7373 6573 2061  ltiple classes a
+00001550: 7420 6f6e 6365 2061 7320 6120 736f 7572  t once as a sour
+00001560: 6365 2c20 796f 7520 6361 6e20 616c 736f  ce, you can also
+00001570: 2075 7365 2074 6865 2060 2d2d 6d6f 6475   use the `--modu
+00001580: 6c65 6020 6f70 7469 6f6e 2e20 5468 6520  le` option. The 
+00001590: 666f 6c6c 6f77 696e 6720 6578 616d 706c  following exampl
+000015a0: 6520 776f 726b 7320 6578 6163 746c 7920  e works exactly 
+000015b0: 6c69 6b65 2074 6865 206f 6e65 2061 626f  like the one abo
+000015c0: 7665 2061 6e64 2077 696c 6c20 7573 6520  ve and will use 
+000015d0: 7468 6520 6041 7070 5365 7474 696e 6773  the `AppSettings
+000015e0: 6020 636c 6173 7320 6175 746f 6d61 7469  ` class automati
+000015f0: 6361 6c6c 792e 0a0a 6060 6073 6865 6c6c  cally...```shell
+00001600: 2073 6372 6970 740a 7365 7474 696e 6773   script.settings
+00001610: 2d64 6f63 2067 656e 6572 6174 6520 2d2d  -doc generate --
+00001620: 6d6f 6475 6c65 2073 7263 2e73 6574 7469  module src.setti
+00001630: 6e67 7320 2d2d 6f75 7470 7574 2d66 6f72  ngs --output-for
+00001640: 6d61 7420 646f 7465 6e76 0a60 6060 0a0a  mat dotenv.```..
+00001650: 4966 206d 756c 7469 706c 6520 636c 6173  If multiple clas
+00001660: 7365 7320 636f 6e74 6169 6e20 6120 6669  ses contain a fi
+00001670: 656c 6420 7769 7468 2074 6865 2073 616d  eld with the sam
+00001680: 6520 6e61 6d65 2c20 616c 6c20 696e 7374  e name, all inst
+00001690: 616e 6365 7320 7769 6c6c 2061 7070 6561  ances will appea
+000016a0: 7220 696e 2074 6865 206f 7574 7075 742e  r in the output.
+000016b0: 0a0a 2323 2041 6464 696e 6720 6d6f 7265  ..## Adding more
+000016c0: 2069 6e66 6f72 6d61 7469 6f6e 0a0a 596f   information..Yo
+000016d0: 7520 6361 6e20 6164 6420 616e 7920 6578  u can add any ex
+000016e0: 7472 6120 6669 656c 6420 7061 7261 6d65  tra field parame
+000016f0: 7465 7273 2074 6f20 7468 6520 7365 7474  ters to the sett
+00001700: 696e 6773 2e20 4279 2064 6566 6175 6c74  ings. By default
+00001710: 2c20 6073 6574 7469 6e67 732d 646f 6360  , `settings-doc`
+00001720: 2077 696c 6c20 7574 696c 6973 6520 7468   will utilise th
+00001730: 6520 6465 6661 756c 7420 7661 6c75 652c  e default value,
+00001740: 2077 6865 7468 6572 2074 6865 2070 6172   whether the par
+00001750: 616d 6574 6572 2069 7320 7265 7175 6972  ameter is requir
+00001760: 6564 206f 7220 6f70 7469 6f6e 616c 2c20  ed or optional, 
+00001770: 6465 7363 7269 7074 696f 6e2c 2065 7861  description, exa
+00001780: 6d70 6c65 2076 616c 7565 2c20 616e 6420  mple value, and 
+00001790: 6c69 7374 206f 6620 706f 7373 6962 6c65  list of possible
+000017a0: 2076 616c 7565 733a 0a0a 6060 6070 7974   values:..```pyt
+000017b0: 686f 6e0a 6672 6f6d 2070 7964 616e 7469  hon.from pydanti
+000017c0: 6320 696d 706f 7274 2042 6173 6553 6574  c import BaseSet
+000017d0: 7469 6e67 732c 2046 6965 6c64 0a0a 636c  tings, Field..cl
+000017e0: 6173 7320 4170 7053 6574 7469 6e67 7328  ass AppSettings(
+000017f0: 4261 7365 5365 7474 696e 6773 293a 0a20  BaseSettings):. 
+00001800: 2020 206c 6f67 6769 6e67 5f6c 6576 656c     logging_level
+00001810: 3a20 7374 7220 3d20 4669 656c 6428 0a20  : str = Field(. 
+00001820: 2020 2020 2020 2022 5741 524e 494e 4722         "WARNING"
+00001830: 2c0a 2020 2020 2020 2020 6465 7363 7269  ,.        descri
+00001840: 7074 696f 6e3d 224c 6f67 206c 6576 656c  ption="Log level
+00001850: 2e22 2c0a 2020 2020 2020 2020 6578 616d  .",.        exam
+00001860: 706c 653d 2260 5741 524e 494e 4760 222c  ple="`WARNING`",
+00001870: 0a20 2020 2020 2020 2070 6f73 7369 626c  .        possibl
+00001880: 655f 7661 6c75 6573 3d5b 2244 4542 5547  e_values=["DEBUG
+00001890: 222c 2022 494e 464f 222c 2022 5741 524e  ", "INFO", "WARN
+000018a0: 494e 4722 2c20 2245 5252 4f52 222c 2022  ING", "ERROR", "
+000018b0: 4352 4954 4943 414c 225d 2c0a 2020 2020  CRITICAL"],.    
+000018c0: 290a 6060 600a 0a57 6869 6368 2077 696c  ).```..Which wil
+000018d0: 6c20 6765 6e65 7261 7465 2074 6865 2066  l generate the f
+000018e0: 6f6c 6c6f 7769 6e67 206d 6172 6b64 6f77  ollowing markdow
+000018f0: 6e3a 0a0a 6060 606d 6172 6b64 6f77 6e0a  n:..```markdown.
+00001900: 2320 604c 4f47 4749 4e47 5f4c 4556 454c  # `LOGGING_LEVEL
+00001910: 600a 0a2a 4f70 7469 6f6e 616c 2a2c 2064  `..*Optional*, d
+00001920: 6566 6175 6c74 2076 616c 7565 3a20 6057  efault value: `W
+00001930: 4152 4e49 4e47 600a 0a4c 6f67 206c 6576  ARNING`..Log lev
+00001940: 656c 2e0a 0a23 2320 4578 616d 706c 6573  el...## Examples
+00001950: 0a0a 6057 4152 4e49 4e47 600a 0a23 2320  ..`WARNING`..## 
+00001960: 506f 7373 6962 6c65 2076 616c 7565 730a  Possible values.
+00001970: 0a60 4445 4255 4760 2c20 6049 4e46 4f60  .`DEBUG`, `INFO`
+00001980: 2c20 6057 4152 4e49 4e47 602c 2060 4552  , `WARNING`, `ER
+00001990: 524f 5260 2c20 6043 5249 5449 4341 4c60  ROR`, `CRITICAL`
+000019a0: 0a60 6060 0a0a 6f72 2060 2e65 6e76 6020  .```..or `.env` 
+000019b0: 6669 6c65 3a0a 0a60 6060 646f 7465 6e76  file:..```dotenv
+000019c0: 0a23 204c 6f67 206c 6576 656c 2e0a 2320  .# Log level..# 
+000019d0: 506f 7373 6962 6c65 2076 616c 7565 733a  Possible values:
+000019e0: 0a23 2020 2060 4445 4255 4760 2c20 6049  .#   `DEBUG`, `I
+000019f0: 4e46 4f60 2c20 6057 4152 4e49 4e47 602c  NFO`, `WARNING`,
+00001a00: 2060 4552 524f 5260 2c20 6043 5249 5449   `ERROR`, `CRITI
+00001a10: 4341 4c60 0a23 204c 4f47 4749 4e47 5f4c  CAL`.# LOGGING_L
+00001a20: 4556 454c 3d57 4152 4e49 4e47 0a60 6060  EVEL=WARNING.```
+00001a30: 0a0a 596f 7520 6361 6e20 6669 6e64 2065  ..You can find e
+00001a40: 7665 6e20 6d6f 7265 2063 6f6d 706c 6578  ven more complex
+00001a50: 2075 7361 6765 206f 6620 6073 6574 7469   usage of `setti
+00001a60: 6e67 732d 646f 6360 2069 6e20 5b6f 6e65  ngs-doc` in [one
+00001a70: 206f 6620 6d79 206f 7468 6572 2070 726f   of my other pro
+00001a80: 6a65 6374 735d 2868 7474 7073 3a2f 2f67  jects](https://g
+00001a90: 6974 6875 622e 636f 6d2f 7261 6465 6b6c  ithub.com/radekl
+00001aa0: 6174 2f6d 7174 742d 696e 666c 7578 6462  at/mqtt-influxdb
+00001ab0: 2d67 6174 6577 6179 2f62 6c6f 622f 6d61  -gateway/blob/ma
+00001ac0: 696e 2f52 4541 444d 452e 6d64 2365 6e76  in/README.md#env
+00001ad0: 6972 6f6e 6d65 6e74 2d76 6172 6961 626c  ironment-variabl
+00001ae0: 6573 292e 0a0a 2323 2055 7064 6174 696e  es)...## Updatin
+00001af0: 6720 6578 6973 7469 6e67 2064 6f63 756d  g existing docum
+00001b00: 656e 7461 7469 6f6e 0a0a 4974 2069 7320  entation..It is 
+00001b10: 706f 7373 6962 6c65 2074 6f20 6765 6e65  possible to gene
+00001b20: 7261 7465 2064 6f63 756d 656e 7461 7469  rate documentati
+00001b30: 6f6e 2069 6e74 6f20 616e 2065 7869 7374  on into an exist
+00001b40: 696e 6720 646f 6375 6d65 6e74 2e20 546f  ing document. To
+00001b50: 2066 6974 2077 6974 6820 7468 6520 6865   fit with the he
+00001b60: 6164 696e 6720 7374 7275 6374 7572 652c  ading structure,
+00001b70: 2079 6f75 2063 616e 2061 646a 7573 7420   you can adjust 
+00001b80: 7468 6520 6865 6164 696e 6720 6c65 7665  the heading leve
+00001b90: 6c73 2077 6974 6820 602d 2d68 6561 6469  ls with `--headi
+00001ba0: 6e67 2d6f 6666 7365 7460 2e20 4164 6469  ng-offset`. Addi
+00001bb0: 7469 6f6e 616c 6c79 2c20 796f 7520 6361  tionally, you ca
+00001bc0: 6e20 7370 6563 6966 7920 7468 6520 6c6f  n specify the lo
+00001bd0: 6361 7469 6f6e 2077 6865 7265 2074 6f20  cation where to 
+00001be0: 6765 6e65 7261 7465 2074 6865 2064 6f63  generate the doc
+00001bf0: 756d 656e 7461 7469 6f6e 2077 6974 6820  umentation with 
+00001c00: 7477 6f20 6d61 726b 7320 7365 7420 6279  two marks set by
+00001c10: 2060 2d2d 6265 7477 6565 6e20 3c53 5441   `--between <STA
+00001c20: 5254 204d 4152 4b3e 203c 454e 4420 4d41  RT MARK> <END MA
+00001c30: 524b 3e60 2e0a 0a4c 6574 2773 2061 7373  RK>`...Let's ass
+00001c40: 756d 6520 796f 7572 2060 5245 4144 4d45  ume your `README
+00001c50: 2e6d 6460 206c 6f6f 6b73 206c 696b 6520  .md` looks like 
+00001c60: 7468 6973 3a0a 0a60 6060 6d61 726b 646f  this:..```markdo
+00001c70: 776e 0a23 204d 7920 6170 700a 0a54 6869  wn.# My app..Thi
+00001c80: 7320 6170 7020 6973 2064 6973 7472 6962  s app is distrib
+00001c90: 7574 6573 2061 7320 6120 646f 636b 6572  utes as a docker
+00001ca0: 2069 6d61 6765 2061 6e64 2063 6f6e 6669   image and confi
+00001cb0: 6775 7261 626c 6520 7669 6120 656e 7669  gurable via envi
+00001cc0: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00001cd0: 732e 2053 6565 2074 6865 206c 6973 7420  s. See the list 
+00001ce0: 6265 6c6f 772e 0a0a 2320 456e 7669 726f  below...# Enviro
+00001cf0: 6e6d 656e 7420 7661 7269 6162 6c65 730a  nment variables.
+00001d00: 3c21 2d2d 2067 656e 6572 6174 6564 2065  <!-- generated e
+00001d10: 6e76 2e20 7661 7273 2e20 7374 6172 7420  nv. vars. start 
+00001d20: 2d2d 3e0a 3c21 2d2d 2067 656e 6572 6174  -->.<!-- generat
+00001d30: 6564 2065 6e76 2e20 7661 7273 2e20 656e  ed env. vars. en
+00001d40: 6420 2d2d 3e0a 6060 600a 0a57 6865 6e20  d -->.```..When 
+00001d50: 796f 7520 7275 6e3a 0a0a 6060 6073 6865  you run:..```she
+00001d60: 6c6c 2073 6372 6970 740a 7365 7474 696e  ll script.settin
+00001d70: 6773 2d64 6f63 2067 656e 6572 6174 6520  gs-doc generate 
+00001d80: 5c0a 2020 2d2d 636c 6173 7320 7372 632e  \.  --class src.
+00001d90: 7365 7474 696e 6773 2e41 7070 5365 7474  settings.AppSett
+00001da0: 696e 6773 205c 0a20 202d 2d6f 7574 7075  ings \.  --outpu
+00001db0: 742d 666f 726d 6174 206d 6172 6b64 6f77  t-format markdow
+00001dc0: 6e20 5c20 0a20 202d 2d75 7064 6174 6520  n \ .  --update 
+00001dd0: 5245 4144 4d45 2e6d 6420 5c0a 2020 2d2d  README.md \.  --
+00001de0: 6265 7477 6565 6e20 223c 212d 2d20 6765  between "<!-- ge
+00001df0: 6e65 7261 7465 6420 656e 762e 2076 6172  nerated env. var
+00001e00: 732e 2073 7461 7274 202d 2d3e 2220 223c  s. start -->" "<
+00001e10: 212d 2d20 6765 6e65 7261 7465 6420 656e  !-- generated en
+00001e20: 762e 2076 6172 732e 2065 6e64 202d 2d3e  v. vars. end -->
+00001e30: 2220 5c0a 2020 2d2d 6865 6164 696e 672d  " \.  --heading-
+00001e40: 6f66 6673 6574 2031 0a60 6060 0a0a 7468  offset 1.```..th
+00001e50: 6520 7570 6461 7465 6420 6052 4541 444d  e updated `READM
+00001e60: 452e 6d64 6020 7769 6c6c 2067 6574 206f  E.md` will get o
+00001e70: 6e6c 7920 7468 6520 7370 6563 6966 6965  nly the specifie
+00001e80: 6420 6c6f 6361 7469 6f6e 206f 7665 7277  d location overw
+00001e90: 7269 7474 656e 3a0a 0a60 6060 6d61 726b  ritten:..```mark
+00001ea0: 646f 776e 0a23 204d 7920 6170 700a 0a54  down.# My app..T
+00001eb0: 6869 7320 6170 7020 6973 2064 6973 7472  his app is distr
+00001ec0: 6962 7574 6573 2061 7320 6120 646f 636b  ibutes as a dock
+00001ed0: 6572 2069 6d61 6765 2061 6e64 2063 6f6e  er image and con
+00001ee0: 6669 6775 7261 626c 6520 7669 6120 656e  figurable via en
+00001ef0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00001f00: 6c65 732e 2053 6565 2074 6865 206c 6973  les. See the lis
+00001f10: 7420 6265 6c6f 772e 0a0a 2320 456e 7669  t below...# Envi
+00001f20: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00001f30: 730a 3c21 2d2d 2067 656e 6572 6174 6564  s.<!-- generated
+00001f40: 2065 6e76 2e20 7661 7273 2e20 7374 6172   env. vars. star
+00001f50: 7420 2d2d 3e0a 2323 2060 4c4f 4747 494e  t -->.## `LOGGIN
+00001f60: 475f 4c45 5645 4c60 0a0a 2a4f 7074 696f  G_LEVEL`..*Optio
+00001f70: 6e61 6c2a 2c20 6465 6661 756c 7420 7661  nal*, default va
+00001f80: 6c75 653a 2060 5741 524e 494e 4760 0a0a  lue: `WARNING`..
+00001f90: 4c6f 6720 6c65 7665 6c2e 0a0a 2323 2320  Log level...### 
+00001fa0: 4578 616d 706c 6573 0a0a 6057 4152 4e49  Examples..`WARNI
+00001fb0: 4e47 600a 0a23 2323 2050 6f73 7369 626c  NG`..### Possibl
+00001fc0: 6520 7661 6c75 6573 0a0a 6044 4542 5547  e values..`DEBUG
+00001fd0: 602c 2060 494e 464f 602c 2060 5741 524e  `, `INFO`, `WARN
+00001fe0: 494e 4760 2c20 6045 5252 4f52 602c 2060  ING`, `ERROR`, `
+00001ff0: 4352 4954 4943 414c 600a 3c21 2d2d 2067  CRITICAL`.<!-- g
+00002000: 656e 6572 6174 6564 2065 6e76 2e20 7661  enerated env. va
+00002010: 7273 2e20 656e 6420 2d2d 3e0a 6060 600a  rs. end -->.```.
+00002020: 0a23 2041 6476 616e 6365 6420 7573 6167  .# Advanced usag
+00002030: 650a 0a23 2320 4375 7374 6f6d 2074 656d  e..## Custom tem
+00002040: 706c 6174 6573 0a0a 6073 6574 7469 6e67  plates..`setting
+00002050: 732d 646f 6360 2063 6f6d 6573 2077 6974  s-doc` comes wit
+00002060: 6820 6120 6665 7720 6275 696c 742d 696e  h a few built-in
+00002070: 2074 656d 706c 6174 6573 2e20 596f 7520   templates. You 
+00002080: 6361 6e20 6f76 6572 7269 6465 2074 6865  can override the
+00002090: 6d20 6f72 2077 7269 7465 2063 6f6d 706c  m or write compl
+000020a0: 6574 656c 7920 6e65 7720 6f6e 6573 2e0a  etely new ones..
+000020b0: 0a54 6f20 6a75 7374 206d 6f64 6966 7920  .To just modify 
+000020c0: 7468 6520 6578 6973 7469 6e67 206f 6e65  the existing one
+000020d0: 733a 0a31 2e20 436f 7079 2074 6865 2062  s:.1. Copy the b
+000020e0: 7569 6c74 2d69 6e20 7465 6d70 6c61 7465  uilt-in template
+000020f0: 7320 696e 746f 2061 206e 6577 2064 6972  s into a new dir
+00002100: 6563 746f 7279 3a0a 2020 2060 6060 7368  ectory:.   ```sh
+00002110: 656c 6c20 7363 7269 7074 0a20 2020 6d6b  ell script.   mk
+00002120: 6469 7220 6375 7374 6f6d 5f74 656d 706c  dir custom_templ
+00002130: 6174 6573 0a20 2020 7365 7474 696e 6773  ates.   settings
+00002140: 2d64 6f63 2074 656d 706c 6174 6573 202d  -doc templates -
+00002150: 2d63 6f70 792d 746f 2063 7573 746f 6d5f  -copy-to custom_
+00002160: 7465 6d70 6c61 7465 730a 2020 2060 6060  templates.   ```
+00002170: 0a32 2e20 4d6f 6469 6679 2074 6865 2074  .2. Modify the t
+00002180: 656d 706c 6174 6520 636f 7069 6573 2069  emplate copies i
+00002190: 6e20 6063 7573 746f 6d5f 7465 6d70 6c61  n `custom_templa
+000021a0: 7465 7360 2074 6f20 7375 6974 2079 6f75  tes` to suit you
+000021b0: 7220 6e65 6564 732e 2059 6f75 2063 616e  r needs. You can
+000021c0: 206b 6565 7020 6f6e 6c79 2074 6865 206d   keep only the m
+000021d0: 6f64 6966 6965 6420 6f6e 6573 2061 7320  odified ones as 
+000021e0: 6073 6574 7469 6e67 732d 646f 6360 2061  `settings-doc` a
+000021f0: 6c77 6179 7320 6661 6c6c 7320 6261 636b  lways falls back
+00002200: 2074 6f20 7468 6520 6275 696c 742d 696e   to the built-in
+00002210: 206f 6e65 732e 0a33 2e20 5573 6520 7468   ones..3. Use th
+00002220: 656d 2077 6865 6e20 6765 6e65 7261 7469  em when generati
+00002230: 6e67 2074 6865 2064 6f63 756d 656e 7461  ng the documenta
+00002240: 7469 6f6e 3a0a 2020 2060 6060 7368 656c  tion:.   ```shel
+00002250: 6c20 7363 7269 7074 0a20 2020 7365 7474  l script.   sett
+00002260: 696e 6773 2d64 6f63 2067 656e 6572 6174  ings-doc generat
+00002270: 6520 5c0a 2020 2020 202d 2d63 6c61 7373  e \.     --class
+00002280: 2073 7263 2e73 6574 7469 6e67 732e 4170   src.settings.Ap
+00002290: 7053 6574 7469 6e67 7320 5c0a 2020 2020  pSettings \.    
+000022a0: 202d 2d6f 7574 7075 742d 666f 726d 6174   --output-format
+000022b0: 2064 6f74 656e 7620 5c0a 2020 2020 202d   dotenv \.     -
+000022c0: 2d74 656d 706c 6174 6573 2063 7573 746f  -templates custo
+000022d0: 6d5f 7465 6d70 6c61 7465 730a 2020 2060  m_templates.   `
+000022e0: 6060 0a0a 546f 2063 7265 6174 6520 6e65  ``..To create ne
+000022f0: 7720 6f6e 6573 2c20 6372 6561 7465 2061  w ones, create a
+00002300: 2066 6f6c 6465 7220 616e 6420 7468 656e   folder and then
+00002310: 2061 204a 696e 6a61 3220 7465 6d70 6c61   a Jinja2 templa
+00002320: 7465 2077 6974 6820 6120 6669 6c65 206e  te with a file n
+00002330: 616d 6573 2060 3c4f 5554 5055 545f 464f  ames `<OUTPUT_FO
+00002340: 524d 4154 3e2e 6a69 6e6a 6160 2e20 5468  RMAT>.jinja`. Th
+00002350: 656e 2073 696d 706c 7920 7265 6665 7265  en simply refere
+00002360: 6e63 6520 626f 7468 2069 6e20 7468 6520  nce both in the 
+00002370: 636f 6d6d 616e 6420 6c69 6e65 206f 7074  command line opt
+00002380: 696f 6e73 3a0a 0a60 6060 7368 656c 6c20  ions:..```shell 
+00002390: 7363 7269 7074 0a6d 6b64 6972 2063 7573  script.mkdir cus
+000023a0: 746f 6d5f 7465 6d70 6c61 7465 730a 0a65  tom_templates..e
+000023b0: 6368 6f20 227b 7b20 6669 656c 642e 7469  cho "{{ field.ti
+000023c0: 746c 6520 7d7d 2220 3e20 6375 7374 6f6d  tle }}" > custom
+000023d0: 5f74 656d 706c 6174 6573 2f6f 6e6c 795f  _templates/only_
+000023e0: 7469 746c 6573 2e6a 696e 6a61 0a0a 7365  titles.jinja..se
+000023f0: 7474 696e 6773 2d64 6f63 2067 656e 6572  ttings-doc gener
+00002400: 6174 6520 5c0a 202d 2d63 6c61 7373 2073  ate \. --class s
+00002410: 7263 2e73 6574 7469 6e67 732e 4170 7053  rc.settings.AppS
+00002420: 6574 7469 6e67 7320 5c0a 202d 2d6f 7574  ettings \. --out
+00002430: 7075 742d 666f 726d 6174 206f 6e6c 795f  put-format only_
+00002440: 7469 746c 6573 205c 0a20 2d2d 7465 6d70  titles \. --temp
+00002450: 6c61 7465 7320 6375 7374 6f6d 5f74 656d  lates custom_tem
+00002460: 706c 6174 6573 0a60 6060 0a0a 2323 2043  plates.```..## C
+00002470: 7573 746f 6d20 7365 7474 696e 6773 2061  ustom settings a
+00002480: 7474 7269 6275 7465 7320 696e 2074 656d  ttributes in tem
+00002490: 706c 6174 6573 0a0a 4279 2064 6566 6175  plates..By defau
+000024a0: 6c74 2c20 7468 6572 6520 6172 6520 7365  lt, there are se
+000024b0: 7665 7261 6c20 7661 7269 6162 6c65 7320  veral variables 
+000024c0: 6176 6169 6c61 626c 6520 696e 2061 6c6c  available in all
+000024d0: 2074 656d 706c 6174 6573 3a0a 2d20 6068   templates:.- `h
+000024e0: 6561 6469 6e67 5f6f 6666 7365 7460 202d  eading_offset` -
+000024f0: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
+00002500: 6520 602d 2d68 6561 6469 6e67 2d6f 6666  e `--heading-off
+00002510: 7365 7460 206f 7074 696f 6e2e 2044 6566  set` option. Def
+00002520: 6175 6c74 7320 746f 2060 3060 2e0a 2d20  aults to `0`..- 
+00002530: 6066 6965 6c64 7360 2074 6865 2076 616c  `fields` the val
+00002540: 7565 206f 6620 6042 6173 6553 6574 7469  ue of `BaseSetti
+00002550: 6e67 732e 5f5f 6669 656c 6473 5f5f 2e76  ngs.__fields__.v
+00002560: 616c 7565 7328 2960 2e20 496e 206f 7468  alues()`. In oth
+00002570: 6572 2077 6f72 6473 2c20 6120 6c69 7374  er words, a list
+00002580: 206f 6620 696e 6469 7669 6475 616c 2073   of individual s
+00002590: 6574 7469 6e67 7320 6669 656c 6473 2e20  ettings fields. 
+000025a0: 4561 6368 2066 6965 6c64 2069 7320 7468  Each field is th
+000025b0: 656e 2061 6e20 696e 7374 616e 6365 206f  en an instance o
+000025c0: 6620 5b60 4d6f 6465 6c46 6965 6c64 605d  f [`ModelField`]
+000025d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000025e0: 636f 6d2f 7361 6d75 656c 636f 6c76 696e  com/samuelcolvin
+000025f0: 2f70 7964 616e 7469 632f 626c 6f62 2f6d  /pydantic/blob/m
+00002600: 6173 7465 722f 7079 6461 6e74 6963 2f66  aster/pydantic/f
+00002610: 6965 6c64 732e 7079 292e 2049 6620 6d75  ields.py). If mu
+00002620: 6c74 6970 6c65 2063 6c61 7373 6573 2061  ltiple classes a
+00002630: 7265 2075 7365 6420 746f 2067 656e 6572  re used to gener
+00002640: 6174 6520 7468 6520 646f 6375 6d65 6e74  ate the document
+00002650: 6174 696f 6e2c 2060 4d6f 6465 6c46 6965  ation, `ModelFie
+00002660: 6c64 6073 2066 726f 6d20 616c 6c20 636c  ld`s from all cl
+00002670: 6173 7365 7320 6172 6520 636f 6c6c 6563  asses are collec
+00002680: 7465 6420 696e 746f 2060 6669 656c 6473  ted into `fields
+00002690: 602e 2054 6865 2069 6e66 6f72 6d61 7469  `. The informati
+000026a0: 6f6e 2061 626f 7574 206f 7269 6769 6e61  on about origina
+000026b0: 6c20 636c 6173 7365 7320 6973 206e 6f74  l classes is not
+000026c0: 2072 6574 6169 6e65 642e 0a2d 2060 636c   retained..- `cl
+000026d0: 6173 7365 7360 202d 2061 2064 6963 7469  asses` - a dicti
+000026e0: 6f6e 6172 792c 2077 6865 7265 206b 6579  onary, where key
+000026f0: 7320 6172 6520 7468 6520 6042 6173 6553  s are the `BaseS
+00002700: 6574 7469 6e67 7360 2073 7562 2d63 6c61  ettings` sub-cla
+00002710: 7373 6573 2061 6e64 2076 616c 7565 7320  sses and values 
+00002720: 6172 6520 6c69 7374 7320 6f66 2065 7874  are lists of ext
+00002730: 7261 6374 6564 2060 4d6f 6465 6c46 6965  racted `ModelFie
+00002740: 6c64 6073 206f 6620 7468 6174 2063 6c61  ld`s of that cla
+00002750: 7373 2e20 5468 6973 2063 616e 2062 6520  ss. This can be 
+00002760: 7573 6564 2066 6f72 2065 7861 6d70 6c65  used for example
+00002770: 2074 6f20 7370 6c69 7420 696e 6469 7669   to split indivi
+00002780: 6475 616c 2063 6c61 7373 6573 2069 6e74  dual classes int
+00002790: 6f20 7365 6374 696f 6e73 2e0a 0a45 7874  o sections...Ext
+000027a0: 7261 2070 6172 616d 6574 6572 7320 756e  ra parameters un
+000027b0: 6b6e 6f77 6e20 746f 2070 7964 616e 7469  known to pydanti
+000027c0: 6320 6172 6520 7374 6f72 6564 2069 6e20  c are stored in 
+000027d0: 6066 6965 6c64 2e66 6965 6c64 5f69 6e66  `field.field_inf
+000027e0: 6f2e 6578 7472 6160 2e20 4578 616d 706c  o.extra`. Exampl
+000027f0: 6573 206f 6620 7375 6368 2070 6172 616d  es of such param
+00002800: 6574 6572 7320 6172 6520 6065 7861 6d70  eters are `examp
+00002810: 6c65 6020 616e 6420 6070 6f73 7369 626c  le` and `possibl
+00002820: 655f 7661 6c75 6573 602e 0a0a 4576 656e  e_values`...Even
+00002830: 2074 6865 2062 6172 6520 604d 6f64 656c   the bare `Model
+00002840: 4669 656c 6460 2077 6974 686f 7574 2061  Field` without a
+00002850: 6e79 2065 7874 7261 2070 6172 616d 6574  ny extra paramet
+00002860: 6572 7320 6861 7320 6120 6c61 7267 6520  ers has a large 
+00002870: 6e75 6d62 6572 206f 6620 6174 7472 6962  number of attrib
+00002880: 7574 6573 2e20 546f 2073 6565 2074 6865  utes. To see the
+00002890: 6d20 616c 6c2c 2072 756e 2074 6869 7320  m all, run this 
+000028a0: 6073 6574 7469 6e67 732d 646f 6360 2077  `settings-doc` w
+000028b0: 6974 6820 602d 2d66 6f72 6d61 7420 6465  ith `--format de
+000028c0: 6275 6760 2e0a 0a54 6f20 6163 6365 7373  bug`...To access
+000028d0: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
+000028e0: 6d20 7468 6520 6042 6173 6553 6574 7469  m the `BaseSetti
+000028f0: 6e67 7360 2063 6c61 7373 6573 2c20 7573  ngs` classes, us
+00002900: 6520 7468 6520 6063 6c61 7373 6573 6020  e the `classes` 
+00002910: 7661 7269 6162 6c65 2069 6e20 7468 6520  variable in the 
+00002920: 7465 6d70 6c61 7465 733a 0a0a 6060 606a  templates:..```j
+00002930: 696e 6a61 320a 7b25 2066 6f72 2063 6c73  inja2.{% for cls
+00002940: 2c20 6669 656c 6473 2069 6e20 636c 6173  , fields in clas
+00002950: 7365 732e 6974 656d 7328 2920 257d 0a23  ses.items() %}.#
+00002960: 207b 7b20 636c 732e 5f5f 6e61 6d65 5f5f   {{ cls.__name__
+00002970: 207d 7d0a 7b25 2065 6e64 666f 7220 257d   }}.{% endfor %}
+00002980: 0a60 6060 0a0a 2320 4665 6174 7572 6573  .```..# Features
+00002990: 206f 7665 7276 6965 770a 0a2d 204f 7574   overview..- Out
+000029a0: 7075 7420 696e 746f 2073 6576 6572 616c  put into several
+000029b0: 2066 6f72 6d61 7473 2077 6974 6820 602d   formats with `-
+000029c0: 2d6f 7574 7075 742d 666f 726d 6174 603a  -output-format`:
+000029d0: 206d 6172 6b64 6f77 6e2c 2064 6f74 656e   markdown, doten
+000029e0: 760a 2d20 5772 6974 6573 2069 6e74 6f20  v.- Writes into 
+000029f0: 7374 646f 7574 2062 7920 6465 6661 756c  stdout by defaul
+00002a00: 742c 2077 6869 6368 2061 6c6c 6f77 7320  t, which allows 
+00002a10: 7069 7069 6e67 2074 6f20 6f74 6865 7220  piping to other 
+00002a20: 746f 6f6c 7320 666f 7220 6675 7274 6865  tools for furthe
+00002a30: 7220 7072 6f63 6573 7369 6e67 2e0a 2d20  r processing..- 
+00002a40: 4162 6c65 2074 6f20 7570 6461 7465 2073  Able to update s
+00002a50: 7065 6369 6669 6564 2066 696c 6520 7769  pecified file wi
+00002a60: 7468 2060 2d2d 7570 6461 7465 602c 206f  th `--update`, o
+00002a70: 7074 696f 6e61 6c6c 7920 6265 7477 6565  ptionally betwee
+00002a80: 6e20 7477 6f20 6769 7665 6e20 7374 7269  n two given stri
+00002a90: 6e67 206d 6172 6b73 2077 6974 6820 602d  ng marks with `-
+00002aa0: 2d62 6574 7765 656e 602e 2055 7365 6675  -between`. Usefu
+00002ab0: 6c20 666f 7220 6b65 6570 696e 6720 646f  l for keeping do
+00002ac0: 6375 6d65 6e74 6174 696f 6e20 7570 2074  cumentation up t
+00002ad0: 6f20 6461 7465 2e0a 2d20 4164 6469 7469  o date..- Additi
+00002ae0: 6f6e 616c 2074 656d 706c 6174 6573 2061  onal templates a
+00002af0: 6e64 2064 6566 6175 6c74 2074 656d 706c  nd default templ
+00002b00: 6174 6520 6f76 6572 7269 6465 7320 7669  ate overrides vi
+00002b10: 6120 602d 2d74 656d 706c 6174 6573 602e  a `--templates`.
+00002b20: 0a0a 2323 204d 6172 6b64 6f77 6e0a 0a2d  ..## Markdown..-
+00002b30: 2041 6c6c 6f77 7320 7365 7474 696e 6720   Allows setting 
+00002b40: 6120 602d 2d68 6561 6469 6e67 2d6f 6666  a `--heading-off
+00002b50: 7365 7460 2074 6f20 6669 7420 696e 746f  set` to fit into
+00002b60: 2065 7869 7374 696e 6720 646f 6375 6d65   existing docume
+00002b70: 6e74 6174 696f 6e2e 0a2d 2049 6e74 656c  ntation..- Intel
+00002b80: 6c69 6765 6e74 6c79 2066 6f72 6d61 7473  ligently formats
+00002b90: 2065 7861 6d70 6c65 2076 616c 7565 7320   example values 
+00002ba0: 6173 3a0a 2020 2d20 5369 6e67 6c65 206c  as:.  - Single l
+00002bb0: 696e 6520 6966 2061 6c6c 2076 616c 7565  ine if all value
+00002bc0: 7320 6669 7420 7769 7468 696e 2037 3520  s fit within 75 
+00002bd0: 6368 6172 6163 7465 7273 2e0a 2020 2d20  characters..  - 
+00002be0: 4c69 7374 206f 6620 7661 6c75 6573 2069  List of values i
+00002bf0: 6620 616c 6c20 7661 6c75 6573 2077 6f6e  f all values won
+00002c00: 2774 2066 6974 206f 6e20 6120 7369 6e67  't fit on a sing
+00002c10: 6c65 206c 696e 652e 0a20 202d 204c 6973  le line..  - Lis
+00002c20: 7420 6f66 2060 3c56 414c 5545 3e3a 203c  t of `<VALUE>: <
+00002c30: 4445 5343 5249 5054 494f 4e3e 6020 6966  DESCRIPTION>` if
+00002c40: 2065 7861 6d70 6c65 2076 616c 7565 7320   example values 
+00002c50: 6172 6520 7475 706c 6573 206f 6620 312d  are tuples of 1-
+00002c60: 3220 6974 656d 732e 0a0a 2323 202e 656e  2 items...## .en
+00002c70: 760a 0a2d 204c 6561 7665 7320 656e 7669  v..- Leaves envi
+00002c80: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00002c90: 7320 636f 6d6d 656e 7465 6420 6966 2074  s commented if t
+00002ca0: 6865 7920 6861 7665 2061 2064 6566 6175  hey have a defau
+00002cb0: 6c74 2076 616c 7565 2061 7320 7468 6520  lt value as the 
+00002cc0: 6170 7020 646f 6573 6e27 7420 7265 7175  app doesn't requ
+00002cd0: 6972 6520 7468 656d 2e0a 0a              ire them...
```

