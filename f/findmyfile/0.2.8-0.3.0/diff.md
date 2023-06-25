# Comparing `tmp/findmyfile-0.2.8.tar.gz` & `tmp/findmyfile-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyfile-0.2.8.tar", last modified: Sun Jun 25 00:54:26 2023, max compression
+gzip compressed data, was "findmyfile-0.3.0.tar", last modified: Sun Jun 25 02:19:32 2023, max compression
```

## Comparing `findmyfile-0.2.8.tar` & `findmyfile-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 00:54:26.845000 findmyfile-0.2.8/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.2.8/LICENCE.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-25 00:54:26.823000 findmyfile-0.2.8/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     3085 2023-06-25 00:01:41.000000 findmyfile-0.2.8/README.md
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 00:54:26.356000 findmyfile-0.2.8/findmyfile/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.2.8/findmyfile/__init__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.2.8/findmyfile/__main__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     9124 2023-06-25 00:31:06.000000 findmyfile-0.2.8/findmyfile/main.py
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 00:54:26.761000 findmyfile-0.2.8/findmyfile.egg-info/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/SOURCES.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/dependency_links.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/entry_points.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       53 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/requires.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/top_level.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-25 00:54:26.841000 findmyfile-0.2.8/setup.cfg
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1715 2023-06-25 00:53:54.000000 findmyfile-0.2.8/setup.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 02:19:32.556000 findmyfile-0.3.0/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.3.0/LICENCE.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      687 2023-06-25 02:19:32.536000 findmyfile-0.3.0/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     4316 2023-06-25 02:18:06.000000 findmyfile-0.3.0/README.md
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 02:19:31.915000 findmyfile-0.3.0/findmyfile/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.3.0/findmyfile/__init__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.3.0/findmyfile/__main__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     9362 2023-06-25 02:06:09.000000 findmyfile-0.3.0/findmyfile/main.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 02:19:32.464000 findmyfile-0.3.0/findmyfile.egg-info/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      687 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/entry_points.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       53 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/requires.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-25 02:19:31.000000 findmyfile-0.3.0/findmyfile.egg-info/top_level.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-25 02:19:32.553000 findmyfile-0.3.0/setup.cfg
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1714 2023-06-25 02:07:41.000000 findmyfile-0.3.0/setup.py
```

### Comparing `findmyfile-0.2.8/LICENCE.txt` & `findmyfile-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `findmyfile-0.2.8/PKG-INFO` & `findmyfile-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.2.8
+Version: 0.3.0
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENCE.txt
```

### Comparing `findmyfile-0.2.8/README.md` & `findmyfile-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,29 @@
-# FMF (File My File)
+# FMF (Find My File)
 
 FMF is a powerful file management system that reads and searches text within files in various formats including PPTX, DOCX, XLSX, PDF, and TXT. It traverses the given directory and its sub-directories and reads the content of the supported files. It provides functionality to search for one or more keywords across all files.
 
 ---
 
+## Installation
+
+You can install FMF directly from the Python Package Index using pip. Open a terminal and run the following command:
+
+```bash
+pip install findmyfile
+```
+
+Please ensure that you have `pip` installed and that your Python environment is correctly set up.
+
+After successful installation, you can use FMF as a library in your project or as a CLI command. 
+
+You can find the findmyfile project on PyPi here: [findmyfile](https://pypi.org/project/findmyfile)
+
+---
+
 ## Usage
 
 ### As a Library
 
 FMF can be imported into your project as a library, and its classes can be used independently. Below are some usage examples:
 
 **Example 1:** Reading a specific .docx file.
@@ -25,30 +41,42 @@
 ```python
 from fmf import FilesDB
 
 db = FilesDB('path/to/directory')
 db.search('keyword1', 'keyword2')
 ```
 
-### As a Script
+Sure, here is a reworded version:
+
+### As a CLI Command
+
+After installation, you can directly use the `fmf` command in your terminal. Here are some usage examples:
 
-You can also run FMF as a standalone script. Here's how you can do it:
+**Example 1:** Searching within files in the current directory
 
-**Example 1:** Reading and searching files in the current directory
+To search for keywords within the files of your current directory, use the following format:
 
 ```bash
-python fmf.py -w keyword1 keyword2
+fmf -w keyword1 keyword2
 ```
 
-**Example 2:** Reading and searching files in a specific directory
+This command will search for `keyword1` and `keyword2` within the files of the directory you're currently in.
+
+**Example 2:** Searching within files in a specific directory
+
+If you want to search for keywords within a specific directory, include the `-path` argument followed by the path to the directory. Here's the format:
 
 ```bash
-python fmf.py -path "path/to/directory" -w keyword1 keyword2
+fmf -path "/path/to/directory" -w keyword1 keyword2
 ```
 
+Replace `/path/to/directory` with the path to your desired directory. This command will then search for `keyword1` and `keyword2` within the files of the specified directory.
+
+Please note that `fmf` does not search in subdirectories. If you want to search in a subdirectory, you need to specify it in the `-path` argument.
+
 ---
 
 ## Classes and Methods
 
 **File**: The base class for all file types.
 
 - **`create(path, extension)`**: A classmethod to create a new File object.
```

### Comparing `findmyfile-0.2.8/findmyfile/main.py` & `findmyfile-0.3.0/findmyfile/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 import fitz
 from docx import Document
 from pptx import Presentation
 import argparse
 import pandas as pd
 
 
@@ -96,18 +95,18 @@
     def read(self):
         """Reads the Excel file and converts the data to a string."""
         try:
             data = ''
             df = pd.read_excel(self.path)
             data = df.to_string()
             self.data = data
-        except:
+        except Exception as e:
+            print(f"Failed to read Excel file: {self.path}. Error: {e}")
             self.readable = False
 
-
 class TxtFile(File):
     """
     The TxtFile class represents a text (.txt) file. It inherits from the File class and
     overrides the read() method to read text files.
     """
 
     def read(self):
@@ -224,25 +223,25 @@
         to print the results to the console or return a dictionary of the results."""
         if print_ans:
             counter = 0
             print("Files matching keywords: ", ', '.join(keywords))
             for file in self.files:
                 counter += 1
                 if file.search_all(*keywords):
-                    print(file.name)
+                    #print name up to 30 chars then at 32 char print '|path: ' followed by path
+                    print(f'{file.name[:36]:<36} | path: {file.path}')
             print("\nFiles not readable:")
             for file in self.files:
                 if file.readable == False:
-                    print(file.name)
+                    print(f'{file.name[:36]:<36} | path: {file.path}')
             print('Files searched:', counter, '\n')
         else:
             # returns a dictionary where key is file.name and value is file.data
             return {file.name: file.data for file in self.files if file.search_all(*keywords)}
 
-
 def main():
     # Add your main script here
     db = FilesDB()
     parser = argparse.ArgumentParser(prog="fmf")
     parser.add_argument('-path', '--source_path', type=str, default=os.getcwd(),
                         help="Takes the directory path in quotes as input")
     parser.add_argument('-w', '--words', nargs='*', default=[],
```

### Comparing `findmyfile-0.2.8/findmyfile.egg-info/PKG-INFO` & `findmyfile-0.3.0/findmyfile.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.2.8
+Version: 0.3.0
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENCE.txt
```

### Comparing `findmyfile-0.2.8/setup.py` & `findmyfile-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='findmyfile',         # How you named your package folder (MyLib)
     packages=find_packages(),   # Chose the same as "name"
-    version='0.2.8',      # Start with a small number and increase it with every change you make
+    version='0.3.0',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='This package allows you to search a directory for documents that match keywords',
     author='Sanjin Dedic',                   # Type in your name
     author_email='sanjindedic8@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
@@ -29,15 +29,15 @@
         'python-pptx',
         'pandas',
         'openpyxl',
         'xlrd'
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

