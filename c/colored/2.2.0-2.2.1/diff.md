# Comparing `tmp/colored-2.2.0.tar.gz` & `tmp/colored-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colored-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "colored-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `colored-2.2.0.tar` & `colored-2.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2349 2023-06-24 14:33:49.000000 colored-2.2.0/README.md
--rw-r--r--   0        0        0      374 2023-06-24 14:33:49.000000 colored-2.2.0/colored/__init__.py
--rw-r--r--   0        0        0     2085 2023-06-24 14:33:49.000000 colored-2.2.0/colored/attributes.py
--rw-r--r--   0        0        0     2137 2023-06-24 14:33:49.000000 colored-2.2.0/colored/background.py
--rw-r--r--   0        0        0    10859 2023-06-24 14:33:49.000000 colored-2.2.0/colored/colored.py
--rw-r--r--   0        0        0     1984 2023-06-24 14:33:49.000000 colored-2.2.0/colored/controls.py
--rw-r--r--   0        0        0     1574 2023-06-24 14:33:49.000000 colored-2.2.0/colored/cprint.py
--rw-r--r--   0        0        0     1089 2023-06-24 14:33:49.000000 colored-2.2.0/colored/exceptions.py
--rw-r--r--   0        0        0     2105 2023-06-24 14:33:49.000000 colored-2.2.0/colored/foreground.py
--rw-r--r--   0        0        0     1854 2023-06-24 14:33:49.000000 colored-2.2.0/colored/hexadecimal.py
--rw-r--r--   0        0        0    15604 2023-06-24 14:33:49.000000 colored-2.2.0/colored/library.py
--rw-r--r--   0        0        0     2628 2023-06-24 14:33:49.000000 colored-2.2.0/colored/utilities.py
--rw-r--r--   0        0        0      991 2023-06-24 14:33:49.000000 colored-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 colored-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3007 2023-06-25 19:28:05.000000 colored-2.2.1/README.md
+-rw-r--r--   0        0        0      374 2023-06-25 19:28:05.000000 colored-2.2.1/colored/__init__.py
+-rw-r--r--   0        0        0     2085 2023-06-25 19:28:05.000000 colored-2.2.1/colored/attributes.py
+-rw-r--r--   0        0        0     2137 2023-06-25 19:28:05.000000 colored-2.2.1/colored/background.py
+-rw-r--r--   0        0        0    10859 2023-06-25 19:28:05.000000 colored-2.2.1/colored/colored.py
+-rw-r--r--   0        0        0     1966 2023-06-25 19:28:05.000000 colored-2.2.1/colored/controls.py
+-rw-r--r--   0        0        0     1574 2023-06-25 19:28:05.000000 colored-2.2.1/colored/cprint.py
+-rw-r--r--   0        0        0     1086 2023-06-25 19:28:05.000000 colored-2.2.1/colored/exceptions.py
+-rw-r--r--   0        0        0     2105 2023-06-25 19:28:05.000000 colored-2.2.1/colored/foreground.py
+-rw-r--r--   0        0        0     1854 2023-06-25 19:28:05.000000 colored-2.2.1/colored/hexadecimal.py
+-rw-r--r--   0        0        0    15604 2023-06-25 19:28:05.000000 colored-2.2.1/colored/library.py
+-rw-r--r--   0        0        0     2628 2023-06-25 19:28:05.000000 colored-2.2.1/colored/utilities.py
+-rw-r--r--   0        0        0     1067 2023-06-25 19:28:05.000000 colored-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 colored-2.2.1/PKG-INFO
```

### Comparing `colored-2.2.0/README.md` & `colored-2.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 <a href="https://dslackw.gitlab.io/colored"> 
 <img src="https://gitlab.com/dslackw/colored/-/raw/site/docs/images/colored.png" title="colored"></a>
 
 ## About
 
 Colored, it's a simple Python library for color and formatting in terminal.
-Collection of color codes and names for 256 color terminal setups.
+Collection of color codes and names for 256 color terminal setups. 
+Colored now supports RGB color mode. As "true color" graphic cards with 16 to <a href="https://en.wikipedia.org/wiki/ANSI_escape_code#24-bit" target="_blank">24 bits</a> of color became common, 
+applications began to support 24-bit colors. Terminal emulators supporting setting 24-bit foreground and background 
+colors with escape sequences include Xterm, KDE's <a href="https://en.wikipedia.org/wiki/Konsole" target="_blank">Konsole</a>, and iTerm, as well as all libvte based terminals,
+including <a href="https://en.wikipedia.org/wiki/GNOME_Terminal" target="_blank">GNOME Terminal</a>.
 
-A list of [256 colors](https://dslackw.gitlab.io/colored/formatting/colors/#full-chart-256-foreground-and-background-colors)
+A list of [256 colors](https://dslackw.gitlab.io/colored/tables/colors/#full-chart-256-foreground-and-background-colors)
 for <a href="https://en.wikipedia.org/wiki/Xterm" target="_blank">Xterm</a>, containing an example of the displayed color, Xterm Name, Xterm Number and HEX.
 
 The colors work with most terminals and terminals emulators.
 <a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">ANSI/VT100 escape sequences</a> can be used in every programming languages.
 
 Colored is powerful and easy to use:
 
@@ -22,19 +26,23 @@
 >>>
 >>> Back.red
 '\x1b[48;5;1m'
 >>>
 >>> Style.reset
 '\x1b[0m'
 >>> 
+>>> Fore.rgb('100%', '50%', '30%')
+'\x1b[38;2;255;130;79m'
+>>>
 >>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}')
 ```
-<p> >>> <span style="background-color: green">
-  <span style="color: white">Colored is Awesome!!!</span></span>
-</p>
+!!! success
+    <p> >>> <span style="background-color: green">
+      <span style="color: white">Colored is Awesome!!!</span></span>
+    </p>
 
 ## Installing
 
 Open up a terminal and install colored with <a href="https://pip.pypa.io/en/stable/" target="_blank">pip</a> command:
 
 ```bash
 $ pip install colored
@@ -55,17 +63,15 @@
 
 ## License
 
 colored is made available under the MIT License. For more details, see [here](https://dslackw.gitlab.io/colored/license/#mit-license).
 
 ## Contributing
 
-
-We happily welcome [contributions](https://dslackw.gitlab.io/colored/contributors/)!
+!!! info
+    We happily welcome [contributions](https://dslackw.gitlab.io/colored/contributors/)!
 
 ## Donate
 
 Did you know that we developers love coffee? 
 
-Donate me a coffee ☕ ⬇
-
 [<img src="https://gitlab.com/dslackw/colored/-/raw/site/docs/images/paypaldonate.png" alt="paypal" title="donate">](https://www.paypal.me/dslackw)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,25 +1,31 @@
 [https://gitlab.com/dslackw/colored/-/raw/site/docs/images/colored.png] ##
 About Colored, it's a simple Python library for color and formatting in
-terminal. Collection of color codes and names for 256 color terminal setups. A
-list of [256 colors](https://dslackw.gitlab.io/colored/formatting/colors/#full-
-chart-256-foreground-and-background-colors) for Xterm, containing an example of
-the displayed color, Xterm Name, Xterm Number and HEX. The colors work with
-most terminals and terminals emulators. ANSI/VT100_escape_sequences can be used
-in every programming languages. Colored is powerful and easy to use: ```python
+terminal. Collection of color codes and names for 256 color terminal setups.
+Colored now supports RGB color mode. As "true color" graphic cards with 16 to
+24_bits of color became common, applications began to support 24-bit colors.
+Terminal emulators supporting setting 24-bit foreground and background colors
+with escape sequences include Xterm, KDE's Konsole, and iTerm, as well as all
+libvte based terminals, including GNOME_Terminal. A list of [256 colors](https:
+//dslackw.gitlab.io/colored/tables/colors/#full-chart-256-foreground-and-
+background-colors) for Xterm, containing an example of the displayed color,
+Xterm Name, Xterm Number and HEX. The colors work with most terminals and
+terminals emulators. ANSI/VT100_escape_sequences can be used in every
+programming languages. Colored is powerful and easy to use: ```python
 title="Python 3.9.17" >>> from colored import Fore, Back, Style >>> >>>
 Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>> >>> Style.reset
-'\x1b[0m' >>> >>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!
-{Style.reset}') ```
+'\x1b[0m' >>> >>> Fore.rgb('100%', '50%', '30%') '\x1b[38;2;255;130;79m' >>>
+>>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}') ```
+!!! success
 >>>  Colored is Awesome!!!
 ## Installing Open up a terminal and install colored with pip command: ```bash
 $ pip install colored ``` Alternatively, you can grab the latest source code
 from GitLab: ```bash $ git clone https://gitlab.com/dslackw/colored.git $ cd
 colored $ pip install . ``` ## Usage The [User Guide](https://
 dslackw.gitlab.io/colored/user_guide/user_guide/#user-guide) is the place to go
 to learn how to use the library. The [API Reference](https://dslackw.gitlab.io/
 colored/api/attributes/) documentation provides API-level documentation. ##
 License colored is made available under the MIT License. For more details, see
 [here](https://dslackw.gitlab.io/colored/license/#mit-license). ## Contributing
-We happily welcome [contributions](https://dslackw.gitlab.io/colored/
-contributors/)! ## Donate Did you know that we developers love coffee? Donate
-me a coffee â â¬ [[paypal]](https://www.paypal.me/dslackw)
+!!! info We happily welcome [contributions](https://dslackw.gitlab.io/colored/
+contributors/)! ## Donate Did you know that we developers love coffee? [
+[paypal]](https://www.paypal.me/dslackw)
```

### Comparing `colored-2.2.0/colored/attributes.py` & `colored-2.2.1/colored/attributes.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/background.py` & `colored-2.2.1/colored/background.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/colored.py` & `colored-2.2.1/colored/colored.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/controls.py` & `colored-2.2.1/colored/controls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from .library import Library
-from .exceptions import InvalidNavigation
+from .exceptions import InvalidControl
 
 
 class Controls:
 
     def __init__(self):
         self._ESC: str = Library.ESC
         self._CONTROLS: dict = Library.CONTROLS
@@ -32,28 +32,28 @@
             ESC[ row; col; H: Cursor Position
             ESC[ row J: Erase in Display
             ESC[ row K: Erase in Line
             ESC[ row S: Scroll Up
             ESC[ row T: Scroll Down
 
         Raises:
-            InvalidNavigation: Raises an Exception.
+            InvalidControl: Raises an Exception.
         """
         self._is_str_object(name)
         self._is_n_exist(name)
 
         if column:
             if name.lower() == 'position':
                 return f'{self._ESC}{row};{column}{self._CONTROLS[name.lower()]}'
             else:
-                raise InvalidNavigation(f"{InvalidNavigation.__name__}: {name}: Expected 'position'")
+                raise InvalidControl(f"{InvalidControl.__name__}: {name}: Expected 'position'")
 
         return f'{self._ESC}{row}{self._CONTROLS[name.lower()]}'
 
     @staticmethod
     def _is_str_object(move: str) -> None:
         if not isinstance(move, str):
             raise AttributeError("'str' object required")
 
     def _is_n_exist(self, move: str) -> None:
         if move.lower() not in self._CONTROLS.keys():
-            raise InvalidNavigation(f'{InvalidNavigation.__name__}: {move}')
+            raise InvalidControl(f'{InvalidControl.__name__}: {move}')
```

### Comparing `colored-2.2.0/colored/cprint.py` & `colored-2.2.1/colored/cprint.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/exceptions.py` & `colored-2.2.1/colored/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         super(Exception, self).__init__(message)
         self.message: str = message
 
     def __str__(self):
         return self.message
 
 
-class InvalidNavigation(Exception):
+class InvalidControl(Exception):
     """ Custom Exception for invalid navigation. """
     def __init__(self, message: str):
         super(Exception, self).__init__(message)
         self.message: str = message
 
     def __str__(self):
         return self.message
```

### Comparing `colored-2.2.0/colored/foreground.py` & `colored-2.2.1/colored/foreground.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/hexadecimal.py` & `colored-2.2.1/colored/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/library.py` & `colored-2.2.1/colored/library.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/colored/utilities.py` & `colored-2.2.1/colored/utilities.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.0/pyproject.toml` & `colored-2.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "colored"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Simple python library for color and formatting to terminal"
 readme = "README.md"
 requires-python = ">=3.9"
-keywords = ['xterm', 'color', 'vt100', 'ansi', 'terminal', 'python']
+keywords = [
+    'xterm',
+    'color',
+    'colour',
+    'vt100',
+    'ansi',
+    'terminal',
+    'text',
+    'rgb',
+    'linux',
+    'windows']
 license = {text = "MIT License"}
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'License :: OSI Approved :: MIT License',
     'Operating System :: POSIX :: Other',
     'Operating System :: POSIX :: Linux',
```

### Comparing `colored-2.2.0/PKG-INFO` & `colored-2.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: colored
-Version: 2.2.0
+Version: 2.2.1
 Summary: Simple python library for color and formatting to terminal
-Keywords: xterm,color,vt100,ansi,terminal,python
+Keywords: xterm,color,colour,vt100,ansi,terminal,text,rgb,linux,windows
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Other
@@ -20,17 +20,21 @@
 
 <a href="https://dslackw.gitlab.io/colored"> 
 <img src="https://gitlab.com/dslackw/colored/-/raw/site/docs/images/colored.png" title="colored"></a>
 
 ## About
 
 Colored, it's a simple Python library for color and formatting in terminal.
-Collection of color codes and names for 256 color terminal setups.
+Collection of color codes and names for 256 color terminal setups. 
+Colored now supports RGB color mode. As "true color" graphic cards with 16 to <a href="https://en.wikipedia.org/wiki/ANSI_escape_code#24-bit" target="_blank">24 bits</a> of color became common, 
+applications began to support 24-bit colors. Terminal emulators supporting setting 24-bit foreground and background 
+colors with escape sequences include Xterm, KDE's <a href="https://en.wikipedia.org/wiki/Konsole" target="_blank">Konsole</a>, and iTerm, as well as all libvte based terminals,
+including <a href="https://en.wikipedia.org/wiki/GNOME_Terminal" target="_blank">GNOME Terminal</a>.
 
-A list of [256 colors](https://dslackw.gitlab.io/colored/formatting/colors/#full-chart-256-foreground-and-background-colors)
+A list of [256 colors](https://dslackw.gitlab.io/colored/tables/colors/#full-chart-256-foreground-and-background-colors)
 for <a href="https://en.wikipedia.org/wiki/Xterm" target="_blank">Xterm</a>, containing an example of the displayed color, Xterm Name, Xterm Number and HEX.
 
 The colors work with most terminals and terminals emulators.
 <a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">ANSI/VT100 escape sequences</a> can be used in every programming languages.
 
 Colored is powerful and easy to use:
 
@@ -42,19 +46,23 @@
 >>>
 >>> Back.red
 '\x1b[48;5;1m'
 >>>
 >>> Style.reset
 '\x1b[0m'
 >>> 
+>>> Fore.rgb('100%', '50%', '30%')
+'\x1b[38;2;255;130;79m'
+>>>
 >>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}')
 ```
-<p> >>> <span style="background-color: green">
-  <span style="color: white">Colored is Awesome!!!</span></span>
-</p>
+!!! success
+    <p> >>> <span style="background-color: green">
+      <span style="color: white">Colored is Awesome!!!</span></span>
+    </p>
 
 ## Installing
 
 Open up a terminal and install colored with <a href="https://pip.pypa.io/en/stable/" target="_blank">pip</a> command:
 
 ```bash
 $ pip install colored
@@ -75,17 +83,15 @@
 
 ## License
 
 colored is made available under the MIT License. For more details, see [here](https://dslackw.gitlab.io/colored/license/#mit-license).
 
 ## Contributing
 
-
-We happily welcome [contributions](https://dslackw.gitlab.io/colored/contributors/)!
+!!! info
+    We happily welcome [contributions](https://dslackw.gitlab.io/colored/contributors/)!
 
 ## Donate
 
 Did you know that we developers love coffee? 
 
-Donate me a coffee ☕ ⬇
-
 [<img src="https://gitlab.com/dslackw/colored/-/raw/site/docs/images/paypaldonate.png" alt="paypal" title="donate">](https://www.paypal.me/dslackw)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,36 +1,43 @@
-Metadata-Version: 2.1 Name: colored Version: 2.2.0 Summary: Simple python
+Metadata-Version: 2.1 Name: colored Version: 2.2.1 Summary: Simple python
 library for color and formatting to terminal Keywords:
-xterm,color,vt100,ansi,terminal,python Author-email: Dimitris Zlatanidis
+xterm,color,colour,vt100,ansi,terminal,text,rgb,linux,windows Author-email:
+Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Other Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: Microsoft :: Windows :: Windows 10 Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Terminals Project-URL: homepage, https://
 dslackw.gitlab.io/colored/ [https://gitlab.com/dslackw/colored/-/raw/site/docs/
 images/colored.png] ## About Colored, it's a simple Python library for color
 and formatting in terminal. Collection of color codes and names for 256 color
-terminal setups. A list of [256 colors](https://dslackw.gitlab.io/colored/
-formatting/colors/#full-chart-256-foreground-and-background-colors) for Xterm,
-containing an example of the displayed color, Xterm Name, Xterm Number and HEX.
-The colors work with most terminals and terminals emulators. ANSI/VT100_escape
-sequences can be used in every programming languages. Colored is powerful and
-easy to use: ```python title="Python 3.9.17" >>> from colored import Fore,
-Back, Style >>> >>> Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>>
->>> Style.reset '\x1b[0m' >>> >>> print(f'{Fore.white}{Back.green}Colored is
-Awesome!!!{Style.reset}') ```
+terminal setups. Colored now supports RGB color mode. As "true color" graphic
+cards with 16 to 24_bits of color became common, applications began to support
+24-bit colors. Terminal emulators supporting setting 24-bit foreground and
+background colors with escape sequences include Xterm, KDE's Konsole, and
+iTerm, as well as all libvte based terminals, including GNOME_Terminal. A list
+of [256 colors](https://dslackw.gitlab.io/colored/tables/colors/#full-chart-
+256-foreground-and-background-colors) for Xterm, containing an example of the
+displayed color, Xterm Name, Xterm Number and HEX. The colors work with most
+terminals and terminals emulators. ANSI/VT100_escape_sequences can be used in
+every programming languages. Colored is powerful and easy to use: ```python
+title="Python 3.9.17" >>> from colored import Fore, Back, Style >>> >>>
+Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>> >>> Style.reset
+'\x1b[0m' >>> >>> Fore.rgb('100%', '50%', '30%') '\x1b[38;2;255;130;79m' >>>
+>>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}') ```
+!!! success
 >>>  Colored is Awesome!!!
 ## Installing Open up a terminal and install colored with pip command: ```bash
 $ pip install colored ``` Alternatively, you can grab the latest source code
 from GitLab: ```bash $ git clone https://gitlab.com/dslackw/colored.git $ cd
 colored $ pip install . ``` ## Usage The [User Guide](https://
 dslackw.gitlab.io/colored/user_guide/user_guide/#user-guide) is the place to go
 to learn how to use the library. The [API Reference](https://dslackw.gitlab.io/
 colored/api/attributes/) documentation provides API-level documentation. ##
 License colored is made available under the MIT License. For more details, see
 [here](https://dslackw.gitlab.io/colored/license/#mit-license). ## Contributing
-We happily welcome [contributions](https://dslackw.gitlab.io/colored/
-contributors/)! ## Donate Did you know that we developers love coffee? Donate
-me a coffee â â¬ [[paypal]](https://www.paypal.me/dslackw)
+!!! info We happily welcome [contributions](https://dslackw.gitlab.io/colored/
+contributors/)! ## Donate Did you know that we developers love coffee? [
+[paypal]](https://www.paypal.me/dslackw)
```

