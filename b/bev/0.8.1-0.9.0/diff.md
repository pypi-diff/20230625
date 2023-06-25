# Comparing `tmp/bev-0.8.1.tar.gz` & `tmp/bev-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bev-0.8.1.tar", last modified: Tue Jun 20 16:08:58 2023, max compression
+gzip compressed data, was "bev-0.9.0.tar", last modified: Sun Jun 25 00:28:14 2023, max compression
```

## Comparing `bev-0.8.1.tar` & `bev-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-20 16:08:52.000000 bev-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-20 16:08:52.000000 bev-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 16:08:58.763427 bev-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-20 16:08:52.000000 bev-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 16:08:52.000000 bev-0.8.1/bev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 16:08:52.000000 bev-0.8.1/bev/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/blame.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-20 16:08:52.000000 bev-0.8.1/bev/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev/config/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-20 16:08:52.000000 bev-0.8.1/bev/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 16:08:52.000000 bev-0.8.1/bev/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-20 16:08:52.000000 bev-0.8.1/bev/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 16:08:52.000000 bev-0.8.1/bev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-20 16:08:52.000000 bev-0.8.1/bev/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-06-20 16:08:52.000000 bev-0.8.1/bev/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 16:08:52.000000 bev-0.8.1/bev/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-20 16:08:52.000000 bev-0.8.1/bev/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:52.000000 bev-0.8.1/bev/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-20 16:08:52.000000 bev-0.8.1/bev/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-20 16:08:52.000000 bev-0.8.1/bev/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-20 16:08:52.000000 bev-0.8.1/bev/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-20 16:08:52.000000 bev-0.8.1/bev/vc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-20 16:08:52.000000 bev-0.8.1/bev/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:58.763427 bev-0.8.1/bev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 16:08:58.000000 bev-0.8.1/bev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-20 16:08:52.000000 bev-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 16:08:52.000000 bev-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:08:58.763427 bev-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 16:08:52.000000 bev-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:14.977631 bev-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-25 00:28:11.000000 bev-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-25 00:28:11.000000 bev-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-06-25 00:28:14.977631 bev-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-25 00:28:11.000000 bev-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:14.977631 bev-0.9.0/bev/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-25 00:28:11.000000 bev-0.9.0/bev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 00:28:11.000000 bev-0.9.0/bev/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:14.977631 bev-0.9.0/bev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/blame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-25 00:28:11.000000 bev-0.9.0/bev/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:14.977631 bev-0.9.0/bev/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-25 00:28:11.000000 bev-0.9.0/bev/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-25 00:28:11.000000 bev-0.9.0/bev/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-25 00:28:11.000000 bev-0.9.0/bev/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-25 00:28:11.000000 bev-0.9.0/bev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-25 00:28:11.000000 bev-0.9.0/bev/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-25 00:28:11.000000 bev-0.9.0/bev/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 00:28:11.000000 bev-0.9.0/bev/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-25 00:28:11.000000 bev-0.9.0/bev/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:11.000000 bev-0.9.0/bev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 00:28:11.000000 bev-0.9.0/bev/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-25 00:28:11.000000 bev-0.9.0/bev/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-25 00:28:11.000000 bev-0.9.0/bev/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-25 00:28:11.000000 bev-0.9.0/bev/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-25 00:28:11.000000 bev-0.9.0/bev/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 00:28:14.977631 bev-0.9.0/bev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-06-25 00:28:14.000000 bev-0.9.0/bev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-25 00:28:14.000000 bev-0.9.0/bev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 00:28:14.000000 bev-0.9.0/bev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 00:28:14.000000 bev-0.9.0/bev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 00:28:14.000000 bev-0.9.0/bev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-25 00:28:14.000000 bev-0.9.0/bev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-25 00:28:11.000000 bev-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-25 00:28:11.000000 bev-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 00:28:14.977631 bev-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-25 00:28:11.000000 bev-0.9.0/setup.py
```

### Comparing `bev-0.8.1/LICENSE` & `bev-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/README.md` & `bev-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/add.py` & `bev-0.9.0/bev/cli/add.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/app.py` & `bev-0.9.0/bev/cli/app.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/blame.py` & `bev-0.9.0/bev/cli/blame.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/fetch.py` & `bev-0.9.0/bev/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/pull.py` & `bev-0.9.0/bev/cli/pull.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/storage.py` & `bev-0.9.0/bev/cli/storage.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/update.py` & `bev-0.9.0/bev/cli/update.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/cli/utils.py` & `bev-0.9.0/bev/cli/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/config/hostname.py` & `bev-0.9.0/bev/config/hostname.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if isinstance(v, str):
             return StrHostName(v)
 
         assert isinstance(v, dict), f'Not a dict: {v}'
         assert len(v) == 1, v
         (k, v), = v.items()
 
-        return find(HostName, k)(v)
+        return find(k, HostName)(v)
 
 
 @register('str')
 class StrHostName(HostName):
     def match(self, name) -> bool:
         return name == self.value
```

### Comparing `bev-0.8.1/bev/config/include.py` & `bev-0.9.0/bev/config/include.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             return v
 
         assert isinstance(v, dict), f'Not a dict: {v}'
         optional = v.pop('optional', False)
         assert len(v) == 1, v
         (k, v), = v.items()
 
-        return find(Include, k)(v, optional)
+        return find(k, Include)(v, optional)
 
 
 @register('file')
 class FileInclude(Include):
     def __init__(self, value, optional):
         super().__init__(Path(value).expanduser(), optional)
```

### Comparing `bev-0.8.1/bev/config/parse.py` & `bev-0.9.0/bev/config/parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,64 @@
 import importlib
 from pathlib import Path
-from typing import Callable, NamedTuple, Sequence, Tuple
+from typing import Callable, ContextManager, NamedTuple, Sequence, Tuple, Union
 
-from tarn import DiskDict, HashKeyStorage, Location
+from jboc import collect
+from tarn import HashKeyStorage, Location, Writable
 from yaml import safe_load
+from tarn.interface import Key, MaybeLabels, Value
 
 from ..exceptions import ConfigError
-from .base import ConfigMeta, RepositoryConfig, StorageCluster, StorageLevelConfig
-from .utils import CONFIG, _filter_levels, choose_local, default_choose, identity, wrap_levels
+from .base import ConfigMeta, RepositoryConfig, StorageCluster
+from .utils import CONFIG, choose_local, default_choose
 
 
 class CacheStorageIndex(NamedTuple):
-    local: Sequence[StorageLevelConfig]
+    local: Location
     remote: Sequence[Location]
     storage: HashKeyStorage
 
 
 def load_config(config: Path) -> RepositoryConfig:
     with open(config, 'r') as file:
         return parse(Path(config), safe_load(file))
 
 
 def build_storage(root: Path) -> Tuple[HashKeyStorage, CacheStorageIndex]:
     config = load_config(root / CONFIG)
     meta = config.meta
 
-    order_func: Callable[[Sequence[Location]], Sequence[Location]] = identity
-    if meta.order is not None:
-        path, attr = meta.order.rsplit('.', 1)
-        order_func = getattr(importlib.import_module(path), attr)
-
     storage = HashKeyStorage(
-        wrap_levels(config.local.storage, DiskDict, order_func),
+        config.local.storage.local.build(),
         remote=filter_remotes([remote.storage for remote in config.remotes]),
         labels=meta.labels,
     )
     index = None
     if config.local.cache is not None:
         cache_storage = HashKeyStorage(
-            wrap_levels(config.local.cache.storage, DiskDict, order_func),
+            config.local.cache.storage.local.build(),
             remote=filter_remotes([remote.cache.storage for remote in config.remotes if remote.cache is not None]),
             labels=meta.labels,
         )
         index = CacheStorageIndex(
-            tuple(_filter_levels(config.local.cache.index)),
+            GetItemPatch(config.local.cache.index.local.build()),
             filter_remotes([remote.cache.index for remote in config.remotes if remote.cache is not None]),
             cache_storage,
         )
     return storage, index
 
 
+@collect
 def filter_remotes(entries):
-    remotes = []
     for entry in entries:
-        for level in entry:
-            for location in level.locations:
-                for remote in location.remote:
-                    remote = remote.build(location.root, location.optional)
-                    if remote is not None:
-                        remotes.append(remote)
-
-    return remotes
+        # TODO: add a test for a None remote
+        if entry.remote is not None:
+            entry = entry.remote.build()
+            if entry is not None:
+                yield entry
 
 
 def parse(root, config) -> RepositoryConfig:
     meta, entries = _parse(root, config, root)
 
     filter_func: Callable[[StorageCluster], bool] = default_choose
     if meta.choose is not None:
@@ -80,32 +74,36 @@
             raise ConfigError(f'No matching entry in config {root}')
         local = entries.pop(name)
         remotes = tuple(entries.values())
 
     return RepositoryConfig(local=local, remotes=remotes, meta=meta)
 
 
+def _parse_entry(name, entry):
+    if isinstance(entry, str):
+        entry = {'storage': entry}
+    if not isinstance(entry, dict):
+        raise ConfigError(f'{name}: Each config entry must be either a dict or a string')
+    if 'name' in entry:
+        raise ConfigError(f'{name}: The key "name" is not available')
+    entry = entry.copy()
+    entry['name'] = name
+    return StorageCluster(**entry)
+
+
 def _parse(name, config, root):
     if not isinstance(config, dict):
         raise ConfigError(f'{name}: The config must be a dict')
 
     config = config.copy()
     meta = ConfigMeta.parse_obj(config.pop('meta', {}))
     # parse own items
     entries = {}
     for name, entry in config.items():
-        if isinstance(entry, str):
-            entry = {'storage': entry}
-        if not isinstance(entry, dict):
-            raise ConfigError(f'{name}: Each config entry must be either a dict or a string')
-        if 'name' in entry:
-            raise ConfigError(f'{name}: The key "name" is not available')
-        entry = entry.copy()
-        entry['name'] = name
-        entries[name] = StorageCluster(**entry)
+        entries[name] = _parse_entry(name, entry)
 
     # parse parents
     override = {}
     for parent in meta.include:
         parent_root, parent_config = parent.read(root)
         if parent_config is None:
             if parent.optional:
@@ -128,7 +126,35 @@
                 f'{meta.hash} vs {parent_meta.hash}'
             )
 
         entries.update(items)
 
     meta = meta.copy(update=override)
     return meta, entries
+
+
+class GetItemPatch(Writable):
+    def __init__(self, location):
+        self.location = location
+        self.locations = [location]
+
+    def __getattr__(self, attr):
+        return getattr(self.location, attr)
+
+    def __getitem__(self, item):
+        assert item == 0
+        return self
+
+    def read(self, *args, **kwargs):
+        return self.location.read(*args, **kwargs)
+    
+    def read_batch(self, *args, **kwargs):
+        return self.location.read_batch(*args, **kwargs)
+    
+    def write(self, *args, **kwargs):
+        return self.location.write(*args, **kwargs)
+    
+    def delete(self, *args, **kwargs):
+        return self.location.delete(*args, **kwargs)
+
+    def contents(self, *args, **kwargs):
+        return self.location.contents(*args, **kwargs)
```

### Comparing `bev-0.8.1/bev/hash.py` & `bev-0.9.0/bev/hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import tempfile
 from collections import OrderedDict
 from pathlib import Path
 from typing import Dict, NamedTuple, Union
 
 from tarn import HashKeyStorage
+from tarn.utils import value_to_buffer
 
 from .exceptions import HashError
 from .utils import PathOrStr, deprecate
 
 Key = str
 Tree = Dict[PathOrStr, Union[Key, Dict]]
 HashType = Union[Key, Tree]
@@ -39,16 +40,16 @@
 
 def load_key(path: PathOrStr):
     with open(path, 'r') as file:
         return file.read().strip()
 
 
 def load_tree(path: Path):
-    with open(path, 'r') as file:
-        return json.load(file)
+    with value_to_buffer(path) as buffer:
+        return json.load(buffer)
 
 
 def strip_tree(key):
     if key.startswith('T:'):
         key = key[2:]
     return key
```

### Comparing `bev-0.8.1/bev/interface.py` & `bev-0.9.0/bev/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .exceptions import HashNotFound, InconsistentHash, InconsistentRepositories, NameConflict, RepositoryNotFound
 from .hash import Key, is_hash, is_tree, load_key, load_tree, strip_tree, to_hash
 from .local import Local
 from .utils import PathOrStr
 from .vc import VC, CommittedVersion, SubprocessGit, Version
 from .wc import BevLocalGlob, BevVCGlob
 
-
 _NoArg = object()
 
 
 class Repository:
     """
     Interface that represents a `bev` repository.
```

### Comparing `bev-0.8.1/bev/ops.py` & `bev-0.9.0/bev/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 from tarn import HashKeyStorage
 
-from .config import identity
+from .config.utils import identity
 from .hash import HashType, from_hash, is_hash, is_tree, load_key, load_tree, normalize_tree, strip_tree, tree_to_hash
 from .interface import Repository
 from .utils import PathOrStr
 
 
 class Conflict(Enum):
     """
```

### Comparing `bev-0.8.1/bev/shortcuts.py` & `bev-0.9.0/bev/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/testing.py` & `bev-0.9.0/bev/testing.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/utils.py` & `bev-0.9.0/bev/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/vc.py` & `bev-0.9.0/bev/vc.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev/wc.py` & `bev-0.9.0/bev/wc.py`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/bev.egg-info/SOURCES.txt` & `bev-0.9.0/bev.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 bev/cli/storage.py
 bev/cli/update.py
 bev/cli/utils.py
 bev/config/__init__.py
 bev/config/base.py
 bev/config/hostname.py
 bev/config/include.py
+bev/config/location.py
 bev/config/parse.py
 bev/config/registry.py
 bev/config/remote.py
 bev/config/utils.py
```

### Comparing `bev-0.8.1/pyproject.toml` & `bev-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bev-0.8.1/setup.py` & `bev-0.9.0/setup.py`

 * *Files identical despite different names*

