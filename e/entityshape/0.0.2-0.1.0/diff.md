# Comparing `tmp/entityshape-0.0.2.tar.gz` & `tmp/entityshape-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entityshape-0.0.2.tar", max compression
+gzip compressed data, was "entityshape-0.1.0.tar", max compression
```

## Comparing `entityshape-0.0.2.tar` & `entityshape-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-06-23 08:56:36.556587 entityshape-0.0.2/LICENSE
--rw-r--r--   0        0        0     2865 2023-06-24 09:13:25.089278 entityshape-0.0.2/README.md
--rw-r--r--   0        0        0     2208 2023-06-24 12:40:28.882874 entityshape-0.0.2/entityshape/__init__.py
--rw-r--r--   0        0        0      538 2023-06-24 12:30:09.051783 entityshape-0.0.2/entityshape/enums.py
--rw-r--r--   0        0        0      167 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/__init__.py
--rw-r--r--   0        0        0      183 2023-06-24 12:27:51.347797 entityshape-0.0.2/entityshape/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14398 2023-06-24 12:27:51.351131 entityshape-0.0.2/entityshape/models/__pycache__/compareshape.cpython-311.pyc
--rw-r--r--   0        0        0     1724 2023-06-23 12:36:47.097067 entityshape-0.0.2/entityshape/models/__pycache__/conditions.cpython-311.pyc
--rw-r--r--   0        0        0      812 2023-06-24 12:27:51.451131 entityshape-0.0.2/entityshape/models/__pycache__/property_value.cpython-311.pyc
--rw-r--r--   0        0        0     2504 2023-06-23 12:36:00.409117 entityshape-0.0.2/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc
--rw-r--r--   0        0        0     9989 2023-06-24 12:46:17.549232 entityshape-0.0.2/entityshape/models/__pycache__/result.cpython-311.pyc
--rw-r--r--   0        0        0    17190 2023-06-24 12:27:51.461131 entityshape-0.0.2/entityshape/models/__pycache__/shape.cpython-311.pyc
--rw-r--r--   0        0        0     6532 2023-06-23 12:36:00.409117 entityshape-0.0.2/entityshape/models/__pycache__/shape_claim.cpython-311.pyc
--rw-r--r--   0        0        0      967 2023-06-24 12:43:06.050877 entityshape-0.0.2/entityshape/models/__pycache__/statement_value.cpython-311.pyc
--rw-r--r--   0        0        0    12458 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/compareshape.py
--rw-r--r--   0        0        0      245 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/property_value.py
--rw-r--r--   0        0        0     5981 2023-06-24 12:46:17.125895 entityshape-0.0.2/entityshape/models/result.py
--rw-r--r--   0        0        0    14070 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/shape.py
--rw-r--r--   0        0        0      377 2023-06-24 12:41:01.799816 entityshape-0.0.2/entityshape/models/statement_value.py
--rw-r--r--   0        0        0     3138 2023-06-24 12:54:46.053903 entityshape-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 entityshape-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 08:56:36.556587 entityshape-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3914 2023-06-25 14:47:24.433237 entityshape-0.1.0/README.md
+-rw-r--r--   0        0        0     2040 2023-06-25 15:16:53.263700 entityshape-0.1.0/entityshape/__init__.py
+-rw-r--r--   0        0        0      538 2023-06-24 12:30:09.051783 entityshape-0.1.0/entityshape/enums.py
+-rw-r--r--   0        0        0      167 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-24 12:27:51.347797 entityshape-0.1.0/entityshape/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14398 2023-06-24 12:27:51.351131 entityshape-0.1.0/entityshape/models/__pycache__/compareshape.cpython-311.pyc
+-rw-r--r--   0        0        0     1724 2023-06-23 12:36:47.097067 entityshape-0.1.0/entityshape/models/__pycache__/conditions.cpython-311.pyc
+-rw-r--r--   0        0        0      812 2023-06-24 12:27:51.451131 entityshape-0.1.0/entityshape/models/__pycache__/property_value.cpython-311.pyc
+-rw-r--r--   0        0        0     2504 2023-06-23 12:36:00.409117 entityshape-0.1.0/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc
+-rw-r--r--   0        0        0    11008 2023-06-25 14:39:11.690780 entityshape-0.1.0/entityshape/models/__pycache__/result.cpython-311.pyc
+-rw-r--r--   0        0        0    17190 2023-06-24 12:27:51.461131 entityshape-0.1.0/entityshape/models/__pycache__/shape.cpython-311.pyc
+-rw-r--r--   0        0        0     6532 2023-06-23 12:36:00.409117 entityshape-0.1.0/entityshape/models/__pycache__/shape_claim.cpython-311.pyc
+-rw-r--r--   0        0        0      967 2023-06-24 12:43:06.050877 entityshape-0.1.0/entityshape/models/__pycache__/statement_value.cpython-311.pyc
+-rw-r--r--   0        0        0    12458 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/compareshape.py
+-rw-r--r--   0        0        0      245 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/property_value.py
+-rw-r--r--   0        0        0     7004 2023-06-25 14:39:11.244107 entityshape-0.1.0/entityshape/models/result.py
+-rw-r--r--   0        0        0    14070 2023-06-23 15:26:04.636468 entityshape-0.1.0/entityshape/models/shape.py
+-rw-r--r--   0        0        0      377 2023-06-24 12:41:01.799816 entityshape-0.1.0/entityshape/models/statement_value.py
+-rw-r--r--   0        0        0     3138 2023-06-25 15:24:27.303751 entityshape-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 entityshape-0.1.0/PKG-INFO
```

### Comparing `entityshape-0.0.2/LICENSE` & `entityshape-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/__init__.py` & `entityshape-0.1.0/entityshape/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,44 +18,41 @@
     eid = ""  # entityshape
     lang = ""  # language
     result: Result = Result()
     eid_regex = re.compile(r"E\d+")
     qid_regex = re.compile(r"Q\d+")
     compare_shape_result: dict = {}
 
-    def __check__(self):
+    def __check_inputs__(self):
         if not self.lang:
             raise LangError("We only support 2 and 3 letter language codes")
         if not self.eid:
             raise EidError("We need an entityshape EID")
         if not re.match(self.eid_regex, self.eid):
             raise EidError("EID has to be E followed by only numbers like this: E100")
         if not self.qid:
             raise QidError("We need an item QID")
         if not re.match(self.qid_regex, self.qid):
             raise QidError("QID has to be Q followed by only numbers like this: Q100")
 
-    def get_result(self) -> Result:
+    def validate_and_get_result(self) -> Result:
         """This method checks if we got the 3 parameters we need and
         gets the results and return them"""
-        self.__check__()
+        self.__check_inputs__()
+        self.__validate__()
+        return self.__parse_result__()
+
+    def __validate__(self):
         shape: Shape = Shape(self.eid, self.lang)
         comparison: CompareShape = CompareShape(
             shape.get_schema_shape(), self.qid, self.lang
         )
         self.compare_shape_result: dict = {
             "general": comparison.get_general(),
             "properties": comparison.get_properties(),
             "statements": comparison.get_statements(),
         }
+
+    def __parse_result__(self) -> Result:
         self.result = Result(**self.compare_shape_result)
         self.result.analyze()
-        # print(self.result)
         return self.result
-
-    # def check_lang(self):
-    #     if not self.lang or 4 > len(self.lang) > 1:
-    #         raise LangError("We only support 2 and 3 letter language codes")
-    #
-    # def check_eid(self):
-    #     if not self.eid or :
-    #         raise LangError("We only support 2 and 3 letter language codes")
```

### Comparing `entityshape-0.0.2/entityshape/enums.py` & `entityshape-0.1.0/entityshape/enums.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/compareshape.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/compareshape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/conditions.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/conditions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/property_value.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/property_value.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/result.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/result.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x99e59664 (Sat Jun 24 12:46:17 2023 UTC)
-files sz: 5981
+moddate:  0x8f519864 (Sun Jun 25 14:39:11 2023 UTC)
+files sz: 7004
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
@@ -119,15 +119,16 @@
             000000650664113c000000651b64128400a6000000ab0000000000000000
             005a1c651b64138400a6000000ab0000000000000000005a1d651b641484
             00a6000000ab0000000000000000005a1e651b64158400a6000000ab0000
             000000000000005a1f651b64168400a6000000ab0000000000000000005a
             20651b64176515660264188404a6000000ab0000000000000000005a2165
             1b64198400a6000000ab0000000000000000005a22641a84005a23641b84
             005a24641c84005a25641d84005a26641e84005a27641f84005a28642084
-            005a29642184005a2a642284005a2b642384005a2c64245300
+            005a29642184005a2a642284005a2b642384005a2c642484005a2d642584
+            005a2e64265300
           13           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Result')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -406,16 +407,24 @@
          131         758 LOAD_CONST              34 (<code object __find_properties_that_are_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 131>)
                      760 MAKE_FUNCTION            0
                      762 STORE_NAME              43 (__find_properties_that_are_not_allowed__)
          
          137         764 LOAD_CONST              35 (<code object __find_statements_with_property_that_is_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 137>)
                      766 MAKE_FUNCTION            0
                      768 STORE_NAME              44 (__find_statements_with_property_that_is_not_allowed__)
-                     770 LOAD_CONST              36 (None)
-                     772 RETURN_VALUE
+         
+         143         770 LOAD_CONST              36 (<code object __str__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 143>)
+                     772 MAKE_FUNCTION            0
+                     774 STORE_NAME              45 (__str__)
+         
+         146         776 LOAD_CONST              37 (<code object __repr__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 146>)
+                     778 MAKE_FUNCTION            0
+                     780 STORE_NAME              46 (__repr__)
+                     782 LOAD_CONST              38 (None)
+                     784 RETURN_VALUE
          consts
             'Result'
             'general'
             ''
             'name'
             'properties'
             'statements'
@@ -1271,27 +1280,152 @@
                varnames   ('self', 'statement', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_statements_with_property_that_is_not_allowed__'
                firstlineno 137
                lnotab 0x020112011a012a0140fd
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c00a0000000000000000000000000000000000000000000a60000
+                  00ab000000000000000000010064005300
+               143           0 RESUME                   0
+               
+               144           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (__repr__)
+                            26 PRECALL                  0
+                            30 CALL                     0
+                            40 POP_TOP
+                            42 LOAD_CONST               0 (None)
+                            44 RETURN_VALUE
+               consts
+                  None
+               names      ('__repr__',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
+               name       '__str__'
+               firstlineno 143
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x970064017c006a0000000000000000009b009d027d017c006a00000000
+                  000000000072027c0153007c006a010000000000000000720d7c0164027c
+                  006a0200000000000000009b009d027a0d00007d017c006a030000000000
+                  000000720d7c0164037c006a0400000000000000009b009d027a0d00007d
+                  017c006a050000000000000000720d7c0164047c006a0500000000000000
+                  009b009d027a0d00007d017c006a060000000000000000720d7c0164057c
+                  006a0600000000000000009b009d027a0d00007d017c015300
+               146           0 RESUME                   0
+               
+               149           2 LOAD_CONST               1 ('Valid: ')
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (is_valid)
+                            16 FORMAT_VALUE             0
+                            18 BUILD_STRING             2
+                            20 STORE_FAST               1 (string)
+               
+               150          22 LOAD_FAST                0 (self)
+                            24 LOAD_ATTR                0 (is_valid)
+                            34 POP_JUMP_FORWARD_IF_FALSE     2 (to 40)
+               
+               151          36 LOAD_FAST                1 (string)
+                            38 RETURN_VALUE
+               
+               153     >>   40 LOAD_FAST                0 (self)
+                            42 LOAD_ATTR                1 (properties_with_too_many_statements_found)
+                            52 POP_JUMP_FORWARD_IF_FALSE    13 (to 80)
+               
+               154          54 LOAD_FAST                1 (string)
+                            56 LOAD_CONST               2 ('\nproperties_with_too_many_statements: ')
+                            58 LOAD_FAST                0 (self)
+                            60 LOAD_ATTR                2 (properties_with_too_many_statements)
+                            70 FORMAT_VALUE             0
+                            72 BUILD_STRING             2
+                            74 BINARY_OP               13 (+=)
+                            78 STORE_FAST               1 (string)
+               
+               155     >>   80 LOAD_FAST                0 (self)
+                            82 LOAD_ATTR                3 (properties_without_enough_correct_statements_found)
+                            92 POP_JUMP_FORWARD_IF_FALSE    13 (to 120)
+               
+               156          94 LOAD_FAST                1 (string)
+                            96 LOAD_CONST               3 ('\nproperties_without_enough_correct_statements: ')
+                            98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                4 (properties_without_enough_correct_statements)
+                           110 FORMAT_VALUE             0
+                           112 BUILD_STRING             2
+                           114 BINARY_OP               13 (+=)
+                           118 STORE_FAST               1 (string)
+               
+               157     >>  120 LOAD_FAST                0 (self)
+                           122 LOAD_ATTR                5 (required_properties_that_are_missing)
+                           132 POP_JUMP_FORWARD_IF_FALSE    13 (to 160)
+               
+               158         134 LOAD_FAST                1 (string)
+                           136 LOAD_CONST               4 ('\nrequired_properties_that_are_missing: ')
+                           138 LOAD_FAST                0 (self)
+                           140 LOAD_ATTR                5 (required_properties_that_are_missing)
+                           150 FORMAT_VALUE             0
+                           152 BUILD_STRING             2
+                           154 BINARY_OP               13 (+=)
+                           158 STORE_FAST               1 (string)
+               
+               159     >>  160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                6 (incorrect_statements)
+                           172 POP_JUMP_FORWARD_IF_FALSE    13 (to 200)
+               
+               160         174 LOAD_FAST                1 (string)
+                           176 LOAD_CONST               5 ('\nincorrect_statements: ')
+                           178 LOAD_FAST                0 (self)
+                           180 LOAD_ATTR                6 (incorrect_statements)
+                           190 FORMAT_VALUE             0
+                           192 BUILD_STRING             2
+                           194 BINARY_OP               13 (+=)
+                           198 STORE_FAST               1 (string)
+               
+               161     >>  200 LOAD_FAST                1 (string)
+                           202 RETURN_VALUE
+               consts
+                  'Return the result of the validation as a formatted string\n        with output exactly describing what caused the validation to fail'
+                  'Valid: '
+                  '\nproperties_with_too_many_statements: '
+                  '\nproperties_without_enough_correct_statements: '
+                  '\nrequired_properties_that_are_missing: '
+                  '\nincorrect_statements: '
+               names      ('is_valid', 'properties_with_too_many_statements_found', 'properties_with_too_many_statements', 'properties_without_enough_correct_statements_found', 'properties_without_enough_correct_statements', 'required_properties_that_are_missing', 'incorrect_statements')
+               varnames   ('self', 'string')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
+               name       '__repr__'
+               firstlineno 146
+               lnotab 0x020314010e0104020e011a010e011a010e011a010e011a01
             None
-         names      ('__name__', '__module__', '__qualname__', 'general', 'Dict', 'Any', '__annotations__', 'name', 'str', 'properties', 'PropertyValue', 'statements', 'StatementValue', 'set', 'missing_properties', 'Set', 'required_properties', 'incorrect_statements', 'missing_statements', 'properties_with_too_many_statements', 'analyzed', 'bool', 'required_properties_that_are_missing', 'optional_properties_that_are_missing', 'properties_without_enough_correct_statements', 'properties_that_are_not_allowed', 'statements_with_property_that_is_not_allowed', 'property', 'some_required_properties_are_missing', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found', 'is_valid', 'is_empty', 'analyze', '__find_properties_with_too_many_statements__', '__find_incorrect_statements__', '__find_required_properties__', '__find_missing_properties__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_with_not_enough_correct_statements__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__')
+         names      ('__name__', '__module__', '__qualname__', 'general', 'Dict', 'Any', '__annotations__', 'name', 'str', 'properties', 'PropertyValue', 'statements', 'StatementValue', 'set', 'missing_properties', 'Set', 'required_properties', 'incorrect_statements', 'missing_statements', 'properties_with_too_many_statements', 'analyzed', 'bool', 'required_properties_that_are_missing', 'optional_properties_that_are_missing', 'properties_without_enough_correct_statements', 'properties_that_are_not_allowed', 'statements_with_property_that_is_not_allowed', 'property', 'some_required_properties_are_missing', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found', 'is_valid', 'is_empty', 'analyze', '__find_properties_with_too_many_statements__', '__find_incorrect_statements__', '__find_required_properties__', '__find_missing_properties__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_with_not_enough_correct_statements__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__', '__str__', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
          name       'Result'
          firstlineno 13
          lnotab
             0x0c011e010e011e011e012a012a012a012a012a010e012a012a012a012a
             012a02020104ff0e010203020104ff0e010203020104ff0e010203020104
             ff0e010203020104ff0e01020302010aff0e01020e020104ff0e01020306
-            0d0606060c060606060607060606060606
+            0d0606060c06060606060706060606060606060603
       'Result'
    names      ('logging', 'typing', 'Any', 'Dict', 'Set', 'pydantic', 'BaseModel', 'ValidationError', 'entityshape.enums', 'Necessity', 'PropertyResponse', 'StatementResponse', 'entityshape.models.property_value', 'PropertyValue', 'entityshape.models.statement_value', 'StatementValue', 'getLogger', '__name__', 'logger', 'Result')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
    name       '<module>'
```

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/shape.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/shape.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/shape_claim.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/shape_claim.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/__pycache__/statement_value.cpython-311.pyc` & `entityshape-0.1.0/entityshape/models/__pycache__/statement_value.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/compareshape.py` & `entityshape-0.1.0/entityshape/models/compareshape.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/entityshape/models/result.py` & `entityshape-0.1.0/entityshape/models/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -135,7 +135,27 @@
                 self.properties_that_are_not_allowed.add(property_)
 
     def __find_statements_with_property_that_is_not_allowed__(self):
         for statement in self.statements:
             value: StatementValue = self.statements[statement]
             if value.necessity == Necessity.ABSENT:
                 self.statements_with_property_that_is_not_allowed.add(value.property)
+
+    def __str__(self):
+        self.__repr__()
+
+    def __repr__(self):
+        """Return the result of the validation as a formatted string
+        with output exactly describing what caused the validation to fail"""
+        string = f"Valid: {self.is_valid}"
+        if self.is_valid:
+            return string
+        else:
+            if self.properties_with_too_many_statements_found:
+                string += f"\nproperties_with_too_many_statements: {self.properties_with_too_many_statements}"
+            if self.properties_without_enough_correct_statements_found:
+                string += f"\nproperties_without_enough_correct_statements: {self.properties_without_enough_correct_statements}"
+            if self.required_properties_that_are_missing:
+                string += f"\nrequired_properties_that_are_missing: {self.required_properties_that_are_missing}"
+            if self.incorrect_statements:
+                string += f"\nincorrect_statements: {self.incorrect_statements}"
+            return string
```

### Comparing `entityshape-0.0.2/entityshape/models/shape.py` & `entityshape-0.1.0/entityshape/models/shape.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.2/pyproject.toml` & `entityshape-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Entityshape"
-version = "0.0.2"
+version = "0.1.0"
 description = "Python library to validate Wikidata items."
 authors = ["Mark Tully aka Teester", "Dennis Priskorn <68460690+dpriskorn@users.noreply.github.com>"]
 license = "GPLv3+"
 readme = "README.md"
 repository = "https://github.com/dpriskorn/entityshape"
 keywords = ["wikidata", "entityschema", "entity validation"]
 classifiers = [
```

### Comparing `entityshape-0.0.2/PKG-INFO` & `entityshape-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,8 @@
-Metadata-Version: 2.1
-Name: entityshape
-Version: 0.0.2
-Summary: Python library to validate Wikidata items.
-Home-page: https://github.com/dpriskorn/entityshape
-License: GPLv3+
-Keywords: wikidata,entityschema,entity validation
-Author: Mark Tully aka Teester
-Requires-Python: >=3.8,<=3.12
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Project-URL: Repository, https://github.com/dpriskorn/entityshape
-Description-Content-Type: text/markdown
-
-# Entityshape
+# [Entityshape](https://www.wikidata.org/wiki/Q119899931)
 A python library to compare a wikidata item with an entityschema
 
 Based on https://github.com/Teester/entityshape by Mark Tully 
 and https://github.com/dpriskorn/PyEntityshape by Dennis Priskorn
 
 # Features
 * compare a given wikidata item with an entityschema and dig into missing properties, too many statement, etc.
@@ -39,34 +18,51 @@
 
 # Installation
 Get it from pypi
 
 `$ pip install pyentityshape`
 
 # Usage
+
+## Jupyter Notebooks
+Example notebooks with code for validation of multiple items: 
+[hiking paths](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-hiking-paths-in-sweden.ipynb) 
+[campsites](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-campsites-in-sweden.ipynb) 
+[shelters](https://public-paws.wmcloud.org/User:So9q/Validating%20a%20group%20of%20items-all-shelters-in-sweden.ipynb)
+
+## CLI
 Example:
 ```
 e = EntityShape(eid="E1", lang="en", qid="Q1")
 result = e.get_result()
-result.is_valid
-False|True
-result.required_properties_that_are_missing
-{"P1", "P2"}
+# Get human readable result
+print(result)
+"Valid: False\nproperties_without_enough_correct_statements: {'P31'}"
+# Access the data
+print(result.properties_without_enough_correct_statements)
+"{'P31'}"
 ```
 
 ## Validation
 The is_valid method on the Result object mimics all red warnings displayed by https://www.wikidata.org/wiki/User:Teester/EntityShape.js 
 
 It currently checks these five conditions that all have to be false for the item to be valid:
 1.  properties with too many statements found
 2.   incorrect statements found
 3.   some required properties are missing
 4.   properties without enough correct statements found
 5.   statements with properties that are not allowed found
 
+## Known working schemas
+This library currently only supports a subset of all features in the ShEx specifikation.
+
+The following Entity Schemas are known to work:
+* [hiking path](https://www.wikidata.org/w/index.php?title=EntitySchema:E375&oldid=1833851062)
+* [shelter](https://www.wikidata.org/w/index.php?title=EntitySchema:E398&oldid=1923235264)
+
 # Background
 This library is the glue between libraries like [Wikibase 
 Integrator](https://github.com/LeMyst/WikibaseIntegrator/) and entityschemas. 
 
 It makes it easy to batch check a whole subset of Wikidata 
 items against a schema. Nice!
 
@@ -103,9 +99,10 @@
 advice and help with Ruff to make this better. 
 
 # License
 GPLv3+
 
 # What I learned
 * Forking other peoples undocumented spaghetti code is not much fun.
+* I want to find a more reliable validator that support somevalue and novalue
 * Pydantic is wonderful yet again it makes working with OOP easy peasy :)
-* Ruff is crazy fast and very nice!
+* Ruff is crazy fast and very nice!
```

