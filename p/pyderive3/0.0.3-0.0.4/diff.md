# Comparing `tmp/pyderive3-0.0.3.tar.gz` & `tmp/pyderive3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyderive3-0.0.3.tar", last modified: Tue Jun 20 16:47:30 2023, max compression
+gzip compressed data, was "pyderive3-0.0.4.tar", last modified: Sun Jun 25 07:58:23 2023, max compression
```

## Comparing `pyderive3-0.0.3.tar` & `pyderive3-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-20 16:47:30.588375 pyderive3-0.0.3/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2391 2023-06-20 16:45:30.000000 pyderive3-0.0.3/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/pyderive/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1091 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3212 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/abc.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2980 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/compat.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    10059 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/compile.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)    11349 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/dataclasses.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5695 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/parse.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/pyderive/tests/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      119 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/tests/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2642 2023-06-20 16:45:30.000000 pyderive3-0.0.3/pyderive/tests/dataclasses.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-20 16:47:30.588375 pyderive3-0.0.3/pyderive3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      357 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-06-20 16:47:30.000000 pyderive3-0.0.3/pyderive3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-20 16:47:30.588375 pyderive3-0.0.3/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-06-20 16:45:55.000000 pyderive3-0.0.3/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:58:23.407981 pyderive3-0.0.4/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-25 07:58:23.407981 pyderive3-0.0.4/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2391 2023-05-28 09:26:37.000000 pyderive3-0.0.4/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:58:23.407981 pyderive3-0.0.4/pyderive/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1091 2023-05-28 09:09:02.000000 pyderive3-0.0.4/pyderive/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3212 2023-06-24 00:39:03.000000 pyderive3-0.0.4/pyderive/abc.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7980 2023-06-24 03:59:51.000000 pyderive3-0.0.4/pyderive/compat.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    10103 2023-06-24 00:38:08.000000 pyderive3-0.0.4/pyderive/compile.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    11400 2023-06-23 05:33:39.000000 pyderive3-0.0.4/pyderive/dataclasses.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5936 2023-06-23 05:34:23.000000 pyderive3-0.0.4/pyderive/parse.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:58:23.407981 pyderive3-0.0.4/pyderive/tests/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      119 2023-05-28 08:41:00.000000 pyderive3-0.0.4/pyderive/tests/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2642 2023-05-28 20:41:04.000000 pyderive3-0.0.4/pyderive/tests/dataclasses.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-06-25 07:58:23.407981 pyderive3-0.0.4/pyderive3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2816 2023-06-25 07:58:23.000000 pyderive3-0.0.4/pyderive3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      357 2023-06-25 07:58:23.000000 pyderive3-0.0.4/pyderive3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-06-25 07:58:23.000000 pyderive3-0.0.4/pyderive3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       18 2023-06-25 07:58:23.000000 pyderive3-0.0.4/pyderive3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-06-25 07:58:23.000000 pyderive3-0.0.4/pyderive3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-06-25 07:58:23.407981 pyderive3-0.0.4/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      708 2023-06-25 07:58:03.000000 pyderive3-0.0.4/setup.py
```

### Comparing `pyderive3-0.0.3/PKG-INFO` & `pyderive3-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyderive3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python3 Custom Data Class Helpers
 Home-page: https://github.com/imgurbot12/pyderive
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyderive3-0.0.3/README.md` & `pyderive3-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyderive3-0.0.3/pyderive/__init__.py` & `pyderive3-0.0.4/pyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `pyderive3-0.0.3/pyderive/abc.py` & `pyderive3-0.0.4/pyderive/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 class FieldDef(Protocol):
     name:            str
     anno:            Type
     default:         Any            = MISSING
     default_factory: DefaultFactory = MISSING
     init:            bool           = True
     repr:            bool           = True
-    hash:            bool           = True
+    hash:            Optional[bool] = None
     compare:         bool           = True
     kw_only:         bool           = False
     frozen:          bool           = False
     field_type:      FieldType      = FieldType.STANDARD
  
     @abstractmethod
     def __init__(self, name: str, anno: Type, default: Any = MISSING):
@@ -76,15 +76,15 @@
     def __init__(self,
         name:            str,
         anno:            Type,
         default:         Any            = MISSING,
         default_factory: DefaultFactory = MISSING,
         init:            bool           = True,
         repr:            bool           = True,
-        hash:            bool           = True,
+        hash:            Optional[bool] = None,
         compare:         bool           = True,
         kw_only:         bool           = False,
         frozen:          bool           = False,
         field_type:      FieldType      = FieldType.STANDARD
     ):
         self.name            = name
         self.anno            = anno
```

### Comparing `pyderive3-0.0.3/pyderive/compile.py` & `pyderive3-0.0.4/pyderive/compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,16 @@
 def create_hash(fields: Fields) -> Callable:
     """
     generate hash-function for hashable fields
 
     :param fields: ordered fields used to generate hash-function
     :return:       hash-function
     """
-    names   = [f.name for f in _stdfields(fields) if f.hash]
+    names   = [f.name for f in _stdfields(fields) 
+        if (f.compare if f.hash is None else f.hash)]
     names_t = _tuple_str(names, 'self')
     return _create_fn('__hash__', ['self'], [f'return hash({names_t})'])
 
 def assign_func(cls: Type, func: Callable, 
     name: Optional[str] = None, overwrite: bool = False) -> bool:
     """
     assign function to the object and modify qualname
```

### Comparing `pyderive3-0.0.3/pyderive/dataclasses.py` & `pyderive3-0.0.4/pyderive/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,16 @@
     if match_args:
         match = tuple(f.name for f in fields if f.init)
         assign_func(cls, match, '__match_args__') #type: ignore
     # add slots
     if slots:
         cls = add_slots(cls, fields, freeze)
     # update abstraction-methods on re-creation and return
-    abc.update_abstractmethods(cls)
+    if hasattr(abc, 'update_abstractmethods'):
+        abc.update_abstractmethods(cls)
     return cls
 
 @overload
 @dataclass_transform(field_specifiers=(FieldDef, Field, field))
 def dataclass(cls: Type[T], 
     init:        Optional[bool] = None,
     repr:        Optional[bool] = None,
```

### Comparing `pyderive3-0.0.3/pyderive/parse.py` & `pyderive3-0.0.4/pyderive/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 DataClass Parsing Tools
 """
+from types import MemberDescriptorType
 from typing import Type, Optional, ClassVar, get_origin
 
 from .abc import *
 from .compat import is_stddataclass, convert_fields
 
 #** Variables **#
 __all__ = [
@@ -75,16 +76,18 @@
         annotations = getattr(base, '__annotations__', {})
         for name, anno in annotations.items():
             # handle ClassVar
             if get_origin(anno) is ClassVar:
                 remove_field(fields, name)
                 continue
             # retrieve default-value of variable (if exists)
-            default = getattr(base, name, MISSING)
-            if delete and hasattr(base, name):
+            default     = getattr(base, name, MISSING)
+            member_desc = isinstance(default, MemberDescriptorType)
+            default     = MISSING if member_desc else default
+            if delete and hasattr(base, name) and not member_desc:
                 delattr(base, name)
             # preserve order of fields and add vardef
             if name not in fields.order:
                 fields.order.append(name)
             # assign field based on value
             if isinstance(default, ftype):
                 field      = default
@@ -142,15 +145,16 @@
             default = has_default(field)
             missing = name not in struct.fields
             if default and field.init and not field.kw_only:
                 kwargs.add(name)
             elif name in kwargs:
                 kwargs.remove(name)
             # raise error if non-kwarg found after kwargs start
-            if order_kw and kwargs and missing and not default:
+            kwarg = not field.kw_only and kwargs
+            if order_kw and kwarg and missing and not default:
                 raise TypeError(
                     f'non-default argument {name!r} follows default argument')
             # append vardef to order and set/replace definition
             if missing:
                 struct.order.append(name)
             struct.fields[name] = field
     return struct.ordered_fields()
```

### Comparing `pyderive3-0.0.3/pyderive/tests/dataclasses.py` & `pyderive3-0.0.4/pyderive/tests/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyderive3-0.0.3/pyderive3.egg-info/PKG-INFO` & `pyderive3-0.0.4/pyderive3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyderive3
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python3 Custom Data Class Helpers
 Home-page: https://github.com/imgurbot12/pyderive
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyderive3-0.0.3/setup.py` & `pyderive3-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pyderive3',
-    version='0.0.3',
+    version='0.0.4',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pyderive',
     description="Python3 Custom Data Class Helpers",
     long_description=readme,
     long_description_content_type="text/markdown",
```

