# Comparing `tmp/aider-chat-0.6.6.tar.gz` & `tmp/aider-chat-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.6.6.tar", last modified: Sat Jun 17 14:27:49 2023, max compression
+gzip compressed data, was "aider-chat-0.7.0.tar", last modified: Sun Jun 25 15:35:15 2023, max compression
```

## Comparing `aider-chat-0.6.6.tar` & `aider-chat-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:27:49.824157 aider-chat-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 14:27:35.000000 aider-chat-0.6.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 14:27:35.000000 aider-chat-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 14:27:49.824157 aider-chat-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-17 14:27:35.000000 aider-chat-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:27:49.824157 aider-chat-0.6.6/aider/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27031 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-17 14:27:35.000000 aider-chat-0.6.6/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:27:49.824157 aider-chat-0.6.6/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 14:27:49.000000 aider-chat-0.6.6/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-17 14:27:49.000000 aider-chat-0.6.6/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:27:49.000000 aider-chat-0.6.6/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 14:27:49.000000 aider-chat-0.6.6/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 14:27:49.000000 aider-chat-0.6.6/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 14:27:49.000000 aider-chat-0.6.6/aider_chat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 14:27:35.000000 aider-chat-0.6.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:27:49.824157 aider-chat-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-17 14:27:35.000000 aider-chat-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:27:49.824157 aider-chat-0.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-17 14:27:35.000000 aider-chat-0.6.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.827416 aider-chat-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-25 15:35:06.000000 aider-chat-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-25 15:35:06.000000 aider-chat-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-25 15:35:15.827416 aider-chat-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-06-25 15:35:06.000000 aider-chat-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.819416 aider-chat-0.7.0/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.823416 aider-chat-0.7.0/aider/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30047 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/base_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9871 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/editblock_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/editblock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_func_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_func_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/coders/wholefile_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-25 15:35:06.000000 aider-chat-0.7.0/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.827416 aider-chat-0.7.0/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 15:35:15.000000 aider-chat-0.7.0/aider_chat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-25 15:35:06.000000 aider-chat-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 15:35:15.827416 aider-chat-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-25 15:35:06.000000 aider-chat-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:15.827416 aider-chat-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_editblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-25 15:35:06.000000 aider-chat-0.7.0/tests/test_wholefile.py
```

### Comparing `aider-chat-0.6.6/LICENSE.txt` & `aider-chat-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.6/PKG-INFO` & `aider-chat-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.6.6
+Version: 0.7.0
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
 
@@ -50,44 +50,14 @@
 * Request new features, changes, improvements, or bug fixes to your code. Ask for new test cases, updated documentation or code refactors.
 * Aider will apply the edits suggested by GPT directly to your source files.
 * Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
-## GPT-4 vs GPT-3.5
-
-Aider supports all of OpenAI's chat models, including
-the the brand new `gpt-3.5-turbo-16k` model. 
-To use `gpt-3.5-turbo-16k`, install from GitHub per the instructions below and launch with `aider -3`.
-
-You will probably get the best results with one of the GPT-4 models,
-because of their large context windows,
-adherance to system prompt instructions and
-greater competance at coding tasks.
-The GPT-4 models are also able to use a
-[repository map](https://aider.chat/docs/ctags.html)
-to improve their ability to make changes in larger codebases.
-
-The GPT-3.5 models are supported more experimentally
-and are limited to editing somewhat smaller codebases.
-They are less able to follow instructions and
-aren't able to return code edits in a compact format.
-So aider has
-to ask GPT-3.5 to return a full copy of any code that needs to be edited.
-This rapidly uses up tokens and can hit the limits of the context window.
-In practice, this means you can only use `gpt-3.5-turbo` to edit files that are
-smaller than about 2k tokens (8k bytes).
-The new `gpt-3.5-turbo-16k` model should be able to edit code up to 8k tokens (32k bytes).
-
-Aider disables the
-[repository map feature](https://aider.chat/docs/ctags.html)
-when used with GPT-3.5 models.
-The `gpt-3.5-turbo` context window is too small to include a repo map.
-Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
 
 ## Installation
 
 1. Install the package:
   * PyPI: `pip install aider-chat`
   * GitHub: `pip install git+https://github.com/paul-gauthier/aider.git`
   * Local clone: `pip install -e .` 
@@ -102,48 +72,97 @@
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
 ```
 
-Replace `<file1>`, `<file2>`, etc., with the paths to the source code files you want to work on. These files will be added to the chat session.
+Replace `<file1>`, `<file2>`, etc., with the paths to the source code files you want to work on.
+These files will be "added to the chat session", so that GPT can see their contents and edit them according to your instructions.
 
 You can also just launch `aider` anywhere in a git repo without naming
 files on the command line.  It will discover all the files in the
 repo.  You can then add and remove individual files in the chat
 session with the `/add` and `/drop` chat commands described below.
 If you or GPT mention one of the repo's filenames in the conversation,
 aider will ask if you'd like to add it to the chat.
 
-You can also use additional command-line options, environment variables or configuration file
+Aider will work best if you think about which files need to be edited to make your change and add them to the chat.
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
+
+Aider also has many
+additional command-line options, environment variables or configuration file
 to set many options. See `aider --help` for details.
 
 ## In-chat commands
 
 Aider supports commands from within the chat, which all start with `/`. Here are some of the most useful in-chat commands:
 
 * `/add <file>`: Add matching files to the chat session.
 * `/drop <file>`: Remove matching files from the chat session.
 * `/undo`: Undo the last git commit if it was done by aider.
 * `/diff`: Display the diff of the last aider commit.
 * `/run <command>`: Run a shell command and optionally add the output to the chat.
 * `/help`: Show help about all commands.
 
+
 ## Tips
 
+* Think about which files need to be edited to make your change and add them to the chat.
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself. 
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
 * Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
+## GPT-4 vs GPT-3.5
+
+Aider supports all of OpenAI's chat models, including
+the the brand new `gpt-3.5-turbo-16k` model. 
+
+You will probably get the best results with one of the GPT-4 models,
+because of their large context windows,
+adherance to system prompt instructions and
+greater competance at coding tasks.
+The GPT-4 models are able to structure code edits as simple "diffs"
+and use a
+[repository map](https://aider.chat/docs/ctags.html)
+to improve their ability to make changes in larger codebases.
+
+The GPT-3.5 models are supported more experimentally
+and are limited to editing somewhat smaller codebases.
+They are less able to follow instructions and
+aren't able to return code edits in a compact "diff" format.
+So aider has
+to ask GPT-3.5 to return a new copy of the "whole file" with edits included.
+This rapidly uses up tokens and can hit the limits of the context window.
+
+Aider disables the
+[repository map feature](https://aider.chat/docs/ctags.html)
+when used with GPT-3.5 models.
+The `gpt-3.5-turbo` context window is too small to include a repo map.
+Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
+
+In practice, this means you can use aider to edit a set of source files
+that total up to the sizes below.
+You can (and should) add just the specific set of files to the chat
+that are relevant to the change you are requesting.
+This minimizes your use of the context window, as well as costs.
+
+| Model             | Context<br>Size | Edit<br>Format | Max<br>File Size | Max<br>File Size | Repo<br>Map? |
+| ----------------- | -- | --     | -----| -- | -- |
+| gpt-3.5-turbo     |  4k tokens | whole file | 2k tokens | ~8k bytes | no |
+| gpt-3.5-turbo-16k | 16k tokens | whole file | 8k tokens | ~32k bytes | no |
+| gpt-4             |  8k tokens | diffs | 8k tokens | ~32k bytes | yes | 
+| gpt-4-32k         | 32k tokens | diffs | 32k tokens  | ~128k bytes | yes |
+
 ## Kind words from users
 
 * "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
 * "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
 * "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
```

### Comparing `aider-chat-0.6.6/README.md` & `aider-chat-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 It also has features that [help GPT-4 understand and modify larger codebases](https://aider.chat/docs/ctags.html).
 
 ![aider screencast](assets/screencast.svg)
 
 - [Getting started](#getting-started)
 - [Example chat transcripts](#example-chat-transcripts)
 - [Features](#features)
-- [GPT-4 vs GPT-3.5](#gpt-4-vs-gpt-35)
 - [Installation](#installation)
 - [Usage](#usage)
 - [In-chat commands](#in-chat-commands)
 - [Tips](#tips)
+- [GPT-4 vs GPT-3.5](#gpt-4-vs-gpt-35)
 
 ## Getting started
 
 ```
 $ pip install aider-chat
 $ export OPENAI_API_KEY=your-key-goes-here
 $ aider myapp.py
@@ -51,44 +51,14 @@
 * Request new features, changes, improvements, or bug fixes to your code. Ask for new test cases, updated documentation or code refactors.
 * Aider will apply the edits suggested by GPT directly to your source files.
 * Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
-## GPT-4 vs GPT-3.5
-
-Aider supports all of OpenAI's chat models, including
-the the brand new `gpt-3.5-turbo-16k` model. 
-To use `gpt-3.5-turbo-16k`, install from GitHub per the instructions below and launch with `aider -3`.
-
-You will probably get the best results with one of the GPT-4 models,
-because of their large context windows,
-adherance to system prompt instructions and
-greater competance at coding tasks.
-The GPT-4 models are also able to use a
-[repository map](https://aider.chat/docs/ctags.html)
-to improve their ability to make changes in larger codebases.
-
-The GPT-3.5 models are supported more experimentally
-and are limited to editing somewhat smaller codebases.
-They are less able to follow instructions and
-aren't able to return code edits in a compact format.
-So aider has
-to ask GPT-3.5 to return a full copy of any code that needs to be edited.
-This rapidly uses up tokens and can hit the limits of the context window.
-In practice, this means you can only use `gpt-3.5-turbo` to edit files that are
-smaller than about 2k tokens (8k bytes).
-The new `gpt-3.5-turbo-16k` model should be able to edit code up to 8k tokens (32k bytes).
-
-Aider disables the
-[repository map feature](https://aider.chat/docs/ctags.html)
-when used with GPT-3.5 models.
-The `gpt-3.5-turbo` context window is too small to include a repo map.
-Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
 
 ## Installation
 
 1. Install the package:
   * PyPI: `pip install aider-chat`
   * GitHub: `pip install git+https://github.com/paul-gauthier/aider.git`
   * Local clone: `pip install -e .` 
@@ -103,48 +73,97 @@
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
 ```
 
-Replace `<file1>`, `<file2>`, etc., with the paths to the source code files you want to work on. These files will be added to the chat session.
+Replace `<file1>`, `<file2>`, etc., with the paths to the source code files you want to work on.
+These files will be "added to the chat session", so that GPT can see their contents and edit them according to your instructions.
 
 You can also just launch `aider` anywhere in a git repo without naming
 files on the command line.  It will discover all the files in the
 repo.  You can then add and remove individual files in the chat
 session with the `/add` and `/drop` chat commands described below.
 If you or GPT mention one of the repo's filenames in the conversation,
 aider will ask if you'd like to add it to the chat.
 
-You can also use additional command-line options, environment variables or configuration file
+Aider will work best if you think about which files need to be edited to make your change and add them to the chat.
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
+
+Aider also has many
+additional command-line options, environment variables or configuration file
 to set many options. See `aider --help` for details.
 
 ## In-chat commands
 
 Aider supports commands from within the chat, which all start with `/`. Here are some of the most useful in-chat commands:
 
 * `/add <file>`: Add matching files to the chat session.
 * `/drop <file>`: Remove matching files from the chat session.
 * `/undo`: Undo the last git commit if it was done by aider.
 * `/diff`: Display the diff of the last aider commit.
 * `/run <command>`: Run a shell command and optionally add the output to the chat.
 * `/help`: Show help about all commands.
 
+
 ## Tips
 
+* Think about which files need to be edited to make your change and add them to the chat.
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself. 
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
 * Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
+## GPT-4 vs GPT-3.5
+
+Aider supports all of OpenAI's chat models, including
+the the brand new `gpt-3.5-turbo-16k` model. 
+
+You will probably get the best results with one of the GPT-4 models,
+because of their large context windows,
+adherance to system prompt instructions and
+greater competance at coding tasks.
+The GPT-4 models are able to structure code edits as simple "diffs"
+and use a
+[repository map](https://aider.chat/docs/ctags.html)
+to improve their ability to make changes in larger codebases.
+
+The GPT-3.5 models are supported more experimentally
+and are limited to editing somewhat smaller codebases.
+They are less able to follow instructions and
+aren't able to return code edits in a compact "diff" format.
+So aider has
+to ask GPT-3.5 to return a new copy of the "whole file" with edits included.
+This rapidly uses up tokens and can hit the limits of the context window.
+
+Aider disables the
+[repository map feature](https://aider.chat/docs/ctags.html)
+when used with GPT-3.5 models.
+The `gpt-3.5-turbo` context window is too small to include a repo map.
+Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
+
+In practice, this means you can use aider to edit a set of source files
+that total up to the sizes below.
+You can (and should) add just the specific set of files to the chat
+that are relevant to the change you are requesting.
+This minimizes your use of the context window, as well as costs.
+
+| Model             | Context<br>Size | Edit<br>Format | Max<br>File Size | Max<br>File Size | Repo<br>Map? |
+| ----------------- | -- | --     | -----| -- | -- |
+| gpt-3.5-turbo     |  4k tokens | whole file | 2k tokens | ~8k bytes | no |
+| gpt-3.5-turbo-16k | 16k tokens | whole file | 8k tokens | ~32k bytes | no |
+| gpt-4             |  8k tokens | diffs | 8k tokens | ~32k bytes | yes | 
+| gpt-4-32k         | 32k tokens | diffs | 32k tokens  | ~128k bytes | yes |
+
 ## Kind words from users
 
 * "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
 * "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
 * "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
```

### Comparing `aider-chat-0.6.6/aider/coder.py` & `aider-chat-0.7.0/aider/coders/base_coder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,119 +1,152 @@
 #!/usr/bin/env python
 
+import json
 import os
 import sys
 import traceback
+from json.decoder import JSONDecodeError
 from pathlib import Path
 
 import backoff
 import git
 import openai
 import requests
-from openai.error import RateLimitError
+from openai.error import APIError, RateLimitError, ServiceUnavailableError
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 
-from aider import diffs, models, prompts, utils
+from aider import models, prompts, utils
 from aider.commands import Commands
 from aider.repomap import RepoMap
 
-from .dump import dump  # noqa: F401
+from ..dump import dump  # noqa: F401
 
 
 class MissingAPIKeyError(ValueError):
     pass
 
 
+class ExhaustedContextWindow(Exception):
+    pass
+
+
 class Coder:
     abs_fnames = None
     repo = None
     last_aider_commit_hash = None
     last_asked_for_commit_time = 0
     repo_map = None
+    functions = None
+    total_cost = 0.0
+
+    @classmethod
+    def create(
+        self,
+        main_model,
+        edit_format,
+        io,
+        openai_api_key,
+        openai_api_base="https://api.openai.com/v1",
+        **kwargs,
+    ):
+        from . import EditBlockCoder, WholeFileCoder, WholeFileFunctionCoder
+
+        openai.api_key = openai_api_key
+        openai.api_base = openai_api_base
+
+        if not main_model:
+            main_model = models.GPT35_16k
+
+        if not main_model.always_available:
+            if not check_model_availability(main_model):
+                if main_model != models.GPT4:
+                    io.tool_error(
+                        f"API key does not support {main_model.name}, falling back to"
+                        f" {models.GPT35_16k.name}"
+                    )
+                main_model = models.GPT35_16k
 
-    def check_model_availability(self, main_model):
-        available_models = openai.Model.list()
-        model_ids = [model.id for model in available_models["data"]]
-        return main_model.name in model_ids
+        if edit_format is None:
+            edit_format = main_model.edit_format
+
+        if edit_format == "diff":
+            return EditBlockCoder(main_model, io, **kwargs)
+        elif edit_format == "whole":
+            return WholeFileCoder(main_model, io, **kwargs)
+        elif edit_format == "whole-func":
+            return WholeFileFunctionCoder(main_model, io, **kwargs)
+        else:
+            raise ValueError(f"Unknown edit format {edit_format}")
 
     def __init__(
         self,
+        main_model,
         io,
-        main_model=models.GPT4.name,
         fnames=None,
         pretty=True,
         show_diffs=False,
         auto_commits=True,
         dirty_commits=True,
         dry_run=False,
         map_tokens=1024,
         verbose=False,
-        openai_api_key=None,
-        openai_api_base=None,
+        assistant_output_color="blue",
+        stream=True,
+        use_git=True,
     ):
-        if not openai_api_key:
-            raise MissingAPIKeyError("No OpenAI API key provided.")
-        openai.api_key = openai_api_key
-        openai.api_base = openai_api_base
+        if not fnames:
+            fnames = []
 
         self.verbose = verbose
         self.abs_fnames = set()
         self.cur_messages = []
         self.done_messages = []
+        self.num_control_c = 0
 
         self.io = io
+        self.stream = stream
 
         if not auto_commits:
             dirty_commits = False
 
         self.auto_commits = auto_commits
         self.dirty_commits = dirty_commits
+        self.assistant_output_color = assistant_output_color
 
         self.dry_run = dry_run
         self.pretty = pretty
 
         if pretty:
             self.console = Console()
         else:
             self.console = Console(force_terminal=True, no_color=True)
 
-        main_model = models.Model(main_model)
-        if not main_model.is_always_available():
-            if not self.check_model_availability(main_model):
-                if main_model != models.GPT4:
-                    self.io.tool_error(
-                        f"API key does not support {main_model.name}, falling back to"
-                        f" {models.GPT35_16k.name}"
-                    )
-                main_model = models.GPT35_16k
-
         self.main_model = main_model
-        if main_model.is_gpt35():
-            self.gpt_prompts = prompts.GPT35()
-        else:
-            self.gpt_prompts = prompts.GPT4()
 
         self.io.tool_output(f"Model: {main_model.name}")
 
         self.show_diffs = show_diffs
 
         self.commands = Commands(self.io, self)
 
-        self.set_repo(fnames)
+        if use_git:
+            self.set_repo(fnames)
+        else:
+            self.abs_fnames = [str(Path(fname).resolve()) for fname in fnames]
 
         if self.repo:
             rel_repo_dir = os.path.relpath(self.repo.git_dir, os.getcwd())
             self.io.tool_output(f"Git repo: {rel_repo_dir}")
         else:
             self.io.tool_output("Git repo: none")
             self.find_common_root()
 
-        if main_model.is_gpt4():
+        if main_model.use_repo_map and self.repo:
             rm_io = io if self.verbose else None
             self.repo_map = RepoMap(
                 map_tokens,
                 self.root,
                 self.main_model,
                 rm_io,
                 self.gpt_prompts.repo_content_prefix,
@@ -124,23 +157,24 @@
             elif not self.repo_map.has_ctags and map_tokens > 0:
                 self.io.tool_output(
                     f"Repo-map: basic using {map_tokens} tokens (universal-ctags not found)"
                 )
             else:
                 self.io.tool_output("Repo-map: disabled because map_tokens == 0")
         else:
-            self.io.tool_output("Repo-map: disabled for gpt-3.5")
+            self.io.tool_output("Repo-map: disabled")
 
         for fname in self.get_inchat_relative_files():
             self.io.tool_output(f"Added {fname} to the chat.")
 
     def find_common_root(self):
-        if self.abs_fnames:
-            common_prefix = os.path.commonpath(list(self.abs_fnames))
-            self.root = os.path.dirname(common_prefix)
+        if len(self.abs_fnames) == 1:
+            self.root = os.path.dirname(list(self.abs_fnames)[0])
+        elif self.abs_fnames:
+            self.root = os.path.commonpath(list(self.abs_fnames))
         else:
             self.root = os.getcwd()
 
     def set_repo(self, cmd_line_fnames):
         if not cmd_line_fnames:
             cmd_line_fnames = ["."]
 
@@ -240,26 +274,29 @@
         if self.abs_fnames:
             files_messages += [
                 dict(role="system", content=self.gpt_prompts.system_reminder),
             ]
 
         return files_messages
 
-    def run(self):
-        self.done_messages = []
-        self.cur_messages = []
-
-        self.num_control_c = 0
-
+    def run(self, with_message=None):
         while True:
             try:
-                new_user_message = self.run_loop()
+                if with_message:
+                    new_user_message = with_message
+                    self.io.user_input(with_message)
+                else:
+                    new_user_message = self.run_loop()
+
                 while new_user_message:
                     new_user_message = self.send_new_user_message(new_user_message)
 
+                if with_message:
+                    return
+
             except KeyboardInterrupt:
                 self.num_control_c += 1
                 if self.num_control_c >= 2:
                     break
                 self.io.tool_error("^C again or /exit to quit")
             except EOFError:
                 return
@@ -320,55 +357,77 @@
 
     def send_new_user_message(self, inp):
         self.cur_messages += [
             dict(role="user", content=inp),
         ]
 
         main_sys = self.gpt_prompts.main_system
-        if self.main_model.is_gpt4():
+        if self.main_model.max_context_tokens > 4 * 1024:
             main_sys += "\n" + self.gpt_prompts.system_reminder
 
         messages = [
             dict(role="system", content=main_sys),
         ]
 
         messages += self.done_messages
 
         messages += self.get_files_messages()
         messages += self.cur_messages
 
         if self.verbose:
             utils.show_messages(messages)
 
-        content, interrupted = self.send(messages)
+        exhausted = False
+        interrupted = False
+        try:
+            interrupted = self.send(messages, functions=self.functions)
+        except ExhaustedContextWindow:
+            exhausted = True
+        except openai.error.InvalidRequestError as err:
+            if "maximum context length" in str(err):
+                exhausted = True
+
+        if exhausted:
+            self.io.tool_error("The chat session is larger than the context window!\n")
+            self.commands.cmd_tokens("")
+            self.io.tool_error("\nTo reduce token usage:")
+            self.io.tool_error(" - Use /drop to remove unneeded files from the chat session.")
+            self.io.tool_error(" - Use /clear to clear chat history.")
+            return
+
+        if self.partial_response_function_call:
+            args = self.parse_partial_args()
+            if args:
+                content = args["explanation"]
+            else:
+                content = ""
+        elif self.partial_response_content:
+            content = self.partial_response_content
+        else:
+            content = ""
+
         if interrupted:
             self.io.tool_error("\n\n^C KeyboardInterrupt")
+            self.num_control_c += 1
             content += "\n^C KeyboardInterrupt"
 
         self.io.tool_output()
         if interrupted:
             self.cur_messages += [dict(role="assistant", content=content)]
             return
 
-        edited, edit_error = self.apply_updates(content)
+        edited, edit_error = self.apply_updates()
         if edit_error:
             return edit_error
 
-        if self.main_model.is_gpt4() or not edited:
-            # Don't add 3.5 assistant messages to the history if they contain "edits"
-            # Because those edits are actually fully copies of the file!
-            # That wastes too much context window.
-            self.cur_messages += [dict(role="assistant", content=content)]
-        else:
-            self.cur_messages += [
-                dict(role="assistant", content=self.gpt_prompts.redacted_edit_message)
-            ]
+        # TODO: this shouldn't use content, should use self.partial_....
+        self.update_cur_messages(content, edited)
 
         if edited:
-            if self.auto_commits:
+            if self.auto_commits and not self.dry_run:
                 saved_message = self.auto_commit()
             else:
                 saved_message = None
             self.move_back_cur_messages(saved_message)
 
         add_rel_files_message = self.check_for_file_mentions(content)
         if add_rel_files_message:
@@ -381,16 +440,16 @@
             self.last_aider_commit_hash = commit_hash
 
             saved_message = self.gpt_prompts.files_content_gpt_edits.format(
                 hash=commit_hash,
                 message=commit_message,
             )
         else:
-            # TODO: if not self.repo then the files_content_gpt_no_edits isn't appropriate
-            self.io.tool_error("Warning: no changes found in tracked files.")
+            if self.repo:
+                self.io.tool_error("Warning: no changes found in tracked files.")
             saved_message = self.gpt_prompts.files_content_gpt_no_edits
 
         return saved_message
 
     def check_for_file_mentions(self, content):
         words = set(word for word in content.split())
 
@@ -431,201 +490,153 @@
         for rel_fname in mentioned_rel_fnames:
             self.abs_fnames.add(os.path.abspath(os.path.join(self.root, rel_fname)))
 
         return prompts.added_files.format(fnames=", ".join(mentioned_rel_fnames))
 
     @backoff.on_exception(
         backoff.expo,
-        (RateLimitError, requests.exceptions.ConnectionError),
+        (APIError, ServiceUnavailableError, RateLimitError, requests.exceptions.ConnectionError),
         max_tries=5,
         on_backoff=lambda details: print(f"Retry in {details['wait']} seconds."),
     )
-    def send_with_retries(self, model, messages):
-        return openai.ChatCompletion.create(
+    def send_with_retries(self, model, messages, functions):
+        kwargs = dict(
             model=model,
             messages=messages,
             temperature=0,
-            stream=True,
+            stream=self.stream,
         )
+        if functions is not None:
+            kwargs["functions"] = self.functions
+
+        res = openai.ChatCompletion.create(**kwargs)
+        return res
 
-    def send(self, messages, model=None, silent=False):
+    def send(self, messages, model=None, silent=False, functions=None):
         if not model:
             model = self.main_model.name
 
-        self.resp = ""
+        self.partial_response_content = ""
+        self.partial_response_function_call = dict()
+
         interrupted = False
         try:
-            completion = self.send_with_retries(model, messages)
-            self.show_send_output(completion, silent)
+            completion = self.send_with_retries(model, messages, functions)
+            if self.stream:
+                self.show_send_output_stream(completion, silent)
+            else:
+                self.show_send_output(completion, silent)
         except KeyboardInterrupt:
             interrupted = True
 
         if not silent:
-            self.io.ai_output(self.resp)
+            if self.partial_response_content:
+                self.io.ai_output(self.partial_response_content)
+            elif self.partial_response_function_call:
+                # TODO: push this into subclasses
+                args = self.parse_partial_args()
+                if args:
+                    explanation = args.get("explanation")
+                    if explanation:
+                        self.io.ai_output(explanation)
 
-        return self.resp, interrupted
+        return interrupted
 
     def show_send_output(self, completion, silent):
+        if self.verbose:
+            print(completion)
+
+        show_func_err = None
+        show_content_err = None
+        try:
+            self.partial_response_function_call = completion.choices[0].message.function_call
+        except AttributeError as func_err:
+            show_func_err = func_err
+
+        try:
+            self.partial_response_content = completion.choices[0].message.content
+        except AttributeError as content_err:
+            show_content_err = content_err
+
+        if show_func_err and show_content_err:
+            self.io.tool_error(show_func_err)
+            self.io.tool_error(show_content_err)
+            raise Exception("No data found in openai response!")
+
+        prompt_tokens = completion.usage.prompt_tokens
+        completion_tokens = completion.usage.completion_tokens
+
+        tokens = f"{prompt_tokens} prompt tokens, {completion_tokens} completion tokens"
+        if self.main_model.prompt_price:
+            cost = prompt_tokens * self.main_model.prompt_price / 1000
+            cost += completion_tokens * self.main_model.completion_price / 1000
+            tokens += f", ${cost:.6f} cost"
+            self.total_cost += cost
+
+        show_resp = self.render_incremental_response(True)
+        if self.pretty:
+            show_resp = Markdown(show_resp, style=self.assistant_output_color, code_theme="default")
+
+        self.io.console.print(show_resp)
+        self.io.console.print(tokens)
+
+    def show_send_output_stream(self, completion, silent):
         live = None
         if self.pretty and not silent:
             live = Live(vertical_overflow="scroll")
 
         try:
             if live:
                 live.start()
 
             for chunk in completion:
-                if chunk.choices[0].finish_reason not in (None, "stop"):
-                    assert False, "Exceeded context window!"
+                if chunk.choices[0].finish_reason == "length":
+                    raise ExhaustedContextWindow()
+
+                try:
+                    func = chunk.choices[0].delta.function_call
+                    # dump(func)
+                    for k, v in func.items():
+                        if k in self.partial_response_function_call:
+                            self.partial_response_function_call[k] += v
+                        else:
+                            self.partial_response_function_call[k] = v
+                except AttributeError:
+                    pass
 
                 try:
                     text = chunk.choices[0].delta.content
-                    self.resp += text
+                    if text:
+                        self.partial_response_content += text
                 except AttributeError:
-                    continue
+                    pass
 
                 if silent:
                     continue
 
                 if self.pretty:
-                    show_resp = self.resp
-                    if self.main_model.is_gpt35():
-                        try:
-                            show_resp = self.update_files_gpt35(self.resp, mode="diff")
-                        except ValueError:
-                            pass
-                    md = Markdown(show_resp, style="blue", code_theme="default")
-                    live.update(md)
+                    self.live_incremental_response(live, False)
                 else:
                     sys.stdout.write(text)
                     sys.stdout.flush()
         finally:
             if live:
+                self.live_incremental_response(live, True)
                 live.stop()
 
-    def update_files_gpt35(self, content, mode="update"):
-        edited = set()
-        chat_files = self.get_inchat_relative_files()
-        if not chat_files:
-            if mode == "diff":
-                return content
-            return
-
-        output = []
-        lines = content.splitlines(keepends=True)
-        fname = None
-        new_lines = []
-        for i, line in enumerate(lines):
-            if line.startswith("```"):
-                if fname:
-                    # ending an existing block
-                    full_path = os.path.abspath(os.path.join(self.root, fname))
-
-                    if mode == "diff":
-                        with open(full_path, "r") as f:
-                            orig_lines = f.readlines()
-
-                        show_diff = diffs.diff_partial_update(
-                            orig_lines,
-                            new_lines,
-                            final=True,
-                        ).splitlines()
-                        output += show_diff
-                    else:
-                        new_lines = "".join(new_lines)
-                        Path(full_path).write_text(new_lines)
-                        edited.add(fname)
-
-                    fname = None
-                    new_lines = []
-                    continue
-
-                # starting a new block
-                if i == 0:
-                    raise ValueError("No filename provided before ``` block")
-
-                fname = lines[i - 1].strip()
-                if fname not in chat_files:
-                    if len(chat_files) == 1:
-                        fname = list(chat_files)[0]
-                    else:
-                        show_chat_files = " ".join(chat_files)
-                        raise ValueError(f"{fname} is not one of: {show_chat_files}")
-
-            elif fname:
-                new_lines.append(line)
-            else:
-                output.append(line)
-
-        if mode == "diff":
-            if fname:
-                # ending an existing block
-                full_path = os.path.abspath(os.path.join(self.root, fname))
-
-                if mode == "diff":
-                    with open(full_path, "r") as f:
-                        orig_lines = f.readlines()
-
-                    show_diff = diffs.diff_partial_update(
-                        orig_lines,
-                        new_lines,
-                    ).splitlines()
-                    output += show_diff
-
-            return "\n".join(output)
-
-        if fname:
-            raise ValueError("Started a ``` block without closing it")
-
-        return edited
-
-    def update_files_gpt4(self, content):
-        # might raise ValueError for malformed ORIG/UPD blocks
-        edits = list(utils.find_original_update_blocks(content))
-
-        edited = set()
-        for path, original, updated in edits:
-            full_path = os.path.abspath(os.path.join(self.root, path))
+    def live_incremental_response(self, live, final):
+        show_resp = self.render_incremental_response(final)
+        if not show_resp:
+            return
 
-            if full_path not in self.abs_fnames:
-                if not Path(full_path).exists():
-                    question = f"Allow creation of new file {path}?"  # noqa: E501
-                else:
-                    question = (
-                        f"Allow edits to {path} which was not previously provided?"  # noqa: E501
-                    )
-                if not self.io.confirm_ask(question):
-                    self.io.tool_error(f"Skipping edit to {path}")
-                    continue
+        md = Markdown(show_resp, style=self.assistant_output_color, code_theme="default")
+        live.update(md)
 
-                if not Path(full_path).exists():
-                    Path(full_path).parent.mkdir(parents=True, exist_ok=True)
-                    Path(full_path).touch()
-
-                self.abs_fnames.add(full_path)
-
-                # Check if the file is already in the repo
-                if self.repo:
-                    tracked_files = set(self.repo.git.ls_files().splitlines())
-                    relative_fname = self.get_rel_fname(full_path)
-                    if relative_fname not in tracked_files and self.io.confirm_ask(
-                        f"Add {path} to git?"
-                    ):
-                        self.repo.git.add(full_path)
-
-            edited.add(path)
-            if utils.do_replace(full_path, original, updated, self.dry_run):
-                if self.dry_run:
-                    self.io.tool_output(f"Dry run, did not apply edit to {path}")
-                else:
-                    self.io.tool_output(f"Applied edit to {path}")
-            else:
-                self.io.tool_error(f"Failed to apply edit to {path}")
-
-        return edited
+    def render_incremental_response(self, final):
+        return self.partial_response_content
 
     def get_context_from_history(self, history):
         context = ""
         if history:
             context += "# Context:\n"
             for msg in history:
                 context += msg["role"].upper() + ": " + msg["content"] + "\n"
@@ -642,26 +653,27 @@
 
         messages = [
             dict(role="system", content=prompts.commit_system),
             dict(role="user", content=context + diffs),
         ]
 
         try:
-            commit_message, interrupted = self.send(
+            interrupted = self.send(
                 messages,
                 model=models.GPT35.name,
                 silent=True,
             )
         except openai.error.InvalidRequestError:
             self.io.tool_error(
                 f"Failed to generate commit message using {models.GPT35.name} due to an invalid"
                 " request."
             )
             return
 
+        commit_message = self.partial_response_content
         commit_message = commit_message.strip()
         if commit_message and commit_message[0] == '"' and commit_message[-1] == '"':
             commit_message = commit_message[1:-1].strip()
 
         if interrupted:
             self.io.tool_error(
                 f"Unable to get commit message from {models.GPT35.name}. Use /commit to try again."
@@ -787,29 +799,115 @@
         if not files:
             return 0
         return max(Path(path).stat().st_mtime for path in files)
 
     def get_addable_relative_files(self):
         return set(self.get_all_relative_files()) - set(self.get_inchat_relative_files())
 
-    def apply_updates(self, content):
-        if self.main_model.is_gpt4():
-            method = self.update_files_gpt4
-        elif self.main_model.is_gpt35():
-            method = self.update_files_gpt35
+    def allowed_to_edit(self, path, write_content=None):
+        full_path = os.path.abspath(os.path.join(self.root, path))
+
+        if full_path in self.abs_fnames:
+            if not self.dry_run and write_content:
+                Path(full_path).write_text(write_content)
+            return full_path
+
+        if not Path(full_path).exists():
+            question = f"Allow creation of new file {path}?"  # noqa: E501
         else:
-            raise ValueError(f"apply_updates() doesn't support {self.main_model.name}")
+            question = f"Allow edits to {path} which was not previously provided?"  # noqa: E501
+        if not self.io.confirm_ask(question):
+            self.io.tool_error(f"Skipping edit to {path}")
+            return
+
+        if not Path(full_path).exists() and not self.dry_run:
+            Path(full_path).parent.mkdir(parents=True, exist_ok=True)
+            Path(full_path).touch()
+
+        self.abs_fnames.add(full_path)
+
+        # Check if the file is already in the repo
+        if self.repo:
+            tracked_files = set(self.repo.git.ls_files().splitlines())
+            relative_fname = self.get_rel_fname(full_path)
+            if relative_fname not in tracked_files and self.io.confirm_ask(f"Add {path} to git?"):
+                if not self.dry_run:
+                    self.repo.git.add(full_path)
+
+        if not self.dry_run and write_content:
+            Path(full_path).write_text(write_content)
+
+        return full_path
+
+    apply_update_errors = 0
+
+    def apply_updates(self):
+        max_apply_update_errors = 2
 
         try:
-            edited = method(content)
-            return edited, None
+            edited = self.update_files()
         except ValueError as err:
             err = err.args[0]
-            self.io.tool_error("Malformed ORIGINAL/UPDATE blocks, retrying...")
-            self.io.tool_error(str(err))
-            return None, err
+            self.apply_update_errors += 1
+            if self.apply_update_errors < max_apply_update_errors:
+                self.io.tool_error(f"Malformed response #{self.apply_update_errors}, retrying...")
+                self.io.tool_error(str(err))
+                return None, err
+            else:
+                self.io.tool_error(f"Malformed response #{self.apply_update_errors}, aborting.")
+                return False, None
 
         except Exception as err:
             print(err)
             print()
             traceback.print_exc()
-            return None, err
+            self.apply_update_errors += 1
+            if self.apply_update_errors < max_apply_update_errors:
+                self.io.tool_error(f"Update exception #{self.apply_update_errors}, retrying...")
+                return None, err
+            else:
+                self.io.tool_error(f"Update exception #{self.apply_update_errors}, aborting")
+                return False, None
+
+        self.apply_update_errors = 0
+
+        if edited:
+            for path in sorted(edited):
+                if self.dry_run:
+                    self.io.tool_output(f"Did not apply edit to {path} (--dry-run)")
+                else:
+                    self.io.tool_output(f"Applied edit to {path}")
+
+        return edited, None
+
+    def parse_partial_args(self):
+        # dump(self.partial_response_function_call)
+
+        data = self.partial_response_function_call.get("arguments")
+        if not data:
+            return
+
+        try:
+            return json.loads(data)
+        except JSONDecodeError:
+            pass
+
+        try:
+            return json.loads(data + "]}")
+        except JSONDecodeError:
+            pass
+
+        try:
+            return json.loads(data + "}]}")
+        except JSONDecodeError:
+            pass
+
+        try:
+            return json.loads(data + '"}]}')
+        except JSONDecodeError:
+            pass
+
+
+def check_model_availability(main_model):
+    available_models = openai.Model.list()
+    model_ids = [model.id for model in available_models["data"]]
+    return main_model.name in model_ids
```

### Comparing `aider-chat-0.6.6/aider/commands.py` & `aider-chat-0.7.0/aider/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,74 +75,81 @@
             self.io.tool_error("No more changes to commit.")
             return
 
         commit_message = args.strip()
         self.coder.commit(message=commit_message, which="repo_files")
 
     def cmd_clear(self, args):
-        "Clear the chat history and drop all files from the chat context"
+        "Clear the chat history"
 
-        self.coder.abs_fnames = set()
         self.coder.done_messages = []
         self.coder.cur_messages = []
 
     def cmd_tokens(self, args):
         "Report on the number of tokens used by the current chat context"
 
         res = []
 
         # system messages
         msgs = [
             dict(role="system", content=self.coder.gpt_prompts.main_system),
             dict(role="system", content=self.coder.gpt_prompts.system_reminder),
         ]
         tokens = len(self.tokenizer.encode(json.dumps(msgs)))
-        res.append((tokens, "system messages"))
+        res.append((tokens, "system messages", ""))
 
         # chat history
         msgs = self.coder.done_messages + self.coder.cur_messages
         if msgs:
             msgs = [dict(role="dummy", content=msg) for msg in msgs]
             msgs = json.dumps(msgs)
             tokens = len(self.tokenizer.encode(msgs))
-            res.append((tokens, "chat history"))
+            res.append((tokens, "chat history", "use /clear to clear"))
 
         # repo map
         other_files = set(self.coder.get_all_abs_files()) - set(self.coder.abs_fnames)
         if self.coder.repo_map:
             repo_content = self.coder.repo_map.get_repo_map(self.coder.abs_fnames, other_files)
             if repo_content:
                 tokens = len(self.tokenizer.encode(repo_content))
-                res.append((tokens, "repository map"))
+                res.append((tokens, "repository map", "use --map-tokens to resize"))
 
         # files
         for fname in self.coder.abs_fnames:
             relative_fname = self.coder.get_rel_fname(fname)
             quoted = utils.quoted_file(fname, relative_fname)
             tokens = len(self.tokenizer.encode(quoted))
-            res.append((tokens, relative_fname))
+            res.append((tokens, f"{relative_fname}", "use /drop to drop from chat"))
 
-        print("Context window usage, in tokens:")
-        print()
+        self.io.tool_output("Approximate context window usage, in tokens:")
+        self.io.tool_output()
+
+        width = 8
 
         def fmt(v):
-            return format(int(v), ",").rjust(6)
+            return format(int(v), ",").rjust(width)
+
+        col_width = max(len(row[1]) for row in res)
 
         total = 0
-        for tk, msg in res:
+        for tk, msg, tip in res:
             total += tk
-            print(f"{fmt(tk)} {msg}")
+            msg = msg.ljust(col_width)
+            self.io.tool_output(f"{fmt(tk)} {msg} {tip}")
 
-        print()
-        print(f"{fmt(total)} total")
+        self.io.tool_output("=" * width)
+        self.io.tool_output(f"{fmt(total)} tokens total")
 
         limit = self.coder.main_model.max_context_tokens
         remaining = limit - total
-        print(f"{fmt(remaining)} remaining")
-        print(f"{fmt(limit)} max context window")
+        if remaining > 0:
+            self.io.tool_output(f"{fmt(remaining)} tokens remaining in context window")
+        else:
+            self.io.tool_error(f"{fmt(remaining)} tokens remaining, window exhausted!")
+        self.io.tool_output(f"{fmt(limit)} tokens max context window size")
 
     def cmd_undo(self, args):
         "Undo the last git commit if it was done by aider"
         if not self.coder.repo:
             self.io.tool_error("No git repository found.")
             return
 
@@ -179,15 +186,15 @@
         self.coder.repo.git.reset("--hard", "HEAD~1")
         self.io.tool_output(
             f"{last_commit.message.strip()}\n"
             f"The above commit {self.coder.last_aider_commit_hash} "
             "was reset and removed from git.\n"
         )
 
-        if self.coder.main_model.is_gpt4():
+        if self.coder.main_model.send_undo_reply:
             return prompts.undo_command_reply
 
     def cmd_diff(self, args):
         "Display the diff of the last aider commit"
         if not self.coder.repo:
             self.io.tool_error("No git repository found.")
             return
@@ -266,14 +273,18 @@
         for fname in files:
             if partial.lower() in fname.lower():
                 yield Completion(fname, start_position=-len(partial))
 
     def cmd_drop(self, args):
         "Remove matching files from the chat session"
 
+        if not args.strip():
+            self.io.tool_output("Dropping all files from the chat session.")
+            self.coder.abs_fnames = []
+
         for word in args.split():
             matched_files = [
                 file
                 for file in self.coder.abs_fnames
                 if word.lower() in os.path.relpath(file, self.coder.root).lower()
             ]
             if not matched_files:
@@ -291,15 +302,15 @@
             result = subprocess.run(
                 parsed_args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, text=True
             )
             combined_output = result.stdout
         except Exception as e:
             self.io.tool_error(f"Error running command: {e}")
 
-        print(combined_output)
+        self.io.tool_output(combined_output)
 
         if self.io.confirm_ask("Add the output to the chat?", default="y"):
             for line in combined_output.splitlines():
                 self.io.tool_output(line, log_only=True)
 
             msg = prompts.run_output.format(
                 command=args,
```

### Comparing `aider-chat-0.6.6/aider/diffs.py` & `aider-chat-0.7.0/aider/diffs.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,50 +29,63 @@
     total_blocks = 30
     filled_blocks = int(total_blocks * percentage // 100)
     empty_blocks = total_blocks - filled_blocks
     bar = block * filled_blocks + empty * empty_blocks
     return bar
 
 
-def diff_partial_update(lines_orig, lines_updated, final=False):
+def diff_partial_update(lines_orig, lines_updated, final=False, fname=None):
     """
     Given only the first part of an updated file, show the diff while
     ignoring the block of "deleted" lines that are past the end of the
     partially complete update.
     """
 
     # dump(lines_orig)
     # dump(lines_updated)
 
-    last_non_deleted = find_last_non_deleted(lines_orig, lines_updated)
+    num_orig_lines = len(lines_orig)
+
+    if final:
+        last_non_deleted = num_orig_lines
+    else:
+        last_non_deleted = find_last_non_deleted(lines_orig, lines_updated)
+
     # dump(last_non_deleted)
     if last_non_deleted is None:
         return ""
 
-    num_orig_lines = len(lines_orig)
-    pct = last_non_deleted * 100 / num_orig_lines
+    if num_orig_lines:
+        pct = last_non_deleted * 100 / num_orig_lines
+    else:
+        pct = 50
     bar = create_progress_bar(pct)
     bar = f"! {last_non_deleted:3d} / {num_orig_lines:3d} lines [{bar}] {pct:3.0f}%\n\n"
 
     lines_orig = lines_orig[:last_non_deleted]
 
     if not final:
         lines_updated = lines_updated[:-1] + ["...\n"]
 
     diff = difflib.unified_diff(lines_orig, lines_updated, n=5)
 
     diff = list(diff)[2:]
 
     diff = "".join(diff)
+    if not diff.endswith("\n"):
+        diff += "\n"
 
     show = "```diff\n"
+    if fname:
+        show += f"--- {fname} original\n"
+        show += f"+++ {fname} updated\n"
     if not final:
         show += bar
 
-    show += diff + "```\n"
+    show += diff + "```\n\n"
 
     # print(diff)
 
     return show
 
 
 def find_last_non_deleted(lines_orig, lines_updated):
```

### Comparing `aider-chat-0.6.6/aider/dump.py` & `aider-chat-0.7.0/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.6/aider/io.py` & `aider-chat-0.7.0/aider/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from prompt_toolkit.styles import Style
 from pygments.lexers import MarkdownLexer, guess_lexer_for_filename
 from pygments.token import Token
 from pygments.util import ClassNotFound
 from rich.console import Console
 from rich.text import Text
 
+from .dump import dump  # noqa: F401
+
 
 class AutoCompleter(Completer):
     def __init__(self, root, rel_fnames, addable_rel_fnames, commands):
         self.commands = commands
         self.addable_rel_fnames = addable_rel_fnames
         self.rel_fnames = rel_fnames
 
@@ -101,14 +103,15 @@
         self.tool_output_color = tool_output_color if pretty else None
         self.tool_error_color = tool_error_color if pretty else None
 
         self.input = input
         self.output = output
         self.pretty = pretty
         self.yes = yes
+
         self.input_history_file = input_history_file
         if chat_history_file is not None:
             self.chat_history_file = Path(chat_history_file)
         else:
             self.chat_history_file = None
 
         if pretty:
@@ -164,63 +167,70 @@
 
             if self.input_history_file is not None:
                 session_kwargs["history"] = FileHistory(self.input_history_file)
 
             session = PromptSession(**session_kwargs)
             line = session.prompt()
 
-            if line.strip() == "{" and not multiline_input:
+            if line and line[0] == "{" and not multiline_input:
                 multiline_input = True
+                inp += line[1:] + "\n"
                 continue
-            elif line.strip() == "}" and multiline_input:
+            elif line and line[-1] == "}" and multiline_input:
+                inp += line[:-1] + "\n"
                 break
             elif multiline_input:
                 inp += line + "\n"
             else:
                 inp = line
                 break
 
         print()
+        self.user_input(inp)
+        return inp
 
+    def user_input(self, inp):
         prefix = "####"
         if inp:
             hist = inp.splitlines()
         else:
             hist = ["<blank>"]
 
         hist = f"  \n{prefix} ".join(hist)
 
         hist = f"""
 {prefix} {hist}"""
         self.append_chat_history(hist, linebreak=True)
 
-        return inp
-
     # OUTPUT
 
     def ai_output(self, content):
         hist = "\n" + content.strip() + "\n\n"
         self.append_chat_history(hist)
 
     def confirm_ask(self, question, default="y"):
-        if self.yes:
+        if self.yes is True:
             res = "yes"
+        elif self.yes is False:
+            res = "no"
         else:
             res = prompt(question + " ", default=default)
 
         hist = f"{question.strip()} {res.strip()}"
         self.append_chat_history(hist, linebreak=True, blockquote=True)
 
         if not res or not res.strip():
             return
         return res.strip().lower().startswith("y")
 
     def prompt_ask(self, question, default=None):
-        if self.yes:
+        if self.yes is True:
             res = "yes"
+        elif self.yes is False:
+            res = "no"
         else:
             res = prompt(question + " ", default=default)
 
         hist = f"{question.strip()} {res.strip()}"
         self.append_chat_history(hist, linebreak=True, blockquote=True)
 
         return res
```

### Comparing `aider-chat-0.6.6/aider/main.py` & `aider-chat-0.7.0/aider/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 import configargparse
 import git
 
-from aider import models, __version__
-from aider.coder import Coder
+from aider import __version__, models
+from aider.coders import Coder
 from aider.io import InputOutput
 
 
 def get_git_root():
     try:
         repo = git.Repo(search_parent_directories=True)
         return repo.working_tree_dir
@@ -34,15 +34,18 @@
         add_config_file_help=True,
         default_config_files=default_config_files,
         config_file_parser_class=configargparse.YAMLConfigFileParser,
         auto_env_var_prefix="AIDER_",
     )
 
     parser.add_argument(
-        "--version", action="version", version=f"%(prog)s {__version__}", help="Show the version number and exit"
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+        help="Show the version number and exit",
     )
 
     parser.add_argument(
         "-c",
         "--config",
         is_config_file=True,
         metavar="CONFIG_FILE",
@@ -87,26 +90,46 @@
         "-3",
         action="store_const",
         dest="model",
         const=models.GPT35_16k.name,
         help=f"Use {models.GPT35_16k.name} model for the main chat (gpt-4 is better)",
     )
     parser.add_argument(
+        "--edit-format",
+        metavar="EDIT_FORMAT",
+        default=None,
+        help="Specify what edit format GPT should use (default depends on model)",
+    )
+    parser.add_argument(
         "--pretty",
         action="store_true",
         default=True,
         help="Enable pretty, colorized output (default: True)",
     )
     parser.add_argument(
         "--no-pretty",
         action="store_false",
         dest="pretty",
         help="Disable pretty, colorized output",
     )
     parser.add_argument(
+        "--no-stream",
+        action="store_false",
+        dest="stream",
+        default=True,
+        help="Disable streaming responses",
+    )
+    parser.add_argument(
+        "--no-git",
+        action="store_false",
+        dest="git",
+        default=True,
+        help="Do not look for a git repo",
+    )
+    parser.add_argument(
         "--user-input-color",
         default="green",
         help="Set the color for user input (default: green)",
     )
     parser.add_argument(
         "--tool-output-color",
         default=None,
@@ -114,14 +137,19 @@
     )
     parser.add_argument(
         "--tool-error-color",
         default="red",
         help="Set the color for tool error messages (default: red)",
     )
     parser.add_argument(
+        "--assistant-output-color",
+        default="blue",
+        help="Set the color for assistant output (default: blue)",
+    )
+    parser.add_argument(
         "--apply",
         metavar="FILE",
         help="Apply the changes from the given file instead of running the chat (debug)",
     )
     parser.add_argument(
         "--auto-commits",
         action="store_true",
@@ -179,23 +207,30 @@
         default=1024,
         help="Max number of tokens to use for repo map, use 0 to disable (default: 1024)",
     )
     parser.add_argument(
         "--yes",
         action="store_true",
         help="Always say yes to every confirmation",
-        default=False,
+        default=None,
     )
     parser.add_argument(
         "-v",
         "--verbose",
         action="store_true",
         help="Enable verbose output",
         default=False,
     )
+    parser.add_argument(
+        "--message",
+        "--msg",
+        "-m",
+        metavar="COMMAND",
+        help="Specify a single message to send GPT, process reply then exit (disables chat mode)",
+    )
     args = parser.parse_args(args)
 
     io = InputOutput(
         args.pretty,
         args.yes,
         args.input_history_file,
         args.chat_history_file,
@@ -215,38 +250,49 @@
 
     io.tool_output(*sys.argv, log_only=True)
 
     if not args.openai_api_key:
         io.tool_error("No OpenAI API key provided. Use --openai-api-key or env OPENAI_API_KEY.")
         return 1
 
-    coder = Coder(
+    main_model = models.Model(args.model)
+
+    coder = Coder.create(
+        main_model,
+        args.edit_format,
         io,
-        main_model=args.model,
+        args.openai_api_key,
+        args.openai_api_base,
+        ##
         fnames=args.files,
         pretty=args.pretty,
         show_diffs=args.show_diffs,
         auto_commits=args.auto_commits,
         dirty_commits=args.dirty_commits,
         dry_run=args.dry_run,
         map_tokens=args.map_tokens,
         verbose=args.verbose,
-        openai_api_key=args.openai_api_key,
-        openai_api_base=args.openai_api_base,
+        assistant_output_color=args.assistant_output_color,
+        stream=args.stream,
+        use_git=args.git,
     )
 
     if args.dirty_commits:
         coder.commit(ask=True, which="repo_files")
 
     if args.apply:
         with open(args.apply, "r") as f:
             content = f.read()
         coder.apply_updates(content)
         return
 
     io.tool_output("Use /help to see in-chat commands.")
-    coder.run()
+    if args.message:
+        io.tool_output()
+        coder.run(with_message=args.message)
+    else:
+        coder.run()
 
 
 if __name__ == "__main__":
     status = main()
     sys.exit(status)
```

### Comparing `aider-chat-0.6.6/aider/prompts.py` & `aider-chat-0.7.0/aider/coders/editblock_prompts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa: E501
-# MAIN
 
+from .base_prompts import CoderPrompts
 
-class GPT4:
+
+class EditBlockPrompts(CoderPrompts):
     main_system = """Act as an expert software developer.
 Be concise!
 
 Take requests for changes to the supplied code.
 If the request is ambiguous, ask questions.
 
 Once you understand the request you MUST:
@@ -41,73 +42,15 @@
 - A new file path, including dir name if needed
 - An empty ORIGINAL section
 - The new file's contents in the UPDATED section
 
 If a request requires many changes, stop often to ask the user for feedback.
 """
 
-    files_content_gpt_edits = "I committed the changes with git hash {hash} & commit msg: {message}"
-
-    files_content_gpt_no_edits = "I didn't see any properly formatted edits in your reply?!"
-
-    files_content_local_edits = "I edited the files myself."
-
     files_content_prefix = "These are the *read-write* files:\n"
 
     files_no_full_files = "I am not sharing any *read-write* files yet."
 
     repo_content_prefix = (
         "Below here are summaries of other files! Do not propose changes to these *read-only*"
         " files without asking me first.\n"
     )
-
-
-class GPT35(GPT4):
-    main_system = """Act as an expert software developer.
-Take requests for changes to the supplied code.
-If the request is ambiguous, ask questions.
-
-Once you understand the request you MUST:
-1. Determine if any code changes are needed.
-2. Explain any needed changes.
-3. If changes are needed, output a copy of each file that needs changes.
-"""
-
-    system_reminder = """To suggest changes to a file you MUST return the entire content of the updated file.
-You MUST use this format:
-
-exact/path/to/filename.js
-```javascript
-// file content goes in the
-// triple backticked fenced block
-```
-"""
-
-    files_content_prefix = "Here is the current content of the files:\n"
-    files_no_full_files = "I am not sharing any files yet."
-
-    redacted_edit_message = "No changes are needed."
-
-
-# COMMIT
-commit_system = """You are an expert software engineer.
-Review the provided context and diffs which are about to be committed to a git repo.
-Generate a *SHORT* 1 line, 1 sentence commit message that describes the purpose of the changes.
-The commit message MUST be in the past tense.
-It must describe the changes *which have been made* in the diffs!
-Reply with JUST the commit message, without quotes, comments, questions, etc!
-"""
-
-# COMMANDS
-undo_command_reply = "I did `git reset --hard HEAD~1` to discard the last edits."
-
-added_files = "I added these *read-write* files: {fnames}"
-
-
-run_output = """I ran this command:
-
-{command}
-
-And got this output:
-
-{output}
-"""
```

### Comparing `aider-chat-0.6.6/aider/repomap.py` & `aider-chat-0.7.0/aider/repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.6/aider/utils.py` & `aider-chat-0.7.0/aider/coders/editblock_coder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 import math
 import re
 from difflib import SequenceMatcher
 from pathlib import Path
 
-from .dump import dump  # noqa: F401
+from .base_coder import Coder
+from .editblock_prompts import EditBlockPrompts
+
+
+class EditBlockCoder(Coder):
+    def __init__(self, *args, **kwargs):
+        self.gpt_prompts = EditBlockPrompts()
+        super().__init__(*args, **kwargs)
+
+    def update_cur_messages(self, content, edited):
+        self.cur_messages += [dict(role="assistant", content=content)]
+
+    def update_files(self):
+        content = self.partial_response_content
+
+        # might raise ValueError for malformed ORIG/UPD blocks
+        edits = list(find_original_update_blocks(content))
+
+        edited = set()
+        for path, original, updated in edits:
+            full_path = self.allowed_to_edit(path)
+            if not full_path:
+                continue
+            if do_replace(full_path, original, updated, self.dry_run):
+                edited.add(path)
+                continue
+            self.io.tool_error(f"Failed to apply edit to {path}")
+
+        return edited
 
 
 def try_dotdotdots(whole, part, replace):
     """
     See if the edit block has ... lines.
     If not, return none.
 
@@ -63,15 +91,15 @@
     whole_lines = whole.splitlines()
     part_lines = part.splitlines()
     replace_lines = replace.splitlines()
 
     # If all lines in the part start with whitespace, then honor it.
     # But GPT often outdents the part and replace blocks completely,
     # thereby discarding the actual leading whitespace in the file.
-    if all(pline[0].isspace() for pline in part_lines):
+    if all((not pline or pline[0].isspace()) for pline in part_lines):
         return
 
     for i in range(len(whole_lines) - len(part_lines) + 1):
         leading_whitespace = ""
         for j, c in enumerate(whole_lines[i]):
             if c == part_lines[0][0]:
                 leading_whitespace = whole_lines[i][:j]
@@ -150,29 +178,14 @@
 
     if whole.endswith("\n"):
         modified_whole += "\n"
 
     return modified_whole
 
 
-def quoted_file(fname, display_fname, number=False):
-    prompt = "\n"
-    prompt += display_fname
-    prompt += "\n```\n"
-    file_content = Path(fname).read_text()
-    lines = file_content.splitlines()
-    for i, line in enumerate(lines, start=1):
-        if number:
-            prompt += f"{i:4d} "
-        prompt += line + "\n"
-
-    prompt += "```\n"
-    return prompt
-
-
 def strip_quoted_wrapping(res, fname=None):
     """
     Given an input string which may have extra "wrapping" around it, remove the wrapping.
     For example:
 
     filename.ext
     ```
@@ -219,25 +232,14 @@
 
     if not dry_run:
         fname.write_text(new_content)
 
     return True
 
 
-def show_messages(messages, title=None):
-    if title:
-        print(title.upper(), "*" * 50)
-
-    for msg in messages:
-        role = msg["role"].upper()
-        content = msg["content"].splitlines()
-        for line in content:
-            print(role, line)
-
-
 ORIGINAL = "<<<<<<< ORIGINAL"
 DIVIDER = "======="
 UPDATED = ">>>>>>> UPDATED"
 
 separators = "|".join([ORIGINAL, DIVIDER, UPDATED])
 
 split_re = re.compile(r"^((?:" + separators + r")[ ]*\n)", re.MULTILINE | re.DOTALL)
```

### Comparing `aider-chat-0.6.6/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.7.0/aider_chat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.6.6
+Version: 0.7.0
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
 
@@ -50,44 +50,14 @@
 * Request new features, changes, improvements, or bug fixes to your code. Ask for new test cases, updated documentation or code refactors.
 * Aider will apply the edits suggested by GPT directly to your source files.
 * Aider will automatically commit each changeset to your local git repo with a descriptive commit message. These frequent, automatic commits provide a safety net. It's easy to undo changes or use standard git workflows to manage longer sequences of changes.
 * You can use aider with multiple source files at once, so GPT can make coordinated code changes across all of them in a single changeset/commit.
 * Aider can [give *GPT-4* a map of your entire git repo](https://aider.chat/docs/ctags.html), which helps it understand and modify large codebases.
 * You can also edit files by hand using your editor while chatting with aider. Aider will notice these out-of-band edits and ask if you'd like to commit them. This lets you bounce back and forth between the aider chat and your editor, to collaboratively code with GPT.
 
-## GPT-4 vs GPT-3.5
-
-Aider supports all of OpenAI's chat models, including
-the the brand new `gpt-3.5-turbo-16k` model. 
-To use `gpt-3.5-turbo-16k`, install from GitHub per the instructions below and launch with `aider -3`.
-
-You will probably get the best results with one of the GPT-4 models,
-because of their large context windows,
-adherance to system prompt instructions and
-greater competance at coding tasks.
-The GPT-4 models are also able to use a
-[repository map](https://aider.chat/docs/ctags.html)
-to improve their ability to make changes in larger codebases.
-
-The GPT-3.5 models are supported more experimentally
-and are limited to editing somewhat smaller codebases.
-They are less able to follow instructions and
-aren't able to return code edits in a compact format.
-So aider has
-to ask GPT-3.5 to return a full copy of any code that needs to be edited.
-This rapidly uses up tokens and can hit the limits of the context window.
-In practice, this means you can only use `gpt-3.5-turbo` to edit files that are
-smaller than about 2k tokens (8k bytes).
-The new `gpt-3.5-turbo-16k` model should be able to edit code up to 8k tokens (32k bytes).
-
-Aider disables the
-[repository map feature](https://aider.chat/docs/ctags.html)
-when used with GPT-3.5 models.
-The `gpt-3.5-turbo` context window is too small to include a repo map.
-Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
 
 ## Installation
 
 1. Install the package:
   * PyPI: `pip install aider-chat`
   * GitHub: `pip install git+https://github.com/paul-gauthier/aider.git`
   * Local clone: `pip install -e .` 
@@ -102,48 +72,97 @@
 
 Run the `aider` tool by executing the following command:
 
 ```
 aider <file1> <file2> ...
 ```
 
-Replace `<file1>`, `<file2>`, etc., with the paths to the source code files you want to work on. These files will be added to the chat session.
+Replace `<file1>`, `<file2>`, etc., with the paths to the source code files you want to work on.
+These files will be "added to the chat session", so that GPT can see their contents and edit them according to your instructions.
 
 You can also just launch `aider` anywhere in a git repo without naming
 files on the command line.  It will discover all the files in the
 repo.  You can then add and remove individual files in the chat
 session with the `/add` and `/drop` chat commands described below.
 If you or GPT mention one of the repo's filenames in the conversation,
 aider will ask if you'd like to add it to the chat.
 
-You can also use additional command-line options, environment variables or configuration file
+Aider will work best if you think about which files need to be edited to make your change and add them to the chat.
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself.
+
+Aider also has many
+additional command-line options, environment variables or configuration file
 to set many options. See `aider --help` for details.
 
 ## In-chat commands
 
 Aider supports commands from within the chat, which all start with `/`. Here are some of the most useful in-chat commands:
 
 * `/add <file>`: Add matching files to the chat session.
 * `/drop <file>`: Remove matching files from the chat session.
 * `/undo`: Undo the last git commit if it was done by aider.
 * `/diff`: Display the diff of the last aider commit.
 * `/run <command>`: Run a shell command and optionally add the output to the chat.
 * `/help`: Show help about all commands.
 
+
 ## Tips
 
+* Think about which files need to be edited to make your change and add them to the chat.
+Aider has some ability to help GPT figure out which files to edit all by itself, but the most effective approach is to explicitly add the needed files to the chat yourself. 
 * Large changes are best performed as a sequence of thoughtful bite sized steps, where you plan out the approach and overall design. Walk GPT through changes like you might with a junior dev. Ask for a refactor to prepare, then ask for the actual change. Spend the time to ask for code quality/structure improvements.
 * Use Control-C to safely interrupt GPT if it isn't providing a useful response. The partial response remains in the conversation, so you can refer to it when you reply to GPT with more information or direction.
 * Use the `/run` command to run tests, linters, etc and show the output to GPT so it can fix any issues.
 * Enter a multiline chat message by entering `{` alone on the first line. End the multiline message with `}` alone on the last line.
 * If your code is throwing an error, share the error output with GPT using `/run` or by pasting it into the chat. Let GPT figure out and fix the bug.
 * GPT knows about a lot of standard tools and libraries, but may get some of the fine details wrong about APIs and function arguments. You can paste doc snippets into the chat to resolve these issues.
 * Aider will notice if you launch it on a git repo with uncommitted changes and offer to commit them before proceeding.
 * GPT can only see the content of the files you specifically "add to the chat". Aider also sends GPT-4 a [map of your entire git repo](https://aider.chat/docs/ctags.html). So GPT may ask to see additional files if it feels that's needed for your requests.
 * I also shared some general [GPT coding tips on Hacker News](https://news.ycombinator.com/item?id=36211879).
 
+## GPT-4 vs GPT-3.5
+
+Aider supports all of OpenAI's chat models, including
+the the brand new `gpt-3.5-turbo-16k` model. 
+
+You will probably get the best results with one of the GPT-4 models,
+because of their large context windows,
+adherance to system prompt instructions and
+greater competance at coding tasks.
+The GPT-4 models are able to structure code edits as simple "diffs"
+and use a
+[repository map](https://aider.chat/docs/ctags.html)
+to improve their ability to make changes in larger codebases.
+
+The GPT-3.5 models are supported more experimentally
+and are limited to editing somewhat smaller codebases.
+They are less able to follow instructions and
+aren't able to return code edits in a compact "diff" format.
+So aider has
+to ask GPT-3.5 to return a new copy of the "whole file" with edits included.
+This rapidly uses up tokens and can hit the limits of the context window.
+
+Aider disables the
+[repository map feature](https://aider.chat/docs/ctags.html)
+when used with GPT-3.5 models.
+The `gpt-3.5-turbo` context window is too small to include a repo map.
+Evaluation is still needed to determine if `gpt-3.5-turbo-16k` can make use of a repo map.
+
+In practice, this means you can use aider to edit a set of source files
+that total up to the sizes below.
+You can (and should) add just the specific set of files to the chat
+that are relevant to the change you are requesting.
+This minimizes your use of the context window, as well as costs.
+
+| Model             | Context<br>Size | Edit<br>Format | Max<br>File Size | Max<br>File Size | Repo<br>Map? |
+| ----------------- | -- | --     | -----| -- | -- |
+| gpt-3.5-turbo     |  4k tokens | whole file | 2k tokens | ~8k bytes | no |
+| gpt-3.5-turbo-16k | 16k tokens | whole file | 8k tokens | ~32k bytes | no |
+| gpt-4             |  8k tokens | diffs | 8k tokens | ~32k bytes | yes | 
+| gpt-4-32k         | 32k tokens | diffs | 32k tokens  | ~128k bytes | yes |
+
 ## Kind words from users
 
 * "Aider ... has easily quadrupled my coding productivity." -- [SOLAR_FIELDS](https://news.ycombinator.com/item?id=36212100)
 * "What an amazing tool. It's incredible." -- [valyagolev](https://github.com/paul-gauthier/aider/issues/6#issue-1722897858)
 * "It was WAY faster than I would be getting off the ground and making the first few working versions." -- [Daniel Feldman](https://twitter.com/d_feldman/status/1662295077387923456)
```

### Comparing `aider-chat-0.6.6/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.7.0/aider_chat.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 aider/__init__.py
-aider/coder.py
 aider/commands.py
 aider/diffs.py
 aider/dump.py
 aider/io.py
 aider/main.py
 aider/models.py
 aider/prompts.py
 aider/repomap.py
 aider/utils.py
+aider/coders/__init__.py
+aider/coders/base_coder.py
+aider/coders/base_prompts.py
+aider/coders/editblock_coder.py
+aider/coders/editblock_prompts.py
+aider/coders/wholefile_coder.py
+aider/coders/wholefile_func_coder.py
+aider/coders/wholefile_func_prompts.py
+aider/coders/wholefile_prompts.py
 aider_chat.egg-info/PKG-INFO
 aider_chat.egg-info/SOURCES.txt
 aider_chat.egg-info/dependency_links.txt
 aider_chat.egg-info/entry_points.txt
 aider_chat.egg-info/requires.txt
 aider_chat.egg-info/top_level.txt
 tests/__init__.py
 tests/test_coder.py
 tests/test_commands.py
+tests/test_editblock.py
 tests/test_io.py
 tests/test_main.py
+tests/test_models.py
 tests/test_repomap.py
-tests/test_utils.py
+tests/test_wholefile.py
```

### Comparing `aider-chat-0.6.6/setup.py` & `aider-chat-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.6/tests/test_coder.py` & `aider-chat-0.7.0/tests/test_coder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import unittest
 from unittest.mock import MagicMock, patch
 
 import openai
 import requests
 
-from aider.coder import Coder
+from aider import models
+from aider.coders import Coder
 
 
 class TestCoder(unittest.TestCase):
     def setUp(self):
-        self.patcher = patch("aider.coder.Coder.check_model_availability")
+        self.patcher = patch("aider.coders.base_coder.check_model_availability")
         self.mock_check = self.patcher.start()
         self.mock_check.return_value = True
 
     def tearDown(self):
         self.patcher.stop()
 
     def test_check_for_file_mentions(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Mock the git repo
         mock_repo = MagicMock()
         mock_repo.git.ls_files.return_value = "file1.txt\nfile2.py"
         coder.repo = mock_repo
 
         # Call the check_for_file_mentions method
@@ -37,15 +38,15 @@
         self.assertEqual(coder.abs_fnames, expected_files)
 
     def test_check_for_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Mock the git repo
         mock_repo = MagicMock()
         mock_repo.git.ls_files.return_value = "./file1.txt\n./file2.py"
         coder.repo = mock_repo
 
         # Call the check_for_file_mentions method
@@ -56,15 +57,15 @@
         self.assertEqual(coder.abs_fnames, expected_files)
 
     def test_check_for_ambiguous_filename_mentions_of_longer_paths(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Mock the git repo
         mock_repo = MagicMock()
         mock_repo.git.ls_files.return_value = "./file1.txt\n./other/file1.txt"
         coder.repo = mock_repo
 
         # Call the check_for_file_mentions method
@@ -73,97 +74,109 @@
         self.assertEqual(coder.abs_fnames, set())
 
     def test_get_commit_message(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
-        # Mock the send method to return a tuple with a message and False
-        coder.send = MagicMock(return_value=("a good commit message", False))
+        # Mock the send method to set partial_response_content and return False
+        def mock_send(*args, **kwargs):
+            coder.partial_response_content = "a good commit message"
+            return False
+
+        coder.send = MagicMock(side_effect=mock_send)
 
         # Call the get_commit_message method with dummy diff and context
         result = coder.get_commit_message("dummy diff", "dummy context")
 
         # Assert that the returned message is the expected one
         self.assertEqual(result, "a good commit message")
 
     def test_get_commit_message_strip_quotes(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+
+        # Mock the send method to set partial_response_content and return False
+        def mock_send(*args, **kwargs):
+            coder.partial_response_content = "a good commit message"
+            return False
 
-        # Mock the send method to return a tuple with a message and False
-        coder.send = MagicMock(return_value=('"a good commit message"', False))
+        coder.send = MagicMock(side_effect=mock_send)
 
         # Call the get_commit_message method with dummy diff and context
         result = coder.get_commit_message("dummy diff", "dummy context")
 
         # Assert that the returned message is the expected one
         self.assertEqual(result, "a good commit message")
 
     def test_get_commit_message_no_strip_unmatched_quotes(self):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
+
+        # Mock the send method to set partial_response_content and return False
+        def mock_send(*args, **kwargs):
+            coder.partial_response_content = 'a good "commit message"'
+            return False
 
-        # Mock the send method to return a tuple with a message and False
-        coder.send = MagicMock(return_value=('a good "commit message"', False))
+        coder.send = MagicMock(side_effect=mock_send)
 
         # Call the get_commit_message method with dummy diff and context
         result = coder.get_commit_message("dummy diff", "dummy context")
 
         # Assert that the returned message is the expected one
         self.assertEqual(result, 'a good "commit message"')
 
-    @patch("aider.coder.openai.ChatCompletion.create")
+    @patch("aider.coders.base_coder.openai.ChatCompletion.create")
     @patch("builtins.print")
     def test_send_with_retries_rate_limit_error(self, mock_print, mock_chat_completion_create):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Set up the mock to raise RateLimitError on
         # the first call and return None on the second call
         mock_chat_completion_create.side_effect = [
             openai.error.RateLimitError("Rate limit exceeded"),
             None,
         ]
 
         # Call the send_with_retries method
-        coder.send_with_retries("model", ["message"])
+        coder.send_with_retries("model", ["message"], None)
 
         # Assert that print was called once
         mock_print.assert_called_once()
 
-    @patch("aider.coder.openai.ChatCompletion.create")
+    @patch("aider.coders.base_coder.openai.ChatCompletion.create")
     @patch("builtins.print")
     def test_send_with_retries_connection_error(self, mock_print, mock_chat_completion_create):
         # Mock the IO object
         mock_io = MagicMock()
 
         # Initialize the Coder object with the mocked IO and mocked repo
-        coder = Coder(io=mock_io, openai_api_key="fake_key")
+        coder = Coder.create(models.GPT4, None, mock_io, openai_api_key="fake_key")
 
         # Set up the mock to raise ConnectionError on the first call
         # and return None on the second call
         mock_chat_completion_create.side_effect = [
             requests.exceptions.ConnectionError("Connection error"),
             None,
         ]
 
         # Call the send_with_retries method
-        coder.send_with_retries("model", ["message"])
+        coder.send_with_retries("model", ["message"], None)
 
         # Assert that print was called once
         mock_print.assert_called_once()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aider-chat-0.6.6/tests/test_commands.py` & `aider-chat-0.7.0/tests/test_commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 import os
 import shutil
 import tempfile
 from unittest import TestCase
-from unittest.mock import patch
 
+from aider import models
 from aider.commands import Commands
 from aider.io import InputOutput
 
 
 class TestCommands(TestCase):
     def setUp(self):
         self.original_cwd = os.getcwd()
         self.tempdir = tempfile.mkdtemp()
         os.chdir(self.tempdir)
 
-        self.patcher = patch("aider.coder.Coder.check_model_availability")
-        self.mock_check = self.patcher.start()
-        self.mock_check.return_value = True
-
     def tearDown(self):
         os.chdir(self.original_cwd)
         shutil.rmtree(self.tempdir)
 
-        self.patcher.stop()
-
     def test_cmd_add(self):
         # Initialize the Commands and InputOutput objects
         io = InputOutput(pretty=False, yes=True)
-        from aider.coder import Coder
+        from aider.coders import Coder
 
-        coder = Coder(io, openai_api_key="deadbeef")
+        coder = Coder.create(models.GPT35, None, io, openai_api_key="deadbeef")
         commands = Commands(io, coder)
 
         # Call the cmd_add method with 'foo.txt' and 'bar.txt' as a single string
         commands.cmd_add("foo.txt bar.txt")
 
         # Check if both files have been created in the temporary directory
         self.assertTrue(os.path.exists("foo.txt"))
```

### Comparing `aider-chat-0.6.6/tests/test_main.py` & `aider-chat-0.7.0/tests/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class TestMain(TestCase):
     def setUp(self):
         os.environ["OPENAI_API_KEY"] = "deadbeef"
         self.original_cwd = os.getcwd()
         self.tempdir = tempfile.mkdtemp()
         os.chdir(self.tempdir)
-        self.patcher = patch("aider.main.Coder.check_model_availability")
+        self.patcher = patch("aider.coders.base_coder.check_model_availability")
         self.mock_check = self.patcher.start()
         self.mock_check.return_value = True
 
     def tearDown(self):
         os.chdir(self.original_cwd)
         shutil.rmtree(self.tempdir)
         self.patcher.stop()
@@ -44,43 +44,43 @@
         subprocess.run(["git", "config", "user.name", "Dummy User"])
         pipe_input = create_input(StringIO(""))
         main(["--yes", "foo.txt"], input=pipe_input, output=DummyOutput())
         pipe_input.close()
         self.assertTrue(os.path.exists("foo.txt"))
 
     def test_main_args(self):
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main(["--no-auto-commits"])
             _, kwargs = MockCoder.call_args
             assert kwargs["auto_commits"] is False
 
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main(["--auto-commits"])
             _, kwargs = MockCoder.call_args
             assert kwargs["auto_commits"] is True
 
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main([])
             _, kwargs = MockCoder.call_args
             assert kwargs["dirty_commits"] is True
             assert kwargs["auto_commits"] is True
             assert kwargs["pretty"] is True
 
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main(["--no-pretty"])
             _, kwargs = MockCoder.call_args
             assert kwargs["pretty"] is False
 
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main(["--pretty"])
             _, kwargs = MockCoder.call_args
             assert kwargs["pretty"] is True
 
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main(["--no-dirty-commits"])
             _, kwargs = MockCoder.call_args
             assert kwargs["dirty_commits"] is False
 
-        with patch("aider.main.Coder") as MockCoder:
+        with patch("aider.main.Coder.create") as MockCoder:
             main(["--dirty-commits"])
             _, kwargs = MockCoder.call_args
             assert kwargs["dirty_commits"] is True
```

### Comparing `aider-chat-0.6.6/tests/test_repomap.py` & `aider-chat-0.7.0/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.6/tests/test_utils.py` & `aider-chat-0.7.0/tests/test_editblock.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # flake8: noqa: E501
 
 import unittest
 
-from aider import utils
+from aider.coders import editblock_coder as eb
 
 
 class TestUtils(unittest.TestCase):
     def test_replace_most_similar_chunk(self):
         whole = "This is a sample text.\nAnother line of text.\nYet another line.\n"
         part = "This is a sample text"
         replace = "This is a replaced text."
         expected_output = "This is a replaced text..\nAnother line of text.\nYet another line.\n"
 
-        result = utils.replace_most_similar_chunk(whole, part, replace)
+        result = eb.replace_most_similar_chunk(whole, part, replace)
         self.assertEqual(result, expected_output)
 
     def test_replace_most_similar_chunk_not_perfect_match(self):
         whole = "This is a sample text.\nAnother line of text.\nYet another line."
         part = "This was a sample text.\nAnother line of txt"
         replace = "This is a replaced text.\nModified line of text."
         expected_output = "This is a replaced text.\nModified line of text.\nYet another line."
 
-        result = utils.replace_most_similar_chunk(whole, part, replace)
+        result = eb.replace_most_similar_chunk(whole, part, replace)
         self.assertEqual(result, expected_output)
 
     def test_strip_quoted_wrapping(self):
         input_text = (
             "filename.ext\n```\nWe just want this content\nNot the filename and triple quotes\n```"
         )
         expected_output = "We just want this content\nNot the filename and triple quotes\n"
-        result = utils.strip_quoted_wrapping(input_text, "filename.ext")
+        result = eb.strip_quoted_wrapping(input_text, "filename.ext")
         self.assertEqual(result, expected_output)
 
     def test_strip_quoted_wrapping_no_filename(self):
         input_text = "```\nWe just want this content\nNot the triple quotes\n```"
         expected_output = "We just want this content\nNot the triple quotes\n"
-        result = utils.strip_quoted_wrapping(input_text)
+        result = eb.strip_quoted_wrapping(input_text)
         self.assertEqual(result, expected_output)
 
     def test_strip_quoted_wrapping_no_wrapping(self):
         input_text = "We just want this content\nNot the triple quotes\n"
         expected_output = "We just want this content\nNot the triple quotes\n"
-        result = utils.strip_quoted_wrapping(input_text)
+        result = eb.strip_quoted_wrapping(input_text)
         self.assertEqual(result, expected_output)
 
     def test_find_original_update_blocks(self):
         edit = """
 Here's the change:
 
 ```text
@@ -56,15 +56,15 @@
 Tooooo
 >>>>>>> UPDATED
 ```
 
 Hope you like it!
 """
 
-        edits = list(utils.find_original_update_blocks(edit))
+        edits = list(eb.find_original_update_blocks(edit))
         self.assertEqual(edits, [("foo.txt", "Two\n", "Tooooo\n")])
 
     def test_find_original_update_blocks_quote_below_filename(self):
         edit = """
 Here's the change:
 
 foo.txt
@@ -75,15 +75,15 @@
 Tooooo
 >>>>>>> UPDATED
 ```
 
 Hope you like it!
 """
 
-        edits = list(utils.find_original_update_blocks(edit))
+        edits = list(eb.find_original_update_blocks(edit))
         self.assertEqual(edits, [("foo.txt", "Two\n", "Tooooo\n")])
 
     def test_find_original_update_blocks_unclosed(self):
         edit = """
 Here's the change:
 
 ```text
@@ -94,15 +94,15 @@
 Tooooo
 
 
 oops!
 """
 
         with self.assertRaises(ValueError) as cm:
-            list(utils.find_original_update_blocks(edit))
+            list(eb.find_original_update_blocks(edit))
         self.assertIn("Incomplete", str(cm.exception))
 
     def test_find_original_update_blocks_missing_filename(self):
         edit = """
 Here's the change:
 
 ```text
@@ -112,15 +112,15 @@
 Tooooo
 
 
 oops!
 """
 
         with self.assertRaises(ValueError) as cm:
-            list(utils.find_original_update_blocks(edit))
+            list(eb.find_original_update_blocks(edit))
         self.assertIn("filename", str(cm.exception))
 
     def test_find_original_update_blocks_no_final_newline(self):
         edit = """
 aider/coder.py
 <<<<<<< ORIGINAL
             self.console.print("[red]^C again to quit")
@@ -148,15 +148,15 @@
 <<<<<<< ORIGINAL
             self.console.print("[red]Skipped commmit.")
 =======
             self.io.tool_error("Skipped commmit.")
 >>>>>>> UPDATED"""
 
         # Should not raise a ValueError
-        list(utils.find_original_update_blocks(edit))
+        list(eb.find_original_update_blocks(edit))
 
     def test_incomplete_edit_block_missing_filename(self):
         edit = """
 No problem! Here are the changes to patch `subprocess.check_output` instead of `subprocess.run` in both tests:
 
 ```python
 tests/test_repomap.py
@@ -191,24 +191,38 @@
   "kind": "variable"
 }'''
 >>>>>>> UPDATED
 ```
 
 These changes replace the `subprocess.run` patches with `subprocess.check_output` patches in both `test_check_for_ctags_failure` and `test_check_for_ctags_success` tests.
 """
-        edit_blocks = list(utils.find_original_update_blocks(edit))
+        edit_blocks = list(eb.find_original_update_blocks(edit))
         self.assertEqual(len(edit_blocks), 2)  # 2 edits
         self.assertEqual(edit_blocks[0][0], "tests/test_repomap.py")
         self.assertEqual(edit_blocks[1][0], "tests/test_repomap.py")
 
-
     def test_replace_part_with_missing_leading_whitespace(self):
         whole = "    line1\n    line2\n    line3\n"
         part = "line1\nline2"
         replace = "new_line1\nnew_line2"
         expected_output = "    new_line1\n    new_line2\n    line3\n"
 
-        result = utils.replace_part_with_missing_leading_whitespace(whole, part, replace)
+        result = eb.replace_part_with_missing_leading_whitespace(whole, part, replace)
         self.assertEqual(result, expected_output)
 
+    def test_replace_part_with_missing_leading_whitespace_including_blank_lines(self):
+        """
+        The part has leading whitespace on all lines, so should be ignored.
+        But it has a *blank* line with no whitespace at all, which was causing a
+        bug per issue #25. Test case to repro and confirm fix.
+        """
+        whole = "    line1\n    line2\n    line3\n"
+        part = "\n  line1\n  line2"
+        replace = "new_line1\nnew_line2"
+        expected_output = None
+
+        result = eb.replace_part_with_missing_leading_whitespace(whole, part, replace)
+        self.assertEqual(result, expected_output)
+
+
 if __name__ == "__main__":
     unittest.main()
```

