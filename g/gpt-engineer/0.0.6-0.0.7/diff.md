# Comparing `tmp/gpt-engineer-0.0.6.tar.gz` & `tmp/gpt-engineer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-engineer-0.0.6.tar", last modified: Thu Jun 22 09:31:36 2023, max compression
+gzip compressed data, was "gpt-engineer-0.0.7.tar", last modified: Sun Jun 25 13:56:49 2023, max compression
```

## Comparing `gpt-engineer-0.0.6.tar` & `gpt-engineer-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.446110 gpt-engineer-0.0.6/gpt_engineer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/gpt_engineer/preprompts/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/fix_code
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/generate
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/philosophy
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/qa
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/respec
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/spec
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/unit_tests
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/use_feedback
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/use_qa
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/gpt_engineer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/tests/test_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/tests/test_chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:49.472354 gpt-engineer-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-25 13:56:49.472354 gpt-engineer-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:49.468354 gpt-engineer-0.0.7/gpt_engineer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:49.472354 gpt-engineer-0.0.7/gpt_engineer/preprompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/fix_code
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/generate
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/philosophy
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/qa
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/respec
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/spec
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/unit_tests
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/use_feedback
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/preprompts/use_qa
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/gpt_engineer/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:49.468354 gpt-engineer-0.0.7/gpt_engineer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-25 13:56:49.000000 gpt-engineer-0.0.7/gpt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 13:56:49.000000 gpt-engineer-0.0.7/gpt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 13:56:49.000000 gpt-engineer-0.0.7/gpt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-25 13:56:49.000000 gpt-engineer-0.0.7/gpt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-25 13:56:49.000000 gpt-engineer-0.0.7/gpt_engineer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 13:56:49.000000 gpt-engineer-0.0.7/gpt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:56:49.472354 gpt-engineer-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:56:49.472354 gpt-engineer-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/tests/test_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/tests/test_chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/tests/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-25 13:56:39.000000 gpt-engineer-0.0.7/tests/test_db.py
```

### Comparing `gpt-engineer-0.0.6/LICENSE` & `gpt-engineer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.6/PKG-INFO` & `gpt-engineer-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,93 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPT Engineer
+
 [![Discord Follow](https://dcbadge.vercel.app/api/server/4t5vXHhu?style=flat)](https://discord.gg/4t5vXHhu)
 [![GitHub Repo stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer?style=social)](https://github.com/AntonOsika/gpt-engineer)
 [![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/AntonOsika)
 
 
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
 ## Project philosophy
+
 - Simple to get value
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-## Setup
+## Usage
+
+Choose either **stable** or **development**.
+
+For **stable** release:
+
+- `pip install gpt-engineer`
+
+For **development**:
 - `git clone git@github.com:AntonOsika/gpt-engineer.git`
 - `cd gpt-engineer`
 - `pip install -e .`
   - (or: `make install && source venv/bin/activate` for a venv)
 
+**Setup**
+
 With an api key that has GPT4 access run:
 
 - `export OPENAI_API_KEY=[your api key]`
 
 
 **Run**:
+
 - Create an empty folder. If inside the repo, you can run:
   - `cp -r projects/example/ projects/my-new-project`
-- Fill in the `main_prompt` file in your new folder
-- Run: `gpt-engineer projects/my-new-project`
+- Fill in the `prompt` file in your new folder
+- `gpt-engineer projects/my-new-project`
+  - (Note, `gpt-engineer --help` lets you see all available options. For example `--steps use_feedback` lets you improve/fix code in a project)
+
+By running gpt-engineer you agree to our [ToS](https://github.com/AntonOsika/gpt-engineer/TERMS_OF_USE.md).
 
 **Results**
 - Check the generated files in `projects/my-new-project/workspace`
 
 
 ## Features
-You can specify the "identity" of the AI agent by editing the files in the `identity` folder.
 
-Editing the identity, and evolving the `main_prompt`, is currently how you make the agent remember things between projects.
+You can specify the "identity" of the AI agent by editing the files in the `preprompts` folder.
+
+Editing the `preprompts`, and evolving how you write the project prompt, is currently how you make the agent remember things between projects.
 
 Each step in `steps.py` will have its communication history with GPT4 stored in the logs folder, and can be rerun with `scripts/rerun_edited_message_logs.py`.
 
 ## Contributing
-We are building the open platform for devs to tinker with and build their personal code-generation toolbox.
+The gpt-engineer community is building the **open platform for devs to tinker with and build their personal code-generation toolbox**.
+
+If you are interested in contributing to this, we would be interested in having you!
 
-If you want to contribute, please check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo. You are welcome to read the [contributing document](.github/CONTRIBUTING.md) and join our [Discord 💬](https://discord.gg/4t5vXHhu).
+You can check for good first issues [here](https://github.com/AntonOsika/gpt-engineer/issues).
+Contributing document [here](.github/CONTRIBUTING.md).
 
 We are currently looking for more maintainers and community organisers. Email anton.osika@gmail.com if you are interested in an official role.
 
+If you want to see our broader ambitions, check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), and join
+[discord ](https://discord.gg/4t5vXHhu)
+to get input on how you can contribute to it.
 
 ## Example
 
 https://github.com/AntonOsika/gpt-engineer/assets/4467025/6e362e45-4a94-4b0d-973d-393a31d92d9b
```

### Comparing `gpt-engineer-0.0.6/README.md` & `gpt-engineer-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,83 @@
 # GPT Engineer
+
 [![Discord Follow](https://dcbadge.vercel.app/api/server/4t5vXHhu?style=flat)](https://discord.gg/4t5vXHhu)
 [![GitHub Repo stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer?style=social)](https://github.com/AntonOsika/gpt-engineer)
 [![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/AntonOsika)
 
 
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
 ## Project philosophy
+
 - Simple to get value
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-## Setup
+## Usage
+
+Choose either **stable** or **development**.
+
+For **stable** release:
+
+- `pip install gpt-engineer`
+
+For **development**:
 - `git clone git@github.com:AntonOsika/gpt-engineer.git`
 - `cd gpt-engineer`
 - `pip install -e .`
   - (or: `make install && source venv/bin/activate` for a venv)
 
+**Setup**
+
 With an api key that has GPT4 access run:
 
 - `export OPENAI_API_KEY=[your api key]`
 
 
 **Run**:
+
 - Create an empty folder. If inside the repo, you can run:
   - `cp -r projects/example/ projects/my-new-project`
-- Fill in the `main_prompt` file in your new folder
-- Run: `gpt-engineer projects/my-new-project`
+- Fill in the `prompt` file in your new folder
+- `gpt-engineer projects/my-new-project`
+  - (Note, `gpt-engineer --help` lets you see all available options. For example `--steps use_feedback` lets you improve/fix code in a project)
+
+By running gpt-engineer you agree to our [ToS](https://github.com/AntonOsika/gpt-engineer/TERMS_OF_USE.md).
 
 **Results**
 - Check the generated files in `projects/my-new-project/workspace`
 
 
 ## Features
-You can specify the "identity" of the AI agent by editing the files in the `identity` folder.
 
-Editing the identity, and evolving the `main_prompt`, is currently how you make the agent remember things between projects.
+You can specify the "identity" of the AI agent by editing the files in the `preprompts` folder.
+
+Editing the `preprompts`, and evolving how you write the project prompt, is currently how you make the agent remember things between projects.
 
 Each step in `steps.py` will have its communication history with GPT4 stored in the logs folder, and can be rerun with `scripts/rerun_edited_message_logs.py`.
 
 ## Contributing
-We are building the open platform for devs to tinker with and build their personal code-generation toolbox.
+The gpt-engineer community is building the **open platform for devs to tinker with and build their personal code-generation toolbox**.
+
+If you are interested in contributing to this, we would be interested in having you!
 
-If you want to contribute, please check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo. You are welcome to read the [contributing document](.github/CONTRIBUTING.md) and join our [Discord 💬](https://discord.gg/4t5vXHhu).
+You can check for good first issues [here](https://github.com/AntonOsika/gpt-engineer/issues).
+Contributing document [here](.github/CONTRIBUTING.md).
 
 We are currently looking for more maintainers and community organisers. Email anton.osika@gmail.com if you are interested in an official role.
 
+If you want to see our broader ambitions, check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), and join
+[discord ](https://discord.gg/4t5vXHhu)
+to get input on how you can contribute to it.
 
 ## Example
 
 https://github.com/AntonOsika/gpt-engineer/assets/4467025/6e362e45-4a94-4b0d-973d-393a31d92d9b
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer/ai.py` & `gpt-engineer-0.0.7/gpt_engineer/ai.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class AI:
     def __init__(self, model="gpt-4", temperature=0.1):
         self.temperature = temperature
-
-        try:
-            openai.Model.retrieve(model)
-            self.model = model
-        except openai.InvalidRequestError:
-            print(
-                f"Model {model} not available for provided API key. Reverting "
-                "to gpt-3.5-turbo. Sign up for the GPT-4 wait list here: "
-                "https://openai.com/waitlist/gpt-4-api"
-            )
-            self.model = "gpt-3.5-turbo"
+        self.model = model
 
     def start(self, system, user):
         messages = [
             {"role": "system", "content": system},
             {"role": "user", "content": user},
         ]
 
@@ -57,7 +47,20 @@
             msg = delta.get("content", "")
             print(msg, end="")
             chat.append(msg)
         print()
         messages += [{"role": "assistant", "content": "".join(chat)}]
         logger.debug(f"Chat completion finished: {messages}")
         return messages
+
+
+def fallback_model(model: str) -> str:
+    try:
+        openai.Model.retrieve(model)
+        return model
+    except openai.InvalidRequestError:
+        print(
+            f"Model {model} not available for provided API key. Reverting "
+            "to gpt-3.5-turbo. Sign up for the GPT-4 wait list here: "
+            "https://openai.com/waitlist/gpt-4-api\n"
+        )
+        return "gpt-3.5-turbo"
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer/chat_to_files.py` & `gpt-engineer-0.0.7/gpt_engineer/chat_to_files.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.6/gpt_engineer/db.py` & `gpt-engineer-0.0.7/gpt_engineer/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,20 @@
         full_path = self.path / key
 
         if not full_path.is_file():
             raise KeyError(key)
         with full_path.open("r", encoding="utf-8") as f:
             return f.read()
 
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except KeyError:
+            return default
+
     def __setitem__(self, key, val):
         full_path = self.path / key
         full_path.parent.mkdir(parents=True, exist_ok=True)
 
         if isinstance(val, str):
             full_path.write_text(val, encoding="utf-8")
         else:
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer/preprompts/generate` & `gpt-engineer-0.0.7/gpt_engineer/preprompts/generate`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.6/gpt_engineer/preprompts/philosophy` & `gpt-engineer-0.0.7/gpt_engineer/preprompts/philosophy`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.6/gpt_engineer/preprompts/respec` & `gpt-engineer-0.0.7/gpt_engineer/preprompts/respec`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 - Is there anything that might not work the way intended by the instructions?
 - Is there anything in the specification missing for the program to work as expected?
 - Is there anything that can be simplified without significant drawback?
 
 You are asked to make educated assumptions for each unclear item.
 For each of these, communicate which assumptions you'll make when implementing the feature.
 
-Think step by step to make sure we don't miss anything.
+Think step by step to make sure we don't miss anything.
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer/preprompts/spec` & `gpt-engineer-0.0.7/gpt_engineer/preprompts/spec`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 Think step by step to make sure we get a high quality specification and we don't miss anything.
 First, be super explicit about what the program should do, which features it should have
 and give details about anything that might be unclear. **Don't leave anything unclear or undefined.**
 
 Second, lay out the names of the core classes, functions, methods that will be necessary,
 as well as a quick comment on their purpose.
 
-This specification will be used later as the basis for the implementation.
+This specification will be used later as the basis for the implementation.
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer/preprompts/use_qa` & `gpt-engineer-0.0.7/gpt_engineer/preprompts/use_qa`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.6/gpt_engineer/steps.py` & `gpt-engineer-0.0.7/gpt_engineer/steps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,114 @@
 import json
 import re
 import subprocess
 
 from enum import Enum
-from typing import Callable, TypeVar
+from typing import List
+
+from termcolor import colored
 
 from gpt_engineer.ai import AI
 from gpt_engineer.chat_to_files import to_files
 from gpt_engineer.db import DBs
+from gpt_engineer.learning import human_input
 
 
-def setup_sys_prompt(dbs):
+def setup_sys_prompt(dbs: DBs) -> str:
     return (
         dbs.preprompts["generate"] + "\nUseful to know:\n" + dbs.preprompts["philosophy"]
     )
 
 
-Step = TypeVar("Step", bound=Callable[[AI, DBs], list[dict]])
+def get_prompt(dbs: DBs) -> str:
+    """While we migrate we have this fallback getter"""
+    assert (
+        "prompt" in dbs.input or "main_prompt" in dbs.input
+    ), "Please put your prompt in the file `prompt` in the project directory"
+
+    if "prompt" not in dbs.input:
+        print(
+            colored("Please put the prompt in the file `prompt`, not `main_prompt", "red")
+        )
+        print()
+        return dbs.input["main_prompt"]
+
+    return dbs.input["prompt"]
+
+
+# All steps below have the signature Step
 
 
-def simple_gen(ai: AI, dbs: DBs):
+def simple_gen(ai: AI, dbs: DBs) -> List[dict]:
     """Run the AI on the main prompt and save the results"""
-    messages = ai.start(
-        setup_sys_prompt(dbs),
-        dbs.input["main_prompt"],
-    )
+    messages = ai.start(setup_sys_prompt(dbs), get_prompt(dbs))
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
-def clarify(ai: AI, dbs: DBs):
+def clarify(ai: AI, dbs: DBs) -> List[dict]:
     """
     Ask the user if they want to clarify anything and save the results to the workspace
     """
     messages = [ai.fsystem(dbs.preprompts["qa"])]
-    user = dbs.input["main_prompt"]
+    user_input = get_prompt(dbs)
     while True:
-        messages = ai.next(messages, user)
+        messages = ai.next(messages, user_input)
+
+        if messages[-1]["content"].strip() == "Nothing more to clarify.":
+            break
 
         if messages[-1]["content"].strip().lower().startswith("no"):
+            print("Nothing more to clarify.")
             break
 
         print()
-        user = input('(answer in text, or "c" to move on)\n')
+        user_input = input('(answer in text, or "c" to move on)\n')
         print()
 
-        if not user or user == "c":
-            break
+        if not user_input or user_input == "c":
+            print("(letting gpt-engineer make its own assumptions)")
+            print()
+            messages = ai.next(
+                messages,
+                "Make your own assumptions and state them explicitly before starting",
+            )
+            print()
+            return messages
 
-        user += (
+        user_input += (
             "\n\n"
             "Is anything else unclear? If yes, only answer in the form:\n"
             "{remaining unclear areas} remaining questions.\n"
             "{Next question}\n"
-            'If everything is sufficiently clear, only answer "no".'
+            'If everything is sufficiently clear, only answer "Nothing more to clarify.".'
         )
 
     print()
     return messages
 
 
-def gen_spec(ai: AI, dbs: DBs):
+def gen_spec(ai: AI, dbs: DBs) -> List[dict]:
     """
     Generate a spec from the main prompt + clarifications and save the results to
     the workspace
     """
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
-        ai.fsystem(f"Instructions: {dbs.input['main_prompt']}"),
+        ai.fsystem(f"Instructions: {dbs.input['prompt']}"),
     ]
 
     messages = ai.next(messages, dbs.preprompts["spec"])
 
     dbs.memory["specification"] = messages[-1]["content"]
 
     return messages
 
 
-def respec(ai: AI, dbs: DBs):
+def respec(ai: AI, dbs: DBs) -> List[dict]:
     messages = json.loads(dbs.logs[gen_spec.__name__])
     messages += [ai.fsystem(dbs.preprompts["respec"])]
 
     messages = ai.next(messages)
     messages = ai.next(
         messages,
         (
@@ -94,93 +121,107 @@
         ),
     )
 
     dbs.memory["specification"] = messages[-1]["content"]
     return messages
 
 
-def gen_unit_tests(ai: AI, dbs: DBs):
+def gen_unit_tests(ai: AI, dbs: DBs) -> List[dict]:
     """
     Generate unit tests based on the specification, that should work.
     """
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
-        ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
+        ai.fuser(f"Instructions: {dbs.input['prompt']}"),
         ai.fuser(f"Specification:\n\n{dbs.memory['specification']}"),
     ]
 
     messages = ai.next(messages, dbs.preprompts["unit_tests"])
 
     dbs.memory["unit_tests"] = messages[-1]["content"]
     to_files(dbs.memory["unit_tests"], dbs.workspace)
 
     return messages
 
 
-def gen_clarified_code(ai: AI, dbs: DBs):
-    # get the messages from previous step
+def gen_clarified_code(ai: AI, dbs: DBs) -> List[dict]:
+    """Takes clarification and generates code"""
 
     messages = json.loads(dbs.logs[clarify.__name__])
 
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
     ] + messages[1:]
     messages = ai.next(messages, dbs.preprompts["use_qa"])
 
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
-def gen_code(ai: AI, dbs: DBs):
+def gen_code(ai: AI, dbs: DBs) -> List[dict]:
     # get the messages from previous step
 
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
-        ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
+        ai.fuser(f"Instructions: {dbs.input['prompt']}"),
         ai.fuser(f"Specification:\n\n{dbs.memory['specification']}"),
         ai.fuser(f"Unit tests:\n\n{dbs.memory['unit_tests']}"),
     ]
     messages = ai.next(messages, dbs.preprompts["use_qa"])
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
-def execute_entrypoint(ai, dbs):
+def execute_entrypoint(ai: AI, dbs: DBs) -> List[dict]:
     command = dbs.workspace["run.sh"]
 
     print("Do you want to execute this code?")
     print()
     print(command)
     print()
     print('If yes, press enter. Otherwise, type "no"')
     print()
     if input() not in ["", "y", "yes"]:
         print("Ok, not executing the code.")
         return []
     print("Executing the code...")
+    print()
     print(
-        "\033[92m"  # green color
-        + "Note: If it does not work as expected, please consider running the code'"
-        + " in another way than above."
-        + "\033[0m"
+        colored(
+            "Note: If it does not work as expected, consider running the code"
+            + " in another way than above.",
+            "green",
+        )
     )
     print()
-    subprocess.run("bash run.sh", shell=True, cwd=dbs.workspace.path)
+    print("You can press ctrl+c *once* to stop the execution.")
+    print()
+
+    p = subprocess.Popen("bash run.sh", shell=True, cwd=dbs.workspace.path)
+    try:
+        p.wait()
+    except KeyboardInterrupt:
+        print()
+        print("Stopping execution.")
+        print("Execution stopped.")
+        p.kill()
+        print()
+
     return []
 
 
-def gen_entrypoint(ai, dbs):
+def gen_entrypoint(ai: AI, dbs: DBs) -> List[dict]:
     messages = ai.start(
         system=(
             "You will get information about a codebase that is currently on disk in "
             "the current folder.\n"
             "From this you will answer with code blocks that includes all the necessary "
             "unix terminal commands to "
             "a) install dependencies "
-            "b) run all necessary parts of the codebase (in parallell if necessary).\n"
+            "b) run all necessary parts of the codebase (in parallel if necessary).\n"
             "Do not install globally. Do not use sudo.\n"
             "Do not explain the code, just give the commands.\n"
             "Do not use placeholders, use example values (like . for a folder argument) "
             "if necessary.\n"
         ),
         user="Information about the codebase:\n\n" + dbs.workspace["all_output.txt"],
     )
@@ -191,88 +232,101 @@
     dbs.workspace["run.sh"] = "\n".join(match.group(1) for match in matches)
     return messages
 
 
 def use_feedback(ai: AI, dbs: DBs):
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
-        ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
+        ai.fuser(f"Instructions: {dbs.input['prompt']}"),
         ai.fassistant(dbs.workspace["all_output.txt"]),
         ai.fsystem(dbs.preprompts["use_feedback"]),
     ]
     messages = ai.next(messages, dbs.input["feedback"])
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
 def fix_code(ai: AI, dbs: DBs):
     code_output = json.loads(dbs.logs[gen_code.__name__])[-1]["content"]
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
-        ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
+        ai.fuser(f"Instructions: {dbs.input['prompt']}"),
         ai.fuser(code_output),
         ai.fsystem(dbs.preprompts["fix_code"]),
     ]
     messages = ai.next(messages, "Please fix any errors in the code above.")
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
+def human_review(ai: AI, dbs: DBs):
+    review = human_input()
+    dbs.memory["review"] = review.to_json()  # type: ignore
+    return []
+
+
 class Config(str, Enum):
     DEFAULT = "default"
     BENCHMARK = "benchmark"
     SIMPLE = "simple"
     TDD = "tdd"
     TDD_PLUS = "tdd+"
     CLARIFY = "clarify"
     RESPEC = "respec"
     EXECUTE_ONLY = "execute_only"
+    EVALUATE = "evaluate"
     USE_FEEDBACK = "use_feedback"
 
 
 # Different configs of what steps to run
 STEPS = {
     Config.DEFAULT: [
         clarify,
         gen_clarified_code,
         gen_entrypoint,
         execute_entrypoint,
+        human_review,
     ],
     Config.BENCHMARK: [simple_gen, gen_entrypoint],
     Config.SIMPLE: [simple_gen, gen_entrypoint, execute_entrypoint],
     Config.TDD: [
         gen_spec,
         gen_unit_tests,
         gen_code,
         gen_entrypoint,
         execute_entrypoint,
+        human_review,
     ],
     Config.TDD_PLUS: [
         gen_spec,
         gen_unit_tests,
         gen_code,
         fix_code,
         gen_entrypoint,
         execute_entrypoint,
+        human_review,
     ],
     Config.CLARIFY: [
         clarify,
         gen_clarified_code,
         gen_entrypoint,
         execute_entrypoint,
+        human_review,
     ],
     Config.RESPEC: [
         gen_spec,
         respec,
         gen_unit_tests,
         gen_code,
         fix_code,
         gen_entrypoint,
         execute_entrypoint,
+        human_review,
     ],
-    Config.USE_FEEDBACK: [use_feedback, gen_entrypoint, execute_entrypoint],
-    Config.EXECUTE_ONLY: [gen_entrypoint, execute_entrypoint],
+    Config.USE_FEEDBACK: [use_feedback, gen_entrypoint, execute_entrypoint, human_review],
+    Config.EXECUTE_ONLY: [execute_entrypoint],
+    Config.EVALUATE: [execute_entrypoint, human_review],
 }
 
 # Future steps that can be added:
 # run_tests_and_fix_files
-# execute_entrypoint_and_fix_files_if_needed
+# execute_entrypoint_and_fix_files_if_it_results_in_error
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer.egg-info/PKG-INFO` & `gpt-engineer-0.0.7/gpt_engineer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,93 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.6
+Version: 0.0.7
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPT Engineer
+
 [![Discord Follow](https://dcbadge.vercel.app/api/server/4t5vXHhu?style=flat)](https://discord.gg/4t5vXHhu)
 [![GitHub Repo stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer?style=social)](https://github.com/AntonOsika/gpt-engineer)
 [![Twitter Follow](https://img.shields.io/twitter/follow/antonosika?style=social)](https://twitter.com/AntonOsika)
 
 
 **Specify what you want it to build, the AI asks for clarification, and then builds it.**
 
 GPT Engineer is made to be easy to adapt, extend, and make your agent learn how you want your code to look. It generates an entire codebase based on a prompt.
 
 [Demo](https://twitter.com/antonosika/status/1667641038104674306) 👶🤖
 
 ## Project philosophy
+
 - Simple to get value
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-## Setup
+## Usage
+
+Choose either **stable** or **development**.
+
+For **stable** release:
+
+- `pip install gpt-engineer`
+
+For **development**:
 - `git clone git@github.com:AntonOsika/gpt-engineer.git`
 - `cd gpt-engineer`
 - `pip install -e .`
   - (or: `make install && source venv/bin/activate` for a venv)
 
+**Setup**
+
 With an api key that has GPT4 access run:
 
 - `export OPENAI_API_KEY=[your api key]`
 
 
 **Run**:
+
 - Create an empty folder. If inside the repo, you can run:
   - `cp -r projects/example/ projects/my-new-project`
-- Fill in the `main_prompt` file in your new folder
-- Run: `gpt-engineer projects/my-new-project`
+- Fill in the `prompt` file in your new folder
+- `gpt-engineer projects/my-new-project`
+  - (Note, `gpt-engineer --help` lets you see all available options. For example `--steps use_feedback` lets you improve/fix code in a project)
+
+By running gpt-engineer you agree to our [ToS](https://github.com/AntonOsika/gpt-engineer/TERMS_OF_USE.md).
 
 **Results**
 - Check the generated files in `projects/my-new-project/workspace`
 
 
 ## Features
-You can specify the "identity" of the AI agent by editing the files in the `identity` folder.
 
-Editing the identity, and evolving the `main_prompt`, is currently how you make the agent remember things between projects.
+You can specify the "identity" of the AI agent by editing the files in the `preprompts` folder.
+
+Editing the `preprompts`, and evolving how you write the project prompt, is currently how you make the agent remember things between projects.
 
 Each step in `steps.py` will have its communication history with GPT4 stored in the logs folder, and can be rerun with `scripts/rerun_edited_message_logs.py`.
 
 ## Contributing
-We are building the open platform for devs to tinker with and build their personal code-generation toolbox.
+The gpt-engineer community is building the **open platform for devs to tinker with and build their personal code-generation toolbox**.
+
+If you are interested in contributing to this, we would be interested in having you!
 
-If you want to contribute, please check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), [projects](https://github.com/AntonOsika/gpt-engineer/projects?query=is%3Aopen) or [issues tab](https://github.com/AntonOsika/gpt-engineer/issues) in the GitHub repo. You are welcome to read the [contributing document](.github/CONTRIBUTING.md) and join our [Discord 💬](https://discord.gg/4t5vXHhu).
+You can check for good first issues [here](https://github.com/AntonOsika/gpt-engineer/issues).
+Contributing document [here](.github/CONTRIBUTING.md).
 
 We are currently looking for more maintainers and community organisers. Email anton.osika@gmail.com if you are interested in an official role.
 
+If you want to see our broader ambitions, check out the [roadmap](https://github.com/AntonOsika/gpt-engineer/blob/main/ROADMAP.md), and join
+[discord ](https://discord.gg/4t5vXHhu)
+to get input on how you can contribute to it.
 
 ## Example
 
 https://github.com/AntonOsika/gpt-engineer/assets/4467025/6e362e45-4a94-4b0d-973d-393a31d92d9b
```

### Comparing `gpt-engineer-0.0.6/gpt_engineer.egg-info/SOURCES.txt` & `gpt-engineer-0.0.7/gpt_engineer.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 gpt_engineer/__init__.py
 gpt_engineer/ai.py
 gpt_engineer/chat_to_files.py
+gpt_engineer/collect.py
 gpt_engineer/db.py
+gpt_engineer/domain.py
+gpt_engineer/learning.py
 gpt_engineer/main.py
 gpt_engineer/steps.py
 gpt_engineer.egg-info/PKG-INFO
 gpt_engineer.egg-info/SOURCES.txt
 gpt_engineer.egg-info/dependency_links.txt
 gpt_engineer.egg-info/entry_points.txt
 gpt_engineer.egg-info/requires.txt
@@ -21,8 +24,9 @@
 gpt_engineer/preprompts/respec
 gpt_engineer/preprompts/spec
 gpt_engineer/preprompts/unit_tests
 gpt_engineer/preprompts/use_feedback
 gpt_engineer/preprompts/use_qa
 tests/test_ai.py
 tests/test_chat_to_files.py
+tests/test_collect.py
 tests/test_db.py
```

### Comparing `gpt-engineer-0.0.6/pyproject.toml` & `gpt-engineer-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpt-engineer"
-version = "0.0.6"
+version = "0.0.7"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 readme = "README.md"
 requires-python = ">=3"
 dependencies = [
   'black == 23.3.0',
   'mypy == 1.3.0',
   'openai == 0.27.8',
   'pre-commit == 3.3.3',
   'pytest == 7.3.1',
   'ruff == 0.0.272',
   'termcolor==2.3.0',
   'typer == 0.9.0',
+  'rudder-sdk-python == 2.0.2',
+  'dataclasses-json == 0.5.7',
 ]
 
 [project.scripts]
 gpt-engineer = 'gpt_engineer.main:app'
 
 [tool.setuptools]
 packages = ["gpt_engineer"]
```

### Comparing `gpt-engineer-0.0.6/tests/test_chat_to_files.py` & `gpt-engineer-0.0.7/tests/test_chat_to_files.py`

 * *Files identical despite different names*

