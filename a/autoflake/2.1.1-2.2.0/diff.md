# Comparing `tmp/autoflake-2.1.1.tar.gz` & `tmp/autoflake-2.2.0.tar.gz`

## Comparing `autoflake-2.1.1.tar` & `autoflake-2.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rwxr-xr-x   0        0        0    46884 2020-02-02 00:00:00.000000 autoflake-2.1.1/autoflake.py
--rwxr-xr-x   0        0        0    90488 2020-02-02 00:00:00.000000 autoflake-2.1.1/test_autoflake.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 autoflake-2.1.1/.gitignore
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 autoflake-2.1.1/AUTHORS.rst
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoflake-2.1.1/LICENSE
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 autoflake-2.1.1/README.md
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 autoflake-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 autoflake-2.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0    50180 2020-02-02 00:00:00.000000 autoflake-2.2.0/autoflake.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autoflake-2.2.0/py.typed
+-rwxr-xr-x   0        0        0    92651 2020-02-02 00:00:00.000000 autoflake-2.2.0/test_autoflake.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 autoflake-2.2.0/.gitignore
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 autoflake-2.2.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 autoflake-2.2.0/LICENSE
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 autoflake-2.2.0/README.md
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 autoflake-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 autoflake-2.2.0/PKG-INFO
```

### Comparing `autoflake-2.1.1/autoflake.py` & `autoflake-2.2.0/autoflake.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,49 +16,59 @@
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
 # CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
 # TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 # SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """Removes unused imports and unused variables as reported by pyflakes."""
+from __future__ import annotations
+
 import ast
 import collections
 import difflib
 import fnmatch
 import io
 import logging
 import os
 import pathlib
 import re
 import signal
 import string
 import sys
 import sysconfig
 import tokenize
+from typing import Any
+from typing import Callable
+from typing import cast
+from typing import IO
+from typing import Iterable
+from typing import Mapping
+from typing import MutableMapping
+from typing import Sequence
 
 import pyflakes.api
 import pyflakes.messages
 import pyflakes.reporter
 
 
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 
 _LOGGER = logging.getLogger("autoflake")
 _LOGGER.propagate = False
 
 ATOMS = frozenset([tokenize.NAME, tokenize.NUMBER, tokenize.STRING])
 
 EXCEPT_REGEX = re.compile(r"^\s*except [\s,()\w]+ as \w+:$")
 PYTHON_SHEBANG_REGEX = re.compile(r"^#!.*\bpython[3]?\b\s*$")
 
 MAX_PYTHON_FILE_DETECTION_BYTES = 1024
 
 
-def standard_paths():
+def standard_paths() -> Iterable[str]:
     """Yield paths to standard modules."""
     paths = sysconfig.get_paths()
     path_names = ("stdlib", "platstdlib")
     for path_name in path_names:
         # Yield lib paths.
         if path_name in paths:
             path = paths[path_name]
@@ -67,15 +77,15 @@
 
             # Yield lib-dynload paths.
             dynload_path = os.path.join(path, "lib-dynload")
             if os.path.isdir(dynload_path):
                 yield from os.listdir(dynload_path)
 
 
-def standard_package_names():
+def standard_package_names() -> Iterable[str]:
     """Yield standard module names."""
     for name in standard_paths():
         if name.startswith("_") or "-" in name:
             continue
 
         if "." in name and not name.endswith(("so", "py", "pyc")):
             continue
@@ -103,56 +113,69 @@
 }
 
 SAFE_IMPORTS = (
     frozenset(standard_package_names()) - IMPORTS_WITH_SIDE_EFFECTS | BINARY_IMPORTS
 )
 
 
-def unused_import_line_numbers(messages):
+def unused_import_line_numbers(
+    messages: Iterable[pyflakes.messages.Message],
+) -> Iterable[int]:
     """Yield line numbers of unused imports."""
     for message in messages:
         if isinstance(message, pyflakes.messages.UnusedImport):
             yield message.lineno
 
 
-def unused_import_module_name(messages):
+def unused_import_module_name(
+    messages: Iterable[pyflakes.messages.Message],
+) -> Iterable[tuple[int, str]]:
     """Yield line number and module name of unused imports."""
-    pattern = r"\'(.+?)\'"
+    pattern = re.compile(r"\'(.+?)\'")
     for message in messages:
         if isinstance(message, pyflakes.messages.UnusedImport):
-            module_name = re.search(pattern, str(message))
+            module_name = pattern.search(str(message))
             if module_name:
                 module_name = module_name.group()[1:-1]
                 yield (message.lineno, module_name)
 
 
-def star_import_used_line_numbers(messages):
+def star_import_used_line_numbers(
+    messages: Iterable[pyflakes.messages.Message],
+) -> Iterable[int]:
     """Yield line number of star import usage."""
     for message in messages:
         if isinstance(message, pyflakes.messages.ImportStarUsed):
             yield message.lineno
 
 
-def star_import_usage_undefined_name(messages):
+def star_import_usage_undefined_name(
+    messages: Iterable[pyflakes.messages.Message],
+) -> Iterable[tuple[int, str, str]]:
     """Yield line number, undefined name, and its possible origin module."""
     for message in messages:
         if isinstance(message, pyflakes.messages.ImportStarUsage):
             undefined_name = message.message_args[0]
             module_name = message.message_args[1]
             yield (message.lineno, undefined_name, module_name)
 
 
-def unused_variable_line_numbers(messages):
+def unused_variable_line_numbers(
+    messages: Iterable[pyflakes.messages.Message],
+) -> Iterable[int]:
     """Yield line numbers of unused variables."""
     for message in messages:
         if isinstance(message, pyflakes.messages.UnusedVariable):
             yield message.lineno
 
 
-def duplicate_key_line_numbers(messages, source):
+def duplicate_key_line_numbers(
+    messages: Iterable[pyflakes.messages.Message],
+    source: str,
+) -> Iterable[int]:
     """Yield line numbers of duplicate keys."""
     messages = [
         message
         for message in messages
         if isinstance(message, pyflakes.messages.MultiValueRepeatedKeyLiteral)
     ]
 
@@ -174,57 +197,62 @@
                     good = False
 
             if good:
                 for message in messages:
                     yield message.lineno
 
 
-def create_key_to_messages_dict(messages):
+def create_key_to_messages_dict(
+    messages: Iterable[pyflakes.messages.MultiValueRepeatedKeyLiteral],
+) -> Mapping[Any, Iterable[pyflakes.messages.MultiValueRepeatedKeyLiteral]]:
     """Return dict mapping the key to list of messages."""
-    dictionary = collections.defaultdict(lambda: [])
+    dictionary: dict[
+        Any,
+        list[pyflakes.messages.MultiValueRepeatedKeyLiteral],
+    ] = collections.defaultdict(list)
     for message in messages:
         dictionary[message.message_args[0]].append(message)
     return dictionary
 
 
-def check(source):
+def check(source: str) -> Iterable[pyflakes.messages.Message]:
     """Return messages from pyflakes."""
     reporter = ListReporter()
     try:
         pyflakes.api.check(source, filename="<string>", reporter=reporter)
     except (AttributeError, RecursionError, UnicodeDecodeError):
         pass
     return reporter.messages
 
 
 class StubFile:
     """Stub out file for pyflakes."""
 
-    def write(self, *_):
+    def write(self, *_: Any) -> None:
         """Stub out."""
 
 
 class ListReporter(pyflakes.reporter.Reporter):
     """Accumulate messages in messages list."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize.
 
         Ignore errors from Reporter.
         """
         ignore = StubFile()
         pyflakes.reporter.Reporter.__init__(self, ignore, ignore)
-        self.messages = []
+        self.messages: list[pyflakes.messages.Message] = []
 
-    def flake(self, message):
+    def flake(self, message: pyflakes.messages.Message) -> None:
         """Accumulate messages."""
         self.messages.append(message)
 
 
-def extract_package_name(line):
+def extract_package_name(line: str) -> str | None:
     """Return package name in import statement."""
     assert "\\" not in line
     assert "(" not in line
     assert ")" not in line
     assert ";" not in line
 
     if line.lstrip().startswith(("import", "from")):
@@ -235,24 +263,24 @@
 
     package = word.split(".")[0]
     assert " " not in package
 
     return package
 
 
-def multiline_import(line, previous_line=""):
+def multiline_import(line: str, previous_line: str = "") -> bool:
     """Return True if import is spans multiples lines."""
     for symbol in "()":
         if symbol in line:
             return True
 
     return multiline_statement(line, previous_line)
 
 
-def multiline_statement(line, previous_line=""):
+def multiline_statement(line: str, previous_line: str = "") -> bool:
     """Return True if this is part of a multiline statement."""
     for symbol in "\\:;":
         if symbol in line:
             return True
 
     sio = io.StringIO(line)
     try:
@@ -266,50 +294,53 @@
     """Allows a rewrite operation to span multiple lines.
 
     In the main rewrite loop, every time a helper function returns a
     ``PendingFix`` object instead of a string, this object will be called
     with the following line.
     """
 
-    def __init__(self, line):
+    def __init__(self, line: str) -> None:
         """Analyse and store the first line."""
         self.accumulator = collections.deque([line])
 
-    def __call__(self, line):
+    def __call__(self, line: str) -> PendingFix | str:
         """Process line considering the accumulator.
 
         Return self to keep processing the following lines or a string
         with the final result of all the lines processed at once.
         """
         raise NotImplementedError("Abstract method needs to be overwritten")
 
 
-def _valid_char_in_line(char, line):
+def _valid_char_in_line(char: str, line: str) -> bool:
     """Return True if a char appears in the line and is not commented."""
     comment_index = line.find("#")
     char_index = line.find(char)
     valid_char_in_line = char_index >= 0 and (
         comment_index > char_index or comment_index < 0
     )
     return valid_char_in_line
 
 
-def _top_module(module_name):
+def _top_module(module_name: str) -> str:
     """Return the name of the top level module in the hierarchy."""
     if module_name[0] == ".":
         return "%LOCAL_MODULE%"
     return module_name.split(".")[0]
 
 
-def _modules_to_remove(unused_modules, safe_to_remove=SAFE_IMPORTS):
+def _modules_to_remove(
+    unused_modules: Iterable[str],
+    safe_to_remove: Iterable[str] = SAFE_IMPORTS,
+) -> Iterable[str]:
     """Discard unused modules that are not safe to remove from the list."""
     return [x for x in unused_modules if _top_module(x) in safe_to_remove]
 
 
-def _segment_module(segment):
+def _segment_module(segment: str) -> str:
     """Extract the module identifier inside the segment.
 
     It might be the case the segment does not have a module (e.g. is composed
     just by a parenthesis or line continuation and whitespace). In this
     scenario we just keep the segment... These characters are not valid in
     identifiers, so they will never be contained in the list of unused modules
     anyway.
@@ -334,27 +365,27 @@
         re.M,
     )
     # ^ module + comma + following space (including new line and continuation)
     IDENTIFIER_RE = re.compile(r"[^,\s]+")
 
     def __init__(
         self,
-        line,
-        unused_module=(),
-        remove_all_unused_imports=False,
-        safe_to_remove=SAFE_IMPORTS,
-        previous_line="",
+        line: str,
+        unused_module: Iterable[str] = (),
+        remove_all_unused_imports: bool = False,
+        safe_to_remove: Iterable[str] = SAFE_IMPORTS,
+        previous_line: str = "",
     ):
         """Receive the same parameters as ``filter_unused_import``."""
-        self.remove = unused_module
-        self.parenthesized = "(" in line
+        self.remove: Iterable[str] = unused_module
+        self.parenthesized: bool = "(" in line
         self.from_, imports = self.IMPORT_RE.split(line, maxsplit=1)
         match = self.BASE_RE.search(self.from_)
         self.base = match.group(1) if match else None
-        self.give_up = False
+        self.give_up: bool = False
 
         if not remove_all_unused_imports:
             if self.base and _top_module(self.base) not in safe_to_remove:
                 self.give_up = True
             else:
                 self.remove = _modules_to_remove(self.remove, safe_to_remove)
 
@@ -362,29 +393,29 @@
             # Ignore tricky things like "try: \<new line> import" ...
             self.give_up = True
 
         self.analyze(line)
 
         PendingFix.__init__(self, imports)
 
-    def is_over(self, line=None):
+    def is_over(self, line: str | None = None) -> bool:
         """Return True if the multiline import statement is over."""
         line = line or self.accumulator[-1]
 
         if self.parenthesized:
             return _valid_char_in_line(")", line)
 
         return not _valid_char_in_line("\\", line)
 
-    def analyze(self, line):
+    def analyze(self, line: str) -> None:
         """Decide if the statement will be fixed or left unchanged."""
         if any(ch in line for ch in ";:#"):
             self.give_up = True
 
-    def fix(self, accumulated):
+    def fix(self, accumulated: Iterable[str]) -> str:
         """Given a collection of accumulated lines, fix the entire import."""
         old_imports = "".join(accumulated)
         ending = get_line_ending(old_imports)
         # Split imports into segments that contain the module name +
         # comma + whitespace and eventual <newline> \ ( ) chars
         segments = [x for x in self.SEGMENT_RE.findall(old_imports) if x]
         modules = [_segment_module(x) for x in segments]
@@ -412,72 +443,80 @@
             # Fix the edge case: inline parenthesis + just one surviving import
             if self.parenthesized and any(ch not in fixed for ch in "()"):
                 fixed = fixed.strip(string.whitespace + "()") + ending
 
         # Replace empty imports with a "pass" statement
         empty = len(fixed.strip(string.whitespace + "\\(),")) < 1
         if empty:
-            indentation = self.INDENTATION_RE.search(self.from_).group(0)
+            match = self.INDENTATION_RE.search(self.from_)
+            assert match is not None
+            indentation = match.group(0)
             return indentation + "pass" + ending
 
         return self.from_ + "import " + fixed
 
-    def __call__(self, line=None):
+    def __call__(self, line: str | None = None) -> PendingFix | str:
         """Accumulate all the lines in the import and then trigger the fix."""
         if line:
             self.accumulator.append(line)
             self.analyze(line)
         if not self.is_over(line):
             return self
         if self.give_up:
             return self.from_ + "import " + "".join(self.accumulator)
 
         return self.fix(self.accumulator)
 
 
-def _filter_imports(imports, parent=None, unused_module=()):
+def _filter_imports(
+    imports: Iterable[str],
+    parent: str | None = None,
+    unused_module: Iterable[str] = (),
+) -> Sequence[str]:
     # We compare full module name (``a.module`` not `module`) to
     # guarantee the exact same module as detected from pyflakes.
     sep = "" if parent and parent[-1] == "." else "."
 
-    def full_name(name):
+    def full_name(name: str) -> str:
         return name if parent is None else parent + sep + name
 
     return [x for x in imports if full_name(x) not in unused_module]
 
 
-def filter_from_import(line, unused_module):
+def filter_from_import(line: str, unused_module: Iterable[str]) -> str:
     """Parse and filter ``from something import a, b, c``.
 
     Return line without unused import modules, or `pass` if all of the
     module in import is unused.
     """
     (indentation, imports) = re.split(
         pattern=r"\bimport\b",
         string=line,
         maxsplit=1,
     )
-    base_module = re.search(
+    match = re.search(
         pattern=r"\bfrom\s+([^ ]+)",
         string=indentation,
-    ).group(1)
+    )
+    assert match is not None
+    base_module = match.group(1)
 
     imports = re.split(pattern=r"\s*,\s*", string=imports.strip())
     filtered_imports = _filter_imports(imports, base_module, unused_module)
 
     # All of the import in this statement is unused
     if not filtered_imports:
         return get_indentation(line) + "pass" + get_line_ending(line)
 
     indentation += "import "
 
     return indentation + ", ".join(filtered_imports) + get_line_ending(line)
 
 
-def break_up_import(line):
+def break_up_import(line: str) -> str:
     """Return line with imports on separate lines."""
     assert "\\" not in line
     assert "(" not in line
     assert ")" not in line
     assert ";" not in line
     assert "#" not in line
     assert not line.lstrip().startswith("from")
@@ -497,54 +536,54 @@
 
     return "".join(
         [indentation + i.strip() + newline for i in imports.split(",")],
     )
 
 
 def filter_code(
-    source,
-    additional_imports=None,
-    expand_star_imports=False,
-    remove_all_unused_imports=False,
-    remove_duplicate_keys=False,
-    remove_unused_variables=False,
-    remove_rhs_for_unused_variables=False,
-    ignore_init_module_imports=False,
-):
+    source: str,
+    additional_imports: Iterable[str] | None = None,
+    expand_star_imports: bool = False,
+    remove_all_unused_imports: bool = False,
+    remove_duplicate_keys: bool = False,
+    remove_unused_variables: bool = False,
+    remove_rhs_for_unused_variables: bool = False,
+    ignore_init_module_imports: bool = False,
+) -> Iterable[str]:
     """Yield code with unused imports removed."""
     imports = SAFE_IMPORTS
     if additional_imports:
         imports |= frozenset(additional_imports)
     del additional_imports
 
     messages = check(source)
 
     if ignore_init_module_imports:
-        marked_import_line_numbers = frozenset()
+        marked_import_line_numbers: frozenset[int] = frozenset()
     else:
         marked_import_line_numbers = frozenset(
             unused_import_line_numbers(messages),
         )
-    marked_unused_module = collections.defaultdict(lambda: [])
+    marked_unused_module: dict[int, list[str]] = collections.defaultdict(list)
     for line_number, module_name in unused_import_module_name(messages):
         marked_unused_module[line_number].append(module_name)
 
+    undefined_names: list[str] = []
     if expand_star_imports and not (
         # See explanations in #18.
         re.search(r"\b__all__\b", source)
         or re.search(r"\bdel\b", source)
     ):
         marked_star_import_line_numbers = frozenset(
             star_import_used_line_numbers(messages),
         )
         if len(marked_star_import_line_numbers) > 1:
             # Auto expanding only possible for single star import
             marked_star_import_line_numbers = frozenset()
         else:
-            undefined_names = []
             for line_number, undefined_name, _ in star_import_usage_undefined_name(
                 messages,
             ):
                 undefined_names.append(undefined_name)
             if not undefined_names:
                 marked_star_import_line_numbers = frozenset()
     else:
@@ -554,25 +593,25 @@
         marked_variable_line_numbers = frozenset(
             unused_variable_line_numbers(messages),
         )
     else:
         marked_variable_line_numbers = frozenset()
 
     if remove_duplicate_keys:
-        marked_key_line_numbers = frozenset(
+        marked_key_line_numbers: frozenset[int] = frozenset(
             duplicate_key_line_numbers(messages, source),
         )
     else:
         marked_key_line_numbers = frozenset()
 
     line_messages = get_messages_by_line(messages)
 
     sio = io.StringIO(source)
     previous_line = ""
-    result = None
+    result: str | PendingFix = ""
     for line_number, line in enumerate(sio.readlines(), start=1):
         if isinstance(result, PendingFix):
             result = result(line)
         elif "#" in line:
             result = line
         elif line_number in marked_import_line_numbers:
             result = filter_unused_import(
@@ -602,35 +641,40 @@
 
         if not isinstance(result, PendingFix):
             yield result
 
         previous_line = line
 
 
-def get_messages_by_line(messages):
+def get_messages_by_line(
+    messages: Iterable[pyflakes.messages.Message],
+) -> Mapping[int, pyflakes.messages.Message]:
     """Return dictionary that maps line number to message."""
-    line_messages = {}
+    line_messages: dict[int, pyflakes.messages.Message] = {}
     for message in messages:
         line_messages[message.lineno] = message
     return line_messages
 
 
-def filter_star_import(line, marked_star_import_undefined_name):
+def filter_star_import(
+    line: str,
+    marked_star_import_undefined_name: Iterable[str],
+) -> str:
     """Return line with the star import expanded."""
     undefined_name = sorted(set(marked_star_import_undefined_name))
     return re.sub(r"\*", ", ".join(undefined_name), line)
 
 
 def filter_unused_import(
-    line,
-    unused_module,
-    remove_all_unused_imports,
-    imports,
-    previous_line="",
-):
+    line: str,
+    unused_module: Iterable[str],
+    remove_all_unused_imports: bool,
+    imports: Iterable[str],
+    previous_line: str = "",
+) -> PendingFix | str:
     """Return line if used, otherwise return None."""
     # Ignore doctests.
     if line.lstrip().startswith(">"):
         return line
 
     if multiline_import(line, previous_line):
         filt = FilterMultilineImport(
@@ -644,29 +688,33 @@
 
     is_from_import = line.lstrip().startswith("from")
 
     if "," in line and not is_from_import:
         return break_up_import(line)
 
     package = extract_package_name(line)
-    if not remove_all_unused_imports and package not in imports:
+    if not remove_all_unused_imports and package is not None and package not in imports:
         return line
 
     if "," in line:
         assert is_from_import
         return filter_from_import(line, unused_module)
     else:
         # We need to replace import with "pass" in case the import is the
         # only line inside a block. For example,
         # "if True:\n    import os". In such cases, if the import is
         # removed, the block will be left hanging with no body.
         return get_indentation(line) + "pass" + get_line_ending(line)
 
 
-def filter_unused_variable(line, previous_line="", drop_rhs=False):
+def filter_unused_variable(
+    line: str,
+    previous_line: str = "",
+    drop_rhs: bool = False,
+) -> str:
     """Return line if used, otherwise return None."""
     if re.match(EXCEPT_REGEX, line):
         return re.sub(r" as \w+:$", ":", line, count=1)
     elif multiline_statement(line, previous_line):
         return line
     elif line.count("=") == 1:
         split_line = line.split("=")
@@ -686,29 +734,29 @@
             return ""
         return get_indentation(line) + value
     else:
         return line
 
 
 def filter_duplicate_key(
-    line,
-    message,
-    line_number,
-    marked_line_numbers,
-    source,
-    previous_line="",
-):
+    line: str,
+    message: pyflakes.messages.Message,
+    line_number: int,
+    marked_line_numbers: Iterable[int],
+    source: str,
+    previous_line: str = "",
+) -> str:
     """Return '' if first occurrence of the key otherwise return `line`."""
     if marked_line_numbers and line_number == sorted(marked_line_numbers)[0]:
         return ""
 
     return line
 
 
-def dict_entry_has_key(line, key):
+def dict_entry_has_key(line: str, key: Any) -> bool:
     """Return True if `line` is a dict entry that uses `key`.
 
     Return False for multiline cases where the line should not be removed by
     itself.
 
     """
     if "#" in line:
@@ -722,37 +770,37 @@
         candidate_key = ast.literal_eval(result.group(1))
     except (SyntaxError, ValueError):
         return False
 
     if multiline_statement(result.group(2)):
         return False
 
-    return candidate_key == key
+    return cast(bool, candidate_key == key)
 
 
-def is_literal_or_name(value):
+def is_literal_or_name(value: str) -> bool:
     """Return True if value is a literal or a name."""
     try:
         ast.literal_eval(value)
         return True
     except (SyntaxError, ValueError):
         pass
 
     if value.strip() in ["dict()", "list()", "set()"]:
         return True
 
     # Support removal of variables on the right side. But make sure
     # there are no dots, which could mean an access of a property.
-    return re.match(r"^\w+\s*$", value)
+    return re.match(r"^\w+\s*$", value) is not None
 
 
 def useless_pass_line_numbers(
-    source,
-    ignore_pass_after_docstring=False,
-):
+    source: str,
+    ignore_pass_after_docstring: bool = False,
+) -> Iterable[int]:
     """Yield line numbers of unneeded "pass" statements."""
     sio = io.StringIO(source)
     previous_token_type = None
     last_pass_row = None
     last_pass_indentation = None
     previous_line = ""
     previous_non_empty_line = ""
@@ -795,21 +843,21 @@
         previous_token_type = token_type
         previous_line = line
         if line.strip():
             previous_non_empty_line = line
 
 
 def filter_useless_pass(
-    source,
-    ignore_pass_statements=False,
-    ignore_pass_after_docstring=False,
-):
+    source: str,
+    ignore_pass_statements: bool = False,
+    ignore_pass_after_docstring: bool = False,
+) -> Iterable[str]:
     """Yield code with useless "pass" lines removed."""
     if ignore_pass_statements:
-        marked_lines = frozenset()
+        marked_lines: frozenset[int] = frozenset()
     else:
         try:
             marked_lines = frozenset(
                 useless_pass_line_numbers(
                     source,
                     ignore_pass_after_docstring,
                 ),
@@ -819,44 +867,44 @@
 
     sio = io.StringIO(source)
     for line_number, line in enumerate(sio.readlines(), start=1):
         if line_number not in marked_lines:
             yield line
 
 
-def get_indentation(line):
+def get_indentation(line: str) -> str:
     """Return leading whitespace."""
     if line.strip():
         non_whitespace_index = len(line) - len(line.lstrip())
         return line[:non_whitespace_index]
     else:
         return ""
 
 
-def get_line_ending(line):
+def get_line_ending(line: str) -> str:
     """Return line ending."""
     non_whitespace_index = len(line.rstrip()) - len(line)
     if not non_whitespace_index:
         return ""
     else:
         return line[non_whitespace_index:]
 
 
 def fix_code(
-    source,
-    additional_imports=None,
-    expand_star_imports=False,
-    remove_all_unused_imports=False,
-    remove_duplicate_keys=False,
-    remove_unused_variables=False,
-    remove_rhs_for_unused_variables=False,
-    ignore_init_module_imports=False,
-    ignore_pass_statements=False,
-    ignore_pass_after_docstring=False,
-):
+    source: str,
+    additional_imports: Iterable[str] | None = None,
+    expand_star_imports: bool = False,
+    remove_all_unused_imports: bool = False,
+    remove_duplicate_keys: bool = False,
+    remove_unused_variables: bool = False,
+    remove_rhs_for_unused_variables: bool = False,
+    ignore_init_module_imports: bool = False,
+    ignore_pass_statements: bool = False,
+    ignore_pass_after_docstring: bool = False,
+) -> str:
     """Return code with all filtering run on it."""
     if not source:
         return source
 
     # pyflakes does not handle "nonlocal" correctly.
     if "nonlocal" in source:
         remove_unused_variables = False
@@ -887,15 +935,19 @@
         if filtered_source == source:
             break
         source = filtered_source
 
     return filtered_source
 
 
-def fix_file(filename, args, standard_out=None) -> int:
+def fix_file(
+    filename: str,
+    args: Mapping[str, Any],
+    standard_out: IO[str] | None = None,
+) -> int:
     """Run fix_code() on a file."""
     if standard_out is None:
         standard_out = sys.stdout
     encoding = detect_encoding(filename)
     with open_with_encoding(filename, encoding=encoding) as input_file:
         return _fix_file(
             input_file,
@@ -904,20 +956,20 @@
             args["write_to_stdout"],
             standard_out,
             encoding=encoding,
         )
 
 
 def _fix_file(
-    input_file,
-    filename,
-    args,
-    write_to_stdout,
-    standard_out,
-    encoding=None,
+    input_file: IO[str],
+    filename: str,
+    args: Mapping[str, Any],
+    write_to_stdout: bool,
+    standard_out: IO[str],
+    encoding: str | None = None,
 ) -> int:
     source = input_file.read()
     original_source = source
 
     isInitFile = os.path.basename(filename) == "__init__.py"
 
     if args["ignore_init_module_imports"] and isInitFile:
@@ -977,56 +1029,56 @@
         else:
             _LOGGER.debug("Clean %s: nothing to fix", filename)
 
     return 0
 
 
 def open_with_encoding(
-    filename,
-    encoding,
-    mode="r",
-    limit_byte_check=-1,
-):
+    filename: str,
+    encoding: str | None,
+    mode: str = "r",
+    limit_byte_check: int = -1,
+) -> IO[str]:
     """Return opened file with a specific encoding."""
     if not encoding:
         encoding = detect_encoding(filename, limit_byte_check=limit_byte_check)
 
     return open(
         filename,
         mode=mode,
         encoding=encoding,
-        newline="",
-    )  # Preserve line endings
+        newline="",  # Preserve line endings
+    )
 
 
-def detect_encoding(filename, limit_byte_check=-1):
+def detect_encoding(filename: str, limit_byte_check: int = -1) -> str:
     """Return file encoding."""
     try:
         with open(filename, "rb") as input_file:
             encoding = _detect_encoding(input_file.readline)
 
             # Check for correctness of encoding.
             with open_with_encoding(filename, encoding) as input_file:
                 input_file.read(limit_byte_check)
 
         return encoding
     except (LookupError, SyntaxError, UnicodeDecodeError):
         return "latin-1"
 
 
-def _detect_encoding(readline):
+def _detect_encoding(readline: Callable[[], bytes]) -> str:
     """Return file encoding."""
     try:
         encoding = tokenize.detect_encoding(readline)[0]
         return encoding
     except (LookupError, SyntaxError, UnicodeDecodeError):
         return "latin-1"
 
 
-def get_diff_text(old, new, filename):
+def get_diff_text(old: Sequence[str], new: Sequence[str], filename: str) -> str:
     """Return text of unified diff between old and new."""
     newline = "\n"
     diff = difflib.unified_diff(
         old,
         new,
         "original/" + filename,
         "fixed/" + filename,
@@ -1040,20 +1092,20 @@
         # Work around missing newline (http://bugs.python.org/issue2142).
         if not line.endswith(newline):
             text += newline + r"\ No newline at end of file" + newline
 
     return text
 
 
-def _split_comma_separated(string):
+def _split_comma_separated(string: str) -> set[str]:
     """Return a set of strings."""
     return {text.strip() for text in string.split(",") if text.strip()}
 
 
-def is_python_file(filename):
+def is_python_file(filename: str) -> bool:
     """Return True if filename is Python file."""
     if filename.endswith(".py"):
         return True
 
     try:
         with open_with_encoding(
             filename,
@@ -1069,42 +1121,46 @@
 
     if not PYTHON_SHEBANG_REGEX.match(first_line):
         return False
 
     return True
 
 
-def is_exclude_file(filename, exclude):
+def is_exclude_file(filename: str, exclude: Iterable[str]) -> bool:
     """Return True if file matches exclude pattern."""
     base_name = os.path.basename(filename)
 
     if base_name.startswith("."):
         return True
 
     for pattern in exclude:
         if fnmatch.fnmatch(base_name, pattern):
             return True
         if fnmatch.fnmatch(filename, pattern):
             return True
     return False
 
 
-def match_file(filename, exclude):
+def match_file(filename: str, exclude: Iterable[str]) -> bool:
     """Return True if file is okay for modifying/recursing."""
     if is_exclude_file(filename, exclude):
         _LOGGER.debug("Skipped %s: matched to exclude pattern", filename)
         return False
 
     if not os.path.isdir(filename) and not is_python_file(filename):
         return False
 
     return True
 
 
-def find_files(filenames, recursive, exclude):
+def find_files(
+    filenames: list[str],
+    recursive: bool,
+    exclude: Iterable[str],
+) -> Iterable[str]:
     """Yield filenames."""
     while filenames:
         name = filenames.pop(0)
         if recursive and os.path.isdir(name):
             for root, directories, children in os.walk(name):
                 filenames += [
                     os.path.join(root, f)
@@ -1125,47 +1181,47 @@
         else:
             if not is_exclude_file(name, exclude):
                 yield name
             else:
                 _LOGGER.debug("Skipped %s: matched to exclude pattern", name)
 
 
-def process_pyproject_toml(toml_file_path):
+def process_pyproject_toml(toml_file_path: str) -> MutableMapping[str, Any] | None:
     """Extract config mapping from pyproject.toml file."""
     try:
         import tomllib
     except ModuleNotFoundError:
         import tomli as tomllib
 
     with open(toml_file_path, "rb") as f:
         return tomllib.load(f).get("tool", {}).get("autoflake", None)
 
 
-def process_config_file(config_file_path):
+def process_config_file(config_file_path: str) -> MutableMapping[str, Any] | None:
     """Extract config mapping from config file."""
     import configparser
 
     reader = configparser.ConfigParser()
     reader.read(config_file_path)
     if not reader.has_section("autoflake"):
         return None
 
     return reader["autoflake"]
 
 
-def find_and_process_config(args):
+def find_and_process_config(args: Mapping[str, Any]) -> MutableMapping[str, Any] | None:
     # Configuration file parsers {filename: parser function}.
-    CONFIG_FILES = {
+    CONFIG_FILES: Mapping[str, Callable[[str], MutableMapping[str, Any] | None]] = {
         "pyproject.toml": process_pyproject_toml,
         "setup.cfg": process_config_file,
     }
     # Traverse the file tree common to all files given as argument looking for
     # a configuration file
     config_path = os.path.commonpath([os.path.abspath(file) for file in args["files"]])
-    config = None
+    config: Mapping[str, Any] | None = None
     while True:
         for config_file, processor in CONFIG_FILES.items():
             config_file_path = os.path.join(
                 os.path.join(config_path, config_file),
             )
             if os.path.isfile(config_file_path):
                 config = processor(config_file_path)
@@ -1175,30 +1231,32 @@
             break
         config_path, tail = os.path.split(config_path)
         if not tail:
             break
     return config
 
 
-def merge_configuration_file(flag_args):
+def merge_configuration_file(
+    flag_args: MutableMapping[str, Any],
+) -> tuple[MutableMapping[str, Any], bool]:
     """Merge configuration from a file into args."""
     BOOL_TYPES = {
         "1": True,
         "yes": True,
         "true": True,
         "on": True,
         "0": False,
         "no": False,
         "false": False,
         "off": False,
     }
 
     if "config_file" in flag_args:
         config_file = pathlib.Path(flag_args["config_file"]).resolve()
-        config = process_config_file(config_file)
+        config = process_config_file(str(config_file))
 
         if not config:
             _LOGGER.error(
                 "can't parse config file '%s'",
                 config_file,
             )
             return flag_args, False
@@ -1218,15 +1276,15 @@
         "remove_all_unused_imports",
         "remove_duplicate_keys",
         "remove_rhs_for_unused_variables",
         "remove_unused_variables",
         "write_to_stdout",
     }
 
-    config_args = {}
+    config_args: dict[str, Any] = {}
     if config is not None:
         for name, value in config.items():
             arg = name.replace("-", "_")
             if arg in BOOL_FLAGS:
                 # boolean properties
                 if isinstance(value, str):
                     value = BOOL_TYPES.get(value.lower(), value)
@@ -1268,15 +1326,20 @@
         **default_args,
         **config_args,
         **flag_args,
         **merged_args,
     }, True
 
 
-def _main(argv, standard_out, standard_error, standard_input=None) -> int:
+def _main(
+    argv: Sequence[str],
+    standard_out: IO[str] | None,
+    standard_error: IO[str] | None,
+    standard_input: IO[str] | None = None,
+) -> int:
     """Return exit status.
 
     0 means no error.
     """
     import argparse
 
     parser = argparse.ArgumentParser(
@@ -1419,16 +1482,15 @@
         dest="write_to_stdout",
         help=(
             "print changed text to stdout. defaults to true "
             "when formatting stdin, or to false otherwise"
         ),
     )
 
-    args = parser.parse_args(argv[1:])
-    args = vars(args)
+    args: MutableMapping[str, Any] = vars(parser.parse_args(argv[1:]))
 
     if standard_error is None:
         _LOGGER.addHandler(logging.NullHandler())
     else:
         _LOGGER.addHandler(logging.StreamHandler(standard_error))
         loglevels = [logging.WARNING, logging.INFO, logging.DEBUG]
         try:
@@ -1472,15 +1534,15 @@
         args["jobs"] == 1
         or len(files) == 1
         or args["jobs"] == 1
         or "-" in files
         or standard_out is not None
     ):
         for name in files:
-            if name == "-":
+            if name == "-" and standard_input is not None:
                 exit_status |= _fix_file(
                     standard_input,
                     args["stdin_display_name"],
                     args=args,
                     write_to_stdout=True,
                     standard_out=standard_out or sys.stdout,
                 )
```

### Comparing `autoflake-2.1.1/test_autoflake.py` & `autoflake-2.2.0/test_autoflake.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 #!/usr/bin/env python
 """Test suite for autoflake."""
+from __future__ import annotations
+
 import contextlib
 import functools
 import io
 import os
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import unittest
+from typing import Any
+from typing import Iterator
+from typing import Mapping
+from typing import Sequence
 
 import autoflake
 
 
 ROOT_DIRECTORY = os.path.abspath(os.path.dirname(__file__))
 
 
@@ -26,86 +32,86 @@
 ]
 
 
 class UnitTests(unittest.TestCase):
 
     """Unit tests."""
 
-    def test_imports(self):
+    def test_imports(self) -> None:
         self.assertGreater(len(autoflake.SAFE_IMPORTS), 0)
 
-    def test_unused_import_line_numbers(self):
+    def test_unused_import_line_numbers(self) -> None:
         self.assertEqual(
             [1],
             list(
                 autoflake.unused_import_line_numbers(
                     autoflake.check("import os\n"),
                 ),
             ),
         )
 
-    def test_unused_import_line_numbers_with_from(self):
+    def test_unused_import_line_numbers_with_from(self) -> None:
         self.assertEqual(
             [1],
             list(
                 autoflake.unused_import_line_numbers(
                     autoflake.check("from os import path\n"),
                 ),
             ),
         )
 
-    def test_unused_import_line_numbers_with_dot(self):
+    def test_unused_import_line_numbers_with_dot(self) -> None:
         self.assertEqual(
             [1],
             list(
                 autoflake.unused_import_line_numbers(
                     autoflake.check("import os.path\n"),
                 ),
             ),
         )
 
-    def test_extract_package_name(self):
+    def test_extract_package_name(self) -> None:
         self.assertEqual("os", autoflake.extract_package_name("import os"))
         self.assertEqual(
             "os",
             autoflake.extract_package_name("from os import path"),
         )
         self.assertEqual(
             "os",
             autoflake.extract_package_name("import os.path"),
         )
 
-    def test_extract_package_name_should_ignore_doctest_for_now(self):
+    def test_extract_package_name_should_ignore_doctest_for_now(self) -> None:
         self.assertFalse(autoflake.extract_package_name(">>> import os"))
 
-    def test_standard_package_names(self):
+    def test_standard_package_names(self) -> None:
         self.assertIn("os", list(autoflake.standard_package_names()))
         self.assertIn("subprocess", list(autoflake.standard_package_names()))
         self.assertIn("urllib", list(autoflake.standard_package_names()))
 
         self.assertNotIn("autoflake", list(autoflake.standard_package_names()))
         self.assertNotIn("pep8", list(autoflake.standard_package_names()))
 
-    def test_get_line_ending(self):
+    def test_get_line_ending(self) -> None:
         self.assertEqual("\n", autoflake.get_line_ending("\n"))
         self.assertEqual("\n", autoflake.get_line_ending("abc\n"))
         self.assertEqual("\t  \t\n", autoflake.get_line_ending("abc\t  \t\n"))
 
         self.assertEqual("", autoflake.get_line_ending("abc"))
         self.assertEqual("", autoflake.get_line_ending(""))
 
-    def test_get_indentation(self):
+    def test_get_indentation(self) -> None:
         self.assertEqual("", autoflake.get_indentation(""))
         self.assertEqual("    ", autoflake.get_indentation("    abc"))
         self.assertEqual("    ", autoflake.get_indentation("    abc  \n\t"))
         self.assertEqual("\t", autoflake.get_indentation("\tabc  \n\t"))
         self.assertEqual(" \t ", autoflake.get_indentation(" \t abc  \n\t"))
         self.assertEqual("", autoflake.get_indentation("    "))
 
-    def test_filter_star_import(self):
+    def test_filter_star_import(self) -> None:
         self.assertEqual(
             "from math import cos",
             autoflake.filter_star_import(
                 "from math import *",
                 ["cos"],
             ),
         )
@@ -114,26 +120,26 @@
             "from math import cos, sin",
             autoflake.filter_star_import(
                 "from math import *",
                 ["sin", "cos"],
             ),
         )
 
-    def test_filter_unused_variable(self):
+    def test_filter_unused_variable(self) -> None:
         self.assertEqual(
             "foo()",
             autoflake.filter_unused_variable("x = foo()"),
         )
 
         self.assertEqual(
             "    foo()",
             autoflake.filter_unused_variable("    x = foo()"),
         )
 
-    def test_filter_unused_variable_with_literal_or_name(self):
+    def test_filter_unused_variable_with_literal_or_name(self) -> None:
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = 1"),
         )
 
         self.assertEqual(
             "pass",
@@ -141,15 +147,15 @@
         )
 
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = {}"),
         )
 
-    def test_filter_unused_variable_with_basic_data_structures(self):
+    def test_filter_unused_variable_with_basic_data_structures(self) -> None:
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = dict()"),
         )
 
         self.assertEqual(
             "pass",
@@ -157,40 +163,40 @@
         )
 
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = set()"),
         )
 
-    def test_filter_unused_variable_should_ignore_multiline(self):
+    def test_filter_unused_variable_should_ignore_multiline(self) -> None:
         self.assertEqual(
             "x = foo()\\",
             autoflake.filter_unused_variable("x = foo()\\"),
         )
 
-    def test_filter_unused_variable_should_multiple_assignments(self):
+    def test_filter_unused_variable_should_multiple_assignments(self) -> None:
         self.assertEqual(
             "x = y = foo()",
             autoflake.filter_unused_variable("x = y = foo()"),
         )
 
-    def test_filter_unused_variable_with_exception(self):
+    def test_filter_unused_variable_with_exception(self) -> None:
         self.assertEqual(
             "except Exception:",
             autoflake.filter_unused_variable("except Exception as exception:"),
         )
 
         self.assertEqual(
             "except (ImportError, ValueError):",
             autoflake.filter_unused_variable(
                 "except (ImportError, ValueError) as foo:",
             ),
         )
 
-    def test_filter_unused_variable_drop_rhs(self):
+    def test_filter_unused_variable_drop_rhs(self) -> None:
         self.assertEqual(
             "",
             autoflake.filter_unused_variable(
                 "x = foo()",
                 drop_rhs=True,
             ),
         )
@@ -199,15 +205,15 @@
             "",
             autoflake.filter_unused_variable(
                 "    x = foo()",
                 drop_rhs=True,
             ),
         )
 
-    def test_filter_unused_variable_with_literal_or_name_drop_rhs(self):
+    def test_filter_unused_variable_with_literal_or_name_drop_rhs(self) -> None:
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = 1", drop_rhs=True),
         )
 
         self.assertEqual(
             "pass",
@@ -215,15 +221,15 @@
         )
 
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = {}", drop_rhs=True),
         )
 
-    def test_filter_unused_variable_with_basic_data_structures_drop_rhs(self):
+    def test_filter_unused_variable_with_basic_data_structures_drop_rhs(self) -> None:
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = dict()", drop_rhs=True),
         )
 
         self.assertEqual(
             "pass",
@@ -231,27 +237,27 @@
         )
 
         self.assertEqual(
             "pass",
             autoflake.filter_unused_variable("x = set()", drop_rhs=True),
         )
 
-    def test_filter_unused_variable_should_ignore_multiline_drop_rhs(self):
+    def test_filter_unused_variable_should_ignore_multiline_drop_rhs(self) -> None:
         self.assertEqual(
             "x = foo()\\",
             autoflake.filter_unused_variable("x = foo()\\", drop_rhs=True),
         )
 
-    def test_filter_unused_variable_should_multiple_assignments_drop_rhs(self):
+    def test_filter_unused_variable_should_multiple_assignments_drop_rhs(self) -> None:
         self.assertEqual(
             "x = y = foo()",
             autoflake.filter_unused_variable("x = y = foo()", drop_rhs=True),
         )
 
-    def test_filter_unused_variable_with_exception_drop_rhs(self):
+    def test_filter_unused_variable_with_exception_drop_rhs(self) -> None:
         self.assertEqual(
             "except Exception:",
             autoflake.filter_unused_variable(
                 "except Exception as exception:",
                 drop_rhs=True,
             ),
         )
@@ -260,15 +266,15 @@
             "except (ImportError, ValueError):",
             autoflake.filter_unused_variable(
                 "except (ImportError, ValueError) as foo:",
                 drop_rhs=True,
             ),
         )
 
-    def test_filter_code(self):
+    def test_filter_code(self) -> None:
         self.assertEqual(
             """\
 import os
 pass
 os.foo()
 """,
             "".join(
@@ -278,15 +284,15 @@
 import re
 os.foo()
 """,
                 ),
             ),
         )
 
-    def test_filter_code_with_indented_import(self):
+    def test_filter_code_with_indented_import(self) -> None:
         self.assertEqual(
             """\
 import os
 if True:
     pass
 os.foo()
 """,
@@ -298,15 +304,15 @@
     import re
 os.foo()
 """,
                 ),
             ),
         )
 
-    def test_filter_code_with_from(self):
+    def test_filter_code_with_from(self) -> None:
         self.assertEqual(
             """\
 pass
 x = 1
 """,
             "".join(
                 autoflake.filter_code(
@@ -314,15 +320,15 @@
 from os import path
 x = 1
 """,
                 ),
             ),
         )
 
-    def test_filter_code_with_not_from(self):
+    def test_filter_code_with_not_from(self) -> None:
         self.assertEqual(
             """\
 pass
 x = 1
 """,
             "".join(
                 autoflake.filter_code(
@@ -331,15 +337,15 @@
 x = 1
 """,
                     remove_all_unused_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_with_used_from(self):
+    def test_filter_code_with_used_from(self) -> None:
         self.assertEqual(
             """\
 import frommer
 print(frommer)
 """,
             "".join(
                 autoflake.filter_code(
@@ -348,45 +354,45 @@
 print(frommer)
 """,
                     remove_all_unused_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_with_ambiguous_from(self):
+    def test_filter_code_with_ambiguous_from(self) -> None:
         self.assertEqual(
             """\
 pass
 """,
             "".join(
                 autoflake.filter_code(
                     """\
 from frommer import abc, frommer, xyz
 """,
                     remove_all_unused_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_should_avoid_inline_except(self):
+    def test_filter_code_should_avoid_inline_except(self) -> None:
         line = """\
 try: from zap import foo
 except: from zap import bar
 """
         self.assertEqual(
             line,
             "".join(
                 autoflake.filter_code(
                     line,
                     remove_all_unused_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_should_avoid_escaped_newlines(self):
+    def test_filter_code_should_avoid_escaped_newlines(self) -> None:
         line = """\
 try:\\
 from zap import foo
 except:\\
 from zap import bar
 """
         self.assertEqual(
@@ -395,15 +401,15 @@
                 autoflake.filter_code(
                     line,
                     remove_all_unused_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_with_remove_all_unused_imports(self):
+    def test_filter_code_with_remove_all_unused_imports(self) -> None:
         self.assertEqual(
             """\
 pass
 pass
 x = 1
 """,
             "".join(
@@ -414,15 +420,15 @@
 x = 1
 """,
                     remove_all_unused_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_with_additional_imports(self):
+    def test_filter_code_with_additional_imports(self) -> None:
         self.assertEqual(
             """\
 pass
 import zap
 x = 1
 """,
             "".join(
@@ -433,15 +439,15 @@
 x = 1
 """,
                     additional_imports=["foo", "bar"],
                 ),
             ),
         )
 
-    def test_filter_code_should_ignore_imports_with_inline_comment(self):
+    def test_filter_code_should_ignore_imports_with_inline_comment(self) -> None:
         self.assertEqual(
             """\
 from os import path  # foo
 pass
 from fake_foo import z  # foo, foo, zap
 x = 1
 """,
@@ -453,15 +459,15 @@
 from fake_foo import z  # foo, foo, zap
 x = 1
 """,
                 ),
             ),
         )
 
-    def test_filter_code_should_respect_noqa(self):
+    def test_filter_code_should_respect_noqa(self) -> None:
         self.assertEqual(
             """\
 pass
 import re  # noqa
 from subprocess import Popen  # NOQA
 x = 1
 """,
@@ -473,15 +479,15 @@
 from subprocess import Popen  # NOQA
 x = 1
 """,
                 ),
             ),
         )
 
-    def test_filter_code_expand_star_imports(self):
+    def test_filter_code_expand_star_imports(self) -> None:
         self.assertEqual(
             """\
 from math import sin
 sin(1)
 """,
             "".join(
                 autoflake.filter_code(
@@ -508,15 +514,15 @@
 cos(1)
 """,
                     expand_star_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_ignore_multiple_star_import(self):
+    def test_filter_code_ignore_multiple_star_import(self) -> None:
         self.assertEqual(
             """\
 from math import *
 from re import *
 sin(1)
 cos(1)
 """,
@@ -529,15 +535,15 @@
 cos(1)
 """,
                     expand_star_imports=True,
                 ),
             ),
         )
 
-    def test_filter_code_with_special_re_symbols_in_key(self):
+    def test_filter_code_with_special_re_symbols_in_key(self) -> None:
         self.assertEqual(
             """\
 a = {
   '????': 2,
 }
 print(a)
 """,
@@ -551,15 +557,15 @@
 print(a)
 """,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_multiline_import(self):
+    def test_multiline_import(self) -> None:
         self.assertTrue(
             autoflake.multiline_import(
                 r"""\
 import os, \
     math, subprocess
 """,
             ),
@@ -582,79 +588,79 @@
             ),
         )
 
         self.assertTrue(
             autoflake.multiline_import("from os import (path, sep)"),
         )
 
-    def test_multiline_statement(self):
+    def test_multiline_statement(self) -> None:
         self.assertFalse(autoflake.multiline_statement("x = foo()"))
 
         self.assertTrue(autoflake.multiline_statement("x = 1;"))
         self.assertTrue(autoflake.multiline_statement("import os, \\"))
         self.assertTrue(autoflake.multiline_statement("foo("))
         self.assertTrue(
             autoflake.multiline_statement(
                 "1",
                 previous_line="x = \\",
             ),
         )
 
-    def test_break_up_import(self):
+    def test_break_up_import(self) -> None:
         self.assertEqual(
             "import abc\nimport subprocess\nimport math\n",
             autoflake.break_up_import("import abc, subprocess, math\n"),
         )
 
-    def test_break_up_import_with_indentation(self):
+    def test_break_up_import_with_indentation(self) -> None:
         self.assertEqual(
             "    import abc\n    import subprocess\n    import math\n",
             autoflake.break_up_import("    import abc, subprocess, math\n"),
         )
 
-    def test_break_up_import_should_do_nothing_on_no_line_ending(self):
+    def test_break_up_import_should_do_nothing_on_no_line_ending(self) -> None:
         self.assertEqual(
             "import abc, subprocess, math",
             autoflake.break_up_import("import abc, subprocess, math"),
         )
 
-    def test_filter_from_import_no_remove(self):
+    def test_filter_from_import_no_remove(self) -> None:
         self.assertEqual(
             """\
     from foo import abc, subprocess, math\n""",
             autoflake.filter_from_import(
                 "    from foo import abc, subprocess, math\n",
                 unused_module=[],
             ),
         )
 
-    def test_filter_from_import_remove_module(self):
+    def test_filter_from_import_remove_module(self) -> None:
         self.assertEqual(
             """\
     from foo import subprocess, math\n""",
             autoflake.filter_from_import(
                 "    from foo import abc, subprocess, math\n",
                 unused_module=["foo.abc"],
             ),
         )
 
-    def test_filter_from_import_remove_all(self):
+    def test_filter_from_import_remove_all(self) -> None:
         self.assertEqual(
             "    pass\n",
             autoflake.filter_from_import(
                 "    from foo import abc, subprocess, math\n",
                 unused_module=[
                     "foo.abc",
                     "foo.subprocess",
                     "foo.math",
                 ],
             ),
         )
 
-    def test_filter_code_multiline_imports(self):
+    def test_filter_code_multiline_imports(self) -> None:
         self.assertEqual(
             r"""\
 import os
 pass
 import os
 os.foo()
 """,
@@ -667,15 +673,15 @@
     math, subprocess
 os.foo()
 """,
                 ),
             ),
         )
 
-    def test_filter_code_multiline_from_imports(self):
+    def test_filter_code_multiline_from_imports(self) -> None:
         self.assertEqual(
             r"""\
 import os
 pass
 from os.path import (
     join,
 )
@@ -705,15 +711,15 @@
     , isdir
 isdir('42')
 """,
                 ),
             ),
         )
 
-    def test_filter_code_should_ignore_semicolons(self):
+    def test_filter_code_should_ignore_semicolons(self) -> None:
         self.assertEqual(
             r"""\
 import os
 pass
 import os; import math, subprocess
 os.foo()
 """,
@@ -725,15 +731,15 @@
 import os; import math, subprocess
 os.foo()
 """,
                 ),
             ),
         )
 
-    def test_filter_code_should_ignore_non_standard_library(self):
+    def test_filter_code_should_ignore_non_standard_library(self) -> None:
         self.assertEqual(
             """\
 import os
 import my_own_module
 pass
 from my_package import another_module
 from my_package import subprocess
@@ -751,15 +757,15 @@
 from my_blah.my_blah_blah import blah
 os.foo()
 """,
                 ),
             ),
         )
 
-    def test_filter_code_should_ignore_unsafe_imports(self):
+    def test_filter_code_should_ignore_unsafe_imports(self) -> None:
         self.assertEqual(
             """\
 import rlcompleter
 pass
 pass
 pass
 print(1)
@@ -773,24 +779,24 @@
 import os
 print(1)
 """,
                 ),
             ),
         )
 
-    def test_filter_code_should_ignore_docstring(self):
+    def test_filter_code_should_ignore_docstring(self) -> None:
         line = """
-def foo():
+def foo() -> None:
     '''
     >>> import math
     '''
 """
         self.assertEqual(line, "".join(autoflake.filter_code(line)))
 
-    def test_with_ignore_init_module_imports_flag(self):
+    def test_with_ignore_init_module_imports_flag(self) -> None:
         # Need a temp directory in order to specify file name as __init__.py
         temp_directory = tempfile.mkdtemp(dir=".")
         temp_file = os.path.join(temp_directory, "__init__.py")
         try:
             with open(temp_file, "w") as output:
                 output.write("import re\n")
 
@@ -800,15 +806,15 @@
             )
             result = p.communicate()[0].decode("utf-8")
 
             self.assertNotIn("import re", result)
         finally:
             shutil.rmtree(temp_directory)
 
-    def test_without_ignore_init_module_imports_flag(self):
+    def test_without_ignore_init_module_imports_flag(self) -> None:
         # Need a temp directory in order to specify file name as __init__.py
         temp_directory = tempfile.mkdtemp(dir=".")
         temp_file = os.path.join(temp_directory, "__init__.py")
         try:
             with open(temp_file, "w") as output:
                 output.write("import re\n")
 
@@ -818,15 +824,15 @@
             )
             result = p.communicate()[0].decode("utf-8")
 
             self.assertIn("import re", result)
         finally:
             shutil.rmtree(temp_directory)
 
-    def test_fix_code(self):
+    def test_fix_code(self) -> None:
         self.assertEqual(
             """\
 import os
 import math
 from sys import version
 os.foo()
 math.pi
@@ -841,15 +847,15 @@
 os.foo()
 math.pi
 x = version
 """,
             ),
         )
 
-    def test_fix_code_with_from_and_as(self):
+    def test_fix_code_with_from_and_as(self) -> None:
         self.assertEqual(
             """\
 from collections import namedtuple as xyz
 xyz
 """,
             autoflake.fix_code(
                 """\
@@ -891,15 +897,15 @@
             autoflake.fix_code(
                 """\
 from collections import defaultdict as abc, namedtuple as xyz
 """,
             ),
         )
 
-    def test_fix_code_with_from_with_and_without_remove_all(self):
+    def test_fix_code_with_from_with_and_without_remove_all(self) -> None:
         code = """\
 from x import a as b, c as d
 """
 
         self.assertEqual(
             """\
 """,
@@ -907,15 +913,15 @@
         )
 
         self.assertEqual(
             code,
             autoflake.fix_code(code, remove_all_unused_imports=False),
         )
 
-    def test_fix_code_with_from_and_depth_module(self):
+    def test_fix_code_with_from_and_depth_module(self) -> None:
         self.assertEqual(
             """\
 from distutils.version import StrictVersion
 StrictVersion('1.0.0')
 """,
             autoflake.fix_code(
                 """\
@@ -934,50 +940,50 @@
                 """\
 from distutils.version import LooseVersion, StrictVersion as version
 version('1.0.0')
 """,
             ),
         )
 
-    def test_fix_code_with_indented_from(self):
+    def test_fix_code_with_indented_from(self) -> None:
         self.assertEqual(
             """\
-def z():
+def z() -> None:
     from ctypes import POINTER, byref
     POINTER, byref
     """,
             autoflake.fix_code(
                 """\
-def z():
+def z() -> None:
     from ctypes import c_short, c_uint, c_int, c_long, pointer, POINTER, byref
     POINTER, byref
     """,
             ),
         )
 
         self.assertEqual(
             """\
-def z():
+def z() -> None:
     pass
 """,
             autoflake.fix_code(
                 """\
-def z():
+def z() -> None:
     from ctypes import c_short, c_uint, c_int, c_long, pointer, POINTER, byref
 """,
             ),
         )
 
-    def test_fix_code_with_empty_string(self):
+    def test_fix_code_with_empty_string(self) -> None:
         self.assertEqual(
             "",
             autoflake.fix_code(""),
         )
 
-    def test_fix_code_with_from_and_as_and_escaped_newline(self):
+    def test_fix_code_with_from_and_as_and_escaped_newline(self) -> None:
         """Make sure stuff after escaped newline is not lost."""
         result = autoflake.fix_code(
             """\
 from collections import defaultdict, namedtuple \\
     as xyz
 xyz
 """,
@@ -991,58 +997,58 @@
             """\
 from collections import namedtuple as xyz
 xyz
 """,
             autoflake.fix_code(result),
         )
 
-    def test_fix_code_with_unused_variables(self):
+    def test_fix_code_with_unused_variables(self) -> None:
         self.assertEqual(
             """\
-def main():
+def main() -> None:
     y = 11
     print(y)
 """,
             autoflake.fix_code(
                 """\
-def main():
+def main() -> None:
     x = 10
     y = 11
     print(y)
 """,
                 remove_unused_variables=True,
             ),
         )
 
-    def test_fix_code_with_unused_variables_drop_rhs(self):
+    def test_fix_code_with_unused_variables_drop_rhs(self) -> None:
         self.assertEqual(
             """\
-def main():
+def main() -> None:
     y = 11
     print(y)
 """,
             autoflake.fix_code(
                 """\
-def main():
+def main() -> None:
     x = 10
     y = 11
     print(y)
 """,
                 remove_unused_variables=True,
                 remove_rhs_for_unused_variables=True,
             ),
         )
 
-    def test_fix_code_with_unused_variables_should_skip_nonlocal(self):
+    def test_fix_code_with_unused_variables_should_skip_nonlocal(self) -> None:
         """pyflakes does not handle nonlocal correctly."""
         code = """\
-def bar():
+def bar() -> None:
     x = 1
 
-    def foo():
+    def foo() -> None:
         nonlocal x
         x = 2
 """
         self.assertEqual(
             code,
             autoflake.fix_code(
                 code,
@@ -1051,73 +1057,73 @@
         )
 
     def test_fix_code_with_unused_variables_should_skip_nonlocal_drop_rhs(
         self,
     ):
         """pyflakes does not handle nonlocal correctly."""
         code = """\
-def bar():
+def bar() -> None:
     x = 1
 
-    def foo():
+    def foo() -> None:
         nonlocal x
         x = 2
 """
         self.assertEqual(
             code,
             autoflake.fix_code(
                 code,
                 remove_unused_variables=True,
                 remove_rhs_for_unused_variables=True,
             ),
         )
 
-    def test_detect_encoding_with_bad_encoding(self):
+    def test_detect_encoding_with_bad_encoding(self) -> None:
         with temporary_file("# -*- coding: blah -*-\n") as filename:
             self.assertEqual(
                 "latin-1",
                 autoflake.detect_encoding(filename),
             )
 
-    def test_fix_code_with_comma_on_right(self):
+    def test_fix_code_with_comma_on_right(self) -> None:
         """pyflakes does not handle nonlocal correctly."""
         self.assertEqual(
             """\
-def main():
+def main() -> None:
     pass
 """,
             autoflake.fix_code(
                 """\
-def main():
+def main() -> None:
     x = (1, 2, 3)
 """,
                 remove_unused_variables=True,
             ),
         )
 
-    def test_fix_code_with_comma_on_right_drop_rhs(self):
+    def test_fix_code_with_comma_on_right_drop_rhs(self) -> None:
         """pyflakes does not handle nonlocal correctly."""
         self.assertEqual(
             """\
-def main():
+def main() -> None:
     pass
 """,
             autoflake.fix_code(
                 """\
-def main():
+def main() -> None:
     x = (1, 2, 3)
 """,
                 remove_unused_variables=True,
                 remove_rhs_for_unused_variables=True,
             ),
         )
 
-    def test_fix_code_with_unused_variables_should_skip_multiple(self):
+    def test_fix_code_with_unused_variables_should_skip_multiple(self) -> None:
         code = """\
-def main():
+def main() -> None:
     (x, y, z) = (1, 2, 3)
     print(z)
 """
         self.assertEqual(
             code,
             autoflake.fix_code(
                 code,
@@ -1125,35 +1131,35 @@
             ),
         )
 
     def test_fix_code_with_unused_variables_should_skip_multiple_drop_rhs(
         self,
     ):
         code = """\
-def main():
+def main() -> None:
     (x, y, z) = (1, 2, 3)
     print(z)
 """
         self.assertEqual(
             code,
             autoflake.fix_code(
                 code,
                 remove_unused_variables=True,
                 remove_rhs_for_unused_variables=True,
             ),
         )
 
-    def test_fix_code_should_handle_pyflakes_recursion_error_gracefully(self):
+    def test_fix_code_should_handle_pyflakes_recursion_error_gracefully(self) -> None:
         code = "x = [{}]".format("+".join(["abc" for _ in range(2000)]))
         self.assertEqual(
             code,
             autoflake.fix_code(code),
         )
 
-    def test_fix_code_with_duplicate_key(self):
+    def test_fix_code_with_duplicate_key(self) -> None:
         self.assertEqual(
             """\
 a = {
   (0,1): 3,
 }
 print(a)
 """,
@@ -1168,15 +1174,15 @@
 print(a)
 """,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_with_duplicate_key_longer(self):
+    def test_fix_code_with_duplicate_key_longer(self) -> None:
         self.assertEqual(
             """\
 {
     'a': 0,
     'c': 2,
     'd': 3,
     'e': 4,
@@ -1198,15 +1204,15 @@
 }
 """,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_with_duplicate_key_with_many_braces(self):
+    def test_fix_code_with_duplicate_key_with_many_braces(self) -> None:
         self.assertEqual(
             """\
 a = None
 
 {None: {None: None},
  }
 
@@ -1228,15 +1234,15 @@
 }
 """,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_should_ignore_complex_case_of_duplicate_key(self):
+    def test_fix_code_should_ignore_complex_case_of_duplicate_key(self) -> None:
         """We only handle simple cases."""
         code = """\
 a = {(0,1): 1, (0, 1): 'two',
   (0,1): 3,
 }
 print(a)
 """
@@ -1247,15 +1253,15 @@
                 autoflake.fix_code(
                     code,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_should_ignore_complex_case_of_duplicate_key_comma(self):
+    def test_fix_code_should_ignore_complex_case_of_duplicate_key_comma(self) -> None:
         """We only handle simple cases."""
         code = """\
 {
     1: {0,
     },
     1: {2,
     },
@@ -1298,15 +1304,15 @@
                 autoflake.fix_code(
                     code,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_should_ignore_more_cases_of_duplicate_key(self):
+    def test_fix_code_should_ignore_more_cases_of_duplicate_key(self) -> None:
         """We only handle simple cases."""
         code = """\
 a = {
     (0,1):
     1,
     (0, 1): 'two',
   (0,1): 3,
@@ -1320,15 +1326,15 @@
                 autoflake.fix_code(
                     code,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_should_ignore_duplicate_key_with_comments(self):
+    def test_fix_code_should_ignore_duplicate_key_with_comments(self) -> None:
         """We only handle simple cases."""
         code = """\
 a = {
     (0,1)  # : f
     :
     1,
     (0, 1): 'two',
@@ -1363,15 +1369,15 @@
                 autoflake.fix_code(
                     code,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_should_ignore_duplicate_key_with_multiline_key(self):
+    def test_fix_code_should_ignore_duplicate_key_with_multiline_key(self) -> None:
         """We only handle simple cases."""
         code = """\
 a = {
     (0,1
     ): 1,
     (0, 1): 'two',
   (0,1): 3,
@@ -1385,15 +1391,15 @@
                 autoflake.fix_code(
                     code,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_should_ignore_duplicate_key_with_no_comma(self):
+    def test_fix_code_should_ignore_duplicate_key_with_no_comma(self) -> None:
         """We don't want to delete the line and leave a lone comma."""
         code = """\
 a = {
     (0,1) : 1
     ,
     (0, 1): 'two',
   (0,1): 3,
@@ -1407,35 +1413,35 @@
                 autoflake.fix_code(
                     code,
                     remove_duplicate_keys=True,
                 ),
             ),
         )
 
-    def test_fix_code_keeps_pass_statements(self):
+    def test_fix_code_keeps_pass_statements(self) -> None:
         code = """\
     if True:
         pass
     else:
-        def foo():
+        def foo() -> None:
             \"\"\" A docstring. \"\"\"
             pass
-        def foo2():
+        def foo2() -> None:
             \"\"\" A docstring. \"\"\"
 
             pass
-        def foo3():
+        def foo3() -> None:
             \"\"\" A docstring. \"\"\"
 
 
             pass
-        def bar():
+        def bar() -> None:
             # abc
             pass
-        def blah():
+        def blah() -> None:
             123
             pass
             pass  # Nope.
             pass
     """
 
         self.assertEqual(
@@ -1444,71 +1450,71 @@
                 autoflake.fix_code(
                     code,
                     ignore_pass_statements=True,
                 ),
             ),
         )
 
-    def test_fix_code_keeps_passes_after_docstrings(self):
+    def test_fix_code_keeps_passes_after_docstrings(self) -> None:
         actual = autoflake.fix_code(
             """\
     if True:
         pass
     else:
-        def foo():
+        def foo() -> None:
             \"\"\" A docstring. \"\"\"
             pass
-        def foo2():
+        def foo2() -> None:
             \"\"\" A docstring. \"\"\"
 
             pass
-        def foo3():
+        def foo3() -> None:
             \"\"\" A docstring. \"\"\"
 
 
             pass
-        def bar():
+        def bar() -> None:
             # abc
             pass
-        def blah():
+        def blah() -> None:
             123
             pass
             pass  # Nope.
             pass
     """,
             ignore_pass_after_docstring=True,
         )
 
         expected = """\
     if True:
         pass
     else:
-        def foo():
+        def foo() -> None:
             \"\"\" A docstring. \"\"\"
             pass
-        def foo2():
+        def foo2() -> None:
             \"\"\" A docstring. \"\"\"
 
             pass
-        def foo3():
+        def foo3() -> None:
             \"\"\" A docstring. \"\"\"
 
 
             pass
-        def bar():
+        def bar() -> None:
             # abc
             pass
-        def blah():
+        def blah() -> None:
             123
             pass  # Nope.
     """
 
         self.assertEqual(actual, expected)
 
-    def test_useless_pass_line_numbers(self):
+    def test_useless_pass_line_numbers(self) -> None:
         self.assertEqual(
             [1],
             list(
                 autoflake.useless_pass_line_numbers(
                     "pass\n",
                 ),
             ),
@@ -1519,25 +1525,25 @@
             list(
                 autoflake.useless_pass_line_numbers(
                     "if True:\n    pass\n",
                 ),
             ),
         )
 
-    def test_useless_pass_line_numbers_with_escaped_newline(self):
+    def test_useless_pass_line_numbers_with_escaped_newline(self) -> None:
         self.assertEqual(
             [],
             list(
                 autoflake.useless_pass_line_numbers(
                     "if True:\\\n    pass\n",
                 ),
             ),
         )
 
-    def test_useless_pass_line_numbers_with_more_complex(self):
+    def test_useless_pass_line_numbers_with_more_complex(self) -> None:
         self.assertEqual(
             [6],
             list(
                 autoflake.useless_pass_line_numbers(
                     """\
 if True:
     pass
@@ -1546,46 +1552,46 @@
     x = 1
     pass
 """,
                 ),
             ),
         )
 
-    def test_useless_pass_line_numbers_after_docstring(self):
+    def test_useless_pass_line_numbers_after_docstring(self) -> None:
         actual_pass_line_numbers = list(
             autoflake.useless_pass_line_numbers(
                 """\
     @abc.abstractmethod
-    def some_abstract_method():
+    def some_abstract_method() -> None:
         \"\"\"Some docstring.\"\"\"
         pass
     """,
             ),
         )
 
         expected_pass_line_numbers = [4]
         self.assertEqual(expected_pass_line_numbers, actual_pass_line_numbers)
 
-    def test_useless_pass_line_numbers_keep_pass_after_docstring(self):
+    def test_useless_pass_line_numbers_keep_pass_after_docstring(self) -> None:
         actual_pass_line_numbers = list(
             autoflake.useless_pass_line_numbers(
                 """\
     @abc.abstractmethod
-    def some_abstract_method():
+    def some_abstract_method() -> None:
         \"\"\"Some docstring.\"\"\"
         pass
     """,
                 ignore_pass_after_docstring=True,
             ),
         )
 
         expected_pass_line_numbers = []
         self.assertEqual(expected_pass_line_numbers, actual_pass_line_numbers)
 
-    def test_filter_useless_pass(self):
+    def test_filter_useless_pass(self) -> None:
         self.assertEqual(
             """\
 if True:
     pass
 else:
     True
     x = 1
@@ -1600,15 +1606,15 @@
     x = 1
     pass
 """,
                 ),
             ),
         )
 
-    def test_filter_useless_pass_with_syntax_error(self):
+    def test_filter_useless_pass_with_syntax_error(self) -> None:
         source = """\
 if True:
 if True:
             if True:
     if True:
 
 if True:
@@ -1621,65 +1627,65 @@
 """
 
         self.assertEqual(
             source,
             "".join(autoflake.filter_useless_pass(source)),
         )
 
-    def test_filter_useless_pass_more_complex(self):
+    def test_filter_useless_pass_more_complex(self) -> None:
         self.assertEqual(
             """\
 if True:
     pass
 else:
-    def foo():
+    def foo() -> None:
         pass
         # abc
-    def bar():
+    def bar() -> None:
         # abc
         pass
-    def blah():
+    def blah() -> None:
         123
         pass  # Nope.
     True
     x = 1
 """,
             "".join(
                 autoflake.filter_useless_pass(
                     """\
 if True:
     pass
 else:
-    def foo():
+    def foo() -> None:
         pass
         # abc
-    def bar():
+    def bar() -> None:
         # abc
         pass
-    def blah():
+    def blah() -> None:
         123
         pass
         pass  # Nope.
         pass
     True
     x = 1
     pass
 """,
                 ),
             ),
         )
 
-    def test_filter_useless_pass_keep_pass_after_docstring(self):
+    def test_filter_useless_pass_keep_pass_after_docstring(self) -> None:
         source = """\
-    def foo():
+    def foo() -> None:
         \"\"\" This is not a useless 'pass'. \"\"\"
         pass
 
     @abc.abstractmethod
-    def bar():
+    def bar() -> None:
         \"\"\"
             Also this is not a useless 'pass'.
         \"\"\"
         pass
     """
         self.assertEqual(
             source,
@@ -1687,15 +1693,15 @@
                 autoflake.filter_useless_pass(
                     source,
                     ignore_pass_after_docstring=True,
                 ),
             ),
         )
 
-    def test_filter_useless_pass_keeps_pass_statements(self):
+    def test_filter_useless_pass_keeps_pass_statements(self) -> None:
         source = """\
     if True:
         pass
         pass
         pass
         pass
     else:
@@ -1711,15 +1717,15 @@
                 autoflake.filter_useless_pass(
                     source,
                     ignore_pass_statements=True,
                 ),
             ),
         )
 
-    def test_filter_useless_paspasss_with_try(self):
+    def test_filter_useless_paspasss_with_try(self) -> None:
         self.assertEqual(
             """\
 import os
 os.foo()
 try:
     pass
 except ImportError:
@@ -1736,15 +1742,15 @@
 except ImportError:
     pass
 """,
                 ),
             ),
         )
 
-    def test_filter_useless_pass_leading_pass(self):
+    def test_filter_useless_pass_leading_pass(self) -> None:
         self.assertEqual(
             """\
 if True:
     pass
 else:
     True
     x = 1
@@ -1763,101 +1769,101 @@
     x = 1
     pass
 """,
                 ),
             ),
         )
 
-    def test_filter_useless_pass_leading_pass_with_number(self):
+    def test_filter_useless_pass_leading_pass_with_number(self) -> None:
         self.assertEqual(
             """\
-def func11():
+def func11() -> None:
     0, 11 / 2
     return 1
 """,
             "".join(
                 autoflake.filter_useless_pass(
                     """\
-def func11():
+def func11() -> None:
     pass
     0, 11 / 2
     return 1
 """,
                 ),
             ),
         )
 
-    def test_filter_useless_pass_leading_pass_with_string(self):
+    def test_filter_useless_pass_leading_pass_with_string(self) -> None:
         self.assertEqual(
             """\
-def func11():
+def func11() -> None:
     'hello'
     return 1
 """,
             "".join(
                 autoflake.filter_useless_pass(
                     """\
-def func11():
+def func11() -> None:
     pass
     'hello'
     return 1
 """,
                 ),
             ),
         )
 
-    def test_check(self):
+    def test_check(self) -> None:
         self.assertTrue(autoflake.check("import os"))
 
-    def test_check_with_bad_syntax(self):
+    def test_check_with_bad_syntax(self) -> None:
         self.assertFalse(autoflake.check("foo("))
 
-    def test_check_with_unicode(self):
+    def test_check_with_unicode(self) -> None:
         self.assertFalse(autoflake.check('print("∑")'))
 
         self.assertTrue(autoflake.check("import os  # ∑"))
 
-    def test_get_diff_text(self):
+    def test_get_diff_text(self) -> None:
         # We ignore the first two lines since it differs on Python 2.6.
         self.assertEqual(
             """\
 -foo
 +bar
 """,
             "\n".join(
                 autoflake.get_diff_text(["foo\n"], ["bar\n"], "").split(
                     "\n",
                 )[3:],
             ),
         )
 
-    def test_get_diff_text_without_newline(self):
+    def test_get_diff_text_without_newline(self) -> None:
         # We ignore the first two lines since it differs on Python 2.6.
         self.assertEqual(
             """\
 -foo
 \\ No newline at end of file
 +foo
 """,
             "\n".join(
                 autoflake.get_diff_text(["foo"], ["foo\n"], "").split(
                     "\n",
                 )[3:],
             ),
         )
 
-    def test_is_literal_or_name(self):
+    def test_is_literal_or_name(self) -> None:
         self.assertTrue(autoflake.is_literal_or_name("123"))
         self.assertTrue(autoflake.is_literal_or_name("[1, 2, 3]"))
         self.assertTrue(autoflake.is_literal_or_name("xyz"))
 
         self.assertFalse(autoflake.is_literal_or_name("xyz.prop"))
         self.assertFalse(autoflake.is_literal_or_name(" "))
 
-    def test_is_python_file(self):
+    def test_is_python_file(self) -> None:
         self.assertTrue(
             autoflake.is_python_file(
                 os.path.join(ROOT_DIRECTORY, "autoflake.py"),
             ),
         )
 
         with temporary_file("#!/usr/bin/env python", suffix="") as filename:
@@ -1874,15 +1880,15 @@
 
         with temporary_file("###!/usr/bin/python", suffix="") as filename:
             self.assertFalse(autoflake.is_python_file(filename))
 
         self.assertFalse(autoflake.is_python_file(os.devnull))
         self.assertFalse(autoflake.is_python_file("/bin/bash"))
 
-    def test_is_exclude_file(self):
+    def test_is_exclude_file(self) -> None:
         self.assertTrue(
             autoflake.is_exclude_file(
                 "1.py",
                 ["test*", "1*"],
             ),
         )
 
@@ -1911,30 +1917,30 @@
         self.assertFalse(
             autoflake.is_exclude_file(
                 "test/auto_auto.py",
                 ["test/*_test.py"],
             ),
         )
 
-    def test_match_file(self):
+    def test_match_file(self) -> None:
         with temporary_file("", suffix=".py", prefix=".") as filename:
             self.assertFalse(
                 autoflake.match_file(filename, exclude=[]),
                 msg=filename,
             )
 
         self.assertFalse(autoflake.match_file(os.devnull, exclude=[]))
 
         with temporary_file("", suffix=".py", prefix="") as filename:
             self.assertTrue(
                 autoflake.match_file(filename, exclude=[]),
                 msg=filename,
             )
 
-    def test_find_files(self):
+    def test_find_files(self) -> None:
         temp_directory = tempfile.mkdtemp()
         try:
             target = os.path.join(temp_directory, "dir")
             os.mkdir(target)
             with open(os.path.join(target, "a.py"), "w"):
                 pass
 
@@ -1966,15 +1972,15 @@
             file_names = [os.path.basename(f) for f in files]
             self.assertIn("a.py", file_names)
             self.assertNotIn("b.py", file_names)
             self.assertNotIn("c.py", file_names)
         finally:
             shutil.rmtree(temp_directory)
 
-    def test_exclude(self):
+    def test_exclude(self) -> None:
         temp_directory = tempfile.mkdtemp(dir=".")
         try:
             with open(os.path.join(temp_directory, "a.py"), "w") as output:
                 output.write("import re\n")
 
             os.mkdir(os.path.join(temp_directory, "d"))
             with open(
@@ -1996,15 +2002,15 @@
             shutil.rmtree(temp_directory)
 
 
 class SystemTests(unittest.TestCase):
 
     """System tests."""
 
-    def test_diff(self):
+    def test_diff(self) -> None:
         with temporary_file(
             """\
 import re
 import os
 import my_own_module
 x = 1
 """,
@@ -2021,24 +2027,24 @@
 -import os
  import my_own_module
  x = 1
 """,
                 "\n".join(output_file.getvalue().split("\n")[3:]),
             )
 
-    def test_diff_with_nonexistent_file(self):
+    def test_diff_with_nonexistent_file(self) -> None:
         output_file = io.StringIO()
         autoflake._main(
             argv=["my_fake_program", "nonexistent_file"],
             standard_out=output_file,
             standard_error=output_file,
         )
         self.assertIn("no such file", output_file.getvalue().lower())
 
-    def test_diff_with_encoding_declaration(self):
+    def test_diff_with_encoding_declaration(self) -> None:
         with temporary_file(
             """\
 # coding: iso-8859-1
 import re
 import os
 import my_own_module
 x = 1
@@ -2057,15 +2063,15 @@
 -import os
  import my_own_module
  x = 1
 """,
                 "\n".join(output_file.getvalue().split("\n")[3:]),
             )
 
-    def test_in_place(self):
+    def test_in_place(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo
 import subprocess
 x()
 
@@ -2092,30 +2098,30 @@
     pass
 except ImportError:
     pass
 """,
                     f.read(),
                 )
 
-    def test_check_with_empty_file(self):
+    def test_check_with_empty_file(self) -> None:
         line = ""
 
         with temporary_file(line) as filename:
             output_file = io.StringIO()
             autoflake._main(
                 argv=["my_fake_program", "--check", filename],
                 standard_out=output_file,
                 standard_error=None,
             )
             self.assertEqual(
                 f"{filename}: No issues detected!{os.linesep}",
                 output_file.getvalue(),
             )
 
-    def test_check_correct_file(self):
+    def test_check_correct_file(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo.bar
 print(x)
 """,
         ) as filename:
@@ -2126,15 +2132,15 @@
                 standard_error=None,
             )
             self.assertEqual(
                 f"{filename}: No issues detected!{os.linesep}",
                 output_file.getvalue(),
             )
 
-    def test_check_correct_file_with_quiet(self):
+    def test_check_correct_file_with_quiet(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo.bar
 print(x)
 """,
         ) as filename:
@@ -2147,15 +2153,15 @@
                     filename,
                 ],
                 standard_out=output_file,
                 standard_error=None,
             )
             self.assertEqual("", output_file.getvalue())
 
-    def test_check_useless_pass(self):
+    def test_check_useless_pass(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo
 import subprocess
 x()
 
@@ -2176,15 +2182,15 @@
             )
             self.assertEqual(exit_status, 1)
             self.assertEqual(
                 f"{filename}: Unused imports/variables detected{os.linesep}",
                 output_file.getvalue(),
             )
 
-    def test_check_with_multiple_files(self):
+    def test_check_with_multiple_files(self) -> None:
         with temporary_file("import sys") as file1:
             with temporary_file("import sys") as file2:
                 output_file = io.StringIO()
                 exit_status = autoflake._main(
                     argv=["my_fake_program", "--check", file1, file2],
                     standard_out=output_file,
                     standard_error=None,
@@ -2194,30 +2200,30 @@
                     {
                         f"{file1}: Unused imports/variables detected",
                         f"{file2}: Unused imports/variables detected",
                     },
                     set(output_file.getvalue().strip().split(os.linesep)),
                 )
 
-    def test_check_diff_with_empty_file(self):
+    def test_check_diff_with_empty_file(self) -> None:
         line = ""
 
         with temporary_file(line) as filename:
             output_file = io.StringIO()
             autoflake._main(
                 argv=["my_fake_program", "--check-diff", filename],
                 standard_out=output_file,
                 standard_error=None,
             )
             self.assertEqual(
                 f"{filename}: No issues detected!{os.linesep}",
                 output_file.getvalue(),
             )
 
-    def test_check_diff_correct_file(self):
+    def test_check_diff_correct_file(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo.bar
 print(x)
 """,
         ) as filename:
@@ -2228,15 +2234,15 @@
                 standard_error=None,
             )
             self.assertEqual(
                 f"{filename}: No issues detected!{os.linesep}",
                 output_file.getvalue(),
             )
 
-    def test_check_diff_correct_file_with_quiet(self):
+    def test_check_diff_correct_file_with_quiet(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo.bar
 print(x)
 """,
         ) as filename:
@@ -2249,15 +2255,15 @@
                     filename,
                 ],
                 standard_out=output_file,
                 standard_error=None,
             )
             self.assertEqual("", output_file.getvalue())
 
-    def test_check_diff_useless_pass(self):
+    def test_check_diff_useless_pass(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo
 import subprocess
 x()
 try:
@@ -2289,28 +2295,28 @@
      pass
 -    import os
 -    import sys
 """,
                 "\n".join(output_file.getvalue().split("\n")[3:]),
             )
 
-    def test_in_place_with_empty_file(self):
+    def test_in_place_with_empty_file(self) -> None:
         line = ""
 
         with temporary_file(line) as filename:
             output_file = io.StringIO()
             autoflake._main(
                 argv=["my_fake_program", "--in-place", filename],
                 standard_out=output_file,
                 standard_error=None,
             )
             with open(filename) as f:
                 self.assertEqual(line, f.read())
 
-    def test_in_place_with_with_useless_pass(self):
+    def test_in_place_with_with_useless_pass(self) -> None:
         with temporary_file(
             """\
 import foo
 x = foo
 import subprocess
 x()
 
@@ -2340,25 +2346,25 @@
     pass
 except ImportError:
     pass
 """,
                     f.read(),
                 )
 
-    def test_with_missing_file(self):
+    def test_with_missing_file(self) -> None:
         output_file = io.StringIO()
         ignore = StubFile()
         autoflake._main(
             argv=["my_fake_program", "--in-place", ".fake"],
             standard_out=output_file,
-            standard_error=ignore,
+            standard_error=ignore,  # type: ignore
         )
         self.assertFalse(output_file.getvalue())
 
-    def test_ignore_hidden_directories(self):
+    def test_ignore_hidden_directories(self) -> None:
         with temporary_directory() as directory:
             with temporary_directory(
                 prefix=".",
                 directory=directory,
             ) as inner_directory:
                 with temporary_file(
                     """\
@@ -2378,25 +2384,25 @@
                         standard_error=None,
                     )
                     self.assertEqual(
                         "",
                         output_file.getvalue().strip(),
                     )
 
-    def test_in_place_and_stdout(self):
+    def test_in_place_and_stdout(self) -> None:
         output_file = io.StringIO()
         self.assertRaises(
             SystemExit,
             autoflake._main,
             argv=["my_fake_program", "--in-place", "--stdout", __file__],
             standard_out=output_file,
             standard_error=output_file,
         )
 
-    def test_end_to_end(self):
+    def test_end_to_end(self) -> None:
         with temporary_file(
             """\
 import fake_fake, fake_foo, fake_bar, fake_zoo
 import re, os
 x = os.sep
 print(x)
 """,
@@ -2418,15 +2424,15 @@
 +import os
  x = os.sep
  print(x)
 """,
                 "\n".join(process.communicate()[0].decode().split(os.linesep)[3:]),
             )
 
-    def test_end_to_end_multiple_files(self):
+    def test_end_to_end_multiple_files(self) -> None:
         with temporary_file(
             """\
 import fake_fake, fake_foo, fake_bar, fake_zoo
 import re, os
 x = os.sep
 print(x)
 """,
@@ -2449,15 +2455,15 @@
                     ],
                     stdout=subprocess.PIPE,
                 )
 
                 status_code = process.wait()
                 self.assertEqual(1, status_code)
 
-    def test_end_to_end_with_remove_all_unused_imports(self):
+    def test_end_to_end_with_remove_all_unused_imports(self) -> None:
         with temporary_file(
             """\
 import fake_fake, fake_foo, fake_bar, fake_zoo
 import re, os
 x = os.sep
 print(x)
 """,
@@ -2477,15 +2483,15 @@
 +import os
  x = os.sep
  print(x)
 """,
                 "\n".join(process.communicate()[0].decode().split(os.linesep)[3:]),
             )
 
-    def test_end_to_end_with_remove_duplicate_keys_multiple_lines(self):
+    def test_end_to_end_with_remove_duplicate_keys_multiple_lines(self) -> None:
         with temporary_file(
             """\
 a = {
     'b': 456,
     'a': 123,
     'b': 7834,
     'a': 'wow',
@@ -2517,15 +2523,15 @@
      'c': 'hello2',
      'b': 'hiya',
  }
 """,
                 "\n".join(process.communicate()[0].decode().split(os.linesep)[3:]),
             )
 
-    def test_end_to_end_with_remove_duplicate_keys_and_other_errors(self):
+    def test_end_to_end_with_remove_duplicate_keys_and_other_errors(self) -> None:
         with temporary_file(
             """\
 from math import *
 print(sin(4))
 a = { # Hello
     'b': 456,
     'a': 123,
@@ -2561,15 +2567,15 @@
      'c': 'hello2',
      'b': 'hiya',
  }
 """,
                 "\n".join(process.communicate()[0].decode().split(os.linesep)[3:]),
             )
 
-    def test_end_to_end_with_remove_duplicate_keys_tuple(self):
+    def test_end_to_end_with_remove_duplicate_keys_tuple(self) -> None:
         with temporary_file(
             """\
 a = {
   (0,1): 1,
   (0, 1): 'two',
   (0,1): 3,
 }
@@ -2592,15 +2598,15 @@
    (0,1): 3,
  }
  print(a)
 """,
                 "\n".join(process.communicate()[0].decode().split(os.linesep)[3:]),
             )
 
-    def test_end_to_end_with_error(self):
+    def test_end_to_end_with_error(self) -> None:
         with temporary_file(
             """\
 import fake_fake, fake_foo, fake_bar, fake_zoo
 import re, os
 x = os.sep
 print(x)
 """,
@@ -2615,15 +2621,15 @@
                 stderr=subprocess.PIPE,
             )
             self.assertIn(
                 "not allowed with argument",
                 process.communicate()[1].decode(),
             )
 
-    def test_end_to_end_from_stdin(self):
+    def test_end_to_end_from_stdin(self) -> None:
         stdin_data = b"""\
 import fake_fake, fake_foo, fake_bar, fake_zoo
 import re, os
 x = os.sep
 print(x)
 """
         process = subprocess.Popen(
@@ -2637,15 +2643,15 @@
 import os
 x = os.sep
 print(x)
 """,
             "\n".join(stdout.decode().split(os.linesep)),
         )
 
-    def test_end_to_end_from_stdin_with_in_place(self):
+    def test_end_to_end_from_stdin_with_in_place(self) -> None:
         stdin_data = b"""\
 import fake_fake, fake_foo, fake_bar, fake_zoo
 import re, os, sys
 x = os.sep
 print(x)
 """
         process = subprocess.Popen(
@@ -2659,15 +2665,15 @@
 import os
 x = os.sep
 print(x)
 """,
             "\n".join(stdout.decode().split(os.linesep)),
         )
 
-    def test_end_to_end_dont_remove_unused_imports_when_not_using_flag(self):
+    def test_end_to_end_dont_remove_unused_imports_when_not_using_flag(self) -> None:
         with temporary_file(
             """\
 from . import fake_bar
 from . import fake_foo
 fake_foo.fake_function()
 """,
         ) as filename:
@@ -2681,15 +2687,15 @@
             self.assertEqual(
                 "",
                 "\n".join(process.communicate()[0].decode().split(os.linesep)[3:]),
             )
 
 
 class MultilineFromImportTests(unittest.TestCase):
-    def test_is_over(self):
+    def test_is_over(self) -> None:
         filt = autoflake.FilterMultilineImport("from . import (\n")
         self.assertTrue(filt.is_over("module)\n"))
         self.assertTrue(filt.is_over("  )\n"))
         self.assertTrue(filt.is_over("  )  # comment\n"))
         self.assertTrue(filt.is_over("from module import (a, b)\n"))
         self.assertFalse(filt.is_over("#  )"))
         self.assertFalse(filt.is_over("module\n"))
@@ -2709,24 +2715,33 @@
         filt = autoflake.FilterMultilineImport(
             "import os; " "import math, subprocess",
         )
         self.assertTrue(filt.is_over())
 
     unused = ()
 
-    def assert_fix(self, lines, result, remove_all=True):
+    def assert_fix(
+        self,
+        lines: Sequence[str],
+        result: str,
+        remove_all: bool = True,
+    ) -> None:
         fixer = autoflake.FilterMultilineImport(
             lines[0],
             remove_all_unused_imports=remove_all,
             unused_module=self.unused,
         )
-        fixed = functools.reduce(lambda acc, x: acc(x), lines[1:], fixer())
+        fixed = functools.reduce(
+            lambda acc, x: acc(x) if isinstance(acc, autoflake.PendingFix) else acc,
+            lines[1:],
+            fixer(),
+        )
         self.assertEqual(fixed, result)
 
-    def test_fix(self):
+    def test_fix(self) -> None:
         self.unused = ["third_party.lib" + str(x) for x in (1, 3, 4)]
 
         # Example m0 (isort)
         self.assert_fix(
             [
                 "from third_party import (lib1, lib2, lib3,\n",
                 "                         lib4, lib5, lib6)\n",
@@ -2863,15 +2878,15 @@
             "from third_party import (\n"
             "    lib2 \\\n"
             ", \\\n"
             "    lib5 \\\n"
             ")\n",
         )
 
-    def test_indentation(self):
+    def test_indentation(self) -> None:
         # Some weird indentation examples
         self.unused = ["third_party.lib" + str(x) for x in (1, 3, 4)]
         self.assert_fix(
             [
                 "    from third_party import (\n",
                 "            lib1, lib2, lib3, lib4,\n",
                 "    lib5, lib6\n",
@@ -2884,15 +2899,15 @@
                 "\tfrom third_party import \\\n",
                 "\t\tlib1, lib2, lib3, \\\n",
                 "\t\tlib4, lib5, lib6\n",
             ],
             "\tfrom third_party import \\\n" "\t\tlib2, lib5, lib6\n",
         )
 
-    def test_fix_relative(self):
+    def test_fix_relative(self) -> None:
         # Example m0 (isort)
         self.unused = [".lib" + str(x) for x in (1, 3, 4)]
         self.assert_fix(
             [
                 "from . import (lib1, lib2, lib3,\n",
                 "               lib4, lib5, lib6)\n",
             ],
@@ -2937,15 +2952,15 @@
                 "    lib4,\n",
                 "    lib5\n",
                 ")\n",
             ],
             "from .parent import (\n" "    lib2,\n" "    lib5\n" ")\n",
         )
 
-    def test_fix_without_from(self):
+    def test_fix_without_from(self) -> None:
         self.unused = ["lib" + str(x) for x in (1, 3, 4)]
 
         # Multiline but not "from"
         self.assert_fix(
             [
                 "import \\\n",
                 "    lib1, lib2, lib3 \\\n",
@@ -2990,15 +3005,15 @@
                 "    lib4.x.y.z \\\n",
                 "    , \\\n",
                 "    lib5.x.y.z\n",
             ],
             "import \\\n" "    lib2.x.y.z \\" "    , \\\n" "    lib5.x.y.z\n",
         )
 
-    def test_give_up(self):
+    def test_give_up(self) -> None:
         # Semicolon
         self.unused = ["lib" + str(x) for x in (1, 3, 4)]
         self.assert_fix(
             [
                 "import \\\n",
                 "    lib1, lib2, lib3, \\\n",
                 "    lib4, lib5; import lib6\n",
@@ -3026,15 +3041,15 @@
             "    ,lib3, \n"
             "    libB, \n"
             "    \\  \n"
             "    lib4,  # noqa \n"
             ") ; import sys\n",
         )
 
-    def test_just_one_import_used(self):
+    def test_just_one_import_used(self) -> None:
         self.unused = ["lib2"]
         self.assert_fix(
             [
                 "import \\\n",
                 "    lib1\n",
             ],
             "import \\\n" "    lib1\n",
@@ -3051,15 +3066,15 @@
         self.assert_fix(
             [
                 "\tfrom re import (subn)\n",
             ],
             "\tpass\n",
         )
 
-    def test_just_one_import_left(self):
+    def test_just_one_import_left(self) -> None:
         # Examples from issue #8
         self.unused = ["math.sqrt"]
         self.assert_fix(
             [
                 "from math import (\n",
                 "        sqrt,\n",
                 "        log\n",
@@ -3085,15 +3100,15 @@
         self.assert_fix(
             [
                 "from re import (subn)\n",
             ],
             "from re import (subn)\n",
         )
 
-    def test_no_empty_imports(self):
+    def test_no_empty_imports(self) -> None:
         self.unused = ["lib" + str(x) for x in (1, 3, 4)]
         self.assert_fix(
             [
                 "import \\\n",
                 "    lib1, lib3, \\\n",
                 "    lib4 \n",
             ],
@@ -3109,15 +3124,15 @@
                 "    lib3,\n",
                 "    lib4,\n",
                 ")\n",
             ],
             "\t\tpass\n",
         )
 
-    def test_without_remove_all(self):
+    def test_without_remove_all(self) -> None:
         self.unused = ["lib" + str(x) for x in (1, 3, 4)]
         self.assert_fix(
             [
                 "import \\\n",
                 "    lib1,\\\n",
                 "    lib3,\\\n",
                 "    lib4\n",
@@ -3147,34 +3162,33 @@
             ],
             "import \\\n" "    lib1, \\\n" "    lib3\n",
             remove_all=False,
         )
 
 
 class ConfigFileTest(unittest.TestCase):
-    def setUp(self):
+    def setUp(self) -> None:
         self.tmpdir = tempfile.mkdtemp(prefix="autoflake.")
 
-    def tearDown(self):
-        if self.tmpdir is not None:
+    def tearDown(self) -> None:
+        if self.tmpdir:
             shutil.rmtree(self.tmpdir)
-        self.tmpdir = None
 
-    def effective_path(self, path, is_file=True):
+    def effective_path(self, path: str, is_file: bool = True) -> str:
         path = os.path.normpath(path)
         if os.path.isabs(path):
             raise ValueError("Should not create an absolute test path")
         effective_path = os.path.sep.join([self.tmpdir, path])
         if not effective_path.startswith(
             f"{self.tmpdir}{os.path.sep}",
         ) and (effective_path != self.tmpdir or is_file):
             raise ValueError("Should create a path within the tmp dir only")
         return effective_path
 
-    def create_dir(self, path):
+    def create_dir(self, path) -> None:
         effective_path = self.effective_path(path, False)
         if sys.version_info >= (3, 2, 0):
             os.makedirs(effective_path, exist_ok=True)
         else:
             if os.path.exists(effective_path):
                 return
             try:
@@ -3182,21 +3196,21 @@
             except OSError:
                 parent = os.path.split(path)[0]
                 if not parent:
                     raise
                 self.create_dir(parent)
                 os.mkdir(effective_path)
 
-    def create_file(self, path, contents=""):
+    def create_file(self, path, contents="") -> None:
         effective_path = self.effective_path(path)
         self.create_dir(os.path.split(path)[0])
         with open(effective_path, "w") as f:
             f.write(contents)
 
-    def with_defaults(self, **kwargs):
+    def with_defaults(self, **kwargs: Any) -> Mapping[str, Any]:
         return {
             "check": False,
             "check_diff": False,
             "expand_star_imports": False,
             "ignore_init_module_imports": False,
             "ignore_pass_after_docstring": False,
             "ignore_pass_statements": False,
@@ -3207,101 +3221,101 @@
             "remove_duplicate_keys": False,
             "remove_rhs_for_unused_variables": False,
             "remove_unused_variables": False,
             "write_to_stdout": False,
             **kwargs,
         }
 
-    def test_no_config_file(self):
+    def test_no_config_file(self) -> None:
         self.create_file("test_me.py")
         original_args = {
             "files": [self.effective_path("test_me.py")],
         }
         args, success = autoflake.merge_configuration_file(original_args)
         assert success is True
         assert args == self.with_defaults(**original_args)
 
-    def test_non_nested_pyproject_toml_empty(self):
+    def test_non_nested_pyproject_toml_empty(self) -> None:
         self.create_file("test_me.py")
         self.create_file("pyproject.toml", '[tool.other]\nprop="value"\n')
         files = [self.effective_path("test_me.py")]
         original_args = {"files": files}
         args, success = autoflake.merge_configuration_file(original_args)
         assert success is True
         assert args == self.with_defaults(**original_args)
 
-    def test_non_nested_pyproject_toml_non_empty(self):
+    def test_non_nested_pyproject_toml_non_empty(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             "[tool.autoflake]\nexpand-star-imports=true\n",
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             expand_star_imports=True,
         )
 
-    def test_non_nested_setup_cfg_non_empty(self):
+    def test_non_nested_setup_cfg_non_empty(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[other]\nexpand-star-imports = yes\n",
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(files=files)
 
-    def test_non_nested_setup_cfg_empty(self):
+    def test_non_nested_setup_cfg_empty(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[autoflake]\nexpand-star-imports = yes\n",
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             expand_star_imports=True,
         )
 
-    def test_nested_file(self):
+    def test_nested_file(self) -> None:
         self.create_file("nested/file/test_me.py")
         self.create_file(
             "pyproject.toml",
             "[tool.autoflake]\nexpand-star-imports=true\n",
         )
         files = [self.effective_path("nested/file/test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             expand_star_imports=True,
         )
 
-    def test_common_path_nested_file_do_not_load(self):
+    def test_common_path_nested_file_do_not_load(self) -> None:
         self.create_file("nested/file/test_me.py")
         self.create_file("nested/other/test_me.py")
         self.create_file(
             "nested/file/pyproject.toml",
             "[tool.autoflake]\nexpand-star-imports=true\n",
         )
         files = [
             self.effective_path("nested/file/test_me.py"),
             self.effective_path("nested/other/test_me.py"),
         ]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(files=files)
 
-    def test_common_path_nested_file_do_load(self):
+    def test_common_path_nested_file_do_load(self) -> None:
         self.create_file("nested/file/test_me.py")
         self.create_file("nested/other/test_me.py")
         self.create_file(
             "nested/pyproject.toml",
             "[tool.autoflake]\nexpand-star-imports=true\n",
         )
         files = [
@@ -3311,15 +3325,15 @@
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             expand_star_imports=True,
         )
 
-    def test_common_path_instead_of_common_prefix(self):
+    def test_common_path_instead_of_common_prefix(self) -> None:
         """Using common prefix would result in a failure."""
         self.create_file("nested/file-foo/test_me.py")
         self.create_file("nested/file-bar/test_me.py")
         self.create_file(
             "nested/file/pyproject.toml",
             "[tool.autoflake]\nexpand-star-imports=true\n",
         )
@@ -3327,15 +3341,15 @@
             self.effective_path("nested/file-foo/test_me.py"),
             self.effective_path("nested/file-bar/test_me.py"),
         ]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(files=files)
 
-    def test_continue_search_if_no_config_found(self):
+    def test_continue_search_if_no_config_found(self) -> None:
         self.create_file("nested/test_me.py")
         self.create_file(
             "nested/pyproject.toml",
             '[tool.other]\nprop = "value"\n',
         )
         self.create_file(
             "pyproject.toml",
@@ -3345,30 +3359,30 @@
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             expand_star_imports=True,
         )
 
-    def test_stop_search_if_config_found(self):
+    def test_stop_search_if_config_found(self) -> None:
         self.create_file("nested/test_me.py")
         self.create_file(
             "nested/pyproject.toml",
             "[tool.autoflake]\n",
         )
         self.create_file(
             "pyproject.toml",
             "[tool.autoflake]\nexpand-star-imports = true\n",
         )
         files = [self.effective_path("nested/test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(files=files)
 
-    def test_config_option(self):
+    def test_config_option(self) -> None:
         with temporary_file(
             suffix=".ini",
             contents=("[autoflake]\n" "check = True\n"),
         ) as temp_config:
             self.create_file("test_me.py")
             files = [self.effective_path("test_me.py")]
 
@@ -3381,102 +3395,102 @@
             assert success is True
             assert args == self.with_defaults(
                 files=files,
                 config_file=temp_config,
                 check=True,
             )
 
-    def test_load_false(self):
+    def test_load_false(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[autoflake]\nexpand-star-imports = no\n",
         )
         files = [self.effective_path("test_me.py")]
 
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             expand_star_imports=False,
         )
 
-    def test_list_value_pyproject_toml(self):
+    def test_list_value_pyproject_toml(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             '[tool.autoflake]\nimports=["my_lib", "other_lib"]\n',
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             imports="my_lib,other_lib",
         )
 
-    def test_list_value_comma_sep_string_pyproject_toml(self):
+    def test_list_value_comma_sep_string_pyproject_toml(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             '[tool.autoflake]\nimports="my_lib,other_lib"\n',
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             imports="my_lib,other_lib",
         )
 
-    def test_list_value_setup_cfg(self):
+    def test_list_value_setup_cfg(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[autoflake]\nimports=my_lib,other_lib\n",
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file({"files": files})
         assert success is True
         assert args == self.with_defaults(
             files=files,
             imports="my_lib,other_lib",
         )
 
-    def test_non_bool_value_for_bool_property(self):
+    def test_non_bool_value_for_bool_property(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             '[tool.autoflake]\nexpand-star-imports="invalid"\n',
         )
         files = [self.effective_path("test_me.py")]
         _, success = autoflake.merge_configuration_file({"files": files})
         assert success is False
 
-    def test_non_bool_value_for_bool_property_in_setup_cfg(self):
+    def test_non_bool_value_for_bool_property_in_setup_cfg(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "setup.cfg",
             "[autoflake]\nexpand-star-imports=ok\n",
         )
         files = [self.effective_path("test_me.py")]
         _, success = autoflake.merge_configuration_file({"files": files})
         assert success is False
 
-    def test_non_list_value_for_list_property(self):
+    def test_non_list_value_for_list_property(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             "[tool.autoflake]\nexclude=true\n",
         )
         files = [self.effective_path("test_me.py")]
         _, success = autoflake.merge_configuration_file({"files": files})
         assert success is False
 
-    def test_merge_with_cli_set_list_property(self):
+    def test_merge_with_cli_set_list_property(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             '[tool.autoflake]\nimports=["my_lib"]\n',
         )
         files = [self.effective_path("test_me.py")]
         args, success = autoflake.merge_configuration_file(
@@ -3484,15 +3498,15 @@
         )
         assert success is True
         assert args == self.with_defaults(
             files=files,
             imports="my_lib,other_lib",
         )
 
-    def test_merge_prioritizes_flags(self):
+    def test_merge_prioritizes_flags(self) -> None:
         self.create_file("test_me.py")
         self.create_file(
             "pyproject.toml",
             "[tool.autoflake]\ncheck = false\n",
         )
         files = [self.effective_path("test_me.py")]
         flag_args = {
@@ -3506,15 +3520,20 @@
             files=files,
             imports="other_lib",
             check=True,
         )
 
 
 @contextlib.contextmanager
-def temporary_file(contents, directory=".", suffix=".py", prefix=""):
+def temporary_file(
+    contents: str,
+    directory: str = ".",
+    suffix: str = ".py",
+    prefix: str = "",
+) -> Iterator[str]:
     """Write contents to temporary file and yield it."""
     f = tempfile.NamedTemporaryFile(
         suffix=suffix,
         prefix=prefix,
         delete=False,
         dir=directory,
     )
@@ -3523,26 +3542,26 @@
         f.close()
         yield f.name
     finally:
         os.remove(f.name)
 
 
 @contextlib.contextmanager
-def temporary_directory(directory=".", prefix="tmp."):
+def temporary_directory(directory: str = ".", prefix: str = "tmp.") -> Iterator[str]:
     """Create temporary directory and yield its path."""
     temp_directory = tempfile.mkdtemp(prefix=prefix, dir=directory)
     try:
         yield temp_directory
     finally:
         shutil.rmtree(temp_directory)
 
 
 class StubFile:
 
     """Fake file that ignores everything."""
 
-    def write(*_):
+    def write(*_: Any) -> None:
         """Ignore."""
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `autoflake-2.1.1/AUTHORS.rst` & `autoflake-2.2.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `autoflake-2.1.1/LICENSE` & `autoflake-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autoflake-2.1.1/README.md` & `autoflake-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -197,11 +197,11 @@
 
 ## Using [pre-commit](https://pre-commit.com) hooks
 
 Add the following to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
     -   id: autoflake
 ```
```

### Comparing `autoflake-2.1.1/pyproject.toml` & `autoflake-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Quality Assurance",
 ]
 keywords = ["clean", "fix", "automatic", "unused", "import"]
 urls = { Homepage = "https://www.github.com/PyCQA/autoflake" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = ["pyflakes>=3.0.0", "tomli>=2.0.1;python_version<'3.11'"]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
@@ -30,9 +30,15 @@
 [tool.hatch.version]
 path = "autoflake.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/.github"]
 
 [tool.hatch.build]
-include = ["/autoflake.py", "/test_autoflake.py", "/LICENSE", "/README.md"]
+include = [
+  "/autoflake.py",
+  "/test_autoflake.py",
+  "/py.typed",
+  "/LICENSE",
+  "/README.md",
+]
 exclude = ["/.gitignore"]
```

### Comparing `autoflake-2.1.1/PKG-INFO` & `autoflake-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: autoflake
-Version: 2.1.1
+Version: 2.2.0
 Summary: Removes unused imports and unused variables
 Project-URL: Homepage, https://www.github.com/PyCQA/autoflake
 License: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: automatic,clean,fix,import,unused
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: pyflakes>=3.0.0
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # autoflake
 
 [![Build Status](https://github.com/PyCQA/autoflake/actions/workflows/main.yaml/badge.svg?branch=main)](https://github.com/PyCQA/autoflake/actions/workflows/main.yaml)
@@ -217,11 +217,11 @@
 
 ## Using [pre-commit](https://pre-commit.com) hooks
 
 Add the following to your `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/PyCQA/autoflake
-    rev: v2.1.1
+    rev: v2.2.0
     hooks:
     -   id: autoflake
 ```
```

