# Comparing `tmp/chatlab-0.13.0.tar.gz` & `tmp/chatlab-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatlab-0.13.0.tar", max compression
+gzip compressed data, was "chatlab-0.14.0.tar", max compression
```

## Comparing `chatlab-0.13.0.tar` & `chatlab-0.14.0.tar`

### file list

```diff
@@ -1,14 +1,20 @@
--rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 chatlab-0.13.0/LICENSE
--rw-r--r--   0        0        0     6088 2023-06-23 01:47:53.279655 chatlab-0.13.0/README.md
--rw-r--r--   0        0        0     1709 2023-06-23 01:40:58.550859 chatlab-0.13.0/chatlab/__init__.py
--rw-r--r--   0        0        0       23 2023-06-22 08:09:24.541342 chatlab-0.13.0/chatlab/_version.py
--rw-r--r--   0        0        0      742 2023-06-23 01:41:20.797366 chatlab-0.13.0/chatlab/builtins.py
--rw-r--r--   0        0        0     9354 2023-06-23 01:41:19.278550 chatlab-0.13.0/chatlab/conversation.py
--rw-r--r--   0        0        0     7003 2023-06-23 01:41:18.313333 chatlab-0.13.0/chatlab/display.py
--rw-r--r--   0        0        0     3346 2023-06-23 01:40:58.517572 chatlab-0.13.0/chatlab/markdown.py
--rw-r--r--   0        0        0     2136 2023-06-23 01:41:19.913395 chatlab-0.13.0/chatlab/messaging.py
--rw-r--r--   0        0        0     6846 2023-06-23 01:40:58.820467 chatlab-0.13.0/chatlab/registry.py
--rw-r--r--   0        0        0     1998 2023-06-23 01:40:57.757512 chatlab-0.13.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-23 01:40:58.825821 chatlab-0.13.0/tests/__init__.py
--rw-r--r--   0        0        0      624 2023-06-23 01:40:58.859307 chatlab-0.13.0/tests/test_murkrow.py
--rw-r--r--   0        0        0     7088 1970-01-01 00:00:00.000000 chatlab-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-06 23:40:21.685931 chatlab-0.14.0/LICENSE
+-rw-r--r--   0        0        0     7121 2023-06-24 20:10:32.954739 chatlab-0.14.0/README.md
+-rw-r--r--   0        0        0     1863 2023-06-25 17:54:33.824854 chatlab-0.14.0/chatlab/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-25 17:58:11.386691 chatlab-0.14.0/chatlab/_version.py
+-rw-r--r--   0        0        0      897 2023-06-24 22:32:44.193741 chatlab-0.14.0/chatlab/builtins.py
+-rw-r--r--   0        0        0     9684 2023-06-25 05:54:27.338669 chatlab-0.14.0/chatlab/conversation.py
+-rw-r--r--   0        0        0     2382 2023-06-25 17:43:22.956069 chatlab-0.14.0/chatlab/decorators.py
+-rw-r--r--   0        0        0     7698 2023-06-25 17:43:22.956463 chatlab-0.14.0/chatlab/display.py
+-rw-r--r--   0        0        0      114 2023-06-25 04:13:12.062499 chatlab-0.14.0/chatlab/errors.py
+-rw-r--r--   0        0        0     3304 2023-06-25 02:50:41.266379 chatlab-0.14.0/chatlab/markdown.py
+-rw-r--r--   0        0        0     3290 2023-06-24 22:32:44.194023 chatlab-0.14.0/chatlab/messaging.py
+-rw-r--r--   0        0        0     1869 2023-06-25 04:54:08.204496 chatlab-0.14.0/chatlab/models.py
+-rw-r--r--   0        0        0     7212 2023-06-25 17:43:22.956810 chatlab-0.14.0/chatlab/registry.py
+-rw-r--r--   0        0        0     2023 2023-06-25 17:58:11.386497 chatlab-0.14.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-23 17:12:00.817039 chatlab-0.14.0/tests/__init__.py
+-rw-r--r--   0        0        0      357 2023-06-25 17:54:33.826902 chatlab-0.14.0/tests/test_chatlab.py
+-rw-r--r--   0        0        0     1103 2023-06-25 17:43:22.957117 chatlab-0.14.0/tests/test_decorators.py
+-rw-r--r--   0        0        0     1066 2023-06-24 22:32:44.195986 chatlab-0.14.0/tests/test_messaging.py
+-rw-r--r--   0        0        0     6792 2023-06-25 02:49:49.084533 chatlab-0.14.0/tests/test_registry.py
+-rw-r--r--   0        0        0     8121 1970-01-01 00:00:00.000000 chatlab-0.14.0/PKG-INFO
```

### Comparing `chatlab-0.13.0/LICENSE` & `chatlab-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatlab-0.13.0/README.md` & `chatlab-0.14.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,71 @@
 # ChatLab
 
 **Chat Experiments, Simplified**
 
 💬🔬
 
-Chatlab is where chat conversations take shape. It’s your laboratory for experimenting with and crafting intelligent conversations using OpenAI’s chat models.
+ChatLab is a Python package that makes it easy to experiment with OpenAI's chat models. It provides a simple interface for chatting with the models and a way to register functions that can be called from the chat model.
 
-## Introduction
+Best yet, it's interactive in the notebook!
 
-Welcome to Chatlab, your personal workshop for chat innovation. Are you intrigued by conversational AI? Chatlab empowers developers to mold conversations according to their vision. Whether you are an AI enthusiast, researcher, or developer, Chatlab provides you with the building blocks and tools necessary for crafting intelligent conversations seamlessly. 🧪💬
+## Introduction
 
 ```python
 import chatlab
+import random
+
+def flip_a_coin():
+    '''Returns heads or tails'''
+    return random.choice(['heads', 'tails'])
 
 conversation = chatlab.Conversation()
+conversation.register(flip_a_coin)
 
-conversation.submit("How much wood could a")
+conversation.submit("Please flip a coin for me")
 ```
 
-```markdown
-woodchuck chuck if a woodchuck could chuck wood?
+<details style="background:#DDE6ED;color:#27374D;padding:.5rem 1rem;borderRadius:5px">
+<summary>&nbsp;𝑓&nbsp; Ran `flip_a_coin`
+</summary>
+<br />
+
+Input:
+
+```json
+{}
+```
+
+Output:
+
+```json
+"tails"
 ```
 
-In the notebook, text will stream into a Markdown output.
+</details>
+
+```markdown
+It landed on tails!
+```
 
-![image](https://github.com/rgbkrk/chatlab/assets/836375/81b2837c-430c-42eb-ae60-0c3a91ae26b6)
+In the notebook, text will stream into a Markdown output and function inputs and outputs are a nice collapsible display, like with ChatGPT Plugins.
 
-When using chat functions in the notebook\*, you'll get a nice collapsible display of inputs and outputs.
+<details class="details-reset border rounded-2" open="">
+  <summary class="px-3 py-2">
+    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-device-camera-video">
+    <path d="M16 3.75v8.5a.75.75 0 0 1-1.136.643L11 10.575v.675A1.75 1.75 0 0 1 9.25 13h-7.5A1.75 1.75 0 0 1 0 11.25v-6.5C0 3.784.784 3 1.75 3h7.5c.966 0 1.75.784 1.75 1.75v.675l3.864-2.318A.75.75 0 0 1 16 3.75Zm-6.5 1a.25.25 0 0 0-.25-.25h-7.5a.25.25 0 0 0-.25.25v6.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-6.5ZM11 8.825l3.5 2.1v-5.85l-3.5 2.1Z"></path>
+</svg>
+    <span aria-label="Video description flip-a-coin-chatlab.mp4" class="m-1">flip-a-coin-chatlab.mp4</span>
+    <span class="dropdown-caret"></span>
+  </summary>
 
-![click](https://github.com/rgbkrk/chatlab/assets/836375/21c6bd4c-cd3b-48b9-812a-2b86a05c20da)
+  <video src="https://user-images.githubusercontent.com/836375/248335062-fdc523b1-ca31-4506-b3ed-c73be9eb0d88.mp4" data-canonical-src="https://user-images.githubusercontent.com/836375/248335062-fdc523b1-ca31-4506-b3ed-c73be9eb0d88.mp4" controls="controls" muted="muted" class="d-block rounded-bottom-2 border-top width-fit" style="max-height:640px; min-height: 200px">
 
-\* Tested in JupyterLab and Noteable
+  </video>
+</details>
 
 ### Installation
 
 ```bash
 pip install chatlab
 ```
 
@@ -42,20 +73,19 @@
 
 You'll need to set your `OPENAI_API_KEY` environment variable. You can find your API key on your [OpenAI account page](https://platform.openai.com/account/api-keys). I recommend setting it in an `.env` file when working locally.
 
 On hosted environments like Noteable, set it in your Secrets to keep it safe from prying LLM eyes.
 
 ## What can `Conversation`s enable _you_ to do?
 
-<center><img src="https://cdn.donmai.us/original/64/e7/64e78d7968c8317b84a95e152e4a087b.png" height="100" /></center>
-<br />
+💬
 
 Where `Conversation`s take it next level is with _Chat Functions_. You can
 
--   declare a function with a schema
+-   declare a function
 -   register the function in your `Conversation`
 -   watch as Chat Models call your functions!
 
 You may recall this kind of behavior from [ChatGPT Plugins](https://noteable.io/chatgpt-plugin-for-notebook/). Now, you can take this even further with your own custom code.
 
 As an example, let's give the large language models the ability to tell time.
 
@@ -92,24 +122,41 @@
 # Register our function
 conversation.register(what_time, WhatTime)
 
 # Pluck the submit off for easy access as chat
 chat = conversation.submit
 ```
 
-After that, we can call `chat` with direct strings (which are turned into user messages) or using simple message makers from `chatlab` named `human`/`user` and `narrate`/`system`.
+After that, we can call `chat` with direct strings (which are turned into user messages) or using simple message makers from `chatlab` named `user` and `system`.
 
 ```python
 chat("What time is it?")
 ```
 
-```markdown
-▶ 𝑓 Ran `what_time`
+<details style="background:#DDE6ED;color:#27374D;padding:.5rem 1rem;borderRadius:5px">
+<summary>&nbsp;𝑓&nbsp; Ran `what_time`
+</summary>
+<br />
+
+Input:
+
+```json
+{}
+```
+
+Output:
+
+```json
+"11:19 AM"
+```
+
+</details>
 
-The current time is 11:47 PM.
+```markdown
+The current time is 11:19 AM.
 ```
 
 ## Interface
 
 The `chatlab` package exports
 
 ### `Conversation`
@@ -117,15 +164,15 @@
 The `Conversation` class is the main way to chat using OpenAI's models. It keeps a history of your chat in `Conversation.messages`.
 
 #### `Conversation.submit`
 
 When you call `submit`, you're sending over messages to the chat model and getting back an updating `Markdown` display live as well as a interactive details area for any function calls.
 
 ```python
-conversation.submit("What would a parent who says "I have to play zone defense" mean? ")
+conversation.submit('What would a parent who says "I have to play zone defense" mean? ')
 # Markdown response inline
 conversation.messages
 ```
 
 ```js
 [{'role': 'user',
   'content': 'What does a parent of three kids mean by "I have to play zone defense"?'},
```

### Comparing `chatlab-0.13.0/chatlab/__init__.py` & `chatlab-0.14.0/chatlab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 """
 
 __author__ = """Kyle Kelley"""
 __email__ = 'rgbkrk@gmail.com'
 
 from deprecation import deprecated
 
+from . import models
 from ._version import __version__
 from .conversation import Conversation
+from .decorators import ChatlabMetadata, expose_exception_to_llm
 from .display import Markdown
 from .messaging import ai, assistant, assistant_function_call, function_result, human, narrate, system, user
 from .registry import FunctionRegistry
 
 
 # Deprecate Session in favor of Conversation
 class Session(Conversation):
@@ -47,11 +49,14 @@
     "ai",
     "narrate",
     "system",
     "user",
     "assistant",
     "assistant_function_call",
     "function_result",
+    "models",
     "Session",
     "Conversation",
     "FunctionRegistry",
+    "ChatlabMetadata",
+    "expose_exception_to_llm",
 ]
```

### Comparing `chatlab-0.13.0/chatlab/conversation.py` & `chatlab-0.14.0/chatlab/conversation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """The lightweight conversational toolkit for computational notebooks."""
 
-import json
 import logging
-from typing import Callable, List, Optional, Union
+import os
+from typing import Callable, List, Optional, Type, Union
 
 import openai
-from chatlab.registry import FunctionRegistry
 from deprecation import deprecated
 from pydantic import BaseModel
 
 from ._version import __version__
 from .display import ChatFunctionCall, Markdown
+from .errors import ChatLabError
 from .messaging import Message, assistant, assistant_function_call, human
+from .registry import FunctionRegistry
 
 logger = logging.getLogger(__name__)
 
 
 class Conversation:
     """Interactive chats inside of computational notebooks, relying on OpenAI's API.
 
@@ -26,88 +27,97 @@
     Args:
         initial_context (str | Message): The initial context for the conversation.
 
         model (str): The model to use for the conversation.
 
         function_registry (FunctionRegistry): The function registry to use for the conversation.
 
-        auto_continue (bool): Whether to automatically continue the conversation after each message.
-
         allow_hallucinated_python (bool): Whether to include the built-in Python function when hallucinated by the model.
 
     Examples:
         >>> from chatlab import Conversation, narrate
 
         >>> conversation = Conversation(narrate("You are a large bird"))
         >>> conversation.submit("What are you?")
         I am a large bird.
 
     """
 
     messages: List[Message]
     model: str
     function_registry: FunctionRegistry
-    auto_continue: bool
     allow_hallucinated_python: bool
 
     def __init__(
         self,
         *initial_context: Union[Message, str],
         model="gpt-3.5-turbo-0613",
         function_registry: Optional[FunctionRegistry] = None,
-        auto_continue: bool = True,
         allow_hallucinated_python: bool = False,
     ):
         """Initialize a Conversation with an optional initial context of messages.
 
         >>> from chatlab import Conversation, narrate
         >>> convo = Conversation(narrate("You are a large bird"))
         >>> convo.submit("What are you?")
         I am a large bird.
 
         """
+        openai_api_key = os.getenv('OPENAI_API_KEY')
+        if openai_api_key is None:
+            raise ChatLabError(
+                "You must set the environment variable `OPENAI_API_KEY` to use this package.\n"
+                "This key allows chatlab to communicate with OpenAI servers.\n\n"
+                "You can generate API keys in the OpenAI web interface. "
+                "See https://platform.openai.com/account/api-keys for details.\n\n"
+                # TODO: An actual docs page
+                "If you have any questions, tweet at us at https://twitter.com/chatlablib."
+            )
+        else:
+            pass
+
         if initial_context is None:
             initial_context = []  # type: ignore
 
         self.messages: List[Message] = []
 
         self.append(*initial_context)
         self.model = model
-        self.auto_continue = auto_continue
 
         self.allow_hallucinated_python = allow_hallucinated_python
 
         if function_registry is None:
             self.function_registry = FunctionRegistry(allow_hallucinated_python=self.allow_hallucinated_python)
         else:
             self.function_registry = function_registry
 
     @deprecated(
         deprecated_in="0.13.0", removed_in="1.0.0", current_version=__version__, details="Use `submit` instead."
     )
-    def chat(self, *messages: Union[Message, str], auto_continue: Optional[bool] = None):
+    def chat(
+        self,
+        *messages: Union[Message, str],
+    ):
         """Send messages to the chat model and display the response.
 
         Deprecated in 0.13.0, removed in 1.0.0. Use `submit` instead.
         """
-        return self.submit(*messages, auto_continue=auto_continue)
+        return self.submit(*messages)
 
-    def submit(self, *messages: Union[Message, str], auto_continue: Optional[bool] = None):
+    def submit(self, *messages: Union[Message, str]):
         """Send messages to the chat model and display the response.
 
         Side effects:
             - Messages are sent to OpenAI Chat Models.
             - The response(s) are displayed in the output area. Markdown for assistant messages, collapsible display for function calls.
             - conversation.messages is updated with response(s).
 
         Args:
             messages (str | Message): One or more messages to send to the chat, can be strings or Message objects.
 
-            auto_continue (bool): Whether to continue the conversation after the messages are sent. Defaults to the
-
         """
         self.append(*messages)
 
         # Get the output area ready
         mark = Markdown()
         mark.display()
 
@@ -126,18 +136,22 @@
             stream=True,
         )
 
         chat_function = None
         finish_reason = None
 
         for result in resp:  # Go through the results of the stream
+            if not isinstance(result, dict):
+                logger.warning(f"Unknown result type: {type(result)}: {result}")
+                continue
+
             choices: list = result.get('choices', [])
 
             if len(choices) == 0:
-                logger.warning(f"Unexpected result: {result}")
+                logger.warning(f"Result has no choices: {result}")
                 continue
 
             choice = choices[0]
 
             if 'delta' in choice:  # If there is a delta in the result
                 delta = choice['delta']
                 if 'content' in delta and delta['content'] is not None:  # If the delta contains content
@@ -179,26 +193,23 @@
                 assistant_function_call(name=chat_function.function_name, arguments=chat_function.function_args)
             )
             # Make the call
             fn_message = chat_function.call()
             # Include the response (or error) for the model
             self.append(fn_message)
 
-            # Choose whether to let the LLM continue from our function response
-            continuing = auto_continue if auto_continue is not None else self.auto_continue
-
-            if continuing:
-                # Automatically let the LLM continue from our function result
-                self.submit()
+            # Reply back to the LLM with the result of the function call, allow it to continue
+            self.submit()
             return
 
         # All other finish reasons are valid for regular assistant messages
 
         # Wrap up the previous assistant
-        self.messages.append(assistant(mark.message))
+        if mark is not None and mark.message.strip() != "":
+            self.messages.append(assistant(mark.message))
 
         if finish_reason == 'stop':
             return
         elif finish_reason == 'max_tokens' or finish_reason == 'length':
             mark.append("\n...max tokens or overall length is too high...\n")
         elif finish_reason == 'content_filter':
             mark.append("\n...Content omitted due to OpenAI content filters...\n")
@@ -217,24 +228,27 @@
         # Messages are either a dict respecting the {role, content} format or a str that we convert to a human message
         for message in messages:
             if isinstance(message, str):
                 self.messages.append(human(message))
             else:
                 self.messages.append(message)
 
-    def register(
-        self, function: Callable, parameters_model: Optional["BaseModel"] = None, json_schema: Optional[dict] = None
-    ):
+    def register(self, function: Callable, parameter_schema: Optional[Union[Type["BaseModel"], dict]] = None):
         """Register a function with the ChatLab instance.
 
         Args:
             function (Callable): The function to register.
 
-            parameters_model (BaseModel): The pydantic model to use for the function's parameters.
-
-            json_schema (dict): The JSON schema to use for the function's parameters.
+            parameter_schema (BaseModel or dict): The pydantic model or JSON schema for the function's parameters.
 
         """
-        full_schema = self.function_registry.register(function, parameters_model, json_schema)
+        full_schema = self.function_registry.register(function, parameter_schema)
+
+        return full_schema
+
+    def get_history(self):
+        """Returns the conversation history as a list of messages."""
+        return self.messages
 
-        logger.debug("Created function with schema:")
-        logger.debug(json.dumps(full_schema, indent=2))
+    def clear_history(self):
+        """Clears the conversation history."""
+        self.messages = []
```

### Comparing `chatlab-0.13.0/chatlab/display.py` & `chatlab-0.14.0/chatlab/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Stylized representation of a Chat Function Call as we dance with the LLM."""
 
 import os
 from binascii import hexlify
 from typing import Optional
 
-from chatlab.registry import FunctionArgumentError, FunctionRegistry, UnknownFunctionError
 from IPython.core import display_functions
 from vdom import details, div, span, style, summary
 
 # Importing for the sake of backwards compatibility
 from .markdown import Markdown  # noqa: F401
 from .messaging import Message, function_result, system
+from .registry import FunctionArgumentError, FunctionRegistry, UnknownFunctionError
 
 # Palette used here is https://colorhunt.co/palette/27374d526d829db2bfdde6ed
 colors = {
     "darkest": "#27374D",
     "dark": "#526D82",
     "light": "#9DB2BF",
     "lightest": "#DDE6ED",
@@ -68,14 +68,15 @@
             background=colors["ultralight"],
             color=colors["darkest"],
             padding="10px",
             marginBottom="10px",
             unicodeBidi="embed",
             fontFamily="monospace",
             whiteSpace="pre",
+            overflow="scroll",
         ),
     )
 
 
 def ChatFunctionComponent(
     name: str,
     verbage: str,
@@ -172,20 +173,37 @@
             self.finished = True
             self.set_state("Errored")
             return system(f"Function arguments for {function_name} were invalid: {e}")
         except UnknownFunctionError as e:
             self.finished = True
             self.set_state("No function named")
             return system(f"Function {function_name} not found in function registry: {e}")
+        except Exception as e:
+            # Check to see if the user has requested that the exception be exposed to LLM.
+            # If not, then we just raise it and let the user handle it.
+            chatlab_metadata = self.function_registry.get_chatlab_metadata(function_name)
+
+            if not chatlab_metadata.expose_exception_to_llm:
+                # Bubble up the exception to the user
+                raise
+
+            repr_llm = repr(e)
+
+            self.function_result = repr_llm
+            self.finished = True
+            self.state = "Errored"
+            self.update_displays()
+
+            return function_result(name=function_name, content=repr_llm)
 
         repr_llm = repr(output)
 
         self.function_result = repr_llm
         self.finished = True
-        self.state = "Finished"
+        self.state = "Ran"
         self.update_displays()
 
         return function_result(name=function_name, content=repr_llm)
 
     def append_arguments(self, args: str):
         """Append more characters to the `function_args`."""
         if self.function_args is None:
```

### Comparing `chatlab-0.13.0/chatlab/markdown.py` & `chatlab-0.14.0/chatlab/markdown.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,17 +57,14 @@
         self.message += delta
 
     def extend(self, delta_generator: Iterator[str]) -> None:
         """Extend the `Markdown` with a generator/iterator of strings."""
         for delta in delta_generator:
             self.append(delta)
 
-    # Alias consume
-    consume = extend
-
     def display(self) -> None:
         """Display the `Markdown` with a display ID for receiving updates."""
         display_functions.display(self, display_id=self._display_id)
 
     def update_displays(self) -> None:
         """Force an update to all displays of this `Markdown`."""
         display_functions.display(self, display_id=self._display_id, update=True)
```

### Comparing `chatlab-0.13.0/chatlab/messaging.py` & `chatlab-0.14.0/chatlab/messaging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,162 @@
-"""Little messaging helpers for ChatLab.
+"""Helpers for messaging in ChatLab.
 
->>> from chatlab import ChatLab, ai, human, system
->>> chatlab = ChatLab(system("You are a large bird"))
->>> chatlab.submit(human("What are you?"))
-I am a large bird.
+This module contains helper functions for creating different types of messages in ChatLab.
+
+Example:
+    >>> from chatlab import ChatLab, ai, human, system
+    >>> chatlab = ChatLab(system("You are a large bird"))
+    >>> chatlab.submit(human("What are you?"))
+    I am a large bird.
 
 """
-from typing import Iterator, List, Optional, TypedDict
 
-from typing_extensions import NotRequired
+from typing import List, Optional, TypedDict, Union
+
+BasicMessage = TypedDict(
+    "BasicMessage",
+    {
+        "role": str,
+        "content": str,
+    },
+)
+
 
 FunctionCall = TypedDict(
     "FunctionCall",
     {
-        "name": Optional[str],
+        "name": str,
         "arguments": Optional[str],
     },
 )
 
+FunctionCallMessage = TypedDict(
+    "FunctionCallMessage",
+    {
+        "role": str,
+        "content": Optional[str],
+        "function_call": FunctionCall,
+    },
+)
+
+FunctionResultMessage = TypedDict(
+    "FunctionResultMessage",
+    {
+        "role": str,
+        "content": str,
+        "name": str,
+    },
+)
+
+Message = Union[BasicMessage, FunctionCallMessage, FunctionResultMessage]
+
+
 Delta = TypedDict(
     "Delta",
     {
-        "function_call": Optional[FunctionCall],
+        "function_call": FunctionCall,
         "content": Optional[str],
         "finish_reason": Optional[str],
     },
+    total=False,
 )
 
 
 StreamChoice = TypedDict(
     "StreamChoice",
     {
         "delta": Delta,
     },
+    total=False,
 )
 
 StreamCompletion = TypedDict(
     "StreamCompletion",
     {
         "choices": List[StreamChoice],
     },
+    total=False,
 )
 
 
-Message = TypedDict(
-    "Message",
-    {
-        "role": str,
-        "content": Optional[str],
-        "name": NotRequired[str],
-        "function_call": NotRequired[FunctionCall],
-    },
-)
-
-
-def assistant(content: str) -> Message:
+def assistant(content: str) -> BasicMessage:
     """Create a message from the assistant.
 
-    >>> from chatlab import assistant
-    >>> assistant("Hello!")
-    {'role': 'assistant', 'content': 'Hello!'}
+    Args:
+        content: The content of the message.
+
+    Returns:
+        A dictionary representing the assistant's message.
     """
     return {
         'role': 'assistant',
         'content': content,
     }
 
 
-def user(content: str) -> Message:
-    """Create a message from the user."""
+def user(content: str) -> BasicMessage:
+    """Create a message from the user.
+
+    Args:
+        content: The content of the message.
+
+    Returns:
+        A dictionary representing the user's message.
+    """
     return {
         'role': 'user',
         'content': content,
     }
 
 
-def system(content: str) -> Message:
-    """Create a message from the system."""
+def system(content: str) -> BasicMessage:
+    """Create a message from the system.
+
+    Args:
+        content: The content of the message.
+
+    Returns:
+        A dictionary representing the system's message.
+    """
     return {
         'role': 'system',
         'content': content,
     }
 
 
-def assistant_function_call(name: str, arguments: Optional[str]) -> Message:
-    """Create a function call message."""
+def assistant_function_call(name: str, arguments: Optional[str] = None) -> FunctionCallMessage:
+    """Create a function call message from the assistant.
+
+    Args:
+        name: The name of the function to call.
+        arguments: Optional; The arguments to pass to the function.
+
+    Returns:
+        A dictionary representing a function call message from the assistant.
+    """
     return {
         'role': 'assistant',
         'content': None,
         'function_call': {
             'name': name,
             'arguments': arguments,
         },
     }
 
 
-def function_result(name: str, content: str) -> Message:
-    """Create a function message."""
+def function_result(name: str, content: str) -> FunctionResultMessage:
+    """Create a function result message.
+
+    Args:
+        name: The name of the function.
+        content: The content of the message.
+
+    Returns:
+        A dictionary representing a function result message.
+    """
     return {
         'role': 'function',
         'content': content,
         'name': name,
     }
```

### Comparing `chatlab-0.13.0/chatlab/registry.py` & `chatlab-0.14.0/chatlab/registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 
     conversation.submit("What time is it?")
 
 """
 
 import inspect
 import json
-from typing import Callable, Optional, Union, get_args, get_origin
+from typing import Any, Callable, Optional, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel
 
-from chatlab.builtins import run_cell
+from .builtins import run_cell
+from .decorators import ChatlabMetadata
 
 
 class FunctionArgumentError(Exception):
     """Exception raised when a function is called with invalid arguments."""
 
     pass
 
@@ -74,29 +75,34 @@
 
 
 def is_optional_type(t):
     """Check if a type is Optional."""
     return get_origin(t) is Union and len(get_args(t)) == 2 and type(None) in get_args(t)
 
 
-def generate_function_schema(function: Callable, parameters_model: Optional["BaseModel"] = None):
+def generate_function_schema(
+    function: Callable,
+    parameter_schema: Optional[Union[Type["BaseModel"], dict]] = None,
+):
     """Generate a function schema for sending to OpenAI."""
     doc = function.__doc__
     func_name = function.__name__
 
     if not func_name:
         raise Exception("Function must have a name")
     if func_name == "<lambda>":
         raise Exception("Lambdas cannot be registered. Use `def` instead.")
     if not doc:
         raise Exception("Only functions with docstrings can be registered")
 
     schema = None
-    if parameters_model is not None:
-        schema = parameters_model.schema()
+    if isinstance(parameter_schema, dict):
+        schema = parameter_schema
+    elif parameter_schema is not None:
+        schema = parameter_schema.schema()
     else:
         schema_properties = {}
         sig = inspect.signature(function)
         for name, param in sig.parameters.items():
             if param.annotation == inspect.Parameter.empty:
                 raise Exception(f"Parameter {name} of function {func_name} must have a type annotation")
 
@@ -115,15 +121,18 @@
 
             elif param.annotation in ALLOWED_TYPES:
                 schema_properties[name] = {
                     "type": JSON_SCHEMA_TYPES[param.annotation],
                 }
 
             else:
-                raise Exception(f"Type annotation of parameter {name} in function {func_name} is not allowed")
+                raise Exception(
+                    f"Type annotation of parameter {name} in function {func_name} "
+                    f"must be a JSON serializable type ({ALLOWED_TYPES})"
+                )
 
         schema = {"type": "object", "properties": {}, "required": []}
         if len(schema_properties) > 0:
             schema = {
                 "type": "object",
                 "properties": schema_properties,
                 "required": [
@@ -152,36 +161,41 @@
     def __init__(self, allow_hallucinated_python: bool = False):
         """Initialize a FunctionRegistry object."""
         self.__functions = {}
         self.__schemas = {}
         self.allow_hallucinated_python = allow_hallucinated_python
 
     def register(
-        self, function: Callable, parameters_model: Optional["BaseModel"] = None, json_schema: Optional[dict] = None
-    ):
-        """Register a function with a schema for sending to OpenAI."""
-        if parameters_model is not None and json_schema is not None:
-            raise Exception("Cannot specify both parameters_model and json_schema")
-
-        # Assume that if json_schema is passed, it is valid and complete
-        # json_schema takes precedence over parameters_model and auto-inferred schema
-        schema = json_schema
-        if schema is None:
-            schema = generate_function_schema(function, parameters_model)
+        self,
+        function: Callable,
+        parameter_schema: Optional[Union[Type["BaseModel"], dict]] = None,
+    ) -> dict:
+        """Register a function for use in `Conversation`s."""
+        final_schema = generate_function_schema(function, parameter_schema)
 
         self.__functions[function.__name__] = function
-        self.__schemas[function.__name__] = schema
+        self.__schemas[function.__name__] = final_schema
 
-        return schema
+        return final_schema
 
-    def get(self, function_name):
+    def get(self, function_name) -> Optional[Callable]:
         """Get a function by name."""
         return self.__functions.get(function_name)
 
-    def call(self, name: str, arguments: Optional[str] = None):
+    def get_chatlab_metadata(self, function_name) -> ChatlabMetadata:
+        """Get the chatlab metadata for a function by name."""
+        function = self.get(function_name)
+
+        if function is None:
+            raise UnknownFunctionError(f"Function {function_name} is not registered")
+
+        chatlab_metadata = getattr(function, "chatlab_metadata", ChatlabMetadata())
+        return chatlab_metadata
+
+    def call(self, name: str, arguments: Optional[str] = None) -> Any:
         """Call a function by name with the given parameters."""
         function = self.get(name)
         parameters: dict = {}
 
         # Handle the code interpreter hallucination
         if name == "python" and self.allow_hallucinated_python:
             function = run_cell
@@ -195,17 +209,18 @@
         else:
             try:
                 parameters = json.loads(arguments)
                 # TODO: Validate parameters against schema
             except json.JSONDecodeError:
                 raise FunctionArgumentError(f"Invalid JSON for parameters of function {name}")
 
-        return function(**parameters)
+        result = function(**parameters)
+        return result
 
-    def __contains__(self, name):
+    def __contains__(self, name) -> bool:
         """Check if a function is registered by name."""
         return name in self.__functions
 
     @property
     def function_definitions(self) -> list[dict]:
         """Get a list of function definitions."""
         return list(self.__schemas.values())
```

### Comparing `chatlab-0.13.0/pyproject.toml` & `chatlab-0.14.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatlab"
-version = "0.13.0"
+version = "0.14.0"
 homepage = "https://github.com/rgbkrk/chatlab"
 description = "Markdown for LLMs."
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -43,14 +43,15 @@
 pip = "^23.0.1"
 twine = "^4.0.2"
 pre-commit = "^3.2.2"
 toml = "^0.10.2"
 bump2version = "^1.0.1"
 jinja2 = "^3.1.2"
 ipykernel = "^6.23.2"
+types-toml = "^0.10.8.6"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "mypy",
```

### Comparing `chatlab-0.13.0/PKG-INFO` & `chatlab-0.14.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatlab
-Version: 0.13.0
+Version: 0.14.0
 Summary: Markdown for LLMs.
 Home-page: https://github.com/rgbkrk/chatlab
 License: BSD-3-Clause
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,41 +28,72 @@
 
 # ChatLab
 
 **Chat Experiments, Simplified**
 
 💬🔬
 
-Chatlab is where chat conversations take shape. It’s your laboratory for experimenting with and crafting intelligent conversations using OpenAI’s chat models.
+ChatLab is a Python package that makes it easy to experiment with OpenAI's chat models. It provides a simple interface for chatting with the models and a way to register functions that can be called from the chat model.
 
-## Introduction
+Best yet, it's interactive in the notebook!
 
-Welcome to Chatlab, your personal workshop for chat innovation. Are you intrigued by conversational AI? Chatlab empowers developers to mold conversations according to their vision. Whether you are an AI enthusiast, researcher, or developer, Chatlab provides you with the building blocks and tools necessary for crafting intelligent conversations seamlessly. 🧪💬
+## Introduction
 
 ```python
 import chatlab
+import random
+
+def flip_a_coin():
+    '''Returns heads or tails'''
+    return random.choice(['heads', 'tails'])
 
 conversation = chatlab.Conversation()
+conversation.register(flip_a_coin)
 
-conversation.submit("How much wood could a")
+conversation.submit("Please flip a coin for me")
 ```
 
-```markdown
-woodchuck chuck if a woodchuck could chuck wood?
+<details style="background:#DDE6ED;color:#27374D;padding:.5rem 1rem;borderRadius:5px">
+<summary>&nbsp;𝑓&nbsp; Ran `flip_a_coin`
+</summary>
+<br />
+
+Input:
+
+```json
+{}
+```
+
+Output:
+
+```json
+"tails"
 ```
 
-In the notebook, text will stream into a Markdown output.
+</details>
+
+```markdown
+It landed on tails!
+```
 
-![image](https://github.com/rgbkrk/chatlab/assets/836375/81b2837c-430c-42eb-ae60-0c3a91ae26b6)
+In the notebook, text will stream into a Markdown output and function inputs and outputs are a nice collapsible display, like with ChatGPT Plugins.
 
-When using chat functions in the notebook\*, you'll get a nice collapsible display of inputs and outputs.
+<details class="details-reset border rounded-2" open="">
+  <summary class="px-3 py-2">
+    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-device-camera-video">
+    <path d="M16 3.75v8.5a.75.75 0 0 1-1.136.643L11 10.575v.675A1.75 1.75 0 0 1 9.25 13h-7.5A1.75 1.75 0 0 1 0 11.25v-6.5C0 3.784.784 3 1.75 3h7.5c.966 0 1.75.784 1.75 1.75v.675l3.864-2.318A.75.75 0 0 1 16 3.75Zm-6.5 1a.25.25 0 0 0-.25-.25h-7.5a.25.25 0 0 0-.25.25v6.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-6.5ZM11 8.825l3.5 2.1v-5.85l-3.5 2.1Z"></path>
+</svg>
+    <span aria-label="Video description flip-a-coin-chatlab.mp4" class="m-1">flip-a-coin-chatlab.mp4</span>
+    <span class="dropdown-caret"></span>
+  </summary>
 
-![click](https://github.com/rgbkrk/chatlab/assets/836375/21c6bd4c-cd3b-48b9-812a-2b86a05c20da)
+  <video src="https://user-images.githubusercontent.com/836375/248335062-fdc523b1-ca31-4506-b3ed-c73be9eb0d88.mp4" data-canonical-src="https://user-images.githubusercontent.com/836375/248335062-fdc523b1-ca31-4506-b3ed-c73be9eb0d88.mp4" controls="controls" muted="muted" class="d-block rounded-bottom-2 border-top width-fit" style="max-height:640px; min-height: 200px">
 
-\* Tested in JupyterLab and Noteable
+  </video>
+</details>
 
 ### Installation
 
 ```bash
 pip install chatlab
 ```
 
@@ -70,20 +101,19 @@
 
 You'll need to set your `OPENAI_API_KEY` environment variable. You can find your API key on your [OpenAI account page](https://platform.openai.com/account/api-keys). I recommend setting it in an `.env` file when working locally.
 
 On hosted environments like Noteable, set it in your Secrets to keep it safe from prying LLM eyes.
 
 ## What can `Conversation`s enable _you_ to do?
 
-<center><img src="https://cdn.donmai.us/original/64/e7/64e78d7968c8317b84a95e152e4a087b.png" height="100" /></center>
-<br />
+💬
 
 Where `Conversation`s take it next level is with _Chat Functions_. You can
 
--   declare a function with a schema
+-   declare a function
 -   register the function in your `Conversation`
 -   watch as Chat Models call your functions!
 
 You may recall this kind of behavior from [ChatGPT Plugins](https://noteable.io/chatgpt-plugin-for-notebook/). Now, you can take this even further with your own custom code.
 
 As an example, let's give the large language models the ability to tell time.
 
@@ -120,24 +150,41 @@
 # Register our function
 conversation.register(what_time, WhatTime)
 
 # Pluck the submit off for easy access as chat
 chat = conversation.submit
 ```
 
-After that, we can call `chat` with direct strings (which are turned into user messages) or using simple message makers from `chatlab` named `human`/`user` and `narrate`/`system`.
+After that, we can call `chat` with direct strings (which are turned into user messages) or using simple message makers from `chatlab` named `user` and `system`.
 
 ```python
 chat("What time is it?")
 ```
 
-```markdown
-▶ 𝑓 Ran `what_time`
+<details style="background:#DDE6ED;color:#27374D;padding:.5rem 1rem;borderRadius:5px">
+<summary>&nbsp;𝑓&nbsp; Ran `what_time`
+</summary>
+<br />
+
+Input:
+
+```json
+{}
+```
+
+Output:
+
+```json
+"11:19 AM"
+```
+
+</details>
 
-The current time is 11:47 PM.
+```markdown
+The current time is 11:19 AM.
 ```
 
 ## Interface
 
 The `chatlab` package exports
 
 ### `Conversation`
@@ -145,15 +192,15 @@
 The `Conversation` class is the main way to chat using OpenAI's models. It keeps a history of your chat in `Conversation.messages`.
 
 #### `Conversation.submit`
 
 When you call `submit`, you're sending over messages to the chat model and getting back an updating `Markdown` display live as well as a interactive details area for any function calls.
 
 ```python
-conversation.submit("What would a parent who says "I have to play zone defense" mean? ")
+conversation.submit('What would a parent who says "I have to play zone defense" mean? ')
 # Markdown response inline
 conversation.messages
 ```
 
 ```js
 [{'role': 'user',
   'content': 'What does a parent of three kids mean by "I have to play zone defense"?'},
```

