# Comparing `tmp/boxfish-0.1.1.tar.gz` & `tmp/boxfish-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxfish-0.1.1.tar", last modified: Wed Jun 29 21:11:57 2022, max compression
+gzip compressed data, was "boxfish-0.1.2.tar", last modified: Sun Jun 25 12:56:27 2023, max compression
```

## Comparing `boxfish-0.1.1.tar` & `boxfish-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-06-29 21:11:57.825597 boxfish-0.1.1/
--rw-rw-rw-   0        0        0     1092 2022-02-26 16:46:51.000000 boxfish-0.1.1/LICENSE
--rw-rw-rw-   0        0        0        2 2022-06-29 20:51:06.000000 boxfish-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3234 2022-06-29 21:11:57.825597 boxfish-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2464 2022-06-27 20:11:40.000000 boxfish-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-06-29 21:11:57.803612 boxfish-0.1.1/boxfish/
--rw-rw-rw-   0        0        0        5 2022-06-29 21:11:13.000000 boxfish-0.1.1/boxfish/VERSION
--rw-rw-rw-   0        0        0      473 2022-06-29 19:01:34.000000 boxfish-0.1.1/boxfish/__init__.py
--rw-rw-rw-   0        0        0       80 2022-02-26 14:48:45.000000 boxfish-0.1.1/boxfish/__main__.py
-drwxrwxrwx   0        0        0        0 2022-06-29 21:11:57.813604 boxfish-0.1.1/boxfish/data/
--rw-rw-rw-   0        0        0        0 2022-06-29 20:27:56.000000 boxfish-0.1.1/boxfish/data/__init__.py
--rw-rw-rw-   0        0        0    12329 2022-05-21 12:32:30.000000 boxfish-0.1.1/boxfish/data/config.py
--rw-rw-rw-   0        0        0    38119 2022-06-26 19:49:16.000000 boxfish-0.1.1/boxfish/data/soups.py
--rw-rw-rw-   0        0        0     4713 2022-06-26 20:07:57.000000 boxfish-0.1.1/boxfish/data/website.py
-drwxrwxrwx   0        0        0        0 2022-06-29 21:11:57.823599 boxfish-0.1.1/boxfish/utils/
--rw-rw-rw-   0        0        0        0 2022-06-29 20:27:56.000000 boxfish-0.1.1/boxfish/utils/__init__.py
--rw-rw-rw-   0        0        0     2041 2022-03-05 10:29:43.000000 boxfish-0.1.1/boxfish/utils/dataframes.py
--rw-rw-rw-   0        0        0     3919 2022-03-23 19:41:17.000000 boxfish-0.1.1/boxfish/utils/dicts.py
--rw-rw-rw-   0        0        0     6512 2022-04-02 12:41:15.000000 boxfish-0.1.1/boxfish/utils/drivers.py
--rw-rw-rw-   0        0        0     8473 2022-03-11 21:20:55.000000 boxfish-0.1.1/boxfish/utils/lists.py
--rw-rw-rw-   0        0        0     4875 2022-03-26 16:39:24.000000 boxfish-0.1.1/boxfish/utils/strings.py
--rw-rw-rw-   0        0        0     4736 2022-03-03 18:26:20.000000 boxfish-0.1.1/boxfish/utils/times.py
--rw-rw-rw-   0        0        0     5623 2022-06-26 09:44:35.000000 boxfish-0.1.1/boxfish/utils/urls.py
--rw-rw-rw-   0        0        0     3770 2022-03-01 20:36:06.000000 boxfish-0.1.1/boxfish/utils/utils.py
--rw-rw-rw-   0        0        0     3498 2022-02-26 14:48:44.000000 boxfish-0.1.1/boxfish/utils/xpaths.py
-drwxrwxrwx   0        0        0        0 2022-06-29 21:11:57.809606 boxfish-0.1.1/boxfish.egg-info/
--rw-rw-rw-   0        0        0     3234 2022-06-29 21:11:57.000000 boxfish-0.1.1/boxfish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2022-06-29 21:11:57.000000 boxfish-0.1.1/boxfish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-29 21:11:57.000000 boxfish-0.1.1/boxfish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-06-29 21:11:57.000000 boxfish-0.1.1/boxfish.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-29 21:11:57.000000 boxfish-0.1.1/boxfish.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-29 21:11:57.826599 boxfish-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2265 2022-06-29 21:10:04.000000 boxfish-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:56:27.306876 boxfish-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2022-02-26 16:46:51.000000 boxfish-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0        2 2022-06-29 20:51:06.000000 boxfish-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3335 2023-06-25 12:56:27.305887 boxfish-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2565 2023-06-25 12:49:03.000000 boxfish-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 12:56:27.283556 boxfish-0.1.2/boxfish/
+-rw-rw-rw-   0        0        0        5 2023-06-25 12:53:07.000000 boxfish-0.1.2/boxfish/VERSION
+-rw-rw-rw-   0        0        0      421 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-06-17 11:11:19.000000 boxfish-0.1.2/boxfish/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:56:27.293543 boxfish-0.1.2/boxfish/data/
+-rw-rw-rw-   0        0        0        0 2022-06-29 20:27:56.000000 boxfish-0.1.2/boxfish/data/__init__.py
+-rw-rw-rw-   0        0        0    12290 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/data/config.py
+-rw-rw-rw-   0        0        0    40561 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/data/soups.py
+-rw-rw-rw-   0        0        0     4941 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/data/website.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:56:27.304886 boxfish-0.1.2/boxfish/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-29 20:27:56.000000 boxfish-0.1.2/boxfish/utils/__init__.py
+-rw-rw-rw-   0        0        0     2132 2023-06-25 12:29:10.000000 boxfish-0.1.2/boxfish/utils/dataframes.py
+-rw-rw-rw-   0        0        0     4062 2023-06-25 11:28:23.000000 boxfish-0.1.2/boxfish/utils/dicts.py
+-rw-rw-rw-   0        0        0     6884 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/utils/drivers.py
+-rw-rw-rw-   0        0        0     8861 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/utils/lists.py
+-rw-rw-rw-   0        0        0     5048 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/utils/strings.py
+-rw-rw-rw-   0        0        0     5191 2023-06-25 12:29:10.000000 boxfish-0.1.2/boxfish/utils/times.py
+-rw-rw-rw-   0        0        0     5937 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/utils/urls.py
+-rw-rw-rw-   0        0        0     3818 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/utils/utils.py
+-rw-rw-rw-   0        0        0     3573 2023-06-25 12:29:18.000000 boxfish-0.1.2/boxfish/utils/xpaths.py
+drwxrwxrwx   0        0        0        0 2023-06-25 12:56:27.289535 boxfish-0.1.2/boxfish.egg-info/
+-rw-rw-rw-   0        0        0     3335 2023-06-25 12:56:27.000000 boxfish-0.1.2/boxfish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-25 12:56:27.000000 boxfish-0.1.2/boxfish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 12:56:27.000000 boxfish-0.1.2/boxfish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-25 12:56:27.000000 boxfish-0.1.2/boxfish.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 12:56:27.000000 boxfish-0.1.2/boxfish.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 12:56:27.306876 boxfish-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2259 2023-06-17 11:12:17.000000 boxfish-0.1.2/setup.py
```

### Comparing `boxfish-0.1.1/LICENSE` & `boxfish-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boxfish-0.1.1/PKG-INFO` & `boxfish-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxfish
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight tool for table extraction from HTML pages.
 Home-page: https://github.com/peterkorteweg/boxfish/
 Author: Peter Korteweg
 Author-email: boxfish@peterkorteweg.com
 License: MIT
 Keywords: beautifulsoup html pandas scraping tables
 Platform: UNKNOWN
@@ -24,15 +24,16 @@
 # boxfish: lightweight table extraction from HTML
 
 [![PyPI](https://img.shields.io/pypi/v/boxfish)](https://img.shields.io/pypi/v/boxfish)
 [![PyPI - Status](https://img.shields.io/pypi/status/boxfish)](https://img.shields.io/pypi/status/boxfish)
 [![PyPI - License](https://img.shields.io/pypi/l/boxfish)](https://img.shields.io/pypi/l/boxfish)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boxfish)](https://img.shields.io/pypi/pyversions/boxfish)
 
-[![GitHub top language](https://img.shields.io/github/languages/top/peterkorteweg/peterkorteweg)](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)
+[![GitHub top language](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ### What is it?
 Boxfish is a lightweight tool for table extraction from HTML pages. 
 
 ### Main features
 
 - Easy configuration. No knowledge of CSS or Xpaths required.
@@ -43,20 +44,20 @@
 
 
 ``` python
 import boxfish as bf
 import pandas as pd
 
 # Define table layout of an url with strings from two rows.
-aurl = ''
-row1 = ''
-row2 = ''
+aurl = ""
+row1 = ""
+row2 = ""
 
 # Build a configuration 
-aconfig = bf.build(url=aurl, astr = [row1, row2])
+aconfig = bf.build(url=aurl, rows = [row1, row2])
 
 # Extract a table
 data = bf.extract(aconfig, url=aurl)
 
 # View results
 df = pd.DataFrame(data)
 df.head()
```

### Comparing `boxfish-0.1.1/README.md` & `boxfish-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # boxfish: lightweight table extraction from HTML
 
 [![PyPI](https://img.shields.io/pypi/v/boxfish)](https://img.shields.io/pypi/v/boxfish)
 [![PyPI - Status](https://img.shields.io/pypi/status/boxfish)](https://img.shields.io/pypi/status/boxfish)
 [![PyPI - License](https://img.shields.io/pypi/l/boxfish)](https://img.shields.io/pypi/l/boxfish)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boxfish)](https://img.shields.io/pypi/pyversions/boxfish)
 
-[![GitHub top language](https://img.shields.io/github/languages/top/peterkorteweg/peterkorteweg)](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)
+[![GitHub top language](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ### What is it?
 Boxfish is a lightweight tool for table extraction from HTML pages. 
 
 ### Main features
 
 - Easy configuration. No knowledge of CSS or Xpaths required.
@@ -22,20 +23,20 @@
 
 
 ``` python
 import boxfish as bf
 import pandas as pd
 
 # Define table layout of an url with strings from two rows.
-aurl = ''
-row1 = ''
-row2 = ''
+aurl = ""
+row1 = ""
+row2 = ""
 
 # Build a configuration 
-aconfig = bf.build(url=aurl, astr = [row1, row2])
+aconfig = bf.build(url=aurl, rows = [row1, row2])
 
 # Extract a table
 data = bf.extract(aconfig, url=aurl)
 
 # View results
 df = pd.DataFrame(data)
 df.head()
```

### Comparing `boxfish-0.1.1/boxfish/data/config.py` & `boxfish-0.1.2/boxfish/data/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,207 +1,224 @@
 # config.py
 
 """Config is a module that contains functions for boxfish configuration"""
 
+
 import csv
 import os
 import pathlib
 import re
 import shutil
+from typing import Final, Tuple
+
+from bs4 import BeautifulSoup
 
-from boxfish.data import soups
 from boxfish import utils
+from boxfish.data import soups
 
-SEARCH_NAIVE = 'naive'
-SEARCH_STENCIL = 'tree'
-SEARCH_NONE = 'none'
-
-VERSION = (pathlib.Path(__file__).parent.parent / "VERSION").read_text()
-
-CONFIGKEYS = ['driver', 'html', 'output', 'boxfish']
-HTMLKEYS = ['url', 'parser', 'table', 'page']
-TABLEKEYS = ['id', 'rows', 'cols', 'include_strings', 'include_links']
-CONFIGTABLEKEYS = TABLEKEYS + ['search']
-PAGEKEYS = ['id', 'rows', 'index']
-OUTPUTKEYS = ['filename', 'date_format', 'overwrite', 'quoting']
-SEARCHTYPES = [SEARCH_NAIVE, SEARCH_STENCIL, SEARCH_NONE]
-
-BACKUP_EXT = '.bak'
-
-HEADERS = {'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:81.0) Gecko/20100101 Firefox/81.0',
-           'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
-           'accept-language': 'nl,en-US;q=0.7,en;q=0.3',
-           'accept-encoding': 'gzip, deflate, br'
-           }
+SEARCH_NAIVE: Final = "naive"
+SEARCH_STENCIL: Final = "tree"
+SEARCH_NONE: Final = "none"
+
+VERSION: Final = (pathlib.Path(__file__).parent.parent / "VERSION").read_text()
+
+CONFIGKEYS: Final = ["driver", "html", "output", "boxfish"]
+HTMLKEYS: Final = ["url", "parser", "table", "page"]
+TABLEKEYS: Final = ["id", "rows", "cols", "include_strings", "include_links"]
+CONFIGTABLEKEYS: Final = TABLEKEYS + ["search"]
+PAGEKEYS: Final = ["id", "rows", "index"]
+OUTPUTKEYS: Final = ["filename", "date_format", "overwrite", "quoting"]
+SEARCHTYPES: Final = [SEARCH_NAIVE, SEARCH_STENCIL, SEARCH_NONE]
+
+BACKUP_EXT: Final = ".bak"
+
+HEADERS: Final = {
+    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:81.0) Gecko/20100101 Firefox/81.0",
+    "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
+    "accept-language": "nl,en-US;q=0.7,en;q=0.3",
+    "accept-encoding": "gzip, deflate, br",
+}
 
 
 # Initialization
-def create(url=''):
-    """ Creates a boxfish configuration dictionary
+def create(url: str = "") -> dict:
+    """Creates a boxfish configuration dictionary
 
-        config = create(url)
+    config = create(url)
 
-        Args:
-            url (str): Url
+    Args:
+        url (str): Url
 
-        Returns:
-            config(dict)
+    Returns:
+        config(dict)
     """
 
     config = dict.fromkeys(CONFIGKEYS, {})
 
-    config['driver'] = utils.drivers.create_params(package='requests',
-                                                   headers=HEADERS,
-                                                   timeout=10,
-                                                   filename='',
-                                                   log='',
-                                                   sleep={'1': 1, '200': 3600},
-                                                   headless=True)
-
-    config['html'] = dict.fromkeys(HTMLKEYS, {})
-    config['html']['url'] = url
-    config['html']['parser'] = 'html.parser'
-
-    config['html']['table'] = dict.fromkeys(CONFIGTABLEKEYS, {})
-    config['html']['table']['id'] = dict.fromkeys(['elem', 'class'], {})
-    config['html']['table']['id']['elem'] = ''
-    config['html']['table']['id']['class'] = ['']
-    config['html']['table']['rows'] = dict.fromkeys(['elem', 'class'], {})
-    config['html']['table']['rows']['elem'] = ''
-    config['html']['table']['rows']['class'] = ['']
-    config['html']['table']['cols'] = {}
-    config['html']['table']['include_strings'] = True
-    config['html']['table']['include_links'] = True
-    config['html']['table']['search'] = SEARCH_NONE
-
-    config['html']['page'] = dict.fromkeys(PAGEKEYS, {})
-    config['html']['page']['id'] = {}
-    config['html']['page']['rows'] = dict.fromkeys(['elem', 'class'], {})
-    config['html']['page']['rows']['elem'] = ''
-    config['html']['page']['rows']['class'] = ['']
-    config['html']['page']['index'] = -1
-
-    config['output'] = dict.fromkeys(OUTPUTKEYS, {})
-    config['output']['filename'] = ''
-    config['output']['date_format'] = ''
-    config['output']['overwrite'] = False
-    config['output']['quoting'] = csv.QUOTE_NONNUMERIC
+    config["driver"] = utils.drivers.create_params(
+        package="requests",
+        headers=HEADERS,
+        timeout=10,
+        filename="",
+        log="",
+        sleep={"1": 1, "200": 3600},
+        headless=True,
+    )
+
+    config["html"] = dict.fromkeys(HTMLKEYS, {})
+    config["html"]["url"] = url
+    config["html"]["parser"] = "html.parser"
+
+    config["html"]["table"] = dict.fromkeys(CONFIGTABLEKEYS, {})
+    config["html"]["table"]["id"] = dict.fromkeys(["elem", "class"], {})
+    config["html"]["table"]["id"]["elem"] = ""
+    config["html"]["table"]["id"]["class"] = [""]
+    config["html"]["table"]["rows"] = dict.fromkeys(["elem", "class"], {})
+    config["html"]["table"]["rows"]["elem"] = ""
+    config["html"]["table"]["rows"]["class"] = [""]
+    config["html"]["table"]["cols"] = {}
+    config["html"]["table"]["include_strings"] = True
+    config["html"]["table"]["include_links"] = True
+    config["html"]["table"]["search"] = SEARCH_NONE
+
+    config["html"]["page"] = dict.fromkeys(PAGEKEYS, {})
+    config["html"]["page"]["id"] = {}
+    config["html"]["page"]["rows"] = dict.fromkeys(["elem", "class"], {})
+    config["html"]["page"]["rows"]["elem"] = ""
+    config["html"]["page"]["rows"]["class"] = [""]
+    config["html"]["page"]["index"] = -1
+
+    config["output"] = dict.fromkeys(OUTPUTKEYS, {})
+    config["output"]["filename"] = ""
+    config["output"]["date_format"] = ""
+    config["output"]["overwrite"] = False
+    config["output"]["quoting"] = csv.QUOTE_NONNUMERIC
 
-    config['boxfish']['version'] = VERSION
+    config["boxfish"]["version"] = VERSION
 
     return config
 
 
 # I/O
-def read(filename):
-    """ Read a boxfish configuration from file
+def read(filename: str) -> dict:
+    """Read a boxfish configuration from file
 
-        config = read(filename)
+    config = read(filename)
 
-        Args:
-            filename (str): file name of configuration
+    Args:
+        filename (str): file name of configuration
 
-        Returns:
-            config(dict)
+    Returns:
+        config(dict)
     """
 
     config = utils.utils.read_json(filename)
     if config is None:
-        print('Cannot find' + filename)
+        print("Cannot find" + filename)
 
     _process(config)
     return config
 
 
-def write(filename, config):
-    """ Write a boxfish configuration to file. Save current configuration to backup if exists
+def write(filename: str, config: dict) -> None:
+    """Write a boxfish configuration to file. Save current configuration to backup if exists
 
-        write(filename, config)
+    write(filename, config)
 
-        Args:
-            filename (str): file name of configuration
-            config (dict): configuration
+    Args:
+        filename (str): file name of configuration
+        config (dict): configuration
 
-        Returns:
-            None
+    Returns:
+        None
 
-        Raises:
-            IOError (): error in case function cannot write to filename
-        """
+    Raises:
+        IOError (): error in case function cannot write to filename
+    """
 
     if os.path.isfile(filename):
-        shutil.copy(filename, filename+BACKUP_EXT)
+        shutil.copy(filename, filename + BACKUP_EXT)
     utils.utils.write_json(filename, config)
 
 
-def revert(filename):
-    """ Revert a boxfish configuration file to backup.
-        Flips current configuration with backup configuration if both exist
-        Backup is determined by filename + BACKUP_EXT
+def revert(filename: str) -> None:
+    """Revert a boxfish configuration file to backup.
+    Flips current configuration with backup configuration if both exist
+    Backup is determined by filename + BACKUP_EXT
 
-        revert(filename)
+    revert(filename)
 
-        Args:
-            filename (str): file name of configuration
+    Args:
+        filename (str): file name of configuration
 
-        Returns:
-            None
+    Returns:
+        None
 
-        Raises:
-            IOError (): error in case function cannot write to filename
-        """
+    Raises:
+        IOError (): error in case function cannot write to filename
+    """
     utils.utils.flip(filename, filename + BACKUP_EXT)
 
 
 # Editing configurations
-def build(config=None, url='', rows=None, cols=None, search=SEARCH_STENCIL, next_page=''):
-    """ Build configuration
-
-        config = build(config, url= '', rows=[], cols=[], search='none')
-
-        Args:
-            config (dict): configuration
-            url (str): url
-            rows (list): list of strings from two rows
-            cols (list): list of strings from one or more columns
-            search (str): column search type SEARCHTYPES
-            next_page (str): url of next page
-
-        Returns:
-            config (dict): configuration
-
-        Examples:
-            # 1. Rows, no columns
-            config = build(config=config, url='', rows=[rowstring1,rowstring2], search='tree')
-            # 2. Columns, no rows
-            config = build(config=config, url='', cols=[colstring1, colstring2], search='tree')
-            # 3. Rows and columns
-            config = build(config=config, url='', rows=[rowstring1,rowstring2], cols=[colstring1, colstring2], search='tree')
+def build(
+    config: dict = None,
+    url: str = "",
+    rows: list = None,
+    cols: list = None,
+    search: str = SEARCH_STENCIL,
+    next_page: str = "",
+) -> dict:
+    """Build configuration
+
+    config = build(config, url= '', rows=[], cols=[], search='none')
+
+    Args:
+        config (dict): configuration
+        url (str): url
+        rows (list): list of strings from two rows
+        cols (list): list of strings from one or more columns
+        search (str): column search type SEARCHTYPES
+        next_page (str): url of next page
+
+    Returns:
+        config (dict): configuration
+
+    Examples:
+        # 1. Rows, no columns
+        config = build(config=config, url='', rows=[rowstring1,rowstring2], search='tree')
+        # 2. Columns, no rows
+        config = build(config=config, url='', cols=[colstring1, colstring2], search='tree')
+        # 3. Rows and columns
+        config = build(config=config, url='', rows=[rowstring1,rowstring2], cols=[colstring1, colstring2]
+        , search='tree')
 
     """
     if config is None:
         config = create(url)
     if len(url) == 0:
-        url = config['html']['url']
+        url = config["html"]["url"]
 
-    [pdriver] = utils.dicts.extract_values(config, ['driver'])
+    [pdriver] = utils.dicts.extract_values(config, ["driver"])
     page = utils.drivers.get_page(url=url, params=pdriver)
     soup = soups.get_soup(page)
 
     if soup:
         soups.wrap_navigable_strings(soup)
 
-        config = _build_table(soup, config, url=url, rows=rows, cols=cols, search=search)
+        config = _build_table(
+            soup, config, url=url, rows=rows, cols=cols, search=search
+        )
         config = _build_next_page(soup, config, next_page=next_page)
     return config
 
 
 # Private functions
-def _process(config):
-    """ Processes a configuration.
+def _process(config: dict) -> None:
+    """Processes a configuration.
     The function removes non-config keys
     The function adds missing config keys with default values, two levels deep
 
         _process(config)
 
         Args:
             config (dict): configuration
@@ -222,29 +239,36 @@
             config[key] = dconfig[key]
         else:
             for ckey in dconfig[key]:
                 if ckey not in config[key].keys():
                     config[key][ckey] = dconfig[key][ckey]
 
 
-def _build_table(soup, config, url='', rows=None, cols=None, search=SEARCH_STENCIL):
-    """ Build table configuration
-
-        config = _build_table(soup, config, url= '', rows=[], cols=[], search='none')
+def _build_table(
+    soup: BeautifulSoup,
+    config: dict,
+    url: str = "",
+    rows: list = None,
+    cols: list = None,
+    search: str = SEARCH_STENCIL,
+) -> dict:
+    """Build table configuration
+
+    config = _build_table(soup, config, url= '', rows=[], cols=[], search='none')
+
+    Args:
+        soup (bs4.BeautifulSoup): A bs4 object of an HTML page
+        config (dict): configuration
+        url (str): url
+        rows (list): list of strings from two rows
+        cols (list): list of strings from one or more columns
+        search (str): column search type SEARCHTYPES
 
-        Args:
-            soup (bs4.BeautifulSoup): A BS4 object of an HTML page
-            config (dict): configuration
-            url (str): url
-            rows (list): list of strings from two rows
-            cols (list): list of strings from one or more columns
-            search (str): column search type SEARCHTYPES
-
-        Returns:
-            config (dict): configuration
+    Returns:
+        config (dict): configuration
 
     """
     rows = [] if rows is None else rows
     cols = [] if cols is None else cols
     search = SEARCH_STENCIL if search not in SEARCHTYPES else search
 
     if rows or cols:
@@ -252,66 +276,66 @@
         aitems1, aitems2 = _build_table_items(soup, rows, cols)
         atags = soups.get_child_of_common_ancestors(aitems1, aitems2)
         ancestors_unique = soups.get_ancestors_unique_filter(atags)
         afilters = soups.get_filters(ancestors_unique)
         afilter_id = soups.get_filter_most_common(afilters)
 
         if afilter_id:
-            config['html']['url'] = url
-            config['html']['table']['id'] = afilter_id
+            config["html"]["url"] = url
+            config["html"]["table"]["id"] = afilter_id
             tf = True
         else:
             tf = False
 
         # Get rows filter
         if tf:
             aid = soups.find_item(soup, afilter=afilter_id)
             aitems1, aitems2 = _build_table_items(aid, rows, cols)
             atags = soups.get_child_of_common_ancestors(aitems1, aitems2)
             afilters = soups.get_filters(atags)
             afilter_rows = soups.get_filter_most_common(afilters)
             if afilter_rows:
-                config['html']['table']['rows'] = afilter_rows
+                config["html"]["table"]["rows"] = afilter_rows
             else:
                 tf = False
 
         # Get cols filter
         if tf and len(cols) > 0:
             # TODO
             # cols from dict to list
             if search == SEARCH_NONE:
                 ritem = soups.find_item(soup, astr=re.compile(cols[0]))
                 adict = {}
                 for index, col in enumerate(cols):
                     citem = soups.find_item(ritem, astr=re.compile(col))
                     afilter = soups.get_filter(citem)
-                    adict['col' + str(index + 1)] = afilter
-                config['html']['table']['cols'] = adict
+                    adict["col" + str(index + 1)] = afilter
+                config["html"]["table"]["cols"] = adict
             elif search == SEARCH_STENCIL:
                 # TODO
-                config['html']['table']['cols'] = {}
+                config["html"]["table"]["cols"] = {}
             else:
                 # search == SEARCH_NAIVE:
-                config['html']['table']['cols'] = {}
+                config["html"]["table"]["cols"] = {}
 
     return config
 
 
-def _build_table_items(aitem, rows, cols):
-    """ Build table items
+def _build_table_items(aitem, rows: list, cols: list) -> Tuple[list, list]:
+    """Build table items
 
-        aitems1, aitems2 = _build_table_items(aitem, rows, cols)
+    aitems1, aitems2 = _build_table_items(aitem, rows, cols)
 
-        Args:
-            aitem (soup or tag):
-            rows (list): list of strings from two rows
-            cols (list): list of strings from one or more columns
-        Returns:
-            aitems1 (list): list of items from first row or col
-            aitems2 (list): list of items from second row or col
+    Args:
+        aitem (soup or tag):
+        rows (list): list of strings from two rows
+        cols (list): list of strings from one or more columns
+    Returns:
+        aitems1 (list): list of items from first row or col
+        aitems2 (list): list of items from second row or col
 
     """
     aitems1 = None
     aitems2 = None
 
     if soups.is_tag(aitem) or soups.is_soup(aitem):
         if len(rows) >= 2:
@@ -320,50 +344,50 @@
         elif len(cols) >= 2:
             aitems1 = soups.find_items(aitem, astr=re.compile(cols[0]))
             aitems2 = soups.find_items(aitem, astr=re.compile(cols[1]))
 
     return aitems1, aitems2
 
 
-def _build_next_page(soup, config, next_page=''):
-    """ Build next page configuration
+def _build_next_page(soup: BeautifulSoup, config: dict, next_page: str = "") -> dict:
+    """Build next page configuration
 
-        config = _build_next_page(soup, config, url= '', next_page=None)
+    config = _build_next_page(soup, config, url= '', next_page=None)
 
-        Args:
-            soup (bs4.BeautifulSoup): A BS4 object of an HTML page
-            config (dict): configuration
-            next_page (str): next page url
+    Args:
+        soup (bs4.BeautifulSoup): A bs4 object of an HTML page
+        config (dict): configuration
+        next_page (str): next page url
 
-        Returns:
-            config (dict): configuration
+    Returns:
+        config (dict): configuration
 
     """
     if len(next_page) > 0:
         # Create next_page string
         if utils.urls.is_valid_http(next_page):
             durl = utils.urls.get_components(next_page)
-            next_page = durl['path']
-            if len(durl['query']) > 0:
-                next_page = next_page + '?' + durl['query']
-        next_page = next_page.lstrip('/')
+            next_page = durl["path"]
+            if len(durl["query"]) > 0:
+                next_page = next_page + "?" + durl["query"]
+        next_page = next_page.lstrip("/")
 
         # Find next_page tag
         next_page_regex = utils.strings.re_literals(next_page)
-        cresults = soup.find_all('a', href=re.compile(next_page_regex))
-        if len(cresults)>0:
+        cresults = soup.find_all("a", href=re.compile(next_page_regex))
+        if len(cresults) > 0:
             citem = cresults[-1]
             # Find ancestor with unique filter
             ancestor_unique = soups.get_ancestor_unique_filter(citem.parent)
             afilter = soups.get_filter(ancestor_unique)
-            aresults = ancestor_unique.find_all('a')
+            aresults = ancestor_unique.find_all("a")
             if aresults:
                 aindex = aresults.index(citem) - len(aresults)
             else:
                 aindex = -1
 
             # Save ancestor filter and index
-            config['html']['page']['id'] = {}
-            config['html']['page']['rows']['elem'] = afilter['elem']
-            config['html']['page']['rows']['class'] = afilter['class']
-            config['html']['page']['index'] = aindex
+            config["html"]["page"]["id"] = {}
+            config["html"]["page"]["rows"]["elem"] = afilter["elem"]
+            config["html"]["page"]["rows"]["class"] = afilter["class"]
+            config["html"]["page"]["index"] = aindex
     return config
```

### Comparing `boxfish-0.1.1/boxfish/data/soups.py` & `boxfish-0.1.2/boxfish/data/soups.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 atable (list): List of rows (list) of columns (str)
 
 afilter (dict): BS4 filter on keys 'elem' (str) and 'class' (list)
 FILTERKEYS = ['elem', 'class']
 
 """
 
-import copy
 import collections
+import copy
+from typing import Any, List, Optional, Tuple, Union
 
 import bs4
 from bs4 import BeautifulSoup
+from bs4.element import ResultSet, Tag
 
 from boxfish.utils import dicts, lists, urls, utils
 from boxfish.utils.xpaths import split as xsplit
 
 
 # Main functions
-def get_page(aitem):
-    """ Get page from soup, tag or ResultSet object
+def get_page(aitem: Union[BeautifulSoup, Tag, ResultSet]) -> str:
+    """Get page from soup, tag or ResultSet object
 
     page = get_page(bitem)
 
     Args:
         aitem : soup or tag or ResultSet object
 
     Returns:
@@ -46,35 +48,42 @@
             page = aitem.decode()
         elif is_results(aitem):
             alist = [atag.decode() for atag in aitem]
             page = "\n".join(alist)
     return page
 
 
-def get_soup(page):
-    """ Get soup object from page
+def get_soup(page: str) -> BeautifulSoup:
+    """Get soup object from page
 
     soup = get_soup(page)
 
     Args:
         page (str): HTML page or an open file handle
 
     Returns:
         soup (bs4.BeautifulSoup): A BS4 object of an HTML page
     """
 
     if page is not None:
-        soup = BeautifulSoup(page, 'lxml')
+        soup = BeautifulSoup(page, "lxml")
     else:
         soup = None
     return soup
 
 
-def extract_table(soup, id=None, rows=None, cols=None, include_strings=True, include_links=False):
-    """ Extract table from soup
+def extract_table(
+    soup: BeautifulSoup,
+    id: Optional[dict] = None,
+    rows: Optional[dict] = None,
+    cols: Optional[List[dict]] = None,
+    include_strings: bool = True,
+    include_links: bool = False,
+) -> List[Union[list, str]]:
+    """Extract table from soup
 
     [atable] = extract_table(soup, id = {}, rows = rows, cols = cols)
 
     Args:
         soup (bs4.BeautifulSoup): A BS4 object of an HTML page
         id (dict): dict with keys {'elem','class'}
         rows (dict): dict with keys {'elem','class'}
@@ -93,20 +102,27 @@
         # Extract rows
         # TODO Change ID
         new_soup = find_item(soup, id) if id else None
         soup = new_soup if new_soup else soup
         results = find_items(soup, rows)
 
         # Extract columns of all rows
-        atable = to_table(results, cols, include_strings=include_strings, include_links=include_links)
+        atable = to_table(
+            results, cols, include_strings=include_strings, include_links=include_links
+        )
     return atable
 
 
-def to_table(aitem, cols=None, include_strings=True, include_links=False):
-    """ Convert aitem to a table
+def to_table(
+    aitem: Union[ResultSet, Tag],
+    cols: Optional[List[dict]] = None,
+    include_strings: bool = True,
+    include_links: bool = False,
+) -> List[Union[list, str]]:
+    """Convert aitem to a table
 
     [atable] = to_table(aitem, cols=None, include_strings=True, include_links=False)
 
     Args:
         aitem(tag or ResultSet): BS4 object
         # Extract subset of strings
         cols (list): list of dict with keys {'elem','class'}
@@ -117,56 +133,61 @@
         atable (list): List of rows (list) of columns (str)
     """
     atable = []
     if not is_results(aitem):
         aitem = [aitem]
 
     for record in aitem:
-        row = get_text(record, cols=cols, include_strings=include_strings, include_links=include_links)
+        row = get_text(
+            record,
+            cols=cols,
+            include_strings=include_strings,
+            include_links=include_links,
+        )
         if not lists.is_empty(row):
             atable.append(row)
 
     return atable
 
 
 # Editing functions - deep copy
-def set_base(page, url):
-    """ Set <base> in page with url
+def set_base(page: str, url: str) -> str:
+    """Set <base> in page with url
 
     [bpage] = set_base(page, url)
 
     Args:
         page (str): HTML page
         url (str): URL link
 
     Returns:
         bpage (str): HTML page with <base>
 
     """
     asoup = get_soup(page)
 
     # Set base
-    abase = asoup.find('base')
+    abase = asoup.find("base")
     if not abase:
-        abase = asoup.new_tag('base')
+        abase = asoup.new_tag("base")
     abase["href"] = url
 
     # Add base to head
-    ahead = asoup.find('head')
+    ahead = asoup.find("head")
     if not ahead:
-        ahead = asoup.new_tag('head')
+        ahead = asoup.new_tag("head")
         asoup.append(ahead)
     ahead.append(abase)
 
     bpage = get_page(asoup)
     return bpage
 
 
-def split(soup):
-    """ Split HTML soup into objects meta and body. Meta and body are deep copies.
+def split(soup: BeautifulSoup) -> Tuple[Optional[BeautifulSoup], Optional[Tag]]:
+    """Split HTML soup into objects meta and body. Meta and body are deep copies.
 
     [meta, body] = split(soup)
 
     Args:
         soup (bs4.BeautifulSoup): A BS4 object of an HTML page with <html> tag
 
     Returns:
@@ -177,23 +198,23 @@
     meta = None
     body = None
 
     if soup is not None and soup.html is not None:
         meta = copy.copy(soup)
         body = meta.find("body")
         if body is None:
-            body = BeautifulSoup('<body>', 'html.parser').find("body")
+            body = BeautifulSoup("<body>", "html.parser").find("body")
         else:
             body.extract()
-        meta.html.append(BeautifulSoup('<body>', 'html.parser').find("body"))
+        meta.html.append(BeautifulSoup("<body>", "html.parser").find("body"))
     return meta, body
 
 
-def merge(meta, body):
-    """ Merge HTML meta and body into a soup object. Soup contains deep copies of meta and body
+def merge(meta: BeautifulSoup, body: Union[ResultSet, Tag]) -> Optional[BeautifulSoup]:
+    """Merge HTML meta and body into a soup object. Soup contains deep copies of meta and body
 
     [soup] = merge(meta, body)
 
     Args:
         meta (bs4.BeautifulSoup): Contains HTML outside <body> plus empty body
         body (tag or ResultSet): Contains HTML inside <body>
 
@@ -216,91 +237,93 @@
         body_new = copy.copy(body)
         soup.html.append(body_new)
     else:
         soup = None
     return soup
 
 
-def set_urls(aitem, url):
-    """ Set full url paths to all href tags. Returns a deep copy
+def set_urls(
+    aitem: Union[BeautifulSoup, Tag], url: str
+) -> Union[Optional[BeautifulSoup], Optional[Tag]]:
+    """Set full url paths to all href tags. Returns a deep copy
 
     [titem] = set_urls(aitem, url)
 
     Args:
         aitem(tag or soup): BS4 object
         url (str): url string
 
     Returns:
         aitem(tag or soup): BS4 object with full url strings
 
     """
     if is_tag(aitem) or is_soup(aitem):
         titem = copy.copy(aitem)
         if url:
-            results = titem.find_all('a')
+            results = titem.find_all("a")
             results.append(titem)
             for aitem in results:
-                if 'href' in aitem.attrs:
-                    if not urls.is_valid_http(aitem['href']):
-                        aitem['href'] = urls.update_relative_path(url, aitem['href'])
+                if "href" in aitem.attrs:
+                    if not urls.is_valid_http(aitem["href"]):
+                        aitem["href"] = urls.update_relative_path(url, aitem["href"])
     else:
         titem = None
     return titem
 
 
 # Conversion functions
-def to_body(aitem):
-    """ Convert aitem to tag with <body>
+def to_body(aitem: Union[ResultSet, Tag]) -> Optional[Tag]:
+    """Convert aitem to tag with <body>
 
     body = to_body(aitem)
 
     Args:
         aitem(tag or ResultSet): BS4 object
 
     Returns:
         body (tag): tag with a <body>
     """
     if is_tag(aitem):
-        if aitem.name == 'body':
+        if aitem.name == "body":
             body = aitem
         else:
-            temp = BeautifulSoup('<body>', 'html.parser').find("body")
+            temp = BeautifulSoup("<body>", "html.parser").find("body")
             temp.append(aitem)
             body = temp
     elif is_results(aitem):
-        temp = BeautifulSoup('<body>', 'html.parser').find("body")
+        temp = BeautifulSoup("<body>", "html.parser").find("body")
         for btag in aitem:
             temp.append(btag)
         body = temp
     else:
         body = None
     return body
 
 
-def unpack_hrefs(tag):
-    """ Unpacks the href links from all a tags, and append the links as a string tag
-        The function changes the existing tag
-
-        Args:
-            tag (tag): BS4 tag
-
-        Returns:
-        """
-    results = tag.find_all('a')
+def unpack_hrefs(tag: Tag) -> None:
+    """Unpacks the href links from all a tags, and append the links as a string tag
+    The function changes the existing tag
+
+    Args:
+        tag (tag): BS4 tag
+
+    Returns:
+    """
+    results = tag.find_all("a")
     results.append(tag)
 
     for atag in results:
-        if 'href' in atag.attrs:
-            astr = '<span>' + str(atag["href"]) + '</span>'
-            htag = BeautifulSoup(astr, 'html.parser').find("span")
+        if "href" in atag.attrs:
+            astr = "<span>" + str(atag["href"]) + "</span>"
+            htag = BeautifulSoup(astr, "html.parser").find("span")
             atag.append(htag)
 
 
-def remove_navigable_strings(results):
-    """ Remove navigable strings from ResultSet
+def remove_navigable_strings(results: ResultSet) -> ResultSet:
+    """Remove navigable strings from ResultSet
     The function removes list item of type Navigable String.
     Tag items which contain navigable strings are not removed.
 
     results = remove_navigable_strings(results)
 
     Args:
         results (ResultSet): BS4 ResultSet
@@ -310,16 +333,16 @@
     """
     for aitem in reversed(results):
         if is_navigable_string(aitem):
             results.remove(aitem)
     return results
 
 
-def wrap_navigable_strings(tag, empty=False):
-    """ Wrap navigable strings into tags
+def wrap_navigable_strings(tag: Tag, empty: bool = False) -> None:
+    """Wrap navigable strings into tags
     The function wraps navigable string into a span tag if the navigable string
     is not the only child of a tag.
     The function changes the existing tag
 
         wrap_navigable_strings(tag)
 
     Args:
@@ -327,63 +350,63 @@
         empty (bool): Wrap empty strings if True
 
     Returns:
     """
     new_tags = []
     for aitem in tag.descendants:
         if is_navigable_string(aitem) and not aitem.parent.string:
-            if empty or (aitem.string is not None and aitem.string != '\n'):
+            if empty or (aitem.string is not None and aitem.string != "\n"):
                 new_tag = tag.new_tag("span")
                 aitem.wrap(new_tag)
                 new_tags.append(new_tag)
 
     # Strip new tags
     for aitem in new_tags:
         _ = aitem.string.replace_with(aitem.string.strip())
 
 
 # I/O functions
-def read(filename):
-    """ Read page from file
+def read(filename: str) -> str:
+    """Read page from file
 
-        page = read(filename)
+    page = read(filename)
 
-        Args:
-            filename (str): file name of HTML page
+    Args:
+        filename (str): file name of HTML page
 
-        Returns:
-            page(str)
+    Returns:
+        page(str)
     """
 
     page = utils.read(filename)
     return page
 
 
-def write(filename, page):
-    """ Write HTML page to file
+def write(filename: str, page: str) -> None:
+    """Write HTML page to file
 
-            write(filename, page)
+    write(filename, page)
 
-            Args:
-                filename (str): file name
-                page (str): HTML page
+    Args:
+        filename (str): file name
+        page (str): HTML page
 
-            Returns:
-                None
+    Returns:
+        None
 
-            Raises:
-                IOError (): error in case function cannot write to filename
-        """
+    Raises:
+        IOError (): error in case function cannot write to filename
+    """
 
     utils.write(filename, page)
 
 
 # Search functions
-def find_soup(aitem):
-    """ Find soup of aitem
+def find_soup(aitem: Union[BeautifulSoup, Tag]) -> BeautifulSoup:
+    """Find soup of aitem
 
     asoup = find_soupd(aitem)
 
     Args:
         aitem(tag or soup): BS4 object
 
     Returns:
@@ -394,16 +417,20 @@
         asoup = aitem
     elif is_tag(aitem):
         rlist = list(reversed(list(aitem.parents)))
         asoup = rlist[0]
     return asoup
 
 
-def find_items(aitem, afilter=None, astr=''):
-    """ Find items from aitem based on filter and/or string
+def find_items(
+    aitem: Union[BeautifulSoup, ResultSet, Tag],
+    afilter: Optional[dict] = None,
+    astr: str = "",
+) -> ResultSet:
+    """Find items from aitem based on filter and/or string
 
     ritems = find_items(aitem, filter=afilter, astr='')
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
         afilter (dict): BS4 filter
         astr (str): string or regular expression for filter on aitem.string
@@ -413,28 +440,32 @@
     """
 
     afilter = {} if afilter is None else afilter
     has_item = "elem" in afilter
     has_class = "class" in afilter
 
     if has_item and has_class:
-        class_ = ' '.join(afilter["class"])
+        class_ = " ".join(afilter["class"])
         ritems = aitem.find_all(afilter["elem"], class_=class_, string=astr)
     elif has_item and not has_class:
         ritems = aitem.find_all(afilter["elem"], string=astr)
     elif not has_item and has_class:
-        class_ = ' '.join(afilter["class"])
+        class_ = " ".join(afilter["class"])
         ritems = aitem.find_all(class_=class_, string=astr)
     else:
         ritems = aitem.find_all(True, string=astr)
     return ritems
 
 
-def find_item(aitem, afilter=None, astr=''):
-    """ Find single item from aitem based on filter and/or string
+def find_item(
+    aitem: Union[BeautifulSoup, ResultSet, Tag],
+    afilter: Optional[dict] = None,
+    astr: str = "",
+) -> Tag:
+    """Find single item from aitem based on filter and/or string
 
     ritem = find_item(aitem, filter=afilter, astr='')
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
         afilter (dict): BS4 filter
         astr (str): string or regular expressiom for filter on aitem.string
@@ -444,43 +475,47 @@
     """
 
     afilter = {} if afilter is None else afilter
     has_item = "elem" in afilter
     has_class = "class" in afilter
 
     if has_item and has_class:
-        class_ = ' '.join(afilter["class"])
+        class_ = " ".join(afilter["class"])
         ritem = aitem.find(afilter["elem"], class_=class_, string=astr)
     elif has_item and not has_class:
         ritem = aitem.find(afilter["elem"], string=astr)
     elif not has_item and has_class:
-        class_ = ' '.join(afilter["class"])
+        class_ = " ".join(afilter["class"])
         ritem = aitem.find(class_=class_, string=astr)
     else:
         ritem = aitem.find(True, string=astr)
     return ritem
 
 
-def find_item_by_xpath(aitem, axpath='', relative=True):
-    """ Find single item from aitem based on xpath
+def find_item_by_xpath(aitem: Tag, axpath: str = "", relative: bool = True) -> Tag:
+    """Find single item from aitem based on xpath
 
     ritem = find_item_by_xpath(aitem, xpath=xpath)
 
     Args:
         aitem(tag): BS4 object
         axpath (str): xpath
         relative (bool): xpath is relative to aitem if true, absolute otherwise
 
     Returns:
         ritem (tag): BS4 tag
     """
 
     if not relative:
         asoup = find_soup(aitem)
-        ritem = find_item_by_xpath(asoup, axpath=axpath, relative=True) if is_soup(asoup) else None
+        ritem = (
+            find_item_by_xpath(asoup, axpath=axpath, relative=True)
+            if is_soup(asoup)
+            else None
+        )
     else:
         [names, idx] = xsplit(axpath)
         tf = True
         ritem = aitem
         # Iterate over xpath items and update ritem each step
         while tf:
             if len(names) == 0:
@@ -491,23 +526,27 @@
                 if idx_i == 1:
                     ritem = ritem.find(names_i)
                     if ritem is None:
                         tf = False
                 else:
                     next_items = ritem.find_all(names_i)
                     if len(next_items) >= idx_i:
-                        ritem = next_items[idx_i-1]
+                        ritem = next_items[idx_i - 1]
                     else:
                         ritem = None
                         tf = False
     return ritem
 
 
-def find_lists(aitem, afilter=None, astr=''):
-    """ Find all lists in aitem. Lists are defined as HTML elements <dl>, <ol>, or <ul>
+def find_lists(
+    aitem: Union[BeautifulSoup, ResultSet, Tag],
+    afilter: Optional[dict] = None,
+    astr: str = "",
+) -> ResultSet:
+    """Find all lists in aitem. Lists are defined as HTML elements <dl>, <ol>, or <ul>
 
     ritems = find_lists(aitems)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
         afilter (dict): BS4 filter
         astr (str): string or regular expressiom for filter on aitem.string
@@ -518,16 +557,20 @@
 
     afilter = {} if afilter is None else afilter
     afilter.update({"elem": ["dl", "ol", "ul"]})
     ritems = find_items(aitem, afilter=afilter, astr=astr)
     return ritems
 
 
-def find_tables(aitem, afilter=None, astr=''):
-    """ Find all tables in aitem. Tables are defined as HTML elements <table>
+def find_tables(
+    aitem: Union[BeautifulSoup, ResultSet, Tag],
+    afilter: Optional[dict] = None,
+    astr: str = "",
+) -> ResultSet:
+    """Find all tables in aitem. Tables are defined as HTML elements <table>
 
     ritems = find_tables(aitems)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
         afilter (dict): BS4 filter
         astr (str): string or regular expressiom for filter on aitem.string
@@ -538,90 +581,96 @@
 
     afilter = {} if afilter is None else afilter
     afilter.update({"elem": ["table"]})
     ritems = find_items(aitem, afilter=afilter, astr=astr)
     return ritems
 
 
-def get_filter(aitem):
-    """ Get filter for aitem
+def get_filter(aitem: Tag) -> dict:
+    """Get filter for aitem
 
     afilter = get_filter(aitem)
 
     Args:
         aitem(tag): BS4 object
 
     Returns:
         afilter (dict): dict with keys 'elem' and 'class'
     """
-    afilter = {'elem': '', 'class': ['']}
+    afilter = {"elem": "", "class": [""]}
     if is_tag(aitem):
-        afilter['elem'] = aitem.name
-        afilter['class'] = aitem['class'] if 'class' in aitem.attrs else ['']
+        afilter["elem"] = aitem.name
+        afilter["class"] = aitem["class"] if "class" in aitem.attrs else [""]
     return afilter
 
 
-def get_filters(aitems):
-    """ Get filter for aitem
+def get_filters(aitems: Union[ResultSet, Tag]) -> List[dict]:
+    """Get filter for aitem
 
     alist = get_filters(aitem)
 
     Args:
         aitems(tag or resultset): BS4 object
 
     Returns:
         alist(list): List of filters
     """
     aresults = aitems if isinstance(aitems, list) else [aitems]
     return [get_filter(aitem) for aitem in aresults]
 
 
-def get_filter_most_common(afilters):
-    """ Get filter most common returns the filter with most occurences
+def get_filter_most_common(afilters: List[dict]) -> dict:
+    """Get filter most common returns the filter with most occurences
 
-        afilter = get_filter_most_common(afilters)
+    afilter = get_filter_most_common(afilters)
 
-        Args:
-            afilters (list): List of BS4 filters (dict)
+    Args:
+        afilters (list): List of BS4 filters (dict)
 
-        Returns:
-            afilter (dict): dict with keys 'elem' and 'class'
+    Returns:
+        afilter (dict): dict with keys 'elem' and 'class'
     """
     jfilters = dicts.dumps(afilters)
     coll = collections.Counter(jfilters)
     alist = coll.most_common(1)
     tup = alist[0]
     afilter = dicts.loads(tup[0])
     return afilter
 
 
-def remove_filters(afilters, elem=None, class_=None):
-    """ Remove filter from afilters based on elem and/or class_
+def remove_filters(
+    afilters: List[dict],
+    elem: Optional[str] = None,
+    class_: Union[str, list, None] = None,
+) -> List[dict]:
+    """Remove filter from afilters based on elem and/or class_
 
-        afilters = _remove_filters(afilters, elem=None,class_=None)
+    afilters = _remove_filters(afilters, elem=None,class_=None)
 
-        Args:
-            afilters(list): list of filters
-            elem (str):
-            class_ (str or list):
-        Returns:
-            afilters(list): list of filters
+    Args:
+        afilters(list): list of filters
+        elem (str):
+        class_ (str or list):
+    Returns:
+        afilters(list): list of filters
 
     """
     for afilter in afilters[:]:  # [:] creates a copy
-        do_remove = afilter['elem'] == elem if elem is not None else False
-        do_remove = do_remove or (afilter['class'] == class_ if class_ is not None else False)
+        do_remove = afilter["elem"] == elem if elem is not None else False
+        do_remove = do_remove or (
+            afilter["class"] == class_ if class_ is not None else False
+        )
         if do_remove:
             afilters.remove(afilter)
     return afilters
 
 
 # Tree functions
-def common_ancestor(aitem1, aitem2):
-    """ Find tag whose descendants contain both aitem1 and aitem2
+def common_ancestor(aitem1: Tag, aitem2: Tag) -> Tag:
+    """Find tag whose descendants contain both aitem1 and aitem2
 
     ritem = common_ancestor(aitem1, aitem2)
 
     Args:
         aitem1 (tag): BS4 tag
         aitem2 (tag): BS4 tag
 
@@ -635,52 +684,56 @@
         parents2 = list(reversed(list(aitem2.parents)))
         for p1, p2 in zip(parents1, parents2):
             if p1 == p2:
                 aitem = p1
     return aitem
 
 
-def common_ancestors(aitems1, aitems2):
-    """ Return a list of common ancestor for all combinations in aitems1 and aitems2
+def common_ancestors(
+    aitems1: Union[ResultSet, Tag], aitems2: Union[ResultSet, Tag]
+) -> List[Tag]:
+    """Return a list of common ancestor for all combinations in aitems1 and aitems2
 
     ritem = common_ancestor(aitem1, aitem2)
 
     Args:
         aitems1 (tag or Resultset): BS4 tag
         aitems2 (tag or Resultset): BS4 tag
 
     Returns:
         ritems (list): List of common ancestors
     """
     aresults1 = aitems1 if isinstance(aitems1, list) else [aitems1]
     aresults2 = aitems2 if isinstance(aitems2, list) else [aitems2]
 
-    return [common_ancestor(aitem1, aitem2) for aitem1 in aresults1 for aitem2 in aresults2]
+    return [
+        common_ancestor(aitem1, aitem2) for aitem1 in aresults1 for aitem2 in aresults2
+    ]
 
 
-def ancestors(aitem):
-    """ Find all ancestor tags on direct line between soup and aitem (exclude both)
-       Returns an ordered list of tags
+def ancestors(aitem: Tag) -> List[Tag]:
+    """Find all ancestor tags on direct line between soup and aitem (exclude both)
+    Returns an ordered list of tags
 
-       rlist = ancestors(aitem)
+    rlist = ancestors(aitem)
 
-       Args:
-           aitem (tag): BS4 tag
+    Args:
+        aitem (tag): BS4 tag
 
-       Returns:
-           rlist (list): List of BS4 tag
-       """
+    Returns:
+        rlist (list): List of BS4 tag
+    """
     alist = list(reversed(list(aitem.parents)))
     if is_soup(alist[0]):
         alist.pop(0)
     return alist
 
 
-def children(aitem, include_navs=False):
-    """ Find all children of aitem
+def children(aitem: Tag, include_navs: bool = False) -> List[Tag]:
+    """Find all children of aitem
     Returns an ordered list of tags
 
     rlist = children(aitem, include_navs=False)
 
     Args:
        aitem (tag): BS4 tag
        include_navs (bool): Include navstrings if True
@@ -690,16 +743,16 @@
     """
     rlist = []
     if is_tag(aitem):
         rlist = [citem for citem in aitem.children if is_tag(citem) or include_navs]
     return rlist
 
 
-def lineage(aancestor, adescendant):
-    """ Find all tags on direct line of descent between ancestor and descendant (exclude both)
+def lineage(aancestor: Tag, adescendant: Tag) -> List[Tag]:
+    """Find all tags on direct line of descent between ancestor and descendant (exclude both)
     Returns an ordered list of tags
 
     rlist = lineage(aancestor, adescendant)
 
     Args:
         aancestor (tag): BS4 tag
         adescendant (tag): BS4 tag
@@ -707,20 +760,20 @@
     Returns:
         rlist (list): List of BS4 tags
     """
     rlist = ancestors(adescendant)
     tf = False
     while not tf and len(rlist) > 0:
         curr_parent = rlist.pop(0)
-        tf = (curr_parent == aancestor)
+        tf = curr_parent == aancestor
     return rlist
 
 
-def position(aitem, include_navs=False):
-    """ Position of aitem in children list of parent
+def position(aitem: Tag, include_navs: bool = False) -> int:
+    """Position of aitem in children list of parent
 
     idx = position(aitem, include_navs=False)
 
     Args:
        aitem (tag): BS4 tag
        include_navs (bool): Include navstrings if True
 
@@ -731,109 +784,119 @@
     if is_tag(aitem) and not is_soup(aitem):
         aparent = aitem.parent
         achildren = children(aparent, include_navs=include_navs)
         idx = achildren.index(aitem)
     return idx
 
 
-def get_child_of_common_ancestor(aitem1, aitem2):
-    """ Get first child of common ancestor.
+def get_child_of_common_ancestor(aitem1: Tag, aitem2: Tag) -> Tag:
+    """Get first child of common ancestor.
 
-        achild = get_child_of_common_ancestor(soup, aitem1, aitem2)
+    achild = get_child_of_common_ancestor(soup, aitem1, aitem2)
 
-        Args:
-            aitem1 (tag): BS4 object
-            aitem2 (tag): BS4 object
+    Args:
+        aitem1 (tag): BS4 object
+        aitem2 (tag): BS4 object
 
-        Returns:
-            achild (tag): First child of common ancestor
+    Returns:
+        achild (tag): First child of common ancestor
     """
     aitem = None
 
     aparent = common_ancestor(aitem1, aitem2)
     if aparent:
         alineage = lineage(aparent, aitem1)
         aitem = alineage[0] if alineage else aitem1
     return aitem
 
 
-def get_child_of_common_ancestors(aitems1, aitems2):
-    """ Get first child of common ancestor.
-        Returns a list with all combinations of aitem1 and aitems2.
-
-        alist = get_child_of_common_ancestor(soup, aitem1, aitem2)
-
-        Args:
-            aitems1 (list): List of BS4 tags
-            aitems2 (list): List of BS4 tags
+def get_child_of_common_ancestors(aitems1: List[Tag], aitems2: List[Tag]) -> List:
+    """Get first child of common ancestor.
+    Returns a list with all combinations of aitem1 and aitems2.
+
+    alist = get_child_of_common_ancestor(soup, aitem1, aitem2)
+
+    Args:
+        aitems1 (list): List of BS4 tags
+        aitems2 (list): List of BS4 tags
 
-        Returns:
-            alist (list): List with first child of common ancestor
+    Returns:
+        alist (list): List with first child of common ancestor
     """
     aresults1 = aitems1 if isinstance(aitems1, list) else [aitems1]
     aresults2 = aitems2 if isinstance(aitems2, list) else [aitems2]
 
-    return [get_child_of_common_ancestor(aitem1, aitem2) for aitem1 in aresults1 for aitem2 in aresults2]
+    return [
+        get_child_of_common_ancestor(aitem1, aitem2)
+        for aitem1 in aresults1
+        for aitem2 in aresults2
+    ]
 
 
-def get_ancestor_unique_filter(aitem):
-    """ Get first ancestor of aitem which has a unique filter in soup
+def get_ancestor_unique_filter(aitem: Tag) -> Tag:
+    """Get first ancestor of aitem which has a unique filter in soup
 
-        aancestor = get_ancestor_unique_filter(aitem)
+    aancestor = get_ancestor_unique_filter(aitem)
 
-        Args:
-            aitem (tag): BS4 object
+    Args:
+        aitem (tag): BS4 object
 
-        Returns:
-            aancestor (tag): BS4 object
+    Returns:
+        aancestor (tag): BS4 object
     """
     aancestors = ancestors(aitem)
     aancestor = None
     is_unique = False
     soup = find_soup(aitem)
 
     while not is_unique and len(aancestors) > 0:
         aancestor = aancestors.pop()
         afilter = get_filter(aancestor)
         is_unique = is_unique_filter(afilter, soup)
     return aancestor
 
 
-def get_ancestors_unique_filter(aitems):
-    """ Get first ancestor of aitem which has a unique filter in soup
+def get_ancestors_unique_filter(aitems: Union[List[Tag], Tag]) -> List:
+    """Get first ancestor of aitem which has a unique filter in soup
 
-        aancestors = get_ancestors_unique_filter(aitems)
+    aancestors = get_ancestors_unique_filter(aitems)
 
-        Args:
-            aitems (list): BS4 object
+    Args:
+        aitems (list): BS4 object
 
-        Returns:
-            aancestors (list): BS4 object
+    Returns:
+        aancestors (list): BS4 object
     """
     aresults = aitems if isinstance(aitems, list) else [aitems]
     return [get_ancestor_unique_filter(aitem) for aitem in aresults]
 
 
-def get_parents(aitems):
-    """ Get parent for each item in aitems
+def get_parents(aitems: List[Tag]) -> List[Tag]:
+    """Get parent for each item in aitems
 
-         aparents = get_parents(aitems)
+    aparents = get_parents(aitems)
 
-         Args:
-             aitems (list): List of BS4 tags
+    Args:
+        aitems (list): List of BS4 tags
 
-         Returns:
-             aparents (list): List of BS4 tags
-     """
+    Returns:
+        aparents (list): List of BS4 tags
+    """
     return [aitem.parent for aitem in aitems]
 
 
 # Text extraction functions
-def get_text(aitem, cols=None, include_strings=True, include_links=False, fill_missing_cols=True):
-    """ Get text from soup objects. Text consists of strings and/or links.
+def get_text(
+    aitem: Union[BeautifulSoup, ResultSet, Tag],
+    cols: Union[list, str, None] = None,
+    include_strings: bool = True,
+    include_links: bool = False,
+    fill_missing_cols: bool = True,
+) -> List[Union[ResultSet, Tag]]:
+    """Get text from soup objects. Text consists of strings and/or links.
         Returns all text of descendant items if no columns are specified, or
         text of specific columns only, if columns are specified.
 
     alist = get_text(aitem, cols=cols, include_strings=True, include_links=False)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
@@ -854,15 +917,17 @@
         do_unpack = False
 
     for atag in aitem:
         do_flatten = False
 
         # Get string item
         if isinstance(cols, list):
-            sitem = _get_cols_as_results(atag, cols, fill_missing_cols=fill_missing_cols)
+            sitem = _get_cols_as_results(
+                atag, cols, fill_missing_cols=fill_missing_cols
+            )
             do_flatten = True
         elif isinstance(cols, str):
             # TODO stencil
             sitem = atag
             # TODO Convert list to Resultset. See get_subtext
         else:
             sitem = atag
@@ -873,26 +938,28 @@
         elif include_links:
             alist_item = get_links(sitem)
         else:
             alist_item = []
 
         # Flatten text
         if do_flatten:
-            alist_item = [[''] if lists.is_empty(val) else val for val in alist_item]
+            alist_item = [[""] if lists.is_empty(val) else val for val in alist_item]
             alist_item = lists.flatten(alist_item)
 
         alist.append(alist_item)
 
     if do_unpack:
         alist = alist[0]
     return alist
 
 
-def get_strings(aitem, include_links=False):
-    """ Get strings from soup objects
+def get_strings(
+    aitem: Union[BeautifulSoup, ResultSet, Tag], include_links: bool = False
+) -> List[Union[ResultSet, Tag]]:
+    """Get strings from soup objects
 
     alist = get_strings(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
         include_links (boolean): Include links as strings if true
 
@@ -904,15 +971,15 @@
         alist = _get_strings_from_tag(aitem, include_links)
     elif is_results(aitem):
         alist = _get_strings_from_results(aitem, include_links)
     return alist
 
 
 def get_links(aitem):
-    """ Get links from soup objects
+    """Get links from soup objects
 
     alist = get_links(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
 
     Returns:
@@ -928,16 +995,16 @@
 
 # Stencil functions
 
 # A stencil provides a tag with mask layout filled with strings and links content from aitem.
 # A mask consists of a bs4 structure without content
 
 
-def stencil(aitem, amask):
-    """ Get stencil from soup or tag
+def stencil(aitem: Union[BeautifulSoup, Tag], amask: Tag) -> Tag:
+    """Get stencil from soup or tag
     # A stencil returns tag sitem with mask layout filled with strings and links content from aitem.
 
     sitem = stencil(aitem, amask)
 
     Args:
         aitem : soup or tag
         amask : tag
@@ -951,21 +1018,23 @@
     # 1. Copy aitem to sitem
     sitem = copy.copy(aitem)
 
     xd_item = xpaths(sitem, root=sitem, first_index=True)
     xd_mask = xpaths(amask, root=amask, first_index=True)
 
     # 2. Find all tags in sitem not in amask and delete these tags from aitem
-    xpaths_redundant = xpaths_set(xd_item, xd_mask, operation='difference', relative=True)
+    xpaths_redundant = xpaths_set(
+        xd_item, xd_mask, operation="difference", relative=True
+    )
     for ax in xpaths_redundant:
         ritem = find_item_by_xpath(sitem, axpath=ax, relative=True)
         ritem.decompose() if ritem else None
 
     # 3. Find all tags in atemplate not in aitem and add in correct position with ''
-    xpaths_missing = xpaths_set(xd_mask, xd_item, operation='difference', relative=True)
+    xpaths_missing = xpaths_set(xd_mask, xd_item, operation="difference", relative=True)
     for ax in xpaths_missing:
         ditem = find_item_by_xpath(amask, axpath=ax, relative=True)
         idx = position(ditem, include_navs=True)
 
         nitem = copy.copy(ditem)
 
         # TODO
@@ -974,215 +1043,221 @@
         # Create tag
         # Fill content of tag
         pass
 
     return sitem
 
 
-def get_mask(aitem, astr='', ahref=''):
-    """ Get Mask from soup or tag
+def get_mask(aitem: Union[BeautifulSoup, Tag], astr: str = "", ahref: str = ""):
+    """Get Mask from soup or tag
     A mask consists of a bs4 structure without content
     Navigable strings and hrefs values are replaced
     All other attributes, except class, are stripped
 
     ritem = get_mask(aitem)
 
     Args:
         aitem : soup or tag
-        astr  : filling string or 'count'
+        astr  : filling string or "count"
         ahref : filling href
 
     Returns:
 
         ritem : soup or tag
     """
 
     ritem = None
     if is_tag(aitem) or is_soup(aitem):
         ritem = copy.copy(aitem)
 
         # strings
         results = ritem.find_all(text=True)
         for i, atag in enumerate(results):
-            rstr = str(i) if astr == 'count' else astr
+            rstr = str(i) if astr == "count" else astr
             _ = atag.string.string.replace_with(rstr)
 
         # hrefs
-        results = ritem.find_all('a')
+        results = ritem.find_all("a")
         results.append(ritem)
         for atag in results:
-            if 'href' in atag.attrs:
-                atag['href'] = ahref
+            if "href" in atag.attrs:
+                atag["href"] = ahref
 
         # Other attributes
         results = ritem.find_all()
         for atag in results:
             for att in atag.attrs:
-                if att not in ('class', 'href'):
-                    atag[att] = ''
+                if att not in ("class", "href"):
+                    atag[att] = ""
 
     return ritem
 
 
 # Identification functions
-def is_tag(aitem):
-    """ Returns true if aitem is bs4.element.Tag
+def is_tag(aitem: Any) -> bool:
+    """Returns true if aitem is bs4.element.Tag
 
     tf = is_tag(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
 
     Returns:
         tf (bool): True if aitem is BS4 tag, False otherwise
     """
     return isinstance(aitem, bs4.element.Tag)
 
 
-def is_results(aitem):
-    """ Returns true if aitem is bs4.element.ResultSet
+def is_results(aitem: Any) -> bool:
+    """Returns true if aitem is bs4.element.ResultSet
 
     tf = is_results(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
 
     Returns:
         tf (bool): True if aitem is BS4 Resultset, False otherwise
     """
     return isinstance(aitem, bs4.element.ResultSet)
 
 
-def is_soup(aitem):
-    """ Returns true if aitem is bs4.BeautifulSoup
+def is_soup(aitem: Any) -> bool:
+    """Returns true if aitem is bs4.BeautifulSoup
 
     tf = is_soup(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
 
     Returns:
         tf (bool): True if aitem is BS4 soup, False otherwise
     """
     return isinstance(aitem, bs4.BeautifulSoup)
 
 
-def is_navigable_string(aitem):
-    """ Returns true if aitem is BS4 NavigableString
+def is_navigable_string(aitem: Any) -> bool:
+    """Returns true if aitem is BS4 NavigableString
 
     tf = is_navigable_string(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
 
     Returns:
         tf (bool): True if aitem is BS4 Navigable String, False otherwise
     """
     return isinstance(aitem, bs4.element.NavigableString)
 
 
-def is_leaf(aitem):
-    """ Returns true if aitem is a leaf bs4.element.Tag.
+def is_leaf(aitem: Any) -> bool:
+    """Returns true if aitem is a leaf bs4.element.Tag.
 
     tf = is_leaf(aitem)
 
     Args:
         aitem(soup or tag or ResultSet): BS4 object
 
     Returns:
         tf (bool): True if aitem is leaf BS4 tag, False otherwise
     """
     return is_tag(aitem) and is_navigable_string(aitem.next)
 
 
-def is_empty_filter(afilter):
-    """ True if filter is empty
+def is_empty_filter(afilter: dict) -> bool:
+    """True if filter is empty
 
     tf = is_empty_filter(afilter)
 
     Args:
         afilter (dict): BS4 filter
 
     Returns:
         tf: True if filter is empty
     """
-    return lists.is_empty(afilter['elem']) and lists.is_empty(afilter['class'])
+    return lists.is_empty(afilter["elem"]) and lists.is_empty(afilter["class"])
 
 
-def is_filter(afilter):
-    """ Returns true if afilter is a filter
+def is_filter(afilter: Any) -> bool:
+    """Returns true if afilter is a filter
 
     tf = is_filter(afilter)
 
     Args:
         afilter (dict): dict with keys 'elem' and 'class' (if True)
 
     Returns:
         tf (bool): True if afilter is filter, False otherwise
     """
-    return isinstance(afilter, dict) and ('elem' in afilter and 'class' in afilter)
+    return isinstance(afilter, dict) and ("elem" in afilter and "class" in afilter)
 
 
-def is_unique_filter(afilter, aitem):
-    """ Returns true if afilter is unique in aitem
+def is_unique_filter(afilter: dict, aitem: Union[BeautifulSoup, Tag]) -> bool:
+    """Returns true if afilter is unique in aitem
 
-        tf = is_unique_filter(afilter, aitem)
+    tf = is_unique_filter(afilter, aitem)
 
-        Args:
-            afilter (dict): dict with keys 'elem' and 'class' (if True)
-            aitem(tag or soup): BS4 object
+    Args:
+        afilter (dict): dict with keys 'elem' and 'class' (if True)
+        aitem(tag or soup): BS4 object
 
-        Returns:
-            tf (bool): True if afilter is unique filter in aitem, False otherwise
+    Returns:
+        tf (bool): True if afilter is unique filter in aitem, False otherwise
     """
     tf = is_filter(afilter) and (is_tag(aitem) or is_soup(aitem))
     if tf:
         results = find_items(aitem, afilter=afilter)
         tf = len(results) == 1
     return tf
 
 
 # Xpath functions
-def xpath(aitem, root=None, first_index=False):
-    """ Returns xpath of aitem.
+def xpath(
+    aitem: Tag, root: Optional[Tag] = None, first_index: bool = False
+) -> Union[list, str]:
+    """Returns xpath of aitem.
     Returns absolute path or relative path to root
 
     xpath = xpath(aitem, root, first_index)
 
     Args:
         aitem(tag): BS4 object
         root(tag): BS4 tag (optional)
         first_index(bool): include first index if true
 
     Returns:
         axpath (str or list): xpath of aitem
     """
-    axpath = ''
+    axpath = ""
     if is_tag(aitem) and not is_soup(aitem):
         if aitem == root:
-            axpath = '//'
+            axpath = "//"
         else:
             # Absolute
             rlist = ancestors(aitem)
             rlist.append(aitem)
             for aparent in rlist:
                 idx = _get_xpath_index(aparent, first_index=first_index)
-                sidx = '[' + str(idx) + ']' if idx > 0 else ''
-                axpath = axpath + '/' + aparent.name + sidx
+                sidx = "[" + str(idx) + "]" if idx > 0 else ""
+                axpath = axpath + "/" + aparent.name + sidx
 
             # Relative
             if is_tag(root):
                 axpath_root = xpath(root, first_index=first_index)
-                axpath = axpath.replace(axpath_root, '/') if axpath.startswith(axpath_root) else ''
+                axpath = (
+                    axpath.replace(axpath_root, "/")
+                    if axpath.startswith(axpath_root)
+                    else ""
+                )
     return axpath
 
 
 # Xpaths. Xpath set functions.
-def xpaths(aitem, root=None, first_index=False):
-    """ Returns list of xpaths of all descendant tags
+def xpaths(aitem: Tag, root: Optional[Tag] = None, first_index: bool = False) -> list:
+    """Returns list of xpaths of all descendant tags
 
     alist = xpaths(aitem, root, first_index)
 
     Args:
         aitem(tag): BS4 object
         root(tag): BS4 tag (optional)
         first_index(bool): include first index if true
@@ -1196,16 +1271,21 @@
         #     alist.append(xpath(aitem, root=root))
         for atag in aitem.descendants:
             if is_tag(atag):
                 alist.append(xpath(atag, root=root, first_index=first_index))
     return alist
 
 
-def xpaths_set(aitem1, aitem2, operation=None, relative=False):
-    """ Returns an unordered list with set operation on xpaths in aitem1 and aitem2
+def xpaths_set(
+    aitem1: Union[List[Tag], Tag],
+    aitem2: Union[List[Tag], Tag],
+    operation: Optional[str] = None,
+    relative: bool = False,
+) -> list:
+    """Returns an unordered list with set operation on xpaths in aitem1 and aitem2
      When relative is true relative xpaths are relative to root of aitem1 and aitem2
 
     alist = xpaths_set(aitem1, aitem2)
 
     Args:
         aitem1(tag): BS4 object
         aitem2(tag): BS4 object
@@ -1215,28 +1295,28 @@
     Returns:
         alist (list): list with xpaths from of aitem1 and aitem2 based on operation
     """
 
     xpath1 = xpaths(aitem1, root=(aitem1 if relative else None), first_index=True)
     xpath2 = xpaths(aitem2, root=(aitem2 if relative else None), first_index=True)
 
-    if operation == 'union':
+    if operation == "union":
         alist = lists.union(xpath1, xpath2)
-    elif operation == 'intersect':
+    elif operation == "intersect":
         alist = lists.intersect(xpath1, xpath2)
-    elif operation == 'difference':
+    elif operation == "difference":
         alist = lists.difference(xpath1, xpath2)
     else:
         alist = []
     return alist
 
 
 # Private xpath functions
-def _get_xpath_index(aitem, first_index=False):
-    """ Returns xpath index. A positive index represents k-th index
+def _get_xpath_index(aitem: Tag, first_index: bool = False) -> int:
+    """Returns xpath index. A positive index represents k-th index
     A zero index represents first index with no further occurences of same name
 
     xpi = _get_xpath_index(aitem, first_index)
 
     Args:
         aitem(tag): BS4 object
         first_index(bool): include first index if true
@@ -1256,98 +1336,104 @@
                     if citem == aitem:
                         xpi = nitems
         xpi = xpi if (nitems > 1 or first_index) else 0
     return xpi
 
 
 # Private functions
-def _get_colnames(ncols):
-    """ Get column names
+def _get_colnames(ncols: int) -> list:
+    """Get column names
 
-        [colnames] = _get_colnames(nitems)
+    [colnames] = _get_colnames(nitems)
 
-        Args:
-            ncols (int): Number of colums
-        Returns:
-            acolnames (list): Column names
-        """
-    return ['Col' + str(i + 1) for i in range(ncols)]
+    Args:
+        ncols (int): Number of colums
+    Returns:
+        acolnames (list): Column names
+    """
+    return ["Col" + str(i + 1) for i in range(ncols)]
 
 
-def _get_cols_as_results(aitem, cols, fill_missing_cols=True):
-    """ Get columns as a Resultset
+def _get_cols_as_results(
+    aitem: Union[BeautifulSoup, ResultSet, Tag],
+    cols: List[dict],
+    fill_missing_cols: bool = True,
+):
+    """Get columns as a Resultset
 
-        aresults = _get_cols_as_results(aitem)
+    aresults = _get_cols_as_results(aitem)
 
-        Args:
-            aitem(soup or tag or ResultSet): BS4 object
-            cols (list): list of dicts with keys {'elem','class'}
-            fill_missing_cols (boolean): Fill missing columns if true
+    Args:
+        aitem(soup or tag or ResultSet): BS4 object
+        cols (list): list of dicts with keys {'elem','class'}
+        fill_missing_cols (boolean): Fill missing columns if true
 
-        Returns:
-            aresults (ResultSet): ResultSet
-        """
+    Returns:
+        aresults (ResultSet): ResultSet
+    """
     if not is_results(aitem):
         aitem = [aitem]
 
     # Create empty ResultSet
     aresults = aitem[0].find_all("")
 
     if fill_missing_cols:
         asoup = find_soup(aitem[0])
-        stag = asoup.new_tag('i')
-        ltag = asoup.new_tag('a', href='')
+        stag = asoup.new_tag("i")
+        ltag = asoup.new_tag("a", href="")
     else:
         stag = None
         ltag = None
 
     for record in aitem:
         for col in cols:
             atag = find_item(record, col)
             if is_tag(atag):
                 aresults.append(atag)
             elif fill_missing_cols:
-                if col['elem'] == 'a':
+                if col["elem"] == "a":
                     aresults.append(ltag)
                 else:
                     aresults.append(stag)
     return aresults
 
 
-def _get_strings_from_results(results, include_links=False):
-    """ Get strings from results
+def _get_strings_from_results(
+    results: ResultSet, include_links: bool = False
+) -> List[str]:
+    """Get strings from results
 
     alist = _get_strings_from_results(results)
 
     Args:
         results (ResultSet): BS4 result set
         include_links (boolean): Include hrefs as strings if true
 
     Returns:
         alist (list): List of strings
     """
     return [_get_strings_from_tag(tag, include_links) for tag in results]
 
 
-def _get_links_from_results(results):
-    """ Get links from results. Links are href strings
+def _get_links_from_results(results: ResultSet) -> list:
+    """Get links from results. Links are href strings
 
     alist = _get_links_from_results(results)
 
     Args:
         results (ResultSet): BS4 result set
 
     Returns:
         alist (list): List of links
     """
     return [_get_links_from_tag(tag) for tag in results]
 
 
-def _get_strings_from_tag(tag, include_links=False):
-    """ Get strings from tag
+def _get_strings_from_tag(tag: Tag, include_links: bool = False) -> List[str]:
+    """Get strings from tag
 
     alist = _get_strings_from_tag(tag)
 
     Args:
         tag (tag): BS4 tag
         include_links (boolean): Include links if true
 
@@ -1358,23 +1444,23 @@
         atag = copy.copy(tag)
         unpack_hrefs(atag)
     else:
         atag = tag
     return [text for text in atag.stripped_strings]
 
 
-def _get_links_from_tag(tag):
-    """ Get links from tag. Links are href strings
+def _get_links_from_tag(tag: Tag) -> list:
+    """Get links from tag. Links are href strings
 
     alist = _get_links_from_tag(tag)
 
     Args:
         tag (tag): BS4 tag
 
     Returns:
         alist (list): List of links
     """
-    results = tag.find_all('a')
+    results = tag.find_all("a")
     results.append(tag)
-    alist = [tag['href'] if 'href' in tag.attrs else None for tag in results]
+    alist = [tag["href"] if "href" in tag.attrs else None for tag in results]
     alist = list(filter(None, alist))
     return alist
```

### Comparing `boxfish-0.1.1/boxfish/data/website.py` & `boxfish-0.1.2/boxfish/data/website.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,174 +1,182 @@
 # website.py
 
 """ Website is a module that contains functions for extracting tables from websites. """
 
-from boxfish.data import config
-from boxfish.data import soups
+from typing import Any, List, Optional, Tuple, Union
 
-from boxfish.utils.dicts import extract_values, get_subset
+from boxfish.data import config, soups
 from boxfish.utils import drivers, lists, urls
+from boxfish.utils.dicts import extract_values, get_subset
 
 
 # Main functions
-def extract(url, config):
-    """ Get data from a website based on config and url
+def extract(url: Union[list, str], config: dict) -> Union[List[list], List[str]]:
+    """Get data from a website based on config and url
 
     data = extract(url=url, config=config):
 
     Args:
         url (str or list):  url
         config (dict):      configuration
 
     Returns:
         data (list): List of rows (list) of columns (str)
     """
 
-    [poutput] = extract_values(config, ['output'])
-    data = extract_data(url,config)
+    [poutput] = extract_values(config, ["output"])
+    data = extract_data(url, config)
     save(data, poutput)
 
     return data
 
 
-def extract_data(url,config):
-    """ Extract data from url to list
+def extract_data(url: Union[list, str], config: dict) -> Union[List[list], List[str]]:
+    """Extract data from url to list
 
     data = extract_data(url, config)
 
     Args:
         url (str or list):  url
         config (dict):      configuration
 
     Returns:
         data (list): List of rows (list) of columns (str)
     """
 
     data = []
 
     if url and config:
-        adriver = drivers.driver_start(config['driver'])
+        adriver = drivers.driver_start(config["driver"])
         try:
             data = _extract_data_from_driver(url, config, adriver)
         finally:
             drivers.driver_stop(adriver)
 
     return data
 
 
 # Beautiful Soup functions
-def extract_table(page, ptable, url=''):
-    """ Extract table from an HTML page
+def extract_table(
+    page: str, ptable: dict, url: str = ""
+) -> Union[List[list], List[str]]:
+    """Extract table from an HTML page
 
-        atable = extract_table(page, ptable, url)
+    atable = extract_table(page, ptable, url)
 
-        Args:
-            page(str): HTML text
-            ptable(dict): Table parameters with keys config.TABLEKEYS
-            url(str): Url current page
-        Returns:
-            atable (list): List of rows (list) of columns (str)
+    Args:
+        page(str): HTML text
+        ptable(dict): Table parameters with keys config.TABLEKEYS
+        url(str): Url current page
+    Returns:
+        atable (list): List of rows (list) of columns (str)
     """
 
     atable = []
 
     if page:
         soup = soups.get_soup(page)
 
         if soup:
             # Pre-processing
-            for s in soup.select('style'):
+            for s in soup.select("style"):
                 s.decompose()
             if url:
                 soup = soups.set_urls(soup, url)
             soups.wrap_navigable_strings(soup)
 
             pparams = get_subset(ptable, config.TABLEKEYS)
             atable = soups.extract_table(soup, **pparams)
     return atable
 
 
-def extract_url_next_page(page, pnext_page, url):
-    """ Extract url that refers to next page
+def extract_url_next_page(page: str, pnext_page: dict, url: str) -> str:
+    """Extract url that refers to next page
 
-        url_next = extract_url_next_page(page,pnext_page,url)
+    url_next = extract_url_next_page(page,pnext_page,url)
 
-        Args:
-            page(str): HTML text
-            next_page(dict): Next page parameters with keys config.PAGEKEYS
-            url(str): Url current page
+    Args:
+        page(str): HTML text
+        next_page(dict): Next page parameters with keys config.PAGEKEYS
+        url(str): Url current page
 
-        Returns:
-            url_next_page (str): Url next page
+    Returns:
+        url_next_page (str): Url next page
     """
-    url_next_page = ''
-    tf = not soups.is_empty_filter(pnext_page['rows']) if pnext_page else False
+    url_next_page = ""
+    tf = not soups.is_empty_filter(pnext_page["rows"]) if pnext_page else False
 
     if tf:
-        [index] = extract_values(pnext_page, ['index'])
+        [index] = extract_values(pnext_page, ["index"])
         index = index if index else -1
 
-        pnext_page['include_strings'] = False
-        pnext_page['include_links'] = True
+        pnext_page["include_strings"] = False
+        pnext_page["include_links"] = True
 
         alinks = extract_table(page, pnext_page, url)
         if alinks:
             alinks = lists.flatten(alinks)
             url_next_page = alinks[index]
-    return  url_next_page
+    return url_next_page
 
 
 # File functions
-def save(data, fileconfig):
-    """ Save data to CSV file
+def save(data: list, fileconfig: dict) -> None:
+    """Save data to CSV file
 
-        save(data, fileconfig)
+    save(data, fileconfig)
+
+    Args:
+        data(list): Data from HTML
+        fileconfig(dict): Parameter with keys {'filename','date_format','replace'}
+
+    Returns:
+        None
+    """
+    lists.to_csv(
+        data,
+        fileconfig["filename"],
+        date_format=fileconfig["date_format"],
+        overwrite=fileconfig["overwrite"],
+        quoting=fileconfig["quoting"],
+    )
 
-        Args:
-            data(dataframe or list): Data from HTML
-            fileconfig(dict): Parameter with keys {'filename','date_format','replace'}
-
-        Returns:
-            None
-    """
-    lists.to_csv(data, fileconfig['filename'],
-             date_format=fileconfig['date_format'],
-             overwrite=fileconfig['overwrite'],
-             quoting=fileconfig['quoting'])
 
 # Private functions
-def _extract_data_from_driver(url, config, adriver):
-    """ Extract data from url to list
+def _extract_data_from_driver(
+    url: Union[List[str], str], config: dict, adriver
+) -> Union[List[list], List[str]]:
+    """Extract data from url to list
 
     data = _extract_data_from_driver(url, config, adriver)
 
     Args:
         url (str or list):  url
         config (dict):      configuration
         adriver (driver):   driver
 
     Returns:
         data (list): List of rows (list) of columns (str)
     """
     data = []
 
     # Extract parameters
-    [phtml] = extract_values(config, ['html'])
-    [ptable] = extract_values(phtml, ['table'])
-    [ppage] = extract_values(phtml, ['page'])
+    [phtml] = extract_values(config, ["html"])
+    [ptable] = extract_values(phtml, ["table"])
+    [ppage] = extract_values(phtml, ["page"])
 
     i_request = 0
     url = lists.to_list(url) if not isinstance(url, list) else url
 
     for url_i in url:
         url_next = url_i
-        url_pre = ['']
+        url_pre = [""]
         while url_next not in url_pre:
             page = drivers.request_page(adriver, url=url_next, count=i_request)
             i_request = i_request + 1
 
             table = extract_table(page, ptable, url_next)
             data.extend(table)
 
             url_pre.append(url_next)
             url_next = extract_url_next_page(page, ppage, url_next)
-    return data
+    return data
```

### Comparing `boxfish-0.1.1/boxfish/utils/dataframes.py` & `boxfish-0.1.2/boxfish/utils/dataframes.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 
 """Dataframes is a module that contains functions for pandas dataframes
 
 """
 
 import csv
 import os
+
 import pandas as pd
+
 from boxfish.utils.strings import filename_append_date
 from boxfish.utils.utils import create_folder_if_not_exist
 
 
-def list_to_dataframe(alist, columns):
-    """ Convert list to dataframe with single column
+def list_to_dataframe(alist: list, columns: list) -> pd.DataFrame:
+    """Convert list to dataframe with single column
 
     df = list_to_dataframe(alist,columns)
 
     Args:
         alist (list): List of items
         columns (list): List with column name
     Returns:
-        df (pandas.core.frame.DataFrame): Dataframe with list as column
+        df (pandas.DataFrame): Dataframe with list as column
 
     Example:
         alist = [1, 2, 3]
         columns = ['Col1']
         df = list_to_dataframe(alist,columns)
         >>    Col1
         >>0      1
@@ -35,35 +37,41 @@
     df = None
     if len(alist) > 0:
         df = pd.DataFrame(alist)
         df.columns = list(columns)
     return df
 
 
-def save(df, filename, date_format='', overwrite=False, quoting=csv.QUOTE_NONNUMERIC):
-    """ Save dataframe to csv file
+def save(
+    df: pd.DataFrame,
+    filename: str,
+    date_format: str = "",
+    overwrite: bool = False,
+    quoting: int = csv.QUOTE_NONNUMERIC,
+) -> str:
+    """Save dataframe to csv file
 
     fullname = save(df, filename, date_format, overwrite, quoting)
 
     Args:
-        df (pandas.core.frame.DataFrame): Dataframe
+        df (pandas.DataFrame): Dataframe
         filename (str): Filename
         date_format (str): Date format in strftime formats
         overwrite (bool): Overwrite existing file if True else append
         quoting (int): CSV quoting constant
     Returns:
-        fullname: Full filename including date
+        fullname (str): Full filename including date
 
     Example:
         fullname = save(df, 'filename.txt', date_format='%Y%m%d', overwrite=True, quoting=csv.QUOTE_NONNUMERIC)
     """
     if (df is not None) and os.path.basename(filename):
         create_folder_if_not_exist(os.path.dirname(filename))
         fullname = filename_append_date(filename, date_format)
 
         if os.path.exists(fullname) and not overwrite:
-            df.to_csv(fullname, mode='a', header=False, quoting=quoting)
+            df.to_csv(fullname, mode="a", header=False, quoting=quoting)
         else:
-            df.to_csv(fullname, mode='w', quoting=quoting)
+            df.to_csv(fullname, mode="w", quoting=quoting)
     else:
-        fullname = ''
+        fullname = ""
     return fullname
```

### Comparing `boxfish-0.1.1/boxfish/utils/dicts.py` & `boxfish-0.1.2/boxfish/utils/dicts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # dicts.py
 
 """Dicts is a module that contains functions for dictionaries"""
 
 import json
+from typing import List, Union
 
 
-def get_subset(adict, akeys):
-    """ Get a dict subset consisting of akeys. Missing akeys are ignored
+def get_subset(adict: dict, akeys: List[str]) -> dict:
+    """Get a dict subset consisting of akeys. Missing akeys are ignored
 
     bdict = get_subset(adict, akeys)
 
     Args:
         adict (dict): Dictionary with key-value pairs
         akeys (list): List of key strings
     Returns:
@@ -21,16 +22,16 @@
         adict = {'key1': val1, 'key2': val1}
         bdict = get_subset(adict, ['key1', 'key3'])
         >> bdict = {'key1': val1}
     """
     return {key: value for key, value in adict.items() if key in akeys}
 
 
-def extract_values(adict, akeys):
-    """ Extract values from adict for akeys
+def extract_values(adict: dict, akeys: List[str]) -> list:
+    """Extract values from adict for akeys
 
     [values1, values2, ...] = extract_values(adict, alist)
 
     Args:
         adict (dict): Dictionary with key-value pairs
         akeys (list): List of key strings
     Returns:
@@ -40,23 +41,23 @@
     Example:
         adict = {'key1': val1, }
         [val1, val3] = extract_values(adict, ['key1', 'key3'])
         >> val1 = 'val1'
         >> val3 = None
     """
 
-    klist = [None]*len(akeys)
+    klist = [None] * len(akeys)
     for i, val in enumerate(akeys):
         if val in adict:
             klist[i] = adict[val]
     return [*klist]
 
 
-def append(adict, bdict):
-    """ Append bdict to adict
+def append(adict: dict, bdict: dict) -> dict:
+    """Append bdict to adict
 
     Duplicate entries in bdict overwrite entries from adict
 
     [values1, values2, ...] = extract_values(adict, alist)
 
     Args:
         adict (dict): Dictionary with key-value pairs
@@ -69,16 +70,16 @@
         bdict = {'key1': 'bval1', 'key3': 'val3'}
         cdict = append(adict, bdict)
         >> {'key1': 'bval1', 'key2': 'val2', 'key3': 'val3'}
     """
     return dict(adict, **bdict) if isinstance(bdict, dict) else adict
 
 
-def remove_nones(adict):
-    """ Remove key-vlaue pairs with a None Value
+def remove_nones(adict: dict) -> dict:
+    """Remove key-vlaue pairs with a None Value
 
     [values1, values2, ...] = extract_values(adict, alist)
 
     Args:
         adict (dict): Dictionary with key-value pairs
     Returns:
         bdict (dict): Result dictionary
@@ -87,59 +88,59 @@
         adict = {'key1': 'val1', 'key2': None,'key3': 'val3'}
         bdict = remove_nones(adict)
         >> {'key1': 'bval1', 'key3': 'val3'}
     """
     return {k: v for k, v in adict.items() if v is not None}
 
 
-def dumps(adict):
-    """ Dumps dictionary into Json string. Generalizes to lists
+def dumps(adict: Union[dict, list]) -> Union[list, str]:
+    """Dumps dictionary into Json string. Generalizes to lists
 
-        ajson = dumps(adict)
+    ajson = dumps(adict)
 
-        Args:
-            adict (dict or list): Dictionary
-        Returns:
-            ajson (str or list): Json strings
-        """
-    ajson = ''
+    Args:
+        adict (dict or list): Dictionary
+    Returns:
+        ajson (str or list): Json strings
+    """
+    ajson = ""
     if isinstance(adict, dict):
         ajson = json.dumps(adict)
     elif isinstance(adict, list):
         ajson = [json.dumps(idict) for idict in adict]
     return ajson
 
 
-def loads(ajson):
-    """ Loads Json string into a dictionary. Generalizes to lists
+def loads(ajson: Union[list, str]) -> Union[dict, list]:
+    """Loads Json string into a dictionary. Generalizes to lists
 
-        adict = loads(ajson)
+    adict = loads(ajson)
 
-        Args:
-            ajson (str or list): Json strings
-        Returns:
-            adict (dict or list): Dictionary
-        """
+    Args:
+        ajson (str or list): Json strings
+    Returns:
+        adict (dict or list): Dictionary
+    """
     adict = {}
     if isinstance(ajson, str):
         adict = json.loads(ajson)
     elif isinstance(ajson, list):
         adict = [json.loads(ijson) for ijson in ajson]
     return adict
 
 
-def set_(alist):
-    """ Return a set of unique dictionaries in alist
+def set_(alist: List[dict]) -> List[dict]:
+    """Return a set of unique dictionaries in alist
 
-        aset = set_(alist)
+    aset = set_(alist)
 
-        Args:
-            alist (list): List of dictionary
-        Returns:
-            aset (list): List of dictionary
-        """
+    Args:
+        alist (list): List of dictionary
+    Returns:
+        aset (list): List of dictionary
+    """
     aset = []
     if isinstance(alist, list):
         ajson = dumps(alist)
         ujson = list(set(ajson))
         aset = loads(ujson)
     return aset
```

### Comparing `boxfish-0.1.1/boxfish/utils/drivers.py` & `boxfish-0.1.2/boxfish/utils/drivers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # drivers.py
 
 """Drivers is a module that contains functions to access HTML pages via HTTP."""
 
 import os
+from typing import Any, Final, Optional
+
 import requests
 from selenium import webdriver
+
 from boxfish.utils import dicts, times, urls, utils
 
-DRIVERKEYS = ['package', 'sleep', 'requests', 'selenium']
-REQUESTSKEYS = ['headers', 'timeout']
-SELENIUMKEYS = ['filename', 'log', 'headless']
-MIN_TIMEOUT = 10
+DRIVERKEYS: Final = ["package", "sleep", "requests", "selenium"]
+REQUESTSKEYS: Final = ["headers", "timeout"]
+SELENIUMKEYS: Final = ["filename", "log", "headless"]
+MIN_TIMEOUT: Final = 10
 
 
-def get_page(url='', params=None, count=0):
-    """ Get single HTTP page from an url with the default driver
+def get_page(url: str = "", params: Optional[dict] = None, count: int = 0) -> str:
+    """Get single HTTP page from an url with the default driver
 
     page = get_page(url):
 
     Args:
         url (str): url
         params (dict): driver parameters
         count (int): page request counter
@@ -32,16 +35,18 @@
     try:
         page = request_page(adriver, url=url, params=params, count=count)
     finally:
         driver_stop(adriver)
     return page
 
 
-def request_page(driver, url='', params=None, count=0):
-    """ Request a single HTTP page from an url with driver
+def request_page(
+    driver: Any, url: str = "", params: Optional[dict] = None, count: int = 0
+) -> str:
+    """Request a single HTTP page from an url with driver
 
     page = request_page(driver, url):
 
     Args:
         driver (object): A driver object.Supported drivers are:
                          requests.sessions.Session or selenium.webdriver
         url (str): url
@@ -55,50 +60,62 @@
         HTTPError
         ConnectionError
         Timeout
         RequestException
     """
 
     params = create_params() if params is None else params
-    [psleep] = dicts.extract_values(params, ['sleep'])
-    page = ''
+    [psleep] = dicts.extract_values(params, ["sleep"])
+    page = ""
     try:
         if urls.is_valid_http(url):
             is_requests = isinstance(driver, requests.sessions.Session)
-            is_selenium = isinstance(driver, webdriver.firefox.webdriver.WebDriver) or \
-                          isinstance(driver, webdriver.chrome.webdriver.WebDriver)
+            is_selenium = isinstance(
+                driver, webdriver.firefox.webdriver.WebDriver
+            ) or isinstance(driver, webdriver.chrome.webdriver.WebDriver)
             if is_requests:
-                headers = driver.headers if 'headers' in dir(driver) else ''
-                timeout = max(driver.timeout if 'timeout' in dir(driver) else MIN_TIMEOUT, MIN_TIMEOUT)
+                headers = driver.headers if "headers" in dir(driver) else ""
+                timeout = max(
+                    driver.timeout if "timeout" in dir(driver) else MIN_TIMEOUT,
+                    MIN_TIMEOUT,
+                )
                 r = driver.get(url, headers=headers, timeout=timeout)
-                r.encoding = 'utf-8'
+                r.encoding = "utf-8"
                 page = r.text
             elif is_selenium:
                 driver.get(url)
                 page = driver.page_source
             else:
-                page = ''
+                page = ""
             times.sleep_on_count(psleep, count)
         else:
-            page = utils.read(url) if os.path.isfile(url) else ''
+            page = utils.read(url) if os.path.isfile(url) else ""
 
     except requests.exceptions.HTTPError as e:
         print("Http Error:", e)
     except requests.exceptions.ConnectionError as e:
         print("Error Connecting:", e)
     except requests.exceptions.Timeout as e:
         print("Timeout Error:", e)
     except requests.exceptions.RequestException as e:
         print("RequestException: ", e)
 
     return page
 
 
-def create_params(package='requests', headers=None, timeout=1, filename='', log='', sleep=None, headless=True):
-    """ Create driver parameters
+def create_params(
+    package: str = "requests",
+    headers: Optional[dict] = None,
+    timeout: int = 1,
+    filename: str = "",
+    log: str = "",
+    sleep: Optional[dict] = None,
+    headless: bool = True,
+) -> dict:
+    """Create driver parameters
 
     params = create_params(package='requests', headers='', timeout=1, filename='', log='', headless=True):
 
     Args:
         package (str): Name of the driver package. Supported packages are 'selenium' and 'requests'
         headers (dict): Driver headers
         timeout (int): Timeout between driver calls, in seconds
@@ -110,79 +127,84 @@
     Returns:
         params (dict): Driver parameters
     """
 
     headers = {} if headers is None else headers
 
     params = dict.fromkeys(DRIVERKEYS, {})
-    params['package'] = package if package in ('selenium', 'requests') else 'requests'
-    params['sleep'] = sleep if isinstance(sleep, dict) else {}
+    params["package"] = package if package in ("selenium", "requests") else "requests"
+    params["sleep"] = sleep if isinstance(sleep, dict) else {}
 
-    params['requests'] = dict.fromkeys(REQUESTSKEYS, {})
-    params['requests']['headers'] = headers
-    params['requests']['timeout'] = max(timeout, MIN_TIMEOUT)
-
-    params['selenium'] = dict.fromkeys(SELENIUMKEYS, {})
-    params['selenium']['filename'] = filename
-    params['selenium']['log'] = log
-    params['selenium']['headless'] = headless
+    params["requests"] = dict.fromkeys(REQUESTSKEYS, {})
+    params["requests"]["headers"] = headers
+    params["requests"]["timeout"] = max(timeout, MIN_TIMEOUT)
+
+    params["selenium"] = dict.fromkeys(SELENIUMKEYS, {})
+    params["selenium"]["filename"] = filename
+    params["selenium"]["log"] = log
+    params["selenium"]["headless"] = headless
     return params
 
 
-def driver_start(params=None):
-    """ Start driver
+def driver_start(params: Optional[dict] = None) -> Any:
+    """Start driver
 
     driver = driver_start(params)
 
     Args:
         params (dict): Driver parameters with keys DRIVERKEYS
 
     Returns:
         driver (obj): Driver object. Supported objects are:
                       requests.sessions.Session or selenium.webdriver
     """
 
     driver = None
 
     if isinstance(params, dict):
-        if params['package'] == 'requests':
+        if params["package"] == "requests":
             driver = requests.Session()
-            driver.headers = params['requests']['headers']
-            driver.timeout = params['requests']['timeout']
-        elif params['package'] == 'selenium':
-            if 'gecko' in params['selenium']['filename']:
+            driver.headers = params["requests"]["headers"]
+            driver.timeout = params["requests"]["timeout"]
+        elif params["package"] == "selenium":
+            if "gecko" in params["selenium"]["filename"]:
                 options = webdriver.firefox.options.Options()
-                options.headless = params['selenium']['headless']
-                driver = webdriver.Firefox(executable_path=params['selenium']['filename'],
-                                           service_log_path=params['selenium']['log'],
-                                           options=options)
-            elif 'chrome' in params['selenium']['filename']:
+                options.headless = params["selenium"]["headless"]
+                driver = webdriver.Firefox(
+                    executable_path=params["selenium"]["filename"],
+                    service_log_path=params["selenium"]["log"],
+                    options=options,
+                )
+            elif "chrome" in params["selenium"]["filename"]:
                 options = webdriver.chrome.options.Options()
-                options.headless = params['selenium']['headless']
-                str_log = "--log-path=" + params['selenium']['log']
-                driver = webdriver.Chrome(executable_path=params['selenium']['filename'],
-                                          service_args=["--verbose", str_log],
-                                          options=options)
+                options.headless = params["selenium"]["headless"]
+                str_log = "--log-path=" + params["selenium"]["log"]
+                driver = webdriver.Chrome(
+                    executable_path=params["selenium"]["filename"],
+                    service_args=["--verbose", str_log],
+                    options=options,
+                )
             else:
                 # TODO error handling
-                print('Driver not found')
+                print("Driver not found")
     return driver
 
 
-def driver_stop(driver):
-    """ Stop driver
+def driver_stop(driver: Any) -> None:
+    """Stop driver
 
     driver_stop(driver)
 
     Args:
         driver (obj): Driver object. Supported objects are:
                       requests.sessions.Session or selenium.webdriver
 
     Returns:
         None
     """
 
     if driver:
-        is_selenium = isinstance(driver, webdriver.firefox.webdriver.WebDriver) or \
-                      isinstance(driver, webdriver.chrome.webdriver.WebDriver)
+        is_selenium = isinstance(
+            driver, webdriver.firefox.webdriver.WebDriver
+        ) or isinstance(driver, webdriver.chrome.webdriver.WebDriver)
         if is_selenium:
             driver.close()
```

### Comparing `boxfish-0.1.1/boxfish/utils/lists.py` & `boxfish-0.1.2/boxfish/utils/lists.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # lists.py
 
 """Lists is a module that contains functions for lists"""
 
 import csv
 import os
+from typing import Optional
+
 from boxfish.utils.strings import filename_append_date
 from boxfish.utils.utils import create_folder_if_not_exist
 
 
 # General
-def is_empty(alist):
-    """ Returns true if list is empty or contains '' or None only
+def is_empty(alist: Optional[list]) -> bool:
+    """Returns true if list is empty or contains '' or None only
 
     tf = is_empty(alist)
 
     Args:
         alist (list): List
     Returns:
         tf (bool): True if list is empty or contains '' or None only
@@ -28,45 +30,48 @@
         tf = is_empty(alist)
         >> True
 
         alist = [0, '']
         tf = is_empty(alist)
         >> False
     """
-    return all(item == '' or item is None for item in alist)
+    return all(item == "" or item is None for item in alist)
 
 
-def flatten(alist):
-    """ Merges a list of lists of items into a single list of items
+def flatten(alist: list) -> list:
+    """Merges a list of lists of items into a single list of items
 
     Source: https://stackoverflow.com/questions/952914/how-to-make-a-flat-list-out-of-list-of-lists
 
     flist = flatten(alist)
 
     Args:
         alist (list): List of lists of items
     Returns:
-        flist (bool): List of items
+        flist (list): List of items
 
     Example:
         alist = [1,2,3]
         blist = [1, alist, 2*alist]
         blist
         >> [1, [1, 2, 3], [1, 2, 3, 1, 2, 3]]
 
         flist = flatten()
         flist
         >> [1, 1, 2, 3, 1, 2, 3, 1, 2, 3]
     """
-    def f(x): return [x] if not isinstance(x, list) else x
+
+    def f(x):
+        return [x] if not isinstance(x, list) else x
+
     return [item for sublist in alist for item in f(sublist)]
 
 
-def unique(alist):
-    """ Return list with duplicates removed
+def unique(alist: list) -> list:
+    """Return list with duplicates removed
 
     ulist = unique(alist)
 
     Args:
         alist (list): List of items
     Returns:
         ulist (list): List of unique items from alist
@@ -77,15 +82,15 @@
         ulist = unique(alist)
         >> ulist = (1,2,3,4,5)
     """
     return list(set(alist))
 
 
 def is_equal_length(*args):
-    """ Returns true if all inputs are lists and have the same length
+    """Returns true if all inputs are lists and have the same length
 
     tf = is_equal_lenght(alist,blist)
 
     Args:
         *args:
             alist (list): List of items
     Returns:
@@ -103,15 +108,15 @@
         tf = tf and isinstance(arg, list)
         tf = tf and (length == len(arg) or length is None)
         length = len(arg) if length is None else length
     return tf
 
 
 def to_list(*args):
-    """ Returns a list with the items in args
+    """Returns a list with the items in args
 
     alist = to_list(*args)
 
     Args:
         *args: list of items
     Returns:
         alist (list): list of items in *args
@@ -122,15 +127,15 @@
         b = 'Hello'
         >> alist = to_list(a, b)
     """
     return [value for value in args]
 
 
 def reshape(*args):
-    """ Reshape returns a tuple of lists of the same length in case
+    """Reshape returns a tuple of lists of the same length in case
     all list arguments have the same length L.
     All non-list arguments are converted to a list of length L by duplication.
     Otherwise, the function returns a tuple of None
 
     alist = reshape(*args)
 
     Args:
@@ -145,86 +150,101 @@
         d = 'Hello'
         >> [a2,b2,c2,d2] = reshape(a, b, c, d)
     """
     arglists = [arg if isinstance(arg, list) else to_list(arg) for arg in args]
     lenlists = [len(i) for i in arglists]
     length = max(lenlists)
     is_valid = all(alen == length or alen == 1 for alen in lenlists)
-    return (length*alist if len(alist) == 1 else alist for alist in arglists) if is_valid \
+    return (
+        (length * alist if len(alist) == 1 else alist for alist in arglists)
+        if is_valid
         else tuple([None for _ in arglists])
+    )
+
 
 # I/O functions
 
 
-def to_csv(alist, filename, date_format='', overwrite=False, header=None, quoting=csv.QUOTE_NONNUMERIC):
-    """ Save list to csv file
+def to_csv(
+    alist: list,
+    filename: str,
+    date_format: str = "",
+    overwrite: bool = False,
+    header: Optional[list] = None,
+    quoting: int = csv.QUOTE_NONNUMERIC,
+) -> str:
+    """Save list to csv file. Dictionaries are converted to lists without key validation.
 
     fullname = to_csv(alist, filename, date_format, overwrite)
 
     Args:
         alist (list): list of rows (lists)
         filename (str): Filename
         # Optional
         date_format (str): Date format in strftime format. Date is added to filename
         overwrite (bool): Overwrite existing file if True else append
-        header (list): Header
+        header (list): Column headers
         quoting (int): CSV quoting constant
     Returns:
-        fullname: Full filename including date
+        fullname (str): Full filename including date
 
     Example:
         fullname = to_csv(alist, 'file.csv', date_format='%Y%m%d, overwrite=True)
     """
     if (alist is not None) and os.path.basename(filename):
         create_folder_if_not_exist(os.path.dirname(filename))
         fullname = filename_append_date(filename, date_format)
 
-        if os.path.exists(fullname) and not overwrite:
-            with open(fullname, 'a', newline='', encoding='utf-8') as f:
-                csv_writer = csv.writer(f, quoting=quoting)
-                if not is_empty(header):
-                    csv_writer.writerow(header)
-                csv_writer.writerows(alist)
-        else:
-            with open(fullname, 'wt', newline='', encoding='utf-8') as f:
-                csv_writer = csv.writer(f, quoting=quoting)
-                if header:
-                    csv_writer.writerow(header)
+        read_mode = "a" if os.path.exists(fullname) and not overwrite else "wt"
+        read_dict = (
+            True
+            if alist and isinstance(alist, list) and isinstance(alist[0], dict)
+            else False
+        )
+
+        with open(fullname, read_mode, newline="", encoding="utf-8") as f:
+            csv_writer = csv.writer(f, quoting=quoting)
+            if header:
+                csv_writer.writerow(header)
+            if read_dict:
+                for arow in alist:
+                    csv_writer.writerow(arow.values())
+            else:
                 csv_writer.writerows(alist)
     else:
-        fullname = ''
+        fullname = ""
     return fullname
 
 
-def from_csv(filename, quoting=csv.QUOTE_NONNUMERIC):
-    """ Load list from csv file
+def from_csv(filename: str, quoting: int = csv.QUOTE_NONNUMERIC) -> list:
+    """Load list from csv file
 
-        alist = from_csv(filename)
+    alist = from_csv(filename)
 
-        Args:
-            filename (str): Filename
-            quoting (int): CSV quoting constant
-        Returns:
-            alist (list): list of rows (lists)
-
-        Example:
-            alist = from_csv('file.csv')
-        """
+    Args:
+        filename (str): Filename
+        quoting (int): CSV quoting constant
+    Returns:
+        alist (list): list of rows (lists)
+
+    Example:
+        alist = from_csv('file.csv')
+    """
     alist = []
     if os.path.exists(filename):
-        with open(filename, 'r', newline='') as f:
+        with open(filename, "r", newline="") as f:
             csv_reader = csv.reader(f, quoting=quoting)
             for row in csv_reader:
                 alist.append(row)
     return alist
 
 
 # Set functions. Set functions remove duplicates
-def intersect(alist, blist):
-    """ Return list with intersection of alist and blist
+def intersect(alist: list, blist: list) -> list:
+    """Return list with intersection of alist and blist
 
     clist = intersect(alist, blist)
 
     Args:
         alist (list): List of items
         blist (list): List of items
     Returns:
@@ -236,16 +256,16 @@
         blist = [2,4,6]
         clist = intesect(alist, blist)
         >> clist = (2,4)
     """
     return list(set(alist) & set(blist))
 
 
-def union(alist, blist):
-    """ Return list with union of alist and blist
+def union(alist: list, blist: list) -> list:
+    """Return list with union of alist and blist
 
     clist = union(alist, blist)
 
     Args:
         alist (list): List of items
         blist (list): List of items
     Returns:
@@ -257,16 +277,16 @@
         blist = [2,4,6]
         clist = union(alist, blist)
         >> clist = (1,2,3,4,5,6)
     """
     return list(set(alist) | set(blist))
 
 
-def difference(alist, blist):
-    """ Return list with difference of alist and blist
+def difference(alist: list, blist: list) -> list:
+    """Return list with difference of alist and blist
 
     clist = difference(alist, blist)
 
     Args:
         alist (list): List of items
         blist (list): List of items
     Returns:
@@ -278,16 +298,16 @@
         blist = [2,4,6]
         clist = difference(alist, blist)
         >> clist = (1,3,5)
     """
     return list(set(alist) - set(blist))
 
 
-def is_subset(alist, blist):
-    """ Return true if alist is a subset of blist
+def is_subset(alist: list, blist: list) -> bool:
+    """Return true if alist is a subset of blist
 
     tf = is_susbet(alist, blist)
 
     Args:
         alist (list): List of items
         blist (list): List of items
     Returns:
@@ -299,16 +319,16 @@
         blist = [6,5,4,3,2,1]
         tf = is_subset(alist, blist)
         >> tf = True
     """
     return set(alist).issubset(set(blist))
 
 
-def is_disjoint(alist, blist):
-    """ Return true if alist and blist are disjoint
+def is_disjoint(alist: list, blist: list) -> bool:
+    """Return true if alist and blist are disjoint
 
     tf = is_disjoint(alist, blist)
 
     Args:
         alist (list): List of items
         blist (list): List of items
     Returns:
```

### Comparing `boxfish-0.1.1/boxfish/utils/strings.py` & `boxfish-0.1.2/boxfish/utils/strings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 # strings.py
 
 """Strings is a module that contains general functions for working with strings"""
 
 import os
 import time
+from typing import Any, Optional
 
-DATE_FILE = '%Y%m%d'
+DATE_FILE = "%Y%m%d"
 
 
 # General
-def rstrip_endswith(string, endswith):
-    """ Strip the right-most characters endswith from string
+def rstrip_endswith(string: str, endswith: str) -> str:
+    """Strip the right-most characters endswith from string
 
     str = rstrip_endswith(string, endswith):
 
     Args:
         string (str): input string
         endswith (str): string to be stripped from the right of string
 
     Returns:
         str (str): stripped string
     """
-    return string[:-len(endswith)] if string.endswith(endswith) else string
+    return string[: -len(endswith)] if string.endswith(endswith) else string
 
 
-def replace_newlines(string, replace_string=''):
-    """ Replace any new line characters (\\r, \\n, \\r\\n) with replace_string
+def replace_newlines(string: str, replace_string: str = "") -> str:
+    """Replace any new line characters (\\r, \\n, \\r\\n) with replace_string
 
     str = replace_newlines(string, replace_string='')
 
     Args:
         string (str): input string
         replace_string (str): string that replaces newline characters
 
     Returns:
         str (str): stripped string
     """
     return replace_string.join(string.splitlines())
 
 
-def is_int(string):
-    """ Returns true if string represents an integer
+def is_int(string: str) -> bool:
+    """Returns true if string represents an integer
 
     tf = is_int(string)
 
     Args:
         string (str): input string
 
     Returns:
@@ -53,16 +54,16 @@
     try:
         int(string)
         return True
     except ValueError:
         return False
 
 
-def is_float(string):
-    """ Returns true if string represents a float
+def is_float(string: str) -> bool:
+    """Returns true if string represents a float
 
     tf = is_float(string)
 
     Args:
         string (str): input string
 
     Returns:
@@ -71,87 +72,88 @@
     try:
         float(string)
         return True
     except ValueError:
         return False
 
 
-def to_int(string):
-    """ Converts a string to int
+def to_int(string: str) -> Optional[int]:
+    """Converts a string to int
 
     aint = to_int(string)
 
     Args:
         string (str): input string
 
     Returns:
         aint (int or None): int representation of astring
     """
     return int(float(string)) if is_float(string) else None
 
 
-def to_float(string):
-    """ Converts a string to float
+def to_float(string: str) -> Optional[float]:
+    """Converts a string to float
 
     afloat = to_float(string)
 
     Args:
         string (str): input string
 
     Returns:
         afloat (int or None): float representation of astring
     """
     return float(string) if is_float(string) else None
 
 
-def get_type(obj):
-    """ Return type as string
+def get_type(obj: Any) -> str:
+    """Return type as string
 
     astr = get_type(obj)
 
     Args:
         obj : object
 
     Returns:
         astr (str): string of type
     """
     astr = str(type(obj))
     alist = astr.split("'")
-    if len(alist)>1:
+    if len(alist) > 1:
         astr = alist[1]
     else:
-        astr = ''
+        astr = ""
     return astr
 
 
 # Regex
 
-def re_literals(string):
-    """ Regex conversion of string creating literals for regex meta characters
 
-        restring = re_literals(string)
+def re_literals(string: str) -> str:
+    """Regex conversion of string creating literals for regex meta characters
 
-        Args:
-            string (str): input string
+    restring = re_literals(string)
 
-        Returns:
-            restring (str): Regex string
-        """
-    re_chars = ['\\', '^', '$', '.', '|', '?', '*', '+', '(', ')', '[', ']', '{', '}']
+    Args:
+        string (str): input string
+
+    Returns:
+        restring (str): Regex string
+    """
+    re_chars = ["\\", "^", "$", ".", "|", "?", "*", "+", "(", ")", "[", "]", "{", "}"]
     restring = string
 
     for char in re_chars:
-        restring = restring.replace(char, '\\' + char)
+        restring = restring.replace(char, "\\" + char)
 
     return restring
 
 
 # Filenames
-def filename_append_date(filename, date_format=DATE_FILE):
-    """ Filename with current date appended
+def filename_append_date(filename: str, date_format: str = DATE_FILE) -> str:
+    """Filename with current date appended
 
     filename_date = filename_append_date(filename, date_format)
 
     Args:
         filename (str): Filename
         date_format (str): Date in strftime format
     Returns:
@@ -163,16 +165,16 @@
         filename_date = filename_append_date(filename, date_format)
         >> 'filename20210513.ext'
     """
     file_pre, file_extension = os.path.splitext(filename)
     return file_pre + time.strftime(date_format) + file_extension
 
 
-def filename_append_extension(filename, default_extension):
-    """ Filename with default extension appended
+def filename_append_extension(filename: str, default_extension: str) -> str:
+    """Filename with default extension appended
 
     filename_ext = filename_append_extension(filename, default_extension)
 
     Args:
         filename (str): Filename
         default_extension (str): Default extension
 
@@ -190,12 +192,12 @@
 
         filename = r'D:\filename'
         default_extension = '.py'
         filename_ext = filename_append_extension(filename, default_extension)
         >> 'D:\\filename.py'
     """
     filename, file_extension = os.path.splitext(filename)
-    file_extension = default_extension if not file_extension else ''
-    if not file_extension[0] == '.':
+    file_extension = default_extension if not file_extension else ""
+    if not file_extension[0] == ".":
         raise TypeError
 
     return filename + file_extension
```

### Comparing `boxfish-0.1.1/boxfish/utils/times.py` & `boxfish-0.1.2/boxfish/utils/times.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # times.py
 
 """Times is a module that contains functions that interact with times and dates"""
 
 import time
+from typing import Any, Final
 
-DATE_JAPANESE = '%Y-%m-%d'
-DATETIME_JAPANESE = '%Y-%m-%d %H:%M:%S'
-DATETIME_FILE = '%Y%m%d%H%M%S'
-DATE_FILE = '%Y%m%d'
-TIME_FILE = '%H%M%S'
+DATE_JAPANESE: Final = "%Y-%m-%d"
+DATETIME_JAPANESE: Final = "%Y-%m-%d %H:%M:%S"
+DATETIME_FILE: Final = "%Y%m%d%H%M%S"
+DATE_FILE: Final = "%Y%m%d"
+TIME_FILE: Final = "%H%M%S"
 
 
 # Strings
-def strftime(t=None, string='', sep=' ', date_format=DATETIME_JAPANESE, string_first=False):
-    """ Return a formatted string which contains date/time and a text string
+def strftime(
+    t: Any = None,
+    string: str = "",
+    sep: str = " ",
+    date_format: str = DATETIME_JAPANESE,
+    string_first: bool = False,
+) -> str:
+    """Return a formatted string which contains date/time and a text string
 
     str = strftime(t=None, string='', sep=' ', date_format=DATETIME_JAPANESE, string_first=True)
 
     Args:
         t (float or tuple or time.struct_time): date/time
         string (str): Input string
         sep (str): Seperator between date and time and string
@@ -27,20 +34,30 @@
     Returns:
         str (str): Output string which contains input string and date/time
 
     Example:
         >>> strftime(t=time.time(),string='Hello World', sep=' ')
         '2021-05-01 18:08:31 Hello World'
     """
-    strdatetime = time.strftime(date_format) if t is None else time.strftime(date_format, to_struct_time(t))
+    strdatetime = (
+        time.strftime(date_format)
+        if t is None
+        else time.strftime(date_format, to_struct_time(t))
+    )
     return string + sep + strdatetime if string_first else strdatetime + sep + string
 
 
-def strfdate(t=None, string='', sep=' ', date_format=DATE_JAPANESE, string_first=False):
-    """ Return a formatted string which contains date and a text string
+def strfdate(
+    t: Any = None,
+    string: str = "",
+    sep: str = " ",
+    date_format: str = DATE_JAPANESE,
+    string_first: bool = False,
+):
+    """Return a formatted string which contains date and a text string
 
     str = strfdate(t=None, string='', sep=' ', date_format=DATE_JAPANESE, string_first=False):
 
     Args:
         t (float or tuple or time.struct_time): date
         string (str): Input string
         sep (str): Seperator between date  and string
@@ -51,19 +68,21 @@
         str (str): Output string which contains input string and date
 
     Example:
         >>> strfdate(t=time.time(),string='Hello World', sep=' ')
         '2021-05-01 Hello World'
     """
 
-    return strftime(t=t, string=string, sep=sep, date_format=date_format, string_first=string_first)
+    return strftime(
+        t=t, string=string, sep=sep, date_format=date_format, string_first=string_first
+    )
 
 
 # Conversion
-def to_float(t=None):
+def to_float(t: Any = None) -> float:
     """Convert time t to type float. Returns current time if no time is provided
 
         t = to_float()
 
     Args:
         t (struct_time or tuple): Time as struct_time or tuple
 
@@ -72,24 +91,30 @@
 
     Raises:
           OverflowError or ValueError for invalid time t
     """
 
     t = time.time() if t is None else t
 
-    if not isinstance(t, tuple) and not isinstance(t, time.struct_time) \
-            and not isinstance(t, int) and not isinstance(t, float):
+    if (
+        not isinstance(t, tuple)
+        and not isinstance(t, time.struct_time)
+        and not isinstance(t, int)
+        and not isinstance(t, float)
+    ):
         raise ValueError
 
-    ftime = time.mktime(t) if isinstance(t, tuple) or isinstance(t, time.struct_time) else t
+    ftime = (
+        time.mktime(t) if isinstance(t, tuple) or isinstance(t, time.struct_time) else t
+    )
 
     return ftime
 
 
-def to_struct_time(t=None):
+def to_struct_time(t: Any = None) -> tuple:
     """Convert time t to type time.struct_time. Returns current time if no time is provided
 
         t = to_struct_time()
 
     Args:
         t (float or tuple): Time as float or float
 
@@ -102,15 +127,15 @@
 
     t = time.time() if t is None else t
     stime = time.localtime(t) if isinstance(t, float) else time.struct_time(t)
 
     return stime
 
 
-def to_tuple(t=None):
+def to_tuple(t: Any = None) -> tuple:
     """Convert time t to type tuple. Returns current time if no time is provided
 
         t = to_tuple()
 
     Args:
         t (float or struct_time): Time as float or struct_time
 
@@ -120,21 +145,30 @@
     Raises:
           OverflowError or ValueError for invalid time t
     """
 
     t = time.time() if t is None else t
     stime = time.localtime(t) if isinstance(t, float) else t
 
-    return (stime.tm_year, stime.tm_mon, stime.tm_mday, stime.tm_hour, stime.tm_min,
-            stime.tm_sec, stime.tm_wday, stime.tm_yday, stime.tm_isdst)
+    return (
+        stime.tm_year,
+        stime.tm_mon,
+        stime.tm_mday,
+        stime.tm_hour,
+        stime.tm_min,
+        stime.tm_sec,
+        stime.tm_wday,
+        stime.tm_yday,
+        stime.tm_isdst,
+    )
 
 
 # Sleep
-def sleep_on_count(adict, cnt):
-    """ Sleeps dict[counter] seconds if cnt+1 is a multiple of counter
+def sleep_on_count(adict: dict, cnt: int) -> None:
+    """Sleeps dict[counter] seconds if cnt+1 is a multiple of counter
 
     Or: when iterating over cnt, sleep_on_count pauses for dict[counter] seconds every counter iterations
 
     sleep_on_count(adict, cnt)
 
     Args:
         adict (dict) Keys are counters (int), values are seconds (int)
@@ -145,16 +179,16 @@
     """
 
     for counter, sec in adict.items():
         if (cnt + 1) % int(counter) == 0:
             time.sleep(sec)
 
 
-def sleep_until(end_time):
-    """ Sleeps until end_time
+def sleep_until(end_time: int) -> None:
+    """Sleeps until end_time
 
     sleep_until(end_time)
 
     Args:
         end_time (struct_time or float or tuple)
 
     Returns:
```

### Comparing `boxfish-0.1.1/boxfish/utils/urls.py` & `boxfish-0.1.2/boxfish/utils/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # urls.py
 
 """ urls contains functions to parse url strings """
 
-from urllib.parse import parse_qsl, urlencode, urlsplit, urljoin
+from typing import Any, List, Optional, Union
+from urllib.parse import parse_qsl, urlencode, urljoin, urlsplit
+
 from boxfish.utils.dicts import get_subset, remove_nones
 from boxfish.utils.lists import reshape
 
 
-def set_components(url, **kwargs):
-    """ Set url components based on dict or key value pairs
+def set_components(url: str, **kwargs) -> str:
+    """Set url components based on dict or key value pairs
 
     url = set_components(url, scheme=scheme, netloc=netloc, path=path, query=query, fragment=fragment)
 
     Args:
         url (str) : url
         **kwargs: # url components
             scheme (str): Scheme
@@ -20,26 +22,32 @@
             path (str): Path
             query (str or dict): Query
             fragment (str or dict): Fragment
     Returns:
         url (str)
     """
 
-    kwargs = get_subset(remove_nones(kwargs), ['scheme', 'netloc', 'path', 'query', 'fragment'])
-    if 'query' in kwargs:
-        kwargs['query'] = _dict_to_query(kwargs['query']) if isinstance(kwargs['query'], dict) else kwargs['query']
+    kwargs = get_subset(
+        remove_nones(kwargs), ["scheme", "netloc", "path", "query", "fragment"]
+    )
+    if "query" in kwargs:
+        kwargs["query"] = (
+            _dict_to_query(kwargs["query"])
+            if isinstance(kwargs["query"], dict)
+            else kwargs["query"]
+        )
 
     pr = urlsplit(url)
     pr = pr._replace(**kwargs)
     url = pr.geturl()
     return url
 
 
-def get_components(url):
-    """ Set url components based on dict or key value pairs
+def get_components(url: str) -> dict:
+    """Set url components based on dict or key value pairs
 
     url = set(url, query=query, path=path, )
 
     Args:
         url (str) : url
     Returns:
         components (dict)
@@ -47,88 +55,90 @@
             netloc (str): Netloc
             path (str): Path
             query (str): Query
             fragment (str): Fragment
     """
     pr = urlsplit(url)
     components = dict()
-    components['scheme'] = pr.scheme
-    components['netloc'] = pr.netloc
-    components['path'] = pr.path
-    components['query'] = pr.query
-    components['fragment'] = pr.fragment
+    components["scheme"] = pr.scheme
+    components["netloc"] = pr.netloc
+    components["path"] = pr.path
+    components["query"] = pr.query
+    components["fragment"] = pr.fragment
     return components
 
 
-def replace_subpath(url, subpath, index):
-    """ Replace subpath replaces a single subpath of the path of an url
+def replace_subpath(url: str, subpath: str, index: int) -> str:
+    """Replace subpath replaces a single subpath of the path of an url
 
     url = replace_subpath(url, subpath, index=0)
 
     Args:
         url (str) : url
         subpath (str): subpath
         index (int): index of path between 0 and n-1 or between -1 and -n
     Returns:
         aurl (str) : url
     """
 
     aurl = url
     adict = get_components(url)
-    dictpath = _path_to_dict(adict['path'])
+    dictpath = _path_to_dict(adict["path"])
     keys = list(dictpath.keys())
 
-    if len(keys)==0:
+    if len(keys) == 0:
         aurl = set_components(url, path=subpath)
     else:
         if -len(keys) <= index < len(keys):
             dictpath[keys[index]] = subpath
             aurl = set_components(url, path=_dict_to_path(dictpath))
     return aurl
 
 
-def replace_subquery(url, subquery):
-    """ Replace subquery replaces part of a query of an url
+def replace_subquery(url: str, subquery: Union[dict, str]) -> str:
+    """Replace subquery replaces part of a query of an url
 
     url = replace_subquery(url, subquery)
 
     Args:
         url (str) : url
         subquery (str or dict): sub query
     Returns:
         aurl (str) : url
     """
 
     adict = get_components(url)
-    dictquery = _query_to_dict(adict['query'])
+    dictquery = _query_to_dict(adict["query"])
     dictsubquery = _query_to_dict(subquery) if isinstance(subquery, str) else subquery
 
     dictquery = dict(dictquery, **dictsubquery)
     aurl = set_components(url, query=_dict_to_query(dictquery))
     return aurl
 
 
-def update_relative_path(url, newpath):
-    """ Update url with a relative newpath.
+def update_relative_path(url: str, newpath: str) -> str:
+    """Update url with a relative newpath.
     Existing path and query are overwritten by newpath
 
     url = update_path(url, newpath)
 
     Args:
         url (str) : url
         newpath (str): subpath
     Returns:
         aurl (str) : url
     """
-    aurl = urljoin(url,newpath)
+    aurl = urljoin(url, newpath)
     return aurl
 
 
-def create_url_list(url, query=None, path=None):
-    """ Create a list of urls based on a url, a query and/or path
+def create_url_list(
+    url: str, query: Union[list, str, None] = None, path: Union[list, str, None] = None
+) -> List[str]:
+    """Create a list of urls based on a url, a query and/or path
 
     url_list = create_url_list(url, query=query, path=path)
 
     Args:
         url (str) : url
         query (str or list): Query list
         path (str or list): Path list
@@ -140,71 +150,71 @@
     if url is not None:
         for index in range(len(url)):
             url_i = set_components(url[index], query=query[index], path=path[index])
             url_list.append(url_i)
     return url_list
 
 
-def is_valid_http(url):
-    """ Validate url syntax for http and https
+def is_valid_http(url: str) -> bool:
+    """Validate url syntax for http and https
 
     url = valid(url)
 
     Args:
         url (str) : url
     Returns:
         tf (bool) : True if url is a valid url
     """
     pr = urlsplit(url)
-    return (pr.scheme == 'http') or (pr.scheme == 'https')
+    return (pr.scheme == "http") or (pr.scheme == "https")
 
 
 # Private functions
-def _dict_to_path(adict):
-    """ Convert a dict to a url path
+def _dict_to_path(adict: dict) -> str:
+    """Convert a dict to a url path
 
-        path = _dict_to_path(adict)
+    path = _dict_to_path(adict)
 
-        Args:
-            adict (dict): key-value pairs
+    Args:
+        adict (dict): key-value pairs
 
-        Returns:
-            path (str): url path /value1/value2 based on values in adict
+    Returns:
+        path (str): url path /value1/value2 based on values in adict
     """
-    path = ''
+    path = ""
     if type(adict) == dict:
         for value in adict.values():
-            path = path + '/' + value.lstrip('/')
+            path = path + "/" + value.lstrip("/")
     return path
 
 
-def _path_to_dict(path, keys=None):
-    """ Convert a url path to a dict
+def _path_to_dict(path: str, keys: Optional[list] = None):
+    """Convert a url path to a dict
 
-        adict = _path_to_dict(path, keys=None)
+    adict = _path_to_dict(path, keys=None)
 
-        Args:
-            path (str): url path /value1/value2
-            keys (list): list of key strings or None
+    Args:
+        path (str): url path /value1/value2
+        keys (list): list of key strings or None
 
-        Returns:
-            adict (dict): key-value pairs for each element in path
+    Returns:
+        adict (dict): key-value pairs for each element in path
     """
     adict = {}
     if type(path) == str:
-        values = list(filter(None, path.split('/')))
+        values = list(filter(None, path.split("/")))
         elems = len(values)
 
         if keys is None:
             keys = ["{}".format(i) for i in range(elems)]
         if len(keys) == elems:
             for i in range(elems):
                 adict[keys[i]] = values[i]
     return adict
 
 
-def _query_to_dict(query):
+def _query_to_dict(query: Any) -> dict:
     return dict(parse_qsl(query))
 
 
-def _dict_to_query(adict):
+def _dict_to_query(adict: dict) -> Any:
     return urlencode(adict)
```

### Comparing `boxfish-0.1.1/boxfish/utils/utils.py` & `boxfish-0.1.2/boxfish/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,153 +2,163 @@
 
 """Utils is a module that contains utility functions without need of their own module"""
 
 import json
 import os
 import shutil
 from pathlib import Path
+from typing import Union
 
 
 # Files
-def makedir(spath):
-    """ Make a new directory
+def makedir(spath: str) -> None:
+    """Make a new directory
 
-        Args:
-            spath (str): Full path of new directory
-        Returns:
-            None
+    Args:
+        spath (str): Full path of new directory
+    Returns:
+        None
 
-        Example:
+    Example:
     """
     try:
         Path(spath).mkdir(parents=True, exist_ok=True)
     except OSError:
-        print('Parent folder does not exist')
+        print("Parent folder does not exist")
 
 
-def create_folder_if_not_exist(folder):
-    """ Create folder
+def create_folder_if_not_exist(folder: str) -> None:
+    """Create folder
 
-        Args:
-            folder (str): Full path of new folder
-        Returns:
-            None
+    Args:
+        folder (str): Full path of new folder
+    Returns:
+        None
 
-        Example:
+    Example:
     """
     if folder and not os.path.exists(folder):
         os.makedirs(folder)
 
 
-def read(filename, filetype='text', encoding='utf-8'):
-    """ Read text from file
+def read(
+    filename: str, filetype: str = "text", encoding: str = "utf-8"
+) -> Union[dict, str]:
+    """Read text from file
 
-        text = read(filename)
+    text = read(filename)
 
-        Args:
-            filename (str): file name
-            filetype (str): file type ('text' or 'json')
-            encoding (str): file encoding
+    Args:
+        filename (str): file name
+        filetype (str): file type ('text' or 'json')
+        encoding (str): file encoding
 
-        Returns:
-            text (str or json):
+    Returns:
+        text (str or json dict):
     """
 
-    text = {} if filetype == 'json' else ''
+    text = {} if filetype == "json" else ""
 
     try:
         with open(filename, "r", encoding=encoding) as file:
-            if filetype == 'json':
+            if filetype == "json":
                 text = json.load(file)
             else:
                 text = file.read()
 
     except IOError:
-        print('Error: File does not appear to exist.')
+        print("Error: File does not appear to exist.")
     return text
 
 
-def read_json(filename, encoding='utf-8'):
-    """ Read json from file
+def read_json(filename: str, encoding: str = "utf-8") -> dict:
+    """Read json from file
 
-        ajson = read(filename)
+    ajson = read(filename)
 
-        Args:
-            filename (str): file name
-            encoding (str): file encoding
+    Args:
+        filename (str): file name
+        encoding (str): file encoding
 
-        Returns:
-            ajson (dict)
+    Returns:
+        ajson (dict)
     """
-    return read(filename, filetype='json', encoding=encoding)
+    return read(filename, filetype="json", encoding=encoding)
 
 
-def write(filename, text, filetype='text', encoding='utf-8', indent=4):
-    """ Write text to file
+def write(
+    filename: str,
+    text: Union[dict, str],
+    filetype: str = "text",
+    encoding: str = "utf-8",
+    indent: int = 4,
+) -> None:
+    """Write text to file
 
-        write(filename)
+    write(filename)
 
-        Args:
-            filename (str): file name of configuration
-            text (str or dict): text
-            filetype (str): file type ('text' or 'json')
-            encoding (str): file encoding
-            indent (int): text indentation
+    Args:
+        filename (str): file name of configuration
+        text (str or dict): text
+        filetype (str): file type ('text' or 'json')
+        encoding (str): file encoding
+        indent (int): text indentation
 
-        Returns:
-            None
+    Returns:
+        None
 
-        Raises:
-            IOError (): error in case function cannot write to filename
+    Raises:
+        IOError (): error in case function cannot write to filename
     """
 
     try:
         with open(filename, "w", encoding=encoding) as file:
-            if filetype == 'json':
+            if filetype == "json":
                 json.dump(text, file, indent=indent)
             else:
                 file.write(text)
     except IOError:
-        print('Error: Cannot write to file.')
+        print("Error: Cannot write to file.")
 
 
-def write_json(filename, ajson, encoding='utf-8', indent=4):
-    """ Write json to file
+def write_json(
+    filename: str, ajson: dict, encoding: str = "utf-8", indent: int = 4
+) -> None:
+    """Write json to file
 
-        write_json(filename, text, indent=4)
+    write_json(filename, text, indent=4)
 
-        Args:
-            filename (str): file name of configuration
-            ajson (dict): dictionary
-            encoding (str): file encoding
-            indent (int): text indentation
+    Args:
+        filename (str): file name of configuration
+        ajson (dict): dictionary
+        encoding (str): file encoding
+        indent (int): text indentation
 
-        Returns:
-            None
+    Returns:
+        None
 
-        Raises:
-            IOError (): error in case function cannot write to filename
+    Raises:
+        IOError (): error in case function cannot write to filename
     """
-    write(filename, ajson, filetype='json', encoding=encoding, indent=indent)
+    write(filename, ajson, filetype="json", encoding=encoding, indent=indent)
 
 
-def flip(filename1, filename2):
-    """ Flips to files.
+def flip(filename1: str, filename2: str) -> None:
+    """Flips two files.
 
-        flip(filename1, filename2)
+    flip(filename1, filename2)
 
-        Args:
-            filename1 (str): file name of configuration
-            filename2 (str): file name of configuration
+    Args:
+        filename1 (str): file name of configuration
+        filename2 (str): file name of configuration
 
-        Returns:
-            None
+    Returns:
+        None
 
-        Raises:
-            IOError (): error in case function cannot write to filename
+    Raises:
+        IOError (): error in case function cannot write to filename
     """
-    filename0 = filename1 + '.tmp'
+    filename0 = filename1 + ".tmp"
     if os.path.isfile(filename1) and os.path.isfile(filename2):
         shutil.copy(filename1, filename0)
         shutil.copy(filename2, filename1)
         shutil.move(filename0, filename2)
-
```

### Comparing `boxfish-0.1.1/boxfish/utils/xpaths.py` & `boxfish-0.1.2/boxfish/utils/xpaths.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,141 @@
 # xpaths.py
 
 """Xpaths is a module that contains functions for working with xpaths
 """
 
+from typing import Tuple, Union
+
 from boxfish.utils.lists import to_list
 from boxfish.utils.strings import to_int
 
 
 # Xpath list functions
-def is_child(axpath, axpaths):
-    """ Returns true is axpath is a child from an item in axpaths
+def is_child(axpath: str, axpaths: Union[list, str]) -> bool:
+    """Returns true is axpath is a child from an item in axpaths
+
+    tf = is_child(axpath, axpaths)
 
-        tf = is_child(axpath, axpaths)
+    Args:
+        axpath(str): xpath
+        axpaths(str or list): xpath list
 
-        Args:
-            axpath(str): xpath
-            axpaths(str or list): xpath list
-
-        Returns:
-            tf (bool): true if axpath is a child of item in axpaths
-        """
+    Returns:
+        tf (bool): true if axpath is a child of item in axpaths
+    """
     axpaths = to_list(axpaths) if not isinstance(axpaths, list) else axpaths
     tf = False
     i = 0
     while not tf and i < len(axpaths):
         tf = _is_child(axpath, axpaths[i])
         i = i + 1
     return tf
 
 
-def is_descendant(axpath, axpaths):
-    """ Returns true is axpath is a descdendant from an item in axpaths
+def is_descendant(axpath: str, axpaths: Union[list, str]) -> bool:
+    """Returns true is axpath is a descdendant from an item in axpaths
 
-        tf = is_child(axpath, axpaths)
+    tf = is_child(axpath, axpaths)
 
-        Args:
-            axpath(str): xpath
-            axpaths(str or list): xpath list
-
-        Returns:
-            tf (bool): true if axpath is a descendant of item in axpaths
-        """
+    Args:
+        axpath(str): xpath
+        axpaths(str or list): xpath list
+
+    Returns:
+        tf (bool): true if axpath is a descendant of item in axpaths
+    """
     axpaths = to_list(axpaths) if not isinstance(axpaths, list) else axpaths
     tf = False
     i = 0
     while not tf and i < len(axpaths):
         tf = _is_descendant(axpath, axpaths[i])
         i = i + 1
     return tf
 
 
-def parent(axpath):
-    """ Returns xpath of parent of axpath
+def parent(axpath: str) -> str:
+    """Returns xpath of parent of axpath
 
-        pxpath = parent(axpath)
+    pxpath = parent(axpath)
 
-        Args:
-            axpath(str): xpath
+    Args:
+        axpath(str): xpath
 
-        Returns:
-            pxpath(str): xpath parent
-        """
-    sep  = '/'
-    stripped = axpath.split(sep,-1)
+    Returns:
+        pxpath(str): xpath parent
+    """
+    sep = "/"
+    stripped = axpath.split(sep, -1)
     return sep.join(stripped[:-1])
 
 
-def split(axpath):
-    """ Returns two lists with xpath name attributes and indices
+def split(axpath: str) -> Tuple[list, list]:
+    """Returns two lists with xpath name attributes and indices
 
     [anames aindices] = split(xpath)
 
     Args:
         axpath(str): Xpath
 
     Returns:
         anames (list): list with names
         aindices (list): list with indices
     """
-    anames = axpath.split('/')
+    anames = axpath.split("/")
     aindices = [1] * len(anames)
-    for i in range(len(anames)-1, -1, -1):
-        if anames[i] == '':
+    for i in range(len(anames) - 1, -1, -1):
+        if anames[i] == "":
             anames.pop(i)
             aindices.pop(i)
         else:
-            tlist = anames[i].replace('[', ']').split(sep=']')
+            tlist = anames[i].replace("[", "]").split(sep="]")
             anames[i] = tlist[0]
             if len(tlist) > 1:
                 index = to_int(tlist[1])
                 aindices[i] = index if index else 1
     return anames, aindices
 
 
 # Private functions
 
-def _is_child(axpath, bxpath):
-    """ Returns true if axpath is a child of bxpath
 
-     tf = _is_child(axpath, bxpath)
+def _is_child(axpath: str, bxpath: str) -> bool:
+    """Returns true if axpath is a child of bxpath
+
+    tf = _is_child(axpath, bxpath)
 
-     Args:
-         axpath(str): xpath
-         bxpath(str): xpath
-
-     Returns:
-         tf (bool): true if axpath is a child of bxpath
-     """
+    Args:
+        axpath(str): xpath
+        bxpath(str): xpath
+
+    Returns:
+        tf (bool): true if axpath is a child of bxpath
+    """
 
     [anames, aidx] = split(axpath)
     [bnames, bidx] = split(bxpath)
     tf = len(anames) == len(bnames) + 1
     if tf:
         tf = tf and anames[:-1] == bnames
         tf = tf and aidx[:-1] == bidx
     return tf
 
 
-def _is_descendant(axpath, bxpath):
-    """ Returns true if axpath is a descendant of bxpath
+def _is_descendant(axpath: str, bxpath: str) -> bool:
+    """Returns true if axpath is a descendant of bxpath
+
+    tf = _is_descendant(axpath, bxpath)
 
-     tf = _is_descendant(axpath, bxpath)
+    Args:
+        axpath(str): xpath
+        bxpath(str): xpath
 
-     Args:
-         axpath(str): xpath
-         bxpath(str): xpath
-
-     Returns:
-         tf (bool): true if axpath is a desdendant of bxpath
-     """
+    Returns:
+        tf (bool): true if axpath is a desdendant of bxpath
+    """
 
     [anames, aidx] = split(axpath)
     [bnames, bidx] = split(bxpath)
     levels = len(anames) - len(bnames)
     tf = levels >= 1
     if tf:
         tf = tf and anames[:-levels] == bnames
```

### Comparing `boxfish-0.1.1/boxfish.egg-info/PKG-INFO` & `boxfish-0.1.2/boxfish.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boxfish
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight tool for table extraction from HTML pages.
 Home-page: https://github.com/peterkorteweg/boxfish/
 Author: Peter Korteweg
 Author-email: boxfish@peterkorteweg.com
 License: MIT
 Keywords: beautifulsoup html pandas scraping tables
 Platform: UNKNOWN
@@ -24,15 +24,16 @@
 # boxfish: lightweight table extraction from HTML
 
 [![PyPI](https://img.shields.io/pypi/v/boxfish)](https://img.shields.io/pypi/v/boxfish)
 [![PyPI - Status](https://img.shields.io/pypi/status/boxfish)](https://img.shields.io/pypi/status/boxfish)
 [![PyPI - License](https://img.shields.io/pypi/l/boxfish)](https://img.shields.io/pypi/l/boxfish)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boxfish)](https://img.shields.io/pypi/pyversions/boxfish)
 
-[![GitHub top language](https://img.shields.io/github/languages/top/peterkorteweg/peterkorteweg)](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)
+[![GitHub top language](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)](https://img.shields.io/github/languages/top/peterkorteweg/boxfish)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ### What is it?
 Boxfish is a lightweight tool for table extraction from HTML pages. 
 
 ### Main features
 
 - Easy configuration. No knowledge of CSS or Xpaths required.
@@ -43,20 +44,20 @@
 
 
 ``` python
 import boxfish as bf
 import pandas as pd
 
 # Define table layout of an url with strings from two rows.
-aurl = ''
-row1 = ''
-row2 = ''
+aurl = ""
+row1 = ""
+row2 = ""
 
 # Build a configuration 
-aconfig = bf.build(url=aurl, astr = [row1, row2])
+aconfig = bf.build(url=aurl, rows = [row1, row2])
 
 # Extract a table
 data = bf.extract(aconfig, url=aurl)
 
 # View results
 df = pd.DataFrame(data)
 df.head()
```

### Comparing `boxfish-0.1.1/boxfish.egg-info/SOURCES.txt` & `boxfish-0.1.2/boxfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxfish-0.1.1/setup.py` & `boxfish-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pathlib
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of README and VERSION
 README = (HERE / "README.md").read_text()
 VERSION = (HERE / "boxfish/VERSION").read_text()
@@ -20,39 +21,33 @@
     author_email="boxfish@peterkorteweg.com",
     license="MIT",
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 3 - Alpha',
-
+        "Development Status :: 3 - Alpha",
         # Pick your license as you wish
         "License :: OSI Approved :: MIT License",
-
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
-    keywords='beautifulsoup html pandas scraping tables',
-
+    keywords="beautifulsoup html pandas scraping tables",
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
-    #package_dir={'': 'boxfish'},  # Required
+    # package_dir={'': 'boxfish'},  # Required
     packages=find_packages(),  # Required
-
-    package_data={'boxfish': ['VERSION']},
-
-    python_requires='>=3.6',
-
+    package_data={"boxfish": ["VERSION"]},
+    python_requires=">=3.6",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
-    install_requires=['requests','beautifulsoup4','selenium','lxml'],  # Optional
+    install_requires=["requests", "beautifulsoup4", "selenium", "lxml"],  # Optional
 )
```

