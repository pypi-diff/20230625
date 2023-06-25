# Comparing `tmp/fast_depends-2.0.4.tar.gz` & `tmp/fast_depends-2.0.5.tar.gz`

## Comparing `fast_depends-2.0.4.tar` & `fast_depends-2.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/_compat.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/use.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/core/build.py
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.4/LICENSE
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fast_depends-2.0.4/README.md
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 fast_depends-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/_compat.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/use.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/core/build.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.5/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.5/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.5/LICENSE
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fast_depends-2.0.5/README.md
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 fast_depends-2.0.5/PKG-INFO
```

### Comparing `fast_depends-2.0.4/CONTRIBUTING.md` & `fast_depends-2.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/.github/workflows/documentation.yml` & `fast_depends-2.0.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/.github/workflows/publish_coverage.yml` & `fast_depends-2.0.5/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/.github/workflows/publish_pypi.yml` & `fast_depends-2.0.5/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/.github/workflows/tests.yml` & `fast_depends-2.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/fast_depends/_compat.py` & `fast_depends-2.0.5/fast_depends/_compat.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/fast_depends/use.py` & `fast_depends-2.0.5/fast_depends/use.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import AsyncExitStack, ExitStack
 from functools import wraps
-from typing import Any, Awaitable, Callable, Optional, Sequence, Union
+from typing import Any, Awaitable, Callable, Optional, Sequence, Union, overload
 
 from typing_extensions import ParamSpec, TypeVar
 
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.dependencies import dependency_provider, model
 
 P = ParamSpec("P")
@@ -23,26 +23,51 @@
     return model.Depends(
         dependency=dependency,
         use_cache=use_cache,
         cast=cast,
     )
 
 
+@overload
+def inject(  # pragma: no covers
+    func: None,
+    *,
+    dependency_overrides_provider: Optional[Any] = dependency_provider,
+    extra_dependencies: Sequence[model.Depends] = (),
+    wrap_model: Callable[[CallModel[P, T]], CallModel[P, T]] = lambda x: x,
+) -> Callable[
+    [Union[Callable[P, T], Callable[P, Awaitable[T]]]],
+    Union[Callable[P, T], Callable[P, Awaitable[T]]],
+]:
+    ...
+
+
+@overload
+def inject(  # pragma: no covers
+    func: Callable[P, T],
+    *,
+    dependency_overrides_provider: Optional[Any] = dependency_provider,
+    extra_dependencies: Sequence[model.Depends] = (),
+    wrap_model: Callable[[CallModel[P, T]], CallModel[P, T]] = lambda x: x,
+) -> Callable[P, T]:
+    ...
+
+
 def inject(
     func: Optional[Union[Callable[P, T], Callable[P, Awaitable[T]]]] = None,
     *,
     dependency_overrides_provider: Optional[Any] = dependency_provider,
     extra_dependencies: Sequence[model.Depends] = (),
     wrap_model: Callable[[CallModel[P, T]], CallModel[P, T]] = lambda x: x,
 ) -> Union[
+    Union[Callable[P, T], Callable[P, Awaitable[T]]],
     Callable[
         [Union[Callable[P, T], Callable[P, Awaitable[T]]]],
         Union[Callable[P, T], Callable[P, Awaitable[T]]],
     ],
-    Union[Callable[P, T], Callable[P, Awaitable[T]]],
 ]:
     decorator = _wrap_inject(
         dependency_overrides_provider=dependency_overrides_provider,
         wrap_model=wrap_model,
         extra_dependencies=extra_dependencies,
     )
 
@@ -107,10 +132,10 @@
                         stack=stack,
                         dependency_overrides=overrides,
                         cache_dependencies={},
                         **kwargs,
                     )
                 return r
 
-        return wraps(func)(injected_wrapper)
+        return injected_wrapper
 
     return func_wrapper
```

### Comparing `fast_depends-2.0.4/fast_depends/utils.py` & `fast_depends-2.0.5/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/fast_depends/core/build.py` & `fast_depends-2.0.5/fast_depends/core/build.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/fast_depends/core/model.py` & `fast_depends-2.0.5/fast_depends/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     ]
     is_async: bool
     is_generator: bool
     model: Type[BaseModel]
     response_model: Optional[Type[BaseModel]]
 
     params: Dict[str, FieldInfo]
-    flat_params: Dict[str, FieldInfo]
     alias_arguments: List[str]
 
     dependencies: Dict[str, "CallModel[..., Any]"]
     extra_dependencies: Iterable["CallModel[..., Any]"]
     custom_fields: Dict[str, CustomField]
 
     # Dependencies and custom fields
@@ -87,15 +86,15 @@
         custom_fields: Optional[Dict[str, CustomField]] = None,
     ):
         self.call = call
         self.model = model
         self.response_model = response_model
 
         fields: Dict[str, FieldInfo]
-        if PYDANTIC_V2:  # pragma: no cover
+        if PYDANTIC_V2:
             fields = self.model.model_fields  # type: ignore
         else:
             fields = self.model.__fields__  # type: ignore
 
         self.dependencies = dependencies or {}
         self.extra_dependencies = extra_dependencies or []
         self.custom_fields = custom_fields or {}
```

### Comparing `fast_depends-2.0.4/fast_depends/dependencies/model.py` & `fast_depends-2.0.5/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/fast_depends/library/model.py` & `fast_depends-2.0.5/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/LICENSE` & `fast_depends-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/README.md` & `fast_depends-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/pyproject.toml` & `fast_depends-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.4/PKG-INFO` & `fast_depends-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.0.4
+Version: 2.0.5
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

