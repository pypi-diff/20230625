# Comparing `tmp/hat_asn1-0.6.5-cp38.cp39.cp310-none-any.whl.zip` & `tmp/hat_asn1-0.6.6-cp310.cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 22806 bytes, number of entries: 11
--rw-r--r--  2.0 unx     8663 b- defN 22-Apr-11 19:09 hat/asn1/__init__.py
--rw-r--r--  2.0 unx    23063 b- defN 22-Apr-11 19:09 hat/asn1/ber.py
--rw-r--r--  2.0 unx     8968 b- defN 22-Jul-16 17:17 hat/asn1/common.py
--rw-r--r--  2.0 unx     4615 b- defN 22-Apr-11 17:39 hat/asn1/doc.py
--rw-r--r--  2.0 unx    41443 b- defN 21-Jul-29 22:16 hat/asn1/parser.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-23 20:00 hat_asn1-0.6.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     1908 b- defN 23-Feb-23 20:00 hat_asn1-0.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx      132 b- defN 23-Feb-23 20:00 hat_asn1-0.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-23 20:00 hat_asn1-0.6.5.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-23 20:00 hat_asn1-0.6.5.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      852 b- defN 23-Feb-23 20:00 hat_asn1-0.6.5.dist-info/RECORD
-11 files, 101007 bytes uncompressed, 21382 bytes compressed:  78.8%
+Zip file size: 22864 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     8643 b- defN 23-Jun-25 12:49 hat/asn1/__init__.py
+-rw-r--r--  2.0 unx    23029 b- defN 23-Jun-25 12:50 hat/asn1/ber.py
+-rw-r--r--  2.0 unx     8777 b- defN 23-Jun-25 13:11 hat/asn1/common.py
+-rw-r--r--  2.0 unx     4593 b- defN 23-Jun-25 13:11 hat/asn1/doc.py
+-rw-r--r--  2.0 unx    41422 b- defN 23-Jun-25 13:12 hat/asn1/parser.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2331 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      852 b- defN 23-Jun-25 13:12 hat_asn1-0.6.6.dist-info/RECORD
+11 files, 101124 bytes uncompressed, 21440 bytes compressed:  78.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: hat/asn1/doc.py
 Comment: 
 
 Filename: hat/asn1/parser.py
 Comment: 
 
-Filename: hat_asn1-0.6.5.dist-info/LICENSE
+Filename: hat_asn1-0.6.6.dist-info/LICENSE
 Comment: 
 
-Filename: hat_asn1-0.6.5.dist-info/METADATA
+Filename: hat_asn1-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: hat_asn1-0.6.5.dist-info/WHEEL
+Filename: hat_asn1-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: hat_asn1-0.6.5.dist-info/top_level.txt
+Filename: hat_asn1-0.6.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_asn1-0.6.5.dist-info/zip-safe
+Filename: hat_asn1-0.6.6.dist-info/zip-safe
 Comment: 
 
-Filename: hat_asn1-0.6.5.dist-info/RECORD
+Filename: hat_asn1-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/asn1/__init__.py

```diff
@@ -140,15 +140,15 @@
             elif isinstance(arg, Repository):
                 self._refs.update(arg._refs)
 
             else:
                 raise ValueError('invalid argument')
 
     @staticmethod
-    def from_json(data: typing.Union[pathlib.PurePath, json.Data]
+    def from_json(data: pathlib.PurePath | json.Data
                   ) -> 'Repository':
         """Create repository from JSON data representation"""
         if isinstance(data, pathlib.PurePath):
             data = json.decode_file(data)
 
         repo = Repository()
         repo._refs = {common.type_from_json(k): common.type_from_json(v)
@@ -247,15 +247,15 @@
         if self._encoding == Encoding.BER:
             return ber.encode_entity(entity)
 
         raise ValueError('invalid encoding')
 
     def decode_entity(self,
                       data: Bytes
-                      ) -> typing.Tuple[Entity, Bytes]:
+                      ) -> tuple[Entity, Bytes]:
         """Decode entity from data
 
         Returns entity and remaining data.
 
         """
         if self._encoding == Encoding.BER:
             return ber.decode_entity(data)
```

## hat/asn1/ber.py

```diff
@@ -14,21 +14,21 @@
 class ConstructedContent(typing.NamedTuple):
     elements: typing.List['Entity']
 
 
 class Entity(typing.NamedTuple):
     class_type: common.ClassType
     tag_number: int
-    content: typing.Union[PrimitiveContent, ConstructedContent]
+    content: PrimitiveContent | ConstructedContent
 
 
 common.Entity.register(Entity)
 
 
-def encode_value(refs: typing.Dict[common.TypeRef, common.Type],
+def encode_value(refs: dict[common.TypeRef, common.Type],
                  t: common.Type,
                  value: common.Value
                  ) -> Entity:
     """Encode value to entity"""
     while isinstance(t, common.TypeRef):
         t = refs[t]
 
@@ -129,15 +129,15 @@
         return Entity(class_type=t.class_type,
                       tag_number=t.tag_number,
                       content=content)
 
     raise ValueError('invalid type definition')
 
 
-def decode_value(refs: typing.Dict[common.TypeRef, common.Type],
+def decode_value(refs: dict[common.TypeRef, common.Type],
                  t: common.Type,
                  entity: Entity
                  ) -> common.Value:
     """Decode value from entity"""
     while isinstance(t, common.TypeRef):
         t = refs[t]
 
@@ -276,15 +276,15 @@
 
     else:
         raise ValueError('invalid entity content')
 
     return bytes(entity_bytes)
 
 
-def decode_entity(data: common.Bytes) -> typing.Tuple[Entity, common.Bytes]:
+def decode_entity(data: common.Bytes) -> tuple[Entity, common.Bytes]:
     """Decode entity
 
     Returns entity and remaining data.
 
     """
     class_type = common.ClassType(data[0] >> 6)
     is_constructed = bool(data[0] & 0x20)
```

## hat/asn1/common.py

```diff
@@ -1,16 +1,15 @@
 import abc
 import enum
 import typing
 
 from hat import json
-from hat import util
 
 
-Bytes = typing.Union[bytes, bytearray, memoryview]
+Bytes = bytes | bytearray | memoryview
 
 
 class ClassType(enum.Enum):
     UNIVERSAL = 0
     APPLICATION = 1
     CONTEXT_SPECIFIC = 2
     PRIVATE = 3
@@ -82,28 +81,28 @@
 
 
 class EmbeddedPDVType(typing.NamedTuple):
     pass
 
 
 class ChoiceType(typing.NamedTuple):
-    choices: typing.List[TypeProperty]
+    choices: list[TypeProperty]
 
 
 class SetType(typing.NamedTuple):
-    elements: typing.List[TypeProperty]
+    elements: list[TypeProperty]
 
 
 class SetOfType(typing.NamedTuple):
     type: 'Type'
     "elements type definition"
 
 
 class SequenceType(typing.NamedTuple):
-    elements: typing.List[TypeProperty]
+    elements: list[TypeProperty]
 
 
 class SequenceOfType(typing.NamedTuple):
     type: 'Type'
     "elements type definition"
 
 
@@ -118,127 +117,131 @@
 class PrefixedType(typing.NamedTuple):
     type: 'Type'
     class_type: ClassType
     tag_number: int
     implicit: bool
 
 
-Type = typing.Union[TypeRef,
-                    BooleanType,
-                    IntegerType,
-                    BitStringType,
-                    OctetStringType,
-                    NullType,
-                    ObjectIdentifierType,
-                    StringType,
-                    ExternalType,
-                    RealType,
-                    EnumeratedType,
-                    EmbeddedPDVType,
-                    ChoiceType,
-                    SetType,
-                    SetOfType,
-                    SequenceType,
-                    SequenceOfType,
-                    EntityType,
-                    UnsupportedType,
-                    PrefixedType]
+Type: typing.TypeAlias = (TypeRef |
+                          BooleanType |
+                          IntegerType |
+                          BitStringType |
+                          OctetStringType |
+                          NullType |
+                          ObjectIdentifierType |
+                          StringType |
+                          ExternalType |
+                          RealType |
+                          EnumeratedType |
+                          EmbeddedPDVType |
+                          ChoiceType |
+                          SetType |
+                          SetOfType |
+                          SequenceType |
+                          SequenceOfType |
+                          EntityType |
+                          UnsupportedType |
+                          PrefixedType)
 """Type"""
 
 
-Boolean = bool
+Boolean: typing.TypeAlias = bool
 """Boolean"""
 
 
-Integer = int
+Integer: typing.TypeAlias = int
 """Integer"""
 
 
-BitString = typing.List[bool]
+BitString: typing.TypeAlias = list[bool]
 """Bit string"""
 
 
-OctetString = Bytes
+OctetString: typing.TypeAlias = Bytes
 """Octet string"""
 
 
-Null = None
+Null: typing.TypeAlias = None
 """Null"""
 
 
-ObjectIdentifier = typing.Tuple[int, ...]
+ObjectIdentifier: typing.TypeAlias = tuple[int, ...]
 """Object identifier"""
 
 
-String = str
+String: typing.TypeAlias = str
 """String"""
 
 
 class External(typing.NamedTuple):
-    data: typing.Union['Entity', Bytes, typing.List[bool]]
-    direct_ref: typing.Optional[ObjectIdentifier]
-    indirect_ref: typing.Optional[int]
+    data: typing.Union['Entity', Bytes, list[bool]]
+    direct_ref: ObjectIdentifier | None
+    indirect_ref: int | None
 
 
-Real = float
+Real: typing.TypeAlias = float
 """Real"""
 
 
-Enumerated = int
+Enumerated: typing.TypeAlias = int
 """Enumerated"""
 
 
-# TODO: if abstract is ObjectIdentifier then transfer must be defined
 class EmbeddedPDV(typing.NamedTuple):
-    abstract: typing.Optional[typing.Union[int, ObjectIdentifier]]
-    transfer: typing.Optional[ObjectIdentifier]
+    """EmbeddedPDV
+
+    If `abstract` is `ObjectIdentifier`, `transfer` must be defined
+
+    """
+    abstract: int | ObjectIdentifier | None
+    transfer: ObjectIdentifier | None
     data: Bytes
 
 
-Choice = typing.Tuple[str, 'Value']
+Choice: typing.TypeAlias = typing.Tuple[str, 'Value']
 """Choice"""
 
 
-Set = typing.Dict[str, 'Value']
+Set: typing.TypeAlias = typing.Dict[str, 'Value']
 """Set"""
 
 
-SetOf = typing.Iterable['Value']
+SetOf: typing.TypeAlias = typing.Iterable['Value']
 """Set of"""
 
 
-Sequence = typing.Dict[str, 'Value']
+Sequence: typing.TypeAlias = typing.Dict[str, 'Value']
 """Sequence"""
 
 
-SequenceOf = typing.List['Value']
+SequenceOf: typing.TypeAlias = typing.List['Value']
 """Sequence of"""
 
 
 class Entity(abc.ABC):
     """Encoding independent ASN.1 Entity"""
 
 
-Value = typing.Union[Boolean,
-                     Integer,
-                     BitString,
-                     OctetString,
-                     Null,
-                     ObjectIdentifier,
-                     String,
-                     External,
-                     Real,
-                     Enumerated,
-                     EmbeddedPDV,
-                     Choice,
-                     Set,
-                     SetOf,
-                     Sequence,
-                     SequenceOf,
-                     Entity]
+Value: typing.TypeAlias = (Boolean |
+                           Integer |
+                           BitString |
+                           OctetString |
+                           Null |
+                           ObjectIdentifier |
+                           String |
+                           External |
+                           Real |
+                           Enumerated |
+                           EmbeddedPDV |
+                           Choice |
+                           Set |
+                           SetOf |
+                           Sequence |
+                           SequenceOf |
+                           Entity)
 """Value"""
 
 
 def type_to_json(t: Type) -> json.Data:
     """Convert type definition to JSON data"""
     if isinstance(t, TypeRef):
         return ['TypeRef', t.module, t.name]
@@ -378,26 +381,7 @@
     if data[0] == 'PrefixedType':
         return PrefixedType(type=type_from_json(data[1]),
                             class_type=ClassType[data[2]],
                             tag_number=data[3],
                             implicit=data[4])
 
     raise ValueError('invalid data')
-
-
-# HACK type alias
-util.register_type_alias('Type')
-util.register_type_alias('Boolean')
-util.register_type_alias('Integer')
-util.register_type_alias('BitString')
-util.register_type_alias('OctetString')
-util.register_type_alias('Null')
-util.register_type_alias('ObjectIdentifier')
-util.register_type_alias('String')
-util.register_type_alias('Real')
-util.register_type_alias('Enumerated')
-util.register_type_alias('Choice')
-util.register_type_alias('Set')
-util.register_type_alias('SetOf')
-util.register_type_alias('Sequence')
-util.register_type_alias('SequenceOf')
-util.register_type_alias('Value')
```

## hat/asn1/doc.py

```diff
@@ -1,13 +1,11 @@
-import typing
-
 from hat.asn1 import common
 
 
-def generate_html(refs: typing.Dict[common.TypeRef, common.Type]
+def generate_html(refs: dict[common.TypeRef, common.Type]
                   ) -> str:
     """Generate HTML documentation"""
     modules = {}
     for ref, t in refs.items():
         if ref.module not in modules:
             modules[ref.module] = {}
         modules[ref.module][ref] = t
```

## hat/asn1/parser.py

```diff
@@ -1,17 +1,16 @@
 import itertools
-import typing
 
 from hat import util
 from hat import peg
 from hat.asn1 import common
 
 
 def parse(asn1_def: str
-          ) -> typing.Dict[common.TypeRef, common.Type]:
+          ) -> dict[common.TypeRef, common.Type]:
     """Parse ASN.1"""
     ast = _grammar.parse(asn1_def)
     refs = peg.walk_ast(ast, _actions)
     return refs
 
 
 def _act_Root(n, c):
```

## Comparing `hat_asn1-0.6.5.dist-info/LICENSE` & `hat_asn1-0.6.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_asn1-0.6.5.dist-info/METADATA` & `hat_asn1-0.6.6.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,88 @@
 Metadata-Version: 2.1
 Name: hat-asn1
-Version: 0.6.5
+Version: 0.6.6
 Summary: Hat ASN.1 parser and encoder
 Home-page: https://github.com/hat-open/hat-asn1
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: hat-json (~=0.5.15)
-Requires-Dist: hat-peg (~=0.5.6)
-Requires-Dist: hat-util (~=0.6.7)
+Requires-Dist: hat-json (~=0.5.19)
+Requires-Dist: hat-peg (~=0.5.7)
+Requires-Dist: hat-util (~=0.6.10)
+
+.. _online documentation: https://hat-asn1.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-asn1.git
+.. _PyPI project: https://pypi.org/project/hat-asn1
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
+
 
 hat-asn1 - Abstract Syntax Notation One
 =======================================
 
-This library is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
-
-Development of Hat Open and associated repositories is sponsored by
-`Končar Digital <https://www.koncar.hr>`_.
-
 For more information see:
 
-    * hat-asn1 documentation - `<https://hat-asn1.hat-open.com>`_
-    * hat-asn1 git repository - `<https://github.com/hat-open/hat-asn1.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
+* `online documentation`_
+* `git repository`_
+
 
-.. warning::
+Runtime requirements
+--------------------
 
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+* python >=3.10
 
 
 Install
 -------
 
-::
+`hat-asn1` is available as `PyPI project`_::
 
     $ pip install hat-asn1
 
 
+Build
+-----
+
+Build tool used for `hat-asn1` is `pydoit`_. It can be installed together
+with other python dependencies by running::
+
+    $ pip install -r requirements.pip.dev.txt
+
+For listing available doit tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-asn1` is part of `Hat Open`_ project - open-source framework of tools
+and libraries for developing applications used for remote monitoring, control
+and management of intelligent electronic devices such as IoT devices, PLCs,
+industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2022 Hat Open AUTHORS
+Copyright 2020-2023 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `hat_asn1-0.6.5.dist-info/RECORD` & `hat_asn1-0.6.6.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-hat/asn1/__init__.py,sha256=WQHl1vVTmYP6nabklURxmtWmMxv3HAFeHhxr13eKXrQ,8663
-hat/asn1/ber.py,sha256=81aaicLZAMV2mKIHSjuCPTbWOuY0GgjbsN8kjGBxufc,23063
-hat/asn1/common.py,sha256=P4l9sno-Ii2VX1_WQl8N-Nkk_8W0z_uchLvQ8U2ox1U,8968
-hat/asn1/doc.py,sha256=F21VqsusBxLGovyeWUf1lh6o4TKT1MUjTL1Td0Sge1o,4615
-hat/asn1/parser.py,sha256=uQjcOPr48bZvBE6KnHZMGSwey7jx65STS7Iba0Ymyb0,41443
-hat_asn1-0.6.5.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_asn1-0.6.5.dist-info/METADATA,sha256=eUfQ9j1A3kuZykTpr97QffSQdjqSZFzLaNv0PvZv1B0,1908
-hat_asn1-0.6.5.dist-info/WHEEL,sha256=CV8iyE3A7V2uhg9OaTlpshab_dzxBhIEuLDh8OHPmAw,132
-hat_asn1-0.6.5.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_asn1-0.6.5.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-hat_asn1-0.6.5.dist-info/RECORD,,
+hat/asn1/__init__.py,sha256=9AMkL1I0AFTPZPl_Rzj2zKPCvTjDUbEmWY2vm0_pW7c,8643
+hat/asn1/ber.py,sha256=eRl6AyzZFU1_ovUHS-LJlPAgxkh-q7IDdMLaH1N4mUc,23029
+hat/asn1/common.py,sha256=_kRG4DK7kWnNnPOqO0IXD_D9p3PacgDOYFduTUkdht8,8777
+hat/asn1/doc.py,sha256=YGCVBxS_d_fAlTqZG1Wb-iq8_oz0J_KJ9Eqyjd1UuLI,4593
+hat/asn1/parser.py,sha256=G4w4KsyxjcmarMyIUCkj4ruMgrHbQ0j_48hcXbQb8KY,41422
+hat_asn1-0.6.6.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_asn1-0.6.6.dist-info/METADATA,sha256=Ziui-tY9JRE7d_ObxdpgxbEgqtq9WbvVs60XrIci6z8,2331
+hat_asn1-0.6.6.dist-info/WHEEL,sha256=md_Sk-cFyicIH6eY_0BVqmsgC0wAFfbS1oq2bLoZiOk,114
+hat_asn1-0.6.6.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
+hat_asn1-0.6.6.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+hat_asn1-0.6.6.dist-info/RECORD,,
```

