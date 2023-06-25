# Comparing `tmp/sqlalchemy_model_builder-0.1.0.tar.gz` & `tmp/sqlalchemy_model_builder-0.2.0.tar.gz`

## Comparing `sqlalchemy_model_builder-0.1.0.tar` & `sqlalchemy_model_builder-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/exceptions.py
--rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/model_builder.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/models.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/random_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/test_model_builder_primitive_types.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/test_model_builder_relationships.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/tests/test_random_builder.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/LICENSE
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/README.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/_models.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/exceptions.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/model_builder.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/random_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/test_model_builder_relationships.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/test_model_builder_types.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/test_random_builder.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/README.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/PKG-INFO
```

### Comparing `sqlalchemy_model_builder-0.1.0/.github/workflows/publish.yml` & `sqlalchemy_model_builder-0.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/.github/workflows/test.yml` & `sqlalchemy_model_builder-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/model_builder.py` & `sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/model_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 from datetime import date, datetime, time, timedelta
-from typing import Any, Callable, Optional, Type
+from typing import Any, Generic, Optional, Type, TypeVar
+from uuid import UUID
 
 from sqlalchemy import inspect
 from sqlalchemy.exc import NoInspectionAvailable
 from sqlalchemy.orm import Mapper, Session
 
+from sqlalchemy_model_builder._models import ColumnValuePair, ColumnValuePairList
 from sqlalchemy_model_builder.exceptions import ModelBuilderException
-from sqlalchemy_model_builder.models import ColumnValuePair, ColumnValuePairList
 from sqlalchemy_model_builder.random_builder import RandomBuilder
 
+T = TypeVar("T")
 
-class ModelBuilder:
-    def __init__(self, db_model: Type, minimal: bool = False):
+_TYPE_MAPPING = {
+    bool: RandomBuilder.next_bool,
+    bytes: RandomBuilder.next_bytes,
+    date: RandomBuilder.next_date,
+    datetime: RandomBuilder.next_datetime,
+    float: RandomBuilder.next_float,
+    int: RandomBuilder.next_int,
+    str: RandomBuilder.next_str,
+    time: RandomBuilder.next_time,
+    timedelta: RandomBuilder.next_timedelta,
+    UUID: RandomBuilder.next_uuid,
+}
+
+
+class ModelBuilder(Generic[T]):
+    def __init__(self, db_model: Type[T], minimal: bool = False):
         self.db: Optional[Session] = None
-        self.db_model: Type = db_model
-        self.minimal: bool = minimal
+        self.db_model = db_model
+        self.minimal = minimal
 
-    def build(self, **attrs: Any) -> Any:
+    def build(self, **attrs: Any) -> T:
         """Build SQLAlchemy model with random data and
         return it without persisting into database.
 
         :returns: a SQLAlchemy database model with generated random data
         :rtype: Any
         """
         try:
@@ -37,15 +53,15 @@
         except TypeError as sqlalchemy_exception:
             raise ModelBuilderException(
                 f"Invalid fields for model: {self.db_model}"
             ) from sqlalchemy_exception
 
         return instance
 
-    def save(self, db: Session, **attrs: Any) -> Any:
+    def save(self, db: Session, **attrs: Any) -> T:
         """Build SQLAlchemy model with random data and
         persist it into database using provided db.
 
         :param db: SQLAlchemy database session
         :type db: Session
         :returns: a SQLAlchemy database model with generated random data
         :rtype: Any
@@ -115,49 +131,31 @@
 
             if self.minimal and column.nullable:
                 continue
 
             if column.foreign_keys:
                 continue
 
-            random_value = self.__map_field_to_random_builder_method(python_type)()
+            if column.type.__class__.__name__ == "Enum":
+                random_value = RandomBuilder.next_from_list(column.type.enums)
+            else:
+                random_value = self.__map_field_to_random_builder_method(python_type)()
+
             column_value = ColumnValuePair(column.key, random_value)
             column_values.append(column_value)
 
         return ColumnValuePairList(column_values)
 
-    def __map_field_to_random_builder_method(
-        self, field_type: type
-    ) -> Callable[[], Any]:
+    def __map_field_to_random_builder_method(self, field_type: type) -> Any:
         """Mapping between field type and RandomBuilder methods
 
         :returns: a RandomBuilder method for the provided type
         :rtype: function
         """
-        func: Callable[[], Any] = RandomBuilder.next_str
-
-        if field_type == bool:
-            func = RandomBuilder.next_bool
-        elif field_type == bytes:
-            func = RandomBuilder.next_bytes
-        elif field_type == date:
-            func = RandomBuilder.next_date
-        elif field_type == datetime:
-            func = RandomBuilder.next_datetime
-        elif field_type == float:
-            func = RandomBuilder.next_float
-        elif field_type == int:
-            func = RandomBuilder.next_int
-        elif field_type == str:
-            func = RandomBuilder.next_str
-        elif field_type == time:
-            func = RandomBuilder.next_time
-        elif field_type == timedelta:
-            func = RandomBuilder.next_timedelta
 
-        return func
+        return _TYPE_MAPPING.get(field_type, RandomBuilder.next_str)
 
-    def __save(self, instance: Any) -> None:
+    def __save(self, instance: T) -> None:
         assert self.db is not None
 
         self.db.add(instance)
         self.db.commit()
```

### Comparing `sqlalchemy_model_builder-0.1.0/sqlalchemy_model_builder/random_builder.py` & `sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/random_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
 import random
 import string
-import typing
 import uuid
 from datetime import date, datetime, time, timedelta, timezone
+from typing import Any, List, Type
 
 
 class RandomBuilder:
     @classmethod
     def next_bool(cls) -> bool:
         return random.choice([True, False])
 
@@ -35,24 +35,28 @@
         )
 
     @classmethod
     def next_datetime_utc(cls) -> datetime:
         return cls.next_datetime().astimezone(timezone.utc)
 
     @classmethod
-    def next_enum(cls, e: typing.Type[enum.Enum]) -> typing.Any:
+    def next_enum(cls, e: Type[enum.Enum]) -> Any:
         return random.choice([item.value for item in e])
 
     @classmethod
     def next_float(
         cls, minimum: float = 0, maximum: float = 2147483647, precision: int = 5
     ) -> float:
         return round(random.uniform(minimum, maximum), precision)
 
     @classmethod
+    def next_from_list(cls, seq: List[Any]) -> Any:
+        return random.choice(seq)
+
+    @classmethod
     def next_int(cls, minimum: int = 0, maximum: int = 2147483647) -> int:
         return random.randint(minimum, maximum)
 
     @classmethod
     def next_int64(cls, minimum: int = 0, maximum: int = 9223372036854775807) -> int:
         return random.randint(minimum, maximum)
```

### Comparing `sqlalchemy_model_builder-0.1.0/tests/test_model_builder_relationships.py` & `sqlalchemy_model_builder-0.2.0/tests/test_model_builder_relationships.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session, relationship, sessionmaker
 
 from sqlalchemy_model_builder import ModelBuilder, ModelBuilderException
 
 Base = declarative_base()
 
-engine = create_engine("sqlite://", echo=True)
+engine = create_engine("sqlite://")
 
 
 class Address(Base):
     __tablename__ = "addresses"
 
     id = Column(Integer, primary_key=True)
     user_id = Column(Integer, ForeignKey("users.id"))
@@ -30,15 +30,15 @@
 Base.metadata.create_all(engine)
 
 LocalSession = sessionmaker(bind=engine)
 
 db: Session = LocalSession()
 
 
-class TestModelBuilderPrimitiveTypes(unittest.TestCase):
+class TestModelBuilderRelationships(unittest.TestCase):
     def test_build_model_with_foreign_key(self):
         ModelBuilder(Address).build()
 
     def test_build_related_model_and_use_in_build(self):
         user = ModelBuilder(User).build()
         address = ModelBuilder(Address).build(user_id=user.id)
```

### Comparing `sqlalchemy_model_builder-0.1.0/tests/test_random_builder.py` & `sqlalchemy_model_builder-0.2.0/tests/test_random_builder.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/.gitignore` & `sqlalchemy_model_builder-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/LICENSE` & `sqlalchemy_model_builder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/README.md` & `sqlalchemy_model_builder-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/pyproject.toml` & `sqlalchemy_model_builder-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.1.0/PKG-INFO` & `sqlalchemy_model_builder-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-model-builder
-Version: 0.1.0
+Version: 0.2.0
 Summary: SQLAlchemy Model Builder
 Project-URL: Documentation, https://github.com/aminalaee/sqlalchemy-model-builder
 Project-URL: Issues, https://github.com/aminalaee/sqlalchemy-model-builder/issues
 Project-URL: Source, https://github.com/aminalaee/sqlalchemy-model-builder
 Author-email: Amin Alaee <me@aminalaee.dev>
 License-Expression: MIT
 License-File: LICENSE
```

