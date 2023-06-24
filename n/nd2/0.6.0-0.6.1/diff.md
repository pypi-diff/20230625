# Comparing `tmp/nd2-0.6.0.tar.gz` & `tmp/nd2-0.6.1.tar.gz`

## Comparing `nd2-0.6.0.tar` & `nd2-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.6.0/.github_changelog_generator
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 nd2-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    16851 2020-02-02 00:00:00.000000 nd2-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.6.0/.github/workflows/cron.yml
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/bf_describe.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/compare.py
--rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/comparison.json
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/download_samples.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/gather.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nd2-0.6.0/scripts/nd2_describe.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_binary.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_clx_lite.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_clx_xml.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_version.py
--rw-r--r--   0        0        0    29445 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/nd2file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/py.typed
--rw-r--r--   0        0        0    12135 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/structures.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_legacy/__init__.py
--rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_legacy/_legacy.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_legacy/_legacy_xml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/__init__.py
--rw-r--r--   0        0        0    14676 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_chunk_decode.py
--rw-r--r--   0        0        0    22012 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_parse.py
--rw-r--r--   0        0        0    18816 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_pysdk.py
--rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 nd2-0.6.0/src/nd2/_pysdk/_sdk_types.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/readlim_output.json
--rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/samples_metadata.json
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_aicsimage.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_binary.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_dask_dispatch.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_deprecations.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_metadata.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_parse.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_reader.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_readme.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_rescue.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_rois.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_segfaults.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/test_xml.py
--rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/variant.xml
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.6.0/tests/variant_CustomDataV2_0.xml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.6.0/.gitignore
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.6.0/LICENSE
--rw-r--r--   0        0        0    30192 2020-02-02 00:00:00.000000 nd2-0.6.0/README.md
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 nd2-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    32443 2020-02-02 00:00:00.000000 nd2-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.6.1/.github_changelog_generator
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 nd2-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17666 2020-02-02 00:00:00.000000 nd2-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.6.1/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/bf_describe.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/compare.py
+-rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/comparison.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/download_samples.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/gather.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nd2-0.6.1/scripts/nd2_describe.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_binary.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_clx_lite.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_clx_xml.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_version.py
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/index.py
+-rw-r--r--   0        0        0    33458 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/nd2file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/py.typed
+-rw-r--r--   0        0        0    13163 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/structures.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_legacy/__init__.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_legacy/_legacy.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_legacy/_legacy_xml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/__init__.py
+-rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_chunk_decode.py
+-rw-r--r--   0        0        0    24874 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_parse.py
+-rw-r--r--   0        0        0    21321 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_pysdk.py
+-rw-r--r--   0        0        0    19912 2020-02-02 00:00:00.000000 nd2-0.6.1/src/nd2/_pysdk/_sdk_types.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/readlim_output.json
+-rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/samples_metadata.json
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_aicsimage.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_binary.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_dask_dispatch.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_deprecations.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_index.py
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_metadata.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_parse.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_reader.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_readme.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_rescue.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_rois.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_segfaults.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/test_xml.py
+-rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/variant.xml
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.6.1/tests/variant_CustomDataV2_0.xml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.6.1/LICENSE
+-rw-r--r--   0        0        0    32117 2020-02-02 00:00:00.000000 nd2-0.6.1/README.md
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 nd2-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    34241 2020-02-02 00:00:00.000000 nd2-0.6.1/PKG-INFO
```

### Comparing `nd2-0.6.0/.pre-commit-config.yaml` & `nd2-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/CHANGELOG.md` & `nd2-0.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 # Changelog
 
-## [0.6.0](https://github.com/tlambert03/nd2/tree/0.6.0) (2023-06-15)
+## [v0.6.1](https://github.com/tlambert03/nd2/tree/v0.6.1) (2023-06-24)
 
-[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.5.3...0.6.0)
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.6.0...v0.6.1)
+
+**Implemented enhancements:**
+
+- feat: support files with custom experiment loops [\#148](https://github.com/tlambert03/nd2/pull/148) ([tlambert03](https://github.com/tlambert03))
+- feat: add `python -m nd2.index` cli [\#147](https://github.com/tlambert03/nd2/pull/147) ([tlambert03](https://github.com/tlambert03))
+- feat: big update to events parsing.  add .events method, deprecate recorded\_date [\#144](https://github.com/tlambert03/nd2/pull/144) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- build: remove wurlitzer from build [\#142](https://github.com/tlambert03/nd2/pull/142) ([tlambert03](https://github.com/tlambert03))
+
+## [v0.6.0](https://github.com/tlambert03/nd2/tree/v0.6.0) (2023-06-15)
+
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.5.3...v0.6.0)
 
 **Implemented enhancements:**
 
 - feat: Remove sdk, use all python [\#135](https://github.com/tlambert03/nd2/pull/135) ([tlambert03](https://github.com/tlambert03))
 
 **Fixed bugs:**
```

### Comparing `nd2-0.6.0/.github/workflows/ci.yml` & `nd2-0.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/.github/workflows/cron.yml` & `nd2-0.6.1/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/scripts/bf_describe.py` & `nd2-0.6.1/scripts/bf_describe.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/scripts/compare.py` & `nd2-0.6.1/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/scripts/comparison.json` & `nd2-0.6.1/scripts/comparison.json`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/scripts/gather.py` & `nd2-0.6.1/scripts/gather.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/scripts/nd2_describe.py` & `nd2-0.6.1/scripts/nd2_describe.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,19 +27,23 @@
     raise RuntimeError("Not an ND2 file")
 
 
 def get_nd2_stats(path: Path) -> "tuple[str, dict]":
     data = {"ver": _get_version(path)}
 
     with nd2.ND2File(path) as nd:
+        meta = nd.metadata if isinstance(nd.metadata, dict) else asdict(nd.metadata)
+        for channel in meta.get("channels", []):
+            # Remove custom loops if null... they're super rare, and
+            # readlimfile.json doesn't include them
+            if channel.get("loops") and not channel["loops"].get("CustomLoop"):
+                channel["loops"].pop("CustomLoop", None)
         data["attributes"] = nd.attributes._asdict()
         data["experiment"] = [asdict(x) for x in nd.experiment]
-        data["metadata"] = (
-            nd.metadata if isinstance(nd.metadata, dict) else asdict(nd.metadata)
-        )
+        data["metadata"] = meta
         data["textinfo"] = nd.text_info
 
     return path.name, data
 
 
 if __name__ == "__main__":
     import json
```

### Comparing `nd2-0.6.0/src/nd2/__init__.py` & `nd2-0.6.1/src/nd2/__init__.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/src/nd2/_binary.py` & `nd2-0.6.1/src/nd2/_binary.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/src/nd2/_clx_lite.py` & `nd2-0.6.1/src/nd2/_clx_lite.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/src/nd2/_clx_xml.py` & `nd2-0.6.1/src/nd2/_clx_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,18 @@
     if bxml.startswith(b"<?xml"):
         bxml = bxml.split(b"?>", 1)[-1]  # strip xml header
 
     try:
         node = parser(bxml)
     except SyntaxError:  # when there are invalid characters in the XML
         # could go straight to this ... not sure if it's slower
-        node = parser(bxml.decode(encoding="utf-8", errors="ignore"))
+        try:
+            node = parser(bxml.decode(encoding="utf-8", errors="ignore"))
+        except Exception:
+            node = parser(bxml.decode(encoding="utf-16", errors="ignore"))
 
     is_legacy = node.attrib.get("_VERSION") == "1.000000"
     name, val = _node_name_value(node, strip_prefix, include_attrs=is_legacy)
 
     # the special case of a single <variant><no_name>...</no_name></variant>
     # this is mostly here for Attributes, Experiment, Metadata, and TextInfo
     # LIM handles these special cases in JsonMetadata::composeRawMetadata
```

### Comparing `nd2-0.6.0/src/nd2/nd2file.py` & `nd2-0.6.1/src/nd2/nd2file.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 import warnings
 from itertools import product
 from pathlib import Path
 from typing import TYPE_CHECKING, cast, overload
 
 import numpy as np
 
-from ._pysdk._chunk_decode import ND2_FILE_SIGNATURE
-from ._util import AXIS, VoxelSize, get_reader, is_supported_file
+from nd2 import _util
+
+from ._pysdk._chunk_decode import ND2_FILE_SIGNATURE, get_version
+from ._util import AXIS, TIME_KEY, is_supported_file
 from .structures import ROI
 
 try:
     from functools import cached_property
 except ImportError:
     cached_property = property  # type: ignore
 
@@ -24,15 +26,15 @@
 
     import dask.array.core
     import xarray as xr
     from typing_extensions import Literal
 
     from ._binary import BinaryLayers
     from ._pysdk._pysdk import ND2Reader as LatestSDKReader
-    from ._util import StrOrBytesPath
+    from ._util import DictOfDicts, DictOfLists, ListOfDicts, StrOrBytesPath
     from .structures import (
         Attributes,
         ExpLoop,
         FrameMetadata,
         Metadata,
         TextInfo,
         XYPosLoop,
@@ -79,29 +81,41 @@
             warnings.warn(
                 "The `read_using_sdk` argument is deprecated and will be removed in "
                 "a future version.",
                 FutureWarning,
                 stacklevel=2,
             )
         self._path = str(path)
-        self._rdr = get_reader(
+        self._rdr = _util.get_reader(
             self._path,
             validate_frames=validate_frames,
             search_window=search_window,
         )
         self._closed = False
         self._is_legacy = "Legacy" in type(self._rdr).__name__
         self._lock = threading.RLock()
+        self._version: tuple[int, ...] | None = None
 
     @staticmethod
     def is_supported_file(path: StrOrBytesPath) -> bool:
         """Return True if the file is supported by this reader."""
         return is_supported_file(path)
 
     @property
+    def version(self) -> tuple[int, ...]:
+        """Return the file format version as a tuple of ints."""
+        if self._version is None:
+            try:
+                self._version = get_version(self._rdr._fh or self._rdr._path)
+            except Exception:
+                self._version = (-1, -1)
+                raise
+        return self._version
+
+    @property
     def path(self) -> str:
         """Path of the image."""
         return self._path
 
     @property
     def is_legacy(self) -> bool:
         """Whether file is a legacy nd2 (JPEG2000) file."""
@@ -150,15 +164,15 @@
         del state["_lock"]
         return state
 
     def __setstate__(self, d: dict[str, Any]) -> None:
         """Load state from pickling."""
         self.__dict__ = d
         self._lock = threading.RLock()
-        self._rdr = get_reader(self._path)
+        self._rdr = _util.get_reader(self._path)
         if self._closed:
             self._rdr.close()
 
     @cached_property
     def attributes(self) -> Attributes:
         """Core image attributes."""
         return self._rdr.attributes
@@ -185,14 +199,97 @@
         return {r.id: r for r in _rois}
 
     @cached_property
     def experiment(self) -> list[ExpLoop]:
         """Loop information for each nd axis."""
         return self._rdr.experiment()
 
+    @overload
+    def events(
+        self, *, orient: Literal["records"] = ..., null_value: Any = ...
+    ) -> ListOfDicts:
+        ...
+
+    @overload
+    def events(self, *, orient: Literal["list"], null_value: Any = ...) -> DictOfLists:
+        ...
+
+    @overload
+    def events(self, *, orient: Literal["dict"], null_value: Any = ...) -> DictOfDicts:
+        ...
+
+    def events(
+        self,
+        *,
+        orient: Literal["records", "list", "dict"] = "records",
+        null_value: Any = float("nan"),
+    ) -> ListOfDicts | DictOfLists | DictOfDicts:
+        """Return tabular data recorded for each frame and/or event of the experiment.
+
+        This method returns tabular data in the format specified by the `orient`
+        argument:
+            - 'records' : list of dict - `[{column -> value}, ...]` (default)
+            - 'dict' :    dict of dict - `{column -> {index -> value}, ...}`
+            - 'list' :    dict of list - `{column -> [value, ...]}`
+
+        All return types are passable to pd.DataFrame(). It matches the tabular data
+        reported in the Image Properties > Recorded Data tab of the NIS Viewer.
+
+        There will be a column for each tag in the `CustomDataV2_0` section of
+        `ND2File.custom_data`, as well columns for any events recorded in the
+        data.  Not all cells will be populated, and empty cells will be filled
+        with `null_value` (default `float('nan')`).
+
+        Legacy ND2 files are not supported.
+
+        Parameters
+        ----------
+        orient : {'records', 'dict', 'list'}, default 'records'
+            The format of the returned data. See `pandas.DataFrame
+                - 'records' : list of dict - `[{column -> value}, ...]` (default)
+                - 'dict' :    dict of dict - `{column -> {index -> value}, ...}`
+                - 'list' :    dict of list - `{column -> [value, ...]}`
+        null_value : Any, default float('nan')
+            The value to use for missing data.
+        """
+        if orient not in ("records", "dict", "list"):  # pragma: no cover
+            raise ValueError("orient must be one of 'records', 'dict', or 'list'")
+
+        if self.is_legacy:  # pragma: no cover
+            warnings.warn(
+                "`recorded_data` is not implemented for legacy ND2 files",
+                UserWarning,
+                stacklevel=2,
+            )
+            return [] if orient == "records" else {}  # type: ignore[return-value]
+
+        rdr = cast("LatestSDKReader", self._rdr)
+        acq_data = rdr._acquisition_data()  # comes back as a dict of lists
+        acq_data.update(rdr._custom_tags())
+
+        img_events = rdr._img_exp_events()
+        if not img_events and orient == "list":
+            # by default, acq_data is already oriented as a dict of lists,
+            # so if we don't have any image events, we can just return it
+            return acq_data
+
+        # re-orient acq_data as a list of dicts, to combine with events
+        records = _util.convert_dict_of_lists_to_records(acq_data)
+        for e in img_events:
+            records.append({TIME_KEY: e.time / 1000, "Events": e.description})
+
+        # sort by time
+        records.sort(key=lambda x: x.get(TIME_KEY, 0))
+
+        if orient == "dict":
+            return _util.convert_records_to_dict_of_dicts(records, null_val=null_value)
+        elif orient == "list":
+            return _util.convert_records_to_dict_of_lists(records, null_val=null_value)
+        return records
+
     def unstructured_metadata(
         self,
         *,
         strip_prefix: bool = True,
         include: set[str] | None = None,
         exclude: set[str] | None = None,
         unnest: bool | None = None,
@@ -356,28 +453,28 @@
     @cached_property
     def dtype(self) -> np.dtype:
         """Image data type."""
         attrs = self.attributes
         d = attrs.pixelDataType[0] if attrs.pixelDataType else "u"
         return np.dtype(f"{d}{attrs.bitsPerComponentInMemory // 8}")
 
-    def voxel_size(self, channel: int = 0) -> VoxelSize:
+    def voxel_size(self, channel: int = 0) -> _util.VoxelSize:
         """XYZ voxel size.
 
         Parameters
         ----------
         channel : int
             Channel for which to retrieve voxel info, by default 0
 
         Returns
         -------
         VoxelSize
             Named tuple with attrs `x`, `y`, and `z`.
         """
-        return VoxelSize(*self._rdr.voxel_size())
+        return _util.VoxelSize(*self._rdr.voxel_size())
 
     def asarray(self, position: int | None = None) -> np.ndarray:
         """Read image into numpy array.
 
         Parameters
         ----------
         position : int, optional
@@ -679,35 +776,38 @@
         try:
             details = " (closed)" if self.closed else f" {self.dtype}: {self.sizes!r}"
             extra = f": {Path(self.path).name!r}{details}"
         except Exception:
             extra = ""
         return f"<ND2File at {hex(id(self))}{extra}>"
 
-    @cached_property
-    def recorded_data(self) -> dict[str, np.ndarray | Sequence]:
+    @property
+    def recorded_data(
+        self,
+    ) -> DictOfLists:
         """Return tabular data recorded for each frame of the experiment.
 
         This method returns a dict of equal-length sequences (passable to
         pd.DataFrame()). It matches the tabular data reported in the Image Properties >
         Recorded Data tab of the NIS Viewer.
 
         (There will be a column for each tag in the `CustomDataV2_0` section of
         `ND2File.custom_data`)
 
         Legacy ND2 files are not supported.
         """
-        if self.is_legacy:  # pragma: no cover
-            warnings.warn(
-                "`recorded_data` is not supported for legacy ND2 files",
-                UserWarning,
-                stacklevel=2,
-            )
-            return {}
-        return cast("LatestSDKReader", self._rdr).recorded_data()
+        warnings.warn(
+            "recorded_data is deprecated and will be removed in a future version."
+            "Please use the `events` method instead. To get the same dict-of-lists "
+            "output, use `events(orient='list')`",
+            FutureWarning,
+            stacklevel=2,
+        )
+
+        return self.events(orient="list")
 
     @cached_property
     def binary_data(self) -> BinaryLayers | None:
         """Return binary layers embedded in the file.
 
         The returned `BinaryLayers` object is an immutable sequence of `BinaryLayer`
         objects, one for each binary layer in the file.  Each `BinaryLayer` object in
```

### Comparing `nd2-0.6.0/src/nd2/structures.py` & `nd2-0.6.1/src/nd2/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import builtins
 from dataclasses import dataclass, field
 from enum import IntEnum
 from typing import NamedTuple, Union
 
 from typing_extensions import Literal, TypeAlias, TypedDict
 
+from ._pysdk._sdk_types import EventMeaning, StimulationType
+
 
 class TextInfo(TypedDict, total=False):
     imageId: str
     type: str
     group: str
     sampleId: str
     author: str
@@ -86,24 +88,32 @@
 ]
 
 
 @dataclass
 class _Loop:
     count: int
     nestingLevel: int
-    parameters: LoopParams
+    parameters: LoopParams | None
     type: LoopTypeString
 
 
 @dataclass
 class SpectLoop:
     count: int
     type: Literal["SpectLoop"] = "SpectLoop"
 
 
+@dataclass
+class CustomLoop(_Loop):
+    count: int
+    nestingLevel: int = 0
+    parameters: None = None
+    type: Literal["CustomLoop"] = "CustomLoop"
+
+
 #####
 
 
 @dataclass
 class TimeLoop(_Loop):
     parameters: TimeLoopParams
     type: Literal["TimeLoop"] = "TimeLoop"
@@ -221,15 +231,15 @@
     stepUm: float
     bottomToTop: bool
     deviceName: str | None = None
 
 
 ###
 
-ExpLoop = Union[TimeLoop, NETimeLoop, XYPosLoop, ZStackLoop]
+ExpLoop = Union[TimeLoop, NETimeLoop, XYPosLoop, ZStackLoop, CustomLoop]
 LoopParams = Union[TimeLoopParams, NETimeLoopParams, XYPosLoopParams, ZStackLoopParams]
 
 # metadata #################
 
 
 @dataclass
 class Metadata:
@@ -280,14 +290,15 @@
 
 @dataclass
 class LoopIndices:
     NETimeLoop: int | None = None
     TimeLoop: int | None = None
     XYPosLoop: int | None = None
     ZStackLoop: int | None = None
+    CustomLoop: int | None = field(default=None, repr=False, compare=False)
 
 
 @dataclass
 class Microscope:
     objectiveMagnification: float | None = None
     objectiveName: str | None = None
     objectiveNumericalAperture: float | None = None
@@ -504,7 +515,27 @@
             if key == "shapeType":
                 self.shapeType = RoiShapeType(self.shapeType)
             elif key == "interpType":
                 self.interpType = InterpType(self.interpType)
             else:
                 type_ = getattr(builtins, anno)
                 setattr(self, key, type_(getattr(self, key)))
+
+
+@dataclass
+class ExperimentEvent:
+    id: int = 0  #  ID of the event
+    # meaning of the time/time2 could be found in the globalmetadata-eTimeSource
+    time: float = 0.0  # time in msec, in the same axis as time in image metaformat
+    time2: float = 0.0  # time in msec, similar to acqtime2
+    meaning: EventMeaning = EventMeaning.Unspecified
+    description: str = ""  # description that the user typed in (if any)
+    data: str = ""  # the additional data (command code, macro file path etc.)
+    stimulation: StimulationEvent | None = None
+
+
+@dataclass
+class StimulationEvent:
+    type: StimulationType = StimulationType.NoStimulation
+    loop_index: int = 0
+    position: int = 0
+    description: str = ""
```

### Comparing `nd2-0.6.0/src/nd2/_legacy/_legacy.py` & `nd2-0.6.1/src/nd2/_legacy/_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,17 +199,20 @@
     def _get_xml_dict(self, key: bytes, index: int = 0) -> dict:
         try:
             bxml = self._read_chunk(self._chunkmap[key][index])
             return parse_xml_block(bxml)
         except KeyError:
             return {}
 
-    @cached_property
-    def events(self) -> dict:
-        return self._get_xml_dict(b"IEVE")
+    def _img_exp_events(self) -> list[strct.ExperimentEvent]:
+        from nd2._pysdk._parse import load_legacy_events
+
+        _events = self._get_xml_dict(b"IEVE")
+        events: list[dict] = _events.get("FirstEvent", {}).get("no_name", [])
+        return load_legacy_events(events)
 
     # def sizes(self):
     #     attrs = cast(Attributes, self.attributes)
 
     def text_info(self) -> dict:
         d = self._get_xml_dict(b"TINF")
         for i in d.get("TextInfoItem", []):
```

### Comparing `nd2-0.6.0/src/nd2/_legacy/_legacy_xml.py` & `nd2-0.6.1/src/nd2/_legacy/_legacy_xml.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/src/nd2/_pysdk/_chunk_decode.py` & `nd2-0.6.1/src/nd2/_pysdk/_chunk_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from __future__ import annotations
 
 import mmap
 import struct
 from contextlib import contextmanager
 from io import BufferedReader
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterator, cast
+from typing import TYPE_CHECKING, BinaryIO, Iterator, cast
 
 import numpy as np
 
 if TYPE_CHECKING:
     from os import PathLike
-    from typing import BinaryIO, Final
+    from typing import Final
 
     from numpy.typing import DTypeLike
 
     StrOrBytesPath = str | bytes | PathLike[str] | PathLike[bytes]
 
     StartFileChunk = tuple[int, int, int, bytes, bytes]
     #              = (magic, name_length, data_length, name, data)
@@ -62,15 +62,15 @@
 
 SIG_CHUNKMAP_LOC = struct.Struct("32sQ")
 # the last 40 bytes of the file, containing the signature and location of chunkmap
 # char name[32]
 # uint64_t offset
 
 
-def get_version(fh: BufferedReader | StrOrBytesPath) -> tuple[int, int]:
+def get_version(fh: BinaryIO | StrOrBytesPath) -> tuple[int, int]:
     """Get the version of the ND2 file or raise an exception.
 
     Parameters
     ----------
     fh : BufferedReader | str | bytes | Path
         The file handle or path to the ND2 file.
 
@@ -80,15 +80,15 @@
         (major, minor) version of the ND2 file
 
     Raises
     ------
     ValueError
         If the file is not a valid ND2 file or the header chunk is corrupt.
     """
-    if not isinstance(fh, BufferedReader):
+    if not isinstance(fh, (BinaryIO, BufferedReader)):
         with open(fh, "rb") as fh:
             chunk = START_FILE_CHUNK.unpack(fh.read(START_FILE_CHUNK.size))
     else:
         # leave it open if it came in open
         fh.seek(0)
         chunk = START_FILE_CHUNK.unpack(fh.read(START_FILE_CHUNK.size))
```

### Comparing `nd2-0.6.0/src/nd2/_pysdk/_parse.py` & `nd2-0.6.1/src/nd2/_pysdk/_parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from __future__ import annotations
 
 import re
+import warnings
 from dataclasses import asdict
 from math import ceil
 from struct import Struct
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING, Iterable, cast
 
 import numpy as np
 
 from nd2 import structures as strct
 
-from ._sdk_types import ELxModalityMask
+from ._sdk_types import ELxModalityMask, EventMeaning, StimulationType
 
 if TYPE_CHECKING:
+    from typing_extensions import TypeGuard
+
     from nd2.structures import AxisInterpretation, ExpLoop, XYPosLoopParams
 
     from ._sdk_types import (
         CompressionType,
         FilterDict,
         FluorescentProbeDict,
         GlobalMetadata,
         NETimeLoopPars,
         PicturePlanesDict,
         PlaneDict,
         RawAttributesDict,
         RawExperimentDict,
+        RawExperimentRecordDict,
+        RawLiteEventDict,
         RawMetaDict,
         RawTextInfoDict,
         SpectLoopPars,
         SpectrumDict,
         TimeLoopPars,
         XYPosLoopPars,
         ZStackLoopPars,
@@ -208,23 +213,23 @@
             dest = load_experiment(level + 1, item, dest)
 
     return dest
 
 
 def _load_single_experiment_loop(
     exp: RawExperimentDict,
-) -> ExpLoop | strct.SpectLoop | None:
+) -> ExpLoop | strct.SpectLoop | strct.CustomLoop | None:
     loop_type = exp.get("eType", 0)
     loop_params = exp.get("uLoopPars", {})
     if not loop_params or loop_type > max(strct.LoopType):
         return None
 
     # FIXME: sometimes it's a dict with a single i000000 key?
     # this only happens with version < (3, 0)
-    if len(loop_params) == 1:
+    if list(loop_params) == ["i0000000000"]:
         loop_params = next(iter(loop_params.values()))  # type: ignore
 
     if loop_type == strct.LoopType.TimeLoop:  # 1
         return _parse_time_loop(cast("TimeLoopPars", loop_params))
     elif loop_type == strct.LoopType.XYPosLoop:  # 2
         valid = exp.get("pItemValid", [])
         return _parse_xy_pos_loop(cast("XYPosLoopPars", loop_params), valid)
@@ -233,14 +238,17 @@
     elif loop_type == strct.LoopType.NETimeLoop:  # 8
         return _parse_ne_time_loop(cast("NETimeLoopPars", loop_params))
     elif loop_type == strct.LoopType.SpectLoop:  # 6
         loop_params = cast("SpectLoopPars", loop_params)
         count = loop_params.get("uiCount", 0)
         count = loop_params.get("pPlanes", {}).get("uiCount", count)
         return strct.SpectLoop(count=count)
+    elif loop_type == strct.LoopType.CustomLoop:  # 7
+        count = cast("int", loop_params.get("uiCount", 0))
+        return strct.CustomLoop(count=count)
 
     raise NotImplementedError(  # pragma: no cover
         f"We've never seen a file like this! (loop_type={loop_type!r}). We'd "
         "appreciate it if you would submit this file at "
         "https://github.com/tlambert03/nd2/issues/new",
     )
 
@@ -344,14 +352,90 @@
     # return the wavelength associated with the max value, or 0.0 if no spectrum
     if not item:
         return 0.0
     spectrum = _get_spectrum(item)
     return max(spectrum, key=lambda x: x[0])[1] if spectrum else 0.0
 
 
+LITE_EVENT_KEYS = {"T", "T2", "M", "D", "A", "I", "S"}
+
+
+def _is_lite_events(events: dict) -> TypeGuard[dict[str, RawLiteEventDict]]:
+    event_keys = set.union(*(set(x) for x in events.values()))
+    return event_keys.issubset(LITE_EVENT_KEYS)
+
+
+def load_events(events: RawExperimentRecordDict) -> list[strct.ExperimentEvent]:
+    # found in b'CustomData|ExperimentEventsV1_0!'
+    count = events.get("uiCount", 0)
+    if count == 0:
+        return []
+    p_events = events.get("pEvents", {})
+    if _is_lite_events(p_events):
+        return [_load_lite_event(x[1]) for x in sorted(p_events.items())]
+    warnings.warn(  # pragma: no cover
+        "We haven't seen this event type before, we'd appreciate if you submit this "
+        "file at https://github.com/tlambert03/nd2/issues/new",
+        stacklevel=2,
+    )
+    return []
+
+
+def load_legacy_events(events: Iterable[dict]) -> list[strct.ExperimentEvent]:
+    return [_load_legacy_event(*ie) for ie in enumerate(events)]
+
+
+def _load_legacy_event(id: int, event: dict) -> strct.ExperimentEvent:
+    # event will have keys: 'Time', 'Meaning', 'Description', 'Data',
+    # meaning seems to almost always be 7
+
+    meaning = EventMeaning(event.get("Meaning", 0))
+    description = event.get("Description", "") or meaning.description()
+    data = event.get("Data", "")
+    if data:
+        description += f" - {data}"
+
+    return strct.ExperimentEvent(
+        id=id,
+        time=event.get("Time", 0.0),
+        meaning=meaning,
+        description=description,
+        data=data,
+    )
+
+
+def _load_lite_event(event: RawLiteEventDict) -> strct.ExperimentEvent:
+    stim_event = event.get("S", {})
+    if stim_event:
+        stim_struct = strct.StimulationEvent(
+            type=StimulationType(stim_event.get("T", 0)),
+            loop_index=stim_event.get("L", 0),
+            position=stim_event.get("P", 0),
+            description=stim_event.get("D", ""),
+        )
+    else:
+        stim_struct = None
+
+    meaning = EventMeaning(event.get("M", 0))
+    description = event.get("D", "") or meaning.description()
+    if stim_struct:
+        description += f" Phase {stim_struct.type.name}"
+        if stim_struct.description:
+            description += f" - {stim_struct.description}"
+    return strct.ExperimentEvent(
+        id=event.get("I", 0),
+        time=event.get("T", 0.0),
+        time2=event.get("T2", 0.0),
+        meaning=meaning,
+        description=description,
+        data=event.get("A", ""),
+        stimulation=stim_struct,
+    )
+
+
 def load_text_info(raw_txt_info: RawTextInfoDict) -> strct.TextInfo:
     # we only want keys that are present in the raw_txt_info
 
     out = {
         key: raw_txt_info.get(lookup)
         for key, lookup in (
             ("imageId", "TextInfoItem_0"),
```

### Comparing `nd2-0.6.0/src/nd2/_pysdk/_pysdk.py` & `nd2-0.6.1/src/nd2/_pysdk/_pysdk.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 from __future__ import annotations
 
 import mmap
 import os
 import warnings
-from typing import TYPE_CHECKING, Sequence, cast
+from pathlib import Path
+from typing import TYPE_CHECKING, Iterable, Sequence, cast
 
 import numpy as np
 
 from nd2 import structures
 from nd2._clx_lite import json_from_clx_lite_variant
 from nd2._clx_xml import json_from_clx_variant
 from nd2._pysdk._chunk_decode import (
     _robustly_read_named_chunk,
     get_chunkmap,
     get_version,
     read_nd2_chunk,
 )
 from nd2._pysdk._parse import (
     load_attributes,
+    load_events,
     load_experiment,
     load_frame_metadata,
     load_global_metadata,
     load_metadata,
     load_text_info,
 )
+from nd2._util import TIME_KEY, Z_SERIES_KEY
 
 if TYPE_CHECKING:
+    import datetime
     from io import BufferedReader
     from os import PathLike
-    from pathlib import Path
     from typing import Any
 
     from typing_extensions import TypeAlias
 
     from ._chunk_decode import ChunkMap
     from ._sdk_types import (
         GlobalMetadata,
         RawAttributesDict,
         RawExperimentDict,
+        RawExperimentRecordDict,
         RawMetaDict,
+        RawTagDict,
         RawTextInfoDict,
     )
 
     StrOrBytesPath: TypeAlias = str | bytes | PathLike[str] | PathLike[bytes]
     StartFileChunk: TypeAlias = tuple[int, int, int, bytes, bytes]
 
 
 class ND2Reader:
     def __init__(
         self, path: str | Path, validate_frames: bool = False, search_window: int = 100
     ) -> None:
-        self._filename = path
+        self._path = Path(path)
         self._fh: BufferedReader | None = None
         self._mmap: mmap.mmap | None = None
         self._chunkmap: ChunkMap = {}
         self._cached_decoded_chunks: dict[bytes, Any] = {}
         self._error_radius: int | None = (
             search_window * 1000 if validate_frames else None
         )
 
         self._version: tuple[int, int] | None = None
         self._attributes: structures.Attributes | None = None
         self._experiment: list[structures.ExpLoop] | None = None
         self._text_info: structures.TextInfo | None = None
         self._metadata: structures.Metadata | None = None
+        self._events: list[structures.ExperimentEvent] | None = None
 
         self._global_metadata: GlobalMetadata | None = None
         self._cached_frame_offsets: dict[int, int] | None = None
         self._raw_frame_shape_: tuple[int, ...] | None = None
         self._dtype_: np.dtype | None = None
         self._strides_: tuple[int, ...] | None = None
         self._frame_times: list[float] | None = None
@@ -77,15 +83,15 @@
         self._raw_text_info: RawTextInfoDict | None = None
         self._raw_image_metadata: RawMetaDict | None = None
 
         self.open()
 
     def open(self) -> None:
         if self._fh is None:
-            self._fh = open(self._filename, "rb")
+            self._fh = open(self._path, "rb")
             self._mmap = mmap.mmap(self._fh.fileno(), 0, access=mmap.ACCESS_READ)
 
     def close(self) -> None:
         if self._fh is not None:
             self._fh.close()
             self._fh = None
         if self._mmap is not None:
@@ -174,15 +180,15 @@
         return self._cached_decoded_chunks[name]
 
     @property
     def version(self) -> tuple[int, int]:
         """Return the file format version as a tuple of ints."""
         if self._version is None:
             try:
-                self._version = get_version(self._fh or self._filename)
+                self._version = get_version(self._fh or self._path)
             except Exception:
                 self._version = (-1, -1)
                 raise
         return self._version
 
     def _get_raw_image_metadata(self) -> RawMetaDict:
         if not self._raw_image_metadata:
@@ -204,15 +210,15 @@
             self._global_metadata = load_global_metadata(
                 attrs=self.attributes,
                 raw_meta=self._get_raw_image_metadata(),
                 exp_loops=self.experiment(),
                 text_info=self.text_info(),
             )
             if self._global_metadata["time"]["absoluteJulianDayNumber"] < 1:
-                julian_day = os.stat(self._filename).st_ctime / 86400.0 + 2440587.5
+                julian_day = os.stat(self._path).st_ctime / 86400.0 + 2440587.5
                 self._global_metadata["time"]["absoluteJulianDayNumber"] = julian_day
 
         return self._global_metadata
 
     def metadata(self) -> structures.Metadata:
         if not self._metadata:
             self._metadata = load_metadata(
@@ -248,14 +254,30 @@
             else:
                 exp = self._decode_chunk(k, strip_prefix=False)
                 exp = exp.get("SLxExperiment", exp)  # for v3 only
                 self._raw_experiment = cast("RawExperimentDict", exp)
                 self._experiment = load_experiment(0, self._raw_experiment)
         return self._experiment
 
+    def _img_exp_events(self) -> list[structures.ExperimentEvent]:
+        """Parse and return all Image and Experiment events."""
+        if not self._events:
+            events = []
+            for key in (
+                b"ImageEvents",
+                b"ImageEventsLV!",
+                b"CustomData|ExperimentEventsV1_0!",
+            ):
+                if key in self.chunkmap:
+                    e = self._decode_chunk(key, strip_prefix=False)
+                    e = e.get("RLxExperimentRecord", e)
+                    events.extend(load_events(cast("RawExperimentRecordDict", e)))
+            self._events = events
+        return self._events
+
     def _cached_frame_times(self) -> list[float]:
         """Returns frame times in milliseconds."""
         if self._frame_times is None:
             try:
                 acq_times = self._load_chunk(b"CustomData|AcqTimesCache!")
                 times = np.frombuffer(acq_times, dtype=np.float64).tolist()
                 self._frame_times = times[: self._seq_count()]  # limit to valid frames
@@ -288,14 +310,17 @@
     def _coord_size(self) -> int:
         return len(self.experiment())
 
     def _coord_info(self) -> list[tuple[int, str, int]]:
         return [(i, x.type, x.count) for i, x in enumerate(self.experiment())]
 
     def _seq_count(self) -> int:
+        # this differs from self.attributes.SequenceCount in that it
+        # includes the actual number of frames in the experiment,
+        # excluding "invalid" frames.
         return int(np.prod([x.count for x in self.experiment()]))
 
     @property
     def _frame_offsets(self) -> dict[int, int]:
         """Return map of frame number to offset in the file."""
         if self._cached_frame_offsets is None:
             # image frames are stored in the chunkmap as "ImageDataSeq|<frame>!"
@@ -406,92 +431,139 @@
     def _custom_data(self) -> dict[str, Any]:
         return {
             k.decode()[14:-1]: self._decode_chunk(k)
             for k in self.chunkmap
             if k.startswith(b"CustomDataVar|")
         }
 
-    def recorded_data(self) -> dict[str, np.ndarray | Sequence]:
-        """Return tabular data recorded for each frame of the experiment.
-
-        This method returns a dict of equal-length sequences (passable to
-        pd.DataFrame()). It matches the tabular data reported in the Image Properties >
-        Recorded Data tab of the NIS Viewer.
-
-        (There will be a column for each tag in the `CustomDataV2_0` section of
-        `ND2File.custom_data`)
+    def _acquisition_data(self) -> dict[str, Sequence[Any]]:
+        """Return a dict of acquisition times and z-series indices for each image.
 
-        Legacy ND2 files are not supported.
+        {
+            "Time [s]": [0.0, 0.0, 0.0, ...],
+            "Z-Series": [-1.0, 0., 1.0, ...],
+        }
         """
-        try:
-            cd = self._decode_chunk(b"CustomDataVar|CustomDataV2_0!")
-        except KeyError:
-            return {}
-
-        if not cd:
-            return {}
-
-        if "CustomTagDescription_v1.0" not in cd:
-            warnings.warn(
-                "Could not find 'CustomTagDescription_v1' tag, please open an issue "
-                "with this nd2 file at https://github.com/tlambert03/nd2/issues/new",
-                stacklevel=2,
-            )
-            return {}
-
         data: dict[str, np.ndarray | Sequence] = {}
         frame_times = self._cached_frame_times()
         if frame_times:
-            data["Time [s]"] = [x / 1000 for x in frame_times]
+            data[TIME_KEY] = [x / 1000 for x in frame_times]
 
+        # FIXME: this whole thing is dumb... must be a better way
         experiment = self.experiment()
-        for i, loop in enumerate(experiment):
-            if not isinstance(loop, structures.ZStackLoop):
+        for i, z_loop in enumerate(experiment):
+            if not isinstance(z_loop, structures.ZStackLoop):
                 continue
 
-            z_loop = loop
             z_positions = [
                 z_loop.parameters.stepUm * (i - z_loop.parameters.homeIndex)
                 for i in range(z_loop.count)
             ]
             if not z_loop.parameters.bottomToTop:
-                z_positions = list(reversed(z_positions))
+                z_positions.reverse()
 
             def _seq_z_pos(
                 seq_index: int, z_idx: int = i, _zp: list[float] = z_positions
             ) -> float:
                 """Convert a sequence index to a coordinate tuple."""
                 for n, _loop in enumerate(experiment):
                     if n == z_idx:
                         return _zp[seq_index % _loop.count]
                     seq_index //= _loop.count
                 raise ValueError("Invalid sequence index or z_idx")
 
-            seq_count = self.attributes.sequenceCount
-            data["Z-Series"] = np.array([_seq_z_pos(i) for i in range(seq_count)])
+            seq_count = self._seq_count()
+            data[Z_SERIES_KEY] = np.array([_seq_z_pos(i) for i in range(seq_count)])
+
+        return data  # type: ignore [return-value]
+
+    def _custom_tags(self) -> dict[str, Any]:
+        """Return tags mentioned in in CustomDataVar|CustomDataV2_0.
+
+        This is a dict of {header: [values]}, where
+        len([values]) == self.attributes.sequenceCount
+
+        {
+            "Camera_ExposureTime1": [0.0, 0.0, 0.0, ...],
+            "PFS_OFFSET": [-1.0, 0., 1.0, ...],
+            "PFS_STATUS": [0, 0, 0, ...],
+        }
+        """
+        data: dict[str, Any] = {}
+        try:
+            cd = self._decode_chunk(b"CustomDataVar|CustomDataV2_0!")
+        except KeyError:
+            return data
+
+        if not cd:  # pragma: no cover
+            return data
+
+        if "CustomTagDescription_v1.0" not in cd:  # pragma: no cover
+            warnings.warn(
+                "Could not find 'CustomTagDescription_v1' tag, please open an issue "
+                "with this nd2 file at https://github.com/tlambert03/nd2/issues/new",
+                stacklevel=2,
+            )
+            return {}
 
         # tags will be a dict of dicts: eg:
         # {
         #     'Tag0': {'ID': 'Camera_ExposureTime1', 'Type': 3, ... },
         #     'Tag1': {'ID': 'PFS_OFFSET', 'Type': 2, 'Group': 0, 'Size': 1, ...},
         #     'Tag2': {'ID': 'PFS_STATUS', 'Type': 2, 'Group': 0, 'Size': 1, ...},
         # }
-        # FIXME: technically, it is possible to have multiple tags with the same Desc
-        # (e.g. for IDs PFS_OFFSET and Z2). In the current implementation, the
-        # 2nd tag will overwrite the first one.
-        for tag in cd["CustomTagDescription_v1.0"].values():
+        tags = cast("Iterable[RawTagDict]", cd["CustomTagDescription_v1.0"].values())
+        for tag in tags:
             if tag["Type"] == 1:
                 warnings.warn(
                     f"{tag['Desc']!r} column skipped: "
-                    "(parsing string data is not yet implemented)",
+                    "(parsing string data is not yet implemented).  Please open an "
+                    "issue with this nd2 file at "
+                    "https://github.com/tlambert03/nd2/issues/new",
                     stacklevel=2,
                 )
                 continue
-            col_header = f"{tag['Desc']}"
-            if tag["Unit"]:
+
+            col_header = tag["Desc"]
+            if col_header in data:  # pragma: no cover
+                # sourcery skip: hoist-if-from-if
+                col_header = tag["ID"]
+                if col_header in data:
+                    col_header = f"{tag['Desc']} ({tag['ID']})"
+
+            if tag["Unit"].strip():
                 col_header += f" [{tag['Unit']}]"
 
-            buffer = self._load_chunk(f"CustomData|{tag['ID']}!".encode())
+            buffer_ = self._load_chunk(f"CustomData|{tag['ID']}!".encode())
             dtype = {3: np.float64, 2: np.int32}[tag["Type"]]
-            data[col_header] = np.frombuffer(buffer, dtype=dtype, count=tag["Size"])
+            data[col_header] = np.frombuffer(buffer_, dtype=dtype, count=tag["Size"])
 
         return data
+
+    def _app_info(self) -> dict:
+        """Return a dict of app info."""
+        k = b"CustomDataVar|AppInfo_V1_0!"
+        return self._decode_chunk(k) if k in self.chunkmap else {}
+
+    def _acquisition_date(self) -> datetime.datetime | str | None:
+        """Try to extract acquisition date.
+
+        A best effort is made to extract a datetime object from the date string,
+        but if that fails, the raw string is returned.  Use isinstance() to
+        be safe.
+        """
+        from nd2._util import parse_time
+
+        date = self.text_info().get("date")
+        if date:
+            try:
+                return parse_time(date)
+            except ValueError:
+                return date
+
+        time = self._cached_global_metadata().get("time", {})
+        jdn = time.get("absoluteJulianDayNumber")
+        if jdn:
+            from nd2._util import jdn_to_datetime_utc
+
+            return jdn_to_datetime_utc(jdn)
+        return None
```

### Comparing `nd2-0.6.0/tests/conftest.py` & `nd2-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/readlim_output.json` & `nd2-0.6.1/tests/readlim_output.json`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/samples_metadata.json` & `nd2-0.6.1/tests/samples_metadata.json`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_aicsimage.py` & `nd2-0.6.1/tests/test_aicsimage.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_binary.py` & `nd2-0.6.1/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_dask_dispatch.py` & `nd2-0.6.1/tests/test_dask_dispatch.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_metadata.py` & `nd2-0.6.1/tests/test_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+from __future__ import annotations
+
 import json
 import sys
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import dask.array as da
 import pytest
 import xarray as xr
-from nd2 import ND2File, structures
+from nd2 import ND2File, _util, structures
 from nd2._pysdk._chunk_decode import ND2_FILE_SIGNATURE
 
 sys.path.append(str(Path(__file__).parent.parent / "scripts"))
 from nd2_describe import get_nd2_stats  # noqa: E402
 
+if TYPE_CHECKING:
+    from typing_extensions import Literal
+
+
 with open("tests/samples_metadata.json") as f:
     EXPECTED = json.load(f)
 
 DATA = Path(__file__).parent / "data"
 
 
 @pytest.mark.parametrize("path", EXPECTED, ids=lambda x: f'{x}_{EXPECTED[x]["ver"]}')
@@ -70,15 +77,17 @@
         assert isinstance(nd.closed, bool)
         assert isinstance(nd.ndim, int)
         _bd = nd.binary_data
         assert isinstance(nd.is_rgb, bool)
         assert isinstance(nd.nbytes, int)
 
         assert isinstance(nd.unstructured_metadata(), dict)
-        assert isinstance(nd.recorded_data, dict)
+        assert isinstance(nd.events(), list)
+        with pytest.warns(FutureWarning):
+            assert isinstance(nd.recorded_data, dict)
 
     assert nd.closed
 
 
 def test_metadata_extraction_legacy(old_nd2):
     assert ND2File.is_supported_file(old_nd2)
     with ND2File(old_nd2) as nd:
@@ -92,26 +101,31 @@
         # assert isinstance(nd.metadata, structures.Metadata)
         assert isinstance(nd.experiment, list)
         assert isinstance(nd.text_info, dict)
         xarr = nd.to_xarray()
         assert isinstance(xarr, xr.DataArray)
         assert isinstance(xarr.data, da.Array)
 
+        with pytest.warns(UserWarning, match="not implemented"):
+            nd.events()
+
     assert nd.closed
 
 
 def test_recorded_data() -> None:
     # this method is smoke-tested for every file above...
     # but specific values are asserted here:
     with ND2File(DATA / "cluster.nd2") as f:
-        rd = f.recorded_data
+        with pytest.warns(FutureWarning, match="deprecated"):
+            rd = f.recorded_data
+
         headers = list(rd)
         row_0 = [rd[h][0] for h in headers]
         assert headers == [
-            "Time [s]",
+            _util.TIME_KEY,
             "Z-Series",
             "Camera 1 Temperature [°C]",
             "Laser Power; 1.channel [%]",
             "High Voltage; 1.channel",
             "Laser Power; 2.channel [%]",
             "High Voltage; 2.channel",
             "Laser Power; 3.channel [%]",
@@ -142,7 +156,20 @@
             0,
             -1,
             7,
             -26056.951209195162,
             -4155.462732842248,
             3916.7250000000004,
         ]
+
+
+@pytest.mark.parametrize("orient", ["records", "dict", "list"])
+def test_events(new_nd2: Path, orient: Literal["records", "dict", "list"]) -> None:
+    with ND2File(new_nd2) as f:
+        events = f.events(orient=orient)
+
+    assert isinstance(events, list if orient == "records" else dict)
+    if events and isinstance(events, dict):
+        assert _util.TIME_KEY in events
+
+    pd = pytest.importorskip("pandas")
+    print(pd.DataFrame(events))
```

### Comparing `nd2-0.6.0/tests/test_reader.py` & `nd2-0.6.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_readme.py` & `nd2-0.6.1/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_rescue.py` & `nd2-0.6.1/tests/test_rescue.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/test_xml.py` & `nd2-0.6.1/tests/test_xml.py`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/variant.xml` & `nd2-0.6.1/tests/variant.xml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/tests/variant_CustomDataV2_0.xml` & `nd2-0.6.1/tests/variant_CustomDataV2_0.xml`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/.gitignore` & `nd2-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/LICENSE` & `nd2-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nd2-0.6.0/README.md` & `nd2-0.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,17 @@
 f.experiment        # List[nd2.structures.ExpLoop]
 f.rois              # Dict[int, nd2.structures.ROI]
 f.voxel_size()      # VoxelSize(x=0.65, y=0.65, z=1.0)
 f.text_info         # dict of misc info
 
 f.binary_data       # any binary masks stored in the file.  See below.
 f.custom_data       # bits of unstructured metadata that start with CustomData
-f.recorded_data     # returns a dict of lists (passable to pandas.DataFrame) that
-                    # the tabular "Recorded Data" view from in NIS Elements/Viewer
+f.events()          # returns tabular "Recorded Data" view from in NIS Elements/Viewer
                     # with info for each frame in the experiment.
+                    # output is passabled to pandas.DataFrame
 
 # allll the metadata we can find...
 # no attempt made to standardize or parse it
 # look in here if you're searching for metdata that isn't exposed in the above
 # but try not to rely on it, as it's not guaranteed to be stable
 f.unstructured_metadata()
 
@@ -332,14 +332,54 @@
 }
 ```
 
 </details>
 
 <details>
 
+<summary><code>binary_data</code></summary>
+
+This property returns an `nd2.BinaryLayers` object representing all of the
+binary masks in the nd2 file.
+
+A `nd2.BinaryLayers` object is a sequence of individual `nd2.BinaryLayer`
+objects (one for each binary layer found in the file).  Each `BinaryLayer` in
+the sequence is a named tuple that has, among other things, a `name` attribute,
+and a `data` attribute that is list of numpy arrays (one for each frame in the
+experiment) or `None` if the binary layer had no data in that frame.
+
+The most common use case will be to cast either the entire `BinaryLayers` object
+or an individual `BinaryLayer` to a `numpy.ndarray`:
+
+```python
+>>> import nd2
+>>> nd2file = nd2.ND2File('path/to/file.nd2')
+>>> binary_layers = nd2file.binary_data
+
+# The output array will have shape
+# (n_binary_layers, *coord_shape, *frame_shape).
+>>> np.asarray(binary_layers)
+```
+
+For example, if the data in the nd2 file has shape `(nT, nZ, nC, nY, nX)`, and
+there are 4 binary layers, then the output of `np.asarray(nd2file.binary_data)` will
+have shape `(4, nT, nZ, nY, nX)`.  (Note that the `nC` dimension is not present
+in the output array, and the binary layers are always in the first axis).
+
+You can also cast an individual `BinaryLayer` to a numpy array:
+
+```python
+>>> binary_layer = binary_layers[0]
+>>> np.asarray(binary_layer)
+```
+
+</details>
+
+<details>
+
 <summary><code>custom_data</code></summary>
 
 No attempt is made to parse this data.  It will vary from file to file, but you may find something useful here:
 
 ```python
 {
     'StreamDataV1_0': {
@@ -601,51 +641,128 @@
 }
 ```
 
 </details>
 
 <details>
 
-<summary><code>recorded_data</code></summary>
+<summary><code>events</code></summary>
+
+This property returns the tabular data reported in the `Image Properties >
+Recorded Data` tab of the NIS Viewer.
+
+(There will be a column for each tag in the `CustomDataV2_0` section of
+`custom_data` above, as well as any additional events found in the metadata)
 
-This property returns a `dict` of equal-length sequences.
-It matches the tabular data reported in the `Image Properties > Recorded Data` tab of the NIS Viewer.
+The format of the return type data is controlled by the `orient` argument:
 
-(There will be a column for each tag in the `CustomDataV2_0` section of `custom_data` above.)
+- `'records'` : list of dicts - `[{column -> value}, ...]` (default)
+- `'dict'` :    dict of dicts - `{column -> {index -> value}, ...}`
+- `'list'` :    dict of lists - `{column -> [value, ...]}`
+
+Not every column header appears in every event, so when `orient` is either
+`'dict'` or `'list'`, `float('nan')` will be inserted to maintain a consistent
+length for each column.
 
 ```python
+
+# with `orient='records'` (DEFAULT)
+[
+    {
+        'Time [s]': 1.32686654,
+        'Z-Series': -2.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 552.74,
+        'Ti2 ZDrive [µm]': 552.74
+    },
+    {
+        'Time [s]': 1.69089657,
+        'Z-Series': -1.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 553.74,
+        'Ti2 ZDrive [µm]': 553.74
+    },
+    {
+        'Time [s]': 2.04194662,
+        'Z-Series': 0.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 554.74,
+        'Ti2 ZDrive [µm]': 554.74
+    },
+    {
+        'Time [s]': 2.38194662,
+        'Z-Series': 1.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 555.74,
+        'Ti2 ZDrive [µm]': 555.74
+    },
+    {
+        'Time [s]': 2.63795663,
+        'Z-Series': 2.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 556.74,
+        'Ti2 ZDrive [µm]': 556.74
+    }
+]
+
+# with `orient='list'`
+{
+    'Time [s]': array([1.32686654, 1.69089657, 2.04194662, 2.38194662, 2.63795663]),
+    'Z-Series': array([-2., -1.,  0.,  1.,  2.]),
+    'Exposure Time [ms]': array([100., 100., 100., 100., 100.]),
+    'PFS Offset': array([0, 0, 0, 0, 0], dtype=int32),
+    'PFS Status': array([0, 0, 0, 0, 0], dtype=int32),
+    'X Coord [µm]': array([31452.2, 31452.2, 31452.2, 31452.2, 31452.2]),
+    'Y Coord [µm]': array([-1801.6, -1801.6, -1801.6, -1801.6, -1801.6]),
+    'Z Coord [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74]),
+    'Ti2 ZDrive [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74])
+}
+
+# with `orient='dict'`
 {
-    'Time [s]': array([ 1.32686654,  1.69089657,  2.04194662,  2.38194662,  2.63795663,
-        8.7022286 ,  9.03626864,  9.33031869,  9.63934872,  9.90636874,
-       11.48143856, 11.7964786 , 12.0894786 , 12.37153866, 12.66546859]),
-    'Z-Series': array([-2., -1.,  0.,  1.,  2., -2., -1.,  0.,  1.,  2., -2., -1.,  0.,
-        1.,  2.]),
-    'Exposure Time [ms]': array([100., 100., 100., 100., 100., 100., 100., 100., 100., 100., 100.,
-       100., 100., 100., 100.]),
-    'PFS Offset []': array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=int32),
-    'PFS Status []': array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=int32),
-    'X Coord [µm]': array([31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2,
-       31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2,
-       31452.2]),
-    'Y Coord [µm]': array([-1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6,
-       -1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6,
-       -1801.6]),
-    'Z Coord [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74, 552.7 , 553.7 , 554.68,
-       555.7 , 556.64, 552.68, 553.68, 554.68, 555.68, 556.68]),
-    'Ti2 ZDrive [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74, 552.7 , 553.7 , 554.68,
-       555.7 , 556.64, 552.68, 553.68, 554.68, 555.68, 556.68])
+    'Time [s]': {0: 1.32686654, 1: 1.69089657, 2: 2.04194662, 3: 2.38194662, 4: 2.63795663},
+    'Z-Series': {0: -2.0, 1: -1.0, 2: 0.0, 3: 1.0, 4: 2.0},
+    'Exposure Time [ms]': {0: 100.0, 1: 100.0, 2: 100.0, 3: 100.0, 4: 100.0},
+    'PFS Offset []': {0: 0, 1: 0, 2: 0, 3: 0, 4: 0},
+    'PFS Status []': {0: 0, 1: 0, 2: 0, 3: 0, 4: 0},
+    'X Coord [µm]': {0: 31452.2, 1: 31452.2, 2: 31452.2, 3: 31452.2, 4: 31452.2},
+    'Y Coord [µm]': {0: -1801.6, 1: -1801.6, 2: -1801.6, 3: -1801.6, 4: -1801.6},
+    'Z Coord [µm]': {0: 552.74, 1: 553.74, 2: 554.74, 3: 555.74, 4: 556.74},
+    'Ti2 ZDrive [µm]': {0: 552.74, 1: 553.74, 2: 554.74, 3: 555.74, 4: 556.74}
 }
+
+
 ```
 
-You can pass the output of `recorded_data` to `pandas.DataFrame`:
+You can pass the output of `events()` to `pandas.DataFrame`:
 
 ```python
-In [13]: pd.DataFrame(nd2file.recorded_data)
+In [13]: pd.DataFrame(nd2file.events())
 Out[13]:
-     Time [s]  Z-Series  Exposure Time [ms]  PFS Offset []  PFS Status []  X Coord [µm]  Y Coord [µm]  Z Coord [µm]  Ti2 ZDrive [µm]
+     Time [s]  Z-Series  Exposure Time [ms]  PFS Offset  PFS Status []  X Coord [µm]  Y Coord [µm]  Z Coord [µm]  Ti2 ZDrive [µm]
 0    1.326867      -2.0               100.0              0              0       31452.2       -1801.6        552.74           552.74
 1    1.690897      -1.0               100.0              0              0       31452.2       -1801.6        553.74           553.74
 2    2.041947       0.0               100.0              0              0       31452.2       -1801.6        554.74           554.74
 3    2.381947       1.0               100.0              0              0       31452.2       -1801.6        555.74           555.74
 4    2.637957       2.0               100.0              0              0       31452.2       -1801.6        556.74           556.74
 5    8.702229      -2.0               100.0              0              0       31452.2       -1801.6        552.70           552.70
 6    9.036269      -1.0               100.0              0              0       31452.2       -1801.6        553.70           553.70
@@ -658,54 +775,14 @@
 13  12.371539       1.0               100.0              0              0       31452.2       -1801.6        555.68           555.68
 14  12.665469       2.0               100.0              0              0       31452.2       -1801.6        556.68           556.68
 
 ```
 
 </details>
 
-<details>
-
-<summary><code>binary_data</code></summary>
-
-This property returns an `nd2.BinaryLayers` object representing all of the
-binary masks in the nd2 file.
-
-A `nd2.BinaryLayers` object is a sequence of individual `nd2.BinaryLayer`
-objects (one for each binary layer found in the file).  Each `BinaryLayer` in
-the sequence is a named tuple that has, among other things, a `name` attribute,
-and a `data` attribute that is list of numpy arrays (one for each frame in the
-experiment) or `None` if the binary layer had no data in that frame.
-
-The most common use case will be to cast either the entire `BinaryLayers` object
-or an individual `BinaryLayer` to a `numpy.ndarray`:
-
-```python
->>> import nd2
->>> nd2file = nd2.ND2File('path/to/file.nd2')
->>> binary_layers = nd2file.binary_data
-
-# The output array will have shape
-# (n_binary_layers, *coord_shape, *frame_shape).
->>> np.asarray(binary_layers)
-```
-
-For example, if the data in the nd2 file has shape `(nT, nZ, nC, nY, nX)`, and
-there are 4 binary layers, then the output of `np.asarray(nd2file.binary_data)` will
-have shape `(4, nT, nZ, nY, nX)`.  (Note that the `nC` dimension is not present
-in the output array, and the binary layers are always in the first axis).
-
-You can also cast an individual `BinaryLayer` to a numpy array:
-
-```python
->>> binary_layer = binary_layers[0]
->>> np.asarray(binary_layer)
-```
-
-</details>
-
 ## Contributing / Development
 
 To test locally and contribute.  Clone this repo, then:
 
 ```
 pip install -e .[dev]
 ```
```

### Comparing `nd2-0.6.0/pyproject.toml` & `nd2-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,40 +20,38 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = ["resource-backed-dask-array", "typing-extensions", "numpy"]
 
 [project.optional-dependencies]
-legacy = ["imagecodecs", "wurlitzer"]
+legacy = ["imagecodecs"]
 test = [
     "lxml; python_version<'3.11'",
     "aicsimageio; python_version<'3.11'",
     "dask[array]",
     "imagecodecs; platform_system=='Windows' or python_version<'3.11'",
     "psutil",
     "pytest-cov",
     "pytest>=6.0",
     "pytest-pretty",
-    "wurlitzer",
     "xarray",
 ]
 dev = [
     "aicsimageio",
     "black",
     "dask[array]",
     "imagecodecs",
     "ipython",
     "mypy",
     "pre-commit",
     "psutil",
     "pytest-cov",
     "pytest",
     "rich",
-    "wurlitzer",
     "ruff",
     "xarray",
     "lxml-stubs",
 ]
 
 [project.urls]
 homepage = "https://github.com/tlambert03/nd2"
@@ -140,14 +138,15 @@
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "@overload",
     "\\.\\.\\.",
     "except ImportError",
     "except NotImplementedError",
+    "if __name__ == .__main__.:",
 ]
 
 [tool.coverage.run]
 source = ["src"]
 
 # https://github.com/mgedmin/check-manifest#configuration
 [tool.check-manifest]
```

### Comparing `nd2-0.6.0/PKG-INFO` & `nd2-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nd2
-Version: 0.6.0
+Version: 0.6.1
 Summary: Yet another nd2 (Nikon NIS Elements) file reader
 Project-URL: homepage, https://github.com/tlambert03/nd2
 Project-URL: repository, https://github.com/tlambert03/nd2
 Project-URL: changelog, https://github.com/tlambert03/nd2/blob/main/CHANGELOG.md
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -30,29 +30,26 @@
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: psutil; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
-Requires-Dist: wurlitzer; extra == 'dev'
 Requires-Dist: xarray; extra == 'dev'
 Provides-Extra: legacy
 Requires-Dist: imagecodecs; extra == 'legacy'
-Requires-Dist: wurlitzer; extra == 'legacy'
 Provides-Extra: test
 Requires-Dist: aicsimageio; python_version < '3.11' and extra == 'test'
 Requires-Dist: dask[array]; extra == 'test'
 Requires-Dist: imagecodecs; platform_system == 'Windows' or python_version < '3.11' and extra == 'test'
 Requires-Dist: lxml; python_version < '3.11' and extra == 'test'
 Requires-Dist: psutil; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-pretty; extra == 'test'
 Requires-Dist: pytest>=6.0; extra == 'test'
-Requires-Dist: wurlitzer; extra == 'test'
 Requires-Dist: xarray; extra == 'test'
 Description-Content-Type: text/markdown
 
 # nd2
 
 [![License](https://img.shields.io/pypi/l/nd2.svg?color=green)](https://github.com/tlambert03/nd2/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nd2.svg?color=green)](https://pypi.org/project/nd2)
@@ -155,17 +152,17 @@
 f.experiment        # List[nd2.structures.ExpLoop]
 f.rois              # Dict[int, nd2.structures.ROI]
 f.voxel_size()      # VoxelSize(x=0.65, y=0.65, z=1.0)
 f.text_info         # dict of misc info
 
 f.binary_data       # any binary masks stored in the file.  See below.
 f.custom_data       # bits of unstructured metadata that start with CustomData
-f.recorded_data     # returns a dict of lists (passable to pandas.DataFrame) that
-                    # the tabular "Recorded Data" view from in NIS Elements/Viewer
+f.events()          # returns tabular "Recorded Data" view from in NIS Elements/Viewer
                     # with info for each frame in the experiment.
+                    # output is passabled to pandas.DataFrame
 
 # allll the metadata we can find...
 # no attempt made to standardize or parse it
 # look in here if you're searching for metdata that isn't exposed in the above
 # but try not to rely on it, as it's not guaranteed to be stable
 f.unstructured_metadata()
 
@@ -386,14 +383,54 @@
 }
 ```
 
 </details>
 
 <details>
 
+<summary><code>binary_data</code></summary>
+
+This property returns an `nd2.BinaryLayers` object representing all of the
+binary masks in the nd2 file.
+
+A `nd2.BinaryLayers` object is a sequence of individual `nd2.BinaryLayer`
+objects (one for each binary layer found in the file).  Each `BinaryLayer` in
+the sequence is a named tuple that has, among other things, a `name` attribute,
+and a `data` attribute that is list of numpy arrays (one for each frame in the
+experiment) or `None` if the binary layer had no data in that frame.
+
+The most common use case will be to cast either the entire `BinaryLayers` object
+or an individual `BinaryLayer` to a `numpy.ndarray`:
+
+```python
+>>> import nd2
+>>> nd2file = nd2.ND2File('path/to/file.nd2')
+>>> binary_layers = nd2file.binary_data
+
+# The output array will have shape
+# (n_binary_layers, *coord_shape, *frame_shape).
+>>> np.asarray(binary_layers)
+```
+
+For example, if the data in the nd2 file has shape `(nT, nZ, nC, nY, nX)`, and
+there are 4 binary layers, then the output of `np.asarray(nd2file.binary_data)` will
+have shape `(4, nT, nZ, nY, nX)`.  (Note that the `nC` dimension is not present
+in the output array, and the binary layers are always in the first axis).
+
+You can also cast an individual `BinaryLayer` to a numpy array:
+
+```python
+>>> binary_layer = binary_layers[0]
+>>> np.asarray(binary_layer)
+```
+
+</details>
+
+<details>
+
 <summary><code>custom_data</code></summary>
 
 No attempt is made to parse this data.  It will vary from file to file, but you may find something useful here:
 
 ```python
 {
     'StreamDataV1_0': {
@@ -655,51 +692,128 @@
 }
 ```
 
 </details>
 
 <details>
 
-<summary><code>recorded_data</code></summary>
+<summary><code>events</code></summary>
+
+This property returns the tabular data reported in the `Image Properties >
+Recorded Data` tab of the NIS Viewer.
+
+(There will be a column for each tag in the `CustomDataV2_0` section of
+`custom_data` above, as well as any additional events found in the metadata)
 
-This property returns a `dict` of equal-length sequences.
-It matches the tabular data reported in the `Image Properties > Recorded Data` tab of the NIS Viewer.
+The format of the return type data is controlled by the `orient` argument:
 
-(There will be a column for each tag in the `CustomDataV2_0` section of `custom_data` above.)
+- `'records'` : list of dicts - `[{column -> value}, ...]` (default)
+- `'dict'` :    dict of dicts - `{column -> {index -> value}, ...}`
+- `'list'` :    dict of lists - `{column -> [value, ...]}`
+
+Not every column header appears in every event, so when `orient` is either
+`'dict'` or `'list'`, `float('nan')` will be inserted to maintain a consistent
+length for each column.
 
 ```python
+
+# with `orient='records'` (DEFAULT)
+[
+    {
+        'Time [s]': 1.32686654,
+        'Z-Series': -2.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 552.74,
+        'Ti2 ZDrive [µm]': 552.74
+    },
+    {
+        'Time [s]': 1.69089657,
+        'Z-Series': -1.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 553.74,
+        'Ti2 ZDrive [µm]': 553.74
+    },
+    {
+        'Time [s]': 2.04194662,
+        'Z-Series': 0.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 554.74,
+        'Ti2 ZDrive [µm]': 554.74
+    },
+    {
+        'Time [s]': 2.38194662,
+        'Z-Series': 1.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 555.74,
+        'Ti2 ZDrive [µm]': 555.74
+    },
+    {
+        'Time [s]': 2.63795663,
+        'Z-Series': 2.0,
+        'Exposure Time [ms]': 100.0,
+        'PFS Offset': 0,
+        'PFS Status': 0,
+        'X Coord [µm]': 31452.2,
+        'Y Coord [µm]': -1801.6,
+        'Z Coord [µm]': 556.74,
+        'Ti2 ZDrive [µm]': 556.74
+    }
+]
+
+# with `orient='list'`
+{
+    'Time [s]': array([1.32686654, 1.69089657, 2.04194662, 2.38194662, 2.63795663]),
+    'Z-Series': array([-2., -1.,  0.,  1.,  2.]),
+    'Exposure Time [ms]': array([100., 100., 100., 100., 100.]),
+    'PFS Offset': array([0, 0, 0, 0, 0], dtype=int32),
+    'PFS Status': array([0, 0, 0, 0, 0], dtype=int32),
+    'X Coord [µm]': array([31452.2, 31452.2, 31452.2, 31452.2, 31452.2]),
+    'Y Coord [µm]': array([-1801.6, -1801.6, -1801.6, -1801.6, -1801.6]),
+    'Z Coord [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74]),
+    'Ti2 ZDrive [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74])
+}
+
+# with `orient='dict'`
 {
-    'Time [s]': array([ 1.32686654,  1.69089657,  2.04194662,  2.38194662,  2.63795663,
-        8.7022286 ,  9.03626864,  9.33031869,  9.63934872,  9.90636874,
-       11.48143856, 11.7964786 , 12.0894786 , 12.37153866, 12.66546859]),
-    'Z-Series': array([-2., -1.,  0.,  1.,  2., -2., -1.,  0.,  1.,  2., -2., -1.,  0.,
-        1.,  2.]),
-    'Exposure Time [ms]': array([100., 100., 100., 100., 100., 100., 100., 100., 100., 100., 100.,
-       100., 100., 100., 100.]),
-    'PFS Offset []': array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=int32),
-    'PFS Status []': array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=int32),
-    'X Coord [µm]': array([31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2,
-       31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2, 31452.2,
-       31452.2]),
-    'Y Coord [µm]': array([-1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6,
-       -1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6, -1801.6,
-       -1801.6]),
-    'Z Coord [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74, 552.7 , 553.7 , 554.68,
-       555.7 , 556.64, 552.68, 553.68, 554.68, 555.68, 556.68]),
-    'Ti2 ZDrive [µm]': array([552.74, 553.74, 554.74, 555.74, 556.74, 552.7 , 553.7 , 554.68,
-       555.7 , 556.64, 552.68, 553.68, 554.68, 555.68, 556.68])
+    'Time [s]': {0: 1.32686654, 1: 1.69089657, 2: 2.04194662, 3: 2.38194662, 4: 2.63795663},
+    'Z-Series': {0: -2.0, 1: -1.0, 2: 0.0, 3: 1.0, 4: 2.0},
+    'Exposure Time [ms]': {0: 100.0, 1: 100.0, 2: 100.0, 3: 100.0, 4: 100.0},
+    'PFS Offset []': {0: 0, 1: 0, 2: 0, 3: 0, 4: 0},
+    'PFS Status []': {0: 0, 1: 0, 2: 0, 3: 0, 4: 0},
+    'X Coord [µm]': {0: 31452.2, 1: 31452.2, 2: 31452.2, 3: 31452.2, 4: 31452.2},
+    'Y Coord [µm]': {0: -1801.6, 1: -1801.6, 2: -1801.6, 3: -1801.6, 4: -1801.6},
+    'Z Coord [µm]': {0: 552.74, 1: 553.74, 2: 554.74, 3: 555.74, 4: 556.74},
+    'Ti2 ZDrive [µm]': {0: 552.74, 1: 553.74, 2: 554.74, 3: 555.74, 4: 556.74}
 }
+
+
 ```
 
-You can pass the output of `recorded_data` to `pandas.DataFrame`:
+You can pass the output of `events()` to `pandas.DataFrame`:
 
 ```python
-In [13]: pd.DataFrame(nd2file.recorded_data)
+In [13]: pd.DataFrame(nd2file.events())
 Out[13]:
-     Time [s]  Z-Series  Exposure Time [ms]  PFS Offset []  PFS Status []  X Coord [µm]  Y Coord [µm]  Z Coord [µm]  Ti2 ZDrive [µm]
+     Time [s]  Z-Series  Exposure Time [ms]  PFS Offset  PFS Status []  X Coord [µm]  Y Coord [µm]  Z Coord [µm]  Ti2 ZDrive [µm]
 0    1.326867      -2.0               100.0              0              0       31452.2       -1801.6        552.74           552.74
 1    1.690897      -1.0               100.0              0              0       31452.2       -1801.6        553.74           553.74
 2    2.041947       0.0               100.0              0              0       31452.2       -1801.6        554.74           554.74
 3    2.381947       1.0               100.0              0              0       31452.2       -1801.6        555.74           555.74
 4    2.637957       2.0               100.0              0              0       31452.2       -1801.6        556.74           556.74
 5    8.702229      -2.0               100.0              0              0       31452.2       -1801.6        552.70           552.70
 6    9.036269      -1.0               100.0              0              0       31452.2       -1801.6        553.70           553.70
@@ -712,54 +826,14 @@
 13  12.371539       1.0               100.0              0              0       31452.2       -1801.6        555.68           555.68
 14  12.665469       2.0               100.0              0              0       31452.2       -1801.6        556.68           556.68
 
 ```
 
 </details>
 
-<details>
-
-<summary><code>binary_data</code></summary>
-
-This property returns an `nd2.BinaryLayers` object representing all of the
-binary masks in the nd2 file.
-
-A `nd2.BinaryLayers` object is a sequence of individual `nd2.BinaryLayer`
-objects (one for each binary layer found in the file).  Each `BinaryLayer` in
-the sequence is a named tuple that has, among other things, a `name` attribute,
-and a `data` attribute that is list of numpy arrays (one for each frame in the
-experiment) or `None` if the binary layer had no data in that frame.
-
-The most common use case will be to cast either the entire `BinaryLayers` object
-or an individual `BinaryLayer` to a `numpy.ndarray`:
-
-```python
->>> import nd2
->>> nd2file = nd2.ND2File('path/to/file.nd2')
->>> binary_layers = nd2file.binary_data
-
-# The output array will have shape
-# (n_binary_layers, *coord_shape, *frame_shape).
->>> np.asarray(binary_layers)
-```
-
-For example, if the data in the nd2 file has shape `(nT, nZ, nC, nY, nX)`, and
-there are 4 binary layers, then the output of `np.asarray(nd2file.binary_data)` will
-have shape `(4, nT, nZ, nY, nX)`.  (Note that the `nC` dimension is not present
-in the output array, and the binary layers are always in the first axis).
-
-You can also cast an individual `BinaryLayer` to a numpy array:
-
-```python
->>> binary_layer = binary_layers[0]
->>> np.asarray(binary_layer)
-```
-
-</details>
-
 ## Contributing / Development
 
 To test locally and contribute.  Clone this repo, then:
 
 ```
 pip install -e .[dev]
 ```
```

