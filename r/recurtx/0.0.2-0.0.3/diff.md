# Comparing `tmp/recurtx-0.0.2.tar.gz` & `tmp/recurtx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recurtx-0.0.2.tar", last modified: Fri Jun 23 14:45:36 2023, max compression
+gzip compressed data, was "recurtx-0.0.3.tar", last modified: Sun Jun 25 15:37:14 2023, max compression
```

## Comparing `recurtx-0.0.2.tar` & `recurtx-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:45:36.000000 recurtx-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-20 00:32:16.000000 recurtx-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-23 14:45:36.000000 recurtx-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6039 2023-06-23 14:25:23.000000 recurtx-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-20 00:32:16.000000 recurtx-0.0.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:45:36.000000 recurtx-0.0.2/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-21 11:55:26.000000 recurtx-0.0.2/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-22 02:20:02.000000 recurtx-0.0.2/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-23 14:13:28.000000 recurtx-0.0.2/recurtx/find.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-23 14:15:10.000000 recurtx-0.0.2/recurtx/pandas.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-06-23 14:15:26.000000 recurtx-0.0.2/recurtx/polars.py
--rw-r--r--   0 root         (0) root         (0)     3343 2023-06-23 14:09:15.000000 recurtx-0.0.2/recurtx/recur.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-06-23 14:12:56.000000 recurtx-0.0.2/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-06-23 05:44:59.000000 recurtx-0.0.2/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:45:36.000000 recurtx-0.0.2/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-06-23 14:45:36.000000 recurtx-0.0.2/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-23 14:45:36.000000 recurtx-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1303 2023-06-20 00:32:16.000000 recurtx-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 15:37:14.530000 recurtx-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-20 00:32:16.000000 recurtx-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-25 15:37:14.530000 recurtx-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5715 2023-06-25 15:32:39.000000 recurtx-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-20 00:32:16.000000 recurtx-0.0.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 15:37:14.530000 recurtx-0.0.3/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-25 01:35:17.000000 recurtx-0.0.3/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-25 14:34:01.000000 recurtx-0.0.3/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6437 2023-06-25 09:06:46.000000 recurtx-0.0.3/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-06-25 09:08:00.000000 recurtx-0.0.3/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     3775 2023-06-25 11:34:26.000000 recurtx-0.0.3/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-06-25 12:35:43.000000 recurtx-0.0.3/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-25 11:35:32.000000 recurtx-0.0.3/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 15:37:14.530000 recurtx-0.0.3/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      252 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-25 15:37:14.000000 recurtx-0.0.3/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-25 15:37:14.530000 recurtx-0.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1562 2023-06-25 14:33:22.000000 recurtx-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `recurtx-0.0.2/LICENSE` & `recurtx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.2/PKG-INFO` & `recurtx-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.2/README.md` & `recurtx-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,43 +24,43 @@
 git clone https://github.com/Minyus/recurtx.git
 cd recurtx
 pip install -e .
 ```
 
 ## Wrapper Commands
 
-### recurtx under
+### xunder
 
 Run any scripts for each file under a directory recursively.
 
 #### Examples
 
 Run `wc -l {FILEPATH}` for each file under `directory_foo` recursively:
 
 ```
-recurtx under directory_foo "wc -l"
+xunder directory_foo "wc -l"
 ```
 
 Quoting for the script can be omitted for most cases. 
 
 ```
-recurtx under directory_foo wc -l
+xunder directory_foo wc -l
 ```
 
 Caveat: int, float, tuple, list, dict could be formatted unexpectedly (by `fire` package), for example:
 - ` 00 ` (recognized as int by Python) will be converted to ` 0 ` while ` "00" ` (recognized as str by Python) will be kept as is
 
 #### Description
 
 ```
 NAME
-    recurtx under
+    xunder
 
 SYNOPSIS
-    recurtx under PATH <flags> [SCRIPTS]...
+    xunder PATH <flags> [SCRIPTS]...
 
 POSITIONAL ARGUMENTS
     PATH
         Type: str
     SCRIPTS
         Type: str
 
@@ -78,34 +78,34 @@
         Type: bool
         Default: False
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
-### recurtx batch
+### xbatch
 
 Run any scripts for a batch of files in a directory recursively.
 
 #### Examples
 
 Concatenate all the contents in directory_foo.
 
 ```
-recurtx batch directory_foo cat
+xbatch directory_foo cat
 ```
 
 #### Description
 
 ```
 NAME
-    recurtx batch
+    xbatch
 
 SYNOPSIS
-    recurtx batch PATH <flags> [SCRIPTS]...
+    xbatch PATH <flags> [SCRIPTS]...
 
 POSITIONAL ARGUMENTS
     PATH
         Type: str
     SCRIPTS
         Type: str
 
@@ -125,40 +125,40 @@
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
 ## Commands to transform text files
 
-### recurtx search
+### xsearch
 
 Search a keyword, which may include wildcards, in the text file content, and optionally substitute (replace).
 
 #### Examples
 
 Search `keyword_bar` in each file under `directory_foo` recursively:
 
 ```
-recurtx under directory_foo recurtx search keyword_bar
+xunder directory_foo xsearch keyword_bar
 ```
 
 Search `keyword_bar` and substitute (replace) with `keyword_baz` in each file under `directory_foo` recursively:
 
 ```
-recurtx under directory_foo recurtx search keyword_bar --sub keyword_baz
+xunder directory_foo xsearch keyword_bar --sub keyword_baz
 ```
 
 #### Description
 
 ```
 NAME
-    recurtx search
+    xsearch
 
 SYNOPSIS
-    recurtx search TARGET PATH <flags>
+    xsearch TARGET PATH <flags>
 
 POSITIONAL ARGUMENTS
     TARGET
         Type: str
     PATH
         Type: str
 
@@ -173,40 +173,40 @@
         Type: int
         Default: 1
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
-### recurtx find
+### xfind
 
 Find a keyword, which may include wildcards, in the file path, and optionally substitute (replace).
 
 #### Examples
 
 Search `keyword_bar` in each file path under `directory_foo` recursively:
 
 ```
-recurtx under directory_foo recurtx find keyword_bar
+xunder directory_foo xfind keyword_bar
 ```
 
 Search `keyword_bar` and substitute (replace) with `keyword_baz` in each file path under `directory_foo` recursively:
 
 ```
-recurtx under directory_foo recurtx find keyword_bar --sub keyword_baz
+xunder directory_foo xfind keyword_bar --sub keyword_baz
 ```
 
 #### Description
 
 ```
 NAME
-    recurtx find
+    xfind
 
 SYNOPSIS
-    recurtx find TARGET PATH <flags>
+    xfind TARGET PATH <flags>
 
 POSITIONAL ARGUMENTS
     TARGET
         Type: str
     PATH
         Type: str
 
@@ -221,25 +221,15 @@
         Type: int
         Default: 1
 
 NOTES
     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
-### recurtx pandas
-
-Read and transform tabular files using pandas.
-
-#### Install dependency
-
-```
-pip install pandas
-```
-
-### recurtx pandas
+### xpandas
 
 Read and transform tabular data using pandas.
 
 Regarding options, see the documents for `pandas.read_xxx` such as:
 - [pandas.read_csv](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html)
 
 Data types supported by pandas (not all were tested):
@@ -271,18 +261,18 @@
 ```
 
 #### Examples
 
 Read files supported by pandas (such as csv and json) under directory_foo and concatenate:
 
 ```
-recurtx batch directory_foo recurtx pandas
+xbatch directory_foo xpandas
 ```
 
-### recurtx polars
+### xpolars
 
 Read and transform tabular data using polars.
 
 Regarding options, see the documents for `polars.scan_xxx` (or `polars.read_xxx` if scan function is not available), such as:
 - [polars.scan_csv](https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.scan_csv.html)
 
 Data types supported by polars (not all were tested):
@@ -303,13 +293,13 @@
 ```
 
 #### Examples
 
 Read files supported by polars (such as csv and json) under directory_foo and concatenate:
 
 ```
-recurtx batch directory_foo recurtx polars
+xbatch directory_foo xpolars
 ```
 
 ## Dependency to enable CLI
 
 - https://github.com/google/python-fire
```

### Comparing `recurtx-0.0.2/recurtx/pandas.py` & `recurtx-0.0.3/recurtx/pandas.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import sys
 from pathlib import Path
+from typing import List
+
+from .utils import infer_type, stdout_lines
 
 DATA_TYPES = {
     "pickle",
     "table",
     "csv",
     "fwf",
     "clipboard",
@@ -25,14 +28,16 @@
 }
 
 
 def pandas(
     *paths: str,
     package: str = "pandas",
     read_type: str = None,
+    columns: List[str] = None,
+    excluding_columns: List[str] = None,
     join: str = None,
     merge: str = None,
     on: str = None,
     left_on: str = None,
     right_on: str = None,
     left_index: bool = False,
     right_index: bool = False,
@@ -44,14 +49,15 @@
     lsuffix: str = None,
     rsuffix: str = None,
     query: str = None,
     head: int = None,
     tail: int = None,
     sample: int = None,
     method: str = None,
+    write_type: str = None,
     write_path: str = None,
     **kwargs,
 ):
     """Read and transform tabular files using pandas."""
 
     """Workaround for unexpected behavior of Fire"""
     kwargs.pop("package", None)
@@ -70,45 +76,57 @@
     kwargs.pop("lsuffix", "")
     kwargs.pop("rsuffix", "")
     kwargs.pop("query", None)
     kwargs.pop("head", None)
     kwargs.pop("tail", None)
     kwargs.pop("sample", None)
     kwargs.pop("method", None)
+    kwargs.pop("write_type", None)
     kwargs.pop("write_path", None)
 
-    if read_type is not None:
-        assert read_type in DATA_TYPES, (
-            str(read_type) + "not in the supported list: " + str(DATA_TYPES)
-        )
+    _write_type = (
+        infer_type(write_type, write_path, DATA_TYPES.union({"markdown"})) or "csv"
+    )
 
     if package == "modin":
         import modin.pandas as pd
     elif package == "pandas":
         import pandas as pd
     else:
         raise NotImplementedError(
             "'" + package + "' not supported. Set one of ['pandas', 'modin']"
         )
     import numpy as np
 
+    if columns and isinstance(columns, str):
+        columns = [columns]
+    if excluding_columns and isinstance(excluding_columns, str):
+        excluding_columns = [excluding_columns]
+
     ls = []
     for path in paths:
-        if read_type is None:
-            _read_type = path.split(".")[-1]
-        else:
-            _read_type = read_type
-        if _read_type not in DATA_TYPES:
+        _read_type = infer_type(read_type, path, DATA_TYPES)
+        if not _read_type:
             continue
         read_func = getattr(pd, "read_" + _read_type)
         _kwargs = kwargs.copy()
         if read_type == "csv":
             _kwargs.setdefault("dtype", str)
             _kwargs.setdefault("keep_default_na", False)
+            if columns:
+                _kwargs.setdefault("usecols", columns)
         df = read_func(path, **_kwargs)
+
+        if columns:
+            df = df[columns]
+        if excluding_columns:
+            _columns = df.columns
+            _columns = [c for c in _columns if c not in excluding_columns]
+            df = df[_columns]
+
         if query:
             df = df.query(query)
         ls.append(df)
 
     if not ls:
         return
     elif len(ls) == 1:
@@ -186,14 +204,32 @@
         df = eval("df." + method)
 
     if not isinstance(df, pd.DataFrame):
         text = "{}".format(df)
         if write_path:
             Path(write_path).write_text(text)
         else:
-            sys.stdout.write(text)
+            stdout_lines(text)
         return
 
+    _write_func = getattr(df, "to_" + _write_type)
+
+    def write_func(write_path: str = None, index=False):
+        nonlocal _write_func, df
+        try:
+            if _write_type == "json":
+                import json
+
+                ls = df.to_dict(orient="records")
+                if write_path:
+                    json.dump(ls, write_path)
+                else:
+                    return json.dumps(ls)
+            return _write_func(write_path, index=index)
+        except:
+            return _write_func(write_path)
+
     if write_path:
-        df.to_csv(write_path, index=False)
+        write_func(write_path, index=False)
     else:
-        sys.stdout.write(df.to_csv(index=False))
+        text = write_func(index=False)
+        stdout_lines(text)
```

### Comparing `recurtx-0.0.2/recurtx/polars.py` & `recurtx-0.0.3/recurtx/polars.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import sys
 from pathlib import Path
+from typing import List
+
+from .utils import infer_type, stdout_lines
 
 DATA_TYPES = {
     "csv",
     "ipc",
     "parquet",
     "database",
     "json",
@@ -26,69 +29,89 @@
     )
     return df
 
 
 def polars(
     *paths: str,
     read_type: str = None,
+    columns: List[str] = None,
+    excluding_columns: List[str] = None,
     streaming: str = None,  # actually bool
     fetch: int = None,
     join: str = None,
     on: str = None,
     left_on: str = None,
     right_on: str = None,
     suffix: str = "_right",
     validate: str = "m:m",
     head: int = None,
     tail: int = None,
     sample: int = None,
     method: str = None,
+    write_type: str = None,
     write_path: str = None,
     **kwargs,
 ):
     """Read and transform tabular files using polars."""
 
     """Workaround for unexpected behavior of Fire"""
+    kwargs.pop("read_type", None)
+    kwargs.pop("columns", None)
+    kwargs.pop("excluding_columns", None)
     kwargs.pop("streaming", None)
     kwargs.pop("fetch", None)
     kwargs.pop("join", None)
     kwargs.pop("on", None)
     kwargs.pop("left_on", None)
     kwargs.pop("right_on", None)
     kwargs.pop("suffix", "_right")
     kwargs.pop("validate", "m:m")
     kwargs.pop("head", None)
     kwargs.pop("tail", None)
     kwargs.pop("sample", None)
     kwargs.pop("method", None)
+    kwargs.pop("write_type", None)
     kwargs.pop("write_path", None)
 
-    streaming = streaming in {"", "True", "true", "T", "t", "1"}
+    _write_type = (
+        infer_type(write_type, write_path, DATA_TYPES.union({"markdown"}), polars=True)
+        or "csv"
+    )
 
-    if read_type is not None:
-        assert read_type in DATA_TYPES, (
-            str(read_type) + "not in the supported list: " + str(DATA_TYPES)
-        )
+    streaming = streaming in {"", "True", "true", "T", "t", "1"}
 
     import polars as pl
 
     ls = []
     for path in paths:
-        if read_type is None:
-            _read_type = path.split(".")[-1].replace("jsonl", "ndjson")
-        else:
-            _read_type = read_type
-        if _read_type not in DATA_TYPES:
+        _read_type = infer_type(read_type, path, DATA_TYPES, polars=True)
+        if not _read_type:
             continue
+
+        _kwargs = kwargs.copy()
+        if read_type == "csv":
+            _kwargs.setdefault("missing_utf8_is_empty_string", True)
+            _kwargs.setdefault("infer_schema_length", 0)
+
         read_func = getattr(pl, "scan_" + _read_type, None)
         if read_func is None:
             read_func = getattr(pl, "read_" + _read_type)
-            df = read_func(path, **kwargs).lazy()
+            df = read_func(path, **_kwargs).lazy()
         else:
-            df = read_func(path, **kwargs)
+            df = read_func(path, **_kwargs)
+
+        if columns:
+            df = df.select(columns)
+        if excluding_columns:
+            if isinstance(excluding_columns, str):
+                excluding_columns = [excluding_columns]
+            _columns = df.columns
+            _columns = [c for c in _columns if c not in excluding_columns]
+            df = df.select(_columns)
+
         ls.append(df)
 
     if not ls:
         return
     elif len(ls) == 1:
         df = ls[0]
     elif join is not None:
@@ -125,15 +148,30 @@
     df = activate(df, fetch, streaming)
 
     if not isinstance(df, pl.DataFrame):
         text = "{}".format(df)
         if write_path:
             Path(write_path).write_text(text)
         else:
-            sys.stdout.write(text)
+            stdout_lines(text)
         return
 
+    if _write_type == "markdown":
+
+        def write_func(write_path: str = None):
+            from io import StringIO
+
+            import pandas as pd
+
+            nonlocal df
+            csv_text = df.write_csv()
+            df = pd.read_csv(StringIO(csv_text), dtype=str, keep_default_na=False)
+            return df.to_markdown(write_path, index=False)
+
+    else:
+        write_func = getattr(df, "write_" + _write_type)
+
     if write_path:
-        df.write_csv(write_path)
+        write_func(write_path)
     else:
-        sys.stdout.write(df.write_csv())
-    return
+        text = write_func()
+        stdout_lines(text)
```

### Comparing `recurtx-0.0.2/recurtx/recur.py` & `recurtx-0.0.3/recurtx/recur.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,35 @@
+import re
 import sys
 from pathlib import Path
 
 from .utils import get_exception_msg, subprocess_run, upath
 
 
 def recur(
     kind: str,
     path: str,
     *scripts: str,
     **kwargs: str,
 ):
     glob = kwargs.pop("glob", "**/*")
+    regex = kwargs.pop(
+        "regex",
+        r"^(?!.*(\.git\/|__pycache__\/|\.ipynb_checkpoints\/|\.pytest_cache\/|\.vscode\/|\.idea\/|\.DS_Store)).*$",
+    )
     reverse = kwargs.pop("reverse", False)
     replace_str = kwargs.pop("replace_str", "@@")
     show_paths = kwargs.pop("show_paths", False)
     show_scripts = kwargs.pop("show_scripts", False)
 
+    if regex:
+        rx = re.compile(regex)
+    else:
+        rx = None
+
     scripts = list(scripts)
     if len(kwargs) and len(scripts) == 1:
         scripts = scripts[0].split(" ")
     for k, v in kwargs.items():
         if isinstance(v, bool) and v == False:
             continue
         if len(k) >= 2:
@@ -44,27 +54,33 @@
     path = Path(upath(path))
     assert path.exists(), str(path.resolve()) + " does not exist."
 
     if path.is_file():
         path_ls = [str(path)]
     else:
         path_ls = [str(p) for p in path.glob(glob) if p.is_file()]
+        if rx:
+            path_ls = [p for p in path_ls if rx.match(p)]
         path_ls.sort(reverse=reverse)
+
     if show_paths:
         sys.stdout.write(
             "[Searching files]\n" + str("\n".join(["    " + p for p in path_ls]) + "\n")
         )
 
     running_scripts = scripts
     if kind == "under":
         for p in path_ls:
             try:
                 if replace_str:
                     running_scripts = [
-                        script.replace(replace_str, p) for script in scripts
+                        script.replace(replace_str, p)
+                        if isinstance(script, str)
+                        else script
+                        for script in scripts
                     ]
                 if len(running_scripts) == 1:
                     running_scripts = running_scripts[0]
                 subprocess_run(running_scripts, show_scripts)
             except Exception:
                 msg = get_exception_msg()
                 sys.stdout.write(msg)
```

### Comparing `recurtx-0.0.2/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.3/recurtx.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

