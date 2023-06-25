# Comparing `tmp/polyfactory-2.3.3.tar.gz` & `tmp/polyfactory-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.3.3.tar", max compression
+gzip compressed data, was "polyfactory-2.4.0.tar", max compression
```

## Comparing `polyfactory-2.3.3.tar` & `polyfactory-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1092 2023-06-22 17:17:07.017234 polyfactory-2.3.3/LICENSE
--rw-r--r--   0        0        0     9785 2023-06-22 17:17:07.021234 polyfactory-2.3.3/README.md
--rw-r--r--   0        0        0      425 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/__init__.py
--rw-r--r--   0        0        0      825 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    32614 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1897 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2392 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2217 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    11309 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1598 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     8033 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3329 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/py.typed
--rw-r--r--   0        0        0     2891 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3488 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2834 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1880 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-06-22 17:17:07.021234 polyfactory-2.3.3/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13607 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      522 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      529 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      535 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3636 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6186 2023-06-22 17:17:07.025234 polyfactory-2.3.3/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6560 2023-06-22 17:17:07.025234 polyfactory-2.3.3/pyproject.toml
--rw-r--r--   0        0        0    11707 1970-01-01 00:00:00.000000 polyfactory-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-25 17:54:51.308744 polyfactory-2.4.0/LICENSE
+-rw-r--r--   0        0        0    16840 2023-06-25 17:54:51.308744 polyfactory-2.4.0/README.md
+-rw-r--r--   0        0        0      425 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    33164 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1897 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2392 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2217 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    11187 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1598 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     7314 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2919 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3488 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     3113 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13607 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      522 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      529 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      535 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3636 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6186 2023-06-25 17:54:51.312744 polyfactory-2.4.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6554 2023-06-25 17:54:51.312744 polyfactory-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    18762 1970-01-01 00:00:00.000000 polyfactory-2.4.0/PKG-INFO
```

### Comparing `polyfactory-2.3.3/LICENSE` & `polyfactory-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/constants.py` & `polyfactory-2.4.0/polyfactory/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
+
 from collections import abc, defaultdict, deque
 from random import Random
 from typing import (
+    Any,
     DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Iterable,
     List,
     Mapping,
@@ -35,10 +38,10 @@
     abc.Iterable: list,
     abc.Mapping: dict,
     abc.Sequence: list,
     abc.Set: set,
     UnionType: Union,
 }
 
-IGNORED_TYPE_ARGS: Set = {Ellipsis}
+IGNORED_TYPE_ARGS: set[Any] = {Ellipsis}
 
 DEFAULT_RANDOM = Random()
```

### Comparing `polyfactory-2.3.3/polyfactory/decorators.py` & `polyfactory-2.4.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/exceptions.py` & `polyfactory-2.4.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/factories/base.py` & `polyfactory-2.4.0/polyfactory/factories/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
     from polyfactory.field_meta import Constraints, FieldMeta
     from polyfactory.persistence import AsyncPersistenceProtocol, SyncPersistenceProtocol
 
 
-def _create_pydantic_type_map(cls: "type[BaseFactory]") -> dict[type, Callable[[], Any]]:
+def _create_pydantic_type_map(cls: type[BaseFactory[Any]]) -> dict[type, Callable[[], Any]]:
     """Creates a mapping of pydantic types to mock data functions.
 
     :param cls: The base factory class.
     :return: A dict mapping types to callables.
     """
     try:
         import pydantic
@@ -165,15 +165,15 @@
 
     return mapping
 
 
 T = TypeVar("T")
 
 
-def is_factory(value: Any) -> "TypeGuard[type[BaseFactory]]":
+def is_factory(value: Any) -> "TypeGuard[type[BaseFactory[Any]]]":
     """Determine if a given value is a subclass of ModelFactory.
 
     :param value: An arbitrary value.
     :returns: A boolean typeguard.
 
     """
     return isclass(value) and issubclass(value, BaseFactory)
@@ -203,14 +203,20 @@
     If 'True' the factory will be used instead of dynamically generating a factory for the type.
     """
     __is_base_factory__: bool = False
     """
     Flag dictating whether the factory is a 'base' factory. Base factories are registered globally as handlers for types.
     For example, the 'DataclassFactory', 'TypedDictFactory' and 'ModelFactory' are all base factories.
     """
+    __base_factory_overrides__: dict[Any, type[BaseFactory[Any]]] | None = None
+    """
+    A base factory to override with this factory. If this value is set, the given factory will replace the given base factory.
+
+    Note: this value can only be set when '__is_base_factory__' is 'True'.
+    """
     __faker__: ClassVar["Faker"] = Faker()
     """
     A faker instance to use. Can be a user provided value.
     """
     __random__: ClassVar["Random"] = Random()
     """
     An instance of 'random.Random' to use.
@@ -220,16 +226,16 @@
     An integer to seed the factory's Faker and Random instances with.
     This attribute can be used to control random generation.
     """
 
     # cached attributes
     _fields_metadata: list[FieldMeta]
     # BaseFactory only attributes
-    _factory_type_mapping: ClassVar[dict[Any, type["BaseFactory"]]]
-    _base_factories: ClassVar[list[type["BaseFactory"]]]
+    _factory_type_mapping: ClassVar[dict[Any, type[BaseFactory[Any]]]]
+    _base_factories: ClassVar[list[type[BaseFactory[Any]]]]
 
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
         super().__init_subclass__(*args, **kwargs)
 
         if not hasattr(BaseFactory, "_base_factories"):
             BaseFactory._base_factories = []
 
@@ -317,21 +323,26 @@
 
         return field_value
 
     @classmethod
     def _get_or_create_factory(
         cls,
         model: type,
-    ) -> type["BaseFactory"]:
+    ) -> type[BaseFactory[Any]]:
         """Get a factory from registered factories or generate a factory dynamically.
 
         :param model: A model type.
         :returns: A Factory sub-class.
 
         """
+        if cls.__base_factory_overrides__ and (
+            factory := cls.__base_factory_overrides__.get(model, cls.__base_factory_overrides__.get(type(model)))
+        ):
+            return factory.create_factory(model)
+
         if factory := BaseFactory._factory_type_mapping.get(model):
             return factory
 
         for factory in reversed(BaseFactory._base_factories):
             if factory.is_supported_type(model):
                 return factory.create_factory(model)
 
@@ -498,28 +509,28 @@
             f"\n\nEither extend the providers map or add a factory function for this type."
         )
 
     @classmethod
     def create_factory(
         cls,
         model: type,
-        bases: tuple[type["BaseFactory"], ...] | None = None,
+        bases: tuple[type[BaseFactory[Any]], ...] | None = None,
         **kwargs: Any,
-    ) -> type["BaseFactory"]:
+    ) -> type[BaseFactory[Any]]:
         """Generate a factory for the given type dynamically.
 
         :param model: A type to model.
         :param bases: Base classes to use when generating the new class.
         :param kwargs: Any kwargs.
 
         :returns: A 'ModelFactory' subclass.
 
         """
         return cast(
-            "Type[BaseFactory]",
+            "Type[BaseFactory[Any]]",
             type(
                 f"{model.__name__}Factory",
                 (*(bases or ()), cls),
                 {"__model__": model, **kwargs},
             ),
         )
```

### Comparing `polyfactory-2.3.3/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.4.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.4.0/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.4.0/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.4.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.4.0/polyfactory/factories/pydantic_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,23 +98,14 @@
         else:
             constraints = {}
 
         if "url" in constraints:
             # pydantic uses a sentinel value for url constraints
             annotation = str
 
-        constraints = {
-            **constraints,  # type: ignore[misc]
-            "constant": None,
-            "unique_items": None,
-            "upper_case": None,
-            "lower_case": None,
-            "item_type": None,
-        }
-
         return PydanticFieldMeta.from_type(
             name=name,
             random=random,
             annotation=annotation,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
         )
@@ -170,15 +161,23 @@
                 "upper_case": getattr(outer_type, "to_upper", None),
                 "lower_case": getattr(outer_type, "to_lower", None),
                 "item_type": getattr(outer_type, "item_type", None),
             },
         )
 
         # pydantic v1 has constraints set for these values, but we generate them using faker
-        if unwrap_optional(annotation) in (AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn, AmqpDsn, AnyHttpUrl):
+        if pydantic_version == 1 and unwrap_optional(annotation) in (
+            AnyUrl,
+            HttpUrl,
+            KafkaDsn,
+            PostgresDsn,
+            RedisDsn,
+            AmqpDsn,
+            AnyHttpUrl,
+        ):
             constraints = {}
 
         children: list[FieldMeta] = []
         if model_field.key_field:
             children.append(PydanticFieldMeta.from_model_field(model_field.key_field, use_alias))
         if model_field.sub_fields:
             children.extend(
```

### Comparing `polyfactory-2.3.3/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.4.0/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/field_meta.py` & `polyfactory-2.4.0/polyfactory/field_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from dataclasses import asdict, is_dataclass
 from typing import TYPE_CHECKING, Any, Literal, Pattern, TypedDict, cast
 
 from polyfactory.constants import DEFAULT_RANDOM, IGNORED_TYPE_ARGS, TYPE_MAPPING
 from polyfactory.utils.helpers import normalize_annotation, unwrap_annotated, unwrap_args, unwrap_new_type
 from polyfactory.utils.predicates import is_annotated
 
 if TYPE_CHECKING:
@@ -41,15 +42,14 @@
     lt: NotRequired[int | float | Decimal]
     max_digits: NotRequired[int]
     max_length: NotRequired[int]
     min_length: NotRequired[int]
     multiple_of: NotRequired[int | float | Decimal]
     path_type: NotRequired[Literal["file", "dir", "new"]]
     pattern: NotRequired[str | Pattern]
-    strict: NotRequired[bool]
     tz: NotRequired[datetime.tzinfo]
     unique_items: NotRequired[bool]
     upper_case: NotRequired[bool]
     url: NotRequired[UrlConstraints]
     uuid_version: NotRequired[Literal[1, 3, 4, 5]]
 
 
@@ -70,15 +70,15 @@
         *,
         name: str,
         annotation: type,
         random: Random = DEFAULT_RANDOM,
         default: Any = Null,
         children: list[FieldMeta] | None = None,
         constraints: Constraints | None = None,
-    ):
+    ) -> None:
         """Create a factory field metadata instance."""
         self.annotation = annotation
         self.random = random
         self.children = children
         self.default = default
         self.name = name
         self.constraints = constraints
@@ -139,37 +139,22 @@
         for value in metadata:
             if is_annotated(value):
                 _, inner_metadata = unwrap_annotated(value, random=DEFAULT_RANDOM)
                 constraints.update(cast("dict[str, Any]", cls.parse_constraints(metadata=inner_metadata)))
             elif func := getattr(value, "func", None):
                 if func is str.islower:
                     constraints.update({"lower_case": True})
-                if func is str.isupper:
+                elif func is str.isupper:
                     constraints.update({"upper_case": True})
-                if func is str.isascii:
+                elif func is str.isascii:
                     constraints.update({"pattern": "[[:ascii:]]"})
-                if func is str.isdigit:
+                elif func is str.isdigit:
                     constraints.update({"pattern": "[[:digit:]]"})
-            elif allowed_schemas := getattr(value, "allowed_schemas", None):
-                constraints.update(
-                    {
-                        "url": {
-                            k: v
-                            for k, v in {
-                                "max_length": getattr(value, "max_length", None),
-                                "allowed_schemes": allowed_schemas,
-                                "host_required": getattr(value, "host_required", None),
-                                "default_host": getattr(value, "default_host", None),
-                                "default_port": getattr(value, "default_port", None),
-                                "default_path": getattr(value, "default_path", None),
-                            }.items()
-                            if v is not None
-                        }
-                    }
-                )
+            elif is_dataclass(value) and (value_dict := asdict(value)) and ("allowed_schemes" in value_dict):
+                constraints.update({"url": {k: v for k, v in value_dict.items() if v is not None}})
             else:
                 constraints.update(
                     {
                         k: v
                         for k, v in {
                             "allow_inf_nan": getattr(value, "allow_inf_nan", None),
                             "constant": getattr(value, "const", None) is not None,
@@ -182,15 +167,14 @@
                             "lt": getattr(value, "lt", None),
                             "max_digits": getattr(value, "max_digits", None),
                             "max_length": getattr(value, "max_length", getattr(value, "max_length", None)),
                             "min_length": getattr(value, "min_length", getattr(value, "min_items", None)),
                             "multiple_of": getattr(value, "multiple_of", None),
                             "path_type": getattr(value, "path_type", None),
                             "pattern": getattr(value, "regex", getattr(value, "pattern", None)),
-                            "strict": getattr(value, "strict", None),
                             "tz": getattr(value, "tz", None),
                             "unique_items": getattr(value, "unique_items", None),
                             "upper_case": getattr(value, "to_upper", None),
                             "uuid_version": getattr(value, "uuid_version", None),
                         }.items()
                         if v is not None
                     }
```

### Comparing `polyfactory-2.3.3/polyfactory/fields.py` & `polyfactory-2.4.0/polyfactory/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,35 +81,35 @@
         """
         return self.fn["value"](name, values, *self.args, **self.kwargs)
 
 
 class Fixture:
     """Factory field to create a pytest fixture from a factory."""
 
-    __slots__ = ("fixture", "size", "kwargs")
+    __slots__ = ("ref", "size", "kwargs")
 
     def __init__(self, fixture: Callable, size: int | None = None, **kwargs: Any) -> None:
         """Create a fixture from a factory.
 
         :param fixture: A factory that was registered as a fixture.
         :param size: Optional batch size.
         :param kwargs: Any build kwargs.
         """
-        self.fixture: WrappedCallable = {"value": fixture}
+        self.ref: WrappedCallable = {"value": fixture}
         self.size = size
         self.kwargs = kwargs
 
     def to_value(self) -> Any:
         """Call the factory's build or batch method.
 
         :raises: ParameterException
 
         :returns: The build result.
         """
         from polyfactory.pytest_plugin import FactoryFixture
 
-        if factory := FactoryFixture.factory_class_map.get(self.fixture["value"]):
+        if factory := FactoryFixture.factory_class_map.get(self.ref["value"]):
             if self.size:
                 return factory.batch(self.size, **self.kwargs)
             return factory.build(**self.kwargs)
 
         raise ParameterException("fixture has not been registered using the register_factory decorator")
```

### Comparing `polyfactory-2.3.3/polyfactory/persistence.py` & `polyfactory-2.4.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/pytest_plugin.py` & `polyfactory-2.4.0/polyfactory/pytest_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,53 +45,53 @@
 
 
 class FactoryFixture:
     """Decorator that creates a pytest fixture from a factory"""
 
     __slots__ = ("scope", "autouse", "name")
 
-    factory_class_map: ClassVar[dict[Callable, type[BaseFactory]]] = {}
+    factory_class_map: ClassVar[dict[Callable, type[BaseFactory[Any]]]] = {}
 
     def __init__(
         self,
         scope: Scope = "function",
         autouse: bool = False,
         name: str | None = None,
-    ):
+    ) -> None:
         """Create a factory fixture decorator
 
         :param scope: Fixture scope
         :param autouse: Autouse the fixture
         :param name: Fixture name
         """
         self.scope = scope
         self.autouse = autouse
         self.name = name
 
-    def __call__(self, factory: type[BaseFactory]) -> Any:
+    def __call__(self, factory: type[BaseFactory[Any]]) -> Any:
         from polyfactory.factories.base import is_factory
 
         if not is_factory(factory):
             raise ParameterException(f"{factory.__name__} is not a BaseFactory subclass.")
 
         fixture_name = self.name or _get_fixture_name(factory.__name__)
         fixture_register = fixture(scope=self.scope, name=fixture_name, autouse=self.autouse)  # pyright: ignore
 
-        def _factory_fixture() -> type[BaseFactory]:
+        def _factory_fixture() -> type[BaseFactory[Any]]:
             """The wrapped factory"""
             return factory
 
         _factory_fixture.__doc__ = factory.__doc__
         marker = fixture_register(_factory_fixture)
         self.factory_class_map[marker] = factory
         return marker
 
 
 def register_fixture(
-    factory: type[BaseFactory] | None = None,
+    factory: type[BaseFactory[Any]] | None = None,
     *,
     scope: Scope = "function",
     autouse: bool = False,
     name: str | None = None,
 ) -> Any:
     """A decorator that allows registering model factories as fixtures.
```

### Comparing `polyfactory-2.3.3/polyfactory/utils/helpers.py` & `polyfactory-2.4.0/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/utils/predicates.py` & `polyfactory-2.4.0/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/complex_types.py` & `polyfactory-2.4.0/polyfactory/value_generators/complex_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AbstractSet, Any, Collection, MutableMapping, MutableSequence, Set, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    AbstractSet,
+    Any,
+    Collection,
+    MutableMapping,
+    MutableSequence,
+    Set,
+    TypeVar,
+)
 
-from typing_extensions import is_typeddict
+from typing_extensions import get_args, is_typeddict
 
 from polyfactory.utils.helpers import unwrap_annotation
-from polyfactory.utils.predicates import get_type_origin, is_any, is_union
+from polyfactory.utils.predicates import get_type_origin, is_any, is_literal, is_union
 from polyfactory.value_generators.primitives import create_random_string
 
 if TYPE_CHECKING:
     from polyfactory.factories.base import BaseFactory
     from polyfactory.field_meta import FieldMeta
 
 
-def handle_collection_type(field_meta: FieldMeta, container_type: type, factory: type[BaseFactory]) -> Any:
+def handle_collection_type(field_meta: FieldMeta, container_type: type, factory: type[BaseFactory[Any]]) -> Any:
     """Handle generation of container types recursively.
 
     :param container_type: A type that can accept type arguments.
     :param factory: A factory.
     :param field_meta: A field meta instance.
 
     :returns: A built result.
@@ -45,24 +54,29 @@
 
     else:
         raise NotImplementedError(f"Unsupported container type: {container_type}")
 
     return container
 
 
-def handle_complex_type(field_meta: FieldMeta, factory: type[BaseFactory]) -> Any:
+def handle_complex_type(field_meta: FieldMeta, factory: type[BaseFactory[Any]]) -> Any:
     """Recursive type generation based on typing info stored in the graph like structure
     of pydantic field_metas.
 
     :param field_meta: A field meta instance.
     :param factory: A factory.
 
     :returns: A built result.
     """
-    if origin := get_type_origin(unwrap_annotation(field_meta.annotation, random=factory.__random__)):
+    unwrapped_annotation = unwrap_annotation(field_meta.annotation, random=factory.__random__)
+
+    if is_literal(annotation=unwrapped_annotation) and (literal_args := get_args(unwrapped_annotation)):
+        return factory.__random__.choice(literal_args)
+
+    if origin := get_type_origin(unwrapped_annotation):
         if issubclass(origin, Collection):
             return handle_collection_type(field_meta, origin, factory)
         return factory.get_mock_value(origin)
 
     if is_union(field_meta.annotation) and field_meta.children:
         return factory.get_field_value(factory.__random__.choice(field_meta.children))
```

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from polyfactory.field_meta import FieldMeta
 
 T = TypeVar("T", list, set, frozenset)
 
 
 def handle_constrained_collection(
     collection_type: Callable[..., T],
-    factory: type[BaseFactory],
+    factory: type[BaseFactory[Any]],
     field_meta: FieldMeta,
     item_type: Any,
     max_items: int | None = None,
     min_items: int | None = None,
     unique_items: bool = False,
 ) -> T:
     """Generate a constrained list or set.
```

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_path.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_path.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_url.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_url.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/constrained_uuid.py` & `polyfactory-2.4.0/polyfactory/value_generators/constrained_uuid.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/primitives.py` & `polyfactory-2.4.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.3.3/polyfactory/value_generators/regex.py` & `polyfactory-2.4.0/polyfactory/value_generators/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,11 +140,11 @@
             return self._random.choice(candidates)
         return self._random.choice(candidates)
 
     def _handle_repeat(self, start_range: int, end_range: Any, value: SubPattern) -> str:
         result: list[str] = []
         end_range = min(end_range, self._limit)
 
-        for i in range(self._random.randint(start_range, max(start_range, end_range))):
-            result.append("".join(self._handle_state(i) for i in list(value)))  # pyright:ignore
+        for _ in range(self._random.randint(start_range, max(start_range, end_range))):
+            result.append("".join(self._handle_state(v) for v in list(value)))  # pyright:ignore
 
         return "".join(result)
```

### Comparing `polyfactory-2.3.3/pyproject.toml` & `polyfactory-2.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.3.3"
+version = "2.4.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -79,15 +79,15 @@
 msgspec = "*"
 odmantic = "*"
 pre-commit = "*"
 pydantic = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
-annotated-types = ">=0.5.0"
+annotated-types = "*"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = "*"
 blacken-docs = "*"
 auto-pytabs = "*"
 sphinxcontrib-mermaid = "*"
 sphinx-copybutton = "*"
```

