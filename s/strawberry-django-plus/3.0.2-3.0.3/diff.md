# Comparing `tmp/strawberry_django_plus-3.0.2.tar.gz` & `tmp/strawberry_django_plus-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-3.0.2.tar", max compression
+gzip compressed data, was "strawberry_django_plus-3.0.3.tar", max compression
```

## Comparing `strawberry_django_plus-3.0.2.tar` & `strawberry_django_plus-3.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1094 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/LICENSE
--rw-r--r--   0        0        0     3354 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/README.md
--rw-r--r--   0        0        0     4208 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     3088 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5649 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5800 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    30229 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3033 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1556 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0      896 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    24115 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14791 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26666 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1340 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    28069 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0     2532 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1027 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    17885 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/type.py
--rw-r--r--   0        0        0     9889 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13343 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    16244 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-25 13:00:34.004619 strawberry_django_plus-3.0.3/LICENSE
+-rw-r--r--   0        0        0     3354 2023-06-25 13:00:34.004619 strawberry_django_plus-3.0.3/README.md
+-rw-r--r--   0        0        0     4208 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3088 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5649 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5800 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    30229 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3033 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1556 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     2060 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    24115 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14791 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26973 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1340 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    28094 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0     2532 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1027 2023-06-25 13:00:34.008619 strawberry_django_plus-3.0.3/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2423 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    17118 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0     9889 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13343 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     6604 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    16377 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0     1027 2023-06-25 13:00:34.012619 strawberry_django_plus-3.0.3/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.3/PKG-INFO
```

### Comparing `strawberry_django_plus-3.0.2/LICENSE` & `strawberry_django_plus-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/README.md` & `strawberry_django_plus-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/pyproject.toml` & `strawberry_django_plus-3.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "3.0.2"
+version = "3.0.3"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/__init__.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "3.0.2"  # x-release-please-version
+__version__ = "3.0.3"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/directives.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/field.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/filters.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/integrations/guardian.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import contextlib
 import dataclasses
 import weakref
-from typing import Optional, Union, cast
+from typing import TYPE_CHECKING, Optional, Union, cast
 
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import Group
+from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from guardian import backends as _guardian_backends
 from guardian.conf import settings as guardian_settings
 from guardian.core import ObjectPermissionChecker as _ObjectPermissionChecker
 from guardian.models.models import GroupObjectPermissionBase, UserObjectPermissionBase
 from guardian.utils import get_anonymous_user as _get_anonymous_user
 from guardian.utils import get_group_obj_perms_model, get_user_obj_perms_model
+from typing_extensions import TypeAlias
 
 from strawberry_django_plus.utils.typing import UserType
 
+if TYPE_CHECKING:
+    from django.contrib.auth.models import Group
+
+UserOrGroup: TypeAlias = Union["Group", UserType]
+
+
 _cache = weakref.WeakKeyDictionary()
 
 
 @dataclasses.dataclass
 class ObjectPermissionModels:
     user: UserObjectPermissionBase
     group: GroupObjectPermissionBase
@@ -29,22 +35,22 @@
         user=cast(UserObjectPermissionBase, get_user_obj_perms_model(model)),
         group=cast(GroupObjectPermissionBase, get_group_obj_perms_model(model)),
     )
 
 
 def get_user_or_anonymous(user: UserType) -> UserType:
     username = guardian_settings.ANONYMOUS_USER_NAME or ""
-    if user.is_anonymous and user.username != username:
-        with contextlib.suppress(get_user_model().DoesNotExist):
+    if user.is_anonymous and user.get_username() != username:
+        with contextlib.suppress(ObjectDoesNotExist):
             return cast(UserType, _get_anonymous_user())
     return user
 
 
 class ObjectPermissionChecker(_ObjectPermissionChecker):
-    def __new__(cls, user_or_group: Optional[Union[UserType, Group]] = None):
+    def __new__(cls, user_or_group: Optional[UserOrGroup] = None):
         if user_or_group is not None and user_or_group in _cache:
             return _cache[user_or_group]
 
         obj = _ObjectPermissionChecker(user_or_group=user_or_group)
         _cache[user_or_group] = obj
 
         return obj
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
-from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.db import models
 from django.db.models import Prefetch
 from django.db.models.constants import LOOKUP_SEP
 from django.db.models.fields.reverse_related import (
     ManyToManyRel,
     ManyToOneRel,
     OneToOneRel,
@@ -52,25 +51,37 @@
     get_django_type,
     get_model_fields,
     get_possible_type_definitions,
     get_selections,
 )
 from .utils.typing import TypeOrSequence
 
+try:
+    from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
+
+except (ImportError, RuntimeError):  # pragma:nocover
+    GenericForeignKey = None
+    GenericRelation = None
+
+
 __all__ = [
     "OptimizerConfig",
     "DjangoOptimizerExtension",
     "OptimizerStore",
     "PrefetchType",
     "optimize",
 ]
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=models.Model)
 
+if GenericRelation:
+    _relation_fields = (models.ManyToManyField, ManyToManyRel, ManyToOneRel, GenericRelation)
+else:
+    _relation_fields = (models.ManyToManyField, ManyToManyRel, ManyToOneRel)
 _sentinel = object()
 _interfaces: """
 defaultdict[
     Schema,
     Dict[StrawberryObjectDefinition, List[StrawberryObjectDefinition]],
 ]""" = defaultdict(
     dict,
@@ -231,21 +242,21 @@
                         config=config,
                         model_cache=model_cache,
                         level=level + 1,
                     )
                     if f_store is not None:
                         model_cache.setdefault(f_model, []).append((level, f_store))
                         store |= f_store.with_prefix(path, info=info)
-            elif isinstance(model_field, GenericForeignKey):
+            elif GenericForeignKey and isinstance(model_field, GenericForeignKey):
                 # There's not much we can do to optimize generic foreign keys regarding
                 # only/select_related because they can be anything. Just prefetch_related them
                 store.prefetch_related.append(model_fieldname)
             elif isinstance(
                 model_field,
-                (models.ManyToManyField, ManyToManyRel, ManyToOneRel, GenericRelation),
+                _relation_fields,
             ):
                 f_types = list(get_possible_type_definitions(field.type))
                 if len(f_types) > 1:
                     # This might be a generic foreign key. In this case, just prefetch it
                     store.prefetch_related.append(model_fieldname)
                 elif len(f_types) == 1:
                     remote_field = model_field.remote_field
@@ -265,15 +276,15 @@
                         if (
                             (config is None or config.enable_only)
                             and f_store.only
                             and not isinstance(remote_field, ManyToManyRel)
                         ):
                             # If adding a reverse relation, make sure to select its pointer to us,
                             # or else this might causa a refetch from the database
-                            if isinstance(model_field, GenericRelation):
+                            if GenericRelation and isinstance(model_field, GenericRelation):
                                 f_store.only.append(model_field.object_id_field_name)
                                 f_store.only.append(model_field.content_type_field_name)
                             else:
                                 f_store.only.append(remote_field.attname or remote_field.name)
 
                         path_lookup = f"{path}{LOOKUP_SEP}"
                         if store.only and f_store.only:
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/ordering.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/permissions.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 except AttributeError:
     _cache = functools.lru_cache
 
 try:
     from .integrations.guardian import get_user_or_anonymous
 
     get_user_or_anonymous = resolvers.async_safe(get_user_or_anonymous)
-except ImportError:
+except (ImportError, RuntimeError):
     # Access the user's id to force it to be loaded from the database
     get_user_or_anonymous = resolvers.async_safe(lambda u: (u, u.id)[0])
 
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=Model)
 
@@ -129,15 +129,15 @@
 
     for check in checks:
         if check.target != PermTarget.RETVAL:
             continue
 
         qs = filter_for_user(
             qs,
-            cast(UserType, user),
+            user,
             [p.perm for p in check.permissions],
             any_perm=check.any,
             with_superuser=check.with_superuser,
         )
 
     set_perm_safe(True)
     return qs
@@ -223,15 +223,15 @@
     checks = running_checks.get()
     if not checks:
         return instance
 
     user = cast(StrawberryDjangoContext, info.context).request.user
     for check in checks:
         f = any if check.any else all
-        checker = check.obj_perm_checker(info, cast(UserType, user))
+        checker = check.obj_perm_checker(info, user)
         if not f(checker(p, instance) for p in check.permissions):
             raise PermissionDenied(check.message)
 
     return instance
 
 
 @dataclasses.dataclass
@@ -252,15 +252,15 @@
         info: GraphQLResolveInfo,
         *args,
         **kwargs,
     ):
         context = cast(StrawberryDjangoContext, info.context)
         resolver = functools.partial(_next, root, info, *args, **kwargs)
 
-        user = cast(UserType, context.request.user)
+        user = context.request.user
         if not getattr(context, _user_ensured_attr, False):
             return aio.resolve(
                 cast(UserType, get_user_or_anonymous(user)),
                 functools.partial(
                     self.resolve_for_user,
                     helper,
                     resolver,
@@ -446,15 +446,15 @@
     def check_condition(
         self,
         root: Any,
         info: GraphQLResolveInfo,
         user: UserType,
         **kwargs,
     ) -> bool:
-        return user.is_authenticated and user.is_staff
+        return user.is_authenticated and getattr(user, "is_staff", False)
 
 
 @strawberry.schema_directive(
     locations=[Location.FIELD_DEFINITION],
     description=_desc("Can only be resolved by superuser users."),
 )
 @final
@@ -466,15 +466,15 @@
     def check_condition(
         self,
         root: Any,
         info: GraphQLResolveInfo,
         user: UserType,
         **kwargs,
     ) -> bool:
-        return user.is_authenticated and user.is_superuser
+        return user.is_authenticated and getattr(user, "is_superuser", False)
 
 
 @strawberry.input(description="Permission definition for schema directives.")
 @dataclasses.dataclass(eq=True, order=True, frozen=True)
 class PermDefinition:
     """Permission definition.
 
@@ -629,15 +629,15 @@
         helper: SchemaDirectiveHelper,
         resolver: Callable,
         root: Any,
         info: GraphQLResolveInfo,
         user: UserType,
         **kwargs,
     ):
-        if self.with_superuser and user.is_active and user.is_superuser:
+        if self.with_superuser and user.is_active and getattr(user, "is_superuser", False):
             return self.resolve_retval(helper, root, info, resolver, True)
         if self.with_anonymous and user.is_anonymous:
             return self.resolve_retval(helper, root, info, resolver, False)
 
         cache = self.get_cache(info, user)
 
         if self.target is None:
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/relay.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/settings.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/test/client.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/test/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import contextlib
 from typing import Any, Awaitable, Dict, Optional, cast
 
 from asgiref.sync import sync_to_async
-from django.contrib.auth.models import AbstractUser
+from django.contrib.auth.base_user import AbstractBaseUser
 from django.test.client import AsyncClient, Client  # type: ignore
 from strawberry.test import BaseGraphQLTestClient
 from strawberry.test.client import Response
 
 
 class TestClient(BaseGraphQLTestClient):
     def __init__(self, path: str, client: Optional[Client] = None):
@@ -31,15 +31,15 @@
 
         return self.client.post(
             self.path,
             **kwargs,  # type: ignore
         )
 
     @contextlib.contextmanager
-    def login(self, user: AbstractUser):
+    def login(self, user: AbstractBaseUser):
         self.client.force_login(user)
         yield
         self.client.logout()
 
 
 class AsyncTestClient(TestClient):
     def __init__(self, path: str, client: AsyncClient = None):
@@ -69,11 +69,11 @@
         )
         if asserts_errors:
             assert response.errors is None, response.errors
 
         return response
 
     @contextlib.asynccontextmanager
-    async def login(self, user: AbstractUser):
+    async def login(self, user: AbstractBaseUser):
         await sync_to_async(self.client.force_login)(user)
         yield
         await sync_to_async(self.client.logout)()
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/type.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/type.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,20 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import strawberry
-from django.contrib.contenttypes.fields import GenericForeignKey, GenericRel
 from django.core.exceptions import FieldDoesNotExist
 from django.db.models.base import Model
 from django.db.models.fields.reverse_related import ManyToManyRel, ManyToOneRel
 from strawberry import UNSET, relay
 from strawberry.annotation import StrawberryAnnotation
-from strawberry.exceptions import (
-    MissingFieldAnnotationError,
-)
+from strawberry.exceptions import MissingFieldAnnotationError
 from strawberry.field import StrawberryField
 from strawberry.private import is_private
 from strawberry.type import get_object_definition
 from strawberry.unset import UnsetType
 from strawberry_django.fields.field import field as _field
 from strawberry_django.fields.types import get_model_field, resolve_model_field_name
 from strawberry_django.type import StrawberryDjangoType as _StraberryDjangoType
@@ -45,38 +42,35 @@
 from .utils.resolvers import (
     resolve_model_id,
     resolve_model_id_attr,
     resolve_model_node,
     resolve_model_nodes,
 )
 
+try:
+    from django.contrib.contenttypes.fields import GenericForeignKey, GenericRel
+
+    GenericTypes = (GenericForeignKey, GenericRel)
+except (ImportError, RuntimeError):  # pragma:nocover
+    GenericTypes = ()
+
+
 __all = [
     "StrawberryDjangoType",
     "type",
     "interface",
     "input",
     "partial",
 ]
 
 _T = TypeVar("_T")
 _O = TypeVar("_O", bound=type)
 _M = TypeVar("_M", bound=Model)
 
 
-def _has_own_node_resolver(cls, name: str) -> bool:
-    resolver = getattr(cls, name, None)
-    if resolver is None:
-        return False
-
-    if id(resolver.__func__) == id(getattr(relay.Node, name).__func__):
-        return False
-
-    return True
-
-
 def _process_type(
     cls: _O,
     model: Type[Model],
     *,
     field_cls: Type[StrawberryDjangoField] = StrawberryDjangoField,
     filters: Optional[type] = UNSET,
     order: Optional[type] = UNSET,
@@ -156,48 +150,29 @@
 
     # Make sure model is also considered a "virtual subclass" of cls
     if "is_type_of" not in cls.__dict__:
         cls.is_type_of = lambda obj, info: isinstance(obj, (cls, model))  # type: ignore
 
     # Default querying methods for relay
     if issubclass(cls, relay.Node):
-        if not _has_own_node_resolver(cls, "resolve_node"):
-            cls.resolve_node = types.MethodType(resolve_model_node, cls)
-
-        if not _has_own_node_resolver(cls, "resolve_nodes"):
-            cls.resolve_nodes = types.MethodType(
-                lambda *args, **kwargs: resolve_model_nodes(
-                    *args,
-                    filter_perms=True,
-                    **kwargs,
-                ),
-                cls,
-            )
-
-        if not _has_own_node_resolver(cls, "resolve_id"):
-            cls.resolve_id = types.MethodType(
-                lambda cls, root, *args, **kwargs: resolve_model_id(cls, root),
-                cls,
-            )
-
-        if not _has_own_node_resolver(cls, "resolve_id"):
-            cls.resolve_id = types.MethodType(
-                lambda cls, root, *args, **kwargs: resolve_model_id(cls, root),
-                cls,
-            )
-
-        if not _has_own_node_resolver(cls, "resolve_id_attr"):
-            cls.resolve_id_attr = types.MethodType(
-                resolve_model_id_attr,
-                cls,
-            )
+        for attr, func in [
+            ("resolve_id", resolve_model_id),
+            ("resolve_id_attr", resolve_model_id_attr),
+            ("resolve_node", resolve_model_node),
+            ("resolve_nodes", resolve_model_nodes),
+        ]:
+            existing_resolver = getattr(cls, attr, None)
+            if (
+                existing_resolver is None
+                or existing_resolver.__func__ is getattr(relay.Node, attr).__func__
+            ):
+                setattr(cls, attr, types.MethodType(func, cls))
 
-        # Adjust types that inherit from other types/interfaces that implement Node
-        # to make sure they pass themselves as the node type
-        for attr in ["resolve_node", "resolve_nodes", "resolve_id"]:
+            # Adjust types that inherit from other types/interfaces that implement Node
+            # to make sure they pass themselves as the node type
             meth = getattr(cls, attr)
             if isinstance(meth, types.MethodType) and meth.__self__ is not cls:
                 setattr(cls, attr, types.MethodType(cast(classmethod, meth).__func__, cls))
 
     strawberry.type(cls, **kwargs)
 
     # update annotations and fields
@@ -259,15 +234,15 @@
                 django_name = resolve_model_field_name(
                     model_attr,
                     is_input=django_type.is_input,
                     is_filter=bool(django_type.is_filter),
                 )
 
             if description is None:
-                if isinstance(model_attr, (GenericRel, GenericForeignKey)):
+                if isinstance(model_attr, GenericTypes):
                     f_description = None
                 elif isinstance(model_attr, (ManyToOneRel, ManyToManyRel)):
                     f_description = model_attr.field.help_text
                 else:
                     f_description = getattr(model_attr, "help_text", None)
 
                 if f_description:
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/types.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import functools
-from typing import List, Optional, Set, Type, TypeVar
+from typing import TYPE_CHECKING, List, Optional, Set, Type, TypeVar, cast
 
-from django.contrib.auth import get_user_model
-from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import FieldDoesNotExist
 from django.db.models import Exists, F, Model, Q, QuerySet
 from django.db.models.functions import Cast
 from strawberry_django.utils import is_async
 
 from .typing import TypeOrIterable, UserType
 
+if TYPE_CHECKING:
+    from django.contrib.auth.models import AbstractUser
+    from django.contrib.contenttypes.models import ContentType as ContentTypeType
+try:
+    from django.contrib.contenttypes.models import ContentType
+
+except (ImportError, RuntimeError):
+    ContentType = None
+
+
 try:
     from strawberry_django_plus.integrations.guardian import (
         get_object_permission_models,
     )
 
     has_guardian = True
-except ImportError:  # pragma:nocover
+except (ImportError, RuntimeError):  # pragma:nocover
     has_guardian = False
 
-_M = TypeVar("_M", bound=Model)
 _Q = TypeVar("_Q", bound=QuerySet)
 
 
 def _filter(
     qs: _Q,
     perms: List[str],
     *,
     lookup: str = "",
     model: Type[Model],
     any_perm: bool = True,
-    ctype: Optional[ContentType] = None,
+    ctype: Optional["ContentTypeType"] = None,
 ) -> _Q:
     lookup = lookup and f"{lookup}__"
     ctype_attr = f"{lookup}content_type"
 
     if ctype is not None:
         q = Q(**{ctype_attr: ctype})
     else:
@@ -60,38 +68,45 @@
     user: UserType,
     perms: TypeOrIterable[str],
     *,
     any_perm: bool = True,
     with_groups: bool = True,
     with_superuser: bool = False,
 ):
-    if with_superuser and user.is_active and user.is_superuser:
+    if with_superuser and user.is_active and getattr(user, "is_superuser", False):
         return qs
 
     if user.is_anonymous:
         return qs.none()
 
+    groups_field = None
+    try:
+        groups_field = cast("AbstractUser", user)._meta.get_field("groups")
+    except FieldDoesNotExist:
+        with_groups = False
+
     if isinstance(perms, str):
         perms = [perms]
 
-    model = qs.model
+    model = cast(Type[Model], qs.model)
     if model._meta.concrete_model:
-        model = model._meta.concrete_model
+        model = cast(Type[Model], model._meta.concrete_model)
 
     # We don't want to query the database here because this might not be async safe
     # Try to retrieve the ContentType from cache. If it is not there, we will
     # query it through the queryset
-    ctype: Optional[ContentType] = None
-    try:
-        meta = model._meta
-        ctype = ContentType.objects._get_from_cache(meta)  # type: ignore
-    except KeyError:  # pragma:nocover
-        # If we are not running async, retrieve it
-        if not is_async():
-            ctype = ContentType.objects.get_for_model(model)
+    ctype: Optional["ContentTypeType"] = None
+    if ContentType is not None:
+        try:
+            meta = model._meta
+            ctype = cast(ContentType, ContentType.objects._get_from_cache(meta))  # type: ignore
+        except KeyError:  # pragma:nocover
+            # If we are not running async, retrieve it
+            if not is_async():
+                ctype = ContentType.objects.get_for_model(model)
 
     app_labels = set()
     perms_list = []
     for p in perms:
         parts = p.split(".")
         if len(parts) > 1:
             app_labels.add(parts[0])
@@ -109,29 +124,31 @@
     # Small optimization if the user's permissions are cached
     if (perm_cache := getattr(user, "_perm_cache", None)) is not None:  # pragma:nocover
         f = any if any_perm else all
         user_perms: Set[str] = {p.codename for p in perm_cache}
         if f(p in user_perms for p in perms_list):
             return qs
 
-    q = Q(
-        Exists(
-            _filter(
-                user.user_permissions,
-                perms_list,
-                model=model,
-                ctype=ctype,
+    q = Q()
+    if hasattr(user, "user_permissions"):
+        q |= Q(
+            Exists(
+                _filter(
+                    cast("AbstractUser", user).user_permissions,
+                    perms_list,
+                    model=model,
+                    ctype=ctype,
+                ),
             ),
-        ),
-    )
+        )
     if with_groups:
         q |= Q(
             Exists(
                 _filter(
-                    user.groups,
+                    cast("AbstractUser", user).groups,
                     perms_list,
                     lookup="permissions",
                     model=model,
                     ctype=ctype,
                 ),
             ),
         )
@@ -148,19 +165,21 @@
             ctype=ctype,
         )
         if user_model.objects.is_generic():
             user_qs = user_qs.filter(content_type=F("permission__content_type"))
         else:
             user_qs = user_qs.annotate(object_pk=F("content_object"))
 
-        obj_qs = user_qs.values_list(Cast("object_pk", model._meta.pk), flat=True).distinct()
+        obj_qs = user_qs.values_list(
+            Cast("object_pk", cast(str, model._meta.pk)),
+            flat=True,
+        ).distinct()
 
         if with_groups:
             group_model = perm_models.group
-            groups_field = get_user_model()._meta.get_field("groups")
             group_qs = _filter(
                 group_model.objects.filter(
                     **{
                         f"group__{groups_field.related_query_name()}": user,  # type: ignore
                     },
                 ),
                 perms_list,
@@ -170,15 +189,18 @@
             )
             if group_model.objects.is_generic():
                 group_qs = group_qs.filter(content_type=F("permission__content_type"))
             else:
                 group_qs = group_qs.annotate(object_pk=F("content_object"))
 
             obj_qs = obj_qs.union(
-                group_qs.values_list(Cast("object_pk", model._meta.pk), flat=True).distinct(),
+                group_qs.values_list(
+                    Cast("object_pk", cast(str, model._meta.pk)),
+                    flat=True,
+                ).distinct(),
             )
 
         q |= Q(pk__in=obj_qs)
 
     return q
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,17 +459,19 @@
             else:
                 retval.append(results_map.get(str(node_id), None))
 
         return retval  # type: ignore
 
     if inspect.isawaitable(retval):
 
-        async def resolver():
+        async def async_resolver():
             return await sync_to_async(map_results)(await retval)
 
+        return async_resolver()
+
     return map_results(cast(QuerySet[_M], retval))
 
 
 @overload
 def resolve_model_node(
     source: Union[Type[relay.Node], Type[_M]],
     node_id: Union[str, relay.GlobalID],
@@ -554,22 +556,26 @@
 
     return id_attr
 
 
 def resolve_model_id(
     source: Union[Type[relay.Node], Type[_M]],
     root: Model,
+    *,
+    info: Optional[Info] = None,
 ) -> AwaitableOrValue[str]:
     """Resolve the model id, ensuring it is retrieved in a sync context.
 
     Args:
         source:
             The source model or the model type that implements the `Node` interface
         root:
             The source model object.
+        info:
+            Optional gql execution info
 
     Returns:
         The resolved object id
 
     """
     id_attr = cast(relay.Node, source).resolve_id_attr()
```

### Comparing `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-3.0.3/strawberry_django_plus/utils/typing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from typing import Any, Dict, Iterable, Sequence, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Sequence, TypeVar, Union
 
-from django.contrib.auth.models import AbstractUser, AnonymousUser
+from django.contrib.auth.base_user import AbstractBaseUser
 from graphql.type.definition import GraphQLResolveInfo
 from strawberry.auto import StrawberryAuto
 from strawberry.django.context import StrawberryDjangoContext
 from strawberry.types.info import Info
 from typing_extensions import TypeAlias
 
+if TYPE_CHECKING:
+    from django.contrib.auth.models import AnonymousUser
+
 _T = TypeVar("_T")
 
 DictTree: TypeAlias = Dict[str, "DictTree"]
 TypeOrSequence: TypeAlias = Union[_T, Sequence[_T]]
 TypeOrIterable: TypeAlias = Union[_T, Iterable[_T]]
-UserType: TypeAlias = Union[AbstractUser, AnonymousUser]
+UserType: TypeAlias = Union[AbstractBaseUser, "AnonymousUser"]
 ResolverInfo: TypeAlias = Union[Info[StrawberryDjangoContext, Any], GraphQLResolveInfo]
 
 
 def is_auto(type_: Any) -> bool:
     try:
         return isinstance(type_, StrawberryAuto)
     except NameError:
```

### Comparing `strawberry_django_plus-3.0.2/PKG-INFO` & `strawberry_django_plus-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 3.0.2
+Version: 3.0.3
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

