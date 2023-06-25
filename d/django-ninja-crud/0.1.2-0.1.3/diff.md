# Comparing `tmp/django_ninja_crud-0.1.2.tar.gz` & `tmp/django_ninja_crud-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_crud-0.1.2.tar", max compression
+gzip compressed data, was "django_ninja_crud-0.1.3.tar", max compression
```

## Comparing `django_ninja_crud-0.1.2.tar` & `django_ninja_crud-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/LICENSE
--rw-r--r--   0        0        0     4163 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/__init__.py
--rw-r--r--   0        0        0      151 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/apps.py
--rw-r--r--   0        0        0      239 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/schemas.py
--rw-r--r--   0        0        0      574 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/__init__.py
--rw-r--r--   0        0        0     5334 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_abstract.py
--rw-r--r--   0        0        0     4548 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_create.py
--rw-r--r--   0        0        0     2535 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_delete.py
--rw-r--r--   0        0        0     4240 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_list.py
--rw-r--r--   0        0        0     3006 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_retrieve.py
--rw-r--r--   0        0        0     4446 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/test_update.py
--rw-r--r--   0        0        0      303 2023-06-18 20:26:29.360694 django_ninja_crud-0.1.2/ninja_crud/tests/utils.py
--rw-r--r--   0        0        0      397 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/utils.py
--rw-r--r--   0        0        0      409 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/__init__.py
--rw-r--r--   0        0        0      830 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/abstract.py
--rw-r--r--   0        0        0     3836 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/create.py
--rw-r--r--   0        0        0     1551 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/delete.py
--rw-r--r--   0        0        0     3947 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/list.py
--rw-r--r--   0        0        0     1548 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/retrieve.py
--rw-r--r--   0        0        0     1959 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/ninja_crud/views/update.py
--rw-r--r--   0        0        0     1611 2023-06-18 20:26:29.364694 django_ninja_crud-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7755 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/apps.py
+-rw-r--r--   0        0        0      239 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/schemas.py
+-rw-r--r--   0        0        0      574 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/__init__.py
+-rw-r--r--   0        0        0     5288 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_abstract.py
+-rw-r--r--   0        0        0     4581 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_create.py
+-rw-r--r--   0        0        0     2761 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_delete.py
+-rw-r--r--   0        0        0     5103 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_list.py
+-rw-r--r--   0        0        0     3244 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_retrieve.py
+-rw-r--r--   0        0        0     4668 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/test_update.py
+-rw-r--r--   0        0        0      303 2023-06-25 21:06:47.065145 django_ninja_crud-0.1.3/ninja_crud/tests/utils.py
+-rw-r--r--   0        0        0      397 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/utils.py
+-rw-r--r--   0        0        0      409 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/__init__.py
+-rw-r--r--   0        0        0      794 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/abstract.py
+-rw-r--r--   0        0        0     3894 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/create.py
+-rw-r--r--   0        0        0     1582 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/delete.py
+-rw-r--r--   0        0        0     3971 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/list.py
+-rw-r--r--   0        0        0     1567 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/retrieve.py
+-rw-r--r--   0        0        0     2000 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/ninja_crud/views/update.py
+-rw-r--r--   0        0        0     1611 2023-06-25 21:06:47.069146 django_ninja_crud-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9411 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.3/PKG-INFO
```

### Comparing `django_ninja_crud-0.1.2/LICENSE` & `django_ninja_crud-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/__init__.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/test_abstract.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/test_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import inspect
 import json
 from http import HTTPStatus
 from typing import Callable, List, NamedTuple, Optional, Tuple, Type
 
 from django.db.models import Model, QuerySet
 from django.http import HttpResponse
@@ -91,16 +89,16 @@
         )
 
     def assert_content_equals_schema_list(
         self,
         content: List[dict],
         queryset: QuerySet[Model],
         output_schema: Type[Schema],
-        limit: int = 100,
-        offset: int = 0,
+        limit: int,
+        offset: int,
     ):
         self.test_case.assertIsInstance(content, dict)
 
         self.test_case.assertIn("count", content)
         count = content["count"]
         self.test_case.assertIsInstance(count, int)
         self.test_case.assertEqual(count, queryset.count())
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/test_create.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from http import HTTPStatus
-from typing import Callable
+from typing import Callable, Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
@@ -23,15 +23,17 @@
         credentials_getter: Callable[[TestCase], Credentials] = None,
     ) -> None:
         super().__init__(
             instance_getter=instance_getter, credentials_getter=credentials_getter
         )
         self.payloads = payloads
 
-    def create_model(self, id: UUID, data: dict, credentials: dict) -> HttpResponse:
+    def create_model(
+        self, id: Union[int, UUID], data: dict, credentials: dict
+    ) -> HttpResponse:
         model_view: CreateModelView = self.get_model_view()
         model_name = utils.to_snake_case(self.model_view_set.model.__name__)
         if model_view.detail:
             related_model_name = utils.to_snake_case(model_view.related_model.__name__)
             url_name = f"{model_name}_{related_model_name}s"
             kwargs = {"id": id}
         else:
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/test_delete.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/test_delete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+import random
 import uuid
 from http import HTTPStatus
+from typing import Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
 from ninja_crud.views.delete import DeleteModelView
 
 
 class DeleteModelViewTest(AbstractModelViewTest):
     model_view = DeleteModelView
 
-    def delete_model(self, id: UUID, credentials: dict) -> HttpResponse:
+    def delete_model(self, id: Union[int, UUID], credentials: dict) -> HttpResponse:
         kwargs = {"id": id}
         url_name = utils.to_snake_case(self.model_view_set.model.__name__)
         return self.client.delete(
             reverse(f"api:{url_name}", kwargs=kwargs),
             content_type="application/json",
             **credentials,
         )
@@ -43,15 +45,19 @@
         )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_delete_model_not_found(self):
         credentials: Credentials = self.get_credentials(self.test_case)
-        response = self.delete_model(id=uuid.uuid4(), credentials=credentials.ok)
+        instance: Model = self.get_instance(self.test_case)
+        random_id = (
+            uuid.uuid4() if type(instance.pk) is UUID else random.randint(1000, 9999)
+        )
+        response = self.delete_model(id=random_id, credentials=credentials.ok)
         self.assert_response_is_bad_request(response, status_code=HTTPStatus.NOT_FOUND)
 
     def test_delete_model_forbidden(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.forbidden is None:
             self.test_case.skipTest("No forbidden credentials provided")
         instance: Model = self.get_instance(self.test_case)
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/test_list.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/test_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import json
 from http import HTTPStatus
-from typing import Callable, List
+from typing import Callable, Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
 from ninja_crud import utils
-from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
+from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials, Payloads
 from ninja_crud.views.list import ListModelView
 
 
 class ListModelViewTest(AbstractModelViewTest):
     model_view = ListModelView
 
     def __init__(
         self,
         instance_getter: Callable[[TestCase], Model],
         credentials_getter: Callable[[TestCase], Credentials] = None,
-        filters: List[dict] = None,
+        filters: Payloads = None,
     ) -> None:
         super().__init__(
             instance_getter=instance_getter, credentials_getter=credentials_getter
         )
-        if filters is None:
-            filters = []
         self.filters = filters
 
     def list_model(
-        self, id: UUID, credentials: dict, data: dict = None
+        self, id: Union[int, UUID], credentials: dict, data: dict = None
     ) -> HttpResponse:
         model_view: ListModelView = self.get_model_view()
         model_name = utils.to_snake_case(self.model_view_set.model.__name__)
         if model_view.detail:
             related_model_name = utils.to_snake_case(model_view.related_model.__name__)
             url_name = f"{model_name}_{related_model_name}s"
             kwargs = {"id": id}
@@ -47,15 +45,15 @@
             data=data,
             content_type="application/json",
             **credentials,
         )
         return response
 
     def assert_response_is_ok(
-        self, response: HttpResponse, id: UUID, data: dict = None
+        self, response: HttpResponse, id: Union[int, UUID], data: dict = None
     ):
         self.test_case.assertEqual(response.status_code, HTTPStatus.OK)
         content = json.loads(response.content)
 
         model_view: ListModelView = self.get_model_view()
 
         if model_view.detail:
@@ -66,33 +64,58 @@
         else:
             if model_view.get_queryset is not None:
                 queryset = model_view.get_queryset()
             else:
                 queryset = self.model_view_set.model.objects.get_queryset()
 
         if data is not None:
+            limit = data.pop("limit", 100)
+            offset = data.pop("offset", 0)
             filter_instance = model_view.filter_schema(**data)
             queryset = model_view.filter_queryset(queryset, filter_instance)
+        else:
+            limit = 100
+            offset = 0
 
         self.assert_content_equals_schema_list(
-            content, queryset=queryset, output_schema=model_view.output_schema
+            content,
+            queryset=queryset,
+            output_schema=model_view.output_schema,
+            limit=limit,
+            offset=offset,
         )
 
     def test_list_model_ok(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         instance: Model = self.get_instance(self.test_case)
         response = self.list_model(id=instance.pk, credentials=credentials.ok)
         self.assert_response_is_ok(response, id=instance.pk)
 
-        for data in self.filters:
-            with self.test_case.subTest(data=data):
+        if self.filters is not None:
+            with self.test_case.subTest(data=self.filters.ok):
                 response = self.list_model(
-                    id=instance.pk, credentials=credentials.ok, data=data
+                    id=instance.pk, credentials=credentials.ok, data=self.filters.ok
+                )
+                self.assert_response_is_ok(
+                    response, id=instance.pk, data=self.filters.ok
                 )
-                self.assert_response_is_ok(response, id=instance.pk, data=data)
+
+    def test_list_model_bad_request(self):
+        if self.filters is None or self.filters.bad_request is None:
+            self.test_case.skipTest("No bad request filters provided")
+        credentials: Credentials = self.get_credentials(self.test_case)
+        instance: Model = self.get_instance(self.test_case)
+        response = self.list_model(
+            id=instance.pk,
+            credentials=credentials.ok,
+            data=self.filters.bad_request,
+        )
+        self.assert_response_is_bad_request(
+            response, status_code=HTTPStatus.BAD_REQUEST
+        )
 
     def test_list_model_unauthorized(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.unauthorized is None:
             self.test_case.skipTest("No unauthorized credentials provided")
         instance: Model = self.get_instance(self.test_case)
         response = self.list_model(id=instance.pk, credentials=credentials.unauthorized)
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/test_retrieve.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/test_retrieve.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import json
+import random
 import uuid
 from http import HTTPStatus
+from typing import Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
 from ninja_crud.views.retrieve import RetrieveModelView
 
 
 class RetrieveModelViewTest(AbstractModelViewTest):
     model_view = RetrieveModelView
 
-    def retrieve_model(self, id: UUID, credentials: dict) -> HttpResponse:
+    def retrieve_model(self, id: Union[int, UUID], credentials: dict) -> HttpResponse:
         kwargs = {"id": id}
         url_name = utils.to_snake_case(self.model_view_set.model.__name__)
         return self.client.get(
             reverse(f"api:{url_name}", kwargs=kwargs),
             content_type="application/json",
             **credentials,
         )
 
-    def assert_response_is_ok(self, response: HttpResponse, id: UUID):
+    def assert_response_is_ok(self, response: HttpResponse, id: Union[int, UUID]):
         self.test_case.assertEqual(response.status_code, HTTPStatus.OK)
         content = json.loads(response.content)
 
         model_view: RetrieveModelView = self.get_model_view()
 
         if model_view.get_queryset is not None:
             queryset = model_view.get_queryset(id)
@@ -57,15 +59,19 @@
         )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_retrieve_model_not_found(self):
         credentials: Credentials = self.get_credentials(self.test_case)
-        response = self.retrieve_model(id=uuid.uuid4(), credentials=credentials.ok)
+        instance: Model = self.get_instance(self.test_case)
+        random_id = (
+            uuid.uuid4() if type(instance.pk) is UUID else random.randint(1000, 9999)
+        )
+        response = self.retrieve_model(id=random_id, credentials=credentials.ok)
         self.assert_response_is_bad_request(response, status_code=HTTPStatus.NOT_FOUND)
 
     def test_retrieve_model_forbidden(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.forbidden is None:
             self.test_case.skipTest("No forbidden credentials provided")
         instance: Model = self.get_instance(self.test_case)
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/tests/test_update.py` & `django_ninja_crud-0.1.3/ninja_crud/tests/test_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
+import random
 import uuid
 from http import HTTPStatus
-from typing import Callable
+from typing import Callable, Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
@@ -24,15 +25,17 @@
         credentials_getter: Callable[[TestCase], Credentials] = None,
     ) -> None:
         super().__init__(
             instance_getter=instance_getter, credentials_getter=credentials_getter
         )
         self.payloads = payloads
 
-    def update_model(self, id: UUID, data: dict, credentials: dict) -> HttpResponse:
+    def update_model(
+        self, id: Union[int, UUID], data: dict, credentials: dict
+    ) -> HttpResponse:
         kwargs = {"id": id}
         url_name = utils.to_snake_case(self.model_view_set.model.__name__)
         return self.client.put(
             reverse(f"api:{url_name}", kwargs=kwargs),
             data=data,
             content_type="application/json",
             **credentials,
@@ -89,16 +92,20 @@
         )
         self.assert_response_is_bad_request(
             response, status_code=HTTPStatus.UNAUTHORIZED
         )
 
     def test_update_model_not_found(self):
         credentials: Credentials = self.get_credentials(self.test_case)
+        instance: Model = self.get_instance(self.test_case)
+        random_id = (
+            uuid.uuid4() if type(instance.pk) is UUID else random.randint(1000, 9999)
+        )
         response = self.update_model(
-            id=uuid.uuid4(), data=self.payloads.ok, credentials=credentials.ok
+            id=random_id, data=self.payloads.ok, credentials=credentials.ok
         )
         self.assert_response_is_bad_request(response, status_code=HTTPStatus.NOT_FOUND)
 
     def test_update_model_forbidden(self):
         credentials: Credentials = self.get_credentials(self.test_case)
         if credentials.forbidden is None:
             self.test_case.skipTest("No forbidden credentials provided")
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/views/abstract.py` & `django_ninja_crud-0.1.3/ninja_crud/views/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 from abc import ABC, abstractmethod
 from typing import Callable, List, Type
 
 from django.db.models import Model
 from ninja import Router
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/views/create.py` & `django_ninja_crud-0.1.3/ninja_crud/views/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,19 @@
         input_schema: Type[Schema],
         output_schema: Type[Schema],
         decorators: List[Callable] = None,
         detail: bool = False,
         related_model: Type[Model] = None,
         pre_save: Union[
             Callable[[HttpRequest, Model], None],
-            Callable[[HttpRequest, UUID, Model], None],
+            Callable[[HttpRequest, Union[int, UUID], Model], None],
         ] = None,
         post_save: Union[
             Callable[[HttpRequest, Model], None],
-            Callable[[HttpRequest, UUID, Model], None],
+            Callable[[HttpRequest, Union[int, UUID], Model], None],
         ] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.input_schema = input_schema
         self.output_schema = output_schema
         self.detail = detail
         self.related_model = related_model
@@ -85,15 +85,17 @@
             url,
             response={HTTPStatus.CREATED: output_schema},
             url_name=f"{parent_model_name}_{plural_model_name}",
             operation_id=operation_id,
             summary=summary,
         )
         @merge_decorators(self.decorators)
-        def create_model(request: HttpRequest, id: UUID, payload: input_schema):
+        def create_model(
+            request: HttpRequest, id: Union[int, UUID], payload: input_schema
+        ):
             instance = self.related_model()
             for field, value in payload.dict(exclude_unset=True).items():
                 setattr(instance, field, value)
             if self.pre_save:
                 self.pre_save(request, id, instance)
             instance.full_clean()
             instance.save()
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/views/delete.py` & `django_ninja_crud-0.1.3/ninja_crud/views/delete.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import Callable, List, Type
+from typing import Callable, List, Type, Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router
 
 from ninja_crud import utils
@@ -12,15 +12,15 @@
 
 
 class DeleteModelView(AbstractModelView):
     def __init__(
         self,
         decorators: List[Callable] = None,
         pre_delete: Callable[[HttpRequest, Model], None] = None,
-        post_delete: Callable[[HttpRequest, UUID], None] = None,
+        post_delete: Callable[[HttpRequest, Union[int, UUID]], None] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.pre_delete = pre_delete
         self.post_delete = post_delete
 
     def register_route(self, router: Router, model: Type[Model]) -> None:
         model_name = utils.to_snake_case(model.__name__)
@@ -31,15 +31,15 @@
             "/{id}",
             response={HTTPStatus.NO_CONTENT: None},
             url_name=model_name,
             operation_id=operation_id,
             summary=summary,
         )
         @merge_decorators(self.decorators)
-        def delete_model(request: HttpRequest, id: UUID):
+        def delete_model(request: HttpRequest, id: Union[int, UUID]):
             instance = model.objects.get(pk=id)
             if self.pre_delete is not None:
                 self.pre_delete(request, instance)
             instance.delete()
             if self.post_delete is not None:
                 self.post_delete(request, id)
             return HTTPStatus.NO_CONTENT, None
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/views/list.py` & `django_ninja_crud-0.1.3/ninja_crud/views/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class ListModelView(AbstractModelView):
     def __init__(
         self,
         output_schema: Type[Schema],
         filter_schema: Type[FilterSchema] = None,
         queryset_getter: Union[
-            Callable[[], QuerySet[Model]], Callable[[UUID], QuerySet[Model]]
+            Callable[[], QuerySet[Model]], Callable[[Union[int, UUID]], QuerySet[Model]]
         ] = None,
         related_model: Type[Model] = None,
         detail: bool = False,
         decorators: List[Callable] = None,
     ) -> None:
         super().__init__(decorators=decorators)
         self.output_schema = output_schema
@@ -81,15 +81,15 @@
             operation_id=operation_id,
             summary=summary,
         )
         @merge_decorators(self.decorators)
         @paginate(LimitOffsetPagination)
         def list_models(
             request: HttpRequest,
-            id: UUID,
+            id: Union[int, UUID],
             filters: filter_schema = Query(default=FilterSchema()),
         ):
             if self.get_queryset is not None:
                 queryset = self.get_queryset(id)
             else:
                 queryset = self.related_model.objects.get_queryset()
             return self.filter_queryset(queryset=queryset, filters=filters)
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/views/retrieve.py` & `django_ninja_crud-0.1.3/ninja_crud/views/retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import Callable, List, Type
+from typing import Callable, List, Type, Union
 from uuid import UUID
 
 from django.db.models import Model, QuerySet
 from django.http import HttpRequest
 from ninja import Router, Schema
 
 from ninja_crud import utils
@@ -33,14 +33,14 @@
             "/{id}",
             response={HTTPStatus.OK: output_schema},
             url_name=model_name,
             operation_id=operation_id,
             summary=summary,
         )
         @merge_decorators(self.decorators)
-        def retrieve_model(request: HttpRequest, id: UUID):
+        def retrieve_model(request: HttpRequest, id: Union[int, UUID]):
             if self.get_queryset is not None:
                 queryset = self.get_queryset(id)
             else:
                 queryset = model.objects.get_queryset()
             instance = queryset.get(pk=id)
             return HTTPStatus.OK, instance
```

### Comparing `django_ninja_crud-0.1.2/ninja_crud/views/update.py` & `django_ninja_crud-0.1.3/ninja_crud/views/update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http import HTTPStatus
-from typing import Callable, List, Type
+from typing import Callable, List, Type, Union
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router, Schema
 
 from ninja_crud import utils
@@ -38,15 +38,17 @@
             "/{id}",
             response={HTTPStatus.OK: output_schema},
             url_name=model_name,
             operation_id=operation_id,
             summary=summary,
         )
         @merge_decorators(self.decorators)
-        def update_model(request: HttpRequest, id: UUID, payload: input_schema):
+        def update_model(
+            request: HttpRequest, id: Union[int, UUID], payload: input_schema
+        ):
             instance = model.objects.get(id=id)
             for field, value in payload.dict(exclude_unset=True).items():
                 setattr(instance, field, value)
             if self.pre_save is not None:
                 self.pre_save(request, instance)
             instance.full_clean()
             instance.save()
```

### Comparing `django_ninja_crud-0.1.2/pyproject.toml` & `django_ninja_crud-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["ninja_crud", "tests", "examples"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "django-ninja-crud"
-version = "0.1.2"
+version = "0.1.3"
 description = "Django Ninja CRUD is a library that allows you to create CRUD APIs in a few lines of code."
 authors = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 maintainers = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hbakri/django-ninja-crud"
 license = "MIT"
 classifiers = [
@@ -35,15 +35,15 @@
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 packages = [{ include = "ninja_crud" },]
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
-Django = ">= 3.0"
+Django = ">= 3.2"
 django-ninja = ">= 0.21"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 pre-commit = "^2.20.0"
 
 [build-system]
```

