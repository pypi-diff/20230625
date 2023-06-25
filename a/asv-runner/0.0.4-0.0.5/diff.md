# Comparing `tmp/asv_runner-0.0.4.tar.gz` & `tmp/asv_runner-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asv_runner-0.0.4.tar", last modified: Sun Jun 11 15:20:24 2023, max compression
+gzip compressed data, was "asv_runner-0.0.5.tar", last modified: Sun Jun 25 19:16:14 2023, max compression
```

## Comparing `asv_runner-0.0.4.tar` & `asv_runner-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      286 2023-06-11 15:20:15.306004 asv_runner-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/_aux.py
--rw-r--r--   0        0        0      585 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/__init__.py
--rw-r--r--   0        0        0    10646 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/_base.py
--rw-r--r--   0        0        0      183 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/_exceptions.py
--rw-r--r--   0        0        0     3404 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/_maxrss.py
--rw-r--r--   0        0        0      817 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/mem.py
--rw-r--r--   0        0        0      587 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/peakmem.py
--rw-r--r--   0        0        0     5400 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/time.py
--rw-r--r--   0        0        0     1759 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/timeraw.py
--rw-r--r--   0        0        0      581 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/benchmarks/track.py
--rw-r--r--   0        0        0      318 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/check.py
--rw-r--r--   0        0        0    11444 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/console.py
--rw-r--r--   0        0        0     5866 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/discovery.py
--rw-r--r--   0        0        0     1118 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/run.py
--rw-r--r--   0        0        0     5210 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/server.py
--rw-r--r--   0        0        0      474 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/setup_cache.py
--rw-r--r--   0        0        0     9809 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/statistics.py
--rw-r--r--   0        0        0     1941 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/timing.py
--rw-r--r--   0        0        0     3467 2023-06-11 15:20:15.306004 asv_runner-0.0.4/asv_runner/util.py
--rw-r--r--   0        0        0      838 2023-06-11 15:20:24.173978 asv_runner-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 asv_runner-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-06-25 19:16:04.758892 asv_runner-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/__init__.py
+-rw-r--r--   0        0        0     6718 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/_aux.py
+-rw-r--r--   0        0        0     1825 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/benchmarks/__init__.py
+-rw-r--r--   0        0        0    22059 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/benchmarks/_base.py
+-rw-r--r--   0        0        0     1095 2023-06-25 19:16:04.758892 asv_runner-0.0.5/asv_runner/benchmarks/_exceptions.py
+-rw-r--r--   0        0        0     5683 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/_maxrss.py
+-rw-r--r--   0        0        0     2248 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/mem.py
+-rw-r--r--   0        0        0     1965 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/peakmem.py
+-rw-r--r--   0        0        0     9895 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/time.py
+-rw-r--r--   0        0        0     5071 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/timeraw.py
+-rw-r--r--   0        0        0     1912 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/benchmarks/track.py
+-rw-r--r--   0        0        0      915 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/check.py
+-rw-r--r--   0        0        0    14462 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/console.py
+-rw-r--r--   0        0        0    10852 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/discovery.py
+-rw-r--r--   0        0        0     2456 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/run.py
+-rw-r--r--   0        0        0     7956 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/server.py
+-rw-r--r--   0        0        0     1450 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/setup_cache.py
+-rw-r--r--   0        0        0    18701 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/statistics.py
+-rw-r--r--   0        0        0     2744 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/timing.py
+-rw-r--r--   0        0        0     4549 2023-06-25 19:16:04.762892 asv_runner-0.0.5/asv_runner/util.py
+-rw-r--r--   0        0        0     1468 2023-06-25 19:16:14.542956 asv_runner-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 asv_runner-0.0.5/PKG-INFO
```

### Comparing `asv_runner-0.0.4/asv_runner/console.py` & `asv_runner-0.0.5/asv_runner/console.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,44 +15,55 @@
 from asv_runner import util
 
 WIN = os.name == "nt"
 
 
 def isatty(file):
     """
-    Returns `True` if `file` is a tty.
+    Determines if a file is a tty.
 
+    #### Parameters
+    **file** (`file-like object`)
+    : The file-like object to check.
+
+    #### Returns
+    **isatty** (`bool`)
+    : Returns `True` if the file is a tty, `False` otherwise.
+
+    #### Notes
     Most built-in Python file-like objects have an `isatty` member,
-    but some user-defined types may not, so this assumes those are not
-    ttys.
+    but some user-defined types may not. In such cases, this function
+    assumes those are not ttys.
     """
     if hasattr(file, "isatty"):
         return file.isatty()
     return False
 
 
 def _color_text(text, color):
     """
-    Returns a string wrapped in ANSI color codes for coloring the
-    text in a terminal::
-
-        colored_text = color_text('Here is a message', 'blue')
-
-    This won't actually effect the text until it is printed to the
-    terminal.
+    Returns a string wrapped in ANSI color codes for coloring the text in a terminal.
 
-    Parameters
-    ----------
-    text : str
-        The string to return, bounded by the color codes.
-    color : str
-        An ANSI terminal color name. Must be one of:
-        black, red, green, brown, blue, magenta, cyan, lightgrey,
-        default, darkgrey, lightred, lightgreen, yellow, lightblue,
-        lightmagenta, lightcyan, white, or '' (the empty string).
+    #### Parameters
+    **text** (`str`)
+    : The string to colorize.
+
+    **color** (`str`)
+    : An ANSI terminal color name. Must be one of the following:
+      'black', 'red', 'green', 'brown', 'blue', 'magenta', 'cyan', 'lightgrey',
+      'default', 'darkgrey', 'lightred', 'lightgreen', 'yellow', 'lightblue',
+      'lightmagenta', 'lightcyan', 'white', or '' (the empty string).
+
+    #### Returns
+    **colored_text** (`str`)
+    : The input string, bounded by the appropriate ANSI color codes.
+
+    #### Notes
+    This function wraps the input text with ANSI color codes based on the given color.
+    It won't actually affect the text until it is printed to the terminal.
     """
     color_mapping = {
         "black": "0;30",
         "red": "0;31",
         "green": "0;32",
         "brown": "0;33",
         "blue": "0;34",
@@ -70,34 +81,58 @@
         "white": "1;37",
     }
 
     color_code = color_mapping.get(color, "0;39")
     return f"\033[{color_code}m{text}\033[0m"
 
 
-# This is a table of Unicode characters that we want to have
-# reasonable representations in ascii so they aren't just replaced
-# with '?'.  A complete solution to this problem would involve a
-# third-party library such as "unidecode", but this handles the common
-# cases of stuff coming from asv.
+# A dictionary of Unicode characters that have reasonable representations in ASCII.
+# This dictionary contains Unicode characters as keys and their corresponding ASCII
+# representations as values. This allows for convenient replacement of these specific
+# Unicode characters with ASCII ones to prevent them from being replaced by '?'.
 #
-# You can find the characters that need an entry using:
-#    grep -P  -n '[^\x00-\x7F]' -r *
+# The mapping currently includes:
+# - 'μ' maps to 'u'
+# - '·' maps to '-'
+# - '±' maps to '~'
+#
+# You can find additional characters that might need an entry using:
+# `grep -P  -n '[^\x00-\x7F]' -r *`
 # in the `asv` source directory.
-
 _unicode_translations = {ord("μ"): "u", ord("·"): "-", ord("±"): "~"}
 
 
 def _write_with_fallback(s, fileobj):
     """
-    Write the supplied string to the given stream, but switch to
-    the locale's preferred encoding in case of a UnicodeEncodeError.
-    Failing that, replace characters.
-    *fileobj* must be text stream on Py3, on Py2 a `file` byte stream.
-    *s* must be unicode.
+    Writes the supplied string to the given file-like object, handling potential
+    UnicodeEncodeErrors by falling back to the locale's preferred encoding.
+
+    #### Parameters
+    `s` (`str`):
+    The Unicode string to be written to the file-like object. Raises a `ValueError`
+    if `s` is not a Unicode string.
+
+    `fileobj` (file-like object):
+    The file-like object to which the string `s` is to be written. On Python 3,
+    this must be a text stream. On Python 2, this must be a `file` byte stream.
+
+    #### Notes
+    This function first tries to write the input string `s` to the file object
+    `fileobj`. If a `UnicodeError` occurs during this process (indicating that the
+    string contains characters not representable in the file's encoding), the function
+    falls back to encoding the string in the locale's preferred encoding before writing.
+
+    If the string `s` still cannot be encoded in the locale's preferred encoding, the
+    function translates the string to replace problematic Unicode characters with
+    ASCII ones using the `_unicode_translations` dictionary, and then encodes and
+    writes the resulting string to `fileobj` using the "replace" error handling scheme
+    (which replaces any non-encodable characters with a suitable replacement marker).
+
+    After the write operation, the function flushes the file object's output buffer to
+    ensure that the written data is actually saved to the file.
     """
     if not isinstance(s, str):
         raise ValueError("Input string is not a Unicode string")
 
     try:
         fileobj.write(s)
         return
@@ -114,43 +149,47 @@
 
     fileobj.flush()
     fileobj.buffer.write(b)
 
 
 def color_print(*args, **kwargs):
     """
-    Prints colors and styles to the terminal uses ANSI escape
-    sequences.
-
-    ::
+    Prints colored and styled text to the terminal using ANSI escape sequences.
 
-       color_print('This is the color ', 'default', 'GREEN', 'green')
-
-    Parameters
-    ----------
-    positional args : str
-        The positional arguments come in pairs (*msg*, *color*), where
-        *msg* is the string to display and *color* is the color to
-        display it in.
-
-        *color* is an ANSI terminal color name.  Must be one of:
-        black, red, green, brown, blue, magenta, cyan, lightgrey,
-        default, darkgrey, lightred, lightgreen, yellow, lightblue,
-        lightmagenta, lightcyan, white, or '' (the empty string).
-
-    file : writeable file-like object, optional
-        Where to write to.  Defaults to `sys.stdout`.  If file is not
-        a tty (as determined by calling its `isatty` member, if one
-        exists), no coloring will be included.
-
-    end : str, optional
-        The ending of the message.  Defaults to ``\\n``.  The end will
-        be printed after resetting any color or font state.
+    #### Parameters
+    *args (`tuple` of `str`):
+    The positional arguments should come in pairs (`msg`, `color`), where `msg`
+    is the string to display and `color` is the color to display it in. `color`
+    is an ANSI terminal color name. Must be one of: black, red, green, brown,
+    blue, magenta, cyan, lightgrey, default, darkgrey, lightred, lightgreen,
+    yellow, lightblue, lightmagenta, lightcyan, white, or '' (the empty string).
+
+    `file` (writable file-like object, optional):
+    Where to write to. Defaults to `sys.stdout`. If `file` is not a tty (as determined
+    by calling its `isatty` member, if one exists), no coloring will be included. It's
+    passed as a keyword argument.
+
+    `end` (`str`, optional):
+    The ending of the message. Defaults to "\n". The `end` will be printed after
+    resetting any color or font state. It's passed as a keyword argument.
+
+    #### Notes
+    This function allows you to print text in various colors to the console, which can
+    be helpful for distinguishing different kinds of output or for drawing attention to
+    particular messages.
+
+    It works by applying ANSI escape sequences to the input strings according to the
+    specified colors. These escape sequences are interpreted by the terminal emulator
+    to apply the specified colors and styles.
+
+    #### Example
+    ```{code-block} python
+    color_print('This is the color ', 'default', 'GREEN', 'green')
+    ```
     """
-
     file = kwargs.get("file", sys.stdout)
     end = kwargs.get("end", "\n")
 
     if isatty(file) and not WIN:
         for i in range(0, len(args), 2):
             msg = args[i]
             if i + 1 == len(args):
@@ -167,14 +206,36 @@
         for i in range(0, len(args), 2):
             msg = args[i]
             _write_with_fallback(msg, file)
         _write_with_fallback(end, file)
 
 
 def get_answer_default(prompt, default, use_defaults=False):
+    """
+    Prompts the user for input and returns the entered value or a default.
+
+    #### Parameters
+    `prompt` (`str`):
+    The string that is presented to the user.
+
+    `default` (any):
+    The value returned if the user doesn't enter anything and just hits Enter. This
+    value is also shown in the prompt to indicate to the user what the default is.
+
+    `use_defaults` (`bool`, optional):
+    If True, the function will immediately return the default value without prompting
+    the user for input. Defaults to False.
+
+    #### Returns
+    The user's input, or the provided default value if the user didn't enter anything.
+
+    #### Notes
+    This function enhances the built-in `input` function by allowing a default value
+    to be specified, which is returned if the user doesn't enter anything.
+    """
     color_print(f"{prompt} [{default}]: ", end="")
 
     if use_defaults:
         return default
 
     x = input()
     if x.strip() == "":
```

### Comparing `asv_runner-0.0.4/asv_runner/timing.py` & `asv_runner-0.0.5/asv_runner/timing.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,33 @@
 import timeit
 from time import process_time
 
 from .benchmarks.time import TimeBenchmark
 
 
 def _timing(argv):
+    """
+    Executes a timing benchmark.
+
+    #### Parameters
+    **argv** (`list` of `str`)
+    : Command line arguments.
+
+    #### Notes
+    This function parses the command line arguments, including options for setup,
+    number of repeats, timing method, and output format (JSON or not). It selects
+    the appropriate timing function based on the `--timer` argument.
+
+    It creates an instance of the `TimeBenchmark` class, with the provided statement
+    to be executed, and runs it. The setup is provided from the `--setup` argument.
+
+    Once the benchmark is run, it computes the statistics of the results and formats
+    the output. If the `--json` flag is not set, it prints the output in a human-
+    readable format. Otherwise, it outputs the result, samples, and stats as a JSON.
+    """
     import argparse
 
     import asv_runner.console
     import asv_runner.statistics
     import asv_runner.util
 
     parser = argparse.ArgumentParser(
```

### Comparing `asv_runner-0.0.4/asv_runner/util.py` & `asv_runner-0.0.5/asv_runner/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,25 +7,59 @@
 import math
 import shutil
 
 terminal_width = shutil.get_terminal_size().columns
 
 
 def ceildiv(numerator, denominator):
-    """Ceiling division"""
+    """
+    Calculate the ceiling division of two numbers.
+
+    #### Parameters
+    **numerator** (`int`)
+    : The numerator in the division.
+
+    **denominator** (`int`)
+    : The denominator in the division.
+
+    #### Returns
+    `int`: The result of the division rounded up to the nearest integer.
+
+    #### Notes
+    This function calculates the ceiling division of two numbers, i.e.,
+    division that rounds up. It is equivalent to `math.ceil(numerator/denominator)`,
+    but avoids the conversion of numerator and denominator to float.
+    """
     return -((-numerator) // denominator)
 
 
 def human_float(value, significant=3, truncate_small=None, significant_zeros=False):
     """
-    Return a string representing a float with human friendly significant digits.
-    Switches to scientific notation for too large/small numbers.
-    If `truncate_small`, then leading zeros of numbers < 1 are counted as
-    significant. If not `significant_zeros`, trailing unnecessary zeros are
-    stripped.
+    Formats a float into a human-friendly string.
+
+    #### Parameters
+    **value** (`float`)
+    : The float value to format.
+
+    **significant** (`int`)
+    : Number of significant digits to include in the output. Default is 3.
+
+    **truncate_small** (`int`, optional)
+    : If defined, leading zeros of numbers < 1 are counted as significant.
+
+    **significant_zeros** (`bool`)
+    : If True, trailing unnecessary zeros are included. Default is False.
+
+    #### Returns
+    `str`: A string representing the float with human-friendly significant
+    digits.
+
+    #### Notes
+    Switches to scientific notation for very large or very small numbers.
+    The magnitude of the number is calculated using `math.log10(value)`.
     """
     if value == 0:
         return "0"
     elif math.isinf(value) or math.isnan(value):
         return f"{value}"
     elif value < 0:
         sign = "-"
@@ -79,37 +113,37 @@
     ("y", 60 * 60 * 24 * 7 * 52),
     ("C", 60 * 60 * 24 * 7 * 52 * 100),
 )
 
 
 def human_time(seconds, err=None):
     """
-    Returns a human-friendly time string that is always exactly 6
-    characters long.
+    Formats a duration in seconds into a human-friendly time string.
 
     Depending on the number of seconds given, can be one of::
 
         1w 3d
         2d 4h
         1h 5m
         1m 4s
           15s
 
-    Will be in color if console coloring is turned on.
+    The representation is always exactly 6 characters long.
 
-    Parameters
-    ----------
-    seconds : int
-        The number of seconds to represent
-
-    Returns
-    -------
-    time : str
-        A human-friendly representation of the given number of seconds
-        that is always exactly 6 characters.
+    #### Parameters
+    **seconds** (`int`)
+    : The number of seconds to represent.
+
+    **err** (`float`, optional)
+    : If provided, formats the duration as "{value}±{err}", e.g., "1h±5m".
+      It can be used to represent the uncertainty in the measurement.
+
+    #### Returns
+    `str`: A human-friendly representation of the given duration. If the
+           duration is NaN, returns "n/a".
     """
     units = _human_time_units
     seconds = float(seconds)
 
     scale = seconds
 
     if scale == 0 and err is not None:
```

### Comparing `asv_runner-0.0.4/PKG-INFO` & `asv_runner-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: asv-runner
-Version: 0.0.4
+Version: 0.0.5
 Summary: Core Python benchmark code for ASV
 Author-Email: Rohit Goswami <rog32@hi.is>
 Maintainer-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
-Requires-Python: >=3.7
-Provides-Extra: lint
-Requires-Dist: ruff>=0.0.265; extra == "lint"
-Requires-Dist: black>=23.3.0; extra == "lint"
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: System :: Benchmark
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # About
 
 Core Python benchmark code for `asv`.
 
 **This package shall not have any dependencies on external packages and must be
-compatible with all Python versions greater than or equal to `3.7`.**
+compatible with all Python versions greater than or equal to `3.8`.**
 
 
 For other functionality, refer to the `asv` package or consider writing an extension.
```

