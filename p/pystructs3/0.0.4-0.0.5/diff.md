# Comparing `tmp/pystructs3-0.0.4.tar.gz` & `tmp/pystructs3-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructs3-0.0.4.tar", last modified: Thu Apr 27 05:17:19 2023, max compression
+gzip compressed data, was "pystructs3-0.0.5.tar", last modified: Sun Jun 25 07:59:48 2023, max compression
```

## Comparing `pystructs3-0.0.4.tar` & `pystructs3-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.4/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-27 05:17:19.737077 pystructs3-0.0.4/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.4/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/pystructs/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      681 2023-04-21 06:27:06.000000 pystructs3-0.0.4/pystructs/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8814 2023-04-23 23:27:43.000000 pystructs3-0.0.4/pystructs/base.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1928 2023-04-19 00:40:15.000000 pystructs3-0.0.4/pystructs/codec.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2798 2023-04-21 06:25:07.000000 pystructs3-0.0.4/pystructs/list.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/pystructs/struct/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      332 2023-04-19 00:33:47.000000 pystructs3-0.0.4/pystructs/struct/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3060 2023-04-27 05:16:33.000000 pystructs3-0.0.4/pystructs/struct/fields.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5133 2023-04-21 07:24:30.000000 pystructs3-0.0.4/pystructs/struct/struct.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-27 05:17:19.737077 pystructs3-0.0.4/pystructs3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      355 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-27 05:17:19.000000 pystructs3-0.0.4/pystructs3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-27 05:17:19.737077 pystructs3-0.0.4/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-27 05:16:52.000000 pystructs3-0.0.4/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:59:48.017256 pystructs3-0.0.5/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.5/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-06-25 07:59:48.017256 pystructs3-0.0.5/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.5/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:59:48.017256 pystructs3-0.0.5/pystructs/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1522 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2445 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/bytestr.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3997 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/codec.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2359 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/helpers.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3715 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/integer.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3178 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/lists.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4900 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/net.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2662 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:59:48.017256 pystructs3-0.0.5/pystructs/tests/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      323 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1538 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/bytestr.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1432 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/helpers.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2156 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/integer.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1824 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/lists.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2336 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/net.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1471 2023-06-25 07:59:42.000000 pystructs3-0.0.5/pystructs/tests/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:59:48.017256 pystructs3-0.0.5/pystructs3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-06-25 07:59:47.000000 pystructs3-0.0.5/pystructs3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      538 2023-06-25 07:59:48.000000 pystructs3-0.0.5/pystructs3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-25 07:59:47.000000 pystructs3-0.0.5/pystructs3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       28 2023-06-25 07:59:47.000000 pystructs3-0.0.5/pystructs3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-06-25 07:59:47.000000 pystructs3-0.0.5/pystructs3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-25 07:59:48.017256 pystructs3-0.0.5/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      761 2023-06-25 07:59:42.000000 pystructs3-0.0.5/setup.py
```

### Comparing `pystructs3-0.0.4/LICENSE` & `pystructs3-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.4/PKG-INFO` & `pystructs3-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 PyStructs
 ---------
 Dataclass-Like Serialization Helpers for More Complex Data-Types
```

### Comparing `pystructs3-0.0.4/README.md` & `pystructs3-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.4/pystructs/list.py` & `pystructs3-0.0.5/pystructs/lists.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,105 @@
 """
 List Codec Implementations
 """
-from typing import Type, List, Any
+from typing import Protocol, ClassVar, Type, Generic, List, Tuple
 
-from .base import Int, codec
-from .codec import Context, Codec
+from .codec import *
+from .integer import I, Integer
 
 #** Variables **#
 __all__ = ['SizedList', 'StaticList', 'GreedyList']
 
 #** Classes **#
 
-class SizedList(Codec):
+@protocol
+class SizedList(Codec[T], Protocol[I, T]):
     """
     Variable Sized List controlled by a Size-Hint Prefix
     """
-    hint:      Int
-    content:   Type[Codec]
-    base_type: type = list
+    hint:      ClassVar[Integer]
+    content:   ClassVar[Codec]
+    base_type: ClassVar[tuple] = (list, )
+
+    def __class_getitem__(cls, s: Tuple[I, T]):
+        hint, content = s
+        hint, content = deanno(hint, Integer), deanno(content, Codec)
+        name = f'{cname(cls)}[{hint!r},{content!r}]'
+        return type(name, (cls, ), {'hint': hint, 'content': content})
  
-    def __class_getitem__(cls, hint: int, content: Type[Codec]) -> Type[Codec]:
-        name   = f'{cls.__name__}[{hint!r},{content!r}]'
-        hcodec = Int[hint]
-        return codec(name, cls, hint=hcodec, content=content)
- 
-    @classmethod
-    def encode(cls, ctx: Context, value: List[Any]) -> bytes:
+    @protomethod
+    def encode(cls, ctx: Context, value: List[T]) -> bytes:
         data  = bytearray()
         data += cls.hint.encode(ctx, len(value))
         for item in value:
             data += cls.content.encode(ctx, item)
         return bytes(data)
 
-    @classmethod
-    def decode(cls, ctx: Context, value: bytes) -> List[Any]:
-        size    = cls.hint.decode(ctx, value)
+    @protomethod
+    def decode(cls, ctx: Context, raw: bytes) -> List[T]:
+        size    = cls.hint.decode(ctx, raw)
         content = []
         for _ in range(0, size):
-            item = cls.content.decode(ctx, value)
+            item = cls.content.decode(ctx, raw)
             content.append(item)
         return content
 
-class StaticList(Codec):
+@protocol
+class StaticList(Codec[T], Protocol, Generic[I, T]):
     """
     Static List of the specified-type
     """
-    size:      int
-    content:   Type[Codec]
-    base_type: type = list
-
-    def __class_getitem__(cls, size: int, content: Type[Codec]) -> Type[Codec]:
-        name = f'{cls.__name__}[{size!r},{content!r}]'
-        return codec(name, cls, size=size, content=content)
+    size:      ClassVar[int]
+    content:   ClassVar[Type[Codec]]
+    base_type: ClassVar[tuple] = (list, )
+
+    def __class_getitem__(cls, s: Tuple[I, T]):
+        size, content = s
+        size    = deanno(size, int)
+        content = deanno(content, Codec)
+        name    = f'{cname(cls)}[{size!r},{content!r}]'
+        return type(name, (cls,), {'size': size, 'content': content})
  
-    @classmethod
-    def encode(cls, ctx: Context, value: List[Any]) -> bytes:
-        assert len(value) == cls.size, f'len(array)[{len(value)}] != f{cls.size}'
+    @protomethod
+    def encode(cls, ctx: Context, value: List[T]) -> bytes:
+        if len(value) != cls.size:
+            raise CodecError(f'arraylen={len(value)} != {cls.size}')
         data = bytearray()
         for item in value:
             data += cls.content.encode(ctx, item)
         return bytes(data)
 
-    @classmethod
-    def decode(cls, ctx: Context, value: Any) -> list:
+    @protomethod
+    def decode(cls, ctx: Context, raw: bytes) -> List[T]:
         content = []
         for _ in range(0, cls.size):
-            item = cls.content.decode(ctx, value)
+            item = cls.content.decode(ctx, raw)
             content.append(item)
         return content
 
-class GreedyList(Codec):
+@protocol
+class GreedyList(Codec[T], Protocol):
     """
     Greedy List that Consumes All Remaining Bytes
     """
-    content:   Type[Codec]
-    base_type: type = list
+    content:   ClassVar[Type[Codec]]
+    base_type: ClassVar[tuple] = (list, )
 
-    def __class_getitem__(cls, content: Type[Codec]) -> Type[Codec]:
-        name = f'{cls.__name__}[{content!r}]'
-        return codec(name, cls, content=content)
+    def __class_getitem__(cls, anno_content: T):
+        content = deanno(anno_content, Codec)
+        name    = f'{cname(cls)}[{content!r}]'
+        return type(name, (cls,), {'content': content})
 
-    @classmethod
-    def encode(cls, ctx: Context, value: Any) -> bytes:
+    @protomethod
+    def encode(cls, ctx: Context, value: List[T]) -> bytes:
         data = bytearray()
         for item in value:
             data += cls.content.encode(ctx, item)
         return bytes(data)
 
-    @classmethod
-    def decode(cls, ctx: Context, raw: bytes) -> Any:
+    @protomethod
+    def decode(cls, ctx: Context, raw: bytes) -> List[T]:
         content = []
         while ctx.index < len(raw):
             item = cls.content.decode(ctx, raw)
             content.append(item)
         return content
```

### Comparing `pystructs3-0.0.4/pystructs3.egg-info/PKG-INFO` & `pystructs3-0.0.5/pystructs3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 PyStructs
 ---------
 Dataclass-Like Serialization Helpers for More Complex Data-Types
```

### Comparing `pystructs3-0.0.4/setup.py` & `pystructs3-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pystructs3',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pystruct',
     description="Dataclass-Like Serialization Helpers for More Complex Data-Types",
     long_description=readme,
     long_description_content_type="text/markdown",
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     packages=find_packages(),
     install_requires=[
-        'dataclasses',
+        'pyderive3',
         'typing_extensions'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
```

