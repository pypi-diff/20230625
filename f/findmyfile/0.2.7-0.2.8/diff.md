# Comparing `tmp/findmyfile-0.2.7.tar.gz` & `tmp/findmyfile-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyfile-0.2.7.tar", last modified: Sat Jun 24 11:26:19 2023, max compression
+gzip compressed data, was "findmyfile-0.2.8.tar", last modified: Sun Jun 25 00:54:26 2023, max compression
```

## Comparing `findmyfile-0.2.7.tar` & `findmyfile-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:26:19.562000 findmyfile-0.2.7/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.2.7/LICENCE.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-24 11:26:19.546000 findmyfile-0.2.7/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     2500 2023-06-24 10:15:12.000000 findmyfile-0.2.7/README.md
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:26:19.183000 findmyfile-0.2.7/findmyfile/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.2.7/findmyfile/__init__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.2.7/findmyfile/__main__.py
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     7966 2023-06-24 11:01:26.000000 findmyfile-0.2.7/findmyfile/main.py
-drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-24 11:26:19.496000 findmyfile-0.2.7/findmyfile.egg-info/
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/PKG-INFO
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/SOURCES.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/dependency_links.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/entry_points.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/requires.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-24 11:26:18.000000 findmyfile-0.2.7/findmyfile.egg-info/top_level.txt
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-24 11:26:19.560000 findmyfile-0.2.7/setup.cfg
--rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1680 2023-06-24 11:26:11.000000 findmyfile-0.2.7/setup.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 00:54:26.845000 findmyfile-0.2.8/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1061 2023-06-24 01:20:32.000000 findmyfile-0.2.8/LICENCE.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-25 00:54:26.823000 findmyfile-0.2.8/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     3085 2023-06-25 00:01:41.000000 findmyfile-0.2.8/README.md
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 00:54:26.356000 findmyfile-0.2.8/findmyfile/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       39 2023-06-24 10:58:56.000000 findmyfile-0.2.8/findmyfile/__init__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       64 2023-06-24 10:59:26.000000 findmyfile-0.2.8/findmyfile/__main__.py
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     9124 2023-06-25 00:31:06.000000 findmyfile-0.2.8/findmyfile/main.py
+drwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        0 2023-06-25 00:54:26.761000 findmyfile-0.2.8/findmyfile.egg-info/
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      688 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/PKG-INFO
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)      301 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)        1 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       45 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/entry_points.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       53 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/requires.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       11 2023-06-25 00:54:25.000000 findmyfile-0.2.8/findmyfile.egg-info/top_level.txt
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)       38 2023-06-25 00:54:26.841000 findmyfile-0.2.8/setup.cfg
+-rwxrwxrwx   0 sanjin    (1000) sanjin    (1000)     1715 2023-06-25 00:53:54.000000 findmyfile-0.2.8/setup.py
```

### Comparing `findmyfile-0.2.7/LICENCE.txt` & `findmyfile-0.2.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `findmyfile-0.2.7/PKG-INFO` & `findmyfile-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
```

### Comparing `findmyfile-0.2.7/findmyfile/main.py` & `findmyfile-0.2.8/findmyfile/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -134,37 +134,51 @@
                 text += page.get_text()
             self.data = text
         except:
             self.readable = False
 
 
 class ProgressBar():
+    """
+    This class represents a progress bar. It is used to display the progress of a search task.
+    A progress bar is created every time a search task is started and it represents the loading
+    of all files into a FilesDB object.
+    """
+
     def __init__(self, total, prefix='', suffix='', decimals=1, length=50, fill='█', print_end="\r"):
         self.total = total
         self.prefix = prefix
         self.suffix = suffix
         self.decimals = decimals
         self.length = length
         self.fill = fill
         self.print_end = print_end
         self.iteration = 0
 
     def print_progress(self, iteration):
+        # detailed docstring
+        """Prints the progress bar to the console using the given iteration."""
         self.iteration = iteration
         percent = ("{0:." + str(self.decimals) + "f}").format(100 *
                                                               (self.iteration / float(self.total)))
         filled_length = int(self.length * self.iteration // self.total)
         bar = self.fill * filled_length + '-' * (self.length - filled_length)
         print(f'\r{self.prefix} |{bar}| {percent}% {self.suffix}',
               end=self.print_end)
         if self.iteration == self.total:
             print()
 
 
 class FilesDB():
+    """
+    The FilesDB class represents a database of files. It has the add_file_data() method which adds all
+    files in a given path to the database. Each file has object has a name, content, extension and path.
+    The search method allows users to search for files in the database by keyword(s).
+    """
+
     def __init__(self, path=os.getcwd()):
         self.path = path
         self.files = []
         self.add_file_data()
 
     def count_files(self):
         """
@@ -201,26 +215,32 @@
                     db_file = readers[ext](
                         os.path.join(root, file), extension=ext)
                     db_file.read()  # reads file data into the object
                     self.files.append(db_file)
                     loaded_files += 1
                     progress.print_progress(loaded_files)
 
-    def search(self, *keywords):
-        counter = 0
-        print("Files matching keywords: ", ', '.join(keywords))
-        for file in self.files:
-            counter += 1
-            if file.search_all(*keywords):
-                print(file.name)
-        print("\nFiles not readable:")
-        for file in self.files:
-            if file.readable == False:
-                print(file.name)
-        print('Files searched:', counter, '\n')
+    def search(self, print_ans=False, *keywords):
+        """Searches for files in the database by keyword(s). Using the print_ans argument, the user can choose
+        to print the results to the console or return a dictionary of the results."""
+        if print_ans:
+            counter = 0
+            print("Files matching keywords: ", ', '.join(keywords))
+            for file in self.files:
+                counter += 1
+                if file.search_all(*keywords):
+                    print(file.name)
+            print("\nFiles not readable:")
+            for file in self.files:
+                if file.readable == False:
+                    print(file.name)
+            print('Files searched:', counter, '\n')
+        else:
+            # returns a dictionary where key is file.name and value is file.data
+            return {file.name: file.data for file in self.files if file.search_all(*keywords)}
 
 
 def main():
     # Add your main script here
     db = FilesDB()
     parser = argparse.ArgumentParser(prog="fmf")
     parser.add_argument('-path', '--source_path', type=str, default=os.getcwd(),
```

### Comparing `findmyfile-0.2.7/findmyfile.egg-info/PKG-INFO` & `findmyfile-0.2.8/findmyfile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyfile
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package allows you to search a directory for documents that match keywords
 Home-page: https://github.com/Sanjin84/findmyfile
 Download-URL: https://github.com/Sanjin84/findmyfile/archive/refs/tags/v_01.tar.gz
 Author: Sanjin Dedic
 Author-email: sanjindedic8@gmail.com
 License: MIT
 Keywords: file search,find file,search directory
```

### Comparing `findmyfile-0.2.7/setup.py` & `findmyfile-0.2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='findmyfile',         # How you named your package folder (MyLib)
     packages=find_packages(),   # Chose the same as "name"
-    version='0.2.7',      # Start with a small number and increase it with every change you make
+    version='0.2.8',      # Start with a small number and increase it with every change you make
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='This package allows you to search a directory for documents that match keywords',
     author='Sanjin Dedic',                   # Type in your name
     author_email='sanjindedic8@gmail.com',      # Type in your E-Mail
     # Provide either the link to your github or to your website
@@ -24,14 +24,16 @@
     },
     install_requires=[
         # Add your dependencies here
         'PyMuPDF',
         'python-docx',
         'python-pptx',
         'pandas',
+        'openpyxl',
+        'xlrd'
     ],
     classifiers=[
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

