# Comparing `tmp/aissist-0.0.6.tar.gz` & `tmp/aissist-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissist-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aissist-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aissist-0.0.6.tar` & `aissist-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.6/LICENSE
--rw-r--r--   0        0        0      212 2023-06-25 03:44:03.985612 aissist-0.0.6/Pipfile
--rw-r--r--   0        0        0    41743 2023-06-25 03:44:08.209610 aissist-0.0.6/Pipfile.lock
--rw-r--r--   0        0        0     1342 2023-06-25 03:52:36.697190 aissist-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.6/aissist/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-25 03:38:07.089502 aissist-0.0.6/aissist/aissistant.py
--rw-r--r--   0        0        0      740 2023-06-25 03:22:17.259413 aissist-0.0.6/aissist/spinner.py
--rw-r--r--   0        0        0       22 2023-06-25 03:53:01.265161 aissist-0.0.6/aissist/version.py
--rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.6/images/screenshot.png
--rw-r--r--   0        0        0      899 2023-06-25 03:52:49.025175 aissist-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 aissist-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        6 2023-06-25 02:49:07.991665 aissist-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2023-06-22 03:54:21.530635 aissist-0.0.7/LICENSE
+-rw-r--r--   0        0        0       59 2023-06-25 04:29:52.904018 aissist-0.0.7/Makefile
+-rw-r--r--   0        0        0      247 2023-06-25 04:28:51.416891 aissist-0.0.7/Pipfile
+-rw-r--r--   0        0        0    47145 2023-06-25 04:28:58.425264 aissist-0.0.7/Pipfile.lock
+-rw-r--r--   0        0        0     1342 2023-06-25 03:52:36.697190 aissist-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 03:27:17.722060 aissist-0.0.7/aissist/__init__.py
+-rw-r--r--   0        0        0     3343 2023-06-25 04:30:34.361956 aissist-0.0.7/aissist/aissistant.py
+-rw-r--r--   0        0        0      741 2023-06-25 04:30:03.600530 aissist-0.0.7/aissist/spinner.py
+-rw-r--r--   0        0        0      148 2023-06-25 04:24:06.481483 aissist-0.0.7/aissist/version.py
+-rw-r--r--   0        0        0    90052 2023-06-25 03:03:10.211368 aissist-0.0.7/images/screenshot.png
+-rw-r--r--   0        0        0      898 2023-06-25 04:29:41.187446 aissist-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 aissist-0.0.7/PKG-INFO
```

### Comparing `aissist-0.0.6/LICENSE` & `aissist-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aissist-0.0.6/Pipfile.lock` & `aissist-0.0.7/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8090277777777777%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4ff9976d1bbd921f4650dd87531375cc3a06260cbb467df8f57840d8100f5716'}}",*

 * * "'default'": "{'isort': OrderedDict([('hashes', "*

 * *              "['sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504', "*

 * *              "'sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6']), "*

 * *              "('index', 'pypi'), ('version', '==5.12.0')]), 'toml': OrderedDict([('hashes', "*

 * *              "['sha256:806143ae5bfb6a3c6e736a764057db0e6a0e […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "223032408d592f83d55d7787c53d4d3f74ca6001d00ebd23d0f891137c3c05f0"
+            "sha256": "4ff9976d1bbd921f4650dd87531375cc3a06260cbb467df8f57840d8100f5716"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.8"
         },
         "sources": [
             {
@@ -330,14 +330,22 @@
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
+        "isort": {
+            "hashes": [
+                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
+                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
+            ],
+            "index": "pypi",
+            "version": "==5.12.0"
+        },
         "multidict": {
             "hashes": [
                 "sha256:01a3a55bd90018c9c080fbb0b9f4891db37d148a0a18722b42f94694f8b6d4c9",
                 "sha256:0b1a97283e0c85772d613878028fec909f003993e1007eafa715b24b377cb9b8",
                 "sha256:0dfad7a5a1e39c53ed00d2dd0c2e36aed4650936dc18fd9a1826a5ae1cad6f03",
                 "sha256:11bdf3f5e1518b24530b8241529d2050014c884cf18b6fc69c0c2b30ca248710",
                 "sha256:1502e24330eb681bdaa3eb70d6358e818e8e8f908a22a1851dfd4e15bc2f8161",
@@ -442,14 +450,22 @@
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.31.0"
         },
+        "toml": {
+            "hashes": [
+                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
+                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
+            ],
+            "index": "pypi",
+            "version": "==0.10.2"
+        },
         "tomli-w": {
             "hashes": [
                 "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
@@ -562,9 +578,97 @@
                 "sha256:f4e2d08f07a3d7d3e12549052eb5ad3eab1c349c53ac51c209a0e5991bbada78",
                 "sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.9.2"
         }
     },
-    "develop": {}
+    "develop": {
+        "black": {
+            "hashes": [
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
+            ],
+            "index": "pypi",
+            "version": "==23.3.0"
+        },
+        "click": {
+            "hashes": [
+                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
+                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.3"
+        },
+        "mypy-extensions": {
+            "hashes": [
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
+        },
+        "packaging": {
+            "hashes": [
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
+        },
+        "pathspec": {
+            "hashes": [
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
+        },
+        "platformdirs": {
+            "hashes": [
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.8.0"
+        },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
+        "typing-extensions": {
+            "hashes": [
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==4.6.3"
+        }
+    }
 }
```

### Comparing `aissist-0.0.6/README.md` & `aissist-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aissist-0.0.6/aissist/aissistant.py` & `aissist-0.0.7/aissist/aissistant.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 import os
 import sys
-import textwrap
 
 import openai
 from prompt_toolkit import PromptSession
 from pygments import highlight
-from pygments.lexers import guess_lexer
 from pygments.formatters import TerminalFormatter
+from pygments.lexers import guess_lexer
 
-from spinner import Spinner
+from .spinner import Spinner
+from .version import __version__
 
 try:
     openai.api_key = os.environ["OPENAI_API_KEY"]
 except KeyError:
     print("Please put your API key in the OPENAI_API_KEY environment variable.")
     sys.exit(1)
 
 prompt = """You are a helpful but succinct chatbot that assists an impatient programmer by directly answering questions. You understand that the programmer is advanced enough to understand succinct phrases and prefers direct answers with little boilerplate.
 """
 
 session = PromptSession()
 
 
-def prompt_continuation(width: int,
-                        line_number,
-                        is_soft_wrap):
-    return '.' * (width-1) + " "
+def prompt_continuation(width: int, line_number, is_soft_wrap):
+    return "." * (width - 1) + " "
 
 
 def bold_single_backticks(text):
     """Formats a given string by making text enclosed in single backticks bold,
     using ANSI escape codes.
     """
     in_backticks = False
-    result = ''
+    result = ""
     for indx, c in enumerate(text):
-        if c == '`':
-            
+        if c == "`":
             if in_backticks:
-                result += '\033[0m'  # Reset text formatting
+                result += "\033[0m"  # Reset text formatting
                 in_backticks = False
             else:
-                result += '\033[1m'  # Bold text
+                result += "\033[1m"  # Bold text
                 in_backticks = True
         else:
             result += c
 
     if in_backticks:
-        result += '\033[0m'  # Reset text formatting
+        result += "\033[0m"  # Reset text formatting
 
     return result
 
 
 def highlight_codeblocks(markdown, columns: int):
     """Highlights code blocks in a markdown string and prints them to the console
     using pygments library.
     """
 
     inside_block = False
     current_block = ""
     for line in markdown.split("\n"):
-
         if line.startswith("```"):
             if inside_block is True:
                 # We are exiting a block, print it
                 lexer = guess_lexer(current_block)
                 formatted_code = highlight(current_block, lexer, TerminalFormatter())
                 print(formatted_code)
             else:
@@ -74,57 +70,55 @@
 
         elif inside_block is True:
             current_block += line + "\n"
         else:
             line = bold_single_backticks(line)
             sys.stdout.write(line)
 
+
 def loop(messages):
     """Main loop for the program"""
-    
-    result = session.prompt(">>> ", multiline=True,
-                prompt_continuation=prompt_continuation)
 
-    messages.append(
-        {"role": "user", "content": result}
+    result = session.prompt(
+        ">>> ", multiline=True, prompt_continuation=prompt_continuation
     )
 
+    messages.append({"role": "user", "content": result})
+
     spinner = Spinner()
     spinner.start()
 
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=messages,
     )
     message = response["choices"][0]["message"]
 
     spinner.stop()
 
     messages.append(message)
 
-
     print(" ")
     terminal_width = os.get_terminal_size().columns
     highlight_codeblocks(message["content"], columns=terminal_width)
     print(" ")
 
     return messages
 
-def main():
 
-    print("ESCAPE followed by ENTER to send. Ctrl-C to quit")
+def main():
+    print(f"AIssist v.{__version__}. ESCAPE followed by ENTER to send. Ctrl-C to quit")
 
-    messages = [
-        {"role": "system", "content": prompt}
-    ]
+    messages = [{"role": "system", "content": prompt}]
 
     try:
         while True:
             messages = loop(messages)
     except (KeyboardInterrupt, EOFError):
         # Ctrl-C and Ctrl-D
         sys.exit(0)
     except Exception:
         raise
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `aissist-0.0.6/aissist/spinner.py` & `aissist-0.0.7/aissist/spinner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
-import time
 import threading
+import time
 from typing import Optional
 
+
 class Spinner:
     """Simple implementation of a spinner"""
 
     def __init__(self):
         self.spinner_flag: bool = True
         self.thread: Optional[threading.Thread] = None
 
     def spinner(self, spin_delay: float = 0.12):
         while self.spinner_flag:
             for char in "|/-\\":
-                sys.stdout.write('\r' + char)
+                sys.stdout.write("\r" + char)
                 sys.stdout.flush()
                 time.sleep(spin_delay)
         sys.stdout.write("\r")
 
     def stop(self):
         self.spinner_flag = False
         self.thread.join()
```

### Comparing `aissist-0.0.6/images/screenshot.png` & `aissist-0.0.7/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `aissist-0.0.6/pyproject.toml` & `aissist-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aissist"
-version = "0.0.6"
+version = "0.0.7"
 description = "A simple GPT command line interface"
 authors = [
   { name = "Craig Booth", email = "craigmbooth@gmail.com" },
 ]
 license = { file = "LICENSE" }
 
 readme = "README.md"
@@ -33,8 +33,7 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project.scripts]
 ai = "aissist.aissistant:main"
-
```

### Comparing `aissist-0.0.6/PKG-INFO` & `aissist-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissist
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple GPT command line interface
 Author-email: Craig Booth <craigmbooth@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

