# Comparing `tmp/openai_functions-0.5.5.tar.gz` & `tmp/openai_functions-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.5.5.tar", max compression
+gzip compressed data, was "openai_functions-0.6.0.tar", max compression
```

## Comparing `openai_functions-0.5.5.tar` & `openai_functions-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2859 2023-06-24 01:53:23.475835 openai_functions-0.5.5/README.md
--rw-r--r--   0        0        0      561 2023-06-24 01:49:09.012365 openai_functions-0.5.5/openai_functions/__init__.py
--rw-r--r--   0        0        0    10102 2023-06-24 02:01:13.116505 openai_functions-0.5.5/openai_functions/conversation.py
--rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.5.5/openai_functions/functions/__init__.py
--rw-r--r--   0        0        0     2936 2023-06-23 23:39:48.076531 openai_functions-0.5.5/openai_functions/functions/basic_set.py
--rw-r--r--   0        0        0      356 2023-06-24 01:56:28.673664 openai_functions-0.5.5/openai_functions/functions/exceptions.py
--rw-r--r--   0        0        0     2478 2023-06-24 01:57:02.009995 openai_functions-0.5.5/openai_functions/functions/functions.py
--rw-r--r--   0        0        0     4210 2023-06-24 01:50:27.961125 openai_functions-0.5.5/openai_functions/functions/sets.py
--rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.5.5/openai_functions/functions/union.py
--rw-r--r--   0        0        0     6327 2023-06-24 01:44:38.621801 openai_functions-0.5.5/openai_functions/functions/wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.5.5/openai_functions/json_type.py
--rw-r--r--   0        0        0     2794 2023-06-24 01:48:05.913763 openai_functions-0.5.5/openai_functions/nlp.py
--rw-r--r--   0        0        0     6605 2023-06-24 01:58:06.858641 openai_functions-0.5.5/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.5.5/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.5.5/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      975 2023-06-24 00:28:00.470995 openai_functions-0.5.5/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.5.5/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-24 00:45:19.947754 openai_functions-0.5.5/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.5.5/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.5.5/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.5.5/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      520 2023-06-24 01:52:09.574112 openai_functions-0.5.5/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.5.5/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.5.5/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.5.5/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.5.5/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.5.5/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.5.5/openai_functions/py.typed
--rw-r--r--   0        0        0      607 2023-06-24 02:05:04.256832 openai_functions-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     3511 1970-01-01 00:00:00.000000 openai_functions-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     3142 2023-06-25 06:47:00.797450 openai_functions-0.6.0/README.md
+-rw-r--r--   0        0        0      561 2023-06-24 01:49:09.012365 openai_functions-0.6.0/openai_functions/__init__.py
+-rw-r--r--   0        0        0    10879 2023-06-25 06:45:03.861226 openai_functions-0.6.0/openai_functions/conversation.py
+-rw-r--r--   0        0        0      371 2023-06-23 23:16:40.645247 openai_functions-0.6.0/openai_functions/functions/__init__.py
+-rw-r--r--   0        0        0     2936 2023-06-23 23:39:48.076531 openai_functions-0.6.0/openai_functions/functions/basic_set.py
+-rw-r--r--   0        0        0      356 2023-06-24 01:56:28.673664 openai_functions-0.6.0/openai_functions/functions/exceptions.py
+-rw-r--r--   0        0        0     2478 2023-06-24 01:57:02.009995 openai_functions-0.6.0/openai_functions/functions/functions.py
+-rw-r--r--   0        0        0     4210 2023-06-24 01:50:27.961125 openai_functions-0.6.0/openai_functions/functions/sets.py
+-rw-r--r--   0        0        0     1678 2023-06-23 23:33:22.081874 openai_functions-0.6.0/openai_functions/functions/union.py
+-rw-r--r--   0        0        0     6327 2023-06-24 01:44:38.621801 openai_functions-0.6.0/openai_functions/functions/wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.6.0/openai_functions/json_type.py
+-rw-r--r--   0        0        0     5298 2023-06-25 06:49:11.631909 openai_functions-0.6.0/openai_functions/nlp.py
+-rw-r--r--   0        0        0     7508 2023-06-25 06:45:07.662263 openai_functions-0.6.0/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.6.0/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.6.0/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      975 2023-06-24 00:28:00.470995 openai_functions-0.6.0/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.6.0/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-24 00:45:19.947754 openai_functions-0.6.0/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.6.0/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.6.0/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.6.0/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      520 2023-06-24 01:52:09.574112 openai_functions-0.6.0/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.6.0/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.6.0/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.6.0/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.6.0/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.6.0/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.6.0/openai_functions/py.typed
+-rw-r--r--   0        0        0      607 2023-06-24 10:16:51.204572 openai_functions-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 openai_functions-0.6.0/PKG-INFO
```

### Comparing `openai_functions-0.5.5/README.md` & `openai_functions-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -83,17 +83,19 @@
     name: str
     age: int
 ```
 
 4. Ask the AI for a summary of the data:
 
 ```python
-Person.nlp("I'm Jack and I'm 20 years old.", "Person")
+person = Person.from_natural_language("I'm Jack and I'm 20 years old.")
 ```
 
+Note: mypy does not parse class decorators ([#3135](https://github.com/python/mypy/issues/3135)), so you might have trouble getting type checking when using it like this. Consider using something like `nlp(Person).from_natural_language` to get proper type support.
+
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
 - Parsing the function signatures and docstrings.
 - Sending the conversation and function descriptions to the OpenAI model.
 - Deciding whether to call a function based on the model's response.
```

### Comparing `openai_functions-0.5.5/openai_functions/__init__.py` & `openai_functions-0.6.0/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/conversation.py` & `openai_functions-0.6.0/openai_functions/conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """A module for running OpenAI functions"""
 from __future__ import annotations
-from typing import Any, Callable, TYPE_CHECKING, overload
+from typing import Any, Callable, Literal, TYPE_CHECKING, overload
 
 import openai
 
 from .functions.union import UnionSkillSet
 from .openai_types import (
     FinalResponseMessage,
+    FinalResponseMessageType,
+    ForcedFunctionCall,
+    FunctionCallMessage,
     FunctionMessageType,
     GenericMessage,
     IntermediateResponseMessageType,
     Message,
     is_final_response_message,
 )
 
@@ -87,14 +90,32 @@
         """
         return self.messages.pop(index)
 
     def clear_messages(self) -> None:
         """Clear the messages"""
         self.messages = []
 
+    @overload
+    def _generate_message(
+        self, function_call: ForcedFunctionCall
+    ) -> IntermediateResponseMessageType:
+        ...
+
+    @overload
+    def _generate_message(
+        self, function_call: Literal["none"]
+    ) -> FinalResponseMessageType:
+        ...
+
+    @overload
+    def _generate_message(
+        self, function_call: Literal["auto"] = "auto"
+    ) -> NonFunctionMessageType:
+        ...
+
     def _generate_message(
         self, function_call: OpenAiFunctionCallInput = "auto"
     ) -> NonFunctionMessageType:
         """Generate a response
 
         Args:
             function_call (OpenAiFunctionCallInput): The function call.
@@ -206,29 +227,36 @@
 
         Args:
             function_call (OpenAiFunctionCallInput): The function call
 
         Returns:
             GenericMessage: The response
         """
-        if self.run_function_if_needed():
+        if function_call in ["auto", "none"] and self.run_function_if_needed():
             return self.messages[-1]
 
-        message = self._generate_message(function_call)
+        message: NonFunctionMessageType = self._generate_message(function_call)
         self.add_message(message)
         return Message(message)
 
-    def run_until_response(self) -> FinalResponseMessage:
+    def run_until_response(
+        self, allow_function_calls: bool = True
+    ) -> FinalResponseMessage:
         """Run until a response is generated
 
+        Args:
+            allow_function_calls (bool): Whether to allow function calls.
+
         Returns:
             FinalResponseMessage: The response
         """
         while True:
-            message = self.generate_message()
+            message = self.generate_message(
+                function_call="auto" if allow_function_calls else "none"
+            )
             if is_final_response_message(message):
                 return message
 
     @overload
     def add_function(self, function: OpenAIFunction) -> OpenAIFunction:
         ...
 
@@ -331,10 +359,10 @@
             function (str): The function to run
 
         Returns:
             The raw function result
         """
         self.add_message(prompt)
         # We can do type: ignore as we know we're forcing a function call
-        response: IntermediateResponseMessageType
-        response = self._generate_message({"name": function})  # type: ignore
-        return self.skills(response["function_call"])
+        response: FunctionCallMessage
+        response = self.generate_message({"name": function})  # type: ignore
+        return self.skills(response.function_call)
```

### Comparing `openai_functions-0.5.5/openai_functions/functions/basic_set.py` & `openai_functions-0.6.0/openai_functions/functions/basic_set.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/functions/functions.py` & `openai_functions-0.6.0/openai_functions/functions/functions.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/functions/sets.py` & `openai_functions-0.6.0/openai_functions/functions/sets.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/functions/union.py` & `openai_functions-0.6.0/openai_functions/functions/union.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/functions/wrapper.py` & `openai_functions-0.6.0/openai_functions/functions/wrapper.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/openai_types.py` & `openai_functions-0.6.0/openai_functions/openai_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,27 @@
 class FinalResponseMessageType(TypedDict):
     """A type for OpenAI messages that are final responses"""
 
     role: Literal["assistant"]
     content: str
 
 
-class ContentfulMessageType(TypedDict):
-    """A type for OpenAI messages that are contentful"""
+class UserMessageType(TypedDict):
+    """A type for OpenAI messages that are user messages"""
 
-    role: Literal["system", "user", "assistant"]
+    role: Literal[
+        "system",
+        "user",
+    ]
     content: str
 
 
+ContentfulMessageType = Union[FinalResponseMessageType, UserMessageType]
+
+
 class IntermediateResponseMessageType(TypedDict):
     """A type for OpenAI messages that are intermediate responses"""
 
     role: Literal["assistant"]
     content: None
     function_call: FunctionCall
 
@@ -75,17 +81,24 @@
         ...
 
     def __init__(
         self,
         message: MessageType | str,
         role: Literal["system", "user", "assistant"] = "user",
     ):
-        self.message: MessageType = (
-            {"role": role, "content": message} if isinstance(message, str) else message
-        )
+        if isinstance(message, str):
+            if role == "assistant":  # We have to split this up because of mypy
+                self.message: MessageType = {"role": role, "content": message}
+            else:
+                self.message = {
+                    "role": role,
+                    "content": message,
+                }
+        else:
+            self.message = message
 
     @property
     def content(self) -> str | None:
         """Get the content of the message
 
         Returns:
             str | None: The content of the message
@@ -232,14 +245,34 @@
 
     @property
     def is_final_response(self) -> Literal[True]:
         """Check if the message is a final response"""
         ...  # pylint: disable=unnecessary-ellipsis
 
 
+class FunctionCallMessage(GenericMessage, Protocol):
+    """A container for OpenAI function call messages"""
+
+    message: IntermediateResponseMessageType
+
+    @property
+    def content(self) -> None:
+        """Get the content of the message"""
+
+    @property
+    def function_call(self) -> FunctionCall:
+        """Get the function call"""
+        ...  # pylint: disable=unnecessary-ellipsis
+
+    @property
+    def is_final_response(self) -> Literal[False]:
+        """Check if the message is a final response"""
+        ...  # pylint: disable=unnecessary-ellipsis
+
+
 def is_final_response_message(
     message: GenericMessage,
 ) -> TypeGuard[FinalResponseMessage]:
     """Check if a message is a final response message
 
     Args:
         message (GenericMessage): The message to check
```

### Comparing `openai_functions-0.5.5/openai_functions/parsers/abc.py` & `openai_functions-0.6.0/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/default.py` & `openai_functions-0.6.0/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/dict_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/enum_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/float_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/int_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/list_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/none_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/openai_functions/parsers/union_parser.py` & `openai_functions-0.6.0/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.5.5/pyproject.toml` & `openai_functions-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.5.5"
+version = "0.6.0"
 description = "Simplifies the usage of OpenAI's function calling."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.5.5/PKG-INFO` & `openai_functions-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.5.5
+Version: 0.6.0
 Summary: Simplifies the usage of OpenAI's function calling.
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -100,17 +100,19 @@
     name: str
     age: int
 ```
 
 4. Ask the AI for a summary of the data:
 
 ```python
-Person.nlp("I'm Jack and I'm 20 years old.", "Person")
+person = Person.from_natural_language("I'm Jack and I'm 20 years old.")
 ```
 
+Note: mypy does not parse class decorators ([#3135](https://github.com/python/mypy/issues/3135)), so you might have trouble getting type checking when using it like this. Consider using something like `nlp(Person).from_natural_language` to get proper type support.
+
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
 - Parsing the function signatures and docstrings.
 - Sending the conversation and function descriptions to the OpenAI model.
 - Deciding whether to call a function based on the model's response.
```

