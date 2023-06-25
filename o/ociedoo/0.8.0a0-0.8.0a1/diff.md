# Comparing `tmp/ociedoo-0.8.0a0.tar.gz` & `tmp/ociedoo-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ociedoo-0.8.0a0.tar", max compression
+gzip compressed data, was "ociedoo-0.8.0a1.tar", max compression
```

## Comparing `ociedoo-0.8.0a0.tar` & `ociedoo-0.8.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34520 2019-04-24 20:34:30.919076 ociedoo-0.8.0a0/LICENSE
--rw-r--r--   0        0        0     3502 2022-10-24 21:32:42.859135 ociedoo-0.8.0a0/README.md
--rw-r--r--   0        0        0     1163 2023-02-27 13:42:26.177014 ociedoo-0.8.0a0/ociedoo/__init__.py
--rw-r--r--   0        0        0      126 2022-02-15 17:37:55.450743 ociedoo-0.8.0a0/ociedoo/__main__.py
--rw-r--r--   0        0        0     1826 2022-02-15 17:37:55.450743 ociedoo-0.8.0a0/ociedoo/check.py
--rw-r--r--   0        0        0    32817 2023-02-27 13:42:26.181014 ociedoo-0.8.0a0/ociedoo/cli.py
--rw-r--r--   0        0        0     5600 2023-02-23 15:08:27.899614 ociedoo-0.8.0a0/ociedoo/complete.py
--rw-r--r--   0        0        0      414 2023-02-27 13:42:26.181014 ociedoo-0.8.0a0/ociedoo/defaults/config
--rw-r--r--   0        0        0     9529 2023-02-27 13:42:26.181014 ociedoo-0.8.0a0/ociedoo/lib.py
--rw-r--r--   0        0        0     1332 2023-02-27 13:42:26.185014 ociedoo-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0     4606 2023-02-27 13:47:45.345838 ociedoo-0.8.0a0/setup.py
--rw-r--r--   0        0        0     4764 2023-02-27 13:47:45.346199 ociedoo-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2019-04-24 20:34:30.919076 ociedoo-0.8.0a1/LICENSE
+-rw-r--r--   0        0        0     3502 2022-10-24 21:32:42.859135 ociedoo-0.8.0a1/README.md
+-rw-r--r--   0        0        0     1163 2023-06-25 10:00:11.281181 ociedoo-0.8.0a1/ociedoo/__init__.py
+-rw-r--r--   0        0        0      126 2022-02-15 17:37:55.450743 ociedoo-0.8.0a1/ociedoo/__main__.py
+-rw-r--r--   0        0        0     1826 2022-02-15 17:37:55.450743 ociedoo-0.8.0a1/ociedoo/check.py
+-rw-r--r--   0        0        0    32817 2023-06-25 09:43:33.703960 ociedoo-0.8.0a1/ociedoo/cli.py
+-rw-r--r--   0        0        0     5647 2023-06-25 10:00:11.281181 ociedoo-0.8.0a1/ociedoo/complete.py
+-rw-r--r--   0        0        0      414 2023-06-25 09:43:33.703960 ociedoo-0.8.0a1/ociedoo/defaults/config
+-rw-r--r--   0        0        0     9529 2023-06-25 09:43:33.703960 ociedoo-0.8.0a1/ociedoo/lib.py
+-rw-r--r--   0        0        0     1332 2023-06-25 10:00:11.285182 ociedoo-0.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4606 2023-06-25 10:00:44.113989 ociedoo-0.8.0a1/setup.py
+-rw-r--r--   0        0        0     4764 2023-06-25 10:00:44.114423 ociedoo-0.8.0a1/PKG-INFO
```

### Comparing `ociedoo-0.8.0a0/LICENSE` & `ociedoo-0.8.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ociedoo-0.8.0a0/README.md` & `ociedoo-0.8.0a1/README.md`

 * *Files identical despite different names*

### Comparing `ociedoo-0.8.0a0/ociedoo/__init__.py` & `ociedoo-0.8.0a1/ociedoo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 from pathlib import Path
 
 from prgconfig import PrgConfig
 
 __productname__ = "ociedoo"
-__version__ = "0.8.0-alpha.0"
+__version__ = "0.8.0-alpha.1"
 __license__ = "GPL-3.0-or-later"
 
 # Path for default value for config file
 PGRNAME = "ociedoo"
 DEFAULTSPATH = str(Path(__file__).parent / Path("defaults"))
 DEFAULT_CONF = str(Path(DEFAULTSPATH) / "config")
```

### Comparing `ociedoo-0.8.0a0/ociedoo/check.py` & `ociedoo-0.8.0a1/ociedoo/check.py`

 * *Files identical despite different names*

### Comparing `ociedoo-0.8.0a0/ociedoo/cli.py` & `ociedoo-0.8.0a1/ociedoo/cli.py`

 * *Files identical despite different names*

### Comparing `ociedoo-0.8.0a0/ociedoo/complete.py` & `ociedoo-0.8.0a1/ociedoo/complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     """
     Return config object based on context and args.
     If ctx is empty then args should be parsed.
     If ctx is not empty then it means that config as already been loaded
     """
     # Check and read config file given in args if specified
     args = args if args else []
-    cfg = ctx.obj.get("cfg")
+    cfg = None
+    if ctx.obj is not None:
+        cfg = ctx.obj.get("cfg")
     if not cfg:
         cfg = config
         config_filename = None
         optflags = ("-c", "--config")
         for optflag in optflags:
             if optflag in args:
                 optindex = args.index(optflag)
```

### Comparing `ociedoo-0.8.0a0/ociedoo/lib.py` & `ociedoo-0.8.0a1/ociedoo/lib.py`

 * *Files identical despite different names*

### Comparing `ociedoo-0.8.0a0/pyproject.toml` & `ociedoo-0.8.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "ociedoo"
-version = "0.8.0-alpha.0"
+version = "0.8.0-alpha.1"
 description = "CLI tool to simplify the management of Odoo"
 authors = ["Coop IT Easy SCRLfs <remy@coopiteasy.be>"]
 maintainers = ["Rémy Taymans <remy@coopiteasy.be>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/coopiteasy/ociedoo"
 keywords = ["cli", "odoo", "coopiteasy"]
```

### Comparing `ociedoo-0.8.0a0/setup.py` & `ociedoo-0.8.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'sh>=1.12,<2.0']
 
 entry_points = \
 {'console_scripts': ['ociedoo = ociedoo.cli:main']}
 
 setup_kwargs = {
     'name': 'ociedoo',
-    'version': '0.8.0a0',
+    'version': '0.8.0a1',
     'description': 'CLI tool to simplify the management of Odoo',
     'long_description': '[![pipeline status](https://gitlab.com/coopiteasy/ociedoo/badges/master/pipeline.svg)](https://gitlab.com/coopiteasy/ociedoo)\n\nociedoo\n=======\n\nociedoo is a cli collection of tools to simplify the management of odoo\non a server.\n\nSee help for more info.\n\n\nInstallation\n------------\n\nociedoo needs python version >= 3.5. So ensure `pip` points to a correct\nversion of python. To do this run:\n```shell\npip --version\n```\n\nIt should return something like:\n```\npip xx.y from /path/to/pip (python 3.5)\n```\n\nIf `pip` doesn\'t run python >=3.5, try running `pip3` which is on\ncertain distribution the `pip` for python >=3.\n\n\n### Dependencies\n\nociedoo uses external programs via the shell. Be sure they are installed\nand accessible for the current user.\n\n- psql\n- createdb\n- dropdb\n- systemctl\n\n\n### Install for a specific user\n\n\n#### Installation with pipx (recommended python >= 3.6)\n\n```shell\npipx install ociedoo\n```\n\n\n#### Installation with pipsi (recommended python < 3.5)\n\n```shell\npipsi install ociedoo\n```\n\n\n#### Install with pip\n\n```shell\npip install --user ociedoo\n```\n\n\n### Install system wide (for all users)\n\n\n#### Install with pipx (recommended python >= 3.6)\n\nFirst install pipx if not already installed:\n```shell\nsudo pip install pipx\n```\n\nThen install ociedoo:\n```shell\nsudo PIPX_HOME=/usr/local PIPX_BIN_DIR=/usr/local/bin pipx install ociedoo\n```\n\n\n#### Install with pipsi (recommended python < 3.6)\n\nFirst install pipsi, if not already installed:\n```shell\nsudo curl https://raw.githubusercontent.com/mitsuhiko/pipsi/master/get-pipsi.py | sudo python3 - --bin-dir /usr/local/bin --home /usr/local/venvs --no-modify-path\n```\n\nThen install ociedoo:\n```shell\nsudo pipsi --bin-dir /usr/local/bin --home /usr/local/venvs install ociedoo\n```\n\n\n#### Install with pip\n```shell\nsudo pip install ociedoo\n```\n\n\n### Enable bash completion\n\n\n#### Bash completion for a specific user\n\nTo enable bash completion add the following in your `.bashrc`:\n\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source ociedoo)"\nfi\n```\n\nOr if you use zsh, add this to your `.zshrc`:\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source_zsh ociedoo)"\nfi\n```\n\n\n#### Bash completion system wide (for all users)\n\nTo enable bash completion add the following in `/etc/bash.bashrc`:\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source ociedoo)"\nfi\n```\n\nOr if you use zsh, add this to your `/etc/zsh/zshrc`:\n```shell\n# ociedoo\n# =======\nif command -v ociedoo >/dev/null; then\n    eval "$(_OCIEDOO_COMPLETE=source_zsh ociedoo)"\nfi\n```\n\n\nUpgrade\n-------\n\n\n### Upgrade for a specific user\n\n\n#### Upgrade with pipx (recommended python >= 3.6)\n\n```shell\npipx upgrade ociedoo\n```\n\n\n#### Upgrade with pipsi (recommended python < 3.5)\n\n```shell\npipsi upgrade ociedoo\n```\n\n\n#### Upgrade with pip\n\n```shell\npip install --user --upgrade ociedoo\n```\n\n\n### Upgrade system wide (for all users)\n\n\n#### Upgrade with pipx (recommended python >= 3.6)\n\n```shell\nsudo PIPX_HOME=/usr/local PIPX_BIN_DIR=/usr/local/bin pipx upgrade ociedoo\n```\n\n\n#### Upgrade with pipsi (recommended python < 3.5)\n\n```shell\nsudo pipsi --bin-dir /usr/local/bin --home /usr/local/venvs upgrade ociedoo\n```\n\n\n#### Upgrade with pip\n\n```shell\nsudo pip install --upgrade ociedoo\n```\n\nBuild and publish\n-----------------\n\nFirst do not forget to upgrade version. Then:\n\n```shell\npoetry build\npoetry publish -u coopiteasy\n',
     'author': 'Coop IT Easy SCRLfs',
     'author_email': 'remy@coopiteasy.be',
     'maintainer': 'Rémy Taymans',
     'maintainer_email': 'remy@coopiteasy.be',
     'url': 'https://gitlab.com/coopiteasy/ociedoo',
```

### Comparing `ociedoo-0.8.0a0/PKG-INFO` & `ociedoo-0.8.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ociedoo
-Version: 0.8.0a0
+Version: 0.8.0a1
 Summary: CLI tool to simplify the management of Odoo
 Home-page: https://gitlab.com/coopiteasy/ociedoo
 License: GPL-3.0-or-later
 Keywords: cli,odoo,coopiteasy
 Author: Coop IT Easy SCRLfs
 Author-email: remy@coopiteasy.be
 Maintainer: Rémy Taymans
```

