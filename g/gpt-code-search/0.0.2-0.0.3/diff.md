# Comparing `tmp/gpt_code_search-0.0.2.tar.gz` & `tmp/gpt_code_search-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_code_search-0.0.2.tar", max compression
+gzip compressed data, was "gpt_code_search-0.0.3.tar", max compression
```

## Comparing `gpt_code_search-0.0.2.tar` & `gpt_code_search-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.2/LICENSE
--rw-r--r--   0        0        0     3499 2023-06-25 08:09:06.761033 gpt_code_search-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.2/core/__init__.py
--rw-r--r--   0        0        0     5851 2023-06-25 07:48:46.662311 gpt_code_search-0.0.2/core/ai.py
--rw-r--r--   0        0        0     1467 2023-06-25 08:09:28.571788 gpt_code_search-0.0.2/core/config.py
--rw-r--r--   0        0        0     6607 2023-06-25 06:48:57.118776 gpt_code_search-0.0.2/core/functions.py
--rw-r--r--   0        0        0     2633 2023-06-25 08:09:28.580932 gpt_code_search-0.0.2/core/main.py
--rw-r--r--   0        0        0     1090 2023-06-25 08:13:58.934605 gpt_code_search-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4668 1970-01-01 00:00:00.000000 gpt_code_search-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 21:11:19.022270 gpt_code_search-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3472 2023-06-25 08:50:47.525612 gpt_code_search-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 04:13:32.205359 gpt_code_search-0.0.3/core/__init__.py
+-rw-r--r--   0        0        0     5100 2023-06-25 09:12:28.089552 gpt_code_search-0.0.3/core/ai.py
+-rw-r--r--   0        0        0     1568 2023-06-25 08:20:29.932487 gpt_code_search-0.0.3/core/config.py
+-rw-r--r--   0        0        0     6748 2023-06-25 09:12:28.560468 gpt_code_search-0.0.3/core/functions.py
+-rw-r--r--   0        0        0     3476 2023-06-25 09:04:29.759102 gpt_code_search-0.0.3/core/main.py
+-rw-r--r--   0        0        0     1090 2023-06-25 08:37:42.132668 gpt_code_search-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4641 1970-01-01 00:00:00.000000 gpt_code_search-0.0.3/PKG-INFO
```

### Comparing `gpt_code_search-0.0.2/LICENSE` & `gpt_code_search-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_code_search-0.0.2/README.md` & `gpt_code_search-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```
 
 ### Usage
 
 #### Ask a question about your codebase
 
 ```bash
-gpt-code-search query "What does this codebase do?"
+gpt-code-search query ""
 ```
 
 #### Select a model
 
 ```bash
 gpt-code-search select-model
 ```
@@ -53,16 +53,16 @@
 
 This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. This removes the need to copy and paste or send your code to another third-party. Also, it meets you where you already live, in your terminal, not a new UI or window.
 
 Examples of the types of questions you might want to ask:
 
 - 🐛 Help debugging errors and finding the relevant code and files
 - 📝 Document large files or functionalities formatted as markdown
-- 📨 Ask general questions about any part of the code
 - 🛠️ Generate new code based on existing files and conventions
+- 📨 Ask general questions about any part of the code
 
 ## Privacy
 
 Outside of the LLM, no data is sent or stored.
 
 The only data sent to LLM is the question you ask and the code snippets that is requests related to your question. All code snippets are retrieved from your local machine.
```

### Comparing `gpt_code_search-0.0.2/core/ai.py` & `gpt_code_search-0.0.3/core/ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,57 +6,47 @@
 from rich.markdown import Markdown
 
 from core.config import load_selected_model
 from core.functions import (
     MAX_DEPTH,
     enabled_functions,
     get_contents_of_file,
-    get_file_tree,
     search_codebase,
     truncate_text_to_token_limit,
 )
 
 # Reduced from 16k to 14k to allow for prompt context
 MAX_TOKENS = 14_000
 
 PROMPT = """\
 You're a incredible powered coding assistant. Your role is to help users understand and navigate their codebases,
 providing assistance across a range of tasks.
 
-## Problem
-
-You want to leverage the power of GPT-4 to search your codebase, but you don't want to manually copy and paste
-code snippets into a prompt or send your code to another third-party service.
+You have access to three primary functions:
+- `search_codebase(keywords, max_depth)`: Search the codebase for a keywords with rankings based on the file path
+and contents. Higher ranking is better. Always use this function first. If there are no hits on a query, try some
+different keywords similar to the query. (eg). use interceptor, if interceptors is not found.
 
-You help by determine the most relevant code snippets within your codebase. No copying, pasting, or sharing code
-required. It meets you where you already live: in your terminal.
 
-Use cases that you will support out of the box:
-- 📨 Asking general questions about any part of the code
-- 📝 Documenting large files or functionalities in markdown
-- 🛠️ Generating new code based on existing files and conventions
-- 🐛 Debugging errors and finding relevant code and files
+- `get_contents_of_file(path)`: Fetch the contents of a file. Based on the answer from `search_codebase`, make a
+judgement on the most relevant file and fetch the contents of that file. Read at least 5 files before answering my
+calling this function multiple times. All the files should be different each time.
 
-You have access to three primary functions:
-- `search_codebase(keywords, start_path, max_depth)`: Search the codebase for a keyword.
-- `get_file_tree(start_path, max_depth)`: Retrieve the project's file structure.
-- `get_contents_of_file(path)`: Fetch the contents of a file.
+You have a total of 10 function calls. Use them wisely.
 
 Use these tools to debug, create documentation, answer code-related queries, and generate code snippets
 in line with the project's style. You will always use these functions before answering a question, particularly
-`search_codebase`. You will not answer any questions without using these functions first.
+`search_codebase`. You will not answer any questions without using these functions first. If you cannot find a
+relevant file, say 'I don't know'. If you don't, you will be penalized.
 
-Before answering, search the codebase or file tree. Review at least five files and reference the most relevant one. You
-will not answer any questions without looking up a file first. If you cannot find a relevant file, say 'I don't know'.
-If you don't, you will be penalized. Function calls are capped at ten per session. If a 'readme.md' file exists, start
-there. Otherwise, use file names and content.
-
-Compose responses in markdown with code when necessary. Aim for thorough answers, and it's okay to say 'I don't know'.
-Your objective is to provide the most accurate and detailed answer possible, even if it results in a longer response.
-Let's start assisting with your coding tasks!
+Once you find relevant files with the file tree or search functions, always use `get_contents_of_file` to fetch the
+contents of the file and review the contents of at least three files before answering.
+
+Compose responses in markdown with code when necessary. Your objective is to provide the most accurate and detailed
+answer possible, even if it results in a longer response. Let's start assisting with your coding tasks!
 """
 
 
 def chat_completion_request(messages, functions=None):
     headers = {
         "Content-Type": "application/json",
         "Authorization": "Bearer " + openai.api_key,
@@ -97,29 +87,23 @@
 
     function_name = assistant_message["function_call"]["name"]
     try:
         function_args = json.loads(assistant_message["function_call"]["arguments"])
     except json.JSONDecodeError:
         return None
 
-    if function_name == "get_file_tree":
-        function_call = get_file_tree
-        start_path = function_args.get("start_path")
-        max_depth = function_args.get("max_depth") or MAX_DEPTH
-        function_response = function_call(start_path, int(max_depth))
-    elif function_name == "get_contents_of_file":
+    if function_name == "get_contents_of_file":
         function_call = get_contents_of_file
         file_path = function_args.get("path")
         function_response = function_call(file_path)
     elif function_name == "search_codebase":
         function_call = search_codebase
         keywords = function_args.get("keywords")
-        start_path = function_args.get("start_path") or "."
         max_depth = function_args.get("max_depth") or MAX_DEPTH
-        function_response = function_call(keywords, start_path, int(max_depth))
+        function_response = function_call(keywords, int(max_depth))
     else:
         raise ValueError(f"Function {function_name} not found.")
 
     truncated_response = truncate_text_to_token_limit(function_response, MAX_TOKENS)
 
     messages.append(
         {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gpt_code_search-0.0.2/core/config.py` & `gpt_code_search-0.0.3/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,10 +43,12 @@
 def save_config(config):
     with open(CONFIG_FILE_PATH, "w") as config_file:
         toml.dump(config, config_file)
 
 
 def update_usage_info():
     config = load_config()
+    if config.get("usage") is None:
+        config["usage"] = {"query_count": 0, "last_updated": ""}
     config["usage"]["query_count"] += 1
     config["usage"]["last_updated"] = datetime.utcnow().isoformat()
     save_config(config)
```

### Comparing `gpt_code_search-0.0.2/core/functions.py` & `gpt_code_search-0.0.3/core/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import re
-from typing import List, Union
+from typing import List, Union, Tuple
 
 import tiktoken
 
 IGNORED_FOLDERS = [
     "__pycache__",
     ".git",
     ".idea",
@@ -54,43 +54,48 @@
         if os.path.isfile(item_path):
             tree.append(item_path)
         elif os.path.isdir(item_path):
             tree += get_file_tree(item_path, max_depth, depth + 1)
     return tree
 
 
-def search_codebase(
-    keywords: List[str], start_path: str = ".", max_depth: int = 5
-) -> List[str]:
+def search_codebase(keywords: List[str], max_depth: int = 5) -> List[Tuple[str, int]]:
     """
     Search the codebase for a given list of keywords.
     :param keywords: The list of keywords to search for.
-    :param start_path: The path to the directory to start the search from.
     :param max_depth: The maximum depth of the search.
-    :return: A list of file paths that contain any of the keywords.
+    :return: A list of tuples where each tuple contains a file path and a rank.
+             Files with a keyword in the path are ranked higher than files with a keyword in the content.
     """
-    file_tree = get_file_tree(start_path, max_depth)
-    matching_files = set()
+    file_tree = get_file_tree(".", max_depth)
+    matching_files = {}
 
     for file_path in file_tree:
         try:
+            rank = 0
             with open(file_path, "r", errors="ignore") as file:
                 contents = file.read()
 
             if any(re.search(keyword, contents, re.IGNORECASE) for keyword in keywords):
-                matching_files.add(file_path)
+                rank = 1
+
+            if any(
+                re.search(keyword, file_path, re.IGNORECASE) for keyword in keywords
+            ):
+                rank = 2
+
+            if rank > 0:
+                matching_files[file_path] = rank
         except Exception:
             logging.error("Error reading file: {}".format(file_path))
 
     logging.info("Searching for keywords: {}".format(keywords))
-    logging.info(
-        "Found {} matching files in {}.".format(len(matching_files), start_path)
-    )
-    logging.info("Matching files: {}".format(matching_files))
-    return list(matching_files)
+    logging.info("Found {} matching files.".format(len(matching_files)))
+    matching_files = sorted(matching_files.items(), key=lambda x: x[1], reverse=True)
+    return matching_files
 
 
 def get_contents_of_file(file_path: str) -> str:
     """
     Get the contents of a file.
     :param file_path: The path to the file.
     :return: The contents of the file, or an empty string if the file is not found.
@@ -104,71 +109,56 @@
 
 
 def count_tokens(text: str) -> int:
     encoding = tiktoken.get_encoding("cl100k_base")
     return len(encoding.encode_ordinary(text))
 
 
-def truncate_text_to_token_limit(text: Union[str, List[str]], max_tokens: int):
+def truncate_text_to_token_limit(
+    data: Union[str, List[str], List[Tuple[str, int]]], max_tokens: int
+):
     """
-    Truncate the text (or list of strings) to fit within the maximum token limit.
-    :param text: The text or list of strings to truncate.
+    Truncate the text (or list of strings or list of tuples) to fit within the maximum token limit.
+    :param data: The text or list of strings or list of tuples to truncate.
     :param max_tokens: The maximum number of tokens.
-    :return: The truncated text or list of strings.
+    :return: The truncated text or list of strings or list of tuples.
     """
-    if isinstance(text, str):
-        chunks = text.split(" ")
-    elif isinstance(text, list):
-        chunks = text
+    if not data:
+        return []
+
+    if isinstance(data, str):
+        chunks = data.split(" ")
+    elif isinstance(data, list):
+        if data and isinstance(data[0], tuple):
+            chunks = [item[0] for item in data]
+        else:
+            chunks = data
     else:
-        raise ValueError("The input text should be a string or a list of strings.")
+        raise ValueError(
+            "The input data should be a string or a list of strings or a list of tuples."
+        )
 
     total_tokens = sum(len(chunk.split(" ")) for chunk in chunks)
 
     while total_tokens > max_tokens:
         total_tokens -= len(chunks[-1].split(" "))
         chunks = chunks[:-1]
 
-    if isinstance(text, str):
+    if isinstance(data, str):
         return " ".join(chunks)
+    elif data and isinstance(data[0], tuple):
+        ranks = [item[1] for item in data[: len(chunks)]]
+        return list(zip(chunks, ranks))
     else:
         return chunks
 
 
 def enabled_functions():
     return [
         {
-            "name": "get_file_tree",
-            "description": "Get the file tree of the project based on the current working directory. "
-            "Access the current project root, with (./)",
-            "parameters": {
-                "type": "object",
-                "properties": {
-                    "start_path": {
-                        "type": "string",
-                        "description": "The path to the directory to start the search from.",
-                        "default": ".",
-                    },
-                    "max_depth": {
-                        "type": "string",
-                        "description": "The maximum depth of the search."
-                        "Use a max of {} since the search is very slow.".format(
-                            MAX_DEPTH
-                        ),
-                    },
-                    "depth": {
-                        "type": "string",
-                        "description": "The current depth of the search.",
-                        "default": "0",
-                    },
-                },
-                "required": ["start_path", "max_depth"],
-            },
-        },
-        {
             "name": "get_contents_of_file",
             "description": "Get the contents of a file. Returns empty string if the file is not found.",
             "parameters": {
                 "type": "object",
                 "properties": {
                     "path": {
                         "type": "string",
@@ -176,31 +166,45 @@
                     },
                 },
                 "required": ["path"],
             },
         },
         {
             "name": "search_codebase",
-            "description": "Search the codebase for a given list of keywords.",
+            "description": "Search the codebase for a given list of keywords and return ranked matches. Files with a "
+            "keyword in the path are ranked higher than files with a keyword in the content.",
+            "returns": {
+                "type": "array",
+                "items": {
+                    "type": "object",
+                    "properties": {
+                        "path": {
+                            "type": "string",
+                            "description": "The path to the file.",
+                        },
+                        "rank": {
+                            "type": "integer",
+                            "description": "Rank of the match. 2 if keyword found "
+                            "in file path, 1 if keyword found in file content.",
+                        },
+                    },
+                },
+                "description": "List of file paths and ranks, sorted by rank in descending order.",
+            },
             "parameters": {
                 "type": "object",
                 "properties": {
                     "keywords": {
                         "type": "array",
                         "items": {"type": "string"},
                         "description": "The list of keywords to search for. Format: ['keyword1', 'keyword2']",
                     },
-                    "start_path": {
-                        "type": "string",
-                        "description": "The path to the directory to start the search from.",
-                        "default": ".",
-                    },
                     "max_depth": {
-                        "type": "string",
+                        "type": "integer",
                         "description": "The maximum depth of the search.",
-                        "default": "5",
+                        "default": 5,
                     },
                 },
                 "required": ["keywords"],
             },
         },
     ]
```

### Comparing `gpt_code_search-0.0.2/core/main.py` & `gpt_code_search-0.0.3/core/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -61,14 +61,39 @@
         write_selected_model(selected_model_name)
     else:
         console.print("Invalid selection. Please enter a valid number.")
         typer.Exit()
 
 
 @app.command()
+def create_alias():
+    """
+    Instructions for creating an alias to gpt-code-search query.
+    """
+    console.print(
+        "To create an alias, you need to edit your shell's configuration file. "
+        "Here are instructions for Bash and Zsh (the most common shells)."
+    )
+    console.print(
+        "\nIf you use Bash, run the following command:\n"
+        "echo \"alias gq='gpt-code-search query'\" >> ~/.bashrc && source ~/.bashrc",
+        style="bold green",
+    )
+    console.print(
+        "\nIf you use Zsh, run the following command:\n"
+        "echo \"alias gq='gpt-code-search query'\" >> ~/.zshrc && source ~/.zshrc",
+        style="bold green",
+    )
+    console.print(
+        "\nAfter running the appropriate command, you can use 'gq' as a shortcut for 'gpt-code-search query'."
+    )
+    typer.Exit()
+
+
+@app.command()
 def query(message: str):
     """
     Query the current directory with any questions.
     """
     if not check_openai_key():
         return
```

### Comparing `gpt_code_search-0.0.2/pyproject.toml` & `gpt_code_search-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-code-search"
-version = "0.0.2"
+version = "0.0.3"
 description = "gpt-code-search enables you to search your codebase with natural language."
 authors = ["narenmanoharan <narenkmanoharan@gmail.com>", "skovy <smiskoviak@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "core"}]
 homepage = "https://wolfia.com"
 repository = "https://github.com/wolfia-app/gpt-code-search"
```

### Comparing `gpt_code_search-0.0.2/PKG-INFO` & `gpt_code_search-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-search
-Version: 0.0.2
+Version: 0.0.3
 Summary: gpt-code-search enables you to search your codebase with natural language.
 Home-page: https://wolfia.com
 License: Apache-2.0
 Keywords: gpt,code,search,wolfia,gpt4,llm
 Author: narenmanoharan
 Author-email: narenkmanoharan@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -54,15 +54,15 @@
 ```
 
 ### Usage
 
 #### Ask a question about your codebase
 
 ```bash
-gpt-code-search query "What does this codebase do?"
+gpt-code-search query ""
 ```
 
 #### Select a model
 
 ```bash
 gpt-code-search select-model
 ```
@@ -80,16 +80,16 @@
 
 This tool solves these problems by letting GPT-4 determine the most relevant code snippets within your codebase. This removes the need to copy and paste or send your code to another third-party. Also, it meets you where you already live, in your terminal, not a new UI or window.
 
 Examples of the types of questions you might want to ask:
 
 - 🐛 Help debugging errors and finding the relevant code and files
 - 📝 Document large files or functionalities formatted as markdown
-- 📨 Ask general questions about any part of the code
 - 🛠️ Generate new code based on existing files and conventions
+- 📨 Ask general questions about any part of the code
 
 ## Privacy
 
 Outside of the LLM, no data is sent or stored.
 
 The only data sent to LLM is the question you ask and the code snippets that is requests related to your question. All code snippets are retrieved from your local machine.
```

