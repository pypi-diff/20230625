# Comparing `tmp/objectory-0.0.2.tar.gz` & `tmp/objectory-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectory-0.0.2.tar", max compression
+gzip compressed data, was "objectory-0.0.3.tar", max compression
```

## Comparing `objectory-0.0.2.tar` & `objectory-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1501 2023-04-15 03:59:42.869678 objectory-0.0.2/LICENSE
--rw-r--r--   0        0        0     3948 2023-04-15 03:59:42.869678 objectory-0.0.2/README.md
--rw-r--r--   0        0        0     3888 2023-04-15 03:59:42.869678 objectory-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/__init__.py
--rw-r--r--   0        0        0    12973 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/abstract_factory.py
--rw-r--r--   0        0        0      138 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/constants.py
--rw-r--r--   0        0        0     1471 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/errors.py
--rw-r--r--   0        0        0    16025 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/registry.py
--rw-r--r--   0        0        0     1255 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/universal.py
--rw-r--r--   0        0        0      373 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/utils/__init__.py
--rw-r--r--   0        0        0     3185 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/utils/name_resolution.py
--rw-r--r--   0        0        0     7397 2023-04-15 03:59:42.869678 objectory-0.0.2/src/objectory/utils/object_helpers.py
--rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 objectory-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-06-25 05:56:41.507082 objectory-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4516 2023-06-25 05:56:41.507082 objectory-0.0.3/README.md
+-rw-r--r--   0        0        0     3829 2023-06-25 05:56:41.511082 objectory-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/__init__.py
+-rw-r--r--   0        0        0    13109 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/abstract_factory.py
+-rw-r--r--   0        0        0      138 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/constants.py
+-rw-r--r--   0        0        0     1511 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/errors.py
+-rw-r--r--   0        0        0    16099 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/registry.py
+-rw-r--r--   0        0        0     1290 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/universal.py
+-rw-r--r--   0        0        0      373 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/utils/__init__.py
+-rw-r--r--   0        0        0     3192 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/utils/name_resolution.py
+-rw-r--r--   0        0        0     7469 2023-06-25 05:56:41.511082 objectory-0.0.3/src/objectory/utils/object_helpers.py
+-rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 objectory-0.0.3/PKG-INFO
```

### Comparing `objectory-0.0.2/LICENSE` & `objectory-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `objectory-0.0.2/README.md` & `objectory-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 # objectory = object + factory
 
 <p align="center">
     <a href="https://github.com/durandtibo/objectory/actions">
         <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/CI/badge.svg?event=push&branch=main">
     </a>
+    <a href="https://durandtibo.github.io/objectory/">
+        <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/Documentation/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/objectory">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/objectory/maintainability">
+        <img src="https://api.codeclimate.com/v1/badges/1fad6e22f2d38335c26d/maintainability" />
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/objectory/test_coverage">
+        <img src="https://api.codeclimate.com/v1/badges/1fad6e22f2d38335c26d/test_coverage" />
+    </a>
+    <br/>
     <a href="https://pypi.org/project/objectory/">
         <img alt="PYPI version" src="https://img.shields.io/pypi/v/objectory">
     </a>
     <a href="https://pypi.org/project/objectory/">
         <img alt="Python" src="https://img.shields.io/pypi/pyversions/objectory.svg">
     </a>
     <a href="https://opensource.org/licenses/BSD-3-Clause">
         <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/objectory">
     </a>
-    <a href="https://codecov.io/gh/durandtibo/objectory">
-        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
-    </a>
     <a href="https://github.com/psf/black">
         <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
     </a>
     <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
         <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
     </a>
     <br/>
@@ -30,15 +40,15 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/objectory/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-A light Python library for general purpose object factories.
+A Python library for general purpose object factories.
 In particular, it focuses on dynamic object factory implementations where objects can be registered
 dynamically without changing the code of the factory.
 An object factory can be used to instantiate an object from its configuration.
 The current implementation contains both abstract factory and registry approaches.
 
 **factory**
```

### Comparing `objectory-0.0.2/pyproject.toml` & `objectory-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "objectory"
-version = "0.0.2"
+version = "0.0.3"
 description = "A light library for general purpose object factories"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/objectory"
 repository = "https://github.com/durandtibo/objectory"
 keywords = ["factory", "abstract factory", "registry"]
 license = "BSD-3-Clause"
@@ -29,26 +29,26 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 tornado = "^6.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1"
-mkdocstrings = "^0.21"
+mkdocstrings = "^0.22"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3"
-coverage = { extras = ["toml"], version = "^6.5" }
-docformatter = "^1.5"
-pre-commit = "^2.20"
+coverage = { extras = ["toml"], version = "^7.2" }
+docformatter = { extras = ["tomli"], version = "^1.7" }
+pre-commit = "^3.3"
 pylint = "^2.17"
-pytest = "^7.3"
-pytest-cov = "^4.0"
+pytest = "^7.4"
+pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = "^0.0.261"
+ruff = ">=0.0.275,<1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
@@ -149,11 +149,7 @@
 [tool.ruff.pycodestyle]
 max-doc-length = 72
 
 [tool.ruff.isort]
 force-sort-within-sections = true
 combine-as-imports = true
 known-first-party = ["src"]
-
-[tool.ruff.flake8-import-conventions]
-[tool.ruff.flake8-import-conventions.aliases]
-numpy = "np"
```

### Comparing `objectory-0.0.2/src/objectory/abstract_factory.py` & `objectory-0.0.3/src/objectory/abstract_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 r"""This module implements the ``AbstractFactory`` metaclass used to create
 factories."""
 
+from __future__ import annotations
+
 __all__ = ["AbstractFactory", "is_abstract_factory", "register", "register_child_classes"]
 
 import inspect
 import logging
 from abc import ABCMeta
 from collections.abc import Callable
-from typing import Any, Optional, Union
+from typing import Any
 
 from objectory.errors import (
     AbstractFactoryTypeError,
     IncorrectObjectFactoryError,
     UnregisteredObjectFactoryError,
 )
 from objectory.utils import (
@@ -86,31 +88,33 @@
             ``AbstractClassAbstractFactoryError``: if you try to
                 instantiate an abstract class.
             ``UnregisteredClassAbstractFactoryError``: if the target
                 is not found.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import AbstractFactory
             >>> class BaseClass(metaclass=AbstractFactory):
             ...     pass
+            ...
             >>> class MyClass(BaseClass):
             ...     pass
+            ...
             >>> BaseClass.factory("MyClass")
             <__main__.MyClass object at 0x123456789>
         """
         return instantiate_object(
             cls._abstractfactory_get_target_from_name(_target_), *args, _init_=_init_, **kwargs
         )
 
-    def register_object(cls, obj: Union[type, Callable]) -> None:
-        r"""Registers a class or function to the factory. It is useful if you
-        are using a 3rd party library.
+    def register_object(cls, obj: type | Callable) -> None:
+        r"""Registers a class or function to the factory. It is useful if
+        you are using a 3rd party library.
 
         For example, you use a 3rd party library, and you cannot
         modify the classes to add ``AbstractFactory``. You can use
         this function to register some classes or functions of a
         3rd party library.
 
         Args:
@@ -119,21 +123,23 @@
 
         Raises:
             ``IncorrectObjectAbstractFactoryError``: if the object
                 is not a class.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import AbstractFactory
             >>> class BaseClass(metaclass=AbstractFactory):
             ...     pass
+            ...
             >>> class MyClass:
             ...     pass
+            ...
             >>> BaseClass.register_object(MyClass)
             >>> BaseClass.inheritors
             {'__main__.BaseClass': <class '__main__.BaseClass'>,
              '__main__.MyClass': <class '__main__.MyClass'>}
         """
         cls._abstractfactory_check_object(obj)
         name = full_object_name(obj)
@@ -153,34 +159,36 @@
         Args:
             name (string): Specifies the name of the object to remove.
                 This function uses the name resolution mechanism to
                 find the full name if only the short name is given.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import AbstractFactory
             >>> class BaseClass(metaclass=AbstractFactory):
             ...     pass
+            ...
             >>> class MyClass:
             ...     pass
+            ...
             >>> BaseClass.register_object(MyClass)
             >>> BaseClass.unregister("MyClass")
             >>> BaseClass.inheritors
             {'__main__.BaseClass': <class '__main__.BaseClass'>}
         """
         resolved_name = cls._abstractfactory_resolve_name(name)
         if resolved_name is None or not cls._abstractfactory_is_name_registered(resolved_name):
             raise UnregisteredObjectFactoryError(
                 f"It is not possible to remove an object which is not registered (received: {name})"
             )
         cls._abstractfactory_inheritors.pop(resolved_name)
 
-    def _abstractfactory_get_target_from_name(cls, name: str) -> Union[type, Callable]:
+    def _abstractfactory_get_target_from_name(cls, name: str) -> type | Callable:
         """Gets the class or function to used given its name.
 
         Args:
             name (str): Specifies the name of the class or function.
 
         Returns:
             The class or function.
@@ -195,15 +203,15 @@
                 f"Unable to create the object {name}. Registered objects of {cls.__qualname__} "
                 f"are {set(cls._abstractfactory_inheritors.keys())}"
             )
         if not cls._abstractfactory_is_name_registered(resolved_name):
             cls.register_object(import_object(resolved_name))
         return cls._abstractfactory_inheritors[resolved_name]
 
-    def _abstractfactory_resolve_name(cls, name: str) -> Optional[str]:
+    def _abstractfactory_resolve_name(cls, name: str) -> str | None:
         r"""Tries to resolve the name.
 
         This function will look at if it can find an object which
         match with the given name. It is quite useful because there
         are several ways to load an object but only one can be
         registered. If you specify a full name (module path +
         class/function name), it will try to import the module
@@ -228,16 +236,16 @@
 
         Returns:
             bool: ``True`` if the name exists otherwise ``False``.
         """
         return name in cls._abstractfactory_inheritors
 
     def _abstractfactory_check_object(cls, obj: type) -> None:
-        r"""Checks if the object is valid for this factory before to register
-        it.
+        r"""Checks if the object is valid for this factory before to
+        register it.
 
         This function will raise an exception if the object is not
         valid.
 
         Args:
             obj: Specifies the object to check.
 
@@ -264,35 +272,37 @@
 
     Args:
         cls (``AbstractFactory``): Specifies the class where to
             register the function.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.abstract_factory import AbstractFactory, register
         >>> class BaseClass(metaclass=AbstractFactory):
         ...     pass
+        ...
         >>> @register(BaseClass)
         ... def function_to_register(value: int) -> int:
         ...     return value + 2
-        >>> BaseClass.factory('function_to_register', 40)
+        ...
+        >>> BaseClass.factory("function_to_register", 40)
         42
     """
 
     def wrapped(func: Callable) -> Callable:
         cls.register_object(func)
         return func
 
     return wrapped
 
 
 def register_child_classes(
-    factory_cls: Union[AbstractFactory, type], cls: type, ignore_abstract_class: bool = True
+    factory_cls: AbstractFactory | type, cls: type, ignore_abstract_class: bool = True
 ) -> None:
     r"""Registers the given class and its child classes of a given class.
 
     This function registers all the child classes including the child
     classes of the child classes, etc.
 
     Args:
@@ -305,19 +315,20 @@
 
     Raises:
         ``AbstractFactoryTypeError`` if the factory class does not
             implement the ``AbstractFactory`` metaclass.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.abstract_factory import AbstractFactory, register_child_classes
         >>> class BaseClass(metaclass=AbstractFactory):
-        >>>     pass
+        ...     pass
+        ...
         >>> register_child_classes(BaseClass, dict)
         {'__main__.BaseClass': <class '__main__.BaseClass'>,
          'builtins.dict': <class 'dict'>,
          'collections.Counter': <class 'collections.Counter'>,
          'collections.defaultdict': <class 'collections.defaultdict'>,
          'tornado.util.ObjectDict': <class 'tornado.util.ObjectDict'>,
          'collections.OrderedDict': <class 'collections.OrderedDict'>,
@@ -343,18 +354,19 @@
 
     Returns:
         bool: ``True`` if the class implements the ``AbstractFactory``
             metaclass, otherwise ``False``.
 
         Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.abstract_factory import AbstractFactory, is_abstract_factory
         >>> class BaseClass(metaclass=AbstractFactory):
-        >>>     pass
+        ...     pass
+        ...
         >>> is_abstract_factory(BaseClass)
         True
         >>> is_abstract_factory(int)
         False
     """
     return isinstance(cls, AbstractFactory)
```

### Comparing `objectory-0.0.2/src/objectory/errors.py` & `objectory-0.0.3/src/objectory/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-r"""This module defines the main errors of the object factory package."""
+r"""This module defines the main errors of the object factory
+package."""
+
+from __future__ import annotations
 
 __all__ = [
     "AbstractClassFactoryError",
     "AbstractFactoryTypeError",
     "FactoryError",
     "IncorrectObjectFactoryError",
     "InvalidAttributeRegistryError",
@@ -12,30 +15,31 @@
 
 
 class FactoryError(Exception):
     r"""This exception can be used to catch all the factory errors."""
 
 
 class UnregisteredObjectFactoryError(FactoryError):
-    r"""This error is raised when you try to initialize or unregister an object
-    which is not registered to the factory."""
+    r"""This error is raised when you try to initialize or unregister an
+    object which is not registered to the factory."""
 
 
 class IncorrectObjectFactoryError(FactoryError):
-    r"""This error is raised when you try to register an object which cannot be
-    registered."""
+    r"""This error is raised when you try to register an object which
+    cannot be registered."""
 
 
 class AbstractClassFactoryError(FactoryError):
-    r"""This error is raised when you try to initialize an abstract class."""
+    r"""This error is raised when you try to initialize an abstract
+    class."""
 
 
 class InvalidNameFactoryError(FactoryError):
-    r"""This error is raised when you try to use an invalid name to register an
-    object to a factory."""
+    r"""This error is raised when you try to use an invalid name to
+    register an object to a factory."""
 
 
 ###########################
 #     AbstractFactory     #
 ###########################
 
 
@@ -46,9 +50,9 @@
 
 ####################
 #     Registry     #
 ####################
 
 
 class InvalidAttributeRegistryError(FactoryError):
-    r"""This error is raised when you try to access a non Registry object in
-    the registry."""
+    r"""This error is raised when you try to access a non Registry
+    object in the registry."""
```

### Comparing `objectory-0.0.2/src/objectory/registry.py` & `objectory-0.0.3/src/objectory/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 r"""This module implements a registry class."""
 
+from __future__ import annotations
+
 __all__ = ["Registry"]
 
 import inspect
 import logging
-from typing import Any, Callable, Optional, TypeVar, Union
+from typing import Any, Callable, TypeVar
 
 from objectory.errors import (
     IncorrectObjectFactoryError,
     InvalidAttributeRegistryError,
     InvalidNameFactoryError,
     UnregisteredObjectFactoryError,
 )
@@ -35,15 +37,15 @@
 
     _CLASS_FILTER = "class_filter"
 
     def __init__(self) -> None:
         self._state = {}
         self._filters = {}
 
-    def __getattr__(self, key: str) -> Union["Registry", type]:
+    def __getattr__(self, key: str) -> Registry | type:
         if key not in self._state:
             self._state[key] = Registry()
         if self._is_registry(key):
             return self._state[key]
         raise InvalidAttributeRegistryError(
             f"The attribute {key} is not a registry. You can use this function only to access "
             "a Registry object."
@@ -65,15 +67,15 @@
 
         Args:
             nested (bool): Indicates if the sub-registries should
                 be cleared or not. Default: ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             # Clear the main registry.
             >>> registry.clear()
             # Clear only the sub-registry other.
             >>> registry.other.clear()
@@ -92,15 +94,15 @@
         Args:
             nested (bool): Indicates if the filters of all the
                 sub-registries should be cleared or not.
                 Default: ``False``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             # Clear the filters of the main registry.
             >>> registry.clear_filters()
             # Clear the filters of the sub-registry other.
             >>> registry.other.clear_filters()
@@ -136,65 +138,70 @@
             ``AbstractClassAbstractFactoryError``: if you try to
                 instantiate an abstract class.
             ``UnregisteredClassAbstractFactoryError``: if the target
                 name is not found.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             >>> @registry.register()
             ... class MyClass:
             ...     ...
+            ...
             >>> registry.factory("MyClass")
             <__main__.MyClass object at 0x123456789>
         """
         return instantiate_object(
             self._get_target_from_name(_target_), *args, _init_=_init_, **kwargs
         )
 
-    def register(self, name: Optional[str] = None) -> Callable:
-        r"""Defines a decorator to add a class or a function to the registry.
+    def register(self, name: str | None = None) -> Callable:
+        r"""Defines a decorator to add a class or a function to the
+        registry.
 
         Args:
             name (str, optional): Specifies the name to use to
                 register the object. If ``None``, the full name of
                 the object is used as name. Default: ``None``.
 
         Returns:
             The decorated object.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             >>> @registry.register()
             ... class ClassToRegister:
             ...     ...
+            ...
             >>> registry.registered_names()
             {'__main__.ClassToRegister'}
             >>> @registry.register()
             ... def function_to_register(*args, **kwargs):
             ...     ...
+            ...
             >>> registry.registered_names()
             {'__main__.ClassToRegister', '__main__.function_to_register'}
         """
 
         def function_wrapper(obj: T) -> T:
             self.register_object(obj=obj, name=name)
             return obj
 
         return function_wrapper
 
     def register_child_classes(self, cls: type, ignore_abstract_class: bool = True) -> None:
-        r"""Registers a given class and its child classes of a given class.
+        r"""Registers a given class and its child classes of a given
+        class.
 
         This function registers all the child classes including the
         child classes of the child classes, etc. If you use this
         function, you cannot choose the names used to register the
         objects. It will use the full name of each object.
 
         Args:
@@ -202,53 +209,55 @@
             ignore_abstract_class (bool): Indicate if the abstract
                 class should be ignored or not. Be default, the
                 abstract classes are not registered because they
                 cannot be instantiated.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             >>> registry.register_child_classes(dict)
             >>> registry.registered_names()
             {'collections.defaultdict', 'enum._EnumDict', 'tornado.util.ObjectDict',
              'collections.Counter', 'builtins.dict', 'collections.OrderedDict'}
         """
         for class_to_register in [cls] + list(all_child_classes(cls)):
             if ignore_abstract_class and inspect.isabstract(class_to_register):
                 continue
             self.register_object(class_to_register)
 
-    def register_object(self, obj: Union[type, Callable], name: Optional[str] = None) -> None:
+    def register_object(self, obj: type | Callable, name: str | None = None) -> None:
         r"""Registers an object.
 
         Please read the documentation for more information.
 
         Args:
             obj: Specifies the object to register. The object is
                 expected to be a class or a function.
             name (str, optional): Specifies the name to use to
                 register the object. If ``None``, the full name of
                 the object is used as name. Default: ``None``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             >>> class ClassToRegister:
             ...     ...
+            ...
             >>> registry.registered_names()
             {'__main__.ClassToRegister'}
             >>> registry.register_object(ClassToRegister)
             >>> def function_to_register(*args, **kwargs):
             ...     ...
+            ...
             >>> registry.register_object(function_to_register)
             >>> registry.registered_names()
             {'__main__.ClassToRegister', '__main__.function_to_register'}
         """
         self._check_object(obj)
         if name is None:
             name = full_object_name(obj)
@@ -275,15 +284,15 @@
                 Default: ``True``.
 
         Returns:
             set: The names of the registered objects.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
             >>> registry.registered_names()
             # Show name of all the registered objects except the sub-registries.
             >>> registry.registered_names(include_registry=False)
         """
@@ -306,45 +315,45 @@
 
         Raises:
             ``UnregisteredObjectFactoryError`` if the name does not
                 exist in the registry.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from objectory import Registry
             >>> registry = Registry()
-            >>> registry.unregister('my_package.my_module.ClassToUnregister')
+            >>> registry.unregister("my_package.my_module.ClassToUnregister")
         """
         resolved_name = self._resolve_name(name)
         if resolved_name is None or not self._is_name_registered(resolved_name):
             raise UnregisteredObjectFactoryError(
                 f"It is not possible to remove an object which is not registered (received: {name})"
             )
         self._state.pop(resolved_name)
 
-    def set_class_filter(self, cls: Optional[type]) -> None:
-        r"""Sets the class filter so only the child classes of this class can be
-        registered.
+    def set_class_filter(self, cls: type | None) -> None:
+        r"""Sets the class filter so only the child classes of this class
+        can be registered.
 
         If you set this filter, you cannot register functions.
         To unset this filter, you can use ``set_class_filter(None)``.
 
         Args:
             cls (class or ``None``): Specifies the class to use as
                 filter. Only the child classes of this class
                 can be registered.
 
         Raises:
             TypeError if the input is not a class or ``None``.
 
         Example usage:
 
-        .. code-block:: python
+        .. code-block:: pycon
 
             >>> from collections import Counter, OrderedDict
             >>> from objectory import Registry
             >>> registry = Registry()
             >>> registry.mapping.set_class_filter(dict)
             >>> registry.mapping.register_object(OrderedDict)
             >>> registry.mapping.register_object(int)
@@ -357,17 +366,17 @@
             self._filters.pop(self._CLASS_FILTER, None)
             return
 
         if not inspect.isclass(cls):
             raise TypeError(f"The class filter has to be a class (received: {cls})")
         self._filters[self._CLASS_FILTER] = cls
 
-    def _check_object(self, obj: Union[type, Callable]) -> None:
-        r"""Checks if the object is valid for this registry before to register
-        it.
+    def _check_object(self, obj: type | Callable) -> None:
+        r"""Checks if the object is valid for this registry before to
+        register it.
 
         This function will raise an exception if the object is not
         valid.
 
         Args:
             obj: Specifies the object to check.
 
@@ -429,15 +438,15 @@
             name (string): Specifies the name to check.
 
         Returns:
             bool: ``True`` if the name is used as sub-registry, otherwise ``False``.
         """
         return isinstance(self._state[name], Registry)
 
-    def _resolve_name(self, name: str) -> Optional[str]:
+    def _resolve_name(self, name: str) -> str | None:
         r"""Tries to resolve the name.
 
         This function will look at if it can find an object which
         match with the given name. It is quite useful because there
         are several ways to load an object but only one can be
         registered. If you specify a full name (module path +
         class/function name), it will try to import the module
```

### Comparing `objectory-0.0.2/src/objectory/universal.py` & `objectory-0.0.3/src/objectory/universal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 __all__ = ["factory"]
 
 from typing import Any
 
 from objectory.utils import import_object, instantiate_object
 
 
@@ -22,15 +24,15 @@
         The instantiated object with the given parameters.
 
     Raises:
         ``RuntimeError``: if the target cannot be found.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory import factory
         >>> factory("collections.Counter", [1, 2, 1, 3])
         Counter({1: 2, 2: 1, 3: 1})
     """
     target = import_object(_target_)
     if target is None:
```

### Comparing `objectory-0.0.2/src/objectory/utils/name_resolution.py` & `objectory-0.0.3/src/objectory/utils/name_resolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """This module implements the name resolution mechanism."""
 
+from __future__ import annotations
+
 __all__ = ["resolve_name", "find_matches"]
 
-from typing import Optional
 
 from objectory.utils.object_helpers import full_object_name, import_object
 
 
-def resolve_name(name: str, object_names: set[str], allow_import: bool = True) -> Optional[str]:
-    r"""Tries to find a match of the query name in the set of object names.
+def resolve_name(name: str, object_names: set[str], allow_import: bool = True) -> str | None:
+    r"""Tries to find a match of the query name in the set of object
+    names.
 
     The resolution is successful only if there is only one object
     name that can match with the query name.
     Please read the documentation to learn more about the name
     resolution mechanism.
 
     Args:
@@ -22,15 +24,15 @@
 
     Returns:
         str or ``None``: The resolved name if the resolution was
             successful, otherwise ``None``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.utils import resolve_name
         >>> resolve_name("OrderedDict", {"collections.OrderedDict", "collections.Counter"})
         collections.OrderedDict
         >>> resolve_name("objectory.utils.resolve_name", {"math.isclose"})
         'objectory.utils.name_resolution.resolve_name'
         >>> resolve_name("OrderedDict", {"collections.Counter", "math.isclose"})
@@ -64,15 +66,15 @@
             to look for the query.
 
     Returns:
         set: The list of names that matches with the query.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.utils.name_resolution import find_matches
         >>> find_matches("OrderedDict", {"collections.Counter", "math.isclose"})
         set()
         >>> find_matches(
         ...     "OrderedDict", {"collections.OrderedDict", "collections.Counter", "math.isclose"}
         ... )
```

### Comparing `objectory-0.0.2/src/objectory/utils/object_helpers.py` & `objectory-0.0.3/src/objectory/utils/object_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 r"""This module contains some helper functions to manipulate objects."""
 
+from __future__ import annotations
+
 __all__ = [
     "all_child_classes",
     "full_object_name",
     "import_object",
     "instantiate_object",
     "is_lambda_function",
 ]
 
 import inspect
 import logging
-from typing import Any, Callable, Union
+from typing import Any, Callable
 
 from tornado.util import import_object as tornado_import_object
 
 from objectory.errors import AbstractClassFactoryError, IncorrectObjectFactoryError
 
 logger = logging.getLogger(__name__)
 
@@ -28,23 +30,25 @@
         cls: Specifies the class whose child classes you want to get.
 
     Returns:
         set: The set of all the child classes of the given class.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.utils import all_child_classes
         >>> class Foo:
         ...     pass
+        ...
         >>> all_child_classes(Foo)
         set()
         >>> class Bar(Foo):
         ...     pass
+        ...
         >>> all_child_classes(Foo)
         {<class '__main__.Bar'>}
     """
     return set(cls.__subclasses__()).union(
         [s for c in cls.__subclasses__() for s in all_child_classes(c)]
     )
 
@@ -62,23 +66,25 @@
         str: The full name of the object.
 
     Raises:
         ``TypeError`` if the object is not a class or a function.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.utils import full_object_name
         >>> class MyClass:
         ...     pass
+        ...
         >>> full_object_name(MyClass)
         '__main__.MyClass'
         >>> def my_function():
         ...     pass
+        ...
         >>> full_object_name(my_function)
         '__main__.my_function'
     """
     if inspect.isclass(obj) or inspect.isfunction(obj):
         return _full_object_name(obj)
     raise TypeError(f"Incorrect object type: {obj}")
 
@@ -113,35 +119,33 @@
         object_path: Specifies the path of the object to import.
 
     Returns:
         The object if the import was successful otherwise ``None``.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.utils import import_object
-        >>> obj = import_object('collections.Counter')
+        >>> obj = import_object("collections.Counter")
         >>> obj()
         Counter()
-        >>> fn = import_object('math.isclose')
+        >>> fn = import_object("math.isclose")
         >>> fn(1, 1)
         True
     """
     if not isinstance(object_path, str):
         raise TypeError(f"The object_path has to be a string (received: {object_path})")
     try:
         return tornado_import_object(object_path)
     except (ValueError, ImportError):
         return None
 
 
-def instantiate_object(
-    obj: Union[Callable, type], *args, _init_: str = "__init__", **kwargs
-) -> Any:
+def instantiate_object(obj: Callable | type, *args, _init_: str = "__init__", **kwargs) -> Any:
     r"""Instantiates dynamically an object from its configuration.
 
     Args:
         obj (class or function): Specifies the class to instantiate
             or the function to call.
         *args: Variable length argument list.
         _init_ (str, optional): Specifies the function to use to
@@ -155,15 +159,15 @@
             the returned value of the function.
 
     Raises:
         TypeError if ``obj`` is not a class or a function.
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from collections import Counter
         >>> from objectory.utils import instantiate_object
         >>> instantiate_object(Counter, [1, 2, 1])
         Counter({1: 2, 2: 1})
         >>> instantiate_object(list, [1, 2, 1])
         [1, 2, 1]
@@ -226,21 +230,22 @@
 
     Returns:
         bool: ``True`` if the input is a lambda function,
             otherwise ``False``
 
     Example usage:
 
-    .. code-block:: python
+    .. code-block:: pycon
 
         >>> from objectory.utils import is_lambda_function
         >>> is_lambda_function(lambda value: value + 1)
         True
         >>> def my_function(value: int) -> int:
         ...     return value + 1
+        ...
         >>> is_lambda_function(my_function)
         False
         >>> is_lambda_function(1)
         False
     """
     if not inspect.isfunction(obj):
         return False
```

### Comparing `objectory-0.0.2/PKG-INFO` & `objectory-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectory
-Version: 0.0.2
+Version: 0.0.3
 Summary: A light library for general purpose object factories
 Home-page: https://github.com/durandtibo/objectory
 License: BSD-3-Clause
 Keywords: factory,abstract factory,registry
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -14,41 +14,48 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: tornado (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/durandtibo/objectory
 Description-Content-Type: text/markdown
 
 # objectory = object + factory
 
 <p align="center">
     <a href="https://github.com/durandtibo/objectory/actions">
         <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/CI/badge.svg?event=push&branch=main">
     </a>
+    <a href="https://durandtibo.github.io/objectory/">
+        <img alt="CI" src="https://github.com/durandtibo/objectory/workflows/Documentation/badge.svg?event=push&branch=main">
+    </a>
+    <a href="https://codecov.io/gh/durandtibo/objectory">
+        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/objectory/maintainability">
+        <img src="https://api.codeclimate.com/v1/badges/1fad6e22f2d38335c26d/maintainability" />
+    </a>
+    <a href="https://codeclimate.com/github/durandtibo/objectory/test_coverage">
+        <img src="https://api.codeclimate.com/v1/badges/1fad6e22f2d38335c26d/test_coverage" />
+    </a>
+    <br/>
     <a href="https://pypi.org/project/objectory/">
         <img alt="PYPI version" src="https://img.shields.io/pypi/v/objectory">
     </a>
     <a href="https://pypi.org/project/objectory/">
         <img alt="Python" src="https://img.shields.io/pypi/pyversions/objectory.svg">
     </a>
     <a href="https://opensource.org/licenses/BSD-3-Clause">
         <img alt="BSD-3-Clause" src="https://img.shields.io/pypi/l/objectory">
     </a>
-    <a href="https://codecov.io/gh/durandtibo/objectory">
-        <img alt="Codecov" src="https://codecov.io/gh/durandtibo/objectory/branch/main/graph/badge.svg">
-    </a>
     <a href="https://github.com/psf/black">
         <img  alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
     </a>
     <a href="https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings">
         <img  alt="Doc style: google" src="https://img.shields.io/badge/%20style-google-3666d6.svg">
     </a>
     <br/>
@@ -59,15 +66,15 @@
         <img  alt="Monthly downloads" src="https://static.pepy.tech/badge/objectory/month">
     </a>
     <br/>
 </p>
 
 ## Overview
 
-A light Python library for general purpose object factories.
+A Python library for general purpose object factories.
 In particular, it focuses on dynamic object factory implementations where objects can be registered
 dynamically without changing the code of the factory.
 An object factory can be used to instantiate an object from its configuration.
 The current implementation contains both abstract factory and registry approaches.
 
 **factory**
```

