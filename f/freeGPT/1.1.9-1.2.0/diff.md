# Comparing `tmp/freeGPT-1.1.9.tar.gz` & `tmp/freeGPT-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeGPT-1.1.9.tar", last modified: Sat Jun 17 19:34:37 2023, max compression
+gzip compressed data, was "freeGPT-1.2.0.tar", last modified: Sun Jun 25 19:20:57 2023, max compression
```

## Comparing `freeGPT-1.1.9.tar` & `freeGPT-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.527489 freeGPT-1.1.9/
--rw-rw-rw-   0        0        0    35149 2023-06-17 19:31:12.000000 freeGPT-1.1.9/LICENSE
--rw-rw-rw-   0        0        0       96 2023-06-17 19:31:12.000000 freeGPT-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4247 2023-06-17 19:34:37.526492 freeGPT-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3110 2023-06-17 19:31:12.000000 freeGPT-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.372011 freeGPT-1.1.9/freeGPT/
--rw-rw-rw-   0        0        0     2319 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.517521 freeGPT-1.1.9/freeGPT/alpaca_7b/
--rw-rw-rw-   0        0        0     1590 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/alpaca_7b/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.521509 freeGPT-1.1.9/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     5094 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.523502 freeGPT-1.1.9/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2467 2023-06-17 19:31:12.000000 freeGPT-1.1.9/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:34:37.509559 freeGPT-1.1.9/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     4247 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-17 19:34:37.000000 freeGPT-1.1.9/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 19:34:37.528485 freeGPT-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1533 2023-06-17 19:31:12.000000 freeGPT-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:20:57.043224 freeGPT-1.2.0/
+-rw-rw-rw-   0        0        0    35149 2023-06-25 19:15:08.000000 freeGPT-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       96 2023-06-25 19:15:08.000000 freeGPT-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4501 2023-06-25 19:20:57.039200 freeGPT-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3326 2023-06-25 19:15:08.000000 freeGPT-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 19:20:56.997200 freeGPT-1.2.0/freeGPT/
+-rw-rw-rw-   0        0        0      134 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/__init__.py
+-rw-rw-rw-   0        0        0     1632 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/alpaca_7b.py
+-rw-rw-rw-   0        0        0     4725 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/c_a_l.py
+-rw-rw-rw-   0        0        0     1220 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/gpt3.py
+-rw-rw-rw-   0        0        0     2655 2023-06-25 19:15:08.000000 freeGPT-1.2.0/freeGPT/gpt4.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:20:57.037205 freeGPT-1.2.0/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     4501 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 19:20:56.000000 freeGPT-1.2.0/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 19:20:57.044215 freeGPT-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1577 2023-06-25 19:15:08.000000 freeGPT-1.2.0/setup.py
```

### Comparing `freeGPT-1.1.9/LICENSE` & `freeGPT-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.1.9/PKG-INFO` & `freeGPT-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.9
-Summary: freeGPT is a Python package that gives access to GPT and more models for free.
+Version: 1.2.0
+Summary: freeGPT provides access to GPT and other models for free.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discord, https://dsc.gg/ruu3fstudio
-Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,model,free,gpt3,gpt4,gpt,py,ai
+Keywords: artificial-intelligence,machine-learning,ai-models,chatbot,gpt4free,freegpt,chatgpt,python,alpaca,openai,model,c-a-l,free,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 <br>
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
-***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
+***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)***
+<br>
+Join my [Discord Server](https://discord.gg/XH6pUGkwRr) for live chat and support or if you have any issues with this package.
 
 ## Source:
 *GPT-3 has internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
 | gpt3              | [you.com](https://you.com/)                          |
@@ -48,25 +51,26 @@
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
 - [ ] Add a image generation model.
 
-## Support me:
+## Support this repository:
 - Star this repository! :D
-- Join my [Discord Server](https://discord.gg/NcQ26PrNDp):
+- Add the [Discord Bot](https://dsc.gg/freeGPT) :D
+- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
-[![DiscordWidget](https://discordapp.com/api/guilds/1084505055476056184/widget.png?style=banner2)](https://discord.gg/NcQ26PrNDp)
+[![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## Discord bot:
 - Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
 - This bot has ALL the models in this repository available.
 - Its interactive, fast and overall easy to use.
-- And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
+- And lastly its [Open Sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!
 
 ## Examples:
 
 #### GPT-3:
 ```python
 from freeGPT import gpt3
```

### Comparing `freeGPT-1.1.9/README.md` & `freeGPT-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # freeGPT
 freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 <br>
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
-***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
+***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)***
+<br>
+Join my [Discord Server](https://discord.gg/XH6pUGkwRr) for live chat and support or if you have any issues with this package.
 
 ## Source:
 *GPT-3 has internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
 | gpt3              | [you.com](https://you.com/)                          |
@@ -25,25 +27,26 @@
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
 - [ ] Add a image generation model.
 
-## Support me:
+## Support this repository:
 - Star this repository! :D
-- Join my [Discord Server](https://discord.gg/NcQ26PrNDp):
+- Add the [Discord Bot](https://dsc.gg/freeGPT) :D
+- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
-[![DiscordWidget](https://discordapp.com/api/guilds/1084505055476056184/widget.png?style=banner2)](https://discord.gg/NcQ26PrNDp)
+[![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## Discord bot:
 - Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
 - This bot has ALL the models in this repository available.
 - Its interactive, fast and overall easy to use.
-- And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
+- And lastly its [Open Sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!
 
 ## Examples:
 
 #### GPT-3:
 ```python
 from freeGPT import gpt3
```

### Comparing `freeGPT-1.1.9/freeGPT/alpaca_7b/__init__.py` & `freeGPT-1.2.0/freeGPT/alpaca_7b.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import requests
+from fake_useragent import UserAgent
 
 
 class Completion:
     @staticmethod
-    def create(prompt: str):
+    def create(prompt):
         """
-        Creates a completion by sending a POST request to a remote server.
+        Create a completion using a given prompt.
 
         Args:
-            prompt (str): The prompt string to be sent for completion.
+            prompt (str): The prompt for generating the completion.
 
         Returns:
-            str: The completion generated by the server.
+            str: The generated completion.
 
         Raises:
-            Exception: If unable to fetch the response from the server.
+            Exception: If there is an error while fetching the response.
+
         """
-        headers = {
-            "Origin": "https://chatllama.baseten.co",
-            "Referer": "https://chatllama.baseten.co/",
-            "Accept": "application/json, text/plain, */*",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Accept-Language": "en-US,en;q=0.9",
-            "Content-Length": "17",
-            "Content-Type": "application/json",
-            "Sec-Ch-Ua": '"Google Chrome";v="89", "Chromium";v="89", ";Not A Brand";v="99"',
-            "Sec-Ch-Ua-Mobile": "?0",
-            "Sec-Ch-Ua-Platform": "Windows",
-            "Sec-Fetch-Dest": "empty",
-            "Sec-Fetch-Mode": "cors",
-            "Sec-Fetch-Site": "cross-site",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36",
-        }
         try:
             resp = requests.post(
                 "https://us-central1-arched-keyword-306918.cloudfunctions.net/run-inference-1",
-                headers=headers,
+                headers={
+                    "Origin": "https://chatllama.baseten.co",
+                    "Referer": "https://chatllama.baseten.co/",
+                    "Accept": "application/json, text/plain, */*",
+                    "Accept-Encoding": "gzip, deflate, br",
+                    "Accept-Language": "en-US,en;q=0.9",
+                    "Content-Length": "17",
+                    "Content-Type": "application/json",
+                    "Sec-Ch-Ua": '"Google Chrome";v="89", "Chromium";v="89", ";Not A Brand";v="99"',
+                    "Sec-Ch-Ua-Mobile": "?0",
+                    "Sec-Ch-Ua-Platform": "Windows",
+                    "Sec-Fetch-Dest": "empty",
+                    "Sec-Fetch-Mode": "cors",
+                    "Sec-Fetch-Site": "cross-site",
+                    "User-Agent": UserAgent().random,
+                },
                 json={"prompt": prompt},
             ).json()
         except requests.exceptions.RequestException:
             raise Exception("Unable to fetch the response.")
 
         return resp["completion"]
```

### Comparing `freeGPT-1.1.9/freeGPT/gpt3/__init__.py` & `freeGPT-1.2.0/freeGPT/c_a_l.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 import re, json
 import subprocess
 from uuid import uuid4
-from fake_useragent import UserAgent
 from typing import Optional, List
+from fake_useragent import UserAgent
 
 
 class Completion:
-    """A class that provides methods for creating completion requests."""
-
     @staticmethod
     def create(
-        prompt: str,
+        prompt,
         page: int = 1,
         count: int = 10,
         safe_search: str = "Off",
         on_shopping_page: bool = False,
         mkt: str = "",
         response_filter: str = "WebPages, Translations, Computation, RelatedSearches",
         domain: str = "youchat",
         query_trace_id: Optional[str] = None,
         chat: Optional[List[str]] = None,
         include_links: bool = False,
         detailed: bool = False,
         proxies: Optional[str] = None,
     ) -> dict:
         """
-        Creates a completion request.
+        Create a completion.
 
         Args:
-            prompt (str): The prompt text for the completion.
-            page (int, optional): The page number for pagination. Defaults to 1.
-            count (int, optional): The number of results per page. Defaults to 10.
-            safe_search (str, optional): The safe search level. Defaults to 'Off'.
-            on_shopping_page (bool, optional): Indicates if the completion is on a shopping page. Defaults to False.
-            mkt (str, optional): The market for the completion. Defaults to ''.
-            response_filter (str, optional): The filter for the response. Defaults to 'WebPages,Translations,TimeZone,Computation,RelatedSearches'.
-            domain (str, optional): The domain for the completion. Defaults to 'youchat'.
-            query_trace_id (str, optional): The trace ID for the query. Defaults to None.
-            chat (list, optional): A list of chat messages. Defaults to None.
-            include_links (bool, optional): Indicates if links should be included in the response. Defaults to False.
-            detailed (bool, optional): Indicates if detailed results should be included in the response. Defaults to False.
-            proxies (str, optional): The proxy server to use. Defaults to None.
+            prompt (str): The prompt for the completion.
+            page (int): The page number for the search results. Default is 1.
+            count (int): The number of results to return. Default is 10.
+            safe_search (str): The safe search setting. Default is "Off".
+            on_shopping_page (bool): Whether the search is on a shopping page. Default is False.
+            mkt (str): The market code for the search. Default is an empty string.
+            response_filter (str): The response filter for the search. Default is "WebPages, Translations, Computation, RelatedSearches".
+            domain (str): The domain for the search. Default is "youchat".
+            query_trace_id (str, optional): The query trace ID. If not provided, a new UUID will be generated. Default is None.
+            chat (List[str], optional): A list of chat messages. Default is None.
+            include_links (bool): Whether to include third-party search links in the results. Default is False.
+            detailed (bool): Whether to include detailed information in the results. Default is False.
+            proxies (str, optional): Proxies to use for the request. Default is None.
 
         Returns:
-            dict: The completion response as a dictionary.
+            dict: The completion result as a dictionary.
 
         Raises:
-            Exception: If unable to get the response.
+            Exception: If unable to fetch the response.
         """
+
         if chat is None:
             chat = []
 
         try:
             import tls_client
         except ImportError:
             subprocess.run(["pip", "install", "tls_client", "--no-cache-dir"])
             import tls_client
 
         client = tls_client.Session(client_identifier="chrome_108")
-        client.headers = Completion.__get_headers()
+        client.headers = {
+            "authority": "you.com",
+            "accept": "text/event-stream",
+            "accept-language": "en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3",
+            "cache-control": "no-cache",
+            "referer": "https://you.com/search?q=hi&tbm=youchat",
+            "sec-ch-ua": '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": "Linux",
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "cookie": f"safesearch_guest=Off; uuid_guest={str(uuid4())}",
+            "user-agent": UserAgent().random,
+        }
         client.proxies = proxies
 
         response = client.get(
             "https://you.com/api/streamingSearch",
             params={
                 "q": prompt,
                 "page": page,
@@ -104,32 +117,8 @@
             result["links"] = json.loads(third_party_search_results)["search"][
                 "third_party_search_results"
             ]
 
         if detailed:
             result["extra"] = extra
 
-        return result
-
-    @staticmethod
-    def __get_headers() -> dict:
-        """
-        Returns the headers for the completion request.
-
-        Returns:
-            dict: The headers as a dictionary.
-        """
-        return {
-            "authority": "you.com",
-            "accept": "text/event-stream",
-            "accept-language": "en,fr-FR;q=0.9,fr;q=0.8,es-ES;q=0.7,es;q=0.6,en-US;q=0.5,am;q=0.4,de;q=0.3",
-            "cache-control": "no-cache",
-            "referer": "https://you.com/search?q=hi&tbm=youchat",
-            "sec-ch-ua": '"Not_A Brand";v="99", "Google Chrome";v="109", "Chromium";v="109"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Linux"',
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "cookie": f"safesearch_guest=Off; uuid_guest={str(uuid4())}",
-            "user-agent": UserAgent().random,
-        }
+        return result["text"]
```

### Comparing `freeGPT-1.1.9/freeGPT/gpt4/__init__.py` & `freeGPT-1.2.0/freeGPT/gpt4.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-import json, requests
+import json
+import requests
 
 
 class Completion:
+    """
+    A class that interacts with the Ava API to generate completions for prompts.
+    """
+
     @staticmethod
     def create(prompt):
         """
-        Creates a completion for the given prompt using the GPT-4 model.
+        Generates a completion based on the given prompt.
 
         Args:
-            prompt (str): The user prompt for generating the completion.
+            prompt (str): The prompt text to generate a completion for.
 
         Returns:
-            str: The generated completion text.
+            str: The generated completion response.
 
         Raises:
-            Exception: If there is an error while fetching the response.
+            Exception: If there is an error while fetching the response from the API.
         """
-
-        headers = {"Content-Type": "application/json"}
-        payload = {
-            "model": "gpt-4",
-            "temperature": 0.5,
-            "stream": True,
-            "messages": [
-                {
-                    "role": "system",
-                    "content": "You are freeGPT, an AI assistant provided by Ruu3f (an individual). Your model is GPT-4 by OpenAI.",
-                },
-                {"role": "user", "content": prompt},
-            ],
-        }
-
         try:
             resp = ""
             with requests.post(
                 "https://ava-alpha-api.codelink.io/api/chat",
-                headers=headers,
-                data=json.dumps(payload),
+                headers={"Content-Type": "application/json"},
+                data=json.dumps(
+                    {
+                        "model": "gpt-4",
+                        "temperature": 0.7,
+                        "stream": True,
+                        "messages": [
+                            {
+                                "role": "system",
+                                "content": "You are Ava, an AI assistant. You are running on GPT-4 by OpenAI.",
+                            },
+                            {"role": "user", "content": prompt},
+                        ],
+                    }
+                ),
                 stream=True,
             ) as resp_obj:
                 resp_obj.raise_for_status()
                 for line in resp_obj.iter_lines():
                     line_text = line.decode("utf-8").strip()
                     if line_text.startswith("data:"):
                         data = line_text[len("data:") :]
```

### Comparing `freeGPT-1.1.9/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.2.0/freeGPT.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.1.9
-Summary: freeGPT is a Python package that gives access to GPT and more models for free.
+Version: 1.2.0
+Summary: freeGPT provides access to GPT and other models for free.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Project-URL: Discord, https://dsc.gg/ruu3fstudio
-Keywords: artificial-intelligence,machine-learning,ai-models,chatllama,gpt4free,freegpt,chatgpt,python,alpaca,openai,model,free,gpt3,gpt4,gpt,py,ai
+Keywords: artificial-intelligence,machine-learning,ai-models,chatbot,gpt4free,freegpt,chatgpt,python,alpaca,openai,model,c-a-l,free,gpt3,gpt4,gpt,py,ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
 [![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 freeGPT is a Python package that gives free access to GPT3 and GPT4 and more models.
 <br>
 Get started by installing the package:
 ```
 py -m pip install --upgrade freeGPT
 ```
-***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)***
+***Or add our [Discord bot](https://dsc.gg/freegpt), its [Open Sourced!](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)***
+<br>
+Join my [Discord Server](https://discord.gg/XH6pUGkwRr) for live chat and support or if you have any issues with this package.
 
 ## Source:
 *GPT-3 has internet access.*
 <br>
 | Models            | Websites                                             |
 | ----------------- | -----------------------------------------------------|
 | gpt3              | [you.com](https://you.com/)                          |
@@ -48,25 +51,26 @@
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Make GPT-3 & GPT-4 models with web access.
 - [x] Add a non-GPT model.
 - [x] Make a discord bot.
 - [ ] Add a image generation model.
 
-## Support me:
+## Support this repository:
 - Star this repository! :D
-- Join my [Discord Server](https://discord.gg/NcQ26PrNDp):
+- Add the [Discord Bot](https://dsc.gg/freeGPT) :D
+- Join my [Discord Server](https://discord.gg/XH6pUGkwRr):
 
-[![DiscordWidget](https://discordapp.com/api/guilds/1084505055476056184/widget.png?style=banner2)](https://discord.gg/NcQ26PrNDp)
+[![DiscordWidget](https://discordapp.com/api/guilds/1120833966035976273/widget.png?style=banner2)](https://discord.gg/XH6pUGkwRr)
 
 ## Discord bot:
 - Add the official freeGPT discord bot [here](https://dsc.gg/freegpt)
 - This bot has ALL the models in this repository available.
 - Its interactive, fast and overall easy to use.
-- And lastly its [Open Sourced!](https://github.com/Ruu3f/freeGPT-discord-bot)
+- And lastly its [Open Sourced](https://github.com/Ruu3f/freeGPT/tree/main/discord-bot)!
 
 ## Examples:
 
 #### GPT-3:
 ```python
 from freeGPT import gpt3
```

### Comparing `freeGPT-1.1.9/setup.py` & `freeGPT-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.1.9",
-    description="freeGPT is a Python package that gives access to GPT and more models for free.",
+    version="1.2.0",
+    description="freeGPT provides access to GPT and other models for free.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
         "artificial-intelligence",
         "machine-learning",
         "ai-models",
-        "chatllama",
+        "chatbot",
         "gpt4free",
         "freegpt",
         "chatgpt",
         "python",
         "alpaca",
         "openai",
         "model",
+        "c-a-l",
         "free",
         "gpt3",
         "gpt4",
         "gpt",
         "py",
         "ai",
     ],
@@ -37,14 +38,15 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=find_packages(),
     install_requires=[
         "requests",
         "fake-useragent",
     ],
     project_urls={
```

