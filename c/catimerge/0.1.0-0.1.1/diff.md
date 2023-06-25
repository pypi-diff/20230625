# Comparing `tmp/catimerge-0.1.0.tar.gz` & `tmp/catimerge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catimerge-0.1.0.tar", last modified: Sun Jun 25 15:39:34 2023, max compression
+gzip compressed data, was "catimerge-0.1.1.tar", last modified: Sun Jun 25 20:39:16 2023, max compression
```

## Comparing `catimerge-0.1.0.tar` & `catimerge-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 15:39:34.579613 catimerge-0.1.0/
--rw-------   0 fay       (1000) fay       (1000)    34523 2023-06-23 14:00:18.000000 catimerge-0.1.0/LICENSE.AGPLv3
--rw-------   0 fay       (1000) fay       (1000)       85 2023-06-23 17:01:34.000000 catimerge-0.1.0/MANIFEST.in
--rw-------   0 fay       (1000) fay       (1000)      891 2023-06-25 14:54:10.000000 catimerge-0.1.0/Makefile
--rw-------   0 fay       (1000) fay       (1000)     4941 2023-06-25 15:39:34.579613 catimerge-0.1.0/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)     3795 2023-06-24 11:24:56.000000 catimerge-0.1.0/README.md
-drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 15:39:34.579613 catimerge-0.1.0/catimerge/
--rwx------   0 fay       (1000) fay       (1000)    13668 2023-06-25 15:21:32.000000 catimerge-0.1.0/catimerge/__init__.py
--rw-------   0 fay       (1000) fay       (1000)        0 2023-06-23 16:53:48.000000 catimerge-0.1.0/catimerge/py.typed
-drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 15:39:34.579613 catimerge-0.1.0/catimerge.egg-info/
--rw-------   0 fay       (1000) fay       (1000)     4941 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)      277 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/SOURCES.txt
--rw-------   0 fay       (1000) fay       (1000)        1 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/dependency_links.txt
--rw-------   0 fay       (1000) fay       (1000)       45 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/entry_points.txt
--rw-------   0 fay       (1000) fay       (1000)       10 2023-06-25 15:39:34.000000 catimerge-0.1.0/catimerge.egg-info/top_level.txt
--rw-------   0 fay       (1000) fay       (1000)      188 2023-06-25 15:26:25.000000 catimerge-0.1.0/changelog.txt
--rw-------   0 fay       (1000) fay       (1000)       38 2023-06-25 15:39:34.579613 catimerge-0.1.0/setup.cfg
--rw-------   0 fay       (1000) fay       (1000)     1707 2023-06-23 16:54:57.000000 catimerge-0.1.0/setup.py
+drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 20:39:16.405307 catimerge-0.1.1/
+-rw-------   0 fay       (1000) fay       (1000)    34523 2023-06-23 14:00:18.000000 catimerge-0.1.1/LICENSE.AGPLv3
+-rw-------   0 fay       (1000) fay       (1000)       85 2023-06-23 17:01:34.000000 catimerge-0.1.1/MANIFEST.in
+-rw-------   0 fay       (1000) fay       (1000)      891 2023-06-25 14:54:10.000000 catimerge-0.1.1/Makefile
+-rw-------   0 fay       (1000) fay       (1000)     5121 2023-06-25 20:39:16.401307 catimerge-0.1.1/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)     3975 2023-06-25 18:30:55.000000 catimerge-0.1.1/README.md
+drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 20:39:16.401307 catimerge-0.1.1/catimerge/
+-rwx------   0 fay       (1000) fay       (1000)    15713 2023-06-25 20:37:17.000000 catimerge-0.1.1/catimerge/__init__.py
+-rw-------   0 fay       (1000) fay       (1000)        0 2023-06-23 16:53:48.000000 catimerge-0.1.1/catimerge/py.typed
+drwx------   0 fay       (1000) fay       (1000)        0 2023-06-25 20:39:16.401307 catimerge-0.1.1/catimerge.egg-info/
+-rw-------   0 fay       (1000) fay       (1000)     5121 2023-06-25 20:39:16.000000 catimerge-0.1.1/catimerge.egg-info/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)      277 2023-06-25 20:39:16.000000 catimerge-0.1.1/catimerge.egg-info/SOURCES.txt
+-rw-------   0 fay       (1000) fay       (1000)        1 2023-06-25 20:39:16.000000 catimerge-0.1.1/catimerge.egg-info/dependency_links.txt
+-rw-------   0 fay       (1000) fay       (1000)       75 2023-06-25 20:39:16.000000 catimerge-0.1.1/catimerge.egg-info/entry_points.txt
+-rw-------   0 fay       (1000) fay       (1000)       10 2023-06-25 20:39:16.000000 catimerge-0.1.1/catimerge.egg-info/top_level.txt
+-rw-------   0 fay       (1000) fay       (1000)      209 2023-06-25 20:37:08.000000 catimerge-0.1.1/changelog.txt
+-rw-------   0 fay       (1000) fay       (1000)       38 2023-06-25 20:39:16.405307 catimerge-0.1.1/setup.cfg
+-rw-------   0 fay       (1000) fay       (1000)     1823 2023-06-25 17:30:15.000000 catimerge-0.1.1/setup.py
```

### Comparing `catimerge-0.1.0/LICENSE.AGPLv3` & `catimerge-0.1.1/LICENSE.AGPLv3`

 * *Files identical despite different names*

### Comparing `catimerge-0.1.0/Makefile` & `catimerge-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `catimerge-0.1.0/PKG-INFO` & `catimerge-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catimerge
-Version: 0.1.0
+Version: 0.1.1
 Summary: merge two catima.zip exports
 Home-page: https://github.com/obfusk/catimerge
 Author: FC Stegerman
 Author-email: flx@obfusk.net
 License: AGPLv3+
 Keywords: catima export merge
 Classifier: Development Status :: 3 - Alpha
@@ -72,14 +72,20 @@
 ZIP #1 has   1 group(s),   9 card(s),   2 card group(s),   5 image file(s)
 ZIP #2 has   2 group(s),   5 card(s),   3 card group(s),   3 image file(s)
 Merging...
 Output has   3 group(s),  14 card(s),   5 card group(s),   8 image file(s)
 Writing...
 ```
 
+## GUI
+
+The additional `catimerge-gui` command provides a simple GUI.
+
+![screenshot](gui.png)
+
 ## CAVEATS
 
 Unfortunately, Python does not support the password-protected ZIP
 files created by Catima.  You can either export your data without a
 password, or use a tool like 7-Zip to create a temporary passwordless
 ZIP file for the merge process.
 
@@ -156,14 +162,20 @@
 ```bash
 $ cd catimerge
 $ git pull --rebase
 ```
 
 ## Dependencies
 
-* Python >= 3.8.
+* Python >= 3.8 (w/ Tk support for the GUI).
+
+### Debian/Ubuntu
+
+```bash
+$ apt install python3-tk
+```
 
 ## License
 
 [![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://www.gnu.org/licenses/agpl-3.0.html)
 
 <!-- vim: set tw=70 sw=2 sts=2 et fdm=marker : -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catimerge Version: 0.1.0 Summary: merge two
+Metadata-Version: 2.1 Name: catimerge Version: 0.1.1 Summary: merge two
 catima.zip exports Home-page: https://github.com/obfusk/catimerge Author: FC
 Stegerman Author-email: flx@obfusk.net License: AGPLv3+ Keywords: catima export
 merge Classifier: Development Status :: 3 - Alpha Classifier: Environment ::
 Console Classifier: Intended Audience :: End Users/Desktop Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: POSIX Classifier: Operating
@@ -26,31 +26,34 @@
 FIRST_ZIP SECOND_ZIP OUTPUT_ZIP positional arguments: FIRST_ZIP SECOND_ZIP
 OUTPUT_ZIP options: -h, --help show this help message and exit -v, --verbose --
 version show program's version number and exit $ catimerge -v catima1.zip
 catima2.zip out.zip Merging 'catima1.zip' and 'catima2.zip' into 'out.zip'...
 Parsing... Version: 2 ZIP #1 has 1 group(s), 9 card(s), 2 card group(s), 5
 image file(s) ZIP #2 has 2 group(s), 5 card(s), 3 card group(s), 3 image file
 (s) Merging... Output has 3 group(s), 14 card(s), 5 card group(s), 8 image file
-(s) Writing... ``` ## CAVEATS Unfortunately, Python does not support the
-password-protected ZIP files created by Catima. You can either export your data
-without a password, or use a tool like 7-Zip to create a temporary passwordless
-ZIP file for the merge process. For example, if you have two password-protected
-ZIP files as input and want a password-protected output ZIP file as well:
-```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x catima1.zip # extract into
-catima1/ [...] $ 7z -ocatima2 x catima2.zip # extract into catima2/ [...] $ cd
-catima1 $ 7z a ../catima1-nopass.zip * # create passwordless ZIP [...] $ cd ..
-$ cd catima2 $ 7z a ../catima2-nopass.zip * # create passwordless ZIP [...] $
-cd .. $ catimerge -v catima1-nopass.zip catima2-nopass.zip out-nopass.zip
-Merging 'catima1-nopass.zip' and 'catima2-nopass.zip' into 'out-nopass.zip'...
-[...] $ 7z -oout-nopass x out-nopass.zip # extract into out-nopass/ $ cd out-
-nopass $ 7z -p a ../out.zip * # create password-protected ZIP [...] $ cd .. $
-ls catima1 catima1-nopass.zip catima1.zip catima2 catima2-nopass.zip
-catima2.zip out-nopass out-nopass.zip out.zip ```  ## Installing ### Using pip
-```bash $ pip install catimerge ``` NB: depending on your system you may need
-to use e.g. `pip3 --user` instead of just `pip`. ### From git NB: this installs
-the latest development version, not the latest release. ```bash $ git clone
-https://github.com/obfusk/catimerge.git $ cd catimerge $ pip install -e . ```
-NB: you may need to add e.g. `~/.local/bin` to your `$PATH` in order to run
-`catimerge`. To update to the latest development version: ```bash $ cd
-catimerge $ git pull --rebase ``` ## Dependencies * Python >= 3.8. ## License
-[![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://
-www.gnu.org/licenses/agpl-3.0.html)
+(s) Writing... ``` ## GUI The additional `catimerge-gui` command provides a
+simple GUI. ![screenshot](gui.png) ## CAVEATS Unfortunately, Python does not
+support the password-protected ZIP files created by Catima. You can either
+export your data without a password, or use a tool like 7-Zip to create a
+temporary passwordless ZIP file for the merge process. For example, if you have
+two password-protected ZIP files as input and want a password-protected output
+ZIP file as well:  ```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x
+catima1.zip # extract into catima1/ [...] $ 7z -ocatima2 x catima2.zip #
+extract into catima2/ [...] $ cd catima1 $ 7z a ../catima1-nopass.zip * #
+create passwordless ZIP [...] $ cd .. $ cd catima2 $ 7z a ../catima2-nopass.zip
+* # create passwordless ZIP [...] $ cd .. $ catimerge -v catima1-nopass.zip
+catima2-nopass.zip out-nopass.zip Merging 'catima1-nopass.zip' and 'catima2-
+nopass.zip' into 'out-nopass.zip'... [...] $ 7z -oout-nopass x out-nopass.zip #
+extract into out-nopass/ $ cd out-nopass $ 7z -p a ../out.zip * # create
+password-protected ZIP [...] $ cd .. $ ls catima1 catima1-nopass.zip
+catima1.zip catima2 catima2-nopass.zip catima2.zip out-nopass out-nopass.zip
+out.zip ```  ## Installing ### Using pip ```bash $ pip install catimerge ```
+NB: depending on your system you may need to use e.g. `pip3 --user` instead of
+just `pip`. ### From git NB: this installs the latest development version, not
+the latest release. ```bash $ git clone https://github.com/obfusk/catimerge.git
+$ cd catimerge $ pip install -e . ``` NB: you may need to add e.g. `~/.local/
+bin` to your `$PATH` in order to run `catimerge`. To update to the latest
+development version: ```bash $ cd catimerge $ git pull --rebase ``` ##
+Dependencies * Python >= 3.8 (w/ Tk support for the GUI). ### Debian/Ubuntu
+```bash $ apt install python3-tk ``` ## License [![AGPLv3+](https://
+www.gnu.org/graphics/agplv3-155x51.png)](https://www.gnu.org/licenses/agpl-
+3.0.html)
```

### Comparing `catimerge-0.1.0/README.md` & `catimerge-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,20 @@
 ZIP #1 has   1 group(s),   9 card(s),   2 card group(s),   5 image file(s)
 ZIP #2 has   2 group(s),   5 card(s),   3 card group(s),   3 image file(s)
 Merging...
 Output has   3 group(s),  14 card(s),   5 card group(s),   8 image file(s)
 Writing...
 ```
 
+## GUI
+
+The additional `catimerge-gui` command provides a simple GUI.
+
+![screenshot](gui.png)
+
 ## CAVEATS
 
 Unfortunately, Python does not support the password-protected ZIP
 files created by Catima.  You can either export your data without a
 password, or use a tool like 7-Zip to create a temporary passwordless
 ZIP file for the merge process.
 
@@ -127,14 +133,20 @@
 ```bash
 $ cd catimerge
 $ git pull --rebase
 ```
 
 ## Dependencies
 
-* Python >= 3.8.
+* Python >= 3.8 (w/ Tk support for the GUI).
+
+### Debian/Ubuntu
+
+```bash
+$ apt install python3-tk
+```
 
 ## License
 
 [![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://www.gnu.org/licenses/agpl-3.0.html)
 
 <!-- vim: set tw=70 sw=2 sts=2 et fdm=marker : -->
```

#### html2text {}

```diff
@@ -11,31 +11,34 @@
 FIRST_ZIP SECOND_ZIP OUTPUT_ZIP positional arguments: FIRST_ZIP SECOND_ZIP
 OUTPUT_ZIP options: -h, --help show this help message and exit -v, --verbose --
 version show program's version number and exit $ catimerge -v catima1.zip
 catima2.zip out.zip Merging 'catima1.zip' and 'catima2.zip' into 'out.zip'...
 Parsing... Version: 2 ZIP #1 has 1 group(s), 9 card(s), 2 card group(s), 5
 image file(s) ZIP #2 has 2 group(s), 5 card(s), 3 card group(s), 3 image file
 (s) Merging... Output has 3 group(s), 14 card(s), 5 card group(s), 8 image file
-(s) Writing... ``` ## CAVEATS Unfortunately, Python does not support the
-password-protected ZIP files created by Catima. You can either export your data
-without a password, or use a tool like 7-Zip to create a temporary passwordless
-ZIP file for the merge process. For example, if you have two password-protected
-ZIP files as input and want a password-protected output ZIP file as well:
-```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x catima1.zip # extract into
-catima1/ [...] $ 7z -ocatima2 x catima2.zip # extract into catima2/ [...] $ cd
-catima1 $ 7z a ../catima1-nopass.zip * # create passwordless ZIP [...] $ cd ..
-$ cd catima2 $ 7z a ../catima2-nopass.zip * # create passwordless ZIP [...] $
-cd .. $ catimerge -v catima1-nopass.zip catima2-nopass.zip out-nopass.zip
-Merging 'catima1-nopass.zip' and 'catima2-nopass.zip' into 'out-nopass.zip'...
-[...] $ 7z -oout-nopass x out-nopass.zip # extract into out-nopass/ $ cd out-
-nopass $ 7z -p a ../out.zip * # create password-protected ZIP [...] $ cd .. $
-ls catima1 catima1-nopass.zip catima1.zip catima2 catima2-nopass.zip
-catima2.zip out-nopass out-nopass.zip out.zip ```  ## Installing ### Using pip
-```bash $ pip install catimerge ``` NB: depending on your system you may need
-to use e.g. `pip3 --user` instead of just `pip`. ### From git NB: this installs
-the latest development version, not the latest release. ```bash $ git clone
-https://github.com/obfusk/catimerge.git $ cd catimerge $ pip install -e . ```
-NB: you may need to add e.g. `~/.local/bin` to your `$PATH` in order to run
-`catimerge`. To update to the latest development version: ```bash $ cd
-catimerge $ git pull --rebase ``` ## Dependencies * Python >= 3.8. ## License
-[![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://
-www.gnu.org/licenses/agpl-3.0.html)
+(s) Writing... ``` ## GUI The additional `catimerge-gui` command provides a
+simple GUI. ![screenshot](gui.png) ## CAVEATS Unfortunately, Python does not
+support the password-protected ZIP files created by Catima. You can either
+export your data without a password, or use a tool like 7-Zip to create a
+temporary passwordless ZIP file for the merge process. For example, if you have
+two password-protected ZIP files as input and want a password-protected output
+ZIP file as well:  ```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x
+catima1.zip # extract into catima1/ [...] $ 7z -ocatima2 x catima2.zip #
+extract into catima2/ [...] $ cd catima1 $ 7z a ../catima1-nopass.zip * #
+create passwordless ZIP [...] $ cd .. $ cd catima2 $ 7z a ../catima2-nopass.zip
+* # create passwordless ZIP [...] $ cd .. $ catimerge -v catima1-nopass.zip
+catima2-nopass.zip out-nopass.zip Merging 'catima1-nopass.zip' and 'catima2-
+nopass.zip' into 'out-nopass.zip'... [...] $ 7z -oout-nopass x out-nopass.zip #
+extract into out-nopass/ $ cd out-nopass $ 7z -p a ../out.zip * # create
+password-protected ZIP [...] $ cd .. $ ls catima1 catima1-nopass.zip
+catima1.zip catima2 catima2-nopass.zip catima2.zip out-nopass out-nopass.zip
+out.zip ```  ## Installing ### Using pip ```bash $ pip install catimerge ```
+NB: depending on your system you may need to use e.g. `pip3 --user` instead of
+just `pip`. ### From git NB: this installs the latest development version, not
+the latest release. ```bash $ git clone https://github.com/obfusk/catimerge.git
+$ cd catimerge $ pip install -e . ``` NB: you may need to add e.g. `~/.local/
+bin` to your `$PATH` in order to run `catimerge`. To update to the latest
+development version: ```bash $ cd catimerge $ git pull --rebase ``` ##
+Dependencies * Python >= 3.8 (w/ Tk support for the GUI). ### Debian/Ubuntu
+```bash $ apt install python3-tk ``` ## License [![AGPLv3+](https://
+www.gnu.org/graphics/agplv3-155x51.png)](https://www.gnu.org/licenses/agpl-
+3.0.html)
```

### Comparing `catimerge-0.1.0/catimerge/__init__.py` & `catimerge-0.1.1/catimerge/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 
 import csv
 import io
 import re
 import zipfile
 
 from dataclasses import dataclass, field, fields
-from typing import Dict, List, TextIO, Tuple
+from typing import Dict, List, Optional, TextIO, Tuple
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 IMAGE_REGEX_V2 = re.compile(r"(card_)(\d+)(_(?:front|back|icon)\.png)")
 
 
 class Error(Exception):
     """Base class for errors."""
 
 
@@ -357,11 +357,66 @@
     parser.add_argument("second_zip", metavar="SECOND_ZIP")
     parser.add_argument("output_zip", metavar="OUTPUT_ZIP")
     args = parser.parse_args()
     catimerge(args.first_zip, args.second_zip, args.output_zip,
               verbose=args.verbose)
 
 
+def gui() -> None:
+    import tkinter as tk
+    from tkinter import ttk, filedialog, messagebox
+
+    def select_file(i: int, lbl: ttk.Label, what: str, save: bool = False) -> None:
+        title = f"Select {what}"
+        filetypes = [("ZIP files", "*.zip")]
+        if save:
+            file = filedialog.asksaveasfilename(title=title, filetypes=filetypes)
+        else:
+            file = filedialog.askopenfilename(title=title, filetypes=filetypes)
+        if file:
+            files[i] = file
+            lbl.config(text=file)
+            if all(files):
+                btn_merge.config(state=tk.NORMAL)
+
+    def on_open1() -> None:
+        select_file(0, lbl_file1, "ZIP #1")
+
+    def on_open2() -> None:
+        select_file(1, lbl_file2, "ZIP #2")
+
+    def on_open3() -> None:
+        select_file(2, lbl_file3, "output ZIP", save=True)
+
+    def on_merge() -> None:
+        try:
+            first_zip, second_zip, output_zip = files
+            assert first_zip and second_zip and output_zip
+            catimerge(first_zip, second_zip, output_zip)
+        except (Error, zipfile.BadZipFile) as e:
+            messagebox.showerror(title="catimerge", message=f"Error: {e}")
+        else:
+            messagebox.showinfo(title="catimerge", message="Saved")
+
+    files: List[Optional[str]] = [None, None, None]
+    nofile = "(no file selected)"
+    win = tk.Tk()
+    win.title("catimerge")
+    btn_open1 = ttk.Button(win, text="Select ZIP #1", command=on_open1)
+    lbl_file1 = ttk.Label(win, text=nofile)
+    btn_open2 = ttk.Button(win, text="Select ZIP #2", command=on_open2)
+    lbl_file2 = ttk.Label(win, text=nofile)
+    btn_open3 = ttk.Button(win, text="Select output ZIP", command=on_open3)
+    lbl_file3 = ttk.Label(win, text=nofile)
+    btn_merge = ttk.Button(win, text="Merge", command=on_merge)
+    btn_merge.config(state=tk.DISABLED)
+    for w in [btn_open1, lbl_file1, btn_open2, lbl_file2, btn_open3, lbl_file3, btn_merge]:
+        w.pack(padx=5, pady=5)
+    win.minsize(400, 250)
+    win.update()
+    win.mainloop()
+
+
 if __name__ == "__main__":
     main()
 
 # vim: set tw=80 sw=4 sts=4 et fdm=marker :
```

### Comparing `catimerge-0.1.0/catimerge.egg-info/PKG-INFO` & `catimerge-0.1.1/catimerge.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catimerge
-Version: 0.1.0
+Version: 0.1.1
 Summary: merge two catima.zip exports
 Home-page: https://github.com/obfusk/catimerge
 Author: FC Stegerman
 Author-email: flx@obfusk.net
 License: AGPLv3+
 Keywords: catima export merge
 Classifier: Development Status :: 3 - Alpha
@@ -72,14 +72,20 @@
 ZIP #1 has   1 group(s),   9 card(s),   2 card group(s),   5 image file(s)
 ZIP #2 has   2 group(s),   5 card(s),   3 card group(s),   3 image file(s)
 Merging...
 Output has   3 group(s),  14 card(s),   5 card group(s),   8 image file(s)
 Writing...
 ```
 
+## GUI
+
+The additional `catimerge-gui` command provides a simple GUI.
+
+![screenshot](gui.png)
+
 ## CAVEATS
 
 Unfortunately, Python does not support the password-protected ZIP
 files created by Catima.  You can either export your data without a
 password, or use a tool like 7-Zip to create a temporary passwordless
 ZIP file for the merge process.
 
@@ -156,14 +162,20 @@
 ```bash
 $ cd catimerge
 $ git pull --rebase
 ```
 
 ## Dependencies
 
-* Python >= 3.8.
+* Python >= 3.8 (w/ Tk support for the GUI).
+
+### Debian/Ubuntu
+
+```bash
+$ apt install python3-tk
+```
 
 ## License
 
 [![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://www.gnu.org/licenses/agpl-3.0.html)
 
 <!-- vim: set tw=70 sw=2 sts=2 et fdm=marker : -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catimerge Version: 0.1.0 Summary: merge two
+Metadata-Version: 2.1 Name: catimerge Version: 0.1.1 Summary: merge two
 catima.zip exports Home-page: https://github.com/obfusk/catimerge Author: FC
 Stegerman Author-email: flx@obfusk.net License: AGPLv3+ Keywords: catima export
 merge Classifier: Development Status :: 3 - Alpha Classifier: Environment ::
 Console Classifier: Intended Audience :: End Users/Desktop Classifier: License
 :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: POSIX Classifier: Operating
@@ -26,31 +26,34 @@
 FIRST_ZIP SECOND_ZIP OUTPUT_ZIP positional arguments: FIRST_ZIP SECOND_ZIP
 OUTPUT_ZIP options: -h, --help show this help message and exit -v, --verbose --
 version show program's version number and exit $ catimerge -v catima1.zip
 catima2.zip out.zip Merging 'catima1.zip' and 'catima2.zip' into 'out.zip'...
 Parsing... Version: 2 ZIP #1 has 1 group(s), 9 card(s), 2 card group(s), 5
 image file(s) ZIP #2 has 2 group(s), 5 card(s), 3 card group(s), 3 image file
 (s) Merging... Output has 3 group(s), 14 card(s), 5 card group(s), 8 image file
-(s) Writing... ``` ## CAVEATS Unfortunately, Python does not support the
-password-protected ZIP files created by Catima. You can either export your data
-without a password, or use a tool like 7-Zip to create a temporary passwordless
-ZIP file for the merge process. For example, if you have two password-protected
-ZIP files as input and want a password-protected output ZIP file as well:
-```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x catima1.zip # extract into
-catima1/ [...] $ 7z -ocatima2 x catima2.zip # extract into catima2/ [...] $ cd
-catima1 $ 7z a ../catima1-nopass.zip * # create passwordless ZIP [...] $ cd ..
-$ cd catima2 $ 7z a ../catima2-nopass.zip * # create passwordless ZIP [...] $
-cd .. $ catimerge -v catima1-nopass.zip catima2-nopass.zip out-nopass.zip
-Merging 'catima1-nopass.zip' and 'catima2-nopass.zip' into 'out-nopass.zip'...
-[...] $ 7z -oout-nopass x out-nopass.zip # extract into out-nopass/ $ cd out-
-nopass $ 7z -p a ../out.zip * # create password-protected ZIP [...] $ cd .. $
-ls catima1 catima1-nopass.zip catima1.zip catima2 catima2-nopass.zip
-catima2.zip out-nopass out-nopass.zip out.zip ```  ## Installing ### Using pip
-```bash $ pip install catimerge ``` NB: depending on your system you may need
-to use e.g. `pip3 --user` instead of just `pip`. ### From git NB: this installs
-the latest development version, not the latest release. ```bash $ git clone
-https://github.com/obfusk/catimerge.git $ cd catimerge $ pip install -e . ```
-NB: you may need to add e.g. `~/.local/bin` to your `$PATH` in order to run
-`catimerge`. To update to the latest development version: ```bash $ cd
-catimerge $ git pull --rebase ``` ## Dependencies * Python >= 3.8. ## License
-[![AGPLv3+](https://www.gnu.org/graphics/agplv3-155x51.png)](https://
-www.gnu.org/licenses/agpl-3.0.html)
+(s) Writing... ``` ## GUI The additional `catimerge-gui` command provides a
+simple GUI. ![screenshot](gui.png) ## CAVEATS Unfortunately, Python does not
+support the password-protected ZIP files created by Catima. You can either
+export your data without a password, or use a tool like 7-Zip to create a
+temporary passwordless ZIP file for the merge process. For example, if you have
+two password-protected ZIP files as input and want a password-protected output
+ZIP file as well:  ```sh $ ls catima1.zip catima2.zip $ 7z -ocatima1 x
+catima1.zip # extract into catima1/ [...] $ 7z -ocatima2 x catima2.zip #
+extract into catima2/ [...] $ cd catima1 $ 7z a ../catima1-nopass.zip * #
+create passwordless ZIP [...] $ cd .. $ cd catima2 $ 7z a ../catima2-nopass.zip
+* # create passwordless ZIP [...] $ cd .. $ catimerge -v catima1-nopass.zip
+catima2-nopass.zip out-nopass.zip Merging 'catima1-nopass.zip' and 'catima2-
+nopass.zip' into 'out-nopass.zip'... [...] $ 7z -oout-nopass x out-nopass.zip #
+extract into out-nopass/ $ cd out-nopass $ 7z -p a ../out.zip * # create
+password-protected ZIP [...] $ cd .. $ ls catima1 catima1-nopass.zip
+catima1.zip catima2 catima2-nopass.zip catima2.zip out-nopass out-nopass.zip
+out.zip ```  ## Installing ### Using pip ```bash $ pip install catimerge ```
+NB: depending on your system you may need to use e.g. `pip3 --user` instead of
+just `pip`. ### From git NB: this installs the latest development version, not
+the latest release. ```bash $ git clone https://github.com/obfusk/catimerge.git
+$ cd catimerge $ pip install -e . ``` NB: you may need to add e.g. `~/.local/
+bin` to your `$PATH` in order to run `catimerge`. To update to the latest
+development version: ```bash $ cd catimerge $ git pull --rebase ``` ##
+Dependencies * Python >= 3.8 (w/ Tk support for the GUI). ### Debian/Ubuntu
+```bash $ apt install python3-tk ``` ## License [![AGPLv3+](https://
+www.gnu.org/graphics/agplv3-155x51.png)](https://www.gnu.org/licenses/agpl-
+3.0.html)
```

### Comparing `catimerge-0.1.0/setup.py` & `catimerge-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,12 +31,15 @@
         "Programming Language :: Python :: 3.11",
       # "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Utilities",
     ],
     keywords          = "catima export merge",
-    entry_points      = dict(console_scripts = ["catimerge = catimerge:main"]),
+    entry_points      = dict(console_scripts = [
+                            "catimerge = catimerge:main",
+                            "catimerge-gui = catimerge:gui",
+                        ]),
     packages          = ["catimerge"],
     package_data      = dict(catimerge = ["py.typed"]),
     python_requires   = ">=3.8",
 )
```

