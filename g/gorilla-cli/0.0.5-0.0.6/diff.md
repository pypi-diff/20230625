# Comparing `tmp/gorilla-cli-0.0.5.tar.gz` & `tmp/gorilla-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gorilla-cli-0.0.5.tar", last modified: Tue Jun 20 08:41:20 2023, max compression
+gzip compressed data, was "gorilla-cli-0.0.6.tar", last modified: Sun Jun 25 09:10:16 2023, max compression
```

## Comparing `gorilla-cli-0.0.5.tar` & `gorilla-cli-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.366309 gorilla-cli-0.0.5/
--rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/LICENSE
--rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-20 08:41:20.366065 gorilla-cli-0.0.5/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)     1656 2023-06-17 09:55:31.000000 gorilla-cli-0.0.5/README.md
--rw-r--r--   0 shishir    (501) staff       (20)     4301 2023-06-20 08:34:03.000000 gorilla-cli-0.0.5/go_cli.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.362827 gorilla-cli-0.0.5/go_questionary/
--rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/constants.py
--rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/form.py
--rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompt.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.365176 gorilla-cli-0.0.5/go_questionary/prompts/
--rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/autocomplete.py
--rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/checkbox.py
--rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/common.py
--rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/confirm.py
--rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/password.py
--rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/path.py
--rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/rawselect.py
--rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/select.py
--rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/prompts/text.py
--rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/question.py
--rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/utils.py
--rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-17 09:51:12.000000 gorilla-cli-0.0.5/go_questionary/version.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-20 08:41:20.365887 gorilla-cli-0.0.5/gorilla_cli.egg-info/
--rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/SOURCES.txt
--rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/dependency_links.txt
--rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/entry_points.txt
--rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/requires.txt
--rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-20 08:41:20.000000 gorilla-cli-0.0.5/gorilla_cli.egg-info/top_level.txt
--rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-20 08:41:20.366351 gorilla-cli-0.0.5/setup.cfg
--rw-r--r--   0 shishir    (501) staff       (20)     1502 2023-06-20 08:32:13.000000 gorilla-cli-0.0.5/setup.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.242728 gorilla-cli-0.0.6/
+-rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/LICENSE
+-rw-r--r--   0 shishir    (501) staff       (20)     2420 2023-06-25 09:10:16.242452 gorilla-cli-0.0.6/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)     1914 2023-06-25 09:09:40.000000 gorilla-cli-0.0.6/README.md
+-rw-r--r--   0 shishir    (501) staff       (20)     6755 2023-06-25 08:59:47.000000 gorilla-cli-0.0.6/go_cli.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.239848 gorilla-cli-0.0.6/go_questionary/
+-rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/constants.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/form.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompt.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.241428 gorilla-cli-0.0.6/go_questionary/prompts/
+-rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/autocomplete.py
+-rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/checkbox.py
+-rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/common.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/confirm.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/password.py
+-rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/path.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/rawselect.py
+-rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/select.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/prompts/text.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/question.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/utils.py
+-rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.6/go_questionary/version.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-25 09:10:16.242235 gorilla-cli-0.0.6/gorilla_cli.egg-info/
+-rw-r--r--   0 shishir    (501) staff       (20)     2420 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/entry_points.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/requires.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-25 09:10:16.000000 gorilla-cli-0.0.6/gorilla_cli.egg-info/top_level.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-25 09:10:16.242780 gorilla-cli-0.0.6/setup.cfg
+-rw-r--r--   0 shishir    (501) staff       (20)     1502 2023-06-25 01:01:09.000000 gorilla-cli-0.0.6/setup.py
```

### Comparing `gorilla-cli-0.0.5/LICENSE` & `gorilla-cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/PKG-INFO` & `gorilla-cli-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,46 @@
-Metadata-Version: 2.1
-Name: gorilla-cli
-Version: 0.0.5
-Summary: LLMs for CLI
-Home-page: https://github.com/gorilla-llm/gorilla-cli
-Author: Shishir Patil, Tianjun Zhang
-Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Gorilla CLI
 
-Gorilla CLI is a user-friendly command-line interface (CLI) tool that helps you to interact with your system using natural language. Just tell Gorilla CLI what you want to do, and it will suggest possible commands for you. No need to memorize complex command line arguments!
+Gorilla CLI revolutionizes your command-line interactions with a user-centric tool that understands natural language commands. Simply state your objective, and Gorilla CLI will generate potential commands for execution. No more need to recall intricate command-line arguments!
+
+Developed by UC Berkeley as a research prototype, Gorilla-CLI prioritizes user control and confidentiality:
+ - Commands are executed solely with your explicit approval.
+ - While we utilize queries and error logs (stderr) for model enhancement, we NEVER collect output data (stdout).
 
-## Get Started
+## Getting Started
 
-Gorilla CLI can be installed via pip. 
+You can readily install Gorilla CLI via pip. 
 
 ```bash
 pip install gorilla-cli
 ```
 
 ## Usage
 
-Using Gorilla CLI is as simple as typing `go` followed by your command in plain English.
+Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
 
-For example, if you want to list all files in the current directory, simply type:
+For instance, to list all files in the current directory, type:
 
 ```bash
-$go I want to list all files in the current directory
+$ go I want to list all files in the current directory
 ```
 
-Gorilla CLI will then suggest possible commands, which you can select using the arrow keys and then press enter to execute the command. 
+Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
    ls -l
    ls -al
 ```
 
 ## How It Works
 
-Gorilla CLI is tool that combines the power of [Gorilla LLM](https://github.com/ShishirPatil/gorilla/), and other LLMs including OpenAI's GPT-4, Claude v1, to provide a user-friendly interface to the command line. You can now tell your command line what task you want it to execute, and it then presents a few possible commands for you to choose from and execute.
-
-Gorilla will NOT execute any command without the user explicitly executing it themselves.
+Gorilla-CLI fuses the capabilities of various Language Learning Models (LLMs) like [Gorilla LLM](https://github.com/ShishirPatil/gorilla/), OpenAI's GPT-4, Claude v1, and others to present a user-friendly command-line interface. For each user query, we gather responses from all contributing LLMs, filter, sort, and present you with the most relevant options. 
 
 ## Contributions
 
-Contributions to Gorilla CLI are welcome. Please submit a pull request on GitHub if you have made improvements to the tool. 
+We welcome your enhancements to Gorilla CLI! If you have improvements, feel free to submit a pull request on our GitHub page. 
 
 ## License
 
-Gorilla CLI is licensed under the Apache 2.0 license. See the LICENSE file for more details. Thanks to [questionary](https://github.com/tmbo/questionary) for the great UI! 
-
-
+Gorilla CLI operates under the Apache 2.0 license. More details can be found in the LICENSE file. We'd also like to extend our appreciation to [questionary](https://github.com/tmbo/questionary) for their fantastic UI!
```

### Comparing `gorilla-cli-0.0.5/go_cli.py` & `gorilla-cli-0.0.6/go_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,125 +14,163 @@
 
 import datetime
 import os
 import sys
 import uuid
 import requests
 import subprocess
+import urllib.parse
 import sys
 from halo import Halo
 import go_questionary
 
+__version__ = "0.0.6"  # current version
 SERVER_URL = "http://34.135.112.197:8000"
-__version__ = "0.0.5"  # current version
-UPDATE_CHECK_FILE = os.path.expanduser(
-    "~/.gorilla-cli-last-update-check"
-)
+UPDATE_CHECK_FILE = os.path.expanduser("~/.gorilla-cli-last-update-check")
+USERID_FILE = os.path.expanduser("~/.gorilla-cli-userid")
+ISSUE_URL = f"https://github.com/gorilla-llm/gorilla-cli/issues/new"
+WELCOME_TEXT = """🦍 Welcome to Gorilla-CLI! Enhance your Command Line with the power of LLMs! 
+
+Simply use `go <your desired operation>` and Gorilla will do the rest. For instance:
+    go what is the path of my current directory
+    go list all my GCP instances
+
+Created as a research prototype by UC Berkeley, Gorilla-CLI ensures user control and privacy:
+ - Commands are executed only with explicit user approval.
+ - While queries and error (stderr) logs are used to refine our model, we NEVER gather output (stdout) data.
+
+Visit us at github.com/gorilla-llm/gorilla-cli and start talking to your CLI!"""
 
 
 def check_for_updates():
+    # Check if a new version of gorilla-cli is available once a day
     try:
         with open(UPDATE_CHECK_FILE, "r") as f:
-            last_check_date = datetime.datetime.strptime(
-                f.read(), "%Y-%m-%d"
-            )
+            last_check_date = datetime.datetime.strptime(f.read(), "%Y-%m-%d")
     except FileNotFoundError:
-        last_check_date = (
-            datetime.datetime.now() - datetime.timedelta(days=1)
-        )
-
-    if (
-        datetime.datetime.now() - last_check_date
-        >= datetime.timedelta(days=1)
-    ):
+        last_check_date = datetime.datetime.now() - datetime.timedelta(days=1)
+    if datetime.datetime.now() - last_check_date >= datetime.timedelta(days=1):
         try:
-            response = requests.get(
-                "https://pypi.org/pypi/gorilla-cli/json"
-            )
+            response = requests.get("https://pypi.org/pypi/gorilla-cli/json")
             latest_version = response.json()["info"]["version"]
 
             if latest_version > __version__:
-                print(
-                    f"A new version of gorilla-cli is available: {latest_version}"
-                )
+                print(f"A new version of gorilla-cli is available: {latest_version}")
         except Exception as e:
             print("Unable to check for updates:", e)
-
         try:
             with open(UPDATE_CHECK_FILE, "w") as f:
                 f.write(datetime.datetime.now().strftime("%Y-%m-%d"))
         except Exception as e:
             print("Unable to write update check file:", e)
 
 
+def get_user_id():
+    # Unique user identifier for authentication and load balancing
+    # Gorilla-CLI is hosted by UC Berkeley Sky lab for FREE as a
+    #  research prototype. Please don't spam the system or use it
+    #  for commercial serving. If you would like to request rate
+    #  limit increases for your GitHub handle, please raise an issue.
+    try:
+        with open(USERID_FILE, "r") as f:
+            user_id = str(f.read())
+            assert user_id != ""
+        return user_id
+    except FileNotFoundError:
+        try:
+            user_id = (
+                subprocess.check_output(["git", "config", "--global", "user.email"])
+                .decode("utf-8")
+                .strip()
+            )
+            print(WELCOME_TEXT)
+            response = (
+                input(f"Use your Github handle ({user_id}) as user id? [Y/n]: ")
+                .strip()
+                .lower()
+            )
+            if response in ["n", "no"]:
+                user_id = str(uuid.uuid4())
+        except Exception as e:
+            issue_title = urllib.parse.quote(
+                f"Problem with generating userid: {str(e)}"
+            )
+            issue_body = urllib.parse.quote(f"Unable to generate userid: {str(e)}")
+            print("Unable to generate userid:", e)
+            print(
+                f"Please run 'go <command>' again. If the problem persists, please raise an issue: \
+                  {ISSUE_URL}?title={issue_title}&body={issue_body}"
+            )
+        try:
+            with open(USERID_FILE, "w") as f:
+                f.write(user_id)
+            return user_id
+        except Exception as e:
+            issue_title = urllib.parse.quote("Problem with userid file")
+            issue_body = urllib.parse.quote(f"Unable to write userid file: {str(e)}")
+            print("Unable to write userid file:", e)
+            print(
+                f"Try deleting USERID_FILE and run 'go <command>' again. If the problem persists, please raise an issue:\
+                   {ISSUE_URL}?title={issue_title}&body={issue_body}"
+            )
+
+
 def main():
     def execute_command(cmd):
-        process = subprocess.run(cmd, shell=True)
-        return process.returncode
+        process = subprocess.run(cmd, shell=True, stderr=subprocess.PIPE)
+        error_msg = process.stderr.decode("utf-8")
+        if error_msg:
+            print(f"{error_msg}")
+            return error_msg
+        return str(process.returncode)
 
     args = sys.argv[1:]
     user_input = " ".join(args)
+    user_id = get_user_id()
 
-    # Unique user identifier for authentication and load balancing
-    # Gorilla-CLI is hosted by UC Berkeley Sky lab for FREE as a 
-    #  research prototype. Please don't spam the system or use it
-    #  for commercial serving. If you would like to request rate
-    #  limit increases for your GitHub handle, please raise an issue.
-    try:
-        user_id = (
-            subprocess.check_output(
-                ["git", "config", "--global", "user.email"]
-            )
-            .decode("utf-8")
-            .strip()
-        )
-    except Exception:
-        user_id = str(uuid.uuid4())
+    # Generate a unique interaction ID
+    interaction_id = str(uuid.uuid4())
 
     with Halo(text="🦍 Loading", spinner="dots"):
         try:
             data_json = {
                 "user_id": user_id,
                 "user_input": user_input,
+                "interaction_id": interaction_id,
             }
             response = requests.post(
                 f"{SERVER_URL}/commands", json=data_json, timeout=30
             )
             commands = response.json()
         except requests.exceptions.RequestException as e:
             print("Server is unreachable.")
-            print(
-                "Try updating Gorilla-CLI with 'pip install --upgrade gorilla-cli'"
-            )
+            print("Try updating Gorilla-CLI with 'pip install --upgrade gorilla-cli'")
             return
 
     check_for_updates()
 
     if commands:
         selected_command = go_questionary.select(
             "", choices=commands, instruction=""
         ).ask()
-        exit_code = execute_command(selected_command)
+        exit_condition = execute_command(selected_command)
 
         # Commands failed / succeeded?
         try:
             response = requests.post(
                 f"{SERVER_URL}/command-execution-result",
                 json={
                     "user_id": user_id,
                     "command": selected_command,
-                    "exit_code": exit_code,
+                    "exit_condition": exit_condition,
+                    "interaction_id": interaction_id,
                 },
                 timeout=30,
             )
             if response.status_code != 200:
-                print(
-                    "Failed to send command execution result to the server."
-                )
+                print("Failed to send command execution result to the server.")
         except requests.exceptions.Timeout:
-            print(
-                "Failed to send command execution result to the server: Timeout."
-            )
+            print("Failed to send command execution result to the server: Timeout.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gorilla-cli-0.0.5/go_questionary/__init__.py` & `gorilla-cli-0.0.6/go_questionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/constants.py` & `gorilla-cli-0.0.6/go_questionary/constants.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/form.py` & `gorilla-cli-0.0.6/go_questionary/form.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompt.py` & `gorilla-cli-0.0.6/go_questionary/prompt.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/__init__.py` & `gorilla-cli-0.0.6/go_questionary/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/autocomplete.py` & `gorilla-cli-0.0.6/go_questionary/prompts/autocomplete.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/checkbox.py` & `gorilla-cli-0.0.6/go_questionary/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/common.py` & `gorilla-cli-0.0.6/go_questionary/prompts/common.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/confirm.py` & `gorilla-cli-0.0.6/go_questionary/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/password.py` & `gorilla-cli-0.0.6/go_questionary/prompts/password.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/path.py` & `gorilla-cli-0.0.6/go_questionary/prompts/path.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/rawselect.py` & `gorilla-cli-0.0.6/go_questionary/prompts/rawselect.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/select.py` & `gorilla-cli-0.0.6/go_questionary/prompts/select.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/prompts/text.py` & `gorilla-cli-0.0.6/go_questionary/prompts/text.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/question.py` & `gorilla-cli-0.0.6/go_questionary/question.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/go_questionary/utils.py` & `gorilla-cli-0.0.6/go_questionary/utils.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/gorilla_cli.egg-info/PKG-INFO` & `gorilla-cli-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gorilla-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: LLMs for CLI
 Home-page: https://github.com/gorilla-llm/gorilla-cli
 Author: Shishir Patil, Tianjun Zhang
 Author-email: sgp@berkeley.edu, tianjunz@berkeley.edu
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,51 +12,53 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gorilla CLI
 
-Gorilla CLI is a user-friendly command-line interface (CLI) tool that helps you to interact with your system using natural language. Just tell Gorilla CLI what you want to do, and it will suggest possible commands for you. No need to memorize complex command line arguments!
+Gorilla CLI revolutionizes your command-line interactions with a user-centric tool that understands natural language commands. Simply state your objective, and Gorilla CLI will generate potential commands for execution. No more need to recall intricate command-line arguments!
 
-## Get Started
+Developed by UC Berkeley as a research prototype, Gorilla-CLI prioritizes user control and confidentiality:
+ - Commands are executed solely with your explicit approval.
+ - While we utilize queries and error logs (stderr) for model enhancement, we NEVER collect output data (stdout).
 
-Gorilla CLI can be installed via pip. 
+## Getting Started
+
+You can readily install Gorilla CLI via pip. 
 
 ```bash
 pip install gorilla-cli
 ```
 
 ## Usage
 
-Using Gorilla CLI is as simple as typing `go` followed by your command in plain English.
+Activate Gorilla CLI with a straightforward `go` followed by your command in plain English.
 
-For example, if you want to list all files in the current directory, simply type:
+For instance, to list all files in the current directory, type:
 
 ```bash
-$go I want to list all files in the current directory
+$ go I want to list all files in the current directory
 ```
 
-Gorilla CLI will then suggest possible commands, which you can select using the arrow keys and then press enter to execute the command. 
+Gorilla CLI will then generate potential commands. Simply use the arrow keys to navigate through the options, then press enter to execute the chosen command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
    ls -l
    ls -al
 ```
 
 ## How It Works
 
-Gorilla CLI is tool that combines the power of [Gorilla LLM](https://github.com/ShishirPatil/gorilla/), and other LLMs including OpenAI's GPT-4, Claude v1, to provide a user-friendly interface to the command line. You can now tell your command line what task you want it to execute, and it then presents a few possible commands for you to choose from and execute.
-
-Gorilla will NOT execute any command without the user explicitly executing it themselves.
+Gorilla-CLI fuses the capabilities of various Language Learning Models (LLMs) like [Gorilla LLM](https://github.com/ShishirPatil/gorilla/), OpenAI's GPT-4, Claude v1, and others to present a user-friendly command-line interface. For each user query, we gather responses from all contributing LLMs, filter, sort, and present you with the most relevant options. 
 
 ## Contributions
 
-Contributions to Gorilla CLI are welcome. Please submit a pull request on GitHub if you have made improvements to the tool. 
+We welcome your enhancements to Gorilla CLI! If you have improvements, feel free to submit a pull request on our GitHub page. 
 
 ## License
 
-Gorilla CLI is licensed under the Apache 2.0 license. See the LICENSE file for more details. Thanks to [questionary](https://github.com/tmbo/questionary) for the great UI! 
+Gorilla CLI operates under the Apache 2.0 license. More details can be found in the LICENSE file. We'd also like to extend our appreciation to [questionary](https://github.com/tmbo/questionary) for their fantastic UI!
```

### Comparing `gorilla-cli-0.0.5/gorilla_cli.egg-info/SOURCES.txt` & `gorilla-cli-0.0.6/gorilla_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.5/setup.py` & `gorilla-cli-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name="gorilla-cli",
-    version="0.0.5",
+    version="0.0.6",
     url="https://github.com/gorilla-llm/gorilla-cli",
     author="Shishir Patil, Tianjun Zhang",
     author_email="sgp@berkeley.edu, tianjunz@berkeley.edu",
     description="LLMs for CLI",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     py_modules=["go_cli"],
```

