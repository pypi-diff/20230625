# Comparing `tmp/stormlibpp-0.1.2.tar.gz` & `tmp/stormlibpp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormlibpp-0.1.2.tar", last modified: Sun Jun 25 16:32:57 2023, max compression
+gzip compressed data, was "stormlibpp-0.2.0.tar", last modified: Sun Jun 25 18:52:44 2023, max compression
```

## Comparing `stormlibpp-0.1.2.tar` & `stormlibpp-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.509036 stormlibpp-0.1.2/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.1.2/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 16:32:57.508900 stormlibpp-0.1.2/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.1.2/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-25 16:32:52.000000 stormlibpp-0.1.2/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-25 16:32:57.509079 stormlibpp-0.1.2/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.506551 stormlibpp-0.1.2/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.507672 stormlibpp-0.1.2/src/stormlibpp/
--rw-r--r--   0 gormo      (501) staff       (20)      604 2023-06-25 16:32:52.000000 stormlibpp-0.1.2/src/stormlibpp/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)      663 2023-06-25 16:25:46.000000 stormlibpp-0.1.2/src/stormlibpp/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)     8097 2023-06-25 16:31:12.000000 stormlibpp-0.1.2/src/stormlibpp/stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)     1289 2023-06-24 18:47:22.000000 stormlibpp-0.1.2/src/stormlibpp/telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)     1465 2023-06-25 16:27:18.000000 stormlibpp-0.1.2/src/stormlibpp/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.508291 stormlibpp-0.1.2/src/stormlibpp.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      417 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-25 16:32:57.000000 stormlibpp-0.1.2/src/stormlibpp.egg-info/top_level.txt
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 16:32:57.508690 stormlibpp-0.1.2/tests/
--rw-r--r--   0 gormo      (501) staff       (20)     1644 2023-06-25 16:20:13.000000 stormlibpp-0.1.2/tests/test_stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)      481 2023-06-24 18:47:22.000000 stormlibpp-0.1.2/tests/test_telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.916409 stormlibpp-0.2.0/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.2.0/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 18:52:44.916290 stormlibpp-0.2.0/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.2.0/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-25 18:52:40.000000 stormlibpp-0.2.0/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-25 18:52:44.916448 stormlibpp-0.2.0/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.913888 stormlibpp-0.2.0/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.915045 stormlibpp-0.2.0/src/stormlibpp/
+-rw-r--r--   0 gormo      (501) staff       (20)     1419 2023-06-25 18:52:40.000000 stormlibpp-0.2.0/src/stormlibpp/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)      663 2023-06-25 16:40:51.000000 stormlibpp-0.2.0/src/stormlibpp/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)      507 2023-06-25 18:48:29.000000 stormlibpp-0.2.0/src/stormlibpp/node.py
+-rw-r--r--   0 gormo      (501) staff       (20)     9151 2023-06-25 18:31:41.000000 stormlibpp-0.2.0/src/stormlibpp/stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1396 2023-06-25 16:42:23.000000 stormlibpp-0.2.0/src/stormlibpp/telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1507 2023-06-25 18:15:47.000000 stormlibpp-0.2.0/src/stormlibpp/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.915749 stormlibpp-0.2.0/src/stormlibpp.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      440 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.916118 stormlibpp-0.2.0/tests/
+-rw-r--r--   0 gormo      (501) staff       (20)     1699 2023-06-25 18:37:46.000000 stormlibpp-0.2.0/tests/test_stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)      720 2023-06-25 16:42:23.000000 stormlibpp-0.2.0/tests/test_telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.2.0/tests/test_utils.py
```

### Comparing `stormlibpp-0.1.2/LICENSE` & `stormlibpp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.1.2/PKG-INFO` & `stormlibpp-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.1.2
+Version: 0.2.0
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.1.2/pyproject.toml` & `stormlibpp-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stormlibpp"
-version = "0.1.2"
+version = "0.2.0"
 description = "The stormlibpp Python package"
 readme = "README.md"
 requires-python = ">=3.11"
 
 # Fill in dependencies here.
 dependencies = [
     "synapse==2.139.0"
```

### Comparing `stormlibpp-0.1.2/src/stormlibpp/errors.py` & `stormlibpp-0.2.0/src/stormlibpp/errors.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.1.2/src/stormlibpp/stormpkg.py` & `stormlibpp-0.2.0/src/stormlibpp/stormpkg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Python objects for working with Storm Packages."""
 
 
 import json
 import os
 import sys
 
+import synapse.common as s_common
+import synapse.exc as s_exc
+import synapse.tools.genpkg as s_genpkg
+
 from . import errors
-from . import s_common, s_exc, s_genpkg
 from . import utils
 
 
 class StormPkg:
     """A Python representation of a Storm package, proto and definition.
 
     This class must be subclassed - this is how default proto dir loading is supported.
@@ -46,67 +49,80 @@
           is set to a ``dict``.
 
     - Sets the loaded package definition's ``build`` key to a ``dict``
       containing the time using ``synapse.common.now``.
 
     - Stores the package definition ``dict`` in the ``pkdef`` property.
 
+    - If ``check_syntax`` is True, all Storm code that is loaded in the ``pkdef``
+      is passed to Synapse's Storm parser to check for Storm syntax errors.
+      Any errors are raised as a ``StormPkgSyntaxError`` exception.
+
     Parameters
     ----------
     check_syntax : bool, optional
         Whether to check the syntax of this package's loaded Storm code.
         By default True.
     proto_dir : str | None, optional
         The fully resolved directory that the package proto is in. A value
         of ``None`` tells ``StormPkg`` to resolve this path automatically based
         on the rules defined elsewhere in this docstring. By default None.
 
     Properties
     ----------
+    default_name : str
+        The Yaml basename used if ``proto_name`` is empty (not set).
+        Set to the value of ``self.__class__.__name__.lower()``.
     pkgdef : dict
         The loaded Storm package definition.
     proto_dir : str
         The directory that the Storm package's proto is in. This is
         the ``proto_dir`` argument if it is passed. Otherwise, the dir
         is resolved by looking at the ``self.__class__.__module__`` name
         at init, finding the object this resolves to in ``sys.modules``,
         and reading the module's ``__file__``. Then joining this file's
         dir name with the value ``pkgproto``.
-    proto_name : str | None
+    proto_name : str
         A class property containing the name of the Storm package's proto
         Yaml file (without extension). Subclasses may override this class
         property to set a custom proto Yaml file basename. If they don't,
-        this property is automatically set to the value of
-        ``self.__class__.__name__.lower()``.
+        this property is automatically set to the value of ``self.default_name``.
 
     Raises
     ------
     StormPkgBadDefError
         If the package proto either has an invalid schema or bad value.
     StormPkgNoProtoError
         If the proto Yaml file cannot be loaded. This can happen if the file name
-        will not match ``name``/``pkg_name`` but ``proto_name`` is not passed.
+        will not match ``self.default_name`` but ``proto_name`` is not set.
     StormPkgResolveError
         If the default package proto dir cannot be resolved. This can be the case
         if a `StormPkg` is created and doesn't expect to use the default proto dir
         but a custom ``proto_dir`` is not passed.
+    StormPkgSyntaxError
+        If ``check_syntax`` is True and the Storm code in this package has syntax errors.
     RuntimeError
         If this class is instantiated directly and not subclassed.
     """
 
     proto_name: str | None = None
+    """The basename of this Storm package's Yaml proto file."""
 
     def __init__(
         self,
         check_syntax: bool = True,
         proto_dir: str | None = None,
     ) -> None:
         if StormPkg not in self.__class__.__bases__:
             raise RuntimeError("StormPkg must be subclassed.")
 
+        self.default_name = self.__class__.__name__.lower()
+        if not self.proto_name:
+            self.proto_name = self.default_name
+
         if proto_dir:
             self.proto_dir = proto_dir
         else:
             try:
                 resolved_path = sys.modules[self.__class__.__module__].__file__
             except AttributeError as err:
                 raise errors.StormPkgResolveError(
@@ -115,18 +131,18 @@
                 ) from err
 
             self.proto_dir = utils.absjoin(
                 os.path.dirname(resolved_path),
                 "pkgproto",
             )
 
-        if not self.proto_name:
-            self.proto_name = self.__class__.__name__.lower()
-
-        self.proto = os.path.join(self.proto_dir, f"{self.proto_name}.yaml",)
+        self.proto = os.path.join(
+            self.proto_dir,
+            f"{self.proto_name}.yaml",
+        )
 
         self.pkgdef = self._load_proto()
         """A Python dict containing the full Storm package definition."""
 
         if check_syntax:
             self.check_syntax()
 
@@ -152,23 +168,14 @@
                 "The specified package proto was invalid."
             ) from err
 
         pkgdef["build"] = {"time": s_common.now()}
 
         return pkgdef
 
-    def _search_def(self, primkey: str, seckey: str) -> list[str]:
-        """Search the modules or commands of the pkgdef for a secondary key."""
-
-        vals = []
-        for val in self.pkgdef.get(primkey, []):
-            if seckey in val:
-                vals.append(val[seckey])
-        return vals
-
     def asdict(self):
         """Return this objects full Storm package definition as a Python dict.
 
         Pointer to ``self.pkgdef``.
         """
 
         return self.pkgdef
@@ -189,34 +196,61 @@
                 utils.chk_storm_syntax(code)
             except errors.StormSyntaxError as err:
                 raise errors.StormPkgSyntaxError(
                     f"{stormname} from {self.proto_name}.yaml has a Storm "
                     f"syntax error: {err}"
                 ) from err
 
-    def cmds(self) -> list[str]:
-        """The commands this package defines."""
+    def cmds(self) -> list[dict]:
+        """The full definitions of the commands this package defines."""
 
-        return self._search_def("commands", "name")
+        return self.pkgdef.get("commands", [])
 
-    def mods(self) -> list[str]:
-        """The modules this package defines."""
+    def mods(self) -> list[dict]:
+        """The full definitions of the modules this package defines."""
 
-        return self._search_def("modules", "name")
+        return self.pkgdef.get("modules", [])
 
     def storm(self) -> dict[str, str]:
         """The Storm code this package defines.
-        
+
         Returns
         -------
         dict[str, str]
             Keys are the module/command name and values are the Storm code.
         """
 
         storm = {}
-        for mod in self.pkgdef.get("modules", []):
-            if "name" in mod and "storm" in mod:
-                storm[mod["name"]] = mod["storm"]
-        for cmd in self.pkgdef.get("commands", []):
-            if "name" in cmd and "storm" in cmd:
-                storm[cmd["name"]] = cmd["storm"]
+        for item in self.cmds() + self.mods():
+            if "name" in item and "storm" in item:
+                storm[item["name"]] = item["storm"]
         return storm
+
+    @property
+    def cmdnames(self) -> list[str]:
+        """The names of the commands this package defines, if any."""
+
+        return [cmd.get("name") for cmd in self.cmds() if "name" in cmd]
+
+    @property
+    def modnames(self) -> list[str]:
+        """The names of the modules this package defines, if any."""
+
+        return [mod.get("name") for mod in self.mods() if "name" in mod]
+
+    @property
+    def pkg_guid(self) -> str:
+        """The package's guid, None if not set."""
+
+        return self.pkgdef.get("guid")
+
+    @property
+    def pkg_name(self) -> str:
+        """The package's name, None if not set."""
+
+        return self.pkgdef.get("name")
+
+    @property
+    def pkg_ver(self) -> str:
+        """The package's version, None if not set."""
+
+        return self.pkgdef.get("version")
```

### Comparing `stormlibpp-0.1.2/src/stormlibpp/telepath.py` & `stormlibpp-0.2.0/src/stormlibpp/telepath.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,7 +32,12 @@
     """Generate a default TelepathRetn return object, or the given subclass.
 
     Default values have a ``status`` of ``True``, an empty ``mesg``, and
     ``data`` is set to the ``default_data`` arg - which defaults to ``None``.
     """
 
     return obj(status=True, mesg="", data=default_data)
+
+
+class BoolRetn(TelepathRetn):
+    """A TelepathRetn where ``data`` is a boolean value."""
+    data: bool
```

### Comparing `stormlibpp-0.1.2/src/stormlibpp/utils.py` & `stormlibpp-0.2.0/src/stormlibpp/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Miscellaneous functions that are helpful for working with Storm/Synapse."""
 
 
 import os
 
+import synapse.exc as s_exc
+import synapse.lib.parser as s_parser
+
 from . import errors
-from . import s_exc, s_parser
 
 
 def absjoin(*paths: str) -> str:
     """Join paths with os.path.join and then pass it to os.path.abspath.
 
     Parameters
     ----------
-    *paths : str
+    paths : list[str]
         The path strings to join together, as would be passed to ``os.path.join``.
 
     Returns
     -------
     str
         The absolute path derived from the joined ``paths``.
     """
```

### Comparing `stormlibpp-0.1.2/src/stormlibpp.egg-info/PKG-INFO` & `stormlibpp-0.2.0/src/stormlibpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.1.2
+Version: 0.2.0
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.1.2/tests/test_stormpkg.py` & `stormlibpp-0.2.0/tests/test_stormpkg.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,20 +43,21 @@
             pass
 
         test = Test()
         othertest = OtherTest()
 
         assert isinstance(test.asdict(), dict)
         assert isinstance(othertest.pkgdef, dict)
+        assert "othertest.lib" in othertest.modnames
 
     def test_storm_parse(self):
         class BadStorm(stormlibpp.StormPkg):
             pass
 
         with pytest.raises(stormlibpp.errors.StormPkgSyntaxError):
             BadStorm()
 
     def test_storm_parse_disable(self):
         class BadStorm(stormlibpp.StormPkg):
             pass
 
-        assert "badstorm" in BadStorm(check_syntax=False).cmds()
+        assert "badstorm" in BadStorm(check_syntax=False).cmdnames
```

