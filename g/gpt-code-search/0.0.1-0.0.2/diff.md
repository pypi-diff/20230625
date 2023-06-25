# Comparing `tmp/gpt_code_search-0.0.1.tar.gz` & `tmp/gpt_code_search-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.1.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.2.tar", max compression
```

## Comparing `gpt_code_search-0.0.1.tar` & `gpt_code_search-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.1/LICENSE
--rw-r--r--   0        0        0     2470 2023-06-23 21:11:19.022925 gpt_code_search-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.1/core/__init__.py
--rw-r--r--   0        0        0     4753 2023-06-25 04:39:07.965531 gpt_code_search-0.0.1/core/ai.py
--rw-r--r--   0        0        0     4090 2023-06-24 18:02:42.612764 gpt_code_search-0.0.1/core/functions.py
--rw-r--r--   0        0        0      637 2023-06-25 04:22:23.042891 gpt_code_search-0.0.1/core/main.py
--rw-r--r--   0        0        0     1073 2023-06-25 04:36:20.217245 gpt_code_search-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 gpt_code_search-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3499 2023-06-25 08:09:06.761033 gpt_code_search-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.2/core/__init__.py
+-rw-r--r--   0        0        0     5851 2023-06-25 07:48:46.662311 gpt_code_search-0.0.2/core/ai.py
+-rw-r--r--   0        0        0     1467 2023-06-25 08:09:28.571788 gpt_code_search-0.0.2/core/config.py
+-rw-r--r--   0        0        0     6607 2023-06-25 06:48:57.118776 gpt_code_search-0.0.2/core/functions.py
+-rw-r--r--   0        0        0     2633 2023-06-25 08:09:28.580932 gpt_code_search-0.0.2/core/main.py
+-rw-r--r--   0        0        0     1090 2023-06-25 08:13:58.934605 gpt_code_search-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4668 1970-01-01 00:00:00.000000 gpt_code_search-0.0.2/PKG-INFO
```

### Comparing `gpt_code_search-0.0.1/LICENSE` & `gpt_code_search-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.1/README.md` & `gpt_code_search-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,42 +7,98 @@
     src="https://raw.githubusercontent.com/wolfia-app/gpt-code-search/main/public/logo.png"
   />
   <p>
     <b>gpt-code-search</b> enables you to search your codebase with natural language using GPT-4.
   </p>
 </div>
 
+## Features
+
+- 🧠 **GPT-4**: code search, retrieval, and answering all done with OpenAI and [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+- 🔐 **Privacy-first**: code snippets only leave your machine when you ask a question and the LLM requests the relevant code.
+- 🔥 **Works instantly**: no pre-processing, chunking, or indexing, get started right away.
+- 📦 **File-system backed**: works with any code on your machine.
+
+## Getting Started
+
+### Installation
+
+```bash
+pip install gpt-code-search
+```
+
+### Usage
+
+#### Ask a question about your codebase
+
+```bash
+gpt-code-search query "What does this codebase do?"
+```
+
+#### Select a model
+
+```bash
+gpt-code-search select-model
+```
+
+Defaults to `gpt-3.5-turbo-16k`. The selected model is stored in `~/$HOME/.gpt-code-search/config.toml`.
+
+
+### Configuration
+
+The tool will prompt you to configure the `OPENAI_API_KEY`, if you haven't already.
+
 ## Problem
 
 You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste code snippets into a prompt nor send your code to another third-party service.
 
 This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. This removes the need to copy and paste or send your code to another third-party. Also, it meets you where you already live, in your terminal, not a new UI or window.
 
 Examples of the types of questions you might want to ask:
 
 - 🐛 Help debugging errors and finding the relevant code and files
 - 📝 Document large files or functionalities formatted as markdown
 - 📨 Ask general questions about any part of the code
 - 🛠️ Generate new code based on existing files and conventions
 
-## Features
-
-- 🧠 **GPT-4**: code search, retrieval, and answering all done with OpenAI and [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
-- 🔐 **Privacy-first**: code snippets only leave your machine when you ask a question and the LLM requests the relevant code.
-- 🔥 **Works instantly**: no pre-processing, chunking, or indexing, get started right away.
-- 📦 **File-system backed**: works with any code on your machine.
-
-## Getting Started
-
-TODO
-
 ## Privacy
 
 Outside of the LLM, no data is sent or stored.
 
 The only data sent to LLM is the question you ask and the code snippets that is requests related to your question. All code snippets are retrieved from your local machine.
 
 ## Wolfia Codex
 
 This tool is a simplified version of [Wolfia Codex](https://wolfia.com), a cloud tool that enables you to ask any question about open source and private code bases like [`Langchain`](https://wolfia.com/?projectId=2b964031-0ce8-472a-abb7-27079a7b84f3), [`Vercel ai`](https://wolfia.com/?projectId=4710df1f-43f8-4d30-863b-d67876ae0f06), or [`gpt-engineer`](https://wolfia.com/?projectId=8d9dd449-da2d-410e-a4fc-f2ff75a30f73).
 
 If you're looking for a more powerful tool, or avoiding the setup, check out [Wolfia Codex](https://wolfia.com), search codebases, share your questions and answers, and more!
+
+## Development
+
+The project uses [poetry](https://python-poetry.org/) for dependency management and packaging. To get started, install poetry and run the following commands:
+
+```bash
+# Install dependencies
+poetry install
+```
+
+Run the project
+
+```bash
+# Run the project
+poetry run python core/main.py
+```
+
+Install pre-commit hooks
+
+```bash
+# Install pre-commit hooks
+poetry run pre-commit install
+```
+
+## Contact
+
+If you need help or have any questions, please reach out to us at [support@wolfia.com](mailto:support@wolfia.com).
+
+## License
+
+Apache 2.0 © [Wolfia](https://wolfia.com)
```

### Comparing `gpt_code_search-0.0.1/core/ai.py` & `gpt_code_search-0.0.2/core/ai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,93 @@
 import json
 import logging
 
 import openai
 import requests
 from rich.markdown import Markdown
 
-from core.functions import get_file_tree, get_contents_of_file, enabled_functions, truncate_text_to_token_limit
+from core.config import load_selected_model
+from core.functions import (
+    MAX_DEPTH,
+    enabled_functions,
+    get_contents_of_file,
+    get_file_tree,
+    search_codebase,
+    truncate_text_to_token_limit,
+)
 
 # Reduced from 16k to 14k to allow for prompt context
 MAX_TOKENS = 14_000
 
+PROMPT = """\
+You're a incredible powered coding assistant. Your role is to help users understand and navigate their codebases,
+providing assistance across a range of tasks.
 
-def chat_completion_request(messages, functions=None, model="gpt-3.5-turbo-16k"):
+## Problem
+
+You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste
+code snippets into a prompt or send your code to another third-party service.
+
+You help by determine the most relevant code snippets within your codebase. No copying, pasting, or sharing code
+required. It meets you where you already live: in your terminal.
+
+Use cases that you will support out of the box:
+- 📨 Asking general questions about any part of the code
+- 📝 Documenting large files or functionalities in markdown
+- 🛠️ Generating new code based on existing files and conventions
+- 🐛 Debugging errors and finding relevant code and files
+
+You have access to three primary functions:
+- `search_codebase(keywords, start_path, max_depth)`: Search the codebase for a keyword.
+- `get_file_tree(start_path, max_depth)`: Retrieve the project's file structure.
+- `get_contents_of_file(path)`: Fetch the contents of a file.
+
+Use these tools to debug, create documentation, answer code-related queries, and generate code snippets
+in line with the project's style. You will always use these functions before answering a question, particularly
+`search_codebase`. You will not answer any questions without using these functions first.
+
+Before answering, search the codebase or file tree. Review at least five files and reference the most relevant one. You
+will not answer any questions without looking up a file first. If you cannot find a relevant file, say 'I don't know'.
+If you don't, you will be penalized. Function calls are capped at ten per session. If a 'readme.md' file exists, start
+there. Otherwise, use file names and content.
+
+Compose responses in markdown with code when necessary. Aim for thorough answers, and it's okay to say 'I don't know'.
+Your objective is to provide the most accurate and detailed answer possible, even if it results in a longer response.
+Let's start assisting with your coding tasks!
+"""
+
+
+def chat_completion_request(messages, functions=None):
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Bearer " + openai.api_key,
     }
     json_data = {
-        "model": model,
+        "model": load_selected_model(),
         "messages": messages,
         "functions": functions or [],
         "function_call": "auto",
         "temperature": 0,
     }
     try:
         response = requests.post(
             "https://api.openai.com/v1/chat/completions",
             headers=headers,
             json=json_data,
-            timeout=180
+            timeout=180,
         )
         return response
     except requests.exceptions.HTTPError as http_err:
         logging.error(f"HTTP error occurred during ChatCompletion request: {http_err}")
         logging.error(f"Response content: {response.content}")
         return http_err
     except Exception as e:
-        logging.error("Unable to generate ChatCompletion response due to the following exception:")
+        logging.error(
+            "Unable to generate ChatCompletion response due to the following exception:"
+        )
         logging.error(f"Exception: {e}")
         return e
 
 
 def get_next_completion(previous_response, messages, functions):
     assistant_message = previous_response.json()["choices"][0]["message"]
     messages.append(assistant_message)
@@ -50,23 +97,29 @@
 
     function_name = assistant_message["function_call"]["name"]
     try:
         function_args = json.loads(assistant_message["function_call"]["arguments"])
     except json.JSONDecodeError:
         return None
 
-    if function_name == 'get_file_tree':
+    if function_name == "get_file_tree":
         function_call = get_file_tree
-        start_path = function_args.get('start_path')
-        max_depth = int(function_args.get('max_depth'))
-        function_response = function_call(start_path, max_depth)
-    elif function_name == 'get_contents_of_file':
+        start_path = function_args.get("start_path")
+        max_depth = function_args.get("max_depth") or MAX_DEPTH
+        function_response = function_call(start_path, int(max_depth))
+    elif function_name == "get_contents_of_file":
         function_call = get_contents_of_file
-        file_path = function_args.get('path')
+        file_path = function_args.get("path")
         function_response = function_call(file_path)
+    elif function_name == "search_codebase":
+        function_call = search_codebase
+        keywords = function_args.get("keywords")
+        start_path = function_args.get("start_path") or "."
+        max_depth = function_args.get("max_depth") or MAX_DEPTH
+        function_response = function_call(keywords, start_path, int(max_depth))
     else:
         raise ValueError(f"Function {function_name} not found.")
 
     truncated_response = truncate_text_to_token_limit(function_response, MAX_TOKENS)
 
     messages.append(
         {
@@ -82,34 +135,20 @@
     return next_response
 
 
 def chat_completions(query: str):
     while True:
         functions = enabled_functions()
         messages = [
-            {"role": "system",
-             "content": """You are an advanced coding assistant powered by GPT-4. Your task is to assist users in understanding and navigating their codebases, helping them with a variety of tasks, all based on the provided context.
-
-You have access to two powerful functions: get_file_tree(start_path, max_depth) and get_contents_of_file(path). The former returns the project's file tree, while the latter retrieves the contents of a specified file.
-
-Here are some common use-cases:
-
-1. Debugging: Help users debug errors by finding the relevant files and code snippets.
-2. Documentation: Generate well-structured documentation for large files or functionalities.
-3. General Queries: Answer general questions about any part of the code.
-4. Code Generation: Generate new code snippets that adhere to the existing project's style and conventions.
-
-Remember, always lookup the file tree first, before answering any questions. You can call functions a maximum of 10 times per session, so use your calls wisely. Try to lookup at least 5 different files before answering a question, and always reference the most relevant file. If you're unable to find a file or a confident answer, it's okay to say 'I don't know'.
-
-You have full access to the project's codebase, so feel free to use any part of it to answer questions. The current path is the root (.) of the project. And remember to always access the codebase through the functions provided before answering any questions.
-
-Please provide code when necessary and use markdown for the answer.
-                """
-             },
-            {"role": "user", "content": query}]
+            {
+                "role": "system",
+                "content": PROMPT,
+            },
+            {"role": "user", "content": query},
+        ]
 
         response = chat_completion_request(messages, functions)
         max_recursion = 10
         counter = 0
 
         while response is not None and counter < max_recursion:
             response = get_next_completion(response, messages, functions)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpt_code_search-0.0.1/core/functions.py` & `gpt_code_search-0.0.2/core/functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,46 @@
+import logging
 import os
-from typing import Union, List
+import re
+from typing import List, Union
 
 import tiktoken
 
-IGNORED_FOLDERS = ['__pycache__', '.git', '.idea', 'node_modules', '.bundle', '.gradle', 'build', '.DS_Store',
-                   '.ipynb_checkpoints']
-IGNORED_FILES = ['package-lock.json', '.env', 'Gemfile.lock', 'yarn.lock', '*.pyc', 'local.properties', '*.xcodeproj',
-                 '*.xcworkspace', '*.csv', '*.xlsx', '*.json', '.bat']
-
-
-def get_file_tree(start_path: str, max_depth: int, depth: int = 0) -> list:
+IGNORED_FOLDERS = [
+    "__pycache__",
+    ".git",
+    ".idea",
+    "node_modules",
+    ".bundle",
+    ".gradle",
+    "build",
+    ".DS_Store",
+    ".ipynb_checkpoints",
+]
+IGNORED_FILES = [
+    "package-lock.json",
+    ".env",
+    "Gemfile.lock",
+    "yarn.lock",
+    "*.pyc",
+    "local.properties",
+    "*.xcodeproj",
+    "*.xcworkspace",
+    "*.csv",
+    "*.xlsx",
+    "*.json",
+    ".bat",
+]
+
+MAX_DEPTH = 5
+
+
+def get_file_tree(
+    start_path: str = ".", max_depth: int = MAX_DEPTH, depth: int = 0
+) -> list:
     """
     Get the file tree of the project based on the current working directory.
     :param start_path: The path to the directory to start the search from.
     :param max_depth: The maximum depth of the search.
     :param depth: The current depth of the search.
     :return: The file tree.
     """
@@ -27,22 +54,54 @@
         if os.path.isfile(item_path):
             tree.append(item_path)
         elif os.path.isdir(item_path):
             tree += get_file_tree(item_path, max_depth, depth + 1)
     return tree
 
 
+def search_codebase(
+    keywords: List[str], start_path: str = ".", max_depth: int = 5
+) -> List[str]:
+    """
+    Search the codebase for a given list of keywords.
+    :param keywords: The list of keywords to search for.
+    :param start_path: The path to the directory to start the search from.
+    :param max_depth: The maximum depth of the search.
+    :return: A list of file paths that contain any of the keywords.
+    """
+    file_tree = get_file_tree(start_path, max_depth)
+    matching_files = set()
+
+    for file_path in file_tree:
+        try:
+            with open(file_path, "r", errors="ignore") as file:
+                contents = file.read()
+
+            if any(re.search(keyword, contents, re.IGNORECASE) for keyword in keywords):
+                matching_files.add(file_path)
+        except Exception:
+            logging.error("Error reading file: {}".format(file_path))
+
+    logging.info("Searching for keywords: {}".format(keywords))
+    logging.info(
+        "Found {} matching files in {}.".format(len(matching_files), start_path)
+    )
+    logging.info("Matching files: {}".format(matching_files))
+    return list(matching_files)
+
+
 def get_contents_of_file(file_path: str) -> str:
     """
     Get the contents of a file.
     :param file_path: The path to the file.
     :return: The contents of the file, or an empty string if the file is not found.
     """
     try:
-        with open(file_path, 'r') as file:
+        with open(file_path, "r") as file:
+            logging.info("Reading file: {}".format(file_path))
             return file.read()
     except FileNotFoundError:
         return ""
 
 
 def count_tokens(text: str) -> int:
     encoding = tiktoken.get_encoding("cl100k_base")
@@ -53,65 +112,95 @@
     """
     Truncate the text (or list of strings) to fit within the maximum token limit.
     :param text: The text or list of strings to truncate.
     :param max_tokens: The maximum number of tokens.
     :return: The truncated text or list of strings.
     """
     if isinstance(text, str):
-        chunks = text.split(' ')
+        chunks = text.split(" ")
     elif isinstance(text, list):
         chunks = text
     else:
         raise ValueError("The input text should be a string or a list of strings.")
 
-    total_tokens = sum(len(chunk.split(' ')) for chunk in chunks)
+    total_tokens = sum(len(chunk.split(" ")) for chunk in chunks)
 
     while total_tokens > max_tokens:
-        total_tokens -= len(chunks[-1].split(' '))
+        total_tokens -= len(chunks[-1].split(" "))
         chunks = chunks[:-1]
 
     if isinstance(text, str):
-        return ' '.join(chunks)
+        return " ".join(chunks)
     else:
         return chunks
 
 
 def enabled_functions():
     return [
         {
             "name": "get_file_tree",
-            "description": "Get the file tree of the project based on the current working directory. Access the current project root, with (./)",
+            "description": "Get the file tree of the project based on the current working directory. "
+            "Access the current project root, with (./)",
             "parameters": {
                 "type": "object",
                 "properties": {
                     "start_path": {
                         "type": "string",
-                        "description": "The path to the directory to start the search from."
+                        "description": "The path to the directory to start the search from.",
+                        "default": ".",
                     },
                     "max_depth": {
                         "type": "string",
-                        "description": "The maximum depth of the search. Use a max of 3 since the search is very slow.",
+                        "description": "The maximum depth of the search."
+                        "Use a max of {} since the search is very slow.".format(
+                            MAX_DEPTH
+                        ),
                     },
                     "depth": {
                         "type": "string",
                         "description": "The current depth of the search.",
                         "default": "0",
-                    }
+                    },
                 },
                 "required": ["start_path", "max_depth"],
             },
         },
         {
             "name": "get_contents_of_file",
             "description": "Get the contents of a file. Returns empty string if the file is not found.",
             "parameters": {
                 "type": "object",
                 "properties": {
                     "path": {
                         "type": "string",
-                        "description": "The path to the file."
+                        "description": "The path to the file.",
                     },
                 },
                 "required": ["path"],
-            }
+            },
+        },
+        {
+            "name": "search_codebase",
+            "description": "Search the codebase for a given list of keywords.",
+            "parameters": {
+                "type": "object",
+                "properties": {
+                    "keywords": {
+                        "type": "array",
+                        "items": {"type": "string"},
+                        "description": "The list of keywords to search for. Format: ['keyword1', 'keyword2']",
+                    },
+                    "start_path": {
+                        "type": "string",
+                        "description": "The path to the directory to start the search from.",
+                        "default": ".",
+                    },
+                    "max_depth": {
+                        "type": "string",
+                        "description": "The maximum depth of the search.",
+                        "default": "5",
+                    },
+                },
+                "required": ["keywords"],
+            },
         },
     ]
```

### Comparing `gpt_code_search-0.0.1/pyproject.toml` & `gpt_code_search-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.1"
+version = "0.0.2"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
 homepage = "https://wolfia.com"
 repository = "https://github.com/wolfia-app/gpt-code-search"
@@ -22,14 +22,15 @@
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
 rich = "^13.4.2"
 tiktoken = "^0.4.0"
 openai = "^0.27.8"
 termcolor = "^2.3.0"
 requests = "^2.31.0"
+toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.15.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gpt_code_search-0.0.1/PKG-INFO` & `gpt_code_search-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-search
-Version: 0.0.1
+Version: 0.0.2
 Summary: gpt-code-search enables you to search your codebase with natural language.
 Home-page: https://wolfia.com
 License: Apache-2.0
 Keywords: gpt,code,search,wolfia,gpt4,llm
 Author: narenmanoharan
 Author-email: narenkmanoharan@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: termcolor (>=2.3.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/wolfia-app/gpt-code-search
 Project-URL: discussions, https://github.com/wolfia-app/gpt-code-search/discussions
 Project-URL: issues, https://github.com/wolfia-app/gpt-code-search/issues
 Project-URL: wiki, https://github.com/wolfia-app/gpt-code-search/wiki
 Description-Content-Type: text/markdown
 
@@ -33,43 +34,99 @@
     src="https://raw.githubusercontent.com/wolfia-app/gpt-code-search/main/public/logo.png"
   />
   <p>
     <b>gpt-code-search</b> enables you to search your codebase with natural language using GPT-4.
   </p>
 </div>
 
+## Features
+
+- 🧠 **GPT-4**: code search, retrieval, and answering all done with OpenAI and [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
+- 🔐 **Privacy-first**: code snippets only leave your machine when you ask a question and the LLM requests the relevant code.
+- 🔥 **Works instantly**: no pre-processing, chunking, or indexing, get started right away.
+- 📦 **File-system backed**: works with any code on your machine.
+
+## Getting Started
+
+### Installation
+
+```bash
+pip install gpt-code-search
+```
+
+### Usage
+
+#### Ask a question about your codebase
+
+```bash
+gpt-code-search query "What does this codebase do?"
+```
+
+#### Select a model
+
+```bash
+gpt-code-search select-model
+```
+
+Defaults to `gpt-3.5-turbo-16k`. The selected model is stored in `~/$HOME/.gpt-code-search/config.toml`.
+
+
+### Configuration
+
+The tool will prompt you to configure the `OPENAI_API_KEY`, if you haven't already.
+
 ## Problem
 
 You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste code snippets into a prompt nor send your code to another third-party service.
 
 This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. This removes the need to copy and paste or send your code to another third-party. Also, it meets you where you already live, in your terminal, not a new UI or window.
 
 Examples of the types of questions you might want to ask:
 
 - 🐛 Help debugging errors and finding the relevant code and files
 - 📝 Document large files or functionalities formatted as markdown
 - 📨 Ask general questions about any part of the code
 - 🛠️ Generate new code based on existing files and conventions
 
-## Features
-
-- 🧠 **GPT-4**: code search, retrieval, and answering all done with OpenAI and [function calling](https://openai.com/blog/function-calling-and-other-api-updates).
-- 🔐 **Privacy-first**: code snippets only leave your machine when you ask a question and the LLM requests the relevant code.
-- 🔥 **Works instantly**: no pre-processing, chunking, or indexing, get started right away.
-- 📦 **File-system backed**: works with any code on your machine.
-
-## Getting Started
-
-TODO
-
 ## Privacy
 
 Outside of the LLM, no data is sent or stored.
 
 The only data sent to LLM is the question you ask and the code snippets that is requests related to your question. All code snippets are retrieved from your local machine.
 
 ## Wolfia Codex
 
 This tool is a simplified version of [Wolfia Codex](https://wolfia.com), a cloud tool that enables you to ask any question about open source and private code bases like [`Langchain`](https://wolfia.com/?projectId=2b964031-0ce8-472a-abb7-27079a7b84f3), [`Vercel ai`](https://wolfia.com/?projectId=4710df1f-43f8-4d30-863b-d67876ae0f06), or [`gpt-engineer`](https://wolfia.com/?projectId=8d9dd449-da2d-410e-a4fc-f2ff75a30f73).
 
 If you're looking for a more powerful tool, or avoiding the setup, check out [Wolfia Codex](https://wolfia.com), search codebases, share your questions and answers, and more!
 
+## Development
+
+The project uses [poetry](https://python-poetry.org/) for dependency management and packaging. To get started, install poetry and run the following commands:
+
+```bash
+# Install dependencies
+poetry install
+```
+
+Run the project
+
+```bash
+# Run the project
+poetry run python core/main.py
+```
+
+Install pre-commit hooks
+
+```bash
+# Install pre-commit hooks
+poetry run pre-commit install
+```
+
+## Contact
+
+If you need help or have any questions, please reach out to us at [support@wolfia.com](mailto:support@wolfia.com).
+
+## License
+
+Apache 2.0 © [Wolfia](https://wolfia.com)
+
```

